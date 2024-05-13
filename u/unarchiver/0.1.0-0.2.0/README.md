# Comparing `tmp/unarchiver-0.1.0.tar.gz` & `tmp/unarchiver-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unarchiver-0.1.0.tar", max compression
+gzip compressed data, was "unarchiver-0.2.0.tar", max compression
```

## Comparing `unarchiver-0.1.0.tar` & `unarchiver-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      931 2024-05-12 16:15:59.637468 unarchiver-0.1.0/README.md
--rw-r--r--   0        0        0      535 2024-05-12 16:15:59.637468 unarchiver-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-12 16:15:59.637468 unarchiver-0.1.0/unarchiver/__init__.py
--rw-r--r--   0        0        0     4130 2024-05-12 16:15:59.637468 unarchiver-0.1.0/unarchiver/unarchiver.py
--rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 unarchiver-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      931 2024-05-13 16:54:17.945176 unarchiver-0.2.0/README.md
+-rw-r--r--   0        0        0      535 2024-05-13 16:54:17.945176 unarchiver-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-13 16:54:17.945176 unarchiver-0.2.0/unarchiver/__init__.py
+-rw-r--r--   0        0        0     4238 2024-05-13 16:54:17.945176 unarchiver-0.2.0/unarchiver/unarchiver.py
+-rw-r--r--   0        0        0     1557 1970-01-01 00:00:00.000000 unarchiver-0.2.0/PKG-INFO
```

### Comparing `unarchiver-0.1.0/README.md` & `unarchiver-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `unarchiver-0.1.0/pyproject.toml` & `unarchiver-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unarchiver"
-version = "0.1.0"
+version = "0.2.0"
 description = "Unarchive an NSKeyedArchive into a python object."
 authors = ["PandasAreBears <emailadresspanda@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 bpylist2 = "^4.1.1"
```

### Comparing `unarchiver-0.1.0/unarchiver/unarchiver.py` & `unarchiver-0.2.0/unarchiver/unarchiver.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,14 +105,16 @@
                 continue
 
             match type(value):
                 case plistlib.UID:
                     obj[key] = self._value_for_uid(value)
                 case builtins.list:
                     obj[key] = [self._value_for_uid(v) for v in value]
+                case builtins.bytes:
+                    obj[key] = base64.b64encode(value).decode("utf-8")
                 case _:
                     obj[key] = value
 
         return obj
 
 
 @click.command()
```

### Comparing `unarchiver-0.1.0/PKG-INFO` & `unarchiver-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unarchiver
-Version: 0.1.0
+Version: 0.2.0
 Summary: Unarchive an NSKeyedArchive into a python object.
 Author: PandasAreBears
 Author-email: emailadresspanda@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

