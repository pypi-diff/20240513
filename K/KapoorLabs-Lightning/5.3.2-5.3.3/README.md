# Comparing `tmp/KapoorLabs-Lightning-5.3.2.tar.gz` & `tmp/kapoorlabs_lightning-5.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KapoorLabs-Lightning-5.3.2.tar", last modified: Fri Feb 23 15:05:14 2024, max compression
+gzip compressed data, was "kapoorlabs_lightning-5.3.3.tar", last modified: Mon May 13 15:23:48 2024, max compression
```

## Comparing `KapoorLabs-Lightning-5.3.2.tar` & `kapoorlabs_lightning-5.3.3.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-02-23 15:05:14.542251 KapoorLabs-Lightning-5.3.2/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-02-23 15:05:14.534251 KapoorLabs-Lightning-5.3.2/.github/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-02-23 15:05:14.534251 KapoorLabs-Lightning-5.3.2/.github/workflows/
--rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/.github/workflows/deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/.gitignore
--rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/.pre-commit-config.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/LICENSE
--rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/MANIFEST.in
--rw-r--r--   0 debian    (1000) debian    (1000)     4088 2024-02-23 15:05:14.542251 KapoorLabs-Lightning-5.3.2/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/README.md
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-02-23 15:05:14.534251 KapoorLabs-Lightning-5.3.2/licenses/
--rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/licenses/Apache-2
--rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/licenses/BSD-3
--rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/licenses/GPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/licenses/LGPL-3
--rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/licenses/MIT
--rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/licenses/MPL-2
--rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/pyproject.toml
--rw-r--r--   0 debian    (1000) debian    (1000)     1834 2024-02-23 15:05:14.542251 KapoorLabs-Lightning-5.3.2/setup.cfg
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-02-23 15:05:14.534251 KapoorLabs-Lightning-5.3.2/src/
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-02-23 15:05:14.538251 KapoorLabs-Lightning-5.3.2/src/KapoorLabs_Lightning.egg-info/
--rw-r--r--   0 debian    (1000) debian    (1000)     4088 2024-02-23 15:05:14.000000 KapoorLabs-Lightning-5.3.2/src/KapoorLabs_Lightning.egg-info/PKG-INFO
--rw-r--r--   0 debian    (1000) debian    (1000)     1204 2024-02-23 15:05:14.000000 KapoorLabs-Lightning-5.3.2/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
--rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-02-23 15:05:14.000000 KapoorLabs-Lightning-5.3.2/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       72 2024-02-23 15:05:14.000000 KapoorLabs-Lightning-5.3.2/src/KapoorLabs_Lightning.egg-info/entry_points.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       97 2024-02-23 15:05:14.000000 KapoorLabs-Lightning-5.3.2/src/KapoorLabs_Lightning.egg-info/requires.txt
--rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-02-23 15:05:14.000000 KapoorLabs-Lightning-5.3.2/src/KapoorLabs_Lightning.egg-info/top_level.txt
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-02-23 15:05:14.538251 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/
--rw-r--r--   0 debian    (1000) debian    (1000)      859 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/__init__.py
-drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-02-23 15:05:14.538251 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/_tests/
--rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/_tests/__init__.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-02-23 15:03:45.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/_version.py
--rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/caped.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/graph_functions.py
--rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/kapoorlabs.yaml
--rw-r--r--   0 debian    (1000) debian    (1000)    35120 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/lightning_trainer.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3538 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/optimizers.py
--rw-r--r--   0 debian    (1000) debian    (1000)    15688 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/pytorch_datasets.py
--rw-r--r--   0 debian    (1000) debian    (1000)     2715 2024-02-23 15:03:40.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/pytorch_loggers.py
--rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/pytorch_losses.py
--rw-r--r--   0 debian    (1000) debian    (1000)    16569 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/pytorch_models.py
--rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/pytorch_transforms.py
--rw-r--r--   0 debian    (1000) debian    (1000)     3123 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/schedulers.py
--rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/tox.ini
--rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 KapoorLabs-Lightning-5.3.2/update_version.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.422665 kapoorlabs_lightning-5.3.3/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.410665 kapoorlabs_lightning-5.3.3/.github/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.414666 kapoorlabs_lightning-5.3.3/.github/workflows/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1068 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/.github/workflows/deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1963 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 debian    (1000) debian    (1000)      991 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/.gitignore
+-rw-r--r--   0 debian    (1000) debian    (1000)     1008 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/.pre-commit-config.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/LICENSE
+-rw-r--r--   0 debian    (1000) debian    (1000)       96 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/MANIFEST.in
+-rw-r--r--   0 debian    (1000) debian    (1000)     4088 2024-05-13 15:23:48.422665 kapoorlabs_lightning-5.3.3/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     2435 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/README.md
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.414666 kapoorlabs_lightning-5.3.3/licenses/
+-rw-r--r--   0 debian    (1000) debian    (1000)    11358 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/Apache-2
+-rw-r--r--   0 debian    (1000) debian    (1000)     1487 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/BSD-3
+-rw-r--r--   0 debian    (1000) debian    (1000)    35148 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/GPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     7653 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/LGPL-3
+-rw-r--r--   0 debian    (1000) debian    (1000)     1080 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/MIT
+-rw-r--r--   0 debian    (1000) debian    (1000)    16726 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/licenses/MPL-2
+-rw-r--r--   0 debian    (1000) debian    (1000)      116 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/pyproject.toml
+-rw-r--r--   0 debian    (1000) debian    (1000)     1760 2024-05-13 15:23:48.422665 kapoorlabs_lightning-5.3.3/setup.cfg
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.410665 kapoorlabs_lightning-5.3.3/src/
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.418666 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/
+-rw-r--r--   0 debian    (1000) debian    (1000)     4088 2024-05-13 15:23:48.000000 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/PKG-INFO
+-rw-r--r--   0 debian    (1000) debian    (1000)     1269 2024-05-13 15:23:48.000000 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/SOURCES.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)        1 2024-05-13 15:23:48.000000 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/dependency_links.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       97 2024-05-13 15:23:48.000000 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/requires.txt
+-rw-r--r--   0 debian    (1000) debian    (1000)       21 2024-05-13 15:23:48.000000 kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/top_level.txt
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.418666 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/
+-rw-r--r--   0 debian    (1000) debian    (1000)     1520 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/__init__.py
+drwxr-xr-x   0 debian    (1000) debian    (1000)        0 2024-05-13 15:23:48.418666 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/_tests/
+-rw-r--r--   0 debian    (1000) debian    (1000)        0 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/_tests/__init__.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     3106 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/_tests/test_pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       78 2024-05-13 15:18:09.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/_version.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       75 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/caped.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)     2065 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/graph_functions.py
+-rw-r--r--   0 debian    (1000) debian    (1000)       68 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/kapoorlabs.yaml
+-rw-r--r--   0 debian    (1000) debian    (1000)    62956 2024-05-13 15:17:09.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/lightning_trainer.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    13629 2024-05-13 15:18:01.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/metrics.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     4658 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/optimizers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     8759 2024-05-13 15:11:51.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_callbacks.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    16235 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_datasets.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     2680 2024-02-23 15:21:15.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_loggers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      762 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_losses.py
+-rw-r--r--   0 debian    (1000) debian    (1000)    22968 2024-05-13 15:16:47.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_models.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1809 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_transforms.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     6283 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/schedulers.py
+-rw-r--r--   0 debian    (1000) debian    (1000)     1340 2024-05-13 15:11:52.000000 kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/utils.py
+-rw-r--r--   0 debian    (1000) debian    (1000)      615 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/tox.ini
+-rw-r--r--   0 debian    (1000) debian    (1000)      623 2024-01-22 18:41:12.000000 kapoorlabs_lightning-5.3.3/update_version.py
```

### Comparing `KapoorLabs-Lightning-5.3.2/.github/workflows/deploy.yml` & `kapoorlabs_lightning-5.3.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/.github/workflows/test_and_deploy.yml` & `kapoorlabs_lightning-5.3.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/.gitignore` & `kapoorlabs_lightning-5.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/.pre-commit-config.yaml` & `kapoorlabs_lightning-5.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/LICENSE` & `kapoorlabs_lightning-5.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/PKG-INFO` & `kapoorlabs_lightning-5.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.3.2
+Version: 5.3.3
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.3.2/README.md` & `kapoorlabs_lightning-5.3.3/README.md`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/licenses/Apache-2` & `kapoorlabs_lightning-5.3.3/licenses/Apache-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/licenses/BSD-3` & `kapoorlabs_lightning-5.3.3/licenses/BSD-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/licenses/GPL-3` & `kapoorlabs_lightning-5.3.3/licenses/GPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/licenses/LGPL-3` & `kapoorlabs_lightning-5.3.3/licenses/LGPL-3`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/licenses/MIT` & `kapoorlabs_lightning-5.3.3/licenses/MIT`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/licenses/MPL-2` & `kapoorlabs_lightning-5.3.3/licenses/MPL-2`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/setup.cfg` & `kapoorlabs_lightning-5.3.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -44,16 +44,14 @@
 	=src
 setup_requires = setuptools_scm
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
-caped.manifest = 
-	KapoorLabs-Lightning = kapoorlabs_lightning:caped.yaml
 
 [options.extras_require]
 testing = 
 	tox
 	pytest  # https://docs.pytest.org/en/latest/contents.html
 	pytest-cov  # https://pytest-cov.readthedocs.io/en/latest/
