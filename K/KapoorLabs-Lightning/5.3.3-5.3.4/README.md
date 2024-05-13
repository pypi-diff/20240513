# Comparing `tmp/kapoorlabs_lightning-5.3.3.tar.gz` & `tmp/kapoorlabs_lightning-5.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kapoorlabs_lightning-5.3.3.tar", last modified: Mon May 13 15:23:48 2024, max compression
+gzip compressed data, was "kapoorlabs_lightning-5.3.4.tar", last modified: Mon May 13 16:14:52 2024, max compression
```

## Comparing `kapoorlabs_lightning-5.3.3.tar` & `kapoorlabs_lightning-5.3.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.422665 kapoorlabs_lightning-5.3.3/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.410665 kapoorlabs_lightning-5.3.3/.github/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.414666 kapoorlabs_lightning-5.3.3/.github/workflows/
--rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/.github/workflows/deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/.gitignore
--rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/.pre-commit-config.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/LICENSE
--rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/MANIFEST.in
--rw-r--r--   0 debian    (1000) debian    (1000)     4088 2024-05-13 15:23:48.422665 kapoorlabs_lightning-5.3.3/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.414666 kapoorlabs_lightning-5.3.3/licenses/
--rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/Apache-2
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/BSD-3
--rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/GPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/LGPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/MIT
--rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/MPL-2
--rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/pyproject.toml
--rw-r--r--   0 debian    (1000) debian    (1000)     1760 2024-05-13 15:23:48.422665 kapoorlabs_lightning-5.3.3/setup.cfg
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.410665 kapoorlabs_lightning-5.3.3/src/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.418666 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     4088 2024-05-13 15:23:48.000000 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1269 2024-05-13 15:23:48.000000 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-13 15:23:48.000000 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       97 2024-05-13 15:23:48.000000 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-13 15:23:48.000000 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.418666 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/
--rw-r--r--   0 debian    (1000) debian    (1000)     1520 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.418666 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/_tests/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/_tests/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-13 15:18:09.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/_version.py
--rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/caped.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/graph_functions.py
--rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/kapoorlabs.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)    62956 2024-05-13 15:17:09.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/lightning_trainer.py
--rw-r--r--   0 debian    (1000) debian    (1000)    13629 2024-05-13 15:18:01.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/metrics.py
--rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/optimizers.py
--rw-r--r--   0 debian    (1000) debian    (1000)     8759 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_callbacks.py
--rw-r--r--   0 debian    (1000) debian    (1000)    16235 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_datasets.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_loggers.py
--rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_losses.py
--rw-r--r--   0 debian    (1000) debian    (1000)    22968 2024-05-13 15:16:47.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_transforms.py
--rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/schedulers.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1340 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/utils.py
--rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/tox.ini
--rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/update_version.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 16:14:52.593941 kapoorlabs_lightning-5.3.4/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 16:14:52.585941 kapoorlabs_lightning-5.3.4/.github/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 16:14:52.589941 kapoorlabs_lightning-5.3.4/.github/workflows/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/.github/workflows/deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/.gitignore
+-rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/LICENSE
+-rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/MANIFEST.in
+-rw-r--r--   0 debian    (1000) debian    (1000)     4088 2024-05-13 16:14:52.593941 kapoorlabs_lightning-5.3.4/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 16:14:52.589941 kapoorlabs_lightning-5.3.4/licenses/
+-rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/licenses/Apache-2
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/licenses/BSD-3
+-rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/licenses/GPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/licenses/LGPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/licenses/MIT
+-rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/licenses/MPL-2
+-rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/pyproject.toml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1760 2024-05-13 16:14:52.597941 kapoorlabs_lightning-5.3.4/setup.cfg
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 16:14:52.589941 kapoorlabs_lightning-5.3.4/src/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 16:14:52.593941 kapoorlabs_lightning-5.3.4/src/KapoorLabs_Lightning.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     4088 2024-05-13 16:14:52.000000 kapoorlabs_lightning-5.3.4/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1269 2024-05-13 16:14:52.000000 kapoorlabs_lightning-5.3.4/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-13 16:14:52.000000 kapoorlabs_lightning-5.3.4/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       97 2024-05-13 16:14:52.000000 kapoorlabs_lightning-5.3.4/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-13 16:14:52.000000 kapoorlabs_lightning-5.3.4/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 16:14:52.593941 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1566 2024-05-13 15:57:41.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 16:14:52.593941 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/_tests/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/_tests/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-13 16:06:54.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/_version.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/caped.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/graph_functions.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)    62612 2024-05-13 16:03:49.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/lightning_trainer.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    13629 2024-05-13 15:18:01.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/metrics.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/optimizers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     8759 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_callbacks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    16235 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_datasets.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_loggers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_losses.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    22968 2024-05-13 15:16:47.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_transforms.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/schedulers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1340 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/utils.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/tox.ini
+-rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.4/update_version.py
```

### Comparing `kapoorlabs_lightning-5.3.3/.github/workflows/deploy.yml` & `kapoorlabs_lightning-5.3.4/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/.github/workflows/test_and_deploy.yml` & `kapoorlabs_lightning-5.3.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/.gitignore` & `kapoorlabs_lightning-5.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/.pre-commit-config.yaml` & `kapoorlabs_lightning-5.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/LICENSE` & `kapoorlabs_lightning-5.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/PKG-INFO` & `kapoorlabs_lightning-5.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.3.3
+Version: 5.3.4
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `kapoorlabs_lightning-5.3.3/README.md` & `kapoorlabs_lightning-5.3.4/README.md`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/licenses/Apache-2` & `kapoorlabs_lightning-5.3.4/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/licenses/BSD-3` & `kapoorlabs_lightning-5.3.4/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/licenses/GPL-3` & `kapoorlabs_lightning-5.3.4/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/licenses/LGPL-3` & `kapoorlabs_lightning-5.3.4/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/licenses/MIT` & `kapoorlabs_lightning-5.3.4/licenses/MIT`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/licenses/MPL-2` & `kapoorlabs_lightning-5.3.4/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/setup.cfg` & `kapoorlabs_lightning-5.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `kapoorlabs_lightning-5.3.4/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.3.3
+Version: 5.3.4
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `kapoorlabs_lightning-5.3.4/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/__init__.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from .lightning_trainer import (
     AutoLightningModel,
     AutoLightningTrain,
     LightningData,
     LightningModel,
     LightningTrain,
+    MitosisInception,
 )
 from .pytorch_datasets import (
     PointCloudDataset,
     PointCloudNpzDataset,
     PyntCloud,
     ShapeNetDataset,
     SingleCellDataset,
@@ -57,9 +58,10 @@
     "CustomProgressBar",
     "CheckpointModel",
     "CustomVirtualMemory",
     "MitosisDataset",
     "Adam",
     "RMSprop",
     "Rprop",
+    "MitosisInception",
 ]
 __all__.extend(all_pytorch_models)
```

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/graph_functions.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/lightning_trainer.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/lightning_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,14 @@
 
     LOSS_CHOICES = ["cross_entropy", "cosine", "bce", "mse"]
     SCHEDULER_CHOICES = ["cosine", "exponential", "multistep", "plateau", "warmup"]
 
     def __init__(
         self,
         npz_file: str,
-        input_channels,
         num_classes,
         growth_rate: int = 32,
         block_config: tuple = (6, 12, 24, 16),
         num_init_features: int = 32,
         bottleneck_size: int = 4,
         kernel_size: int = 3,
         num_workers: int = 1,
@@ -80,27 +79,26 @@
         learning_rate: float = 0.001,
         eta_min: float = 1.0e-8,
         momentum: float = 0.9,
         decay: float = 1e-4,
         epsilon: float = 1.0,
         gamma: float = 0.94,
         slurm_auto_requeue: bool = False,
-        train_precision: str = "16-mixed",
+        train_precision: str = "32",
         gradient_clip_val: float = None,
         gradient_clip_algorithm: str = None,
         milestones: List = None,
         factor: float = 0.1,
         patience: int = 10,
         threshold: float = 1e-4,
         t_warmup: int = 0,
         t_max: int = 1,
         strategy: str = "auto",
     ):
         self.npz_file = npz_file
