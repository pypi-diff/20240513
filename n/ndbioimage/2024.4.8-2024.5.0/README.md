# Comparing `tmp/ndbioimage-2024.4.8.tar.gz` & `tmp/ndbioimage-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ndbioimage-2024.4.8.tar", max compression
+gzip compressed data, was "ndbioimage-2024.5.0.tar", max compression
```

## Comparing `ndbioimage-2024.4.8.tar` & `ndbioimage-2024.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.4.8/LICENSE
--rw-r--r--   0        0        0     2603 2024-04-12 15:46:18.729984 ndbioimage-2024.4.8/README.md
--rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.4.8/ndbioimage/.DS_Store
--rwxr-xr-x   0        0        0    54330 2024-04-19 14:08:16.717040 ndbioimage-2024.4.8/ndbioimage/__init__.py
--rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.4.8/ndbioimage/jvm.py
--rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.4.8/ndbioimage/readers/__init__.py
--rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.4.8/ndbioimage/readers/bfread.py
--rw-r--r--   0        0        0    28254 2024-04-29 11:09:41.232812 ndbioimage-2024.4.8/ndbioimage/readers/cziread.py
--rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.4.8/ndbioimage/readers/fijiread.py
--rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.4.8/ndbioimage/readers/ndread.py
--rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.4.8/ndbioimage/readers/seqread.py
--rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.4.8/ndbioimage/readers/tifread.py
--rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.4.8/ndbioimage/transform.txt
--rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.4.8/ndbioimage/transforms.py
--rw-r--r--   0        0        0     1248 2024-04-29 11:13:48.376671 ndbioimage-2024.4.8/pyproject.toml
--rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 ndbioimage-2024.4.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-07-15 11:39:50.144787 ndbioimage-2024.5.0/LICENSE
+-rw-r--r--   0        0        0     2603 2024-04-12 15:46:18.729984 ndbioimage-2024.5.0/README.md
+-rw-r--r--   0        0        0     6148 2023-05-26 07:15:21.785168 ndbioimage-2024.5.0/ndbioimage/.DS_Store
+-rwxr-xr-x   0        0        0    54670 2024-05-13 09:41:04.263451 ndbioimage-2024.5.0/ndbioimage/__init__.py
+-rw-r--r--   0        0        0     2649 2023-11-20 13:41:19.468310 ndbioimage-2024.5.0/ndbioimage/jvm.py
+-rw-r--r--   0        0        0       74 2023-12-07 12:44:53.056179 ndbioimage-2024.5.0/ndbioimage/readers/__init__.py
+-rw-r--r--   0        0        0     8368 2024-03-18 13:18:17.532784 ndbioimage-2024.5.0/ndbioimage/readers/bfread.py
+-rw-r--r--   0        0        0    28254 2024-04-29 11:09:41.232812 ndbioimage-2024.5.0/ndbioimage/readers/cziread.py
+-rw-r--r--   0        0        0     2541 2024-03-29 16:56:03.448728 ndbioimage-2024.5.0/ndbioimage/readers/fijiread.py
+-rw-r--r--   0        0        0     2021 2024-03-29 16:56:03.484728 ndbioimage-2024.5.0/ndbioimage/readers/ndread.py
+-rw-r--r--   0        0        0     6405 2024-04-12 14:01:22.758103 ndbioimage-2024.5.0/ndbioimage/readers/seqread.py
+-rw-r--r--   0        0        0     3117 2024-03-29 17:10:12.880871 ndbioimage-2024.5.0/ndbioimage/readers/tifread.py
+-rw-r--r--   0        0        0      187 2022-07-15 08:02:04.684297 ndbioimage-2024.5.0/ndbioimage/transform.txt
+-rw-r--r--   0        0        0    17371 2024-04-02 16:22:30.184194 ndbioimage-2024.5.0/ndbioimage/transforms.py
+-rw-r--r--   0        0        0     1248 2024-05-13 09:41:04.375452 ndbioimage-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 ndbioimage-2024.5.0/PKG-INFO
```

### Comparing `ndbioimage-2024.4.8/LICENSE` & `ndbioimage-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/README.md` & `ndbioimage-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/ndbioimage/.DS_Store` & `ndbioimage-2024.5.0/ndbioimage/.DS_Store`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/ndbioimage/__init__.py` & `ndbioimage-2024.5.0/ndbioimage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,22 +148,31 @@
 
     def __init__(self) -> None:
         super().__init__(64)
 
     def __reduce__(self) -> tuple[type, tuple]:
         return self.__class__, ()
 
-    def __getitem__(self, path: Path) -> OME:
-        return super().__getitem__(self.path_and_lstat(path))
-
-    def __setitem__(self, path: Path, value: OME) -> None:
-        super().__setitem__(self.path_and_lstat(path), value)
-
-    def __contains__(self, path: Path) -> bool:
-        return super().__contains__(self.path_and_lstat(path))
+    def __getitem__(self, path: Path | str | tuple) -> OME:
+        if isinstance(path, tuple):
+            return super().__getitem__(path)
+        else:
+            return super().__getitem__(self.path_and_lstat(path))
+
+    def __setitem__(self, path: Path | str | tuple, value: OME) -> None:
+        if isinstance(path, tuple):
+            super().__setitem__(path, value)
+        else:
+            super().__setitem__(self.path_and_lstat(path), value)
+
+    def __contains__(self, path: Path | str | tuple) -> bool:
+        if isinstance(path, tuple):
+            return super().__contains__(path)
+        else:
+            return super().__contains__(self.path_and_lstat(path))
 
     @staticmethod
     def path_and_lstat(path: str | Path) -> tuple[Path, Optional[os.stat_result], Optional[os.stat_result]]:
         path = Path(path)
         return (path, (path.lstat() if path.exists() else None),
                 (path.with_suffix('.ome.xml').lstat() if path.with_suffix('.ome.xml').exists() else None))
```