```

### Comparing `KapoorLabs-Lightning-5.3.2/src/KapoorLabs_Lightning.egg-info/PKG-INFO` & `kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KapoorLabs-Lightning
-Version: 5.3.2
+Version: 5.3.3
 Summary: Lightning modules for KapoorLabs specific projects
 Home-page: https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/KapoorLabs-Lightning#README.md
```

### Comparing `KapoorLabs-Lightning-5.3.2/src/KapoorLabs_Lightning.egg-info/SOURCES.txt` & `kapoorlabs_lightning-5.3.3/src/KapoorLabs_Lightning.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -14,25 +14,27 @@
 licenses/GPL-3
 licenses/LGPL-3
 licenses/MIT
 licenses/MPL-2
 src/KapoorLabs_Lightning.egg-info/PKG-INFO
 src/KapoorLabs_Lightning.egg-info/SOURCES.txt
 src/KapoorLabs_Lightning.egg-info/dependency_links.txt
-src/KapoorLabs_Lightning.egg-info/entry_points.txt
 src/KapoorLabs_Lightning.egg-info/requires.txt
 src/KapoorLabs_Lightning.egg-info/top_level.txt
 src/kapoorlabs_lightning/__init__.py
 src/kapoorlabs_lightning/_version.py
 src/kapoorlabs_lightning/caped.yaml
 src/kapoorlabs_lightning/graph_functions.py
 src/kapoorlabs_lightning/kapoorlabs.yaml
 src/kapoorlabs_lightning/lightning_trainer.py
