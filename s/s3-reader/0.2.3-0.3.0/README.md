# Comparing `tmp/s3_reader-0.2.3.tar.gz` & `tmp/s3_reader-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3_reader-0.2.3.tar", max compression
+gzip compressed data, was "s3_reader-0.3.0.tar", max compression
```

## Comparing `s3_reader-0.2.3.tar` & `s3_reader-0.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11337 2023-09-23 03:40:43.847301 s3_reader-0.2.3/LICENSE
--rw-r--r--   0        0        0     1073 2023-12-26 08:59:47.832085 s3_reader-0.2.3/README.md
--rw-r--r--   0        0        0     2010 2024-01-09 10:58:50.099946 s3_reader-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       95 2023-09-23 03:40:43.848692 s3_reader-0.2.3/src/s3_reader/__init__.py
--rw-r--r--   0        0        0       93 2023-09-23 03:40:43.848794 s3_reader-0.2.3/src/s3_reader/__version__.py
--rw-r--r--   0        0        0     3649 2023-12-26 08:58:16.204780 s3_reader-0.2.3/src/s3_reader/file.py
--rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 s3_reader-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-09-23 03:40:43.847301 s3_reader-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1073 2023-12-26 08:59:47.832085 s3_reader-0.3.0/README.md
+-rw-r--r--   0        0        0     2010 2024-05-13 03:31:08.361112 s3_reader-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       95 2023-09-23 03:40:43.848692 s3_reader-0.3.0/src/s3_reader/__init__.py
+-rw-r--r--   0        0        0       93 2023-09-23 03:40:43.848794 s3_reader-0.3.0/src/s3_reader/__version__.py
+-rw-r--r--   0        0        0     4357 2024-05-13 03:31:08.356728 s3_reader-0.3.0/src/s3_reader/file.py
+-rw-r--r--   0        0        0     1785 1970-01-01 00:00:00.000000 s3_reader-0.3.0/PKG-INFO
```

### Comparing `s3_reader-0.2.3/LICENSE` & `s3_reader-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `s3_reader-0.2.3/README.md` & `s3_reader-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `s3_reader-0.2.3/pyproject.toml` & `s3_reader-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "s3-reader"
-version = "0.2.3"
+version = "0.3.0"
 description = "Python library to read S3 file as local file."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/s3-reader"
 homepage = "https://github.com/rcmdnk/s3-reader"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = []
@@ -12,20 +12,20 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 boto3-session = "^0.0.6"
 
 [tool.poetry.group.dev.dependencies]
 tomli = { version = "^2.0.1", python = "<3.11"}
-pytest = "^7.4.2"
-pytest-cov = "^4.1.0"
+pytest = "^8.0.0"
+pytest-cov = "^5.0.0"
 pytest-xdist = "^3.3.1"
 pytest-benchmark = "^4.0.0"
 pyproject-pre-commit = "^0.1.0"
-gitpython = "^3.1.37"
+gitpython = "^3.1.43"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "-n auto"
```

### Comparing `s3_reader-0.2.3/src/s3_reader/file.py` & `s3_reader-0.3.0/src/s3_reader/file.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,19 @@
 @dataclass
 class File:
     """A class to manage S3 file as a local file.
 
     Parameters
     ----------
     path : str | Path
-        The path of the file. A local path or path to the S3 (s3://...) can be used.
+        The path of the file. A local path, path to the S3 (s3://...), or URL
+        (http(s)://...) can be used.
+    file_name : str | None
+        The name of the file. If None, the name of the file is extracted from
+        the path.
     profile_name : str | None
         AWS profile name.
     aws_access_key_id : str | None
         AWS access key id.
     aws_secret_access_key : str | None
         AWS secret access key.
     aws_session_token : str | None
@@ -31,79 +35,97 @@
     retry_mode : str
         Retry mode for failed requests. Default is "standard".
     max_attempts : int
         Maximum number of retry attempts for failed requests. Default is 10.
     """
 
     path: str | Path
