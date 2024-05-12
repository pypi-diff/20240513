# Comparing `tmp/pyboiler_anonoei-0.0.3.tar.gz` & `tmp/pyboiler_anonoei-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyboiler_anonoei-0.0.3.tar", last modified: Sun May 12 13:38:03 2024, max compression
+gzip compressed data, was "pyboiler_anonoei-0.0.4.tar", last modified: Sun May 12 18:36:38 2024, max compression
```

## Comparing `pyboiler_anonoei-0.0.3.tar` & `pyboiler_anonoei-0.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 13:38:03.693779 pyboiler_anonoei-0.0.3/
--rw-r--r--   0 anonoei    (501) staff       (20)     1051 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/LICENSE
--rw-r--r--   0 anonoei    (501) staff       (20)     1173 2024-05-12 13:38:03.693415 pyboiler_anonoei-0.0.3/PKG-INFO
--rw-r--r--   0 anonoei    (501) staff       (20)      173 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/README.md
--rw-r--r--   0 anonoei    (501) staff       (20)     1405 2024-05-12 13:37:45.000000 pyboiler_anonoei-0.0.3/pyproject.toml
--rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-12 13:38:03.693838 pyboiler_anonoei-0.0.3/setup.cfg
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 13:38:03.685831 pyboiler_anonoei-0.0.3/src/
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 13:38:03.689435 pyboiler_anonoei-0.0.3/src/pyboiler/
--rw-r--r--   0 anonoei    (501) staff       (20)      730 2024-05-12 13:37:45.000000 pyboiler_anonoei-0.0.3/src/pyboiler/__init__.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 13:38:03.691377 pyboiler_anonoei-0.0.3/src/pyboiler/_log/
--rw-r--r--   0 anonoei    (501) staff       (20)      220 2024-05-12 12:42:29.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/__init__.py
--rw-r--r--   0 anonoei    (501) staff       (20)      129 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/filter.py
--rw-r--r--   0 anonoei    (501) staff       (20)      421 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/format.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1778 2024-05-12 12:42:43.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/handler.py
--rw-r--r--   0 anonoei    (501) staff       (20)      878 2024-05-12 12:03:41.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/level.py
--rw-r--r--   0 anonoei    (501) staff       (20)       77 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/src/pyboiler/_log/record.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2313 2024-05-12 10:43:02.000000 pyboiler_anonoei-0.0.3/src/pyboiler/config.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2591 2024-05-12 13:29:14.000000 pyboiler_anonoei-0.0.3/src/pyboiler/generic.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2908 2024-05-12 10:51:41.000000 pyboiler_anonoei-0.0.3/src/pyboiler/hml.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1103 2024-05-12 10:24:59.000000 pyboiler_anonoei-0.0.3/src/pyboiler/hson.py
--rw-r--r--   0 anonoei    (501) staff       (20)     2137 2024-05-12 11:06:15.000000 pyboiler_anonoei-0.0.3/src/pyboiler/imports.py
--rw-r--r--   0 anonoei    (501) staff       (20)     3391 2024-05-12 13:26:39.000000 pyboiler_anonoei-0.0.3/src/pyboiler/logger.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1583 2024-05-12 13:26:11.000000 pyboiler_anonoei-0.0.3/src/pyboiler/logging.py
--rw-r--r--   0 anonoei    (501) staff       (20)      571 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/src/pyboiler/platform.py
--rw-r--r--   0 anonoei    (501) staff       (20)      594 2024-05-12 10:40:35.000000 pyboiler_anonoei-0.0.3/src/pyboiler/profiler.py
--rw-r--r--   0 anonoei    (501) staff       (20)     3531 2024-05-12 13:29:41.000000 pyboiler_anonoei-0.0.3/src/pyboiler/settings.py
--rw-r--r--   0 anonoei    (501) staff       (20)     1893 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.3/src/pyboiler/version.py
-drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 13:38:03.692707 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/
--rw-r--r--   0 anonoei    (501) staff       (20)     1173 2024-05-12 13:38:03.000000 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/PKG-INFO
--rw-r--r--   0 anonoei    (501) staff       (20)      704 2024-05-12 13:38:03.000000 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/SOURCES.txt
--rw-r--r--   0 anonoei    (501) staff       (20)        1 2024-05-12 13:38:03.000000 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/dependency_links.txt
--rw-r--r--   0 anonoei    (501) staff       (20)       34 2024-05-12 13:38:03.000000 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/requires.txt
--rw-r--r--   0 anonoei    (501) staff       (20)        9 2024-05-12 13:38:03.000000 pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/top_level.txt
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 18:36:38.022911 pyboiler_anonoei-0.0.4/
+-rw-r--r--   0 anonoei    (501) staff       (20)     1051 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.4/LICENSE
+-rw-r--r--   0 anonoei    (501) staff       (20)     1281 2024-05-12 18:36:38.022541 pyboiler_anonoei-0.0.4/PKG-INFO
+-rw-r--r--   0 anonoei    (501) staff       (20)      281 2024-05-12 13:44:40.000000 pyboiler_anonoei-0.0.4/README.md
+-rw-r--r--   0 anonoei    (501) staff       (20)     1405 2024-05-12 18:36:29.000000 pyboiler_anonoei-0.0.4/pyproject.toml
+-rw-r--r--   0 anonoei    (501) staff       (20)       38 2024-05-12 18:36:38.022971 pyboiler_anonoei-0.0.4/setup.cfg
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 18:36:38.016620 pyboiler_anonoei-0.0.4/src/
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 18:36:38.019376 pyboiler_anonoei-0.0.4/src/pyboiler/
+-rw-r--r--   0 anonoei    (501) staff       (20)      736 2024-05-12 18:36:29.000000 pyboiler_anonoei-0.0.4/src/pyboiler/__init__.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 18:36:38.020474 pyboiler_anonoei-0.0.4/src/pyboiler/_log/
+-rw-r--r--   0 anonoei    (501) staff       (20)      220 2024-05-12 12:42:29.000000 pyboiler_anonoei-0.0.4/src/pyboiler/_log/__init__.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      129 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.4/src/pyboiler/_log/filter.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      421 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.4/src/pyboiler/_log/format.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1778 2024-05-12 12:42:43.000000 pyboiler_anonoei-0.0.4/src/pyboiler/_log/handler.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      878 2024-05-12 12:03:41.000000 pyboiler_anonoei-0.0.4/src/pyboiler/_log/level.py
+-rw-r--r--   0 anonoei    (501) staff       (20)       77 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.4/src/pyboiler/_log/record.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     2313 2024-05-12 10:43:02.000000 pyboiler_anonoei-0.0.4/src/pyboiler/config.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     2591 2024-05-12 13:29:14.000000 pyboiler_anonoei-0.0.4/src/pyboiler/generic.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     2908 2024-05-12 10:51:41.000000 pyboiler_anonoei-0.0.4/src/pyboiler/hml.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1103 2024-05-12 10:24:59.000000 pyboiler_anonoei-0.0.4/src/pyboiler/hson.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     2137 2024-05-12 11:06:15.000000 pyboiler_anonoei-0.0.4/src/pyboiler/imports.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     3393 2024-05-12 18:34:49.000000 pyboiler_anonoei-0.0.4/src/pyboiler/logger.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1583 2024-05-12 13:26:11.000000 pyboiler_anonoei-0.0.4/src/pyboiler/logging.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      571 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.4/src/pyboiler/platform.py
+-rw-r--r--   0 anonoei    (501) staff       (20)      594 2024-05-12 10:40:35.000000 pyboiler_anonoei-0.0.4/src/pyboiler/profiler.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     3531 2024-05-12 13:29:41.000000 pyboiler_anonoei-0.0.4/src/pyboiler/settings.py
+-rw-r--r--   0 anonoei    (501) staff       (20)     1893 2024-05-12 09:53:49.000000 pyboiler_anonoei-0.0.4/src/pyboiler/version.py
+drwxr-xr-x   0 anonoei    (501) staff       (20)        0 2024-05-12 18:36:38.021901 pyboiler_anonoei-0.0.4/src/pyboiler_anonoei.egg-info/
+-rw-r--r--   0 anonoei    (501) staff       (20)     1281 2024-05-12 18:36:38.000000 pyboiler_anonoei-0.0.4/src/pyboiler_anonoei.egg-info/PKG-INFO
+-rw-r--r--   0 anonoei    (501) staff       (20)      704 2024-05-12 18:36:38.000000 pyboiler_anonoei-0.0.4/src/pyboiler_anonoei.egg-info/SOURCES.txt
+-rw-r--r--   0 anonoei    (501) staff       (20)        1 2024-05-12 18:36:38.000000 pyboiler_anonoei-0.0.4/src/pyboiler_anonoei.egg-info/dependency_links.txt
+-rw-r--r--   0 anonoei    (501) staff       (20)       34 2024-05-12 18:36:38.000000 pyboiler_anonoei-0.0.4/src/pyboiler_anonoei.egg-info/requires.txt
+-rw-r--r--   0 anonoei    (501) staff       (20)        9 2024-05-12 18:36:38.000000 pyboiler_anonoei-0.0.4/src/pyboiler_anonoei.egg-info/top_level.txt
```

### Comparing `pyboiler_anonoei-0.0.3/LICENSE` & `pyboiler_anonoei-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/PKG-INFO` & `pyboiler_anonoei-0.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboiler_anonoei
-Version: 0.0.3
+Version: 0.0.4
 Summary: Various generic python helpers so I don't keep rewriting them
 Author-email: Anonoei <dev@anonoei.com>
 Project-URL: Homepage, https://github.com/anonoei/pyboiler
 Project-URL: Documentation, https://anonoei.github.io/pyboiler/
 Project-URL: Repository, https://github.com/Anonoei/pyboiler.git
 Project-URL: Issues, https://github.com/Anonoei/pyboiler/issues
 Project-URL: Source, https://github.com/anonoei/pyboiler