+src/kapoorlabs_lightning/metrics.py
 src/kapoorlabs_lightning/optimizers.py
+src/kapoorlabs_lightning/pytorch_callbacks.py
 src/kapoorlabs_lightning/pytorch_datasets.py
 src/kapoorlabs_lightning/pytorch_loggers.py
 src/kapoorlabs_lightning/pytorch_losses.py
 src/kapoorlabs_lightning/pytorch_models.py
 src/kapoorlabs_lightning/pytorch_transforms.py
 src/kapoorlabs_lightning/schedulers.py
+src/kapoorlabs_lightning/utils.py
 src/kapoorlabs_lightning/_tests/__init__.py
 src/kapoorlabs_lightning/_tests/test_pytorch_models.py
```

### Comparing `KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/_tests/test_pytorch_models.py` & `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/_tests/test_pytorch_models.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/graph_functions.py` & `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/graph_functions.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/optimizers.py` & `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/optimizers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 from typing import Optional
 
-import torch
+from torch import optim
 from torch.nn.modules.module import Module
 
-__all__ = ["Adam", "SGD", "Rprop"]
+__all__ = ["Adam", "SGD", "Rprop", "RMSprop"]
 
 
 class _Optimizer(Module):
     def __init__(
         self,
         lr=1e-3,
-        betas=(0.9, 0.9999),
+        betas=(0.9, 0.999),
         eps=1e-8,
         momentum=0,
         dampening=0,
         nesterov=False,
         weight_decay=0,
         amsgrad=False,
+        alpha=0.99,
+        centered=False,
         *,
         foreach: Optional[bool] = None,
         maximize: bool = False,
         capturable: bool = False,
         differentiable: bool = False,
         fused: Optional[bool] = None,
         etas=(0.5, 1.2),
         step_sizes=(1e-6, 50)
     ):
         super().__init__()
 
         self.lr = lr
         self.betas = betas
         self.eps = eps
