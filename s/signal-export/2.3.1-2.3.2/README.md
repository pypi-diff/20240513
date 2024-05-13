# Comparing `tmp/signal_export-2.3.1.tar.gz` & `tmp/signal_export-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signal_export-2.3.1.tar", last modified: Wed May  1 07:52:25 2024, max compression
+gzip compressed data, was "signal_export-2.3.2.tar", last modified: Mon May 13 15:18:21 2024, max compression
```

## Comparing `signal_export-2.3.1.tar` & `signal_export-2.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1170 2024-05-01 07:52:22.194915 signal_export-2.3.1/LICENSE
--rw-r--r--   0        0        0     6921 2024-05-01 07:52:22.194915 signal_export-2.3.1/README.md
--rw-r--r--   0        0        0     2006 2024-05-01 07:52:25.314926 signal_export-2.3.1/pyproject.toml
--rw-r--r--   0        0        0        1 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/__init__.py
--rw-r--r--   0        0        0       69 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/__main__.py
--rw-r--r--   0        0        0     3173 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/create.py
--rw-r--r--   0        0        0     2956 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/data.py
--rw-r--r--   0        0        0     3209 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/files.py
--rw-r--r--   0        0        0     3451 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/html.py
--rw-r--r--   0        0        0      144 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/logging.py
--rwxr-xr-x   0        0        0     8356 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/main.py
--rw-r--r--   0        0        0     2722 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/merge.py
--rw-r--r--   0        0        0     4310 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/models.py
--rw-r--r--   0        0        0     1846 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/style.css
--rw-r--r--   0        0        0     1271 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/templates.py
--rw-r--r--   0        0        0     2467 2024-05-01 07:52:22.194915 signal_export-2.3.1/sigexport/utils.py
--rw-r--r--   0        0        0     2546 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/data/attachments.noindex/image.jpeg
--rw-r--r--   0        0        0    17641 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/data/attachments.noindex/voicenote.m4a
--rw-r--r--   0        0        0       22 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/data/config.json
--rw-r--r--   0        0        0    16384 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/data/sql/db.sqlite
--rw-r--r--   0        0        0     5125 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/test_integration.py
--rw-r--r--   0        0        0       86 2024-05-01 07:52:22.194915 signal_export-2.3.1/tests/test_utils.py
--rw-r--r--   0        0        0     7846 1970-01-01 00:00:00.000000 signal_export-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1170 2024-05-13 15:18:17.715710 signal_export-2.3.2/LICENSE
+-rw-r--r--   0        0        0     6921 2024-05-13 15:18:17.715710 signal_export-2.3.2/README.md
+-rw-r--r--   0        0        0     2006 2024-05-13 15:18:21.031731 signal_export-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/__init__.py
+-rw-r--r--   0        0        0       69 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/__main__.py
+-rw-r--r--   0        0        0     3173 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/create.py
+-rw-r--r--   0        0        0     3017 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/data.py
+-rw-r--r--   0        0        0     3209 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/files.py
+-rw-r--r--   0        0        0     3451 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/html.py
+-rw-r--r--   0        0        0      144 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/logging.py
+-rwxr-xr-x   0        0        0     8356 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/main.py
+-rw-r--r--   0        0        0     2722 2024-05-13 15:18:17.715710 signal_export-2.3.2/sigexport/merge.py
+-rw-r--r--   0        0        0     4548 2024-05-13 15:18:17.719710 signal_export-2.3.2/sigexport/models.py
+-rw-r--r--   0        0        0     1846 2024-05-13 15:18:17.719710 signal_export-2.3.2/sigexport/style.css
+-rw-r--r--   0        0        0     1271 2024-05-13 15:18:17.719710 signal_export-2.3.2/sigexport/templates.py
+-rw-r--r--   0        0        0     2467 2024-05-13 15:18:17.719710 signal_export-2.3.2/sigexport/utils.py
+-rw-r--r--   0        0        0     2546 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/data/attachments.noindex/image.jpeg
+-rw-r--r--   0        0        0    17641 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/data/attachments.noindex/voicenote.m4a
+-rw-r--r--   0        0        0       22 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/data/config.json
+-rw-r--r--   0        0        0    16384 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/data/sql/db.sqlite
+-rw-r--r--   0        0        0     5125 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/test_integration.py
+-rw-r--r--   0        0        0       86 2024-05-13 15:18:17.719710 signal_export-2.3.2/tests/test_utils.py
+-rw-r--r--   0        0        0     7846 1970-01-01 00:00:00.000000 signal_export-2.3.2/PKG-INFO
```

### Comparing `signal_export-2.3.1/LICENSE` & `signal_export-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/README.md` & `signal_export-2.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 
 ### macOS without Docker
 1. Install [Homebrew](https://brew.sh).
 2. Run `brew install openssl sqlcipher`
 3. Export some needed env vars:
 ```bash
 export C_INCLUDE_PATH="$(brew --prefix sqlcipher)/include"
-export LIBRARY_PATH="${brew --prefix sqlcipher)/lib"
+export LIBRARY_PATH="$(brew --prefix sqlcipher)/lib"
 ```
 
 4. Then you can install and run signal-export without Docker:
 ```bash
 pip install 'signal-export[sql]'
 sigexport --no-use-docker ...
 ```
```

### Comparing `signal_export-2.3.1/pyproject.toml` & `signal_export-2.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 ]
 dependencies = [
     "beautifulsoup4 ~= 4.11",
     "emoji ~= 2.0",
     "Markdown ~= 3.4",
     "typer[all] ~= 0.7",
 ]