-        self.input_channels = input_channels
         self.num_classes = num_classes
         self.growth_rate = growth_rate
         self.block_config = block_config
         self.num_init_features = num_init_features
         self.bottleneck_size = bottleneck_size
         self.kernel_size = kernel_size
         self.num_workers = num_workers
@@ -126,15 +124,14 @@
         self.gradient_clip_algorithm = gradient_clip_algorithm
         self.milestones = milestones
         self.factor = factor
         self.patience = patience
         self.threshold = threshold
         self.t_warmup = t_warmup
         self.strategy = strategy
-        self.dataset_path = os.path.join(self.dataset_dir, self.dataset_name + ".h5")
         if self.loss_function not in self.LOSS_CHOICES:
             raise ValueError(
                 f"Invalid loss function choice, must be one of {self.LOSS_CHOICES}"
             )
         if self.scheduler_choice not in self.SCHEDULER_CHOICES:
             raise ValueError(
                 f"Invalid scheduler choice, must be one of {self.SCHEDULER_CHOICES}"
@@ -158,14 +155,16 @@
         )
         train_labels = np.concatenate(
             (train_dividing_labels, train_non_dividing_labels)
         )
 
         self.dataset_train = MitosisDataset(train_arrays, train_labels)
 
+        self.input_channels = self.dataset_train.input_channels
+
         val_arrays = np.concatenate((val_dividing_arrays, val_non_dividing_arrays))
         val_labels = np.concatenate((val_dividing_labels, val_non_dividing_labels))
 
         self.dataset_val = MitosisDataset(val_arrays, val_labels)
 
         self.mitosis_data = LightningData(
             data_train=self.dataset_train,
@@ -236,20 +235,15 @@
                 factor=self.factor, patience=self.patience, threshold=self.threshold
             )
         if self.scheduler_choice == "warmup":
             self.scheduler = WarmCosineAnnealingLR(
                 t_warmup=self.t_warmup, t_max=self.t_max, eta_min=self.eta_min
             )
 