-        self.weight_decay = weight_decay
         self.amsgrad = amsgrad
+        self.alpha = alpha
+        self.weight_decay = weight_decay
+        self.momentum = momentum
         self.foreach = foreach
         self.maximize = maximize
         self.capturable = capturable
         self.differentiable = differentiable
         self.fused = fused
-        self.momentum = momentum
         self.dampening = dampening
         self.nesterov = nesterov
         self.etas = etas
         self.step_sizes = step_sizes
+        self.centered = centered
 
 
 class Adam(_Optimizer):
     def __init__(
         self,
         lr=1e-3,
         betas=(0.9, 0.999),
@@ -70,15 +74,15 @@
             maximize=maximize,
             capturable=capturable,
             differentiable=differentiable,
             fused=fused,
         )
 
     def forward(self, params):
-        return torch.optim.Adam(
+        return optim.Adam(
             params,
             lr=self.lr,
             betas=self.betas,
             eps=self.eps,
             weight_decay=self.weight_decay,
             amsgrad=self.amsgrad,
         )
@@ -105,24 +109,65 @@
             nesterov=nesterov,
             maximize=maximize,
             foreach=foreach,
             differentiable=differentiable,
         )
 
     def forward(self, params):
-        return torch.optim.SGD(
+        return optim.SGD(
             params,
             lr=self.lr,
             momentum=self.momentum,
             dampening=self.dampening,
             weight_decay=self.weight_decay,
             nesterov=self.nesterov,
         )
 
 
+class RMSprop(_Optimizer):
+    def __init__(
+        self,
+        lr=1e-2,
+        alpha=0.99,
+        eps=1e-8,
+        weight_decay=0,
+        momentum=0,
+        centered=False,
+        foreach: Optional[bool] = None,
+        maximize: bool = False,
+        differentiable: bool = False,
+    ):
+
+        super().__init__(
+            lr=lr,
+            alpha=alpha,
+            eps=eps,
+            weight_decay=weight_decay,
+            momentum=momentum,
+            centered=centered,
+            foreach=foreach,
+            maximize=maximize,
+            differentiable=differentiable,
+        )
+
+    def forward(self, params):
+        return optim.RMSprop(
+            params,
+            lr=self.lr,
+            alpha=self.alpha,
+            eps=self.eps,
+            weight_decay=self.weight_decay,
+            momentum=self.momentum,
+            centered=self.centered,
+            foreach=self.foreach,
+            maximize=self.maximize,
+            differentiable=self.differentiable,
+        )
+
+
 class Rprop(_Optimizer):
     def __init__(
         self,
         lr=1e-2,
         etas=(0.5, 1.2),
         step_sizes=(1e-6, 50),
         *,
@@ -134,10 +179,10 @@
         self.etas = etas
         self.step_sizes = step_sizes
         self.foreach = foreach
         self.maximize = maximize
         self.differentiable = differentiable
 
     def forward(self, params):
-        return torch.optim.Rprop(
+        return optim.Rprop(
             params, lr=self.lr, etas=self.etas, step_sizes=self.step_sizes
         )
```

### Comparing `KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/pytorch_datasets.py` & `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,31 @@
         feats = torch.tensor(feats)
 
         serial_number = self.new_df.loc[idx, "serialNumber"]
 
         return image, treatment, feats, serial_number
 
 
+class MitosisDataset(Dataset):
+    def __init__(self, arrays, labels):
+        self.arrays = arrays
+        self.labels = labels
+        self.input_channels = arrays.shape[2]
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+    def __len__(self):
+        return len(self.arrays)
+
+    def __getitem__(self, idx):
+        array = self.arrays[idx]
+        array = torch.tensor(array).permute(1, 0).float().to(self.device)
+        label = torch.tensor(self.labels[idx]).to(self.device)
+        return array, label
+
+
 class GefGapDataset(Dataset):
     def __init__(
         self,
         annotations_file,
         img_dir,
         img_size=100,
         label_col="Treatment",
```

### Comparing `KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/pytorch_loggers.py` & `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_loggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             return self._experiment
         if self._experiment_name:
             self._experiment.set_name(self._experiment_name)
 
     @rank_zero_only
     def log_hyperparams(self, params):
         self.hparams_logged = params
-        self.experiment.log_hparams(params)
+        
 
     @rank_zero_only
     def log_metrics(self, metrics, step):
         if not hasattr(self, "metrics_logged"):
             self.metrics_logged = {}
 
         for key, value in metrics.items():
```

### Comparing `KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/pytorch_losses.py` & `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_losses.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/pytorch_models.py` & `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,228 @@
 import itertools
 
 import numpy as np
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-
+import torch.nn.init as init
+from torch.utils.data import Dataset
 from .graph_functions import get_graph_feature, knn, local_cov, local_maxpool
 
 
+class DenseLayer(nn.Module):
+    """ """
+
+    def __init__(self, input_channels, growth_rate, bottleneck_size, kernel_size):
+        super().__init__()
+        self.use_bottleneck = bottleneck_size > 0
+        self.num_bottleneck_output_filters = growth_rate * bottleneck_size
+        if self.use_bottleneck:
+            self.bn2 = nn.GroupNorm(1, input_channels)
+            self.act2 = nn.ReLU(inplace=True)
+            self.conv2 = nn.Conv1d(
+                input_channels,
+                self.num_bottleneck_output_filters,
+                kernel_size=1,
+                stride=1,
+            )
+        self.bn1 = nn.GroupNorm(1, self.num_bottleneck_output_filters)
+        self.act1 = nn.ReLU(inplace=True)
+        self.conv1 = nn.Conv1d(
+            self.num_bottleneck_output_filters,
+            growth_rate,
+            kernel_size=kernel_size,
+            stride=1,
+            dilation=1,
+            padding=kernel_size // 2,
+        )
+
+    def forward(self, x):
+        if self.use_bottleneck:
+            x = self.bn2(x)
+            x = self.act2(x)
+            x = self.conv2(x)
+        x = self.bn1(x)
+        x = self.act1(x)
+        x = self.conv1(x)
+        return x
+
+
+class DenseBlock(nn.ModuleDict):
+    """ """
+
+    def __init__(
+        self, num_layers, input_channels, growth_rate, kernel_size, bottleneck_size
+    ):
+        super().__init__()
+        self.num_layers = num_layers
+        for i in range(self.num_layers):
+            self.add_module(
+                f"denselayer{i}",
+                DenseLayer(
+                    input_channels + i * growth_rate,
+                    growth_rate,
+                    bottleneck_size,
+                    kernel_size,
+                ),
+            )
+
+    def forward(self, x):
+        layer_outputs = [x]
+        for _, layer in self.items():
+            x = layer(x)
+            layer_outputs.append(x)
+            x = torch.cat(layer_outputs, dim=1)
+        return x
+
+
+class TransitionBlock(nn.Module):
+    """ """
+
+    def __init__(self, input_channels, out_channels):
+        super().__init__()
+        self.bn = nn.GroupNorm(1, input_channels)
+        self.act = nn.ReLU(inplace=True)
+        self.conv = nn.Conv1d(
+            input_channels, out_channels, kernel_size=1, stride=1, dilation=1
+        )
+        self.pool = nn.AvgPool1d(kernel_size=2, stride=2)
+
+    def forward(self, x):
+        x = self.bn(x)
+        x = self.act(x)
+        x = self.conv(x)
+        x = self.pool(x)
+        return x
+
+
+class DenseNet(nn.Module):
+    def __init__(
+        self,
+        input_channels,
+        num_classes,
+        growth_rate: int = 32,
+        block_config: tuple = (6, 12, 24, 16),
+        num_init_features: int = 32,
+        bottleneck_size: int = 4,
+        kernel_size: int = 3,
+    ):
+
+        super().__init__()
+        self._initialize_weights()
+
+        self.features = nn.Sequential(
+            nn.Conv1d(input_channels, num_init_features, kernel_size=1),
+            nn.GroupNorm(1, num_init_features),
+            nn.ReLU(inplace=True),
+            nn.MaxPool1d(kernel_size=1),
+        )
+
+        num_features = num_init_features
+        for i, num_layers in enumerate(block_config):
+            block = DenseBlock(
+                num_layers=num_layers,
+                input_channels=num_features,
+                growth_rate=growth_rate,
+                kernel_size=kernel_size,
+                bottleneck_size=bottleneck_size,
+            )
+            self.features.add_module(f"denseblock{i}", block)
+            num_features = num_features + num_layers * growth_rate
+            if i != len(block_config) - 1:
+                trans = TransitionBlock(
+                    input_channels=num_features, out_channels=num_features // 2
+                )
+                self.features.add_module(f"transition{i}", trans)
+                num_features = num_features // 2
+
+        self.final_bn = nn.GroupNorm(1, num_features)
+        self.final_act = nn.ReLU(inplace=True)
+        self.final_pool = nn.AdaptiveAvgPool1d(1)
+        self.classifier_1 = nn.Linear(num_features, num_classes)
+
+    def _initialize_weights(self):
+        for m in self.modules():
+            if isinstance(m, nn.Conv1d):
+                init.kaiming_normal_(m.weight)
+                if m.bias is not None:
+                    init.constant_(m.bias, 0)
+            elif isinstance(m, nn.BatchNorm1d) or isinstance(m, nn.GroupNorm):
+                init.constant_(m.weight, 1)
+                init.constant_(m.bias, 0)
+            elif isinstance(m, nn.Linear):
+                init.kaiming_normal_(m.weight)
+                init.constant_(m.bias, 0)
+
+    def forward_features(self, x):
+        out = self.features(x)
+        out = self.final_bn(out)
+        out = self.final_act(out)
+        out = self.final_pool(out)
+        return out
+
+    def forward(self, x):
+        features = self.forward_features(x)
+        features = features.squeeze(-1)
+        out_1 = self.classifier_1(features)
+        return out_1
+
+    def reset_classifier(self):
+        self.classifier = nn.Identity()
+
+    def get_classifier(self):
+        return self.classifier
+
+
+class MitosisNet(nn.Module):
+    def __init__(self, input_channels, num_classes):
+
+        super().__init__()
+        self.conv1 = nn.Conv1d(
+            input_channels=input_channels, out_channels=32, kernel_size=3
+        )
+        self.pool1 = nn.MaxPool1d(kernel_size=2)
+        self.conv2 = nn.Conv1d(input_channels=32, out_channels=64, kernel_size=3)
+        self.pool2 = nn.MaxPool1d(kernel_size=2)
+
+        self.global_pooling = nn.AdaptiveAvgPool1d(1)
+        self.fc = nn.Linear(64, num_classes)
+
+    def forward(self, x):
+        x = self.pool1(nn.functional.relu(self.conv1(x)))
+        x = self.pool2(nn.functional.relu(self.conv2(x)))
+        x = self.global_pooling(x).squeeze()
+        x = self.fc(x)
+        return x
+
+
+class MitosisDataset(Dataset):
+    def __init__(self, arrays, labels):
+        self.arrays = arrays
+        self.labels = labels
+        self.input_channels = arrays.shape[2]
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
+    def __len__(self):
+        return len(self.arrays)
+
+    def __getitem__(self, idx):
+        array = self.arrays[idx]
+        array = torch.tensor(array).permute(1, 0).float().to(self.device)
+        label = torch.tensor(self.labels[idx]).to(self.device)
+        return array, label
+
+
 class ClusteringLayer(nn.Module):
     def __init__(self, num_features=10, num_clusters=10, alpha=1.0):
         super().__init__()
         self.num_features = num_features
         self.num_clusters = num_clusters
         self.alpha = alpha
-        self.weight = nn.Parameter(
-            torch.Tensor(self.num_clusters, self.num_features)
-        )
+        self.weight = nn.Parameter(torch.Tensor(self.num_clusters, self.num_features))
         self.weight = nn.init.xavier_uniform_(self.weight)
 
     def forward(self, x):
         x = x.unsqueeze(1) - self.weight
         x = torch.mul(x, x)
         x = torch.sum(x, dim=2)
         x = 1.0 + (x / self.alpha)
@@ -69,23 +271,19 @@
             "foldingnet",
             "foldingnetbasic",
         ], "Please select an decoder type from either foldingnet."
 
         self.encoder_type = encoder_type.lower()
         self.decoder_type = decoder_type.lower()
         if self.encoder_type == "dgcnn":
-            self.encoder = DGCNNEncoder(
-                num_features=self.num_features, k=self.k
-            )
+            self.encoder = DGCNNEncoder(num_features=self.num_features, k=self.k)
         # elif self.encoder_type == "dgcnn_orig":
         #     self.encoder = DGCNN(num_features=self.num_features, k=self.k)
         else:
-            self.encoder = FoldNetEncoder(
-                num_features=self.num_features, k=self.k
-            )
+            self.encoder = FoldNetEncoder(num_features=self.num_features, k=self.k)
 
         if self.decoder_type == "foldingnet":
             self.decoder = FoldNetDecoder(
                 num_features=self.num_features,
                 shape=self.shape,
                 sphere_path=self.sphere_path,
                 gaussian_path=self.gaussian_path,
@@ -174,17 +372,15 @@
             )
 
         if shape == "plane":
             # make grid
             range_x = torch.linspace(-std, std, 45)
             range_y = torch.linspace(-std, std, 45)
             x_coor, y_coor = torch.meshgrid(range_x, range_y, indexing="ij")
-            self.grid = (
-                torch.stack([x_coor, y_coor], axis=-1).float().reshape(-1, 2)
-            )
+            self.grid = torch.stack([x_coor, y_coor], axis=-1).float().reshape(-1, 2)
         elif shape == "sphere":
             self.grid = torch.tensor(np.load(sphere_path))
         elif self.shape == "gaussian":
             self.grid = torch.tensor(np.load(gaussian_path))
 
         # initialise folding module
         self.folding = FoldingModule()
@@ -520,14 +716,16 @@
         """
         batch_size = input.size(0)
         out = input.view(batch_size, -1)
         return out
 
 
 __all__ = [
+    "DenseNet",
+    "MitosisNet",
     "CloudAutoEncoder",
     "DGCNNEncoder",
     "FoldNetEncoder",
     "FoldNetDecoder",
     "FoldingNetBasicDecoder",
     "Flatten",
     "FoldingModule",
```

### Comparing `KapoorLabs-Lightning-5.3.2/src/kapoorlabs_lightning/pytorch_transforms.py` & `kapoorlabs_lightning-5.3.3/src/kapoorlabs_lightning/pytorch_transforms.py`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/tox.ini` & `kapoorlabs_lightning-5.3.3/tox.ini`

 * *Files identical despite different names*

### Comparing `KapoorLabs-Lightning-5.3.2/update_version.py` & `kapoorlabs_lightning-5.3.3/update_version.py`

 * *Files identical despite different names*