+    file_name: str | None = None
     profile_name: str | None = None
     aws_access_key_id: str | None = None
     aws_secret_access_key: str | None = None
     aws_session_token: str | None = None
     region_name: str | None = None
     role_arn: str | None = None
-    session_name: str = "boto3_session"
+    session_name: str = "s3_reader"
     retry_mode: str = "standard"
     max_attempts: int = 10
 
     def __post_init__(self) -> None:
-        self.orig_path = self.path
         self.path = self.fix_path(self.path)
-        self.tmp_file: tempfile._TemporaryFileWrapper[bytes] | None = None
-        if self.path.startswith("s3:"):
-            self.path = self.download_s3_file()
+        self.orig_path = self.path
+        self.load()
 
     def __del__(self) -> None:
-        if self.tmp_file is not None:
-            self.tmp_file.close()
+        self.cleanup()
+
+    def load(self) -> None:
+        if self.file_name is None:
+            self.file_name = Path(self.path).name
+        self.temp_dir: tempfile.TemporaryDirectory | None = None
+        if self.path.startswith("s3:"):
+            self.download_s3_file()
+        elif self.path.startswith("http:") or self.path.startswith("https:"):
+            self.download_http_file()
+
+    def cleanup(self) -> None:
+        if self.temp_dir is not None:
+            self.temp_dir.cleanup()
+            self.temp_dir = None
 
     @staticmethod
     def fix_path(path: str | Path) -> str:
         if not path:
             return ""
         # remove double slash during the path (other than starting of s3://)
         if ":/" in str(path):
             pathes = str(path).split(":/")
             return f"{pathes[0]}:/{Path(pathes[1])}"
         return str(Path(path))
 
     @staticmethod
-    def extract_s3_info(path: str | Path) -> tuple[str, str, str]:
+    def extract_s3_info(path: str | Path) -> tuple[str, str]:
         path = str(path)
         split_path = path.split("/")
         bucket_name = split_path[2]
-        file_name = "/".join(split_path[3:])
-        file_extension = split_path[-1].split(".")[-1]
-        return bucket_name, file_name, file_extension
+        key = "/".join(split_path[3:])
+        return bucket_name, key
 
     def download_s3_file(self) -> str:
         # boto3.session.Session(profile_name=self.s3_profile).resource("s3") uses random.
         # To avoid unnoticed change of random state, restore random state after the process.
         import random
 
         from boto3_session import Session
 
         state = random.getstate()
 
-        bucket_name, file_name, file_extension = self.extract_s3_info(
-            self.path
+        bucket_name, key = self.extract_s3_info(
+            self.orig_path
         )
-        temp_file = tempfile.NamedTemporaryFile(suffix=f".{file_extension}")
+        self.temp_dir = tempfile.TemporaryDirectory()
+        self.path = f"{self.temp_dir.name}/{self.file_name}"
 
         s3 = Session(
             profile_name=self.profile_name,
             aws_access_key_id=self.aws_access_key_id,
             aws_secret_access_key=self.aws_secret_access_key,
             aws_session_token=self.aws_session_token,
             region_name=self.region_name,
             role_arn=self.role_arn,
             session_name=self.session_name,
             retry_mode=self.retry_mode,
             max_attempts=self.max_attempts,
         ).resource("s3")
         bucket = s3.Bucket(bucket_name)
-        bucket.download_file(file_name, temp_file.name)
-        self.tmp_file = temp_file
+        bucket.download_file(key, self.path)
 
         random.setstate(state)
 
-        return temp_file.name
+    def download_http_file(self) -> str:
+        import urllib
+        self.temp_dir = tempfile.TemporaryDirectory()
+        self.path = f"{self.temp_dir.name}/{self.file_name}"
+
+        with urllib.request.urlopen(self.orig_path) as input_file:
+            with open(self.path, 'wb') as dest_file:
+                dest_file.write(input_file.read())
```

### Comparing `s3_reader-0.2.3/PKG-INFO` & `s3_reader-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: s3-reader
-Version: 0.2.3
+Version: 0.3.0
 Summary: Python library to read S3 file as local file.
 Home-page: https://github.com/rcmdnk/s3-reader
 License: Apache-2.0
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