-    def setup_lightning_model(
-        self,
-        tensor_dtype=torch.long,
-        use_bce_loss=False,
-        reduce_lr_metric="val_accuracy_epoch",
-    ):
+    def setup_lightning_model(self):
         if self.loss_function == "cross_entropy":
             self.loss = CrossEntropyLoss()
         if self.loss_function == "cosine":
             self.loss = CosineSimilarity()
         if self.loss_function == "bce":
             self.loss = BCEWithLogitsLoss()
         if self.loss_function == "mse":
@@ -257,17 +251,14 @@
 
         self.progress = CustomProgressBar()
         self.lightning_model = LightningModel(
             self.model,
             self.loss,
             self.optimizer,
             scheduler=self.scheduler,
-            use_bce_loss=use_bce_loss,
-            tensor_dtype=tensor_dtype,
-            reduce_lr_metric=reduce_lr_metric,
         )
         model_hyperparameters = {
             "input_channels": self.input_channels,
             "num_classes": self.num_classes,
             "learning_rate": self.learning_rate,
             "model_path": self.log_path,
             "model_name": self.experiment_name,
```

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/metrics.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/metrics.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/optimizers.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/optimizers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_callbacks.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_callbacks.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_datasets.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_loggers.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_losses.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_models.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_transforms.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/schedulers.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/schedulers.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/utils.py` & `kapoorlabs_lightning-5.3.4/src/kapoorlabs_lightning/utils.py`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/tox.ini` & `kapoorlabs_lightning-5.3.4/tox.ini`

 * *Files identical despite different names*

### Comparing `kapoorlabs_lightning-5.3.3/update_version.py` & `kapoorlabs_lightning-5.3.4/update_version.py`

 * *Files identical despite different names*