### Comparing `ndbioimage-2024.4.8/ndbioimage/jvm.py` & `ndbioimage-2024.5.0/ndbioimage/jvm.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/ndbioimage/readers/bfread.py` & `ndbioimage-2024.5.0/ndbioimage/readers/bfread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/ndbioimage/readers/cziread.py` & `ndbioimage-2024.5.0/ndbioimage/readers/cziread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/ndbioimage/readers/fijiread.py` & `ndbioimage-2024.5.0/ndbioimage/readers/fijiread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/ndbioimage/readers/ndread.py` & `ndbioimage-2024.5.0/ndbioimage/readers/ndread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/ndbioimage/readers/seqread.py` & `ndbioimage-2024.5.0/ndbioimage/readers/seqread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/ndbioimage/readers/tifread.py` & `ndbioimage-2024.5.0/ndbioimage/readers/tifread.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/ndbioimage/transforms.py` & `ndbioimage-2024.5.0/ndbioimage/transforms.py`

 * *Files identical despite different names*

### Comparing `ndbioimage-2024.4.8/pyproject.toml` & `ndbioimage-2024.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ndbioimage"
-version = "2024.4.8"
+version = "2024.5.0"
 description = "Bio image reading, metadata and some affine registration."
 authors = ["W. Pomp <w.pomp@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["bioformats", "imread", "numpy", "metadata"]
 include = ["transform.txt"]
 repository = "https://github.com/wimpomp/ndbioimage"
```

### Comparing `ndbioimage-2024.4.8/PKG-INFO` & `ndbioimage-2024.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ndbioimage
-Version: 2024.4.8
+Version: 2024.5.0
 Summary: Bio image reading, metadata and some affine registration.
 Home-page: https://github.com/wimpomp/ndbioimage
 License: GPLv3
 Keywords: bioformats,imread,numpy,metadata
 Author: W. Pomp
 Author-email: w.pomp@nki.nl
 Requires-Python: >=3.10,<4.0
```

