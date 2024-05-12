# Comparing `tmp/dj-dynamic-settings-0.2.5.tar.gz` & `tmp/dj-dynamic-settings-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dj-dynamic-settings-0.2.5.tar", last modified: Mon May  6 06:45:22 2024, max compression
+gzip compressed data, was "dj-dynamic-settings-0.2.6.tar", last modified: Sun May 12 22:34:09 2024, max compression
```

## Comparing `dj-dynamic-settings-0.2.5.tar` & `dj-dynamic-settings-0.2.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1304 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/.gitignore
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      113 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/.isort.cfg
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       28 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/CHANGELOG.md
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1050 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/LICENSE.txt
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4765 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/PKG-INFO
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     3305 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/README.md
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2629 2024-04-30 14:37:07.000000 dj-dynamic-settings-0.2.5/bitbucket-pipelines.yml
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        0 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/__init__.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       63 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/admin.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      856 2024-04-30 16:15:59.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/app_settings.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      152 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/apps.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      602 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/compat.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     3093 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/conf.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       52 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/exceptions.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      811 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/metadata.py
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/migrations/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      970 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/migrations/0001_initial.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        0 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/migrations/__init__.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1215 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/models.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1352 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/registry.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2515 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/serializers.py
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        0 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/__init__.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1790 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/definitions.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4250 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_dynamic_settings.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2377 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_override_settings.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      624 2024-04-30 16:24:36.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_settings.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4014 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_views.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      225 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/urls.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      630 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/utils.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     3550 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/validators.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1004 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings/views.py
-drwxrwxr-x   0 ozkok     (1000) ozkok     (1000)        0 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     4765 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/PKG-INFO
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1176 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/SOURCES.txt
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        1 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/dependency_links.txt
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)        1 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/not-zip-safe
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       20 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/top_level.txt
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      302 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/pyproject.toml
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       42 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/requirements.txt
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)      430 2024-02-02 07:41:40.000000 dj-dynamic-settings-0.2.5/runtests.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)       38 2024-05-06 06:45:22.000000 dj-dynamic-settings-0.2.5/setup.cfg
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     2257 2024-04-30 14:37:07.000000 dj-dynamic-settings-0.2.5/setup.py
--rw-rw-r--   0 ozkok     (1000) ozkok     (1000)     1385 2024-04-30 14:43:01.000000 dj-dynamic-settings-0.2.5/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/
+-rw-rw-rw-   0 root         (0) root         (0)     1304 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       28 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     4765 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3305 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2637 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:34:09.008124 dj-dynamic-settings-0.2.6/dj_dynamic_settings/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      856 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/app_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      602 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/compat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)       52 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/metadata.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/dj_dynamic_settings/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      970 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1352 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2515 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/serializers.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1790 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/definitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4250 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_dynamic_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_override_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      624 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)     4014 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3550 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1004 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings/views.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4765 2024-05-12 22:34:08.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1176 2024-05-12 22:34:08.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-12 22:34:08.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-12 22:34:08.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-12 22:34:08.000000 dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       42 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/runtests.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-12 22:34:09.012124 dj-dynamic-settings-0.2.6/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2257 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2024-05-12 22:33:45.000000 dj-dynamic-settings-0.2.6/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `dj-dynamic-settings-0.2.5/.gitignore` & `dj-dynamic-settings-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/LICENSE.txt` & `dj-dynamic-settings-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/PKG-INFO` & `dj-dynamic-settings-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-dynamic-settings
-Version: 0.2.5
+Version: 0.2.6
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-dynamic-settings/
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
```

### Comparing `dj-dynamic-settings-0.2.5/README.md` & `dj-dynamic-settings-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/bitbucket-pipelines.yml` & `dj-dynamic-settings-0.2.6/bitbucket-pipelines.yml`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,14 @@
           name: Publish to PyPI
           image: python:3.8-alpine
           script:
             - apk add gcc git libffi-dev musl-dev openssl-dev python3-dev
             - pip install --upgrade pip
             - pip install setuptools==57.5.0 setuptools_scm==7.1.0 twine==4.0.2
             - python setup.py sdist bdist_wheel
-            - twine upload -u $PYPI_USERNAME -p $PYPI_PASSWORD dist/*
+            - twine upload -u __token__ -p $PYPI_TOKEN --skip-existing dist/*
 definitions:
   services:
     postgres:
       image: postgres
       variables:
         POSTGRES_PASSWORD: postgres
```

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/app_settings.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/app_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/compat.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/compat.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/conf.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/conf.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/metadata.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/metadata.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/migrations/0001_initial.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/models.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/models.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/registry.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/registry.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/serializers.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/definitions.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/definitions.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_dynamic_settings.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_dynamic_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_override_settings.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_override_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_settings.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/tests/test_views.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/utils.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/utils.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/validators.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/validators.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings/views.py` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings/views.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/PKG-INFO` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-dynamic-settings
-Version: 0.2.5
+Version: 0.2.6
 Summary: Stay informed of it
 Home-page: https://bitbucket.org/akinonteam/dj-dynamic-settings/
 Author: Akinon
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
```

### Comparing `dj-dynamic-settings-0.2.5/dj_dynamic_settings.egg-info/SOURCES.txt` & `dj-dynamic-settings-0.2.6/dj_dynamic_settings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/setup.py` & `dj-dynamic-settings-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `dj-dynamic-settings-0.2.5/tox.ini` & `dj-dynamic-settings-0.2.6/tox.ini`

 * *Files identical despite different names*