@@ -22,10 +22,14 @@
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pdoc3; extra == "dev"
 
 # pyboiler
  Various generic python helpers so I don't keep rewriting them
 
+URLs:
+ - [PyPI](https://pypi.org/project/pyboiler-anonoei/)
+ - [Docs](https://anonoei.github.io/pyboiler/)
+
 ## Install
 1. Run `python3 -m pip install pyboiler-anonoei`
 2. In your project, `import pyboiler`
```

### Comparing `pyboiler_anonoei-0.0.3/pyproject.toml` & `pyboiler_anonoei-0.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyboiler_anonoei"
-version = "0.0.3"
+version = "0.0.4"
 description = "Various generic python helpers so I don't keep rewriting them"
 dependencies = []
 requires-python = ">=3.6"
 authors = [
     {name = "Anonoei", email="dev@anonoei.com"}
 ]
 readme = "README.md"
@@ -31,15 +31,15 @@
 Issues = "https://github.com/Anonoei/pyboiler/issues"
 Source = "https://github.com/anonoei/pyboiler"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "pytest", "pdoc3"]
 
 [tool.bumpver]
-current_version = "0.0.3"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/__init__.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """pyboiler's initialization and dynamic importer
 
  Imports all files in src/pyboiler/* so they can be imported as
  `pyboiler.config`
 """
 
-__version__ = "0.0.3"
+import pathlib
+
+__version__ = "0.0.4"
 __author__ = "Anonoei <dev@anonoei.com>"
 
 
 def __init():
     """Import all files in `import_path`"""
     from .config import config
     from .imports import get_imports
 
-    import_path = config().PATH_ROOT / "src" / "pyboiler"
+    import_path = pathlib.Path(__file__).parent
 
     # print(f"Running __init on {import_path}")
     for k, v in get_imports(import_path).items():
         globals()[k] = v
 
     globals()["settings"].Settings().deserialize()
```

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/_log/handler.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/_log/handler.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/_log/level.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/_log/level.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/config.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/config.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/generic.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/generic.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/hml.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/hml.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/hson.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/hson.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/imports.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/imports.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/logger.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             path_sep = path_sep[1:]
         log_path = config().PATH_LOGS
         for idx, item in enumerate(path_sep):
             if idx == len(path_sep) - 1:
                 log_path.mkdir(exist_ok=True, parents=True)
                 item = f"{item}.log"
             log_path /= item
-            print(f"{log_path = }")
+            # print(f"{log_path = }")
         return log_path
 
     def _setLogs(self):
         for level in self._log.levels():
             lname = level.name.lower()
             log_cmd = (
                 lambda msg, log=self._log, lvl=level.value, *args, **kwargs: log.log(
```

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/logging.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/logging.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/platform.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/platform.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/profiler.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/profiler.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/settings.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/settings.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler/version.py` & `pyboiler_anonoei-0.0.4/src/pyboiler/version.py`

 * *Files identical despite different names*

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/PKG-INFO` & `pyboiler_anonoei-0.0.4/src/pyboiler_anonoei.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyboiler_anonoei
-Version: 0.0.3
+Version: 0.0.4
 Summary: Various generic python helpers so I don't keep rewriting them
 Author-email: Anonoei <dev@anonoei.com>
 Project-URL: Homepage, https://github.com/anonoei/pyboiler
 Project-URL: Documentation, https://anonoei.github.io/pyboiler/
 Project-URL: Repository, https://github.com/Anonoei/pyboiler.git
 Project-URL: Issues, https://github.com/Anonoei/pyboiler/issues
 Project-URL: Source, https://github.com/anonoei/pyboiler
@@ -22,10 +22,14 @@
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pdoc3; extra == "dev"
 
 # pyboiler
  Various generic python helpers so I don't keep rewriting them
 
+URLs:
+ - [PyPI](https://pypi.org/project/pyboiler-anonoei/)
+ - [Docs](https://anonoei.github.io/pyboiler/)
+
 ## Install
 1. Run `python3 -m pip install pyboiler-anonoei`
 2. In your project, `import pyboiler`
```

### Comparing `pyboiler_anonoei-0.0.3/src/pyboiler_anonoei.egg-info/SOURCES.txt` & `pyboiler_anonoei-0.0.4/src/pyboiler_anonoei.egg-info/SOURCES.txt`

 * *Files identical despite different names*

