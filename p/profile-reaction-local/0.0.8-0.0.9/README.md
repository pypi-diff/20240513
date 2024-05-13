# Comparing `tmp/profile-reaction-local-0.0.8.tar.gz` & `tmp/profile-reaction-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile-reaction-local-0.0.8.tar", last modified: Sun Sep 10 14:53:28 2023, max compression
+gzip compressed data, was "profile-reaction-local-0.0.9.tar", last modified: Sun Sep 10 15:10:35 2023, max compression
```

## Comparing `profile-reaction-local-0.0.8.tar` & `profile-reaction-local-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 14:53:28.319656 profile-reaction-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-09-10 14:53:28.319656 profile-reaction-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-09-10 14:53:03.000000 profile-reaction-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 14:53:28.315657 profile-reaction-local-0.0.8/profile_reaction_local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 14:53:03.000000 profile-reaction-local-0.0.8/profile_reaction_local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 14:53:28.319656 profile-reaction-local-0.0.8/profile_reaction_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 14:53:03.000000 profile-reaction-local-0.0.8/profile_reaction_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-09-10 14:53:03.000000 profile-reaction-local-0.0.8/profile_reaction_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13985 2023-09-10 14:53:03.000000 profile-reaction-local-0.0.8/profile_reaction_local/src/profile_reaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-09-10 14:53:03.000000 profile-reaction-local-0.0.8/profile_reaction_local/src/profile_reaction_dto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 14:53:28.315657 profile-reaction-local-0.0.8/profile_reaction_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-09-10 14:53:28.000000 profile-reaction-local-0.0.8/profile_reaction_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-09-10 14:53:28.000000 profile-reaction-local-0.0.8/profile_reaction_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-10 14:53:28.000000 profile-reaction-local-0.0.8/profile_reaction_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-10 14:53:28.000000 profile-reaction-local-0.0.8/profile_reaction_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      756 2023-09-10 14:53:03.000000 profile-reaction-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-10 14:53:28.319656 profile-reaction-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-09-10 14:53:03.000000 profile-reaction-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 15:10:35.494438 profile-reaction-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2023-09-10 15:10:35.494438 profile-reaction-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-09-10 15:10:05.000000 profile-reaction-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 15:10:35.490438 profile-reaction-local-0.0.9/profile_reaction_local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 15:10:05.000000 profile-reaction-local-0.0.9/profile_reaction_local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 15:10:35.494438 profile-reaction-local-0.0.9/profile_reaction_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-10 15:10:05.000000 profile-reaction-local-0.0.9/profile_reaction_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2023-09-10 15:10:05.000000 profile-reaction-local-0.0.9/profile_reaction_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13985 2023-09-10 15:10:05.000000 profile-reaction-local-0.0.9/profile_reaction_local/src/profile_reaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2023-09-10 15:10:05.000000 profile-reaction-local-0.0.9/profile_reaction_local/src/profile_reaction_dto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-10 15:10:35.490438 profile-reaction-local-0.0.9/profile_reaction_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2023-09-10 15:10:35.000000 profile-reaction-local-0.0.9/profile_reaction_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2023-09-10 15:10:35.000000 profile-reaction-local-0.0.9/profile_reaction_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-10 15:10:35.000000 profile-reaction-local-0.0.9/profile_reaction_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-10 15:10:35.000000 profile-reaction-local-0.0.9/profile_reaction_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2023-09-10 15:10:05.000000 profile-reaction-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-10 15:10:35.494438 profile-reaction-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2023-09-10 15:10:05.000000 profile-reaction-local-0.0.9/setup.py
```

### Comparing `profile-reaction-local-0.0.8/PKG-INFO` & `profile-reaction-local-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-reaction-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles Profile Reaction Local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profile-reaction-local-0.0.8/README.md` & `profile-reaction-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `profile-reaction-local-0.0.8/profile_reaction_local/src/constants.py` & `profile-reaction-local-0.0.9/profile_reaction_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `profile-reaction-local-0.0.8/profile_reaction_local/src/profile_reaction.py` & `profile-reaction-local-0.0.9/profile_reaction_local/src/profile_reaction.py`

 * *Files identical despite different names*

### Comparing `profile-reaction-local-0.0.8/profile_reaction_local/src/profile_reaction_dto.py` & `profile-reaction-local-0.0.9/profile_reaction_local/src/profile_reaction_dto.py`

 * *Files identical despite different names*

### Comparing `profile-reaction-local-0.0.8/profile_reaction_local.egg-info/PKG-INFO` & `profile-reaction-local-0.0.9/profile_reaction_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-reaction-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles Profile Reaction Local Python
 Home-page: https://github.com/circles
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profile-reaction-local-0.0.8/pyproject.toml` & `profile-reaction-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `profile-reaction-local-0.0.8/setup.py` & `profile-reaction-local-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 # Each Python project should have pyproject.toml or setup.py
 # used by python -m build
 # ```python -m build``` needs pyproject.toml or setup.py
 # The need for setup.py is changing as of poetry 1.1.0 (including current pre-release) as we have moved away from needing to generate a setup.py file to enable editable installs - We might able to delete this file in the near future
 setuptools.setup(
     name='profile-reaction-local',
-    version='0.0.8',  # https://pypi.org/project/profile-reaction-local/
+    version='0.0.9',  # https://pypi.org/project/profile-reaction-local/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Profile Reaction Local Python",
     long_description="This is a package for sharing common methods of profile reaction CRUD to profile_reaction database used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/circles",
     packages=setuptools.find_packages(),
```

