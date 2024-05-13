# Comparing `tmp/pydbtools-5.5.8.tar.gz` & `tmp/pydbtools-5.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydbtools-5.5.8.tar", max compression
+gzip compressed data, was "pydbtools-5.5.9.tar", max compression
```

## Comparing `pydbtools-5.5.8.tar` & `pydbtools-5.5.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       48 2023-08-01 10:40:48.026857 pydbtools-5.5.8/docs/README.md
--rw-r--r--   0        0        0      855 2023-08-01 10:40:48.030857 pydbtools-5.5.8/pydbtools/__init__.py
--rw-r--r--   0        0        0     1130 2023-08-01 10:40:48.030857 pydbtools-5.5.8/pydbtools/_sql_render.py
--rw-r--r--   0        0        0    23104 2023-08-01 10:40:48.034857 pydbtools-5.5.8/pydbtools/_wrangler.py
--rw-r--r--   0        0        0     6391 2023-08-01 10:40:48.034857 pydbtools-5.5.8/pydbtools/utils.py
--rw-r--r--   0        0        0      857 2023-08-01 10:40:48.034857 pydbtools-5.5.8/pyproject.toml
--rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 pydbtools-5.5.8/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-10-03 09:31:38.818487 pydbtools-5.5.9/docs/README.md
+-rw-r--r--   0        0        0      855 2023-10-03 09:31:38.822486 pydbtools-5.5.9/pydbtools/__init__.py
+-rw-r--r--   0        0        0     1130 2023-10-03 09:31:38.822486 pydbtools-5.5.9/pydbtools/_sql_render.py
+-rw-r--r--   0        0        0    23104 2023-10-03 09:31:38.822486 pydbtools-5.5.9/pydbtools/_wrangler.py
+-rw-r--r--   0        0        0     6812 2023-10-03 09:31:38.822486 pydbtools-5.5.9/pydbtools/utils.py
+-rw-r--r--   0        0        0      857 2023-10-03 09:31:38.822486 pydbtools-5.5.9/pyproject.toml
+-rw-r--r--   0        0        0      941 1970-01-01 00:00:00.000000 pydbtools-5.5.9/PKG-INFO
```

### Comparing `pydbtools-5.5.8/pydbtools/__init__.py` & `pydbtools-5.5.9/pydbtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,8 +29,8 @@
     create_table,
 )
 
 from ._sql_render import get_sql_from_file, render_sql_template  # noqa: F401
 
 from .utils import s3_path_join  # noqa: F401
 
-__version__ = "5.5.8"
+__version__ = "5.5.9"
```

### Comparing `pydbtools-5.5.8/pydbtools/_sql_render.py` & `pydbtools-5.5.9/pydbtools/_sql_render.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.8/pydbtools/_wrangler.py` & `pydbtools-5.5.9/pydbtools/_wrangler.py`

 * *Files identical despite different names*

### Comparing `pydbtools-5.5.8/pydbtools/utils.py` & `pydbtools-5.5.9/pydbtools/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -137,15 +137,14 @@
     # treat a trailing newline differently
     return "".join(new_query).strip()
 
 
 def get_user_id_and_table_dir(
     boto3_session=None, force_ec2: bool = False, region_name: str = None
 ) -> Tuple[str, str]:
-
     region_name = _set_region_name(region_name)
 
     if boto3_session is None:
         boto3_session = get_boto_session(force_ec2=force_ec2, region_name=region_name)
 
     sts_client = boto3_session.client("sts")
     sts_resp = sts_client.get_caller_identity()
@@ -153,15 +152,30 @@
     if out_path[-1] != "/":
         out_path += "/"
 
     return (sts_resp["UserId"], out_path)
 
 
 def get_database_name_from_userid(user_id: str) -> str:
-    unique_db_name = user_id.split(":")[-1].split("-", 1)[-1].replace("-", "_")
+    """
+    Obtain unique database name for temporary database
+    from various forms of user id
+    """
+    unique_db_name = (
+        # Remove chunk before last ":"
+        user_id.split(":")[-1]
+        # Remove chunk after first "@"
+        .split("@")[0]
+        # Replace remaining dashes with underscores
+        .replace("-", "_")
+    )
+    # Only use permitted characters for AWS Athena databases
+    unique_db_name = "".join(
+        c for c in unique_db_name if c.isalnum() or c == "_"
+    )
     unique_db_name = temp_database_name_prefix + unique_db_name
     return unique_db_name
 
 
 def get_database_name_from_sql(sql: str) -> str:
     """
     Obtains database name from SQL query for use
@@ -210,15 +224,14 @@
 
 def get_boto_client(
     client_name: str,
     boto3_session=None,
     force_ec2: bool = False,
     region_name: str = None,
 ):
-
     region_name = _set_region_name(region_name)
 
     if boto3_session is None:
         boto3_session = get_boto_session(force_ec2=force_ec2, region_name=region_name)
 
     return boto3_session.client(client_name)
```

### Comparing `pydbtools-5.5.8/pyproject.toml` & `pydbtools-5.5.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "pydbtools"
-version = "5.5.8"
+version = "5.5.9"
 description = "A python package to query data via amazon athena and bring it into a pandas df using aws-wrangler."
 license = "MIT"
 authors = ["Karik Isichei <karik.isichei@digital.justice.gov.uk>"]
 readme = "docs/README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
```

### Comparing `pydbtools-5.5.8/PKG-INFO` & `pydbtools-5.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydbtools
-Version: 5.5.8
+Version: 5.5.9
 Summary: A python package to query data via amazon athena and bring it into a pandas df using aws-wrangler.
 License: MIT
 Author: Karik Isichei
 Author-email: karik.isichei@digital.justice.gov.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

