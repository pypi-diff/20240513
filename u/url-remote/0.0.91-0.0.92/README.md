# Comparing `tmp/url_remote-0.0.91.tar.gz` & `tmp/url_remote-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "url_remote-0.0.91.tar", last modified: Mon May  6 16:01:34 2024, max compression
+gzip compressed data, was "url_remote-0.0.92.tar", last modified: Sun May 12 22:47:50 2024, max compression
```

## Comparing `url_remote-0.0.91.tar` & `url_remote-0.0.92.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:01:34.315023 url_remote-0.0.91/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-06 16:01:34.315023 url_remote-0.0.91/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-06 16:01:23.000000 url_remote-0.0.91/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-06 16:01:23.000000 url_remote-0.0.91/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 16:01:34.315023 url_remote-0.0.91/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-06 16:01:23.000000 url_remote-0.0.91/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:01:34.311023 url_remote-0.0.91/url_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:01:34.315023 url_remote-0.0.91/url_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:01:23.000000 url_remote-0.0.91/url_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-06 16:01:23.000000 url_remote-0.0.91/url_remote/src/action_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-06 16:01:23.000000 url_remote-0.0.91/url_remote/src/api_version_dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-06 16:01:23.000000 url_remote-0.0.91/url_remote/src/authentiction_api_version_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-06 16:01:23.000000 url_remote-0.0.91/url_remote/src/brand_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-06 16:01:23.000000 url_remote-0.0.91/url_remote/src/component_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-06 16:01:23.000000 url_remote-0.0.91/url_remote/src/entity_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 16:01:23.000000 url_remote-0.0.91/url_remote/src/environment_name_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-06 16:01:23.000000 url_remote-0.0.91/url_remote/src/url_circlez.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:01:34.315023 url_remote-0.0.91/url_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-06 16:01:34.000000 url_remote-0.0.91/url_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-06 16:01:34.000000 url_remote-0.0.91/url_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:01:34.000000 url_remote-0.0.91/url_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 16:01:34.000000 url_remote-0.0.91/url_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:47:50.047888 url_remote-0.0.92/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-12 22:47:50.047888 url_remote-0.0.92/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-12 22:47:42.000000 url_remote-0.0.92/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-12 22:47:42.000000 url_remote-0.0.92/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 22:47:50.047888 url_remote-0.0.92/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-12 22:47:42.000000 url_remote-0.0.92/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:47:50.043888 url_remote-0.0.92/url_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:47:50.047888 url_remote-0.0.92/url_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/action_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/api_version_dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/authentiction_api_version_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/brand_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/component_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/entity_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/environment_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9047 2024-05-12 22:47:42.000000 url_remote-0.0.92/url_remote/src/url_circlez.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 22:47:50.047888 url_remote-0.0.92/url_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-12 22:47:50.000000 url_remote-0.0.92/url_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-12 22:47:50.000000 url_remote-0.0.92/url_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 22:47:50.000000 url_remote-0.0.92/url_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-12 22:47:50.000000 url_remote-0.0.92/url_remote.egg-info/top_level.txt
```

### Comparing `url_remote-0.0.91/README.md` & `url_remote-0.0.92/README.md`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.91/setup.py` & `url_remote-0.0.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "url-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.91',  # https://pypi.org/project/url-remote
+    version='0.0.92',  # https://pypi.org/project/url-remote
     author="Circles",
     author_email="info@circles.life",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="URL Local",
```

### Comparing `url_remote-0.0.91/url_remote/src/action_name_enum.py` & `url_remote-0.0.92/url_remote/src/action_name_enum.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.91/url_remote/src/component_name_enum.py` & `url_remote-0.0.92/url_remote/src/component_name_enum.py`

 * *Files identical despite different names*

### Comparing `url_remote-0.0.91/url_remote/src/url_circlez.py` & `url_remote-0.0.92/url_remote/src/url_circlez.py`

 * *Files identical despite different names*