-version = "2.3.1"
+version = "2.3.2"
 
 [project.license]
 text = "MIT License"
 
 [project.optional-dependencies]
 sql = [
     "pysqlcipher3 == 1.1.0; python_version <  \"3.11\"",
```

### Comparing `signal_export-2.3.1/sigexport/create.py` & `signal_export-2.3.2/sigexport/create.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/sigexport/data.py` & `signal_export-2.3.2/sigexport/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
                 id=res["id"],
                 type=res.get("type"),
                 body=res.get("body", ""),
                 contact=res.get("contact"),
                 source=res.get("source"),
                 timestamp=res.get("timestamp"),
                 sent_at=res.get("sent_at"),
+                server_timestamp=res.get("serverTimestamp"),
                 has_attachments=res.get("has_attachments", False),
                 attachments=res.get("attachments", []),
                 read_status=res.get("read_status"),
                 seen_status=res.get("seen_status"),
                 call_history=res.get("call_history"),
                 reactions=res.get("reactions", []),
                 sticker=res.get("sticker"),
```

### Comparing `signal_export-2.3.1/sigexport/files.py` & `signal_export-2.3.2/sigexport/files.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/sigexport/html.py` & `signal_export-2.3.2/sigexport/html.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/sigexport/main.py` & `signal_export-2.3.2/sigexport/main.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/sigexport/merge.py` & `signal_export-2.3.2/sigexport/merge.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/sigexport/models.py` & `signal_export-2.3.2/sigexport/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,28 +16,34 @@
     body: str
     type: str | None
     contact: str | None
     source: Any | None
 
     timestamp: int | None
     sent_at: int | None
+    server_timestamp: int | None
 
     has_attachments: bool
     attachments: list[dict[str, str]]
 
     read_status: bool | None
     seen_status: bool | None
 
     call_history: dict[str, Any] | None
     reactions: list[dict[str, Any]]
     sticker: dict[str, Any] | None
     quote: dict[str, Any] | None
 
     def get_ts(self: RawMessage) -> int:
-        if self.sent_at:
+        if self.sent_at and self.server_timestamp:
+            if self.server_timestamp < self.sent_at:
+                return self.server_timestamp
+            else:
+                return self.sent_at
+        elif self.sent_at:
             return self.sent_at
         elif self.timestamp:
             return self.timestamp
         return 0
 
 
 @dataclass
```

### Comparing `signal_export-2.3.1/sigexport/style.css` & `signal_export-2.3.2/sigexport/style.css`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/sigexport/templates.py` & `signal_export-2.3.2/sigexport/templates.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/sigexport/utils.py` & `signal_export-2.3.2/sigexport/utils.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/tests/data/attachments.noindex/image.jpeg` & `signal_export-2.3.2/tests/data/attachments.noindex/image.jpeg`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/tests/data/attachments.noindex/voicenote.m4a` & `signal_export-2.3.2/tests/data/attachments.noindex/voicenote.m4a`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/tests/data/sql/db.sqlite` & `signal_export-2.3.2/tests/data/sql/db.sqlite`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/tests/test_integration.py` & `signal_export-2.3.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `signal_export-2.3.1/PKG-INFO` & `signal_export-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: signal-export
-Version: 2.3.1
+Version: 2.3.2
 Summary: Export Signal conversations to Markdown and HTML
 Keywords: backup,chat,export
 Home-page: https://github.com/carderne/signal-export
 Author-Email: Chris Arderne <chris@rdrn.me>
 License: MIT License
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -112,15 +112,15 @@
 
 ### macOS without Docker
 1. Install [Homebrew](https://brew.sh).
 2. Run `brew install openssl sqlcipher`
 3. Export some needed env vars:
 ```bash
 export C_INCLUDE_PATH="$(brew --prefix sqlcipher)/include"
-export LIBRARY_PATH="${brew --prefix sqlcipher)/lib"
+export LIBRARY_PATH="$(brew --prefix sqlcipher)/lib"
 ```
 
 4. Then you can install and run signal-export without Docker:
 ```bash
 pip install 'signal-export[sql]'
 sigexport --no-use-docker ...
 ```
```

