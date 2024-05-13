# Comparing `tmp/biomero-1.8.0.tar.gz` & `tmp/biomero-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/biomero/biomero/dist/.tmp-dorewbl_/biomero-1.8.0.tar", last modified: Thu Apr  4 16:17:46 2024, max compression
+gzip compressed data, was "/home/runner/work/biomero/biomero/dist/.tmp-2z7ckeqa/biomero-1.9.0.tar", last modified: Mon May 13 13:20:09 2024, max compression
```

## Comparing `biomero-1.8.0.tar` & `biomero-1.9.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-04 16:17:39.000000 biomero-1.8.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-04 16:17:39.000000 biomero-1.8.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-04 16:17:39.000000 biomero-1.8.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-04 16:17:39.000000 biomero-1.8.0/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-04 16:17:39.000000 biomero-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-04-04 16:17:39.000000 biomero-1.8.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 16:17:39.000000 biomero-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 16:17:39.000000 biomero-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-04 16:17:46.000000 biomero-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    38811 2024-04-04 16:17:39.000000 biomero-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-04 16:17:39.000000 biomero-1.8.0/biomero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-04 16:17:39.000000 biomero-1.8.0/biomero/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    79394 2024-04-04 16:17:39.000000 biomero-1.8.0/biomero/slurm_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 16:17:46.000000 biomero-1.8.0/biomero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/omero_slurm_client.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/readme_link.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-04 16:17:39.000000 biomero-1.8.0/docs/tutorial_link.md
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-04-04 16:17:39.000000 biomero-1.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/convert_job_array.sh
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/convert_zarr_to_tiff.def
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/convert_zarr_to_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/example.config
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/job_template.sh
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/pull_images.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/slurm-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/resources/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/resources/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (127)   315936 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/Cells.tif
--rw-r--r--   0 runner    (1001) docker     (127)   315102 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/cellexpansion.png
--rw-r--r--   0 runner    (1001) docker     (127)    83900 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/gc_allow_ssh.PNG
--rw-r--r--   0 runner    (1001) docker     (127)   200759 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/nuclei_labels.png
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/webclient_init_env.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/webclient_init_env_done.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/webclient_run_cellpose.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/images/webclient_run_workflow.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/tutorial_Azure_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/tutorial_GoogleCloud_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/tutorial_cellexpansion.md
--rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/tutorial_cellprofiler.md
--rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-04-04 16:17:39.000000 biomero-1.8.0/resources/tutorials/tutorial_local_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:17:46.000000 biomero-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:39.000000 biomero-1.8.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:46.000000 biomero-1.8.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:17:39.000000 biomero-1.8.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45207 2024-04-04 16:17:39.000000 biomero-1.8.0/tests/unit/test_slurm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 13:20:03.000000 biomero-1.9.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-13 13:20:03.000000 biomero-1.9.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-13 13:20:03.000000 biomero-1.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-13 13:20:03.000000 biomero-1.9.0/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-13 13:20:03.000000 biomero-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-13 13:20:03.000000 biomero-1.9.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 13:20:03.000000 biomero-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 13:20:03.000000 biomero-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    53104 2024-05-13 13:20:09.000000 biomero-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39089 2024-05-13 13:20:03.000000 biomero-1.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 13:20:03.000000 biomero-1.9.0/biomero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-13 13:20:03.000000 biomero-1.9.0/biomero/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82826 2024-05-13 13:20:03.000000 biomero-1.9.0/biomero/slurm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    53104 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/omero_slurm_client.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/readme_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/tutorial_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-13 13:20:03.000000 biomero-1.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/convert_job_array.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/convert_zarr_to_tiff.def
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/convert_zarr_to_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/example.config
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/job_template.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/pull_images.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/slurm-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/resources/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/resources/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   315936 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/Cells.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   315102 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/cellexpansion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83900 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/gc_allow_ssh.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)   200759 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/nuclei_labels.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/webclient_init_env.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/webclient_init_env_done.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/webclient_run_cellpose.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/webclient_run_workflow.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/tutorial_Azure_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/tutorial_GoogleCloud_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/tutorial_cellexpansion.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/tutorial_cellprofiler.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/tutorial_local_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:20:09.000000 biomero-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:03.000000 biomero-1.9.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:03.000000 biomero-1.9.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45395 2024-05-13 13:20:03.000000 biomero-1.9.0/tests/unit/test_slurm_client.py
```

### Comparing `biomero-1.8.0/.github/workflows/python-package.yml` & `biomero-1.9.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/.github/workflows/python-publish.yml` & `biomero-1.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/.github/workflows/sphinx.yml` & `biomero-1.9.0/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/.gitignore` & `biomero-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/CITATION.cff` & `biomero-1.9.0/CITATION.cff`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/LICENSE` & `biomero-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/PKG-INFO` & `biomero-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomero
-Version: 1.8.0
+Version: 1.9.0
 Summary: A python library for easy connecting between OMERO (jobs) and a Slurm cluster
 Author: Core Facility - Cellular Imaging
 Author-email: Torec Luik <t.t.luik@amsterdamumc.nl>, cellularimaging@amsterdamumc.nl
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -320,16 +320,18 @@
 
     - Congratulations! Now the servers are connected. Next, we make sure to setup the connection between OMERO and Slurm.
 
 3. At this point, ensure that the `slurm-config.ini` file is correctly configured with the necessary SSH and Slurm settings, including the host, data path, images path, and model details. Customize the configuration according to the specific Slurm cluster setup. We provide an example in the [resources](./resources/slurm-config.ini) section. To read it automatically, place this `ini` file in one of the following locations (on the OMERO `processor` server):
     - `/etc/slurm-config.ini`
     - `~/slurm-config.ini`
 
+    *Note*: Make sure to place the `slurm-config.ini` in the target folder at build time of your docker container instead of mounting it at runtime. This is because the library reads the config file at import time, and if it is not found, it will not work.
+
 4. Install OMERO scripts from [OMERO Slurm Scripts](https://github.com/NL-BioImaging/biomero-scripts), e.g. 
-    - `cd OMERO_DIST/lib/scripts`
+    - `cd /opt/omero/server/OMERO.server/lib/scripts`
     - `git clone https://github.com/NL-BioImaging/biomero-scripts.git slurm`
 
 !!*NOTE*: Do not install [Example Minimal Slurm Script](https://github.com/NL-BioImaging/biomero-scripts/blob/master/Example_Minimal_Slurm_Script.py) if you do not trust your users with your Slurm cluster. It has literal Command Injection for the SSH user as a **FEATURE**. 
 
 5. Install [BIOMERO Scripts](https://github.com/NL-BioImaging/biomero-scripts/) requirements, e.g.
     - `python3 -m pip install ezomero==1.1.1 tifffile==2020.9.3` 
     - the [OMERO CLI Zarr plugin](https://github.com/ome/omero-cli-zarr), e.g.
```

### Comparing `biomero-1.8.0/README.md` & `biomero-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -97,16 +97,18 @@
 
     - Congratulations! Now the servers are connected. Next, we make sure to setup the connection between OMERO and Slurm.
 
 3. At this point, ensure that the `slurm-config.ini` file is correctly configured with the necessary SSH and Slurm settings, including the host, data path, images path, and model details. Customize the configuration according to the specific Slurm cluster setup. We provide an example in the [resources](./resources/slurm-config.ini) section. To read it automatically, place this `ini` file in one of the following locations (on the OMERO `processor` server):
     - `/etc/slurm-config.ini`
     - `~/slurm-config.ini`
 
+    *Note*: Make sure to place the `slurm-config.ini` in the target folder at build time of your docker container instead of mounting it at runtime. This is because the library reads the config file at import time, and if it is not found, it will not work.
+
 4. Install OMERO scripts from [OMERO Slurm Scripts](https://github.com/NL-BioImaging/biomero-scripts), e.g. 
-    - `cd OMERO_DIST/lib/scripts`
+    - `cd /opt/omero/server/OMERO.server/lib/scripts`
     - `git clone https://github.com/NL-BioImaging/biomero-scripts.git slurm`
 
 !!*NOTE*: Do not install [Example Minimal Slurm Script](https://github.com/NL-BioImaging/biomero-scripts/blob/master/Example_Minimal_Slurm_Script.py) if you do not trust your users with your Slurm cluster. It has literal Command Injection for the SSH user as a **FEATURE**. 
 
 5. Install [BIOMERO Scripts](https://github.com/NL-BioImaging/biomero-scripts/) requirements, e.g.
     - `python3 -m pip install ezomero==1.1.1 tifffile==2020.9.3` 
     - the [OMERO CLI Zarr plugin](https://github.com/ome/omero-cli-zarr), e.g.
```

### Comparing `biomero-1.8.0/biomero/slurm_client.py` & `biomero-1.9.0/biomero/slurm_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,4899 +65,5113 @@
 00000400: 706c 6174 650a 6672 6f6d 2069 6d70 6f72  plate.from impor
 00000410: 746c 6962 5f72 6573 6f75 7263 6573 2069  tlib_resources i
 00000420: 6d70 6f72 7420 6669 6c65 730a 696d 706f  mport files.impo
 00000430: 7274 2069 6f0a 696d 706f 7274 206f 730a  rt io.import os.
 00000440: 0a6c 6f67 6765 7220 3d20 6c6f 6767 696e  .logger = loggin
 00000450: 672e 6765 744c 6f67 6765 7228 5f5f 6e61  g.getLogger(__na
 00000460: 6d65 5f5f 290a 0a0a 636c 6173 7320 536c  me__)...class Sl
-00000470: 7572 6d4a 6f62 3a0a 2020 2020 6465 6620  urmJob:.    def 
-00000480: 5f5f 696e 6974 5f5f 2873 656c 662c 0a20  __init__(self,. 
-00000490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004a0: 7375 626d 6974 5f72 6573 756c 743a 2052  submit_result: R
-000004b0: 6573 756c 742c 0a20 2020 2020 2020 2020  esult,.         
-000004c0: 2020 2020 2020 2020 6a6f 625f 6964 3a20          job_id: 
-000004d0: 696e 7429 3a0a 2020 2020 2020 2020 2222  int):.        ""
-000004e0: 220a 2020 2020 2020 2020 496e 6974 6961  ".        Initia
-000004f0: 6c69 7a65 2061 2053 6c75 726d 4a6f 6220  lize a SlurmJob 
-00000500: 696e 7374 616e 6365 2e0a 0a20 2020 2020  instance...     
-00000510: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00000520: 2020 2020 2073 7562 6d69 745f 7265 7375       submit_resu
-00000530: 6c74 2028 5265 7375 6c74 293a 2054 6865  lt (Result): The
-00000540: 2072 6573 756c 7420 6f66 2073 7562 6d69   result of submi
-00000550: 7474 696e 6720 7468 6520 6a6f 622e 0a20  tting the job.. 
-00000560: 2020 2020 2020 2020 2020 206a 6f62 5f69             job_i
-00000570: 6420 2869 6e74 293a 2054 6865 2053 6c75  d (int): The Slu
-00000580: 726d 206a 6f62 2049 442e 0a20 2020 2020  rm job ID..     
-00000590: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-000005a0: 656c 662e 6a6f 625f 6964 203d 206a 6f62  elf.job_id = job
-000005b0: 5f69 640a 2020 2020 2020 2020 7365 6c66  _id.        self
-000005c0: 2e73 7562 6d69 745f 7265 7375 6c74 203d  .submit_result =
-000005d0: 2073 7562 6d69 745f 7265 7375 6c74 0a20   submit_result. 
-000005e0: 2020 2020 2020 2073 656c 662e 6f6b 203d         self.ok =
-000005f0: 2073 656c 662e 7375 626d 6974 5f72 6573   self.submit_res
-00000600: 756c 742e 6f6b 0a20 2020 2020 2020 2073  ult.ok.        s
-00000610: 656c 662e 6a6f 625f 7374 6174 6520 3d20  elf.job_state = 
-00000620: 4e6f 6e65 0a0a 2020 2020 6465 6620 7761  None..    def wa
-00000630: 6974 5f66 6f72 5f63 6f6d 706c 6574 696f  it_for_completio
-00000640: 6e28 7365 6c66 2c20 736c 7572 6d43 6c69  n(self, slurmCli
-00000650: 656e 742c 206f 6d65 726f 436f 6e6e 2920  ent, omeroConn) 
-00000660: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-00000670: 2222 220a 2020 2020 2020 2020 5761 6974  """.        Wait
-00000680: 2066 6f72 2074 6865 2053 6c75 726d 206a   for the Slurm j
-00000690: 6f62 2074 6f20 7265 6163 6820 636f 6d70  ob to reach comp
-000006a0: 6c65 7469 6f6e 2c20 6361 6e63 656c 6c61  letion, cancella
-000006b0: 7469 6f6e 2c20 6661 696c 7572 652c 206f  tion, failure, o
-000006c0: 7220 7469 6d65 6f75 742e 0a0a 2020 2020  r timeout...    
-000006d0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000006e0: 2020 2020 2020 736c 7572 6d43 6c69 656e        slurmClien
-000006f0: 743a 2054 6865 2053 6c75 726d 2063 6c69  t: The Slurm cli
-00000700: 656e 742e 0a20 2020 2020 2020 2020 2020  ent..           
-00000710: 206f 6d65 726f 436f 6e6e 3a20 5468 6520   omeroConn: The 
-00000720: 4f4d 4552 4f20 636f 6e6e 6563 7469 6f6e  OMERO connection
-00000730: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00000740: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00000750: 7374 723a 2054 6865 2066 696e 616c 2073  str: The final s
-00000760: 7461 7465 206f 6620 7468 6520 536c 7572  tate of the Slur
-00000770: 6d20 6a6f 622e 0a20 2020 2020 2020 2022  m job..        "
-00000780: 2222 0a20 2020 2020 2020 2077 6869 6c65  "".        while
-00000790: 2073 656c 662e 6a6f 625f 7374 6174 6520   self.job_state 
-000007a0: 6e6f 7420 696e 2028 2246 4149 4c45 4422  not in ("FAILED"
-000007b0: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
-000007c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007d0: 2020 2020 2020 2020 2243 4f4d 504c 4554          "COMPLET
-000007e0: 4544 222c 200a 2020 2020 2020 2020 2020  ED", .          
-000007f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000800: 2020 2020 2020 2020 2020 2022 4341 4e43             "CANC
-00000810: 454c 4c45 4422 2c0a 2020 2020 2020 2020  ELLED",.        
-00000820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000830: 2020 2020 2020 2020 2020 2020 2022 5449               "TI
-00000840: 4d45 4f55 5422 2c0a 2020 2020 2020 2020  MEOUT",.        
-00000850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000860: 2020 2020 2020 2020 2020 2020 2022 4641               "FA
-00000870: 494c 4544 2b22 2c20 0a20 2020 2020 2020  ILED+", .       
-00000880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000890: 2020 2020 2020 2020 2020 2020 2020 2243                "C
-000008a0: 4f4d 504c 4554 4544 2b22 2c20 0a20 2020  OMPLETED+", .   
-000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000008d0: 2020 2243 414e 4345 4c4c 4544 2b22 2c0a    "CANCELLED+",.
-000008e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000470: 7572 6d4a 6f62 3a0a 2020 2020 2222 2252  urmJob:.    """R
+00000480: 6570 7265 7365 6e74 7320 6120 6a6f 6220  epresents a job 
+00000490: 7375 626d 6974 7465 6420 746f 2061 2053  submitted to a S
+000004a0: 6c75 726d 2063 6c75 7374 6572 2e0a 0a20  lurm cluster... 
+000004b0: 2020 2054 6869 7320 636c 6173 7320 656e     This class en
+000004c0: 6361 7073 756c 6174 6573 2069 6e66 6f72  capsulates infor
+000004d0: 6d61 7469 6f6e 2061 6e64 206d 6574 686f  mation and metho
+000004e0: 6473 2072 656c 6174 6564 2074 6f20 6d61  ds related to ma
+000004f0: 6e61 6769 6e67 2061 206a 6f62 0a20 2020  naging a job.   
+00000500: 2073 7562 6d69 7474 6564 2074 6f20 6120   submitted to a 
+00000510: 536c 7572 6d20 636c 7573 7465 722e 2049  Slurm cluster. I
+00000520: 7420 7072 6f76 6964 6573 2066 756e 6374  t provides funct
+00000530: 696f 6e61 6c69 7479 2074 6f20 6d6f 6e69  ionality to moni
+00000540: 746f 7220 7468 650a 2020 2020 6a6f 6227  tor the.    job'
+00000550: 7320 7374 6174 652c 2077 6169 7420 666f  s state, wait fo
+00000560: 7220 636f 6d70 6c65 7469 6f6e 2c20 616e  r completion, an
+00000570: 6420 7065 7266 6f72 6d20 636c 6561 6e75  d perform cleanu
+00000580: 7020 6f70 6572 6174 696f 6e73 2e0a 0a20  p operations... 
+00000590: 2020 2041 7474 7269 6275 7465 733a 0a20     Attributes:. 
+000005a0: 2020 2020 2020 206a 6f62 5f69 6420 2869         job_id (i
+000005b0: 6e74 293a 2054 6865 2049 4420 6f66 2074  nt): The ID of t
+000005c0: 6865 2053 6c75 726d 206a 6f62 2e0a 2020  he Slurm job..  
+000005d0: 2020 2020 2020 7375 626d 6974 5f72 6573        submit_res
+000005e0: 756c 7420 2852 6573 756c 7429 3a20 5468  ult (Result): Th
+000005f0: 6520 7265 7375 6c74 206f 6620 7375 626d  e result of subm
+00000600: 6974 7469 6e67 2074 6865 206a 6f62 2e0a  itting the job..
+00000610: 2020 2020 2020 2020 6f6b 2028 626f 6f6c          ok (bool
+00000620: 293a 2049 6e64 6963 6174 6573 2077 6865  ): Indicates whe
+00000630: 7468 6572 2074 6865 206a 6f62 2073 7562  ther the job sub
+00000640: 6d69 7373 696f 6e20 7761 7320 7375 6363  mission was succ
+00000650: 6573 7366 756c 2e0a 2020 2020 2020 2020  essful..        
+00000660: 6a6f 625f 7374 6174 6520 2873 7472 293a  job_state (str):
+00000670: 2054 6865 2063 7572 7265 6e74 2073 7461   The current sta
+00000680: 7465 206f 6620 7468 6520 536c 7572 6d20  te of the Slurm 
+00000690: 6a6f 622e 0a20 2020 2020 2020 2065 7272  job..        err
+000006a0: 6f72 5f6d 6573 7361 6765 2028 7374 7229  or_message (str)
+000006b0: 3a20 5468 6520 6572 726f 7220 6d65 7373  : The error mess
+000006c0: 6167 652c 2069 6620 616e 792e 0a0a 2020  age, if any...  
+000006d0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+000006e0: 7375 626d 6974 5f72 6573 756c 7420 2852  submit_result (R
+000006f0: 6573 756c 7429 3a20 5468 6520 7265 7375  esult): The resu
+00000700: 6c74 206f 6620 7375 626d 6974 7469 6e67  lt of submitting
+00000710: 2074 6865 206a 6f62 2e0a 2020 2020 2020   the job..      
+00000720: 2020 6a6f 625f 6964 2028 696e 7429 3a20    job_id (int): 
+00000730: 5468 6520 536c 7572 6d20 6a6f 6220 4944  The Slurm job ID
+00000740: 2e0a 0a20 2020 2045 7861 6d70 6c65 3a0a  ...    Example:.
+00000750: 2020 2020 2020 2020 2320 5375 626d 6974          # Submit
+00000760: 2073 6f6d 6520 6a6f 6220 7769 7468 2074   some job with t
+00000770: 6865 2053 6c75 726d 436c 6965 6e74 0a20  he SlurmClient. 
+00000780: 2020 2020 2020 2073 7562 6d69 745f 7265         submit_re
+00000790: 7375 6c74 2c20 6a6f 625f 6964 203d 2073  sult, job_id = s
+000007a0: 6c75 726d 436c 6965 6e74 2e72 756e 5f77  lurmClient.run_w
+000007b0: 6f72 6b66 6c6f 7728 0a20 2020 2020 2020  orkflow(.       
+000007c0: 2020 2020 2077 6f72 6b66 6c6f 775f 6e61       workflow_na
+000007d0: 6d65 2c20 776f 726b 666c 6f77 5f76 6572  me, workflow_ver
+000007e0: 7369 6f6e 2c20 696e 7075 745f 6461 7461  sion, input_data
+000007f0: 2c20 656d 6169 6c2c 2074 696d 652c 202a  , email, time, *
+00000800: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
+00000810: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
+00000820: 4372 6561 7465 2061 2053 6c75 726d 4a6f  Create a SlurmJo
+00000830: 6220 696e 7374 616e 6365 0a20 2020 2020  b instance.     
+00000840: 2020 2073 6c75 726d 4a6f 6220 3d20 536c     slurmJob = Sl
+00000850: 7572 6d4a 6f62 2873 7562 6d69 745f 7265  urmJob(submit_re
+00000860: 7375 6c74 2c20 6a6f 625f 6964 290a 0a20  sult, job_id).. 
+00000870: 2020 2020 2020 2069 6620 6e6f 7420 736c         if not sl
+00000880: 7572 6d4a 6f62 2e6f 6b3a 0a20 2020 2020  urmJob.ok:.     
+00000890: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
+000008a0: 726e 696e 6728 6622 4572 726f 7220 7769  rning(f"Error wi
+000008b0: 7468 206a 6f62 3a20 7b73 6c75 726d 4a6f  th job: {slurmJo
+000008c0: 622e 6765 745f 6572 726f 7228 297d 2229  b.get_error()}")
+000008d0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000008e0: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
 000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000900: 2020 2020 2022 5449 4d45 4f55 542b 2229       "TIMEOUT+")
-00000910: 3a0a 2020 2020 2020 2020 2020 2020 6a6f  :.            jo
-00000920: 625f 7374 6174 7573 5f64 6963 742c 2070  b_status_dict, p
-00000930: 6f6c 6c5f 7265 7375 6c74 203d 2073 6c75  oll_result = slu
-00000940: 726d 436c 6965 6e74 2e63 6865 636b 5f6a  rmClient.check_j
-00000950: 6f62 5f73 7461 7475 7328 0a20 2020 2020  ob_status(.     
-00000960: 2020 2020 2020 2020 2020 205b 7365 6c66             [self
-00000970: 2e6a 6f62 5f69 645d 290a 2020 2020 2020  .job_id]).      
-00000980: 2020 2020 2020 6966 206e 6f74 2070 6f6c        if not pol
-00000990: 6c5f 7265 7375 6c74 2e6f 6b3a 0a20 2020  l_result.ok:.   
-000009a0: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-000009b0: 6765 722e 7761 726e 696e 6728 0a20 2020  ger.warning(.   
+00000900: 736c 7572 6d4a 6f62 2e77 6169 745f 666f  slurmJob.wait_fo
+00000910: 725f 636f 6d70 6c65 7469 6f6e 2873 6c75  r_completion(slu
+00000920: 726d 436c 6965 6e74 2c20 636f 6e6e 290a  rmClient, conn).
+00000930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000940: 6966 206e 6f74 2073 6c75 726d 4a6f 622e  if not slurmJob.
+00000950: 636f 6d70 6c65 7465 6428 293a 0a20 2020  completed():.   
+00000960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000970: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
+00000980: 2866 224a 6f62 2069 7320 6e6f 7420 636f  (f"Job is not co
+00000990: 6d70 6c65 7465 643a 207b 736c 7572 6d4a  mpleted: {slurmJ
+000009a0: 6f62 7d22 290a 2020 2020 2020 2020 2020  ob}").          
+000009b0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 000009c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000009d0: 2066 2245 7272 6f72 2063 6865 636b 696e   f"Error checkin
-000009e0: 6720 6a6f 6220 7374 6174 7573 3a7b 706f  g job status:{po
-000009f0: 6c6c 5f72 6573 756c 742e 7374 6465 7272  ll_result.stderr
-00000a00: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-00000a10: 2020 2020 7365 6c66 2e6a 6f62 5f73 7461      self.job_sta
-00000a20: 7465 203d 2022 4641 494c 4544 220a 2020  te = "FAILED".  
-00000a30: 2020 2020 2020 2020 2020 7365 6c66 2e6a            self.j
-00000a40: 6f62 5f73 7461 7465 203d 206a 6f62 5f73  ob_state = job_s
-00000a50: 7461 7475 735f 6469 6374 5b73 656c 662e  tatus_dict[self.
-00000a60: 6a6f 625f 6964 5d0a 2020 2020 2020 2020  job_id].        
-00000a70: 2020 2020 2320 7761 6974 2066 6f72 2031      # wait for 1
-00000a80: 3020 7365 636f 6e64 7320 6265 666f 7265  0 seconds before
-00000a90: 2063 6865 636b 696e 6720 6167 6169 6e0a   checking again.
-00000aa0: 2020 2020 2020 2020 2020 2020 6f6d 6572              omer
-00000ab0: 6f43 6f6e 6e2e 6b65 6570 416c 6976 6528  oConn.keepAlive(
-00000ac0: 2920 2023 206b 6565 7020 7468 6520 4f4d  )  # keep the OM
-00000ad0: 4552 4f20 636f 6e6e 6563 7469 6f6e 2061  ERO connection a
-00000ae0: 6c69 7665 0a20 2020 2020 2020 2020 2020  live.           
-00000af0: 2074 696d 6573 6c65 6570 2e73 6c65 6570   timesleep.sleep
-00000b00: 2831 3029 0a20 2020 2020 2020 206c 6f67  (10).        log
-00000b10: 6765 722e 696e 666f 2866 224a 6f62 207b  ger.info(f"Job {
-00000b20: 7365 6c66 2e6a 6f62 5f69 647d 2066 696e  self.job_id} fin
-00000b30: 6973 6865 643a 207b 7365 6c66 2e6a 6f62  ished: {self.job
-00000b40: 5f73 7461 7465 7d22 290a 2020 2020 2020  _state}").      
-00000b50: 2020 6c6f 6767 6572 2e69 6e66 6f28 0a20    logger.info(. 
-00000b60: 2020 2020 2020 2020 2020 2066 2259 6f75             f"You
-00000b70: 2063 616e 2067 6574 2074 6865 206c 6f67   can get the log
-00000b80: 6669 6c65 2075 7369 6e67 2060 536c 7572  file using `Slur
-00000b90: 6d20 4765 7420 5570 6461 7465 6020 6f6e  m Get Update` on
-00000ba0: 206a 6f62 207b 7365 6c66 2e6a 6f62 5f69   job {self.job_i
-00000bb0: 647d 2229 0a20 2020 2020 2020 2072 6574  d}").        ret
-00000bc0: 7572 6e20 7365 6c66 2e6a 6f62 5f73 7461  urn self.job_sta
-00000bd0: 7465 0a20 2020 200a 2020 2020 6465 6620  te.    .    def 
-00000be0: 636c 6561 6e75 7028 7365 6c66 2c20 736c  cleanup(self, sl
-00000bf0: 7572 6d43 6c69 656e 7429 202d 3e20 5265  urmClient) -> Re
-00000c00: 7375 6c74 3a0a 2020 2020 2020 2020 2222  sult:.        ""
-00000c10: 220a 2020 2020 2020 2020 436c 6561 6e75  ".        Cleanu
-00000c20: 7020 7265 6d61 696e 696e 6720 6c6f 6720  p remaining log 
-00000c30: 6669 6c65 732e 0a0a 2020 2020 2020 2020  files...        
-00000c40: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00000c50: 2020 736c 7572 6d43 6c69 656e 743a 2054    slurmClient: T
-00000c60: 6865 2053 6c75 726d 2063 6c69 656e 742e  he Slurm client.
-00000c70: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00000c80: 733a 0a20 2020 2020 2020 2020 2020 2052  s:.            R
-00000c90: 6573 756c 743a 2054 6865 2072 6573 756c  esult: The resul
-00000ca0: 7420 6f66 2074 6865 2063 6c65 616e 7570  t of the cleanup
-00000cb0: 206f 7065 7261 7469 6f6e 2e0a 2020 2020   operation..    
-00000cc0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00000cd0: 7265 7475 726e 2073 6c75 726d 436c 6965  return slurmClie
-00000ce0: 6e74 2e63 6c65 616e 7570 5f74 6d70 5f66  nt.cleanup_tmp_f
-00000cf0: 696c 6573 2873 656c 662e 6a6f 625f 6964  iles(self.job_id
-00000d00: 290a 0a20 2020 2064 6566 2063 6f6d 706c  )..    def compl
-00000d10: 6574 6564 2873 656c 6629 3a0a 2020 2020  eted(self):.    
-00000d20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00000d30: 4368 6563 6b20 6966 2074 6865 2053 6c75  Check if the Slu
-00000d40: 726d 206a 6f62 2068 6173 2063 6f6d 706c  rm job has compl
-00000d50: 6574 6564 2073 7563 6365 7373 6675 6c6c  eted successfull
-00000d60: 792e 0a0a 2020 2020 2020 2020 5265 7475  y...        Retu
-00000d70: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00000d80: 2062 6f6f 6c3a 2054 7275 6520 6966 2074   bool: True if t
-00000d90: 6865 206a 6f62 2068 6173 2063 6f6d 706c  he job has compl
-00000da0: 6574 6564 3b20 4661 6c73 6520 6f74 6865  eted; False othe
-00000db0: 7277 6973 652e 0a20 2020 2020 2020 2022  rwise..        "
-00000dc0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00000dd0: 6e20 7365 6c66 2e6a 6f62 5f73 7461 7465  n self.job_state
-00000de0: 203d 3d20 2243 4f4d 504c 4554 4544 220a   == "COMPLETED".
-00000df0: 0a20 2020 2064 6566 205f 5f73 7472 5f5f  .    def __str__
-00000e00: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00000e10: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
-00000e20: 726e 2061 2073 7472 696e 6720 7265 7072  rn a string repr
-00000e30: 6573 656e 7461 7469 6f6e 206f 6620 7468  esentation of th
-00000e40: 6520 536c 7572 6d4a 6f62 2069 6e73 7461  e SlurmJob insta
-00000e50: 6e63 652e 0a0a 2020 2020 2020 2020 5265  nce...        Re
-00000e60: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00000e70: 2020 2073 7472 3a20 5374 7269 6e67 2072     str: String r
-00000e80: 6570 7265 7365 6e74 6174 696f 6e2e 0a20  epresentation.. 
-00000e90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00000ea0: 2020 2070 726f 7065 7274 6965 7320 3d20     properties = 
-00000eb0: 272c 2027 2e6a 6f69 6e28 0a20 2020 2020  ', '.join(.     
-00000ec0: 2020 2020 2020 2066 227b 6b65 797d 3d7b         f"{key}={
-00000ed0: 7661 6c75 657d 2220 666f 7220 6b65 792c  value}" for key,
-00000ee0: 2076 616c 7565 2069 6e20 7365 6c66 2e5f   value in self._
-00000ef0: 5f64 6963 745f 5f2e 6974 656d 7328 2929  _dict__.items())
-00000f00: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000f10: 6622 536c 7572 6d4a 6f62 287b 7072 6f70  f"SlurmJob({prop
-00000f20: 6572 7469 6573 7d29 220a 0a0a 636c 6173  erties})"...clas
-00000f30: 7320 536c 7572 6d43 6c69 656e 7428 436f  s SlurmClient(Co
-00000f40: 6e6e 6563 7469 6f6e 293a 0a20 2020 2022  nnection):.    "
-00000f50: 2222 4120 636c 6965 6e74 2066 6f72 2063  ""A client for c
-00000f60: 6f6e 6e65 6374 696e 6720 746f 2061 6e64  onnecting to and
-00000f70: 2069 6e74 6572 6163 7469 6e67 2077 6974   interacting wit
-00000f80: 6820 6120 536c 7572 6d20 636c 7573 7465  h a Slurm cluste
-00000f90: 7220 6f76 6572 0a20 2020 2053 5348 2e0a  r over.    SSH..
-00000fa0: 0a20 2020 2054 6869 7320 636c 6173 7320  .    This class 
-00000fb0: 6578 7465 6e64 7320 7468 6520 436f 6e6e  extends the Conn
-00000fc0: 6563 7469 6f6e 2063 6c61 7373 2c20 6164  ection class, ad
-00000fd0: 6469 6e67 206d 6574 686f 6473 2061 6e64  ding methods and
-00000fe0: 0a20 2020 2061 7474 7269 6275 7465 7320  .    attributes 
-00000ff0: 7370 6563 6966 6963 2074 6f20 776f 726b  specific to work
-00001000: 696e 6720 7769 7468 2053 6c75 726d 2e0a  ing with Slurm..
-00001010: 0a20 2020 2053 6c75 726d 436c 6965 6e74  .    SlurmClient
-00001020: 2061 6363 6570 7473 2074 6865 2073 616d   accepts the sam
-00001030: 6520 6172 6775 6d65 6e74 7320 6173 2043  e arguments as C
-00001040: 6f6e 6e65 6374 696f 6e2e 2042 656c 6f77  onnection. Below
-00001050: 206f 6e6c 790a 2020 2020 6d65 6e74 696f   only.    mentio
-00001060: 6e73 2074 6865 2061 6464 6564 206f 6e65  ns the added one
-00001070: 733a 0a0a 2020 2020 5468 6520 6561 7369  s:..    The easi
-00001080: 6573 7420 7761 7920 746f 2073 6574 2074  est way to set t
-00001090: 6869 7320 636c 6965 6e74 2075 7020 6973  his client up is
-000010a0: 2062 7920 7573 696e 6720 6120 736c 7572   by using a slur
-000010b0: 6d2d 636f 6e66 6967 2e69 6e69 0a20 2020  m-config.ini.   
-000010c0: 2061 6e64 2074 6865 2066 726f 6d2d 636f   and the from-co
-000010d0: 6e66 6967 2829 206d 6574 686f 642e 0a0a  nfig() method...
-000010e0: 2020 2020 4174 7472 6962 7574 6573 3a0a      Attributes:.
-000010f0: 2020 2020 2020 2020 736c 7572 6d5f 6461          slurm_da
-00001100: 7461 5f70 6174 6820 2873 7472 293a 2054  ta_path (str): T
-00001110: 6865 2070 6174 6820 746f 2074 6865 2064  he path to the d
-00001120: 6972 6563 746f 7279 2063 6f6e 7461 696e  irectory contain
-00001130: 696e 6720 7468 650a 2020 2020 2020 2020  ing the.        
-00001140: 2020 2020 6461 7461 2066 696c 6573 2066      data files f
-00001150: 6f72 2053 6c75 726d 206a 6f62 732e 0a20  or Slurm jobs.. 
-00001160: 2020 2020 2020 2073 6c75 726d 5f69 6d61         slurm_ima
-00001170: 6765 735f 7061 7468 2028 7374 7229 3a20  ges_path (str): 
-00001180: 5468 6520 7061 7468 2074 6f20 7468 6520  The path to the 
-00001190: 6469 7265 6374 6f72 7920 636f 6e74 6169  directory contai
-000011a0: 6e69 6e67 0a20 2020 2020 2020 2020 2020  ning.           
-000011b0: 2074 6865 2053 696e 6775 6c61 7269 7479   the Singularity
-000011c0: 2069 6d61 6765 7320 666f 7220 536c 7572   images for Slur
-000011d0: 6d20 6a6f 6273 2e0a 2020 2020 2020 2020  m jobs..        
-000011e0: 736c 7572 6d5f 636f 6e76 6572 7465 7273  slurm_converters
-000011f0: 5f70 6174 6820 2873 7472 293a 2054 6865  _path (str): The
-00001200: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
-00001210: 6563 746f 7279 2063 6f6e 7461 696e 696e  ectory containin
-00001220: 670a 2020 2020 2020 2020 2020 2020 7468  g.            th
-00001230: 6520 5369 6e67 756c 6172 6974 7920 696d  e Singularity im
-00001240: 6167 6573 2066 6f72 2066 696c 6520 636f  ages for file co
-00001250: 6e76 6572 7465 7273 2e0a 2020 2020 2020  nverters..      
-00001260: 2020 736c 7572 6d5f 6d6f 6465 6c5f 7061    slurm_model_pa
-00001270: 7468 7320 2864 6963 7429 3a20 4120 6469  ths (dict): A di
-00001280: 6374 696f 6e61 7279 2063 6f6e 7461 696e  ctionary contain
-00001290: 696e 6720 7468 6520 7061 7468 7320 746f  ing the paths to
-000012a0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
-000012b0: 2053 696e 6775 6c61 7269 7479 2069 6d61   Singularity ima
-000012c0: 6765 7320 666f 7220 7370 6563 6966 6963  ges for specific
-000012d0: 2053 6c75 726d 206a 6f62 206d 6f64 656c   Slurm job model
-000012e0: 732e 0a20 2020 2020 2020 2073 6c75 726d  s..        slurm
-000012f0: 5f6d 6f64 656c 5f72 6570 6f73 2028 6469  _model_repos (di
-00001300: 6374 293a 2041 2064 6963 7469 6f6e 6172  ct): A dictionar
-00001310: 7920 636f 6e74 6169 6e69 6e67 2074 6865  y containing the
-00001320: 2067 6974 0a20 2020 2020 2020 2020 2020   git.           
-00001330: 2072 6570 6f73 6974 6f72 6965 7320 6f66   repositories of
-00001340: 2053 696e 6775 6c61 7269 7479 2069 6d61   Singularity ima
-00001350: 6765 7320 666f 7220 7370 6563 6966 6963  ges for specific
-00001360: 2053 6c75 726d 206a 6f62 206d 6f64 656c   Slurm job model
-00001370: 732e 0a20 2020 2020 2020 2073 6c75 726d  s..        slurm
-00001380: 5f6d 6f64 656c 5f69 6d61 6765 7320 2864  _model_images (d
-00001390: 6963 7429 3a20 4120 6469 6374 696f 6e61  ict): A dictiona
-000013a0: 7279 2063 6f6e 7461 696e 696e 6720 7468  ry containing th
-000013b0: 6520 646f 636b 6572 6875 620a 2020 2020  e dockerhub.    
-000013c0: 2020 2020 2020 2020 6f66 2074 6865 2053          of the S
-000013d0: 696e 6775 6c61 7269 7479 2069 6d61 6765  ingularity image
-000013e0: 7320 666f 7220 7370 6563 6966 6963 2053  s for specific S
-000013f0: 6c75 726d 206a 6f62 206d 6f64 656c 732e  lurm job models.
-00001400: 0a20 2020 2020 2020 2020 2020 2057 696c  .            Wil
-00001410: 6c20 6669 6c6c 2061 7574 6f6d 6174 6963  l fill automatic
-00001420: 616c 6c79 2066 726f 6d20 7468 6520 6461  ally from the da
-00001430: 7461 2069 6e20 7468 6520 6769 7420 7265  ta in the git re
-00001440: 706f 7369 746f 7279 2c0a 2020 2020 2020  pository,.      
-00001450: 2020 2020 2020 6966 2079 6f75 2073 6574        if you set
-00001460: 2069 6e69 745f 736c 7572 6d2e 0a20 2020   init_slurm..   
-00001470: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
-00001480: 745f 7061 7468 2028 7374 7229 3a20 5468  t_path (str): Th
-00001490: 6520 7061 7468 2074 6f20 7468 6520 6469  e path to the di
-000014a0: 7265 6374 6f72 7920 636f 6e74 6169 6e69  rectory containi
-000014b0: 6e67 0a20 2020 2020 2020 2020 2020 2074  ng.            t
-000014c0: 6865 2053 6c75 726d 206a 6f62 2073 7562  he Slurm job sub
-000014d0: 6d69 7373 696f 6e20 7363 7269 7074 7320  mission scripts 
-000014e0: 6f6e 2053 6c75 726d 2e0a 2020 2020 2020  on Slurm..      
-000014f0: 2020 736c 7572 6d5f 7363 7269 7074 5f72    slurm_script_r
-00001500: 6570 6f20 2873 7472 293a 2054 6865 2067  epo (str): The g
-00001510: 6974 2068 7474 7073 2055 524c 2066 6f72  it https URL for
-00001520: 2063 6c6f 6e69 6e67 2074 6865 2072 6570   cloning the rep
-00001530: 6f0a 2020 2020 2020 2020 2020 2020 636f  o.            co
-00001540: 6e74 6169 6e69 6e67 2074 6865 2053 6c75  ntaining the Slu
-00001550: 726d 206a 6f62 2073 7562 6d69 7373 696f  rm job submissio
-00001560: 6e20 7363 7269 7074 732e 204f 7074 696f  n scripts. Optio
-00001570: 6e61 6c2e 0a0a 2020 2020 4578 616d 706c  nal...    Exampl
-00001580: 653a 0a20 2020 2020 2020 2023 2043 7265  e:.        # Cre
-00001590: 6174 6520 6120 536c 7572 6d43 6c69 656e  ate a SlurmClien
-000015a0: 7420 6f62 6a65 6374 2061 7320 636f 6e74  t object as cont
-000015b0: 6578 746d 616e 6167 6572 0a0a 2020 2020  extmanager..    
-000015c0: 2020 2020 7769 7468 2053 6c75 726d 436c      with SlurmCl
-000015d0: 6965 6e74 2e66 726f 6d5f 636f 6e66 6967  ient.from_config
-000015e0: 2829 2061 7320 636c 6965 6e74 3a0a 0a20  () as client:.. 
-000015f0: 2020 2020 2020 2020 2020 2023 2052 756e             # Run
-00001600: 2061 2063 6f6d 6d61 6e64 206f 6e20 7468   a command on th
-00001610: 6520 7265 6d6f 7465 2068 6f73 740a 0a20  e remote host.. 
-00001620: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00001630: 7420 3d20 636c 6965 6e74 2e72 756e 2827  t = client.run('
-00001640: 7362 6174 6368 206d 796a 6f62 2e73 6827  sbatch myjob.sh'
-00001650: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00001660: 2043 6865 636b 2077 6865 7468 6572 2074   Check whether t
-00001670: 6865 2063 6f6d 6d61 6e64 2073 7563 6365  he command succe
-00001680: 6564 6564 0a0a 2020 2020 2020 2020 2020  eded..          
-00001690: 2020 6966 2072 6573 756c 742e 6f6b 3a0a    if result.ok:.
-000016a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016b0: 7072 696e 7428 274a 6f62 2073 7562 6d69  print('Job submi
-000016c0: 7474 6564 2073 7563 6365 7373 6675 6c6c  tted successfull
-000016d0: 7921 2729 0a0a 2020 2020 2020 2020 2020  y!')..          
-000016e0: 2020 2320 5072 696e 7420 7468 6520 6f75    # Print the ou
-000016f0: 7470 7574 206f 6620 7468 6520 636f 6d6d  tput of the comm
-00001700: 616e 640a 0a20 2020 2020 2020 2020 2020  and..           
-00001710: 2070 7269 6e74 2872 6573 756c 742e 7374   print(result.st
-00001720: 646f 7574 290a 0a20 2020 2045 7861 6d70  dout)..    Examp
-00001730: 6c65 2032 3a0a 2020 2020 2020 2020 2320  le 2:.        # 
-00001740: 4372 6561 7465 2061 2053 6c75 726d 436c  Create a SlurmCl
-00001750: 6965 6e74 2061 6e64 2073 6574 7570 2053  ient and setup S
-00001760: 6c75 726d 2028 646f 776e 6c6f 6164 2063  lurm (download c
-00001770: 6f6e 7461 696e 6572 7320 6574 632e 290a  ontainers etc.).
-00001780: 0a20 2020 2020 2020 2077 6974 6820 536c  .        with Sl
-00001790: 7572 6d43 6c69 656e 742e 6672 6f6d 5f63  urmClient.from_c
-000017a0: 6f6e 6669 6728 696e 6974 5f73 6c75 726d  onfig(init_slurm
-000017b0: 3d54 7275 6529 2061 7320 636c 6965 6e74  =True) as client
-000017c0: 3a0a 0a20 2020 2020 2020 2020 2020 2063  :..            c
-000017d0: 6c69 656e 742e 7275 6e5f 776f 726b 666c  lient.run_workfl
-000017e0: 6f77 282e 2e2e 290a 0a20 2020 2022 2222  ow(...)..    """
-000017f0: 0a20 2020 205f 4445 4641 554c 545f 434f  .    _DEFAULT_CO
-00001800: 4e46 4947 5f50 4154 485f 3120 3d20 222f  NFIG_PATH_1 = "/
-00001810: 6574 632f 736c 7572 6d2d 636f 6e66 6967  etc/slurm-config
-00001820: 2e69 6e69 220a 2020 2020 5f44 4546 4155  .ini".    _DEFAU
-00001830: 4c54 5f43 4f4e 4649 475f 5041 5448 5f32  LT_CONFIG_PATH_2
-00001840: 203d 2022 7e2f 736c 7572 6d2d 636f 6e66   = "~/slurm-conf
-00001850: 6967 2e69 6e69 220a 2020 2020 5f44 4546  ig.ini".    _DEF
-00001860: 4155 4c54 5f48 4f53 5420 3d20 2273 6c75  AULT_HOST = "slu
-00001870: 726d 220a 2020 2020 5f44 4546 4155 4c54  rm".    _DEFAULT
-00001880: 5f49 4e4c 494e 455f 5353 485f 454e 5620  _INLINE_SSH_ENV 
-00001890: 3d20 5472 7565 0a20 2020 205f 4445 4641  = True.    _DEFA
-000018a0: 554c 545f 534c 5552 4d5f 4441 5441 5f50  ULT_SLURM_DATA_P
-000018b0: 4154 4820 3d20 226d 792d 7363 7261 7463  ATH = "my-scratc
-000018c0: 682f 6461 7461 220a 2020 2020 5f44 4546  h/data".    _DEF
-000018d0: 4155 4c54 5f53 4c55 524d 5f49 4d41 4745  AULT_SLURM_IMAGE
-000018e0: 535f 5041 5448 203d 2022 6d79 2d73 6372  S_PATH = "my-scr
-000018f0: 6174 6368 2f73 696e 6775 6c61 7269 7479  atch/singularity
-00001900: 5f69 6d61 6765 732f 776f 726b 666c 6f77  _images/workflow
-00001910: 7322 0a20 2020 205f 4445 4641 554c 545f  s".    _DEFAULT_
-00001920: 534c 5552 4d5f 434f 4e56 4552 5445 5253  SLURM_CONVERTERS
-00001930: 5f50 4154 4820 3d20 226d 792d 7363 7261  _PATH = "my-scra
-00001940: 7463 682f 7369 6e67 756c 6172 6974 795f  tch/singularity_
-00001950: 696d 6167 6573 2f63 6f6e 7665 7274 6572  images/converter
-00001960: 7322 0a20 2020 205f 4445 4641 554c 545f  s".    _DEFAULT_
-00001970: 534c 5552 4d5f 4749 545f 5343 5249 5054  SLURM_GIT_SCRIPT
-00001980: 5f50 4154 4820 3d20 2273 6c75 726d 2d73  _PATH = "slurm-s
-00001990: 6372 6970 7473 220a 2020 2020 5f4f 5554  cripts".    _OUT
-000019a0: 5f53 4550 203d 2022 2d2d 7370 6c69 742d  _SEP = "--split-
-000019b0: 2d22 0a20 2020 205f 5645 5253 494f 4e5f  -".    _VERSION_
-000019c0: 434d 4420 3d20 226c 7320 2d68 207b 736c  CMD = "ls -h {sl
-000019d0: 7572 6d5f 696d 6167 6573 5f70 6174 687d  urm_images_path}
-000019e0: 2f7b 696d 6167 655f 7061 7468 7d20 7c20  /{image_path} | 
-000019f0: 6772 6570 202d 6f50 2027 283f 3c3d 5c2d  grep -oP '(?<=\-
-00001a00: 7c5c 5f29 2876 2e2b 7c6c 6174 6573 7429  |\_)(v.+|latest)
-00001a10: 283f 3d2e 7369 6d67 7c2e 7369 6629 2722  (?=.simg|.sif)'"
-00001a20: 0a20 2020 2023 204e 6f74 652c 2067 7265  .    # Note, gre
-00001a30: 7020 7265 7475 726e 7320 6578 6974 636f  p returns exitco
-00001a40: 6465 2031 2069 6620 6e6f 206d 6174 6368  de 1 if no match
-00001a50: 2069 7320 666f 756e 6421 0a20 2020 2023   is found!.    #
-00001a60: 2054 6869 7320 7769 6c6c 2074 7261 6e73   This will trans
-00001a70: 6c61 7465 2069 6e74 6f20 6120 556e 6578  late into a Unex
-00001a80: 7065 6374 6564 4578 6974 2065 7272 6f72  pectedExit error
-00001a90: 2c20 736f 206d 7574 6520 7468 6174 2069  , so mute that i
-00001aa0: 6620 796f 750a 2020 2020 2320 646f 6e27  f you.    # don'
-00001ab0: 7420 6361 7265 2061 626f 7574 2065 6d70  t care about emp
-00001ac0: 7479 2e0a 2020 2020 2320 4c69 6b65 2062  ty..    # Like b
-00001ad0: 656c 6f77 2077 6974 6820 7468 6520 227c  elow with the "|
-00001ae0: 7c20 3a22 2e0a 2020 2020 2320 4461 7461  | :"..    # Data
-00001af0: 2063 6f75 6c64 206c 6567 6974 2062 6520   could legit be 
-00001b00: 656d 7074 792e 0a20 2020 205f 4441 5441  empty..    _DATA
-00001b10: 5f43 4d44 203d 2022 6c73 202d 6820 7b73  _CMD = "ls -h {s
-00001b20: 6c75 726d 5f64 6174 615f 7061 7468 7d20  lurm_data_path} 
-00001b30: 7c20 6772 6570 202d 6f50 2027 2e2b 283f  | grep -oP '.+(?
-00001b40: 3d2e 7a69 7029 2720 7c7c 203a 220a 2020  =.zip)' || :".  
-00001b50: 2020 5f41 4c4c 5f4a 4f42 535f 434d 4420    _ALL_JOBS_CMD 
-00001b60: 3d20 2273 6163 6374 202d 2d73 7461 7274  = "sacct --start
-00001b70: 7469 6d65 207b 7374 6172 745f 7469 6d65  time {start_time
-00001b80: 7d20 2d2d 656e 6474 696d 6520 7b65 6e64  } --endtime {end
-00001b90: 5f74 696d 657d 202d 2d73 7461 7465 207b  _time} --state {
-00001ba0: 7374 6174 6573 7d20 2d6f 207b 636f 6c75  states} -o {colu
-00001bb0: 6d6e 737d 202d 6e20 2d58 2022 0a20 2020  mns} -n -X ".   
-00001bc0: 205f 5a49 505f 434d 4420 3d20 2237 7a20   _ZIP_CMD = "7z 
-00001bd0: 6120 2d79 207b 6669 6c65 6e61 6d65 7d20  a -y {filename} 
-00001be0: 2d74 7a69 7020 7b64 6174 615f 6c6f 6361  -tzip {data_loca
-00001bf0: 7469 6f6e 7d2f 6461 7461 2f6f 7574 220a  tion}/data/out".
-00001c00: 2020 2020 5f41 4354 4956 455f 4a4f 4253      _ACTIVE_JOBS
-00001c10: 5f43 4d44 203d 2022 7371 7565 7565 202d  _CMD = "squeue -
-00001c20: 7520 2455 5345 5220 2d2d 6e6f 6865 6164  u $USER --nohead
-00001c30: 202d 2d66 6f72 6d61 7420 2546 220a 2020   --format %F".  
-00001c40: 2020 5f4a 4f42 5f53 5441 5455 535f 434d    _JOB_STATUS_CM
-00001c50: 4420 3d20 2273 6163 6374 202d 6e20 2d6f  D = "sacct -n -o
-00001c60: 204a 6f62 4964 2c53 7461 7465 2c45 6e64   JobId,State,End
-00001c70: 202d 5820 2d6a 207b 736c 7572 6d5f 6a6f   -X -j {slurm_jo
-00001c80: 625f 6964 7d22 0a20 2020 2023 2054 4f44  b_id}".    # TOD
-00001c90: 4f20 6d6f 7665 2061 6c6c 2063 6f6d 6d61  O move all comma
-00001ca0: 6e64 7320 746f 2061 2073 696d 696c 6172  nds to a similar
-00001cb0: 2066 6f72 6d61 742e 0a20 2020 2023 2054   format..    # T
-00001cc0: 6865 6e20 6d61 7962 6520 616c 6c6f 7720  hen maybe allow 
-00001cd0: 6f76 6572 7772 6974 6520 6672 6f6d 2073  overwrite from s
-00001ce0: 6c75 726d 2d63 6f6e 6669 672e 696e 690a  lurm-config.ini.
-00001cf0: 2020 2020 5f4c 4f47 4649 4c45 203d 2022      _LOGFILE = "
-00001d00: 6f6d 6572 6f2d 7b73 6c75 726d 5f6a 6f62  omero-{slurm_job
-00001d10: 5f69 647d 2e6c 6f67 220a 2020 2020 5f43  _id}.log".    _C
-00001d20: 4f4e 5645 5254 4552 5f4c 4f47 4649 4c45  ONVERTER_LOGFILE
-00001d30: 203d 2022 736c 7572 6d2d 7b73 6c75 726d   = "slurm-{slurm
-00001d40: 5f6a 6f62 5f69 647d 5f2a 2e6f 7574 220a  _job_id}_*.out".
-00001d50: 2020 2020 5f54 4149 4c5f 4c4f 475f 434d      _TAIL_LOG_CM
-00001d60: 4420 3d20 2274 6169 6c20 2d6e 207b 6e7d  D = "tail -n {n}
-00001d70: 207b 6c6f 675f 6669 6c65 7d20 7c20 7374   {log_file} | st
-00001d80: 7269 6e67 7322 0a20 2020 205f 4c4f 4746  rings".    _LOGF
-00001d90: 494c 455f 4441 5441 5f43 4d44 203d 2022  ILE_DATA_CMD = "
-00001da0: 6361 7420 7b6c 6f67 5f66 696c 657d 207c  cat {log_file} |
-00001db0: 2070 6572 6c20 2d77 6e65 2027 2f52 756e   perl -wne '/Run
-00001dc0: 6e69 6e67 205b 5c77 2d5d 2b3f 204a 6f62  ning [\w-]+? Job
-00001dd0: 2077 5c2f 202e 2b3f 205c 7c20 2e2b 3f20   w\/ .+? \| .+? 
-00001de0: 5c7c 2028 2e2b 3f29 205c 7c2e 2a2f 6920  \| (.+?) \|.*/i 
-00001df0: 616e 6420 7072 696e 7424 3127 220a 0a20  and print$1'".. 
-00001e00: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00001e10: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-00001e20: 2020 2020 2020 2068 6f73 743d 5f44 4546         host=_DEF
-00001e30: 4155 4c54 5f48 4f53 542c 0a20 2020 2020  AULT_HOST,.     
-00001e40: 2020 2020 2020 2020 2020 2020 7573 6572              user
-00001e50: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00001e60: 2020 2020 2020 2020 706f 7274 3d4e 6f6e          port=Non
-00001e70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00001e80: 2020 2020 636f 6e66 6967 3d4e 6f6e 652c      config=None,
-00001e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ea0: 2020 6761 7465 7761 793d 4e6f 6e65 2c0a    gateway=None,.
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ec0: 2066 6f72 7761 7264 5f61 6765 6e74 3d4e   forward_agent=N
-00001ed0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00001ee0: 2020 2020 2020 636f 6e6e 6563 745f 7469        connect_ti
-00001ef0: 6d65 6f75 743d 4e6f 6e65 2c0a 2020 2020  meout=None,.    
-00001f00: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00001f10: 6e65 6374 5f6b 7761 7267 733d 4e6f 6e65  nect_kwargs=None
-00001f20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001f30: 2020 2069 6e6c 696e 655f 7373 685f 656e     inline_ssh_en
-00001f40: 763d 5f44 4546 4155 4c54 5f49 4e4c 494e  v=_DEFAULT_INLIN
-00001f50: 455f 5353 485f 454e 562c 0a20 2020 2020  E_SSH_ENV,.     
-00001f60: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-00001f70: 6d5f 6461 7461 5f70 6174 683a 2073 7472  m_data_path: str
-00001f80: 203d 205f 4445 4641 554c 545f 534c 5552   = _DEFAULT_SLUR
-00001f90: 4d5f 4441 5441 5f50 4154 482c 0a20 2020  M_DATA_PATH,.   
-00001fa0: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-00001fb0: 7572 6d5f 696d 6167 6573 5f70 6174 683a  urm_images_path:
-00001fc0: 2073 7472 203d 205f 4445 4641 554c 545f   str = _DEFAULT_
-00001fd0: 534c 5552 4d5f 494d 4147 4553 5f50 4154  SLURM_IMAGES_PAT
-00001fe0: 482c 0a20 2020 2020 2020 2020 2020 2020  H,.             
-00001ff0: 2020 2020 736c 7572 6d5f 636f 6e76 6572      slurm_conver
-00002000: 7465 7273 5f70 6174 683a 2073 7472 203d  ters_path: str =
-00002010: 205f 4445 4641 554c 545f 534c 5552 4d5f   _DEFAULT_SLURM_
-00002020: 434f 4e56 4552 5445 5253 5f50 4154 482c  CONVERTERS_PATH,
-00002030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002040: 2020 736c 7572 6d5f 6d6f 6465 6c5f 7061    slurm_model_pa
-00002050: 7468 733a 2064 6963 7420 3d20 4e6f 6e65  ths: dict = None
-00002060: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002070: 2020 2073 6c75 726d 5f6d 6f64 656c 5f72     slurm_model_r
-00002080: 6570 6f73 3a20 6469 6374 203d 204e 6f6e  epos: dict = Non
-00002090: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-000020a0: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-000020b0: 696d 6167 6573 3a20 6469 6374 203d 204e  images: dict = N
-000020c0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-000020d0: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-000020e0: 6c5f 6a6f 6273 3a20 6469 6374 203d 204e  l_jobs: dict = N
-000020f0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-00002100: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-00002110: 6c5f 6a6f 6273 5f70 6172 616d 733a 2064  l_jobs_params: d
-00002120: 6963 7420 3d20 4e6f 6e65 2c0a 2020 2020  ict = None,.    
-00002130: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
-00002140: 726d 5f73 6372 6970 745f 7061 7468 3a20  rm_script_path: 
-00002150: 7374 7220 3d20 5f44 4546 4155 4c54 5f53  str = _DEFAULT_S
-00002160: 4c55 524d 5f47 4954 5f53 4352 4950 545f  LURM_GIT_SCRIPT_
-00002170: 5041 5448 2c0a 2020 2020 2020 2020 2020  PATH,.          
-00002180: 2020 2020 2020 2073 6c75 726d 5f73 6372         slurm_scr
-00002190: 6970 745f 7265 706f 3a20 7374 7220 3d20  ipt_repo: str = 
-000021a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-000021b0: 2020 2020 2020 2069 6e69 745f 736c 7572         init_slur
-000021c0: 6d3a 2062 6f6f 6c20 3d20 4661 6c73 652c  m: bool = False,
-000021d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000021e0: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-000021f0: 496e 6974 6961 6c69 7a65 7320 6120 6e65  Initializes a ne
-00002200: 7720 696e 7374 616e 6365 206f 6620 7468  w instance of th
-00002210: 6520 536c 7572 6d43 6c69 656e 7420 636c  e SlurmClient cl
-00002220: 6173 732e 0a0a 2020 2020 2020 2020 4974  ass...        It
-00002230: 2069 7320 7072 6566 6572 6162 6c65 2074   is preferable t
-00002240: 6f20 7573 6520 2366 726f 6d5f 636f 6e66  o use #from_conf
-00002250: 6967 282e 2e2e 2920 6d65 7468 6f64 2074  ig(...) method t
-00002260: 6f20 696e 6974 6961 6c69 7a65 0a20 2020  o initialize.   
-00002270: 2020 2020 2070 6172 616d 6574 6572 7320       parameters 
-00002280: 6672 6f6d 2061 2063 6f6e 6669 6720 6669  from a config fi
-00002290: 6c65 2e0a 0a20 2020 2020 2020 2041 7267  le...        Arg
-000022a0: 733a 0a20 2020 2020 2020 2020 2020 2068  s:.            h
-000022b0: 6f73 7420 2873 7472 2c20 6f70 7469 6f6e  ost (str, option
-000022c0: 616c 293a 2054 6865 2068 6f73 746e 616d  al): The hostnam
-000022d0: 6520 6f72 2049 5020 6164 6472 6573 7320  e or IP address 
-000022e0: 6f66 2074 6865 2072 656d 6f74 650a 2020  of the remote.  
-000022f0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00002300: 7276 6572 2e20 4465 6661 756c 7473 2074  rver. Defaults t
-00002310: 6f20 5f44 4546 4155 4c54 5f48 4f53 542e  o _DEFAULT_HOST.
-00002320: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
-00002330: 7220 2873 7472 2c20 6f70 7469 6f6e 616c  r (str, optional
-00002340: 293a 2054 6865 2075 7365 726e 616d 6520  ): The username 
-00002350: 746f 2075 7365 2077 6865 6e20 636f 6e6e  to use when conn
-00002360: 6563 7469 6e67 2074 6f20 0a20 2020 2020  ecting to .     
-00002370: 2020 2020 2020 2020 2020 2074 6865 2072             the r
-00002380: 656d 6f74 6520 7365 7276 6572 2e20 4465  emote server. De
-00002390: 6661 756c 7473 2074 6f20 4e6f 6e65 2c20  faults to None, 
-000023a0: 7768 6963 6820 6465 6661 756c 7473 200a  which defaults .
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 746f 2063 6f6e 6669 672e 7573 6572 2e0a  to config.user..
-000023d0: 2020 2020 2020 2020 2020 2020 706f 7274              port
-000023e0: 2028 696e 742c 206f 7074 696f 6e61 6c29   (int, optional)
-000023f0: 3a20 5468 6520 5353 4820 706f 7274 2074  : The SSH port t
-00002400: 6f20 7573 6520 7768 656e 2063 6f6e 6e65  o use when conne
-00002410: 6374 696e 672e 0a20 2020 2020 2020 2020  cting..         
-00002420: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-00002430: 746f 204e 6f6e 652c 2077 6869 6368 2064  to None, which d
-00002440: 6566 6175 6c74 7320 746f 2063 6f6e 6669  efaults to confi
-00002450: 672e 706f 7274 2e0a 2020 2020 2020 2020  g.port..        
-00002460: 2020 2020 636f 6e66 6967 2028 7374 722c      config (str,
-00002470: 206f 7074 696f 6e61 6c29 3a20 5061 7468   optional): Path
-00002480: 2074 6f20 7468 6520 5353 4820 636f 6e66   to the SSH conf
-00002490: 6967 2066 696c 652e 0a20 2020 2020 2020  ig file..       
-000024a0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-000024b0: 7320 746f 204e 6f6e 652c 2077 6869 6368  s to None, which
-000024c0: 2064 6566 6175 6c74 7320 746f 2079 6f75   defaults to you
-000024d0: 7220 5353 4820 636f 6e66 6967 2066 696c  r SSH config fil
-000024e0: 652e 0a20 2020 2020 2020 2020 2020 2067  e..            g
-000024f0: 6174 6577 6179 2028 436f 6e6e 6563 7469  ateway (Connecti
-00002500: 6f6e 2c20 6f70 7469 6f6e 616c 293a 2041  on, optional): A
-00002510: 6e20 6f70 7469 6f6e 616c 2067 6174 6577  n optional gatew
-00002520: 6179 2066 6f72 2063 6f6e 6e65 6374 696e  ay for connectin
-00002530: 6720 0a20 2020 2020 2020 2020 2020 2020  g .             
-00002540: 2020 2074 6872 6f75 6768 2061 206a 756d     through a jum
-00002550: 7020 686f 7374 2e20 4465 6661 756c 7473  p host. Defaults
-00002560: 2074 6f20 4e6f 6e65 2e0a 2020 2020 2020   to None..      
-00002570: 2020 2020 2020 666f 7277 6172 645f 6167        forward_ag
-00002580: 656e 7420 2862 6f6f 6c2c 206f 7074 696f  ent (bool, optio
-00002590: 6e61 6c29 3a20 5768 6574 6865 7220 746f  nal): Whether to
-000025a0: 2066 6f72 7761 7264 2074 6865 206c 6f63   forward the loc
-000025b0: 616c 2053 5348 200a 2020 2020 2020 2020  al SSH .        
-000025c0: 2020 2020 2020 2020 6167 656e 7420 746f          agent to
-000025d0: 2074 6865 2072 656d 6f74 6520 7365 7276   the remote serv
-000025e0: 6572 2e20 4465 6661 756c 7473 2074 6f20  er. Defaults to 
-000025f0: 4e6f 6e65 2c20 7768 6963 6820 0a20 2020  None, which .   
-00002600: 2020 2020 2020 2020 2020 2020 2064 6566               def
-00002610: 6175 6c74 7320 746f 2063 6f6e 6669 672e  aults to config.
-00002620: 666f 7277 6172 645f 6167 656e 742e 0a20  forward_agent.. 
-00002630: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
-00002640: 6374 5f74 696d 656f 7574 2028 696e 742c  ct_timeout (int,
-00002650: 206f 7074 696f 6e61 6c29 3a20 5469 6d65   optional): Time
-00002660: 6f75 7420 666f 7220 6573 7461 626c 6973  out for establis
-00002670: 6869 6e67 2074 6865 2053 5348 200a 2020  hing the SSH .  
-00002680: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00002690: 6e6e 6563 7469 6f6e 2e20 4465 6661 756c  nnection. Defaul
-000026a0: 7473 2074 6f20 4e6f 6e65 2c20 7768 6963  ts to None, whic
-000026b0: 6820 6465 6661 756c 7473 200a 2020 2020  h defaults .    
-000026c0: 2020 2020 2020 2020 2020 2020 746f 2063              to c
-000026d0: 6f6e 6669 672e 7469 6d65 6f75 7473 2e63  onfig.timeouts.c
-000026e0: 6f6e 6e65 6374 2e0a 2020 2020 2020 2020  onnect..        
-000026f0: 2020 2020 636f 6e6e 6563 745f 6b77 6172      connect_kwar
-00002700: 6773 2028 6469 6374 2c20 6f70 7469 6f6e  gs (dict, option
-00002710: 616c 293a 2041 6464 6974 696f 6e61 6c20  al): Additional 
-00002720: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
-00002730: 7320 666f 7220 0a20 2020 2020 2020 2020  s for .         
-00002740: 2020 2020 2020 2074 6865 2075 6e64 6572         the under
-00002750: 6c79 696e 6720 5353 4820 636f 6e6e 6563  lying SSH connec
-00002760: 7469 6f6e 2e20 4861 6e64 6564 2076 6572  tion. Handed ver
-00002770: 6261 7469 6d20 746f 200a 2020 2020 2020  batim to .      
-00002780: 2020 2020 2020 2020 2020 6053 5348 436c            `SSHCl
-00002790: 6965 6e74 2e63 6f6e 6e65 6374 203c 7061  ient.connect <pa
-000027a0: 7261 6d69 6b6f 2e63 6c69 656e 742e 5353  ramiko.client.SS
-000027b0: 4843 6c69 656e 742e 636f 6e6e 6563 743e  HClient.connect>
-000027c0: 602e 200a 2020 2020 2020 2020 2020 2020  `. .            
-000027d0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-000027e0: 4e6f 6e65 2e20 0a20 2020 2020 2020 2020  None. .         
-000027f0: 2020 2069 6e6c 696e 655f 7373 685f 656e     inline_ssh_en
-00002800: 7620 2862 6f6f 6c2c 206f 7074 696f 6e61  v (bool, optiona
-00002810: 6c29 3a20 5768 6574 6865 7220 746f 2075  l): Whether to u
-00002820: 7365 2069 6e6c 696e 6520 5353 480a 2020  se inline SSH.  
-00002830: 2020 2020 2020 2020 2020 2020 2020 656e                en
-00002840: 7669 726f 6e6d 656e 742e 2054 6869 7320  vironment. This 
-00002850: 6973 206e 6563 6573 7361 7279 2069 6620  is necessary if 
-00002860: 7468 6520 7265 6d6f 7465 2073 6572 7665  the remote serve
-00002870: 7220 6861 7320 0a20 2020 2020 2020 2020  r has .         
-00002880: 2020 2020 2020 2061 2072 6573 7472 6963         a restric
-00002890: 7465 6420 6060 4163 6365 7074 456e 7660  ted ``AcceptEnv`
-000028a0: 6020 7365 7474 696e 6720 2877 6869 6368  ` setting (which
-000028b0: 2069 7320 7468 6520 636f 6d6d 6f6e 200a   is the common .
-000028c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000028d0: 6465 6661 756c 7429 2e20 4465 6661 756c  default). Defaul
-000028e0: 7473 2074 6f20 5f44 4546 4155 4c54 5f49  ts to _DEFAULT_I
-000028f0: 4e4c 494e 455f 5353 485f 454e 562e 0a20  NLINE_SSH_ENV.. 
-00002900: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
-00002910: 5f64 6174 615f 7061 7468 2028 7374 722c  _data_path (str,
-00002920: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-00002930: 7061 7468 2074 6f20 7468 6520 6469 7265  path to the dire
-00002940: 6374 6f72 790a 2020 2020 2020 2020 2020  ctory.          
-00002950: 2020 2020 2020 636f 6e74 6169 6e69 6e67        containing
-00002960: 2074 6865 2064 6174 6120 6669 6c65 7320   the data files 
-00002970: 666f 7220 536c 7572 6d20 6a6f 6273 2e0a  for Slurm jobs..
-00002980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002990: 4465 6661 756c 7473 2074 6f20 5f44 4546  Defaults to _DEF
-000029a0: 4155 4c54 5f53 4c55 524d 5f44 4154 415f  AULT_SLURM_DATA_
-000029b0: 5041 5448 2e0a 2020 2020 2020 2020 2020  PATH..          
-000029c0: 2020 736c 7572 6d5f 696d 6167 6573 5f70    slurm_images_p
-000029d0: 6174 6820 2873 7472 2c20 6f70 7469 6f6e  ath (str, option
-000029e0: 616c 293a 2054 6865 2070 6174 6820 746f  al): The path to
-000029f0: 2074 6865 2064 6972 6563 746f 7279 0a20   the directory. 
-00002a00: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00002a10: 6f6e 7461 696e 696e 6720 7468 6520 5369  ontaining the Si
-00002a20: 6e67 756c 6172 6974 7920 696d 6167 6573  ngularity images
-00002a30: 2066 6f72 2053 6c75 726d 206a 6f62 732e   for Slurm jobs.
-00002a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002a50: 2044 6566 6175 6c74 7320 746f 205f 4445   Defaults to _DE
-00002a60: 4641 554c 545f 534c 5552 4d5f 494d 4147  FAULT_SLURM_IMAG
-00002a70: 4553 5f50 4154 482e 0a20 2020 2020 2020  ES_PATH..       
-00002a80: 2020 2020 2073 6c75 726d 5f63 6f6e 7665       slurm_conve
-00002a90: 7274 6572 735f 7061 7468 2028 7374 722c  rters_path (str,
-00002aa0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-00002ab0: 7061 7468 2074 6f20 7468 6520 6469 7265  path to the dire
-00002ac0: 6374 6f72 790a 2020 2020 2020 2020 2020  ctory.          
-00002ad0: 2020 2020 2020 636f 6e74 6169 6e69 6e67        containing
-00002ae0: 2074 6865 2053 696e 6775 6c61 7269 7479   the Singularity
-00002af0: 2069 6d61 6765 7320 666f 7220 6669 6c65   images for file
-00002b00: 2063 6f6e 7665 7274 6572 732e 0a20 2020   converters..   
-00002b10: 2020 2020 2020 2020 2020 2020 2044 6566               Def
-00002b20: 6175 6c74 7320 746f 205f 4445 4641 554c  aults to _DEFAUL
-00002b30: 545f 534c 5552 4d5f 434f 4e56 4552 5445  T_SLURM_CONVERTE
-00002b40: 5253 5f50 4154 482e 0a20 2020 2020 2020  RS_PATH..       
-00002b50: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
-00002b60: 5f70 6174 6873 2028 6469 6374 2c20 6f70  _paths (dict, op
-00002b70: 7469 6f6e 616c 293a 2041 2064 6963 7469  tional): A dicti
-00002b80: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
-00002b90: 2074 6865 200a 2020 2020 2020 2020 2020   the .          
-00002ba0: 2020 2020 2020 7061 7468 7320 746f 2074        paths to t
-00002bb0: 6865 2053 696e 6775 6c61 7269 7479 2069  he Singularity i
-00002bc0: 6d61 6765 7320 666f 7220 7370 6563 6966  mages for specif
-00002bd0: 6963 2053 6c75 726d 206a 6f62 206d 6f64  ic Slurm job mod
-00002be0: 656c 732e 0a20 2020 2020 2020 2020 2020  els..           
-00002bf0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
-00002c00: 204e 6f6e 652e 0a20 2020 2020 2020 2020   None..         
-00002c10: 2020 2073 6c75 726d 5f6d 6f64 656c 5f72     slurm_model_r
-00002c20: 6570 6f73 2028 6469 6374 2c20 6f70 7469  epos (dict, opti
-00002c30: 6f6e 616c 293a 2041 2064 6963 7469 6f6e  onal): A diction
-00002c40: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
-00002c50: 6865 200a 2020 2020 2020 2020 2020 2020  he .            
-00002c60: 2020 2020 6769 7420 7265 706f 7369 746f      git reposito
-00002c70: 7269 6573 206f 6620 5369 6e67 756c 6172  ries of Singular
-00002c80: 6974 7920 696d 6167 6573 2066 6f72 2073  ity images for s
-00002c90: 7065 6369 6669 6320 536c 7572 6d20 0a20  pecific Slurm . 
-00002ca0: 2020 2020 2020 2020 2020 2020 2020 206a                 j
-00002cb0: 6f62 206d 6f64 656c 732e 0a20 2020 2020  ob models..     
-00002cc0: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
-00002cd0: 6c74 7320 746f 204e 6f6e 652e 0a20 2020  lts to None..   
-00002ce0: 2020 2020 2020 2020 2073 6c75 726d 5f6d           slurm_m
-00002cf0: 6f64 656c 5f69 6d61 6765 7320 2864 6963  odel_images (dic
-00002d00: 742c 206f 7074 696f 6e61 6c29 3a20 4120  t, optional): A 
-00002d10: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
-00002d20: 696e 696e 6720 7468 6520 0a20 2020 2020  ining the .     
-00002d30: 2020 2020 2020 2020 2020 2064 6f63 6b65             docke
-00002d40: 7268 7562 206f 6620 7468 6520 5369 6e67  rhub of the Sing
-00002d50: 756c 6172 6974 7920 696d 6167 6573 2066  ularity images f
-00002d60: 6f72 2073 7065 6369 6669 6320 536c 7572  or specific Slur
-00002d70: 6d20 0a20 2020 2020 2020 2020 2020 2020  m .             
-00002d80: 2020 206a 6f62 206d 6f64 656c 732e 2057     job models. W
-00002d90: 696c 6c20 6669 6c6c 2061 7574 6f6d 6174  ill fill automat
-00002da0: 6963 616c 6c79 2066 726f 6d20 7468 6520  ically from the 
-00002db0: 6461 7461 2069 6e20 7468 6520 6769 7420  data in the git 
-00002dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002dd0: 2072 6570 6f73 6974 6f72 7920 6966 2079   repository if y
-00002de0: 6f75 2073 6574 2069 6e69 745f 736c 7572  ou set init_slur
-00002df0: 6d2e 0a20 2020 2020 2020 2020 2020 2020  m..             
-00002e00: 2020 2044 6566 6175 6c74 7320 746f 204e     Defaults to N
-00002e10: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
-00002e20: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
-00002e30: 7320 2864 6963 742c 206f 7074 696f 6e61  s (dict, optiona
-00002e40: 6c29 3a20 4120 6469 6374 696f 6e61 7279  l): A dictionary
-00002e50: 2063 6f6e 7461 696e 696e 670a 2020 2020   containing.    
-00002e60: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00002e70: 726d 6174 696f 6e20 6162 6f75 7420 7370  rmation about sp
-00002e80: 6563 6966 6963 2053 6c75 726d 206a 6f62  ecific Slurm job
-00002e90: 206d 6f64 656c 732e 0a20 2020 2020 2020   models..       
-00002ea0: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
-00002eb0: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
-00002ec0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00002ed0: 656c 5f6a 6f62 735f 7061 7261 6d73 2028  el_jobs_params (
-00002ee0: 6469 6374 2c20 6f70 7469 6f6e 616c 293a  dict, optional):
-00002ef0: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
-00002f00: 6e74 6169 6e69 6e67 0a20 2020 2020 2020  ntaining.       
-00002f10: 2020 2020 2020 2020 2070 6172 616d 6574           paramet
-00002f20: 6572 7320 666f 7220 7370 6563 6966 6963  ers for specific
-00002f30: 2053 6c75 726d 206a 6f62 206d 6f64 656c   Slurm job model
-00002f40: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-00002f50: 2020 2044 6566 6175 6c74 7320 746f 204e     Defaults to N
-00002f60: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
-00002f70: 2073 6c75 726d 5f73 6372 6970 745f 7061   slurm_script_pa
-00002f80: 7468 2028 7374 722c 206f 7074 696f 6e61  th (str, optiona
-00002f90: 6c29 3a20 5468 6520 7061 7468 2074 6f20  l): The path to 
-00002fa0: 7468 6520 6469 7265 6374 6f72 790a 2020  the directory.  
-00002fb0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00002fc0: 6e74 6169 6e69 6e67 2074 6865 2053 6c75  ntaining the Slu
-00002fd0: 726d 206a 6f62 2073 7562 6d69 7373 696f  rm job submissio
-00002fe0: 6e20 7363 7269 7074 7320 6f6e 2053 6c75  n scripts on Slu
-00002ff0: 726d 2e0a 2020 2020 2020 2020 2020 2020  rm..            
-00003000: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00003010: 5f44 4546 4155 4c54 5f53 4c55 524d 5f47  _DEFAULT_SLURM_G
-00003020: 4954 5f53 4352 4950 545f 5041 5448 2e0a  IT_SCRIPT_PATH..
-00003030: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-00003040: 6d5f 7363 7269 7074 5f72 6570 6f20 2873  m_script_repo (s
-00003050: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
-00003060: 6865 2067 6974 2068 7474 7073 2055 524c  he git https URL
-00003070: 2066 6f72 2063 6c6f 6e69 6e67 0a20 2020   for cloning.   
-00003080: 2020 2020 2020 2020 2020 2020 2074 6865               the
-00003090: 2072 6570 6f20 636f 6e74 6169 6e69 6e67   repo containing
-000030a0: 2074 6865 2053 6c75 726d 206a 6f62 2073   the Slurm job s
-000030b0: 7562 6d69 7373 696f 6e20 7363 7269 7074  ubmission script
-000030c0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-000030d0: 2020 2044 6566 6175 6c74 7320 746f 204e     Defaults to N
-000030e0: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
-000030f0: 2069 6e69 745f 736c 7572 6d20 2862 6f6f   init_slurm (boo
-00003100: 6c29 3a20 5768 6574 6865 7220 746f 2073  l): Whether to s
-00003110: 6574 2075 7020 7468 6520 7265 7175 6972  et up the requir
-00003120: 6564 2073 7472 7563 7475 7265 7320 0a20  ed structures . 
-00003130: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-00003140: 6e20 536c 7572 6d20 6166 7465 7220 696e  n Slurm after in
-00003150: 6974 6961 7469 6e67 2074 6869 7320 636c  itiating this cl
-00003160: 6965 6e74 2e20 5468 6973 2069 6e63 6c75  ient. This inclu
-00003170: 6465 7320 6372 6561 7469 6e67 200a 2020  des creating .  
-00003180: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00003190: 7373 696e 6720 666f 6c64 6572 732c 2064  ssing folders, d
-000031a0: 6f77 6e6c 6f61 6469 6e67 2063 6f6e 7461  ownloading conta
-000031b0: 696e 6572 2069 6d61 6765 732c 2063 6c6f  iner images, clo
-000031c0: 6e69 6e67 2067 6974 2c65 7463 2e0a 2020  ning git,etc..  
-000031d0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
-000031e0: 6973 2077 696c 6c20 7461 6b65 2061 2077  is will take a w
-000031f0: 6869 6c65 2061 7420 6669 7273 7420 6275  hile at first bu
-00003200: 7420 7769 6c6c 2076 616c 6964 6174 6520  t will validate 
-00003210: 796f 7572 2073 6574 7570 2e0a 2020 2020  your setup..    
-00003220: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00003230: 756c 7473 2074 6f20 4661 6c73 6520 746f  ults to False to
-00003240: 2073 6176 6520 7469 6d65 2e0a 2020 2020   save time..    
-00003250: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00003260: 7375 7065 7228 536c 7572 6d43 6c69 656e  super(SlurmClien
-00003270: 742c 2073 656c 6629 2e5f 5f69 6e69 745f  t, self).__init_
-00003280: 5f28 686f 7374 2c0a 2020 2020 2020 2020  _(host,.        
-00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032b0: 2020 7573 6572 2c0a 2020 2020 2020 2020    user,.        
-000032c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032e0: 2020 706f 7274 2c0a 2020 2020 2020 2020    port,.        
-000032f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003310: 2020 636f 6e66 6967 2c0a 2020 2020 2020    config,.      
-00003320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003340: 2020 2020 6761 7465 7761 792c 0a20 2020      gateway,.   
-00003350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003370: 2020 2020 2020 2066 6f72 7761 7264 5f61         forward_a
-00003380: 6765 6e74 2c0a 2020 2020 2020 2020 2020  gent,.          
-00003390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033b0: 636f 6e6e 6563 745f 7469 6d65 6f75 742c  connect_timeout,
-000033c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000033d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033e0: 2020 2020 2020 2020 2020 2063 6f6e 6e65             conne
-000033f0: 6374 5f6b 7761 7267 732c 0a20 2020 2020  ct_kwargs,.     
-00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003420: 2020 2020 2069 6e6c 696e 655f 7373 685f       inline_ssh_
-00003430: 656e 7629 0a20 2020 2020 2020 2073 656c  env).        sel
-00003440: 662e 736c 7572 6d5f 6461 7461 5f70 6174  f.slurm_data_pat
-00003450: 6820 3d20 736c 7572 6d5f 6461 7461 5f70  h = slurm_data_p
-00003460: 6174 680a 2020 2020 2020 2020 7365 6c66  ath.        self
-00003470: 2e73 6c75 726d 5f69 6d61 6765 735f 7061  .slurm_images_pa
-00003480: 7468 203d 2073 6c75 726d 5f69 6d61 6765  th = slurm_image
-00003490: 735f 7061 7468 0a20 2020 2020 2020 2073  s_path.        s
-000034a0: 656c 662e 736c 7572 6d5f 636f 6e76 6572  elf.slurm_conver
-000034b0: 7465 7273 5f70 6174 6820 3d20 736c 7572  ters_path = slur
-000034c0: 6d5f 636f 6e76 6572 7465 7273 5f70 6174  m_converters_pat
-000034d0: 680a 2020 2020 2020 2020 7365 6c66 2e73  h.        self.s
-000034e0: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
-000034f0: 203d 2073 6c75 726d 5f6d 6f64 656c 5f70   = slurm_model_p
-00003500: 6174 6873 0a20 2020 2020 2020 2073 656c  aths.        sel
-00003510: 662e 736c 7572 6d5f 7363 7269 7074 5f70  f.slurm_script_p
-00003520: 6174 6820 3d20 736c 7572 6d5f 7363 7269  ath = slurm_scri
-00003530: 7074 5f70 6174 680a 2020 2020 2020 2020  pt_path.        
-00003540: 7365 6c66 2e73 6c75 726d 5f73 6372 6970  self.slurm_scrip
-00003550: 745f 7265 706f 203d 2073 6c75 726d 5f73  t_repo = slurm_s
-00003560: 6372 6970 745f 7265 706f 0a20 2020 2020  cript_repo.     
-00003570: 2020 2073 656c 662e 736c 7572 6d5f 6d6f     self.slurm_mo
-00003580: 6465 6c5f 7265 706f 7320 3d20 736c 7572  del_repos = slur
-00003590: 6d5f 6d6f 6465 6c5f 7265 706f 730a 2020  m_model_repos.  
-000035a0: 2020 2020 2020 7365 6c66 2e73 6c75 726d        self.slurm
-000035b0: 5f6d 6f64 656c 5f69 6d61 6765 7320 3d20  _model_images = 
-000035c0: 736c 7572 6d5f 6d6f 6465 6c5f 696d 6167  slurm_model_imag
-000035d0: 6573 0a20 2020 2020 2020 2073 656c 662e  es.        self.
-000035e0: 736c 7572 6d5f 6d6f 6465 6c5f 6a6f 6273  slurm_model_jobs
-000035f0: 203d 2073 6c75 726d 5f6d 6f64 656c 5f6a   = slurm_model_j
-00003600: 6f62 730a 2020 2020 2020 2020 7365 6c66  obs.        self
-00003610: 2e73 6c75 726d 5f6d 6f64 656c 5f6a 6f62  .slurm_model_job
-00003620: 735f 7061 7261 6d73 203d 2073 6c75 726d  s_params = slurm
-00003630: 5f6d 6f64 656c 5f6a 6f62 735f 7061 7261  _model_jobs_para
-00003640: 6d73 0a0a 2020 2020 2020 2020 2320 496e  ms..        # In
-00003650: 6974 2063 6163 6865 2e20 4b65 6570 2072  it cache. Keep r
-00003660: 6573 706f 6e73 6573 2066 6f72 2033 3630  esponses for 360
-00003670: 2073 6563 6f6e 6473 0a20 2020 2020 2020   seconds.       
-00003680: 2073 656c 662e 6361 6368 6520 3d20 7265   self.cache = re
-00003690: 7175 6573 7473 5f63 6163 6865 2e62 6163  quests_cache.bac
-000036a0: 6b65 6e64 732e 7371 6c69 7465 2e53 514c  kends.sqlite.SQL
-000036b0: 6974 6543 6163 6865 280a 2020 2020 2020  iteCache(.      
-000036c0: 2020 2020 2020 6462 5f70 6174 683d 2267        db_path="g
-000036d0: 6974 6875 625f 6361 6368 6522 2c20 7573  ithub_cache", us
-000036e0: 655f 7465 6d70 3d54 7275 6529 0a20 2020  e_temp=True).   
-000036f0: 2020 2020 2073 656c 662e 6765 745f 6f72       self.get_or
-00003700: 5f63 7265 6174 655f 6769 7468 7562 5f73  _create_github_s
-00003710: 6573 7369 6f6e 2829 0a0a 2020 2020 2020  ession()..      
-00003720: 2020 7365 6c66 2e69 6e69 745f 776f 726b    self.init_work
-00003730: 666c 6f77 7328 290a 2020 2020 2020 2020  flows().        
-00003740: 7365 6c66 2e76 616c 6964 6174 6528 7661  self.validate(va
-00003750: 6c69 6461 7465 5f73 6c75 726d 5f73 6574  lidate_slurm_set
-00003760: 7570 3d69 6e69 745f 736c 7572 6d29 0a0a  up=init_slurm)..
-00003770: 2020 2020 6465 6620 696e 6974 5f77 6f72      def init_wor
-00003780: 6b66 6c6f 7773 2873 656c 662c 2066 6f72  kflows(self, for
-00003790: 6365 5f75 7064 6174 653a 2062 6f6f 6c20  ce_update: bool 
-000037a0: 3d20 4661 6c73 6529 3a0a 2020 2020 2020  = False):.      
-000037b0: 2020 2222 220a 2020 2020 2020 2020 5265    """.        Re
-000037c0: 7472 6965 7665 7320 7468 6520 7265 7175  trieves the requ
-000037d0: 6972 6564 2069 6e66 6f20 666f 7220 7468  ired info for th
-000037e0: 6520 636f 6e66 6967 7572 6564 2077 6f72  e configured wor
-000037f0: 6b66 6c6f 7773 2066 726f 6d20 6769 7468  kflows from gith
-00003800: 7562 2e0a 2020 2020 2020 2020 4974 2077  ub..        It w
-00003810: 696c 6c20 6669 6c6c 2060 736c 7572 6d5f  ill fill `slurm_
-00003820: 6d6f 6465 6c5f 696d 6167 6573 6020 7769  model_images` wi
-00003830: 7468 2064 6f63 6b65 7268 7562 206c 696e  th dockerhub lin
-00003840: 6b73 2e0a 0a20 2020 2020 2020 2041 7267  ks...        Arg
-00003850: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-00003860: 6f72 6365 5f75 7064 6174 6520 2862 6f6f  orce_update (boo
-00003870: 6c29 3a20 5769 6c6c 206f 7665 7277 7269  l): Will overwri
-00003880: 7465 2061 6c72 6561 6479 2067 6976 656e  te already given
-00003890: 2070 6174 6873 0a20 2020 2020 2020 2020   paths.         
-000038a0: 2020 2020 2020 2069 6e20 6073 6c75 726d         in `slurm
-000038b0: 5f6d 6f64 656c 5f69 6d61 6765 7360 0a0a  _model_images`..
-000038c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000038d0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-000038e0: 736c 7572 6d5f 6d6f 6465 6c5f 696d 6167  slurm_model_imag
-000038f0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00003900: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
-00003910: 5f69 6d61 6765 7320 3d20 7b7d 0a20 2020  _images = {}.   
-00003920: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00003930: 2e73 6c75 726d 5f6d 6f64 656c 5f72 6570  .slurm_model_rep
-00003940: 6f73 3a0a 2020 2020 2020 2020 2020 2020  os:.            
-00003950: 6c6f 6767 6572 2e77 6172 6e69 6e67 2822  logger.warning("
-00003960: 4e6f 2077 6f72 6b66 6c6f 7773 2063 6f6e  No workflows con
-00003970: 6669 6775 7265 6421 2229 0a20 2020 2020  figured!").     
-00003980: 2020 2020 2020 2073 656c 662e 736c 7572         self.slur
-00003990: 6d5f 6d6f 6465 6c5f 7265 706f 7320 3d20  m_model_repos = 
-000039a0: 7b7d 0a20 2020 2020 2020 2020 2020 2023  {}.            #
-000039b0: 2073 6b69 7073 2074 6865 2073 6574 7570   skips the setup
-000039c0: 0a20 2020 2020 2020 2066 6f72 2077 6f72  .        for wor
-000039d0: 6b66 6c6f 7720 696e 2073 656c 662e 736c  kflow in self.sl
-000039e0: 7572 6d5f 6d6f 6465 6c5f 7265 706f 732e  urm_model_repos.
-000039f0: 6b65 7973 2829 3a0a 2020 2020 2020 2020  keys():.        
-00003a00: 2020 2020 6966 2077 6f72 6b66 6c6f 7720      if workflow 
-00003a10: 6e6f 7420 696e 2073 656c 662e 736c 7572  not in self.slur
-00003a20: 6d5f 6d6f 6465 6c5f 696d 6167 6573 206f  m_model_images o
-00003a30: 7220 666f 7263 655f 7570 6461 7465 3a0a  r force_update:.
-00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a50: 6a73 6f6e 5f64 6573 6372 6970 746f 7220  json_descriptor 
-00003a60: 3d20 7365 6c66 2e70 756c 6c5f 6465 7363  = self.pull_desc
-00003a70: 7269 7074 6f72 5f66 726f 6d5f 6769 7468  riptor_from_gith
-00003a80: 7562 2877 6f72 6b66 6c6f 7729 0a20 2020  ub(workflow).   
-00003a90: 2020 2020 2020 2020 2020 2020 206c 6f67               log
-00003aa0: 6765 722e 6465 6275 6728 2725 733a 2025  ger.debug('%s: %
-00003ab0: 7327 2c20 776f 726b 666c 6f77 2c20 6a73  s', workflow, js
-00003ac0: 6f6e 5f64 6573 6372 6970 746f 7229 0a20  on_descriptor). 
-00003ad0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00003ae0: 6d61 6765 203d 206a 736f 6e5f 6465 7363  mage = json_desc
-00003af0: 7269 7074 6f72 5b27 636f 6e74 6169 6e65  riptor['containe
-00003b00: 722d 696d 6167 6527 5d5b 2769 6d61 6765  r-image']['image
-00003b10: 275d 0a20 2020 2020 2020 2020 2020 2020  '].             
-00003b20: 2020 2073 656c 662e 736c 7572 6d5f 6d6f     self.slurm_mo
-00003b30: 6465 6c5f 696d 6167 6573 5b77 6f72 6b66  del_images[workf
-00003b40: 6c6f 775d 203d 2069 6d61 6765 0a0a 2020  low] = image..  
-00003b50: 2020 6465 6620 7365 7475 705f 736c 7572    def setup_slur
-00003b60: 6d28 7365 6c66 293a 0a20 2020 2020 2020  m(self):.       
-00003b70: 2022 2222 0a20 2020 2020 2020 2056 616c   """.        Val
-00003b80: 6964 6174 6573 206f 7220 6372 6561 7465  idates or create
-00003b90: 7320 7468 6520 7265 7175 6972 6564 2073  s the required s
-00003ba0: 6574 7570 206f 6e20 7468 6520 536c 7572  etup on the Slur
-00003bb0: 6d20 636c 7573 7465 722e 0a0a 2020 2020  m cluster...    
-00003bc0: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-00003bd0: 2020 2020 2020 2020 5353 4845 7863 6570          SSHExcep
-00003be0: 7469 6f6e 3a20 6966 2069 7420 6361 6e6e  tion: if it cann
-00003bf0: 6f74 2063 6f6e 6e65 6374 2074 6f20 536c  ot connect to Sl
-00003c00: 7572 6d2c 206f 7220 7275 6e73 2069 6e74  urm, or runs int
-00003c10: 6f20 616e 2065 7272 6f72 0a20 2020 2020  o an error.     
-00003c20: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-00003c30: 6620 7365 6c66 2e76 616c 6964 6174 6528  f self.validate(
-00003c40: 293a 0a20 2020 2020 2020 2020 2020 2023  ):.            #
-00003c50: 2031 2e20 4372 6561 7465 2064 6972 6563   1. Create direc
-00003c60: 746f 7269 6573 0a20 2020 2020 2020 2020  tories.         
-00003c70: 2020 2073 656c 662e 7365 7475 705f 6469     self.setup_di
-00003c80: 7265 6374 6f72 6965 7328 290a 0a20 2020  rectories()..   
-00003c90: 2020 2020 2020 2020 2023 2032 2e20 436c           # 2. Cl
-00003ca0: 6f6e 6520 6769 740a 2020 2020 2020 2020  one git.        
-00003cb0: 2020 2020 7365 6c66 2e73 6574 7570 5f6a      self.setup_j
-00003cc0: 6f62 5f73 6372 6970 7473 2829 0a0a 2020  ob_scripts()..  
-00003cd0: 2020 2020 2020 2020 2020 2320 332e 2053            # 3. S
-00003ce0: 6574 7570 2063 6f6e 7665 7274 6572 730a  etup converters.
-00003cf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003d00: 2e73 6574 7570 5f63 6f6e 7665 7274 6572  .setup_converter
-00003d10: 7328 290a 0a20 2020 2020 2020 2020 2020  s()..           
-00003d20: 2023 2034 2e20 446f 776e 6c6f 6164 2077   # 4. Download w
-00003d30: 6f72 6b66 6c6f 7720 696d 6167 6573 0a20  orkflow images. 
-00003d40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00003d50: 7365 7475 705f 636f 6e74 6169 6e65 725f  setup_container_
-00003d60: 696d 6167 6573 2829 0a0a 2020 2020 2020  images()..      
-00003d70: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00003d80: 2020 2020 7261 6973 6520 5353 4845 7863      raise SSHExc
-00003d90: 6570 7469 6f6e 2822 4661 696c 7572 6520  eption("Failure 
-00003da0: 696e 2063 6f6e 6e65 6374 696e 6720 746f  in connecting to
-00003db0: 2053 6c75 726d 2063 6c75 7374 6572 2229   Slurm cluster")
-00003dc0: 0a0a 2020 2020 6465 6620 7365 7475 705f  ..    def setup_
-00003dd0: 636f 6e74 6169 6e65 725f 696d 6167 6573  container_images
-00003de0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00003df0: 2222 220a 2020 2020 2020 2020 5365 7473  """.        Sets
-00003e00: 2075 7020 636f 6e74 6169 6e65 7220 696d   up container im
-00003e10: 6167 6573 2066 6f72 2053 6c75 726d 206f  ages for Slurm o
-00003e20: 7065 7261 7469 6f6e 732e 0a0a 2020 2020  perations...    
-00003e30: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
-00003e40: 6e20 6372 6561 7465 7320 7370 6563 6966  n creates specif
-00003e50: 6963 2064 6972 6563 746f 7269 6573 2066  ic directories f
-00003e60: 6f72 2063 6f6e 7461 696e 6572 2069 6d61  or container ima
-00003e70: 6765 7320 616e 6420 7075 6c6c 730a 2020  ges and pulls.  
-00003e80: 2020 2020 2020 6e65 6365 7373 6172 7920        necessary 
-00003e90: 696d 6167 6573 2066 726f 6d20 446f 636b  images from Dock
-00003ea0: 6572 2072 6570 6f73 6974 6f72 6965 732e  er repositories.
-00003eb0: 2049 7420 6765 6e65 7261 7465 7320 616e   It generates an
-00003ec0: 6420 6578 6563 7574 6573 0a20 2020 2020  d executes.     
-00003ed0: 2020 2061 2073 6372 6970 7420 746f 2070     a script to p
-00003ee0: 756c 6c20 696d 6167 6573 2061 6e64 2063  ull images and c
-00003ef0: 6f70 6965 7320 6974 2074 6f20 7468 6520  opies it to the 
-00003f00: 7265 6d6f 7465 206c 6f63 6174 696f 6e2e  remote location.
-00003f10: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
-00003f20: 3a0a 2020 2020 2020 2020 2020 2020 5353  :.            SS
-00003f30: 4845 7863 6570 7469 6f6e 3a20 4966 2074  HException: If t
-00003f40: 6865 7265 2069 7320 616e 2069 7373 7565  here is an issue
-00003f50: 2065 7865 6375 7469 6e67 2063 6f6d 6d61   executing comma
-00003f60: 6e64 7320 6f72 2063 6f70 7969 6e67 2066  nds or copying f
-00003f70: 696c 6573 2e0a 2020 2020 2020 2020 2222  iles..        ""
-00003f80: 220a 2020 2020 2020 2020 2320 4372 6561  ".        # Crea
-00003f90: 7465 2073 7065 6369 6669 6320 776f 726b  te specific work
-00003fa0: 666c 6f77 2064 6972 730a 2020 2020 2020  flow dirs.      
-00003fb0: 2020 7769 7468 2073 656c 662e 6364 2873    with self.cd(s
-00003fc0: 656c 662e 736c 7572 6d5f 696d 6167 6573  elf.slurm_images
-00003fd0: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
-00003fe0: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
-00003ff0: 6d5f 6d6f 6465 6c5f 7061 7468 733a 0a20  m_model_paths:. 
-00004000: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-00004010: 6f64 656c 7061 7468 7320 3d20 2220 222e  odelpaths = " ".
-00004020: 6a6f 696e 2873 656c 662e 736c 7572 6d5f  join(self.slurm_
-00004030: 6d6f 6465 6c5f 7061 7468 732e 7661 6c75  model_paths.valu
-00004040: 6573 2829 290a 2020 2020 2020 2020 2020  es()).          
-00004050: 2020 2020 2020 2320 6d6b 6469 7220 6365        # mkdir ce
-00004060: 6c6c 7072 6f66 696c 6572 2069 6d61 6765  llprofiler image
-00004070: 6a20 2e2e 2e0a 2020 2020 2020 2020 2020  j ....          
-00004080: 2020 2020 2020 7220 3d20 7365 6c66 2e72        r = self.r
-00004090: 756e 5f63 6f6d 6d61 6e64 7328 5b66 226d  un_commands([f"m
-000040a0: 6b64 6972 202d 7020 7b6d 6f64 656c 7061  kdir -p {modelpa
-000040b0: 7468 737d 225d 290a 2020 2020 2020 2020  ths}"]).        
-000040c0: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-000040d0: 2e6f 6b3a 0a20 2020 2020 2020 2020 2020  .ok:.           
-000040e0: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-000040f0: 5348 4578 6365 7074 696f 6e28 7229 0a0a  SHException(r)..
-00004100: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00004110: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
-00004120: 696d 6167 6573 3a0a 2020 2020 2020 2020  images:.        
-00004130: 2020 2020 2020 2020 7075 6c6c 5f63 6f6d          pull_com
-00004140: 6d61 6e64 7320 3d20 5b5d 0a20 2020 2020  mands = [].     
-00004150: 2020 2020 2020 2020 2020 2066 6f72 2077             for w
-00004160: 662c 2069 6d61 6765 2069 6e20 7365 6c66  f, image in self
-00004170: 2e73 6c75 726d 5f6d 6f64 656c 5f69 6d61  .slurm_model_ima
-00004180: 6765 732e 6974 656d 7328 293a 0a20 2020  ges.items():.   
-00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041a0: 2072 6570 6f20 3d20 7365 6c66 2e73 6c75   repo = self.slu
-000041b0: 726d 5f6d 6f64 656c 5f72 6570 6f73 5b77  rm_model_repos[w
-000041c0: 665d 0a20 2020 2020 2020 2020 2020 2020  f].             
-000041d0: 2020 2020 2020 2070 6174 6820 3d20 7365         path = se
-000041e0: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f70  lf.slurm_model_p
-000041f0: 6174 6873 5b77 665d 0a20 2020 2020 2020  aths[wf].       
-00004200: 2020 2020 2020 2020 2020 2020 205f 2c20               _, 
-00004210: 7665 7273 696f 6e20 3d20 7365 6c66 2e65  version = self.e
-00004220: 7874 7261 6374 5f70 6172 7473 5f66 726f  xtract_parts_fro
-00004230: 6d5f 7572 6c28 7265 706f 290a 2020 2020  m_url(repo).    
-00004240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004250: 6966 2076 6572 7369 6f6e 203d 3d20 226d  if version == "m
-00004260: 6173 7465 7222 3a0a 2020 2020 2020 2020  aster":.        
-00004270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004280: 7665 7273 696f 6e20 3d20 226c 6174 6573  version = "lates
-00004290: 7422 0a20 2020 2020 2020 2020 2020 2020  t".             
-000042a0: 2020 2020 2020 2070 756c 6c5f 7465 6d70         pull_temp
-000042b0: 6c61 7465 203d 2022 6563 686f 2027 7374  late = "echo 'st
-000042c0: 6172 7469 6e67 2024 7061 7468 2024 7665  arting $path $ve
-000042d0: 7273 696f 6e27 203e 3e20 7369 6e67 2e6c  rsion' >> sing.l
-000042e0: 6f67 5c6e 6e6f 6875 7020 7368 202d 6320  og\nnohup sh -c 
-000042f0: 5c22 7369 6e67 756c 6172 6974 7920 7075  \"singularity pu
-00004300: 6c6c 202d 2d64 6973 6162 6c65 2d63 6163  ll --disable-cac
-00004310: 6865 202d 2d64 6972 2024 7061 7468 2064  he --dir $path d
-00004320: 6f63 6b65 723a 2f2f 2469 6d61 6765 3a24  ocker://$image:$
-00004330: 7665 7273 696f 6e3b 2065 6368 6f20 2766  version; echo 'f
-00004340: 696e 6973 6865 6420 2470 6174 6820 2476  inished $path $v
-00004350: 6572 7369 6f6e 275c 2220 3e3e 2073 696e  ersion'\" >> sin
-00004360: 672e 6c6f 6720 323e 2631 2026 2064 6973  g.log 2>&1 & dis
-00004370: 6f77 6e22 0a20 2020 2020 2020 2020 2020  own".           
-00004380: 2020 2020 2020 2020 2074 203d 2054 656d           t = Tem
-00004390: 706c 6174 6528 7075 6c6c 5f74 656d 706c  plate(pull_templ
-000043a0: 6174 6529 0a20 2020 2020 2020 2020 2020  ate).           
-000043b0: 2020 2020 2020 2020 2073 7562 7374 6974           substit
-000043c0: 7574 6573 203d 207b 7d0a 2020 2020 2020  utes = {}.      
-000043d0: 2020 2020 2020 2020 2020 2020 2020 7375                su
-000043e0: 6273 7469 7475 7465 735b 2770 6174 6827  bstitutes['path'
-000043f0: 5d20 3d20 7061 7468 0a20 2020 2020 2020  ] = path.       
-00004400: 2020 2020 2020 2020 2020 2020 2073 7562               sub
-00004410: 7374 6974 7574 6573 5b27 696d 6167 6527  stitutes['image'
-00004420: 5d20 3d20 696d 6167 650a 2020 2020 2020  ] = image.      
-00004430: 2020 2020 2020 2020 2020 2020 2020 7375                su
-00004440: 6273 7469 7475 7465 735b 2776 6572 7369  bstitutes['versi
-00004450: 6f6e 275d 203d 2076 6572 7369 6f6e 0a20  on'] = version. 
-00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004470: 2020 2063 6d64 203d 2074 2e73 6166 655f     cmd = t.safe_
-00004480: 7375 6273 7469 7475 7465 2873 7562 7374  substitute(subst
-00004490: 6974 7574 6573 290a 2020 2020 2020 2020  itutes).        
-000044a0: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-000044b0: 6572 2e64 6562 7567 2866 2273 7562 7374  er.debug(f"subst
-000044c0: 6974 7574 6564 3a20 7b63 6d64 7d22 290a  ituted: {cmd}").
-000044d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044e0: 2020 2020 7075 6c6c 5f63 6f6d 6d61 6e64      pull_command
-000044f0: 732e 6170 7065 6e64 2863 6d64 290a 2020  s.append(cmd).  
-00004500: 2020 2020 2020 2020 2020 2020 2020 7363                sc
-00004510: 7269 7074 5f6e 616d 6520 3d20 2270 756c  ript_name = "pul
-00004520: 6c5f 696d 6167 6573 2e73 6822 0a20 2020  l_images.sh".   
-00004530: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-00004540: 706c 6174 655f 7363 7269 7074 203d 2066  plate_script = f
-00004550: 696c 6573 2822 7265 736f 7572 6365 7322  iles("resources"
-00004560: 292e 6a6f 696e 7061 7468 2873 6372 6970  ).joinpath(scrip
-00004570: 745f 6e61 6d65 290a 2020 2020 2020 2020  t_name).        
-00004580: 2020 2020 2020 2020 7769 7468 2074 656d          with tem
-00004590: 706c 6174 655f 7363 7269 7074 2e6f 7065  plate_script.ope
-000045a0: 6e28 2772 2729 2061 7320 663a 0a20 2020  n('r') as f:.   
-000045b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000045c0: 2073 7263 203d 2054 656d 706c 6174 6528   src = Template(
-000045d0: 662e 7265 6164 2829 290a 2020 2020 2020  f.read()).      
-000045e0: 2020 2020 2020 2020 2020 2020 2020 7375                su
-000045f0: 6273 7469 7475 7465 203d 207b 2770 756c  bstitute = {'pul
-00004600: 6c63 6f6d 6d61 6e64 7327 3a20 225c 6e22  lcommands': "\n"
-00004610: 2e6a 6f69 6e28 7075 6c6c 5f63 6f6d 6d61  .join(pull_comma
-00004620: 6e64 7329 7d0a 2020 2020 2020 2020 2020  nds)}.          
-00004630: 2020 2020 2020 2020 2020 6a6f 625f 7363            job_sc
-00004640: 7269 7074 203d 2073 7263 2e73 6166 655f  ript = src.safe_
-00004650: 7375 6273 7469 7475 7465 2873 7562 7374  substitute(subst
-00004660: 6974 7574 6529 0a20 2020 2020 2020 2020  itute).         
-00004670: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-00004680: 6275 6728 6622 7375 6273 7469 7475 7465  bug(f"substitute
-00004690: 643a 5c6e 207b 6a6f 625f 7363 7269 7074  d:\n {job_script
-000046a0: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
-000046b0: 2020 2020 2320 636f 7079 2074 6f20 7265      # copy to re
-000046c0: 6d6f 7465 2066 696c 650a 2020 2020 2020  mote file.      
-000046d0: 2020 2020 2020 2020 2020 6675 6c6c 5f70            full_p
-000046e0: 6174 6820 3d20 7365 6c66 2e73 6c75 726d  ath = self.slurm
-000046f0: 5f69 6d61 6765 735f 7061 7468 2b22 2f22  _images_path+"/"
-00004700: 2b73 6372 6970 745f 6e61 6d65 0a20 2020  +script_name.   
-00004710: 2020 2020 2020 2020 2020 2020 205f 203d               _ =
-00004720: 2073 656c 662e 7075 7428 6c6f 6361 6c3d   self.put(local=
-00004730: 696f 2e53 7472 696e 6749 4f28 6a6f 625f  io.StringIO(job_
-00004740: 7363 7269 7074 292c 0a20 2020 2020 2020  script),.       
-00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004760: 2020 2020 2020 7265 6d6f 7465 3d66 756c        remote=ful
-00004770: 6c5f 7061 7468 290a 2020 2020 2020 2020  l_path).        
-00004780: 2020 2020 2020 2020 636d 6420 3d20 6622          cmd = f"
-00004790: 7469 6d65 2073 6820 7b73 6372 6970 745f  time sh {script_
-000047a0: 6e61 6d65 7d22 0a20 2020 2020 2020 2020  name}".         
-000047b0: 2020 2020 2020 2072 203d 2073 656c 662e         r = self.
-000047c0: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
-000047d0: 645d 290a 2020 2020 2020 2020 2020 2020  d]).            
-000047e0: 2020 2020 6966 206e 6f74 2072 2e6f 6b3a      if not r.ok:
-000047f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004800: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
-00004810: 6365 7074 696f 6e28 7229 0a20 2020 2020  ception(r).     
-00004820: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00004830: 722e 696e 666f 2872 2e73 7464 6f75 7429  r.info(r.stdout)
-00004840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004850: 206c 6f67 6765 722e 696e 666f 2822 496e   logger.info("In
-00004860: 6974 6961 7465 6420 646f 776e 6c6f 6164  itiated download
-00004870: 696e 6720 616e 6420 6275 696c 6469 6e67  ing and building
-00004880: 2220 2b0a 2020 2020 2020 2020 2020 2020  " +.            
-00004890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048a0: 2220 636f 6e74 6169 6e65 7220 696d 6167  " container imag
-000048b0: 6573 206f 6e20 536c 7572 6d2e 2220 2b0a  es on Slurm." +.
-000048c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000048d0: 2020 2020 2020 2020 2020 2020 2220 5468              " Th
-000048e0: 6973 2077 696c 6c20 7461 6b65 2061 2077  is will take a w
-000048f0: 6869 6c65 2069 6e20 7468 6520 6261 636b  hile in the back
-00004900: 6772 6f75 6e64 2e22 202b 200a 2020 2020  ground." + .    
-00004910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004920: 2020 2020 2020 2020 2220 4368 6563 6b20          " Check 
-00004930: 2773 696e 672e 6c6f 6727 206f 6e20 536c  'sing.log' on Sl
-00004940: 7572 6d20 666f 7220 7072 6f67 7265 7373  urm for progress
-00004950: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-00004960: 2020 2020 2320 2320 636c 6561 6e75 7020      # # cleanup 
-00004970: 6769 616e 7420 7369 6e67 756c 6172 6974  giant singularit
-00004980: 7920 6361 6368 6521 0a20 2020 2020 2020  y cache!.       
-00004990: 2020 2020 2020 2020 2023 2075 7369 6e67           # using
-000049a0: 202d 2d64 6973 6162 6c65 2d63 6163 6865   --disable-cache
-000049b0: 2062 6563 6175 7365 2077 6520 7275 6e20   because we run 
-000049c0: 696e 2074 6865 2062 6163 6b67 726f 756e  in the backgroun
-000049d0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-000049e0: 2020 2320 636d 6420 3d20 2273 696e 6775    # cmd = "singu
-000049f0: 6c61 7269 7479 2063 6163 6865 2063 6c65  larity cache cle
-00004a00: 616e 202d 6622 0a20 2020 2020 2020 2020  an -f".         
-00004a10: 2020 2020 2020 2023 2072 203d 2073 656c         # r = sel
-00004a20: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
-00004a30: 636d 645d 290a 0a20 2020 2064 6566 2073  cmd])..    def s
-00004a40: 6574 7570 5f63 6f6e 7665 7274 6572 7328  etup_converters(
-00004a50: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00004a60: 2222 0a20 2020 2020 2020 2053 6574 7320  "".        Sets 
-00004a70: 7570 2063 6f6e 7665 7274 6572 7320 666f  up converters fo
-00004a80: 7220 536c 7572 6d20 6f70 6572 6174 696f  r Slurm operatio
-00004a90: 6e73 2e0a 0a20 2020 2020 2020 2054 6869  ns...        Thi
-00004aa0: 7320 6675 6e63 7469 6f6e 2063 7265 6174  s function creat
-00004ab0: 6573 206e 6563 6573 7361 7279 2064 6972  es necessary dir
-00004ac0: 6563 746f 7269 6573 2066 6f72 2063 6f6e  ectories for con
-00004ad0: 7665 7274 6572 7320 616e 6420 636f 7069  verters and copi
-00004ae0: 6573 0a20 2020 2020 2020 2063 6f6e 7665  es.        conve
-00004af0: 7274 6572 2073 6372 6970 7473 2061 6e64  rter scripts and
-00004b00: 2064 6566 696e 6974 696f 6e73 2074 6f20   definitions to 
-00004b10: 7468 6520 6170 7072 6f70 7269 6174 6520  the appropriate 
-00004b20: 6c6f 6361 7469 6f6e 732e 2049 7420 616c  locations. It al
-00004b30: 736f 0a20 2020 2020 2020 2062 7569 6c64  so.        build
-00004b40: 7320 5369 6e67 756c 6172 6974 7920 636f  s Singularity co
-00004b50: 6e74 6169 6e65 7273 2066 726f 6d20 7468  ntainers from th
-00004b60: 6520 7072 6f76 6964 6564 2064 6566 696e  e provided defin
-00004b70: 6974 696f 6e73 2e0a 0a20 2020 2020 2020  itions...       
-00004b80: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-00004b90: 2020 2020 2053 5348 4578 6365 7074 696f       SSHExceptio
-00004ba0: 6e3a 2049 6620 7468 6572 6520 6973 2061  n: If there is a
-00004bb0: 6e20 6973 7375 6520 6578 6563 7574 696e  n issue executin
-00004bc0: 6720 636f 6d6d 616e 6473 206f 7220 636f  g commands or co
-00004bd0: 7079 696e 6720 6669 6c65 732e 0a20 2020  pying files..   
-00004be0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00004bf0: 2063 6f6e 7665 7274 5f63 6d64 7320 3d20   convert_cmds = 
-00004c00: 5b5d 0a20 2020 2020 2020 2069 6620 7365  [].        if se
-00004c10: 6c66 2e73 6c75 726d 5f63 6f6e 7665 7274  lf.slurm_convert
-00004c20: 6572 735f 7061 7468 3a0a 2020 2020 2020  ers_path:.      
-00004c30: 2020 2020 2020 636f 6e76 6572 745f 636d        convert_cm
-00004c40: 6473 2e61 7070 656e 6428 6622 6d6b 6469  ds.append(f"mkdi
-00004c50: 7220 2d70 207b 7365 6c66 2e73 6c75 726d  r -p {self.slurm
-00004c60: 5f63 6f6e 7665 7274 6572 735f 7061 7468  _converters_path
-00004c70: 7d22 290a 2020 2020 2020 2020 7220 3d20  }").        r = 
-00004c80: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-00004c90: 7328 636f 6e76 6572 745f 636d 6473 290a  s(convert_cmds).
-00004ca0: 2020 2020 2020 2020 2320 636f 7079 2067          # copy g
-00004cb0: 656e 6572 6963 206a 6f62 2061 7272 6179  eneric job array
-00004cc0: 2073 6372 6970 7420 6f76 6572 2074 6f20   script over to 
-00004cd0: 736c 7572 6d0a 2020 2020 2020 2020 636f  slurm.        co
-00004ce0: 6e76 6572 745f 6a6f 625f 6c6f 6361 6c20  nvert_job_local 
-00004cf0: 3d20 6669 6c65 7328 2272 6573 6f75 7263  = files("resourc
-00004d00: 6573 2229 2e6a 6f69 6e70 6174 6828 0a20  es").joinpath(. 
-00004d10: 2020 2020 2020 2020 2020 2022 636f 6e76             "conv
-00004d20: 6572 745f 6a6f 625f 6172 7261 792e 7368  ert_job_array.sh
-00004d30: 2229 0a20 2020 2020 2020 205f 203d 2073  ").        _ = s
-00004d40: 656c 662e 7075 7428 6c6f 6361 6c3d 636f  elf.put(local=co
-00004d50: 6e76 6572 745f 6a6f 625f 6c6f 6361 6c2c  nvert_job_local,
-00004d60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004d70: 2020 2020 2020 7265 6d6f 7465 3d73 656c        remote=sel
-00004d80: 662e 736c 7572 6d5f 7363 7269 7074 5f70  f.slurm_script_p
-00004d90: 6174 6829 0a20 2020 2020 2020 2023 2063  ath).        # c
-00004da0: 7572 7265 6e74 6c79 206b 6e6f 776e 2063  urrently known c
-00004db0: 6f6e 7665 7274 6572 730a 2020 2020 2020  onverters.      
-00004dc0: 2020 2320 3361 2e20 5a41 5252 2074 6f20    # 3a. ZARR to 
-00004dd0: 5449 4646 0a20 2020 2020 2020 2023 2054  TIFF.        # T
-00004de0: 4f44 4f20 6578 7472 6163 7420 7468 6573  ODO extract thes
-00004df0: 6520 7661 6c75 6573 2074 6f20 652e 672e  e values to e.g.
-00004e00: 2063 6f6e 6669 6720 6966 2077 6520 6861   config if we ha
-00004e10: 7665 206d 6f72 650a 2020 2020 2020 2020  ve more.        
-00004e20: 636f 6e76 6572 745f 6e61 6d65 203d 2022  convert_name = "
-00004e30: 636f 6e76 6572 745f 7a61 7272 5f74 6f5f  convert_zarr_to_
-00004e40: 7469 6666 220a 2020 2020 2020 2020 636f  tiff".        co
-00004e50: 6e76 6572 745f 7079 203d 2066 227b 636f  nvert_py = f"{co
-00004e60: 6e76 6572 745f 6e61 6d65 7d2e 7079 220a  nvert_name}.py".
-00004e70: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
-00004e80: 7363 7269 7074 5f6c 6f63 616c 203d 2066  script_local = f
-00004e90: 696c 6573 2822 7265 736f 7572 6365 7322  iles("resources"
-00004ea0: 292e 6a6f 696e 7061 7468 280a 2020 2020  ).joinpath(.    
-00004eb0: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
-00004ec0: 7079 290a 2020 2020 2020 2020 636f 6e76  py).        conv
-00004ed0: 6572 745f 6465 6620 3d20 6622 7b63 6f6e  ert_def = f"{con
-00004ee0: 7665 7274 5f6e 616d 657d 2e64 6566 220a  vert_name}.def".
-00004ef0: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
-00004f00: 6465 665f 6c6f 6361 6c20 3d20 6669 6c65  def_local = file
-00004f10: 7328 2272 6573 6f75 7263 6573 2229 2e6a  s("resources").j
-00004f20: 6f69 6e70 6174 6828 0a20 2020 2020 2020  oinpath(.       
-00004f30: 2020 2020 2063 6f6e 7665 7274 5f64 6566       convert_def
-00004f40: 290a 2020 2020 2020 2020 5f20 3d20 7365  ).        _ = se
-00004f50: 6c66 2e70 7574 286c 6f63 616c 3d63 6f6e  lf.put(local=con
-00004f60: 7665 7274 5f73 6372 6970 745f 6c6f 6361  vert_script_loca
-00004f70: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-00004f80: 2020 2020 2020 2020 7265 6d6f 7465 3d73          remote=s
-00004f90: 656c 662e 736c 7572 6d5f 636f 6e76 6572  elf.slurm_conver
-00004fa0: 7465 7273 5f70 6174 6829 0a20 2020 2020  ters_path).     
-00004fb0: 2020 205f 203d 2073 656c 662e 7075 7428     _ = self.put(
-00004fc0: 6c6f 6361 6c3d 636f 6e76 6572 745f 6465  local=convert_de
-00004fd0: 665f 6c6f 6361 6c2c 0a20 2020 2020 2020  f_local,.       
-00004fe0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00004ff0: 6d6f 7465 3d73 656c 662e 736c 7572 6d5f  mote=self.slurm_
-00005000: 636f 6e76 6572 7465 7273 5f70 6174 6829  converters_path)
-00005010: 0a20 2020 2020 2020 2023 2042 7569 6c64  .        # Build
-00005020: 2073 696e 6775 6c61 7269 7479 2063 6f6e   singularity con
-00005030: 7461 696e 6572 2066 726f 6d20 6465 6669  tainer from defi
-00005040: 6e69 7469 6f6e 0a20 2020 2020 2020 2077  nition.        w
-00005050: 6974 6820 7365 6c66 2e63 6428 7365 6c66  ith self.cd(self
-00005060: 2e73 6c75 726d 5f63 6f6e 7665 7274 6572  .slurm_converter
-00005070: 735f 7061 7468 293a 0a20 2020 2020 2020  s_path):.       
-00005080: 2020 2020 2063 6f6e 7665 7274 5f63 6d64       convert_cmd
-00005090: 7320 3d20 5b5d 0a20 2020 2020 2020 2020  s = [].         
-000050a0: 2020 2069 6620 7365 6c66 2e73 6c75 726d     if self.slurm
-000050b0: 5f69 6d61 6765 735f 7061 7468 3a0a 2020  _images_path:.  
-000050c0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-000050d0: 544f 444f 2043 6861 6e67 6520 7468 6520  TODO Change the 
-000050e0: 746d 7020 6469 723f 0a20 2020 2020 2020  tmp dir?.       
-000050f0: 2020 2020 2020 2020 2023 2065 7870 6f72           # expor
-00005100: 7420 5349 4e47 554c 4152 4954 595f 544d  t SINGULARITY_TM
-00005110: 5044 4952 3d7e 2f6d 792d 7363 7261 7463  PDIR=~/my-scratc
-00005120: 682f 746d 703b 0a20 2020 2020 2020 2020  h/tmp;.         
-00005130: 2020 2020 2020 2023 206f 6e6c 7920 6966         # only if
-00005140: 2066 696c 6520 646f 6573 206e 6f74 2065   file does not e
-00005150: 7869 7374 2079 6574 0a20 2020 2020 2020  xist yet.       
-00005160: 2020 2020 2020 2020 2023 2063 6f6e 7665           # conve
-00005170: 7274 5f63 6d64 732e 6170 7065 6e64 2866  rt_cmds.append(f
-00005180: 225b 2021 202d 6620 7b63 6f6e 7665 7274  "[ ! -f {convert
-00005190: 5f6e 616d 657d 2e73 6966 205d 2229 0a20  _name}.sif ]"). 
-000051a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000051b0: 2045 4449 5420 2d2d 204e 4f2c 2074 6865   EDIT -- NO, the
-000051c0: 6e20 7765 2063 616e 2774 2075 7064 6174  n we can't updat
-000051d0: 6521 2046 6f72 6365 2072 6562 7569 6c64  e! Force rebuild
-000051e0: 210a 2020 2020 2020 2020 2020 2020 2020  !.              
-000051f0: 2020 2320 646f 776e 6c6f 6164 202f 6275    # download /bu
-00005200: 696c 6420 6e65 7720 636f 6e74 6169 6e65  ild new containe
-00005210: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-00005220: 2020 636f 6e76 6572 745f 636d 6473 2e61    convert_cmds.a
-00005230: 7070 656e 6428 0a20 2020 2020 2020 2020  ppend(.         
-00005240: 2020 2020 2020 2020 2020 2066 2273 696e             f"sin
-00005250: 6775 6c61 7269 7479 2062 7569 6c64 202d  gularity build -
-00005260: 4620 7b63 6f6e 7665 7274 5f6e 616d 657d  F {convert_name}
-00005270: 2e73 6966 207b 636f 6e76 6572 745f 6465  .sif {convert_de
-00005280: 667d 203e 3e20 7369 6e67 2e6c 6f67 2032  f} >> sing.log 2
-00005290: 3e26 3120 3b20 6563 686f 2027 6669 6e69  >&1 ; echo 'fini
-000052a0: 7368 6564 207b 636f 6e76 6572 745f 6e61  shed {convert_na
-000052b0: 6d65 7d2e 7369 6627 2026 2229 0a20 2020  me}.sif' &").   
-000052c0: 2020 2020 2020 2020 2072 203d 2073 656c           r = sel
-000052d0: 662e 7275 6e5f 636f 6d6d 616e 6473 2863  f.run_commands(c
-000052e0: 6f6e 7665 7274 5f63 6d64 7329 0a0a 2020  onvert_cmds)..  
-000052f0: 2020 6465 6620 7365 7475 705f 6a6f 625f    def setup_job_
-00005300: 7363 7269 7074 7328 7365 6c66 293a 0a20  scripts(self):. 
-00005310: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005320: 2020 2053 6574 7320 7570 206a 6f62 2073     Sets up job s
-00005330: 6372 6970 7473 2066 6f72 2053 6c75 726d  cripts for Slurm
-00005340: 206f 7065 7261 7469 6f6e 732e 0a0a 2020   operations...  
-00005350: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
-00005360: 696f 6e20 6569 7468 6572 2063 6c6f 6e65  ion either clone
-00005370: 7320 6120 4769 7420 7265 706f 7369 746f  s a Git reposito
-00005380: 7279 2063 6f6e 7461 696e 696e 6720 6a6f  ry containing jo
-00005390: 6220 7363 7269 7074 730a 2020 2020 2020  b scripts.      
-000053a0: 2020 696e 746f 2074 6865 2073 7065 6369    into the speci
-000053b0: 6669 6564 2073 6372 6970 7420 7061 7468  fied script path
-000053c0: 206f 7220 6765 6e65 7261 7465 7320 7363   or generates sc
-000053d0: 7269 7074 7320 6c6f 6361 6c6c 7920 6966  ripts locally if
-000053e0: 206e 6f20 7265 706f 7369 746f 7279 0a20   no repository. 
-000053f0: 2020 2020 2020 2069 7320 7072 6f76 6964         is provid
-00005400: 6564 2e0a 0a20 2020 2020 2020 2052 6169  ed...        Rai
-00005410: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
-00005420: 2053 5348 4578 6365 7074 696f 6e3a 2049   SSHException: I
-00005430: 6620 7468 6572 6520 6973 2061 6e20 6973  f there is an is
-00005440: 7375 6520 6578 6563 7574 696e 6720 4769  sue executing Gi
-00005450: 7420 636f 6d6d 616e 6473 206f 7220 6765  t commands or ge
-00005460: 6e65 7261 7469 6e67 2073 6372 6970 7473  nerating scripts
-00005470: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00005480: 2020 2020 2020 6966 2073 656c 662e 736c        if self.sl
-00005490: 7572 6d5f 7363 7269 7074 5f72 6570 6f20  urm_script_repo 
-000054a0: 616e 6420 7365 6c66 2e73 6c75 726d 5f73  and self.slurm_s
-000054b0: 6372 6970 745f 7061 7468 3a0a 2020 2020  cript_path:.    
-000054c0: 2020 2020 2020 2020 2320 6769 7420 636c          # git cl
-000054d0: 6f6e 6520 696e 746f 2073 6372 6970 7420  one into script 
-000054e0: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
-000054f0: 2065 6e76 203d 207b 0a20 2020 2020 2020   env = {.       
-00005500: 2020 2020 2020 2020 2022 5245 504f 5352           "REPOSR
-00005510: 4322 3a20 7365 6c66 2e73 6c75 726d 5f73  C": self.slurm_s
-00005520: 6372 6970 745f 7265 706f 2c0a 2020 2020  cript_repo,.    
-00005530: 2020 2020 2020 2020 2020 2020 224c 4f43              "LOC
-00005540: 414c 5245 504f 223a 2073 656c 662e 736c  ALREPO": self.sl
-00005550: 7572 6d5f 7363 7269 7074 5f70 6174 680a  urm_script_path.
-00005560: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00005570: 2020 2020 2020 2020 2020 636d 6420 3d20            cmd = 
-00005580: 2767 6974 2063 6c6f 6e65 2022 2452 4550  'git clone "$REP
-00005590: 4f53 5243 2220 2224 4c4f 4341 4c52 4550  OSRC" "$LOCALREP
-000055a0: 4f22 2032 3e20 2f64 6576 2f6e 756c 6c20  O" 2> /dev/null 
-000055b0: 7c7c 2067 6974 202d 4320 2224 4c4f 4341  || git -C "$LOCA
-000055c0: 4c52 4550 4f22 2070 756c 6c27 0a20 2020  LREPO" pull'.   
-000055d0: 2020 2020 2020 2020 2072 203d 2073 656c           r = sel
-000055e0: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
-000055f0: 636d 645d 2c20 656e 7629 0a20 2020 2020  cmd], env).     
-00005600: 2020 2020 2020 2069 6620 6e6f 7420 722e         if not r.
-00005610: 6f6b 3a0a 2020 2020 2020 2020 2020 2020  ok:.            
-00005620: 2020 2020 7261 6973 6520 5353 4845 7863      raise SSHExc
-00005630: 6570 7469 6f6e 2872 290a 2020 2020 2020  eption(r).      
-00005640: 2020 656c 6966 2073 656c 662e 736c 7572    elif self.slur
-00005650: 6d5f 7363 7269 7074 5f70 6174 683a 0a20  m_script_path:. 
-00005660: 2020 2020 2020 2020 2020 2023 2067 656e             # gen
-00005670: 6572 6174 6520 7363 7269 7074 730a 2020  erate scripts.  
-00005680: 2020 2020 2020 2020 2020 7365 6c66 2e75            self.u
-00005690: 7064 6174 655f 736c 7572 6d5f 7363 7269  pdate_slurm_scri
-000056a0: 7074 7328 6765 6e65 7261 7465 5f6a 6f62  pts(generate_job
-000056b0: 733d 5472 7565 290a 0a20 2020 2064 6566  s=True)..    def
-000056c0: 2073 6574 7570 5f64 6972 6563 746f 7269   setup_directori
-000056d0: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
-000056e0: 2020 2222 220a 2020 2020 2020 2020 4372    """.        Cr
-000056f0: 6561 7465 7320 6e65 6365 7373 6172 7920  eates necessary 
-00005700: 6469 7265 6374 6f72 6965 7320 666f 7220  directories for 
-00005710: 536c 7572 6d20 6f70 6572 6174 696f 6e73  Slurm operations
-00005720: 2e0a 0a20 2020 2020 2020 2054 6869 7320  ...        This 
-00005730: 6675 6e63 7469 6f6e 2063 7265 6174 6573  function creates
-00005740: 2064 6972 6563 746f 7269 6573 2066 6f72   directories for
-00005750: 2064 6174 6120 7374 6f72 6167 652c 2073   data storage, s
-00005760: 6372 6970 7473 2c20 616e 6420 776f 726b  cripts, and work
-00005770: 666c 6f77 730a 2020 2020 2020 2020 6173  flows.        as
-00005780: 2073 7065 6369 6669 6564 2069 6e20 7468   specified in th
-00005790: 6520 536c 7572 6d43 6c69 656e 7420 6f62  e SlurmClient ob
-000057a0: 6a65 6374 2e0a 0a20 2020 2020 2020 2052  ject...        R
-000057b0: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
-000057c0: 2020 2053 5348 4578 6365 7074 696f 6e3a     SSHException:
-000057d0: 2049 6620 7468 6572 6520 6973 2061 6e20   If there is an 
-000057e0: 6973 7375 6520 6578 6563 7574 696e 6720  issue executing 
-000057f0: 6469 7265 6374 6f72 7920 6372 6561 7469  directory creati
-00005800: 6f6e 2063 6f6d 6d61 6e64 732e 0a20 2020  on commands..   
-00005810: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005820: 2064 6972 5f63 6d64 7320 3d20 5b5d 0a20   dir_cmds = []. 
-00005830: 2020 2020 2020 2023 2061 2e20 6461 7461         # a. data
-00005840: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00005850: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
-00005860: 3a0a 2020 2020 2020 2020 2020 2020 6469  :.            di
-00005870: 725f 636d 6473 2e61 7070 656e 6428 6622  r_cmds.append(f"
-00005880: 6d6b 6469 7220 2d70 207b 7365 6c66 2e73  mkdir -p {self.s
-00005890: 6c75 726d 5f64 6174 615f 7061 7468 7d22  lurm_data_path}"
-000058a0: 290a 2020 2020 2020 2020 2020 2020 2320  ).            # 
-000058b0: 622e 2073 6372 6970 7473 0a20 2020 2020  b. scripts.     
-000058c0: 2020 2069 6620 7365 6c66 2e73 6c75 726d     if self.slurm
-000058d0: 5f73 6372 6970 745f 7061 7468 3a0a 2020  _script_path:.  
-000058e0: 2020 2020 2020 2020 2020 6469 725f 636d            dir_cm
-000058f0: 6473 2e61 7070 656e 6428 6622 6d6b 6469  ds.append(f"mkdi
-00005900: 7220 2d70 207b 7365 6c66 2e73 6c75 726d  r -p {self.slurm
-00005910: 5f73 6372 6970 745f 7061 7468 7d22 290a  _script_path}").
-00005920: 2020 2020 2020 2020 2020 2020 2320 632e              # c.
-00005930: 2077 6f72 6b66 6c6f 7773 0a20 2020 2020   workflows.     
-00005940: 2020 2069 6620 7365 6c66 2e73 6c75 726d     if self.slurm
-00005950: 5f69 6d61 6765 735f 7061 7468 3a0a 2020  _images_path:.  
-00005960: 2020 2020 2020 2020 2020 6469 725f 636d            dir_cm
-00005970: 6473 2e61 7070 656e 6428 6622 6d6b 6469  ds.append(f"mkdi
-00005980: 7220 2d70 207b 7365 6c66 2e73 6c75 726d  r -p {self.slurm
-00005990: 5f69 6d61 6765 735f 7061 7468 7d22 290a  _images_path}").
-000059a0: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
-000059b0: 2e72 756e 5f63 6f6d 6d61 6e64 7328 6469  .run_commands(di
-000059c0: 725f 636d 6473 290a 2020 2020 2020 2020  r_cmds).        
-000059d0: 6966 206e 6f74 2072 2e6f 6b3a 0a20 2020  if not r.ok:.   
-000059e0: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-000059f0: 5348 4578 6365 7074 696f 6e28 7229 0a0a  SHException(r)..
-00005a00: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00005a10: 0a20 2020 2064 6566 2066 726f 6d5f 636f  .    def from_co
-00005a20: 6e66 6967 2863 6c73 2c20 636f 6e66 6967  nfig(cls, config
-00005a30: 6669 6c65 3a20 7374 7220 3d20 2727 2c0a  file: str = '',.
-00005a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a50: 2020 2020 696e 6974 5f73 6c75 726d 3a20      init_slurm: 
-00005a60: 626f 6f6c 203d 2046 616c 7365 2920 2d3e  bool = False) ->
-00005a70: 2027 536c 7572 6d43 6c69 656e 7427 3a0a   'SlurmClient':.
-00005a80: 2020 2020 2020 2020 2222 2243 7265 6174          """Creat
-00005a90: 6573 2061 206e 6577 2053 6c75 726d 436c  es a new SlurmCl
-00005aa0: 6965 6e74 206f 626a 6563 7420 7573 696e  ient object usin
-00005ab0: 6720 7468 6520 7061 7261 6d65 7465 7273  g the parameters
-00005ac0: 2072 6561 6420 6672 6f6d 2061 0a20 2020   read from a.   
-00005ad0: 2020 2020 2063 6f6e 6669 6775 7261 7469       configurati
-00005ae0: 6f6e 2066 696c 6520 282e 696e 6929 2e0a  on file (.ini)..
-00005af0: 0a20 2020 2020 2020 2044 6566 6175 6c74  .        Default
-00005b00: 7320 7061 7468 7320 746f 206c 6f6f 6b20  s paths to look 
-00005b10: 666f 7220 636f 6e66 6967 2066 696c 6573  for config files
-00005b20: 2061 7265 3a0a 2020 2020 2020 2020 2020   are:.          
-00005b30: 2020 2d20 2f65 7463 2f73 6c75 726d 2d63    - /etc/slurm-c
-00005b40: 6f6e 6669 672e 696e 690a 2020 2020 2020  onfig.ini.      
-00005b50: 2020 2020 2020 2d20 7e2f 736c 7572 6d2d        - ~/slurm-
-00005b60: 636f 6e66 6967 2e69 6e69 0a0a 2020 2020  config.ini..    
-00005b70: 2020 2020 4e6f 7465 2074 6861 7420 7468      Note that th
-00005b80: 6973 2069 7320 6f6e 6c79 2066 6f72 2074  is is only for t
-00005b90: 6865 2053 4c55 524d 2073 7065 6369 6669  he SLURM specifi
-00005ba0: 6320 7661 6c75 6573 2074 6861 7420 7765  c values that we
-00005bb0: 2061 6464 6564 2e0a 2020 2020 2020 2020   added..        
-00005bc0: 4d6f 7374 2063 6f6e 6669 6775 7261 7469  Most configurati
-00005bd0: 6f6e 2076 616c 7565 7320 6172 6520 7365  on values are se
-00005be0: 7420 7669 6120 636f 6e66 6967 7572 6174  t via configurat
-00005bf0: 696f 6e20 6d65 6368 616e 6973 6d73 2066  ion mechanisms f
-00005c00: 726f 6d0a 2020 2020 2020 2020 4661 6272  rom.        Fabr
-00005c10: 6963 206c 6962 7261 7279 2c0a 2020 2020  ic library,.    
-00005c20: 2020 2020 6c69 6b65 2053 5348 2073 6574      like SSH set
-00005c30: 7469 6e67 7320 6265 696e 6720 6c6f 6164  tings being load
-00005c40: 6564 2066 726f 6d20 5353 4820 636f 6e66  ed from SSH conf
-00005c50: 6967 2c20 2f65 7463 2f66 6162 7269 632e  ig, /etc/fabric.
-00005c60: 796d 6c20 6f72 0a20 2020 2020 2020 2065  yml or.        e
-00005c70: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00005c80: 626c 6573 2e0a 2020 2020 2020 2020 5365  bles..        Se
-00005c90: 6520 4661 6272 6963 2773 2064 6f63 756d  e Fabric's docum
-00005ca0: 656e 7461 7469 6f6e 2066 6f72 206d 6f72  entation for mor
-00005cb0: 6520 696e 666f 206f 6e20 636f 6e66 6967  e info on config
-00005cc0: 7572 6174 696f 6e20 6966 206e 6565 6465  uration if neede
-00005cd0: 642e 0a0a 2020 2020 2020 2020 4172 6773  d...        Args
-00005ce0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00005cf0: 6e66 6967 6669 6c65 2028 7374 7229 3a20  nfigfile (str): 
-00005d00: 5468 6520 7061 7468 2074 6f20 796f 7572  The path to your
-00005d10: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-00005d20: 696c 652e 204f 7074 696f 6e61 6c2e 0a20  ile. Optional.. 
-00005d30: 2020 2020 2020 2020 2020 2069 6e69 745f             init_
-00005d40: 736c 7572 6d20 2862 6f6f 6c29 3a20 496e  slurm (bool): In
-00005d50: 6974 6961 7465 202f 2076 616c 6964 6174  itiate / validat
-00005d60: 6520 736c 7572 6d20 7365 7475 702e 204f  e slurm setup. O
-00005d70: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-00005d80: 2020 2020 2020 2020 4d69 6768 7420 7461          Might ta
-00005d90: 6b65 2073 6f6d 6520 7469 6d65 2074 6865  ke some time the
-00005da0: 2066 6972 7374 2074 696d 6520 7769 7468   first time with
-00005db0: 2064 6f77 6e6c 6f61 6469 6e67 2065 7463   downloading etc
-00005dc0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00005dd0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00005de0: 536c 7572 6d43 6c69 656e 743a 2041 206e  SlurmClient: A n
-00005df0: 6577 2053 6c75 726d 436c 6965 6e74 206f  ew SlurmClient o
-00005e00: 626a 6563 742e 0a20 2020 2020 2020 2022  bject..        "
-00005e10: 2222 0a20 2020 2020 2020 2023 204c 6f61  "".        # Loa
-00005e20: 6420 7468 6520 636f 6e66 6967 7572 6174  d the configurat
-00005e30: 696f 6e20 6669 6c65 0a20 2020 2020 2020  ion file.       
-00005e40: 2063 6f6e 6669 6773 203d 2063 6f6e 6669   configs = confi
-00005e50: 6770 6172 7365 722e 436f 6e66 6967 5061  gparser.ConfigPa
-00005e60: 7273 6572 2861 6c6c 6f77 5f6e 6f5f 7661  rser(allow_no_va
-00005e70: 6c75 653d 5472 7565 290a 2020 2020 2020  lue=True).      
-00005e80: 2020 2320 4c6f 6164 7320 6672 6f6d 2064    # Loads from d
-00005e90: 6566 6175 6c74 206c 6f63 6174 696f 6e73  efault locations
-00005ea0: 2061 6e64 2067 6976 656e 206c 6f63 6174   and given locat
-00005eb0: 696f 6e2c 206d 6973 7369 6e67 2066 696c  ion, missing fil
-00005ec0: 6573 2061 7265 206f 6b0a 2020 2020 2020  es are ok.      
-00005ed0: 2020 636f 6e66 6967 732e 7265 6164 285b    configs.read([
-00005ee0: 636c 732e 5f44 4546 4155 4c54 5f43 4f4e  cls._DEFAULT_CON
-00005ef0: 4649 475f 5041 5448 5f31 2c0a 2020 2020  FIG_PATH_1,.    
-00005f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f10: 2063 6c73 2e5f 4445 4641 554c 545f 434f   cls._DEFAULT_CO
-00005f20: 4e46 4947 5f50 4154 485f 322c 0a20 2020  NFIG_PATH_2,.   
-00005f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005f40: 2020 636f 6e66 6967 6669 6c65 5d29 0a20    configfile]). 
-00005f50: 2020 2020 2020 2023 2052 6561 6420 7468         # Read th
-00005f60: 6520 7265 7175 6972 6564 2070 6172 616d  e required param
-00005f70: 6574 6572 7320 6672 6f6d 2074 6865 2063  eters from the c
-00005f80: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-00005f90: 652c 0a20 2020 2020 2020 2023 2066 616c  e,.        # fal
-00005fa0: 6c62 6163 6b20 746f 2064 6566 6175 6c74  lback to default
-00005fb0: 730a 2020 2020 2020 2020 686f 7374 203d  s.        host =
-00005fc0: 2063 6f6e 6669 6773 2e67 6574 2822 5353   configs.get("SS
-00005fd0: 4822 2c20 2268 6f73 7422 2c20 6661 6c6c  H", "host", fall
-00005fe0: 6261 636b 3d63 6c73 2e5f 4445 4641 554c  back=cls._DEFAUL
-00005ff0: 545f 484f 5354 290a 2020 2020 2020 2020  T_HOST).        
-00006000: 696e 6c69 6e65 5f73 7368 5f65 6e76 203d  inline_ssh_env =
-00006010: 2063 6f6e 6669 6773 2e67 6574 626f 6f6c   configs.getbool
-00006020: 6561 6e28 0a20 2020 2020 2020 2020 2020  ean(.           
-00006030: 2022 5353 4822 2c20 2269 6e6c 696e 655f   "SSH", "inline_
-00006040: 7373 685f 656e 7622 2c20 6661 6c6c 6261  ssh_env", fallba
-00006050: 636b 3d63 6c73 2e5f 4445 4641 554c 545f  ck=cls._DEFAULT_
-00006060: 494e 4c49 4e45 5f53 5348 5f45 4e56 290a  INLINE_SSH_ENV).
-00006070: 2020 2020 2020 2020 736c 7572 6d5f 6461          slurm_da
-00006080: 7461 5f70 6174 6820 3d20 636f 6e66 6967  ta_path = config
-00006090: 732e 6765 7428 0a20 2020 2020 2020 2020  s.get(.         
-000060a0: 2020 2022 534c 5552 4d22 2c20 2273 6c75     "SLURM", "slu
-000060b0: 726d 5f64 6174 615f 7061 7468 222c 2066  rm_data_path", f
-000060c0: 616c 6c62 6163 6b3d 636c 732e 5f44 4546  allback=cls._DEF
-000060d0: 4155 4c54 5f53 4c55 524d 5f44 4154 415f  AULT_SLURM_DATA_
-000060e0: 5041 5448 290a 2020 2020 2020 2020 736c  PATH).        sl
-000060f0: 7572 6d5f 696d 6167 6573 5f70 6174 6820  urm_images_path 
-00006100: 3d20 636f 6e66 6967 732e 6765 7428 0a20  = configs.get(. 
-00006110: 2020 2020 2020 2020 2020 2022 534c 5552             "SLUR
-00006120: 4d22 2c20 2273 6c75 726d 5f69 6d61 6765  M", "slurm_image
-00006130: 735f 7061 7468 222c 0a20 2020 2020 2020  s_path",.       
-00006140: 2020 2020 2066 616c 6c62 6163 6b3d 636c       fallback=cl
-00006150: 732e 5f44 4546 4155 4c54 5f53 4c55 524d  s._DEFAULT_SLURM
-00006160: 5f49 4d41 4745 535f 5041 5448 290a 2020  _IMAGES_PATH).  
-00006170: 2020 2020 2020 736c 7572 6d5f 636f 6e76        slurm_conv
-00006180: 6572 7465 7273 5f70 6174 6820 3d20 636f  erters_path = co
-00006190: 6e66 6967 732e 6765 7428 0a20 2020 2020  nfigs.get(.     
-000061a0: 2020 2020 2020 2022 534c 5552 4d22 2c20         "SLURM", 
-000061b0: 2273 6c75 726d 5f63 6f6e 7665 7274 6572  "slurm_converter
-000061c0: 735f 7061 7468 222c 0a20 2020 2020 2020  s_path",.       
-000061d0: 2020 2020 2066 616c 6c62 6163 6b3d 636c       fallback=cl
-000061e0: 732e 5f44 4546 4155 4c54 5f53 4c55 524d  s._DEFAULT_SLURM
-000061f0: 5f43 4f4e 5645 5254 4552 535f 5041 5448  _CONVERTERS_PATH
-00006200: 290a 0a20 2020 2020 2020 2023 2053 706c  )..        # Spl
-00006210: 6974 2074 6865 204d 4f44 454c 5320 696e  it the MODELS in
-00006220: 746f 2070 6174 6873 2c20 7265 706f 7320  to paths, repos 
-00006230: 616e 6420 696d 6167 6573 0a20 2020 2020  and images.     
-00006240: 2020 206d 6f64 656c 735f 6469 6374 203d     models_dict =
-00006250: 2064 6963 7428 636f 6e66 6967 732e 6974   dict(configs.it
-00006260: 656d 7328 224d 4f44 454c 5322 2929 0a20  ems("MODELS")). 
-00006270: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00006280: 656c 5f70 6174 6873 203d 207b 7d0a 2020  el_paths = {}.  
-00006290: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-000062a0: 6c5f 7265 706f 7320 3d20 7b7d 0a20 2020  l_repos = {}.   
-000062b0: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
-000062c0: 5f6a 6f62 7320 3d20 7b7d 0a20 2020 2020  _jobs = {}.     
-000062d0: 2020 2073 6c75 726d 5f6d 6f64 656c 5f6a     slurm_model_j
-000062e0: 6f62 735f 7061 7261 6d73 203d 207b 7d0a  obs_params = {}.
-000062f0: 2020 2020 2020 2020 666f 7220 6b2c 2076          for k, v
-00006300: 2069 6e20 6d6f 6465 6c73 5f64 6963 742e   in models_dict.
-00006310: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-00006320: 2020 2020 2073 7566 6669 785f 7265 706f       suffix_repo
-00006330: 203d 2027 5f72 6570 6f27 0a20 2020 2020   = '_repo'.     
-00006340: 2020 2020 2020 2073 7566 6669 785f 6a6f         suffix_jo
-00006350: 6220 3d20 275f 6a6f 6227 0a20 2020 2020  b = '_job'.     
-00006360: 2020 2020 2020 206a 6f62 5f70 6172 616d         job_param
-00006370: 5f70 6174 7465 726e 203d 2022 282e 2b29  _pattern = "(.+)
-00006380: 5f6a 6f62 5f28 2e2b 2922 0a20 2020 2020  _job_(.+)".     
-00006390: 2020 2020 2020 206a 6f62 5f70 6172 616d         job_param
-000063a0: 5f6d 6174 6368 203d 2072 652e 6d61 7463  _match = re.matc
-000063b0: 6828 6a6f 625f 7061 7261 6d5f 7061 7474  h(job_param_patt
-000063c0: 6572 6e2c 206b 290a 2020 2020 2020 2020  ern, k).        
-000063d0: 2020 2020 6966 206b 2e65 6e64 7377 6974      if k.endswit
-000063e0: 6828 7375 6666 6978 5f72 6570 6f29 3a0a  h(suffix_repo):.
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006400: 736c 7572 6d5f 6d6f 6465 6c5f 7265 706f  slurm_model_repo
-00006410: 735b 6b5b 3a2d 6c65 6e28 7375 6666 6978  s[k[:-len(suffix
-00006420: 5f72 6570 6f29 5d5d 203d 2076 0a20 2020  _repo)]] = v.   
-00006430: 2020 2020 2020 2020 2065 6c69 6620 6b2e           elif k.
-00006440: 656e 6473 7769 7468 2873 7566 6669 785f  endswith(suffix_
-00006450: 6a6f 6229 3a0a 2020 2020 2020 2020 2020  job):.          
-00006460: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-00006470: 6c5f 6a6f 6273 5b6b 5b3a 2d6c 656e 2873  l_jobs[k[:-len(s
-00006480: 7566 6669 785f 6a6f 6229 5d5d 203d 2076  uffix_job)]] = v
-00006490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000064a0: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
-000064b0: 735f 7061 7261 6d73 5b6b 5b3a 2d6c 656e  s_params[k[:-len
-000064c0: 2873 7566 6669 785f 6a6f 6229 5d5d 203d  (suffix_job)]] =
-000064d0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
-000064e0: 656c 6966 206a 6f62 5f70 6172 616d 5f6d  elif job_param_m
-000064f0: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
-00006500: 2020 2020 2020 7072 696e 7428 6622 4d61        print(f"Ma
-00006510: 7463 683a 207b 736c 7572 6d5f 6d6f 6465  tch: {slurm_mode
-00006520: 6c5f 6a6f 6273 5f70 6172 616d 737d 2229  l_jobs_params}")
-00006530: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006540: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
-00006550: 735f 7061 7261 6d73 5b6a 6f62 5f70 6172  s_params[job_par
-00006560: 616d 5f6d 6174 6368 2e67 726f 7570 2831  am_match.group(1
-00006570: 295d 2e61 7070 656e 6428 0a20 2020 2020  )].append(.     
-00006580: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00006590: 2220 2d2d 7b6a 6f62 5f70 6172 616d 5f6d  " --{job_param_m
-000065a0: 6174 6368 2e67 726f 7570 2832 297d 3d7b  atch.group(2)}={
-000065b0: 767d 2229 0a20 2020 2020 2020 2020 2020  v}").           
-000065c0: 2020 2020 2070 7269 6e74 2866 2241 6464       print(f"Add
-000065d0: 6564 3a20 7b73 6c75 726d 5f6d 6f64 656c  ed: {slurm_model
-000065e0: 5f6a 6f62 735f 7061 7261 6d73 7d22 290a  _jobs_params}").
-000065f0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00006600: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00006610: 2020 736c 7572 6d5f 6d6f 6465 6c5f 7061    slurm_model_pa
-00006620: 7468 735b 6b5d 203d 2076 0a0a 2020 2020  ths[k] = v..    
-00006630: 2020 2020 736c 7572 6d5f 7363 7269 7074      slurm_script
-00006640: 5f70 6174 6820 3d20 636f 6e66 6967 732e  _path = configs.
-00006650: 6765 7428 0a20 2020 2020 2020 2020 2020  get(.           
-00006660: 2022 534c 5552 4d22 2c20 2273 6c75 726d   "SLURM", "slurm
-00006670: 5f73 6372 6970 745f 7061 7468 222c 0a20  _script_path",. 
-00006680: 2020 2020 2020 2020 2020 2066 616c 6c62             fallb
-00006690: 6163 6b3d 636c 732e 5f44 4546 4155 4c54  ack=cls._DEFAULT
-000066a0: 5f53 4c55 524d 5f47 4954 5f53 4352 4950  _SLURM_GIT_SCRIP
-000066b0: 545f 5041 5448 290a 2020 2020 2020 2020  T_PATH).        
-000066c0: 736c 7572 6d5f 7363 7269 7074 5f72 6570  slurm_script_rep
-000066d0: 6f20 3d20 636f 6e66 6967 732e 6765 7428  o = configs.get(
-000066e0: 0a20 2020 2020 2020 2020 2020 2022 534c  .            "SL
-000066f0: 5552 4d22 2c20 2273 6c75 726d 5f73 6372  URM", "slurm_scr
-00006700: 6970 745f 7265 706f 222c 0a20 2020 2020  ipt_repo",.     
-00006710: 2020 2020 2020 2066 616c 6c62 6163 6b3d         fallback=
-00006720: 4e6f 6e65 0a20 2020 2020 2020 2029 0a20  None.        ). 
-00006730: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
-00006740: 7468 6520 536c 7572 6d43 6c69 656e 7420  the SlurmClient 
-00006750: 6f62 6a65 6374 2077 6974 6820 7468 6520  object with the 
-00006760: 7061 7261 6d65 7465 7273 2072 6561 6420  parameters read 
-00006770: 6672 6f6d 0a20 2020 2020 2020 2023 2074  from.        # t
-00006780: 6865 2063 6f6e 6669 6720 6669 6c65 0a20  he config file. 
-00006790: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-000067a0: 7328 686f 7374 3d68 6f73 742c 0a20 2020  s(host=host,.   
-000067b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067c0: 696e 6c69 6e65 5f73 7368 5f65 6e76 3d69  inline_ssh_env=i
-000067d0: 6e6c 696e 655f 7373 685f 656e 762c 0a20  nline_ssh_env,. 
-000067e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067f0: 2020 736c 7572 6d5f 6461 7461 5f70 6174    slurm_data_pat
-00006800: 683d 736c 7572 6d5f 6461 7461 5f70 6174  h=slurm_data_pat
-00006810: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
-00006820: 2020 2020 2020 736c 7572 6d5f 696d 6167        slurm_imag
-00006830: 6573 5f70 6174 683d 736c 7572 6d5f 696d  es_path=slurm_im
-00006840: 6167 6573 5f70 6174 682c 0a20 2020 2020  ages_path,.     
-00006850: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-00006860: 7572 6d5f 636f 6e76 6572 7465 7273 5f70  urm_converters_p
-00006870: 6174 683d 736c 7572 6d5f 636f 6e76 6572  ath=slurm_conver
-00006880: 7465 7273 5f70 6174 682c 0a20 2020 2020  ters_path,.     
-00006890: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-000068a0: 7572 6d5f 6d6f 6465 6c5f 7061 7468 733d  urm_model_paths=
-000068b0: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
-000068c0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-000068d0: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-000068e0: 6c5f 7265 706f 733d 736c 7572 6d5f 6d6f  l_repos=slurm_mo
-000068f0: 6465 6c5f 7265 706f 732c 0a20 2020 2020  del_repos,.     
-00006900: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-00006910: 7572 6d5f 6d6f 6465 6c5f 696d 6167 6573  urm_model_images
-00006920: 3d4e 6f6e 652c 0a20 2020 2020 2020 2020  =None,.         
-00006930: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
-00006940: 6d6f 6465 6c5f 6a6f 6273 3d73 6c75 726d  model_jobs=slurm
-00006950: 5f6d 6f64 656c 5f6a 6f62 732c 0a20 2020  _model_jobs,.   
-00006960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006970: 736c 7572 6d5f 6d6f 6465 6c5f 6a6f 6273  slurm_model_jobs
-00006980: 5f70 6172 616d 733d 736c 7572 6d5f 6d6f  _params=slurm_mo
-00006990: 6465 6c5f 6a6f 6273 5f70 6172 616d 732c  del_jobs_params,
-000069a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000069b0: 2020 2020 736c 7572 6d5f 7363 7269 7074      slurm_script
-000069c0: 5f70 6174 683d 736c 7572 6d5f 7363 7269  _path=slurm_scri
-000069d0: 7074 5f70 6174 682c 0a20 2020 2020 2020  pt_path,.       
-000069e0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-000069f0: 6d5f 7363 7269 7074 5f72 6570 6f3d 736c  m_script_repo=sl
-00006a00: 7572 6d5f 7363 7269 7074 5f72 6570 6f2c  urm_script_repo,
-00006a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006a20: 2020 2020 696e 6974 5f73 6c75 726d 3d69      init_slurm=i
-00006a30: 6e69 745f 736c 7572 6d29 0a0a 2020 2020  nit_slurm)..    
-00006a40: 6465 6620 636c 6561 6e75 705f 746d 705f  def cleanup_tmp_
-00006a50: 6669 6c65 7328 7365 6c66 2c0a 2020 2020  files(self,.    
-00006a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006a70: 2020 2020 2020 736c 7572 6d5f 6a6f 625f        slurm_job_
-00006a80: 6964 3a20 7374 722c 0a20 2020 2020 2020  id: str,.       
-00006a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006aa0: 2020 2066 696c 656e 616d 653a 2073 7472     filename: str
-00006ab0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-00006ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006ad0: 2020 2064 6174 615f 6c6f 6361 7469 6f6e     data_location
-00006ae0: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00006af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b00: 2020 2020 2020 2020 6c6f 6766 696c 653a          logfile:
-00006b10: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-00006b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006b30: 2020 2020 2020 2029 202d 3e20 5265 7375         ) -> Resu
-00006b40: 6c74 3a0a 2020 2020 2020 2020 2222 220a  lt:.        """.
-00006b50: 2020 2020 2020 2020 436c 6561 6e75 7020          Cleanup 
-00006b60: 7a69 7020 616e 6420 756e 7a69 7070 6564  zip and unzipped
-00006b70: 2066 696c 6573 2f66 6f6c 6465 7273 2061   files/folders a
-00006b80: 7373 6f63 6961 7465 6420 7769 7468 2061  ssociated with a
-00006b90: 2053 6c75 726d 206a 6f62 2e0a 0a20 2020   Slurm job...   
-00006ba0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00006bb0: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
-00006bc0: 5f69 6420 2873 7472 293a 2054 6865 206a  _id (str): The j
-00006bd0: 6f62 2049 4420 6f66 2074 6865 2053 6c75  ob ID of the Slu
-00006be0: 726d 2073 6372 6970 742e 0a20 2020 2020  rm script..     
-00006bf0: 2020 2020 2020 2066 696c 656e 616d 6520         filename 
-00006c00: 2873 7472 293a 2054 6865 207a 6970 2066  (str): The zip f
-00006c10: 696c 656e 616d 6520 6f6e 2053 6c75 726d  ilename on Slurm
-00006c20: 2e0a 2020 2020 2020 2020 2020 2020 6461  ..            da
-00006c30: 7461 5f6c 6f63 6174 696f 6e20 2873 7472  ta_location (str
-00006c40: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00006c50: 206c 6f63 6174 696f 6e20 6f66 2064 6174   location of dat
-00006c60: 6120 6669 6c65 7320 6f6e 2053 6c75 726d  a files on Slurm
-00006c70: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006c80: 2020 4966 206e 6f74 2070 726f 7669 6465    If not provide
-00006c90: 642c 2069 7420 7769 6c6c 2062 6520 6578  d, it will be ex
-00006ca0: 7472 6163 7465 6420 6672 6f6d 2074 6865  tracted from the
-00006cb0: 206c 6f67 2066 696c 652e 0a20 2020 2020   log file..     
-00006cc0: 2020 2020 2020 206c 6f67 6669 6c65 2028         logfile (
-00006cd0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-00006ce0: 5468 6520 6c6f 6720 6669 6c65 206f 6620  The log file of 
-00006cf0: 7468 6520 536c 7572 6d20 6a6f 622e 200a  the Slurm job. .
-00006d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006d10: 4966 206e 6f74 2070 726f 7669 6465 642c  If not provided,
-00006d20: 2061 2064 6566 6175 6c74 206c 6f67 2066   a default log f
-00006d30: 696c 6520 7769 6c6c 2062 6520 7573 6564  ile will be used
-00006d40: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00006d50: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00006d60: 5265 7375 6c74 3a20 5468 6520 7265 7375  Result: The resu
-00006d70: 6c74 206f 6620 7468 6520 636c 6561 6e75  lt of the cleanu
-00006d80: 7020 6f70 6572 6174 696f 6e2e 0a0a 2020  p operation...  
-00006d90: 2020 2020 2020 4e6f 7465 3a0a 2020 2020        Note:.    
-00006da0: 2020 2020 2020 2020 5468 6520 636c 6561          The clea
-00006db0: 6e75 7020 7072 6f63 6573 7320 696e 766f  nup process invo
-00006dc0: 6c76 6573 2072 656d 6f76 696e 6720 7468  lves removing th
-00006dd0: 6520 7370 6563 6966 6965 6420 7a69 7020  e specified zip 
-00006de0: 6669 6c65 2c20 0a20 2020 2020 2020 2020  file, .         
-00006df0: 2020 2074 6865 206c 6f67 2066 696c 652c     the log file,
-00006e00: 2061 6e64 2061 7373 6f63 6961 7465 6420   and associated 
-00006e10: 6461 7461 2066 696c 6573 2061 6e64 2066  data files and f
-00006e20: 6f6c 6465 7273 2e0a 0a20 2020 2020 2020  olders...       
-00006e30: 2045 7861 6d70 6c65 3a0a 2020 2020 2020   Example:.      
-00006e40: 2020 2020 2020 2320 436c 6561 6e75 7020        # Cleanup 
-00006e50: 7465 6d70 6f72 6172 7920 6669 6c65 7320  temporary files 
-00006e60: 666f 7220 6120 536c 7572 6d20 6a6f 620a  for a Slurm job.
-00006e70: 2020 2020 2020 2020 2020 2020 636c 6965              clie
-00006e80: 6e74 2e63 6c65 616e 7570 5f74 6d70 5f66  nt.cleanup_tmp_f
-00006e90: 696c 6573 2822 3132 3334 3522 2c20 226f  iles("12345", "o
-00006ea0: 7574 7075 742e 7a69 7022 290a 2020 2020  utput.zip").    
-00006eb0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00006ec0: 636d 6473 203d 205b 5d0a 2020 2020 2020  cmds = [].      
-00006ed0: 2020 2320 7a69 700a 2020 2020 2020 2020    # zip.        
-00006ee0: 6966 2066 696c 656e 616d 653a 0a20 2020  if filename:.   
-00006ef0: 2020 2020 2020 2020 2072 6d7a 6970 203d           rmzip =
-00006f00: 2066 2272 6d20 7b66 696c 656e 616d 657d   f"rm {filename}
-00006f10: 2e2a 220a 2020 2020 2020 2020 2020 2020  .*".            
-00006f20: 636d 6473 2e61 7070 656e 6428 726d 7a69  cmds.append(rmzi
-00006f30: 7029 0a20 2020 2020 2020 2023 206c 6f67  p).        # log
-00006f40: 0a20 2020 2020 2020 2069 6620 6c6f 6766  .        if logf
-00006f50: 696c 6520 6973 204e 6f6e 653a 0a20 2020  ile is None:.   
-00006f60: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
-00006f70: 203d 2073 656c 662e 5f4c 4f47 4649 4c45   = self._LOGFILE
-00006f80: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00006f90: 6669 6c65 203d 206c 6f67 6669 6c65 2e66  file = logfile.f
-00006fa0: 6f72 6d61 7428 736c 7572 6d5f 6a6f 625f  ormat(slurm_job_
-00006fb0: 6964 3d73 6c75 726d 5f6a 6f62 5f69 6429  id=slurm_job_id)
-00006fc0: 0a20 2020 2020 2020 2072 6d6c 6f67 203d  .        rmlog =
-00006fd0: 2066 2272 6d20 7b6c 6f67 6669 6c65 7d22   f"rm {logfile}"
-00006fe0: 0a20 2020 2020 2020 2063 6d64 732e 6170  .        cmds.ap
-00006ff0: 7065 6e64 2872 6d6c 6f67 290a 2020 2020  pend(rmlog).    
-00007000: 2020 2020 2320 636f 6e76 6572 7465 7220      # converter 
-00007010: 6c6f 6773 0a20 2020 2020 2020 2063 6c6f  logs.        clo
-00007020: 6720 3d20 7365 6c66 2e5f 434f 4e56 4552  g = self._CONVER
-00007030: 5445 525f 4c4f 4746 494c 450a 2020 2020  TER_LOGFILE.    
-00007040: 2020 2020 636c 6f67 203d 2063 6c6f 672e      clog = clog.
-00007050: 666f 726d 6174 2873 6c75 726d 5f6a 6f62  format(slurm_job
-00007060: 5f69 643d 736c 7572 6d5f 6a6f 625f 6964  _id=slurm_job_id
-00007070: 290a 2020 2020 2020 2020 726d 636c 6f67  ).        rmclog
-00007080: 203d 2066 2272 6d20 7b63 6c6f 677d 220a   = f"rm {clog}".
-00007090: 2020 2020 2020 2020 636d 6473 2e61 7070          cmds.app
-000070a0: 656e 6428 726d 636c 6f67 290a 2020 2020  end(rmclog).    
-000070b0: 2020 2020 0a20 2020 2020 2020 2023 2064      .        # d
-000070c0: 6174 610a 2020 2020 2020 2020 6966 2064  ata.        if d
-000070d0: 6174 615f 6c6f 6361 7469 6f6e 2069 7320  ata_location is 
-000070e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-000070f0: 2020 6461 7461 5f6c 6f63 6174 696f 6e20    data_location 
-00007100: 3d20 7365 6c66 2e65 7874 7261 6374 5f64  = self.extract_d
-00007110: 6174 615f 6c6f 6361 7469 6f6e 5f66 726f  ata_location_fro
-00007120: 6d5f 6c6f 6728 6c6f 6766 696c 6529 0a20  m_log(logfile). 
-00007130: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00007140: 2020 2020 6966 2064 6174 615f 6c6f 6361      if data_loca
-00007150: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
-00007160: 2020 726d 6461 7461 203d 2066 2272 6d20    rmdata = f"rm 
-00007170: 2d72 6620 7b64 6174 615f 6c6f 6361 7469  -rf {data_locati
-00007180: 6f6e 7d20 7b64 6174 615f 6c6f 6361 7469  on} {data_locati
-00007190: 6f6e 7d2e 2a22 0a20 2020 2020 2020 2020  on}.*".         
-000071a0: 2020 2063 6d64 732e 6170 7065 6e64 2872     cmds.append(r
-000071b0: 6d64 6174 6129 0a20 2020 2020 2020 2020  mdata).         
-000071c0: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-000071d0: 2320 636f 6e76 6572 7420 636f 6e66 6967  # convert config
-000071e0: 2066 696c 650a 2020 2020 2020 2020 2020   file.          
-000071f0: 2020 636f 6e66 6967 5f66 696c 6520 3d20    config_file = 
-00007200: 6622 636f 6e66 6967 5f7b 6f73 2e70 6174  f"config_{os.pat
-00007210: 682e 6261 7365 6e61 6d65 2864 6174 615f  h.basename(data_
-00007220: 6c6f 6361 7469 6f6e 297d 2e74 7874 220a  location)}.txt".
-00007230: 2020 2020 2020 2020 2020 2020 726d 636f              rmco
-00007240: 6e66 6967 203d 2066 2272 6d20 7b63 6f6e  nfig = f"rm {con
-00007250: 6669 675f 6669 6c65 7d22 0a20 2020 2020  fig_file}".     
-00007260: 2020 2020 2020 2063 6d64 732e 6170 7065         cmds.appe
-00007270: 6e64 2872 6d63 6f6e 6669 6729 0a20 2020  nd(rmconfig).   
-00007280: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00007290: 2020 2020 2020 206c 6f67 6765 722e 7761         logger.wa
-000072a0: 726e 696e 6728 6622 436f 756c 6420 6e6f  rning(f"Could no
-000072b0: 7420 6578 7472 6163 7420 6461 7461 206c  t extract data l
-000072c0: 6f63 6174 696f 6e20 6672 6f6d 206c 6f67  ocation from log
-000072d0: 207b 6c6f 6766 696c 657d 2e20 536b 6970   {logfile}. Skip
-000072e0: 7069 6e67 2063 6c65 616e 7570 2e22 290a  ping cleanup.").
-000072f0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00007300: 2020 2020 2020 2020 2020 2320 646f 2061            # do a
-00007310: 7320 6d75 6368 2061 7320 706f 7373 6962  s much as possib
-00007320: 6c65 2c20 6e6f 7420 636f 6e64 6974 696f  le, not conditio
-00007330: 6e61 6c20 7265 6d6f 7661 6c0a 2020 2020  nal removal.    
-00007340: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00007350: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
-00007360: 6473 2863 6d64 732c 2073 6570 3d27 203b  ds(cmds, sep=' ;
-00007370: 2027 290a 2020 2020 2020 2020 6578 6365   ').        exce
-00007380: 7074 2055 6e65 7870 6563 7465 6445 7869  pt UnexpectedExi
-00007390: 7420 6173 2065 3a0a 2020 2020 2020 2020  t as e:.        
-000073a0: 2020 2020 6c6f 6767 6572 2e77 6172 6e69      logger.warni
-000073b0: 6e67 2865 290a 2020 2020 2020 2020 2020  ng(e).          
-000073c0: 2020 7265 7375 6c74 203d 2065 2e72 6573    result = e.res
-000073d0: 756c 740a 2020 2020 2020 2020 7265 7475  ult.        retu
-000073e0: 726e 2072 6573 756c 7420 6f72 204e 6f6e  rn result or Non
-000073f0: 650a 0a20 2020 2064 6566 2076 616c 6964  e..    def valid
-00007400: 6174 6528 7365 6c66 2c20 7661 6c69 6461  ate(self, valida
-00007410: 7465 5f73 6c75 726d 5f73 6574 7570 3a20  te_slurm_setup: 
-00007420: 626f 6f6c 203d 2046 616c 7365 293a 0a20  bool = False):. 
-00007430: 2020 2020 2020 2022 2222 5661 6c69 6461         """Valida
-00007440: 7465 2074 6865 2063 6f6e 6e65 6374 696f  te the connectio
-00007450: 6e20 746f 2074 6865 2053 6c75 726d 2063  n to the Slurm c
-00007460: 6c75 7374 6572 2062 7920 7275 6e6e 696e  luster by runnin
-00007470: 670a 2020 2020 2020 2020 6120 7369 6d70  g.        a simp
-00007480: 6c65 2063 6f6d 6d61 6e64 2e0a 0a20 2020  le command...   
-00007490: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-000074a0: 2020 2020 2020 2076 616c 6964 6174 655f         validate_
-000074b0: 736c 7572 6d5f 7365 7475 7020 2862 6f6f  slurm_setup (boo
-000074c0: 6c29 3a20 5768 6574 6865 7220 746f 2061  l): Whether to a
-000074d0: 6c73 6f20 6368 6563 6b0a 2020 2020 2020  lso check.      
-000074e0: 2020 2020 2020 2020 2020 616e 6420 6669            and fi
-000074f0: 7820 7468 6520 536c 7572 6d20 7365 7475  x the Slurm setu
-00007500: 7020 2866 6f6c 6465 7273 2c20 696d 6167  p (folders, imag
-00007510: 6573 2c20 6574 632e 290a 0a20 2020 2020  es, etc.)..     
-00007520: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00007530: 2020 2020 2020 2020 626f 6f6c 3a0a 2020          bool:.  
-00007540: 2020 2020 2020 2020 2020 2020 2020 5472                Tr
-00007550: 7565 2069 6620 7468 6520 7661 6c69 6461  ue if the valida
-00007560: 7469 6f6e 2069 7320 7375 6363 6573 7366  tion is successf
-00007570: 756c 2c0a 2020 2020 2020 2020 2020 2020  ul,.            
-00007580: 2020 2020 4661 6c73 6520 6f74 6865 7277      False otherw
-00007590: 6973 652e 0a20 2020 2020 2020 2022 2222  ise..        """
-000075a0: 0a20 2020 2020 2020 2063 6f6e 6e65 6374  .        connect
-000075b0: 6564 203d 2073 656c 662e 7275 6e28 2765  ed = self.run('e
-000075c0: 6368 6f20 2220 2227 292e 6f6b 0a20 2020  cho " "').ok.   
-000075d0: 2020 2020 2069 6620 636f 6e6e 6563 7465       if connecte
-000075e0: 6420 616e 6420 7661 6c69 6461 7465 5f73  d and validate_s
-000075f0: 6c75 726d 5f73 6574 7570 3a0a 2020 2020  lurm_setup:.    
-00007600: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-00007610: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00007620: 662e 7365 7475 705f 736c 7572 6d28 290a  f.setup_slurm().
-00007630: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00007640: 7074 2053 5348 4578 6365 7074 696f 6e20  pt SSHException 
-00007650: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00007660: 2020 2020 2020 6c6f 6767 6572 2e65 7272        logger.err
-00007670: 6f72 2865 290a 2020 2020 2020 2020 2020  or(e).          
-00007680: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00007690: 7365 0a20 2020 2020 2020 2072 6574 7572  se.        retur
-000076a0: 6e20 636f 6e6e 6563 7465 640a 0a20 2020  n connected..   
-000076b0: 2064 6566 2067 6574 5f72 6563 656e 745f   def get_recent_
-000076c0: 6c6f 675f 636f 6d6d 616e 6428 7365 6c66  log_command(self
-000076d0: 2c20 6c6f 675f 6669 6c65 3a20 7374 722c  , log_file: str,
-000076e0: 206e 3a20 696e 7420 3d20 3130 2920 2d3e   n: int = 10) ->
-000076f0: 2073 7472 3a0a 2020 2020 2020 2020 2222   str:.        ""
-00007700: 220a 2020 2020 2020 2020 4765 7420 7468  ".        Get th
-00007710: 6520 636f 6d6d 616e 6420 746f 2072 6574  e command to ret
-00007720: 7269 6576 6520 7468 6520 7265 6365 6e74  rieve the recent
-00007730: 206c 6f67 2065 6e74 7269 6573 2066 726f   log entries fro
-00007740: 6d20 610a 2020 2020 2020 2020 7370 6563  m a.        spec
-00007750: 6966 6965 6420 6c6f 6720 6669 6c65 2e0a  ified log file..
-00007760: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00007770: 2020 2020 2020 2020 2020 206c 6f67 5f66             log_f
-00007780: 696c 6520 2873 7472 293a 2054 6865 2070  ile (str): The p
-00007790: 6174 6820 746f 2074 6865 206c 6f67 2066  ath to the log f
-000077a0: 696c 652e 0a20 2020 2020 2020 2020 2020  ile..           
-000077b0: 206e 2028 696e 742c 206f 7074 696f 6e61   n (int, optiona
-000077c0: 6c29 3a20 5468 6520 6e75 6d62 6572 206f  l): The number o
-000077d0: 6620 7265 6365 6e74 206c 6f67 2065 6e74  f recent log ent
-000077e0: 7269 6573 2074 6f20 7265 7472 6965 7665  ries to retrieve
-000077f0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007800: 2020 4465 6661 756c 7473 2074 6f20 3130    Defaults to 10
-00007810: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00007820: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00007830: 7374 723a 2054 6865 2063 6f6d 6d61 6e64  str: The command
-00007840: 2074 6f20 7265 7472 6965 7665 2074 6865   to retrieve the
-00007850: 2072 6563 656e 7420 6c6f 6720 656e 7472   recent log entr
-00007860: 6965 732e 0a20 2020 2020 2020 2022 2222  ies..        """
-00007870: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00007880: 7365 6c66 2e5f 5441 494c 5f4c 4f47 5f43  self._TAIL_LOG_C
-00007890: 4d44 2e66 6f72 6d61 7428 6e3d 6e2c 206c  MD.format(n=n, l
-000078a0: 6f67 5f66 696c 653d 6c6f 675f 6669 6c65  og_file=log_file
-000078b0: 290a 0a20 2020 2064 6566 2067 6574 5f61  )..    def get_a
-000078c0: 6374 6976 655f 6a6f 625f 7072 6f67 7265  ctive_job_progre
-000078d0: 7373 2873 656c 662c 0a20 2020 2020 2020  ss(self,.       
-000078e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000078f0: 2020 2020 2020 2020 2073 6c75 726d 5f6a           slurm_j
-00007900: 6f62 5f69 643a 2073 7472 2c0a 2020 2020  ob_id: str,.    
-00007910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007920: 2020 2020 2020 2020 2020 2020 7061 7474              patt
-00007930: 6572 6e3a 2073 7472 203d 2072 225c 642b  ern: str = r"\d+
-00007940: 2522 2c0a 2020 2020 2020 2020 2020 2020  %",.            
-00007950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007960: 2020 2020 656e 763a 204f 7074 696f 6e61      env: Optiona
-00007970: 6c5b 4469 6374 5b73 7472 2c20 7374 725d  l[Dict[str, str]
-00007980: 5d20 3d20 4e6f 6e65 2920 2d3e 2073 7472  ] = None) -> str
-00007990: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-000079a0: 2020 2020 2020 4765 7420 7468 6520 7072        Get the pr
-000079b0: 6f67 7265 7373 206f 6620 616e 2061 6374  ogress of an act
-000079c0: 6976 6520 536c 7572 6d20 6a6f 6220 6672  ive Slurm job fr
-000079d0: 6f6d 2069 7473 206c 6f67 6669 6c65 732e  om its logfiles.
-000079e0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000079f0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
-00007a00: 6d5f 6a6f 625f 6964 2028 7374 7229 3a20  m_job_id (str): 
-00007a10: 5468 6520 4944 206f 6620 7468 6520 536c  The ID of the Sl
-00007a20: 7572 6d20 6a6f 622e 0a20 2020 2020 2020  urm job..       
-00007a30: 2020 2020 2070 6174 7465 726e 2028 7374       pattern (st
-00007a40: 7229 3a20 5468 6520 7061 7474 6572 6e20  r): The pattern 
-00007a50: 746f 206d 6174 6368 2069 6e20 7468 6520  to match in the 
-00007a60: 6a6f 6220 6c6f 6720 746f 2065 7874 7261  job log to extra
-00007a70: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
-00007a80: 2020 2074 6865 2070 726f 6772 6573 7320     the progress 
-00007a90: 2864 6566 6175 6c74 3a20 7222 5c64 2b25  (default: r"\d+%
-00007aa0: 2229 2e0a 0a20 2020 2020 2020 2020 2020  ")...           
-00007ab0: 2065 6e76 2028 4469 6374 5b73 7472 2c20   env (Dict[str, 
-00007ac0: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
-00007ad0: 204f 7074 696f 6e61 6c20 656e 7669 726f   Optional enviro
-00007ae0: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
-00007af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007b00: 2074 6f20 7365 7420 7768 656e 2072 756e   to set when run
-00007b10: 6e69 6e67 2074 6865 2063 6f6d 6d61 6e64  ning the command
-00007b20: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-00007b30: 6e65 2e0a 0a20 2020 2020 2020 2052 6574  ne...        Ret
-00007b40: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00007b50: 2020 7374 723a 2054 6865 2070 726f 6772    str: The progr
-00007b60: 6573 7320 6f66 2074 6865 2053 6c75 726d  ess of the Slurm
-00007b70: 206a 6f62 2e0a 2020 2020 2020 2020 2222   job..        ""
-00007b80: 220a 2020 2020 2020 2020 636d 646c 6973  ".        cmdlis
-00007b90: 7420 3d20 5b5d 0a20 2020 2020 2020 2063  t = [].        c
-00007ba0: 6d64 203d 2073 656c 662e 6765 745f 7265  md = self.get_re
-00007bb0: 6365 6e74 5f6c 6f67 5f63 6f6d 6d61 6e64  cent_log_command
-00007bc0: 280a 2020 2020 2020 2020 2020 2020 6c6f  (.            lo
-00007bd0: 675f 6669 6c65 3d73 656c 662e 5f4c 4f47  g_file=self._LOG
-00007be0: 4649 4c45 2e66 6f72 6d61 7428 736c 7572  FILE.format(slur
-00007bf0: 6d5f 6a6f 625f 6964 3d73 6c75 726d 5f6a  m_job_id=slurm_j
-00007c00: 6f62 5f69 6429 290a 2020 2020 2020 2020  ob_id)).        
-00007c10: 636d 646c 6973 742e 6170 7065 6e64 2863  cmdlist.append(c
-00007c20: 6d64 290a 2020 2020 2020 2020 6966 2065  md).        if e
-00007c30: 6e76 2069 7320 4e6f 6e65 3a0a 2020 2020  nv is None:.    
-00007c40: 2020 2020 2020 2020 656e 7620 3d20 7b7d          env = {}
-00007c50: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00007c60: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00007c70: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
-00007c80: 616e 6473 2863 6d64 6c69 7374 2c20 656e  ands(cmdlist, en
-00007c90: 763d 656e 7629 0a20 2020 2020 2020 2065  v=env).        e
-00007ca0: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00007cb0: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00007cc0: 2020 6c6f 6767 6572 2e65 7272 6f72 2866    logger.error(f
-00007cd0: 2249 7373 7565 2077 6974 6820 7275 6e20  "Issue with run 
-00007ce0: 636f 6d6d 616e 643a 207b 657d 2229 0a20  command: {e}"). 
-00007cf0: 2020 2020 2020 2023 204d 6174 6368 2074         # Match t
-00007d00: 6865 2073 7065 6369 6669 6564 2070 6174  he specified pat
-00007d10: 7465 726e 2069 6e20 7468 6520 7265 7375  tern in the resu
-00007d20: 6c74 2773 2073 7464 6f75 740a 2020 2020  lt's stdout.    
-00007d30: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00007d40: 2020 2020 206c 6174 6573 745f 7072 6f67       latest_prog
-00007d50: 7265 7373 203d 2072 652e 6669 6e64 616c  ress = re.findal
-00007d60: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
-00007d70: 2020 2070 6174 7465 726e 2c20 7265 7375     pattern, resu
-00007d80: 6c74 2e73 7464 6f75 7429 5b2d 315d 0a20  lt.stdout)[-1]. 
-00007d90: 2020 2020 2020 2065 7863 6570 7420 4578         except Ex
-00007da0: 6365 7074 696f 6e20 6173 2065 3a0a 2020  ception as e:.  
-00007db0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-00007dc0: 2e65 7272 6f72 2866 2249 7373 7565 2077  .error(f"Issue w
-00007dd0: 6974 6820 6578 7472 6163 7469 6e67 2070  ith extracting p
-00007de0: 726f 6772 6573 733a 207b 657d 2229 0a0a  rogress: {e}")..
-00007df0: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-00007e00: 2250 726f 6772 6573 733a 207b 6c61 7465  "Progress: {late
-00007e10: 7374 5f70 726f 6772 6573 737d 5c6e 220a  st_progress}\n".
-00007e20: 0a20 2020 2064 6566 2072 756e 5f63 6f6d  .    def run_com
-00007e30: 6d61 6e64 7328 7365 6c66 2c20 636d 646c  mands(self, cmdl
-00007e40: 6973 743a 204c 6973 745b 7374 725d 2c0a  ist: List[str],.
-00007e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007e60: 2020 2020 2065 6e76 3a20 4f70 7469 6f6e       env: Option
-00007e70: 616c 5b44 6963 745b 7374 722c 2073 7472  al[Dict[str, str
-00007e80: 5d5d 203d 204e 6f6e 652c 0a20 2020 2020  ]] = None,.     
-00007e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ea0: 7365 703a 2073 7472 203d 2027 2026 2620  sep: str = ' && 
-00007eb0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-00007ec0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-00007ed0: 2920 2d3e 2052 6573 756c 743a 0a20 2020  ) -> Result:.   
-00007ee0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00007ef0: 2052 756e 2061 206c 6973 7420 6f66 2073   Run a list of s
-00007f00: 6865 6c6c 2063 6f6d 6d61 6e64 7320 636f  hell commands co
-00007f10: 6e73 6563 7574 6976 656c 7920 6f6e 2074  nsecutively on t
-00007f20: 6865 2053 6c75 726d 2063 6c75 7374 6572  he Slurm cluster
-00007f30: 2c0a 2020 2020 2020 2020 656e 7375 7269  ,.        ensuri
-00007f40: 6e67 2074 6865 2073 7563 6365 7373 206f  ng the success o
-00007f50: 6620 6561 6368 2062 6566 6f72 6520 7072  f each before pr
-00007f60: 6f63 6565 6469 6e67 2074 6f20 7468 6520  oceeding to the 
-00007f70: 6e65 7874 2e0a 0a20 2020 2020 2020 2054  next...        T
-00007f80: 6865 2065 6e76 6972 6f6e 6d65 6e74 2076  he environment v
-00007f90: 6172 6961 626c 6573 2063 616e 2062 6520  ariables can be 
-00007fa0: 7365 7420 7573 696e 6720 7468 6520 6065  set using the `e
-00007fb0: 6e76 6020 6172 6775 6d65 6e74 2e0a 2020  nv` argument..  
-00007fc0: 2020 2020 2020 5468 6573 6520 636f 6d6d        These comm
-00007fd0: 616e 6473 2072 6574 6169 6e20 7468 6520  ands retain the 
-00007fe0: 7361 6d65 2073 6573 7369 6f6e 2028 656e  same session (en
-00007ff0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00008000: 6c65 730a 2020 2020 2020 2020 6574 632e  les.        etc.
-00008010: 292c 2075 6e6c 696b 6520 7275 6e6e 696e  ), unlike runnin
-00008020: 6720 7468 656d 2073 6570 6172 6174 656c  g them separatel
-00008030: 792e 0a0a 2020 2020 2020 2020 4172 6773  y...        Args
-00008040: 3a0a 2020 2020 2020 2020 2020 2020 636d  :.            cm
-00008050: 646c 6973 7420 284c 6973 745b 7374 725d  dlist (List[str]
-00008060: 293a 2041 206c 6973 7420 6f66 2073 6865  ): A list of she
-00008070: 6c6c 2063 6f6d 6d61 6e64 7320 746f 2072  ll commands to r
-00008080: 756e 206f 6e20 536c 7572 6d2e 0a20 2020  un on Slurm..   
-00008090: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
-000080a0: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
-000080b0: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
-000080c0: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
-000080d0: 7269 6162 6c65 7320 746f 0a20 2020 2020  riables to.     
-000080e0: 2020 2020 2020 2020 2020 2073 6574 2077             set w
-000080f0: 6865 6e20 7275 6e6e 696e 6720 7468 6520  hen running the 
-00008100: 636f 6d6d 616e 642e 2044 6566 6175 6c74  command. Default
-00008110: 7320 746f 204e 6f6e 652e 0a20 2020 2020  s to None..     
-00008120: 2020 2020 2020 2073 6570 2028 7374 722c         sep (str,
-00008130: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
-00008140: 7365 7061 7261 746f 7220 7573 6564 2074  separator used t
-00008150: 6f20 636f 6e63 6174 656e 6174 6520 7468  o concatenate th
-00008160: 6520 0a20 2020 2020 2020 2020 2020 2020  e .             
-00008170: 2020 2063 6f6d 6d61 6e64 732e 2044 6566     commands. Def
-00008180: 6175 6c74 7320 746f 2027 2026 2620 272e  aults to ' && '.
-00008190: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
-000081a0: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
-000081b0: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
-000081c0: 6e74 732e 0a0a 2020 2020 2020 2020 5265  nts...        Re
-000081d0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-000081e0: 2020 2052 6573 756c 743a 2054 6865 2072     Result: The r
-000081f0: 6573 756c 7420 6f66 2074 6865 206c 6173  esult of the las
-00008200: 7420 636f 6d6d 616e 6420 696e 2074 6865  t command in the
-00008210: 206c 6973 742e 0a20 2020 2020 2020 2022   list..        "
-00008220: 2222 0a20 2020 2020 2020 2069 6620 656e  "".        if en
-00008230: 7620 6973 204e 6f6e 653a 0a20 2020 2020  v is None:.     
-00008240: 2020 2020 2020 2065 6e76 203d 207b 7d0a         env = {}.
-00008250: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
-00008260: 702e 6a6f 696e 2863 6d64 6c69 7374 290a  p.join(cmdlist).
-00008270: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00008280: 6e66 6f28 0a20 2020 2020 2020 2020 2020  nfo(.           
-00008290: 2066 2252 756e 6e69 6e67 2063 6f6d 6d61   f"Running comma
-000082a0: 6e64 732c 2077 6974 6820 656e 7620 7b65  nds, with env {e
-000082b0: 6e76 7d20 616e 6420 7365 7020 7b73 6570  nv} and sep {sep
-000082c0: 7d20 5c0a 2020 2020 2020 2020 2020 2020  } \.            
-000082d0: 2020 2020 616e 6420 7b6b 7761 7267 737d      and {kwargs}
-000082e0: 3a20 7b63 6d64 7d22 290a 2020 2020 2020  : {cmd}").      
-000082f0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-00008300: 7275 6e28 636d 642c 2065 6e76 3d65 6e76  run(cmd, env=env
-00008310: 2c20 2a2a 6b77 6172 6773 2920 2023 206f  , **kwargs)  # o
-00008320: 7574 5f73 7472 6561 6d3d 6f75 745f 7374  ut_stream=out_st
-00008330: 7265 616d 2c0a 0a20 2020 2020 2020 2074  ream,..        t
-00008340: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-00008350: 2320 5761 7463 6820 6f75 7420 666f 7220  # Watch out for 
-00008360: 556e 6963 6f64 6545 6e63 6f64 6545 7272  UnicodeEncodeErr
-00008370: 6f72 2077 6865 6e20 796f 7520 7374 7228  or when you str(
-00008380: 2920 7468 6973 2e0a 2020 2020 2020 2020  ) this..        
-00008390: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-000083a0: 6622 7b72 6573 756c 742e 7374 646f 7574  f"{result.stdout
-000083b0: 7d22 290a 2020 2020 2020 2020 6578 6365  }").        exce
-000083c0: 7074 2055 6e69 636f 6465 456e 636f 6465  pt UnicodeEncode
-000083d0: 4572 726f 7220 6173 2065 3a0a 2020 2020  Error as e:.    
-000083e0: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
-000083f0: 7272 6f72 2866 2255 6e69 636f 6465 2065  rror(f"Unicode e
-00008400: 7272 6f72 3a20 7b65 7d22 290a 2020 2020  rror: {e}").    
-00008410: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
-00008420: 4f4e 4c59 2073 7464 6f75 7420 5245 434f  ONLY stdout RECO
-00008430: 4445 204e 4545 4445 443f 3f20 6f72 2061  DE NEEDED?? or a
-00008440: 6c73 6f20 6572 726f 723f 0a20 2020 2020  lso error?.     
-00008450: 2020 2020 2020 2072 6573 756c 742e 7374         result.st
-00008460: 646f 7574 203d 2072 6573 756c 742e 7374  dout = result.st
-00008470: 646f 7574 2e65 6e63 6f64 6528 0a20 2020  dout.encode(.   
-00008480: 2020 2020 2020 2020 2020 2020 2027 7574               'ut
-00008490: 662d 3827 2c20 2769 676e 6f72 6527 292e  f-8', 'ignore').
-000084a0: 6465 636f 6465 2827 7574 662d 3827 290a  decode('utf-8').
-000084b0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000084c0: 6573 756c 740a 0a20 2020 2064 6566 2073  esult..    def s
-000084d0: 7472 5f74 6f5f 636c 6173 7328 7365 6c66  tr_to_class(self
-000084e0: 2c20 6d6f 6475 6c65 5f6e 616d 653a 2073  , module_name: s
-000084f0: 7472 2c20 636c 6173 735f 6e61 6d65 3a20  tr, class_name: 
-00008500: 7374 722c 202a 6172 6773 2c20 2a2a 6b77  str, *args, **kw
-00008510: 6172 6773 293a 0a20 2020 2020 2020 2022  args):.        "
-00008520: 2222 0a20 2020 2020 2020 2052 6574 7572  "".        Retur
-00008530: 6e20 6120 636c 6173 7320 696e 7374 616e  n a class instan
-00008540: 6365 2066 726f 6d20 6120 7374 7269 6e67  ce from a string
-00008550: 2072 6566 6572 656e 6365 2e0a 0a20 2020   reference...   
-00008560: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00008570: 2020 2020 2020 206d 6f64 756c 655f 6e61         module_na
-00008580: 6d65 2028 7374 7229 3a20 5468 6520 6e61  me (str): The na
-00008590: 6d65 206f 6620 7468 6520 6d6f 6475 6c65  me of the module
-000085a0: 2e0a 2020 2020 2020 2020 2020 2020 636c  ..            cl
-000085b0: 6173 735f 6e61 6d65 2028 7374 7229 3a20  ass_name (str): 
-000085c0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-000085d0: 636c 6173 732e 0a20 2020 2020 2020 2020  class..         
-000085e0: 2020 202a 6172 6773 3a20 4164 6469 7469     *args: Additi
-000085f0: 6f6e 616c 2070 6f73 6974 696f 6e61 6c20  onal positional 
-00008600: 6172 6775 6d65 6e74 7320 666f 7220 7468  arguments for th
-00008610: 6520 636c 6173 7320 636f 6e73 7472 7563  e class construc
-00008620: 746f 722e 0a20 2020 2020 2020 2020 2020  tor..           
-00008630: 202a 2a6b 7761 7267 733a 2041 6464 6974   **kwargs: Addit
-00008640: 696f 6e61 6c20 6b65 7977 6f72 6420 6172  ional keyword ar
-00008650: 6775 6d65 6e74 7320 666f 7220 7468 6520  guments for the 
-00008660: 636c 6173 7320 636f 6e73 7472 7563 746f  class constructo
-00008670: 722e 0a0a 2020 2020 2020 2020 5265 7475  r...        Retu
-00008680: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00008690: 206f 626a 6563 743a 2041 6e20 696e 7374   object: An inst
-000086a0: 616e 6365 206f 6620 7468 6520 7370 6563  ance of the spec
-000086b0: 6966 6965 6420 636c 6173 732c 206f 7220  ified class, or 
-000086c0: 4e6f 6e65 2069 6620 7468 6520 636c 6173  None if the clas
-000086d0: 7320 6f72 0a20 2020 2020 2020 2020 2020  s or.           
-000086e0: 2020 2020 206d 6f64 756c 6520 646f 6573       module does
-000086f0: 206e 6f74 2065 7869 7374 2e0a 2020 2020   not exist..    
-00008700: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008710: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00008720: 206d 6f64 756c 655f 203d 2069 6d70 6f72   module_ = impor
-00008730: 746c 6962 2e69 6d70 6f72 745f 6d6f 6475  tlib.import_modu
-00008740: 6c65 286d 6f64 756c 655f 6e61 6d65 290a  le(module_name).
-00008750: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-00008760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008770: 2063 6c61 7373 5f20 3d20 6765 7461 7474   class_ = getatt
-00008780: 7228 6d6f 6475 6c65 5f2c 2063 6c61 7373  r(module_, class
-00008790: 5f6e 616d 6529 282a 6172 6773 2c20 2a2a  _name)(*args, **
-000087a0: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
-000087b0: 2020 2020 6578 6365 7074 2041 7474 7269      except Attri
-000087c0: 6275 7465 4572 726f 723a 0a20 2020 2020  buteError:.     
-000087d0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-000087e0: 722e 6572 726f 7228 2743 6c61 7373 2064  r.error('Class d
-000087f0: 6f65 7320 6e6f 7420 6578 6973 7427 290a  oes not exist').
-00008800: 2020 2020 2020 2020 6578 6365 7074 2049          except I
-00008810: 6d70 6f72 7445 7272 6f72 3a0a 2020 2020  mportError:.    
-00008820: 2020 2020 2020 2020 6c6f 6767 6572 2e65          logger.e
-00008830: 7272 6f72 2827 4d6f 6475 6c65 2064 6f65  rror('Module doe
-00008840: 7320 6e6f 7420 6578 6973 7427 290a 2020  s not exist').  
-00008850: 2020 2020 2020 7265 7475 726e 2063 6c61        return cla
-00008860: 7373 5f20 6f72 204e 6f6e 650a 0a20 2020  ss_ or None..   
-00008870: 2064 6566 2072 756e 5f63 6f6d 6d61 6e64   def run_command
-00008880: 735f 7370 6c69 745f 6f75 7428 7365 6c66  s_split_out(self
-00008890: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000088a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088b0: 2063 6d64 6c69 7374 3a20 4c69 7374 5b73   cmdlist: List[s
-000088c0: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 2020 656e 763a 204f 7074 696f 6e61      env: Optiona
-000088f0: 6c5b 4469 6374 5b73 7472 2c20 7374 725d  l[Dict[str, str]
-00008900: 5d20 3d20 4e6f 6e65 0a20 2020 2020 2020  ] = None.       
-00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008920: 2020 2020 2020 2020 2920 2d3e 204c 6973          ) -> Lis
-00008930: 745b 7374 725d 3a0a 2020 2020 2020 2020  t[str]:.        
-00008940: 2222 2252 756e 2061 206c 6973 7420 6f66  """Run a list of
-00008950: 2073 6865 6c6c 2063 6f6d 6d61 6e64 7320   shell commands 
-00008960: 636f 6e73 6563 7574 6976 656c 7920 616e  consecutively an
-00008970: 6420 7370 6c69 7420 7468 6520 6f75 7470  d split the outp
-00008980: 7574 0a20 2020 2020 2020 206f 6620 6561  ut.        of ea
-00008990: 6368 2063 6f6d 6d61 6e64 2e0a 0a20 2020  ch command...   
-000089a0: 2020 2020 2045 6163 6820 636f 6d6d 616e       Each comman
-000089b0: 6420 696e 2074 6865 206c 6973 7420 6973  d in the list is
-000089c0: 2065 7865 6375 7465 6420 7769 7468 2061   executed with a
-000089d0: 2073 6570 6172 6174 6f72 2069 6e20 6265   separator in be
-000089e0: 7477 6565 6e0a 2020 2020 2020 2020 7468  tween.        th
-000089f0: 6174 2069 7320 756e 6971 7565 2061 6e64  at is unique and
-00008a00: 2063 616e 2062 6520 7573 6564 2074 6f20   can be used to 
-00008a10: 7370 6c69 740a 2020 2020 2020 2020 7468  split.        th
-00008a20: 6520 6f75 7470 7574 206f 6620 6561 6368  e output of each
-00008a30: 2063 6f6d 6d61 6e64 206c 6174 6572 2e20   command later. 
-00008a40: 5468 6520 7365 7061 7261 746f 7220 7573  The separator us
-00008a50: 6564 2069 7320 7370 6563 6966 6965 640a  ed is specified.
-00008a60: 2020 2020 2020 2020 6279 2074 6865 2060          by the `
-00008a70: 5f4f 5554 5f53 4550 6020 6174 7472 6962  _OUT_SEP` attrib
-00008a80: 7574 6520 6f66 2074 6865 0a20 2020 2020  ute of the.     
-00008a90: 2020 2053 6c75 726d 436c 6965 6e74 2069     SlurmClient i
-00008aa0: 6e73 7461 6e63 652e 0a0a 2020 2020 2020  nstance...      
-00008ab0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00008ac0: 2020 2020 636d 646c 6973 7420 284c 6973      cmdlist (Lis
-00008ad0: 745b 7374 725d 293a 2041 206c 6973 7420  t[str]): A list 
-00008ae0: 6f66 2073 6865 6c6c 2063 6f6d 6d61 6e64  of shell command
-00008af0: 7320 746f 2072 756e 2e0a 2020 2020 2020  s to run..      
-00008b00: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
-00008b10: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
-00008b20: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
-00008b30: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00008b40: 626c 6573 200a 2020 2020 2020 2020 2020  bles .          
-00008b50: 2020 2020 2020 746f 2073 6574 2077 6865        to set whe
-00008b60: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
-00008b70: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
-00008b80: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
-00008b90: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00008ba0: 2020 2020 2020 204c 6973 745b 7374 725d         List[str]
-00008bb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00008bc0: 2020 4120 6c69 7374 206f 6620 7374 7269    A list of stri
-00008bd0: 6e67 732c 2077 6865 7265 2065 6163 6820  ngs, where each 
-00008be0: 7374 7269 6e67 2063 6f72 7265 7370 6f6e  string correspon
-00008bf0: 6473 2074 6f0a 2020 2020 2020 2020 2020  ds to.          
-00008c00: 2020 2020 2020 7468 6520 6f75 7470 7574        the output
-00008c10: 206f 6620 6120 7369 6e67 6c65 2063 6f6d   of a single com
-00008c20: 6d61 6e64 2069 6e20 6063 6d64 6c69 7374  mand in `cmdlist
-00008c30: 6020 7370 6c69 740a 2020 2020 2020 2020  ` split.        
-00008c40: 2020 2020 2020 2020 6279 2074 6865 2073          by the s
-00008c50: 6570 6172 6174 6f72 2060 5f4f 5554 5f53  eparator `_OUT_S
-00008c60: 4550 602e 0a0a 2020 2020 2020 2020 5261  EP`...        Ra
-00008c70: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
-00008c80: 2020 5353 4845 7863 6570 7469 6f6e 3a20    SSHException: 
-00008c90: 4966 2061 6e79 206f 6620 7468 6520 636f  If any of the co
-00008ca0: 6d6d 616e 6473 2066 6169 6c20 746f 2065  mmands fail to e
-00008cb0: 7865 6375 7465 2073 7563 6365 7373 6675  xecute successfu
-00008cc0: 6c6c 792e 0a20 2020 2020 2020 2022 2222  lly..        """
-00008cd0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-00008ce0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-00008cf0: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
-00008d00: 616e 6473 2863 6d64 6c69 7374 3d63 6d64  ands(cmdlist=cmd
-00008d10: 6c69 7374 2c0a 2020 2020 2020 2020 2020  list,.          
-00008d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d30: 2020 2020 2020 2020 2020 2020 2065 6e76               env
-00008d40: 3d65 6e76 2c0a 2020 2020 2020 2020 2020  =env,.          
-00008d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008d60: 2020 2020 2020 2020 2020 2020 2073 6570               sep
-00008d70: 3d66 2220 3b20 6563 686f 207b 7365 6c66  =f" ; echo {self
-00008d80: 2e5f 4f55 545f 5345 507d 203b 2022 290a  ._OUT_SEP} ; ").
-00008d90: 2020 2020 2020 2020 6578 6365 7074 2055          except U
-00008da0: 6e65 7870 6563 7465 6445 7869 7420 6173  nexpectedExit as
-00008db0: 2065 3a0a 2020 2020 2020 2020 2020 2020   e:.            
-00008dc0: 6c6f 6767 6572 2e77 6172 6e69 6e67 2865  logger.warning(e
-00008dd0: 290a 2020 2020 2020 2020 2020 2020 7265  ).            re
-00008de0: 7375 6c74 203d 2065 2e72 6573 756c 740a  sult = e.result.
-00008df0: 2020 2020 2020 2020 6966 2072 6573 756c          if resul
-00008e00: 742e 6f6b 3a0a 2020 2020 2020 2020 2020  t.ok:.          
-00008e10: 2020 7265 7370 6f6e 7365 203d 2072 6573    response = res
-00008e20: 756c 742e 7374 646f 7574 0a20 2020 2020  ult.stdout.     
-00008e30: 2020 2020 2020 2073 706c 6974 5f72 6573         split_res
-00008e40: 706f 6e73 6573 203d 2072 6573 706f 6e73  ponses = respons
-00008e50: 652e 7370 6c69 7428 7365 6c66 2e5f 4f55  e.split(self._OU
-00008e60: 545f 5345 5029 0a20 2020 2020 2020 2020  T_SEP).         
-00008e70: 2020 2072 6574 7572 6e20 7370 6c69 745f     return split_
-00008e80: 7265 7370 6f6e 7365 730a 2020 2020 2020  responses.      
-00008e90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00008ea0: 2020 2020 2320 4966 2074 6865 2072 6573      # If the res
-00008eb0: 756c 7420 6973 206e 6f74 206f 6b2c 206c  ult is not ok, l
-00008ec0: 6f67 2074 6865 2065 7272 6f72 2061 6e64  og the error and
-00008ed0: 2072 6169 7365 2061 6e20 5353 4845 7863   raise an SSHExc
-00008ee0: 6570 7469 6f6e 0a20 2020 2020 2020 2020  eption.         
-00008ef0: 2020 2065 7272 6f72 203d 2066 2252 6573     error = f"Res
-00008f00: 756c 7420 6973 206e 6f74 206f 6b3a 207b  ult is not ok: {
-00008f10: 7265 7375 6c74 7d22 0a20 2020 2020 2020  result}".       
-00008f20: 2020 2020 206c 6f67 6765 722e 6572 726f       logger.erro
-00008f30: 7228 6572 726f 7229 0a20 2020 2020 2020  r(error).       
-00008f40: 2020 2020 2072 6169 7365 2053 5348 4578       raise SSHEx
-00008f50: 6365 7074 696f 6e28 6572 726f 7229 0a0a  ception(error)..
-00008f60: 2020 2020 6465 6620 6c69 7374 5f61 6374      def list_act
-00008f70: 6976 655f 6a6f 6273 2873 656c 662c 0a20  ive_jobs(self,. 
-00008f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008f90: 2020 2020 2020 2020 656e 763a 204f 7074          env: Opt
-00008fa0: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
-00008fb0: 7374 725d 5d20 3d20 4e6f 6e65 2920 2d3e  str]] = None) ->
-00008fc0: 204c 6973 745b 7374 725d 3a0a 2020 2020   List[str]:.    
-00008fd0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008fe0: 4765 7420 6120 6c69 7374 206f 6620 6163  Get a list of ac
-00008ff0: 7469 7665 206a 6f62 7320 6672 6f6d 2053  tive jobs from S
-00009000: 4c55 524d 2e0a 0a20 2020 2020 2020 2041  LURM...        A
-00009010: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00009020: 2065 6e76 2028 4469 6374 5b73 7472 2c20   env (Dict[str, 
-00009030: 7374 725d 2c20 6f70 7469 6f6e 616c 293a  str], optional):
-00009040: 204f 7074 696f 6e61 6c20 656e 7669 726f   Optional enviro
-00009050: 6e6d 656e 7420 7661 7269 6162 6c65 7320  nment variables 
-00009060: 746f 200a 2020 2020 2020 2020 2020 2020  to .            
-00009070: 2020 2020 7365 7420 7768 656e 2072 756e      set when run
-00009080: 6e69 6e67 2074 6865 2063 6f6d 6d61 6e64  ning the command
-00009090: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
-000090a0: 6e65 2e0a 0a20 2020 2020 2020 2052 6574  ne...        Ret
-000090b0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-000090c0: 2020 4c69 7374 5b73 7472 5d3a 2041 206c    List[str]: A l
-000090d0: 6973 7420 6f66 206a 6f62 2049 4473 2e0a  ist of job IDs..
-000090e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000090f0: 2020 2020 2320 636d 6420 3d20 7365 6c66      # cmd = self
-00009100: 2e5f 4143 5449 5645 5f4a 4f42 535f 434d  ._ACTIVE_JOBS_CM
-00009110: 440a 2020 2020 2020 2020 636d 6420 3d20  D.        cmd = 
-00009120: 7365 6c66 2e67 6574 5f6a 6f62 735f 696e  self.get_jobs_in
-00009130: 666f 5f63 6f6d 6d61 6e64 2873 7461 7274  fo_command(start
-00009140: 5f74 696d 653d 226e 6f77 222c 2073 7461  _time="now", sta
-00009150: 7465 733d 2272 2229 0a20 2020 2020 2020  tes="r").       
-00009160: 206c 6f67 6765 722e 696e 666f 2822 5265   logger.info("Re
-00009170: 7472 6965 7669 6e67 206c 6973 7420 6f66  trieving list of
-00009180: 2061 6374 6976 6520 6a6f 6273 2066 726f   active jobs fro
-00009190: 6d20 536c 7572 6d22 290a 2020 2020 2020  m Slurm").      
-000091a0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-000091b0: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
-000091c0: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
-000091d0: 2020 2020 206a 6f62 5f6c 6973 7420 3d20       job_list = 
-000091e0: 7265 7375 6c74 2e73 7464 6f75 742e 7374  result.stdout.st
-000091f0: 7269 7028 292e 7370 6c69 7428 275c 6e27  rip().split('\n'
-00009200: 290a 2020 2020 2020 2020 6a6f 625f 6c69  ).        job_li
-00009210: 7374 2e72 6576 6572 7365 2829 0a20 2020  st.reverse().   
-00009220: 2020 2020 2072 6574 7572 6e20 6a6f 625f       return job_
-00009230: 6c69 7374 0a0a 2020 2020 6465 6620 6c69  list..    def li
-00009240: 7374 5f63 6f6d 706c 6574 6564 5f6a 6f62  st_completed_job
-00009250: 7328 7365 6c66 2c0a 2020 2020 2020 2020  s(self,.        
-00009260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009270: 2020 2020 656e 763a 204f 7074 696f 6e61      env: Optiona
-00009280: 6c5b 4469 6374 5b73 7472 2c20 7374 725d  l[Dict[str, str]
-00009290: 5d20 3d20 4e6f 6e65 2920 2d3e 204c 6973  ] = None) -> Lis
-000092a0: 745b 7374 725d 3a0a 2020 2020 2020 2020  t[str]:.        
-000092b0: 2222 220a 2020 2020 2020 2020 4765 7420  """.        Get 
-000092c0: 6120 6c69 7374 206f 6620 636f 6d70 6c65  a list of comple
-000092d0: 7465 6420 6a6f 6273 2066 726f 6d20 534c  ted jobs from SL
-000092e0: 5552 4d2e 0a0a 2020 2020 2020 2020 4172  URM...        Ar
-000092f0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00009300: 656e 7620 2844 6963 745b 7374 722c 2073  env (Dict[str, s
-00009310: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
-00009320: 4f70 7469 6f6e 616c 2065 6e76 6972 6f6e  Optional environ
-00009330: 6d65 6e74 2076 6172 6961 626c 6573 2074  ment variables t
-00009340: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
-00009350: 2020 7365 7420 7768 656e 2072 756e 6e69    set when runni
-00009360: 6e67 2074 6865 2063 6f6d 6d61 6e64 2e20  ng the command. 
-00009370: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-00009380: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00009390: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-000093a0: 4c69 7374 5b73 7472 5d3a 2041 206c 6973  List[str]: A lis
-000093b0: 7420 6f66 206a 6f62 2049 4473 2e0a 2020  t of job IDs..  
-000093c0: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
-000093d0: 2020 2063 6d64 203d 2073 656c 662e 6765     cmd = self.ge
-000093e0: 745f 6a6f 6273 5f69 6e66 6f5f 636f 6d6d  t_jobs_info_comm
-000093f0: 616e 6428 7374 6174 6573 3d22 6364 2229  and(states="cd")
-00009400: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00009410: 696e 666f 2822 5265 7472 6965 7669 6e67  info("Retrieving
-00009420: 2061 206c 6973 7420 6f66 2063 6f6d 706c   a list of compl
-00009430: 6574 6564 206a 6f62 7320 6672 6f6d 2053  eted jobs from S
-00009440: 6c75 726d 2229 0a20 2020 2020 2020 2072  lurm").        r
-00009450: 6573 756c 7420 3d20 7365 6c66 2e72 756e  esult = self.run
-00009460: 5f63 6f6d 6d61 6e64 7328 5b63 6d64 5d2c  _commands([cmd],
-00009470: 2065 6e76 3d65 6e76 290a 2020 2020 2020   env=env).      
-00009480: 2020 6a6f 625f 6c69 7374 203d 205b 6a6f    job_list = [jo
-00009490: 622e 7374 7269 7028 2920 666f 7220 6a6f  b.strip() for jo
-000094a0: 6220 696e 2072 6573 756c 742e 7374 646f  b in result.stdo
-000094b0: 7574 2e73 7472 6970 2829 2e73 706c 6974  ut.strip().split
-000094c0: 2827 5c6e 2729 5d0a 2020 2020 2020 2020  ('\n')].        
-000094d0: 6a6f 625f 6c69 7374 2e72 6576 6572 7365  job_list.reverse
-000094e0: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
-000094f0: 6e20 6a6f 625f 6c69 7374 0a0a 2020 2020  n job_list..    
-00009500: 6465 6620 6c69 7374 5f61 6c6c 5f6a 6f62  def list_all_job
-00009510: 7328 7365 6c66 2c20 656e 763a 204f 7074  s(self, env: Opt
-00009520: 696f 6e61 6c5b 4469 6374 5b73 7472 2c20  ional[Dict[str, 
-00009530: 7374 725d 5d20 3d20 4e6f 6e65 2920 2d3e  str]] = None) ->
-00009540: 204c 6973 745b 7374 725d 3a0a 2020 2020   List[str]:.    
-00009550: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00009560: 4765 7420 6120 6c69 7374 206f 6620 616c  Get a list of al
-00009570: 6c20 6a6f 6273 2066 726f 6d20 534c 5552  l jobs from SLUR
-00009580: 4d2e 0a0a 2020 2020 2020 2020 4172 6773  M...        Args
-00009590: 3a0a 2020 2020 2020 2020 2020 2020 656e  :.            en
-000095a0: 7620 2844 6963 745b 7374 722c 2073 7472  v (Dict[str, str
-000095b0: 5d2c 206f 7074 696f 6e61 6c29 3a20 4f70  ], optional): Op
-000095c0: 7469 6f6e 616c 2065 6e76 6972 6f6e 6d65  tional environme
-000095d0: 6e74 2076 6172 6961 626c 6573 200a 2020  nt variables .  
-000095e0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-000095f0: 2073 6574 2077 6865 6e20 7275 6e6e 696e   set when runnin
-00009600: 6720 7468 6520 636f 6d6d 616e 642e 2044  g the command. D
-00009610: 6566 6175 6c74 7320 746f 204e 6f6e 652e  efaults to None.
-00009620: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00009630: 733a 0a20 2020 2020 2020 2020 2020 204c  s:.            L
-00009640: 6973 745b 7374 725d 3a20 4120 6c69 7374  ist[str]: A list
-00009650: 206f 6620 6a6f 6220 4944 732e 0a20 2020   of job IDs..   
-00009660: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-00009670: 2020 636d 6420 3d20 7365 6c66 2e67 6574    cmd = self.get
-00009680: 5f6a 6f62 735f 696e 666f 5f63 6f6d 6d61  _jobs_info_comma
-00009690: 6e64 2829 0a20 2020 2020 2020 206c 6f67  nd().        log
-000096a0: 6765 722e 696e 666f 2822 5265 7472 6965  ger.info("Retrie
-000096b0: 7669 6e67 2061 206c 6973 7420 6f66 2061  ving a list of a
-000096c0: 6c6c 206a 6f62 7320 6672 6f6d 2053 6c75  ll jobs from Slu
-000096d0: 726d 2229 0a20 2020 2020 2020 2072 6573  rm").        res
-000096e0: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
-000096f0: 6f6d 6d61 6e64 7328 5b63 6d64 5d2c 2065  ommands([cmd], e
-00009700: 6e76 3d65 6e76 290a 2020 2020 2020 2020  nv=env).        
-00009710: 6a6f 625f 6c69 7374 203d 2072 6573 756c  job_list = resul
-00009720: 742e 7374 646f 7574 2e73 7472 6970 2829  t.stdout.strip()
-00009730: 2e73 706c 6974 2827 5c6e 2729 0a20 2020  .split('\n').   
-00009740: 2020 2020 206a 6f62 5f6c 6973 742e 7265       job_list.re
-00009750: 7665 7273 6528 290a 2020 2020 2020 2020  verse().        
-00009760: 7265 7475 726e 206a 6f62 5f6c 6973 740a  return job_list.
-00009770: 0a20 2020 2064 6566 2067 6574 5f6a 6f62  .    def get_job
-00009780: 735f 696e 666f 5f63 6f6d 6d61 6e64 2873  s_info_command(s
-00009790: 656c 662c 2073 7461 7274 5f74 696d 653a  elf, start_time:
-000097a0: 2073 7472 203d 2022 3230 3233 2d30 312d   str = "2023-01-
-000097b0: 3031 222c 0a20 2020 2020 2020 2020 2020  01",.           
-000097c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000097d0: 2020 2065 6e64 5f74 696d 653a 2073 7472     end_time: str
-000097e0: 203d 2022 6e6f 7722 2c0a 2020 2020 2020   = "now",.      
-000097f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009800: 2020 2020 2020 2020 636f 6c75 6d6e 733a          columns:
-00009810: 2073 7472 203d 2022 4a6f 6249 6422 2c0a   str = "JobId",.
-00009820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009830: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00009840: 6174 6573 3a20 7374 7220 3d20 2272 2c63  ates: str = "r,c
-00009850: 642c 662c 746f 2c72 732c 646c 2c6e 6622  d,f,to,rs,dl,nf"
-00009860: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-00009870: 2020 2222 2252 6574 7572 6e20 7468 6520    """Return the 
-00009880: 536c 7572 6d20 636f 6d6d 616e 6420 746f  Slurm command to
-00009890: 2072 6574 7269 6576 6520 696e 666f 726d   retrieve inform
-000098a0: 6174 696f 6e20 6162 6f75 7420 6f6c 6420  ation about old 
-000098b0: 6a6f 6273 2e0a 0a20 2020 2020 2020 2054  jobs...        T
-000098c0: 6865 2063 6f6d 6d61 6e64 2077 696c 6c20  he command will 
-000098d0: 6265 2066 6f72 6d61 7474 6564 2077 6974  be formatted wit
-000098e0: 6820 7468 6520 7370 6563 6966 6965 6420  h the specified 
-000098f0: 7374 6172 7420 7469 6d65 2c20 7768 6963  start time, whic
-00009900: 6820 6973 0a20 2020 2020 2020 2065 7870  h is.        exp
-00009910: 6563 7465 6420 746f 2062 6520 696e 2074  ected to be in t
-00009920: 6865 2049 534f 2066 6f72 6d61 7420 2259  he ISO format "Y
-00009930: 5959 592d 4d4d 2d44 4422 2e0a 2020 2020  YYY-MM-DD"..    
-00009940: 2020 2020 5468 6520 636f 6d6d 616e 6420      The command 
-00009950: 7769 6c6c 2075 7365 2074 6865 2022 7361  will use the "sa
-00009960: 6363 7422 2074 6f6f 6c20 746f 2071 7565  cct" tool to que
-00009970: 7279 2074 6865 0a20 2020 2020 2020 2053  ry the.        S
-00009980: 6c75 726d 2061 6363 6f75 6e74 696e 6720  lurm accounting 
-00009990: 6461 7461 6261 7365 2066 6f72 206a 6f62  database for job
-000099a0: 7320 7468 6174 2073 7461 7274 6564 206f  s that started o
-000099b0: 6e20 6f72 2061 6674 6572 2074 6865 0a20  n or after the. 
-000099c0: 2020 2020 2020 2073 7065 6369 6669 6564         specified
-000099d0: 2073 7461 7274 2074 696d 652c 2061 6e64   start time, and
-000099e0: 2077 696c 6c20 6f75 7470 7574 206f 6e6c   will output onl
-000099f0: 7920 7468 6520 6a6f 6220 4944 7320 282d  y the job IDs (-
-00009a00: 6f20 4a6f 6249 6429 0a20 2020 2020 2020  o JobId).       
-00009a10: 2077 6974 686f 7574 2068 6561 6465 7220   without header 
-00009a20: 6f72 2074 7261 696c 6572 206c 696e 6573  or trailer lines
-00009a30: 2028 2d6e 202d 5829 2e0a 0a20 2020 2020   (-n -X)...     
-00009a40: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00009a50: 2020 2020 2073 7461 7274 5f74 696d 6520       start_time 
-00009a60: 2873 7472 293a 2054 6865 2073 7461 7274  (str): The start
-00009a70: 2074 696d 6520 6672 6f6d 2077 6869 6368   time from which
-00009a80: 2074 6f20 7265 7472 6965 7665 206a 6f62   to retrieve job
-00009a90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009aa0: 2069 6e66 6f72 6d61 7469 6f6e 2e20 4465   information. De
-00009ab0: 6661 756c 7473 2074 6f20 2232 3032 332d  faults to "2023-
-00009ac0: 3031 2d30 3122 2e0a 2020 2020 2020 2020  01-01"..        
-00009ad0: 2020 2020 656e 645f 7469 6d65 2028 7374      end_time (st
-00009ae0: 7229 3a20 5468 6520 656e 6420 7469 6d65  r): The end time
-00009af0: 2075 6e74 696c 2077 6869 6368 2074 6f20   until which to 
-00009b00: 7265 7472 6965 7665 206a 6f62 0a20 2020  retrieve job.   
-00009b10: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
-00009b20: 6f72 6d61 7469 6f6e 2e20 4465 6661 756c  ormation. Defaul
-00009b30: 7473 2074 6f20 226e 6f77 222e 0a20 2020  ts to "now"..   
-00009b40: 2020 2020 2020 2020 2063 6f6c 756d 6e73           columns
-00009b50: 2028 7374 7229 3a20 5468 6520 636f 6c75   (str): The colu
-00009b60: 6d6e 7320 746f 2072 6574 7269 6576 6520  mns to retrieve 
-00009b70: 6672 6f6d 2074 6865 206a 6f62 2069 6e66  from the job inf
-00009b80: 6f72 6d61 7469 6f6e 2e0a 2020 2020 2020  ormation..      
-00009b90: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00009ba0: 7473 2074 6f20 224a 6f62 4964 222e 2049  ts to "JobId". I
-00009bb0: 7420 6973 2063 6f6d 6d61 2073 6570 6172  t is comma separ
-00009bc0: 6174 6564 2c20 652e 672e 2022 4a6f 6249  ated, e.g. "JobI
-00009bd0: 642c 5374 6174 6522 2e0a 2020 2020 2020  d,State"..      
-00009be0: 2020 2020 2020 7374 6174 6573 2028 7374        states (st
-00009bf0: 7229 3a20 5468 6520 6a6f 6220 7374 6174  r): The job stat
-00009c00: 6573 2074 6f20 696e 636c 7564 6520 696e  es to include in
-00009c10: 2074 6865 2071 7565 7279 2e0a 2020 2020   the query..    
-00009c20: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-00009c30: 756c 7473 2074 6f20 2272 2c63 642c 662c  ults to "r,cd,f,
-00009c40: 746f 2c72 732c 646c 2c6e 6622 2e0a 0a20  to,rs,dl,nf"... 
-00009c50: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00009c60: 2020 2020 2020 2020 2020 2020 7374 723a              str:
-00009c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009c80: 2041 2073 7472 696e 6720 7265 7072 6573   A string repres
-00009c90: 656e 7469 6e67 2074 6865 2053 6c75 726d  enting the Slurm
-00009ca0: 2063 6f6d 6d61 6e64 2074 6f20 7265 7472   command to retr
-00009cb0: 6965 7665 0a20 2020 2020 2020 2020 2020  ieve.           
-00009cc0: 2020 2020 2069 6e66 6f72 6d61 7469 6f6e       information
-00009cd0: 2061 626f 7574 206f 6c64 206a 6f62 732e   about old jobs.
-00009ce0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00009cf0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-00009d00: 2e5f 414c 4c5f 4a4f 4253 5f43 4d44 2e66  ._ALL_JOBS_CMD.f
-00009d10: 6f72 6d61 7428 7374 6172 745f 7469 6d65  ormat(start_time
-00009d20: 3d73 7461 7274 5f74 696d 652c 0a20 2020  =start_time,.   
-00009d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d50: 2020 2020 2020 656e 645f 7469 6d65 3d65        end_time=e
-00009d60: 6e64 5f74 696d 652c 0a20 2020 2020 2020  nd_time,.       
-00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d90: 2020 7374 6174 6573 3d73 7461 7465 732c    states=states,
-00009da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dc0: 2020 2020 2020 2020 2020 636f 6c75 6d6e            column
-00009dd0: 733d 636f 6c75 6d6e 7329 0a0a 2020 2020  s=columns)..    
-00009de0: 6465 6620 7472 616e 7366 6572 5f64 6174  def transfer_dat
-00009df0: 6128 7365 6c66 2c20 6c6f 6361 6c5f 7061  a(self, local_pa
-00009e00: 7468 3a20 7374 7229 202d 3e20 5265 7375  th: str) -> Resu
-00009e10: 6c74 3a0a 2020 2020 2020 2020 2222 220a  lt:.        """.
-00009e20: 2020 2020 2020 2020 5472 616e 7366 6572          Transfer
-00009e30: 7320 6120 6669 6c65 206f 7220 6469 7265  s a file or dire
-00009e40: 6374 6f72 7920 6672 6f6d 2074 6865 206c  ctory from the l
-00009e50: 6f63 616c 206d 6163 6869 6e65 2074 6f20  ocal machine to 
-00009e60: 7468 6520 7265 6d6f 7465 0a20 2020 2020  the remote.     
-00009e70: 2020 2053 6c75 726d 2063 6c75 7374 6572     Slurm cluster
-00009e80: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00009e90: 0a20 2020 2020 2020 2020 2020 206c 6f63  .            loc
-00009ea0: 616c 5f70 6174 6820 2873 7472 293a 2054  al_path (str): T
-00009eb0: 6865 206c 6f63 616c 2070 6174 6820 746f  he local path to
-00009ec0: 2074 6865 2066 696c 6520 6f72 2064 6972   the file or dir
-00009ed0: 6563 746f 7279 2074 6f0a 2020 2020 2020  ectory to.      
-00009ee0: 2020 2020 2020 2020 2020 7472 616e 7366            transf
-00009ef0: 6572 2e0a 0a20 2020 2020 2020 2052 6574  er...        Ret
-00009f00: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-00009f10: 2020 5265 7375 6c74 3a20 5468 6520 7265    Result: The re
-00009f20: 7375 6c74 206f 6620 7468 6520 6669 6c65  sult of the file
-00009f30: 2074 7261 6e73 6665 7220 6f70 6572 6174   transfer operat
-00009f40: 696f 6e2e 0a20 2020 2020 2020 2022 2222  ion..        """
-00009f50: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-00009f60: 696e 666f 280a 2020 2020 2020 2020 2020  info(.          
-00009f70: 2020 6622 5472 616e 7366 6572 696e 6720    f"Transfering 
-00009f80: 6669 6c65 207b 6c6f 6361 6c5f 7061 7468  file {local_path
-00009f90: 7d20 746f 207b 7365 6c66 2e73 6c75 726d  } to {self.slurm
-00009fa0: 5f64 6174 615f 7061 7468 7d22 290a 2020  _data_path}").  
-00009fb0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00009fc0: 662e 7075 7428 6c6f 6361 6c3d 6c6f 6361  f.put(local=loca
-00009fd0: 6c5f 7061 7468 2c20 7265 6d6f 7465 3d73  l_path, remote=s
-00009fe0: 656c 662e 736c 7572 6d5f 6461 7461 5f70  elf.slurm_data_p
-00009ff0: 6174 6829 0a0a 2020 2020 6465 6620 756e  ath)..    def un
-0000a000: 7061 636b 5f64 6174 6128 7365 6c66 2c20  pack_data(self, 
-0000a010: 7a69 7066 696c 653a 2073 7472 2c0a 2020  zipfile: str,.  
-0000a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a030: 2020 656e 763a 204f 7074 696f 6e61 6c5b    env: Optional[
-0000a040: 4469 6374 5b73 7472 2c20 7374 725d 5d20  Dict[str, str]] 
-0000a050: 3d20 4e6f 6e65 2920 2d3e 2052 6573 756c  = None) -> Resul
-0000a060: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
-0000a070: 2020 2020 2020 2055 6e70 6163 6b73 2061         Unpacks a
-0000a080: 207a 6970 7065 6420 6669 6c65 206f 6e20   zipped file on 
-0000a090: 7468 6520 7265 6d6f 7465 2053 6c75 726d  the remote Slurm
-0000a0a0: 2063 6c75 7374 6572 2e0a 0a20 2020 2020   cluster...     
-0000a0b0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000a0c0: 2020 2020 207a 6970 6669 6c65 2028 7374       zipfile (st
-0000a0d0: 7229 3a20 5468 6520 6e61 6d65 206f 6620  r): The name of 
-0000a0e0: 7468 6520 7a69 7070 6564 2066 696c 6520  the zipped file 
-0000a0f0: 746f 2062 6520 756e 7061 636b 6564 2e0a  to be unpacked..
-0000a100: 0a20 2020 2020 2020 2020 2020 2065 6e76  .            env
-0000a110: 2028 4469 6374 5b73 7472 2c20 7374 725d   (Dict[str, str]
-0000a120: 2c20 6f70 7469 6f6e 616c 293a 204f 7074  , optional): Opt
-0000a130: 696f 6e61 6c20 656e 7669 726f 6e6d 656e  ional environmen
-0000a140: 7420 7661 7269 6162 6c65 7320 0a20 2020  t variables .   
-0000a150: 2020 2020 2020 2020 2020 2020 2074 6f20               to 
-0000a160: 7365 7420 7768 656e 2072 756e 6e69 6e67  set when running
-0000a170: 2074 6865 2063 6f6d 6d61 6e64 2e20 4465   the command. De
-0000a180: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
-0000a190: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000a1a0: 3a0a 2020 2020 2020 2020 2020 2020 5265  :.            Re
-0000a1b0: 7375 6c74 3a20 5468 6520 7265 7375 6c74  sult: The result
-0000a1c0: 206f 6620 7468 6520 636f 6d6d 616e 642e   of the command.
-0000a1d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000a1e0: 2020 2020 2063 6d64 203d 2073 656c 662e       cmd = self.
-0000a1f0: 6765 745f 756e 7a69 705f 636f 6d6d 616e  get_unzip_comman
-0000a200: 6428 7a69 7066 696c 6529 0a20 2020 2020  d(zipfile).     
-0000a210: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
-0000a220: 2255 6e70 6163 6b69 6e67 207b 7a69 7066  "Unpacking {zipf
-0000a230: 696c 657d 206f 6e20 536c 7572 6d22 290a  ile} on Slurm").
-0000a240: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000a250: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
-0000a260: 285b 636d 645d 2c20 656e 763d 656e 7629  ([cmd], env=env)
-0000a270: 0a0a 2020 2020 6465 6620 636f 6e76 6572  ..    def conver
-0000a280: 745f 6461 7461 2873 656c 662c 207a 6970  t_data(self, zip
-0000a290: 6669 6c65 3a20 7374 722c 0a20 2020 2020  file: str,.     
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2b0: 656e 763a 204f 7074 696f 6e61 6c5b 4469  env: Optional[Di
-0000a2c0: 6374 5b73 7472 2c20 7374 725d 5d20 3d20  ct[str, str]] = 
-0000a2d0: 4e6f 6e65 2920 2d3e 2052 6573 756c 743a  None) -> Result:
-0000a2e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000a2f0: 2020 2020 2055 6e70 6163 6b73 2061 207a       Unpacks a z
-0000a300: 6970 7065 6420 6669 6c65 206f 6e20 7468  ipped file on th
-0000a310: 6520 7265 6d6f 7465 2053 6c75 726d 2063  e remote Slurm c
-0000a320: 6c75 7374 6572 2e0a 0a20 2020 2020 2020  luster...       
-0000a330: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0000a340: 2020 207a 6970 6669 6c65 2028 7374 7229     zipfile (str)
-0000a350: 3a20 5468 6520 6e61 6d65 206f 6620 7468  : The name of th
-0000a360: 6520 7a69 7070 6564 2066 696c 6520 746f  e zipped file to
-0000a370: 2062 6520 756e 7061 636b 6564 2e0a 0a20   be unpacked... 
-0000a380: 2020 2020 2020 2020 2020 2065 6e76 2028             env (
-0000a390: 4469 6374 5b73 7472 2c20 7374 725d 2c20  Dict[str, str], 
-0000a3a0: 6f70 7469 6f6e 616c 293a 204f 7074 696f  optional): Optio
-0000a3b0: 6e61 6c20 656e 7669 726f 6e6d 656e 7420  nal environment 
-0000a3c0: 7661 7269 6162 6c65 7320 0a20 2020 2020  variables .     
-0000a3d0: 2020 2020 2020 2020 2020 2074 6f20 7365             to se
-0000a3e0: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
-0000a3f0: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
-0000a400: 756c 7473 2074 6f20 4e6f 6e65 2e0a 0a20  ults to None... 
-0000a410: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000a420: 2020 2020 2020 2020 2020 2020 5265 7375              Resu
-0000a430: 6c74 3a20 5468 6520 7265 7375 6c74 206f  lt: The result o
-0000a440: 6620 7468 6520 636f 6d6d 616e 642e 0a20  f the command.. 
-0000a450: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000a460: 2020 2063 6d64 203d 2073 656c 662e 6765     cmd = self.ge
-0000a470: 745f 636f 6e76 6572 745f 636f 6d6d 616e  t_convert_comman
-0000a480: 6428 7a69 7066 696c 6529 0a20 2020 2020  d(zipfile).     
-0000a490: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
-0000a4a0: 2243 6f6e 7665 7274 696e 6720 7b7a 6970  "Converting {zip
-0000a4b0: 6669 6c65 7d20 6f6e 2053 6c75 726d 2229  file} on Slurm")
-0000a4c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000a4d0: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-0000a4e0: 7328 5b63 6d64 5d2c 2065 6e76 3d65 6e76  s([cmd], env=env
-0000a4f0: 290a 0a20 2020 2064 6566 2067 656e 6572  )..    def gener
-0000a500: 6174 655f 736c 7572 6d5f 6a6f 625f 666f  ate_slurm_job_fo
-0000a510: 725f 776f 726b 666c 6f77 2873 656c 662c  r_workflow(self,
-0000a520: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a540: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
-0000a550: 773a 2073 7472 2c0a 2020 2020 2020 2020  w: str,.        
-0000a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a580: 7375 6273 7469 7475 7465 733a 2044 6963  substitutes: Dic
-0000a590: 745b 7374 722c 2073 7472 5d2c 0a20 2020  t[str, str],.   
-0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5c0: 2020 2020 2074 656d 706c 6174 653a 2073       template: s
-0000a5d0: 7472 203d 2022 6a6f 625f 7465 6d70 6c61  tr = "job_templa
-0000a5e0: 7465 2e73 6822 0a20 2020 2020 2020 2020  te.sh".         
+000009d0: 736c 7572 6d4a 6f62 2e63 6c65 616e 7570  slurmJob.cleanup
+000009e0: 2873 6c75 726d 436c 6965 6e74 290a 2020  (slurmClient).  
+000009f0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+00000a00: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
+00000a10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000a20: 206c 6f67 6765 722e 6572 726f 7228 6622   logger.error(f"
+00000a30: 2045 5252 4f52 2057 4954 4820 4a4f 423a   ERROR WITH JOB:
+00000a40: 207b 657d 2229 0a20 2020 2020 2020 2020   {e}").         
+00000a50: 2020 2020 2020 2072 6169 7365 2065 0a0a         raise e..
+00000a60: 2020 2020 2222 220a 2020 2020 0a20 2020      """.    .   
+00000a70: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
+00000a80: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+00000a90: 2020 2020 2073 7562 6d69 745f 7265 7375       submit_resu
+00000aa0: 6c74 3a20 5265 7375 6c74 2c0a 2020 2020  lt: Result,.    
+00000ab0: 2020 2020 2020 2020 2020 2020 206a 6f62               job
+00000ac0: 5f69 643a 2069 6e74 293a 0a20 2020 2020  _id: int):.     
+00000ad0: 2020 2022 2222 0a20 2020 2020 2020 2049     """.        I
+00000ae0: 6e69 7469 616c 697a 6520 6120 536c 7572  nitialize a Slur
+00000af0: 6d4a 6f62 2069 6e73 7461 6e63 652e 0a0a  mJob instance...
+00000b00: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00000b10: 2020 2020 2020 2020 2020 7375 626d 6974            submit
+00000b20: 5f72 6573 756c 7420 2852 6573 756c 7429  _result (Result)
+00000b30: 3a20 5468 6520 7265 7375 6c74 206f 6620  : The result of 
+00000b40: 7375 626d 6974 7469 6e67 2074 6865 206a  submitting the j
+00000b50: 6f62 2e0a 2020 2020 2020 2020 2020 2020  ob..            
+00000b60: 6a6f 625f 6964 2028 696e 7429 3a20 5468  job_id (int): Th
+00000b70: 6520 536c 7572 6d20 6a6f 6220 4944 2e0a  e Slurm job ID..
+00000b80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00000b90: 2020 2020 7365 6c66 2e6a 6f62 5f69 6420      self.job_id 
+00000ba0: 3d20 6a6f 625f 6964 0a20 2020 2020 2020  = job_id.       
+00000bb0: 2073 656c 662e 7375 626d 6974 5f72 6573   self.submit_res
+00000bc0: 756c 7420 3d20 7375 626d 6974 5f72 6573  ult = submit_res
+00000bd0: 756c 740a 2020 2020 2020 2020 7365 6c66  ult.        self
+00000be0: 2e6f 6b20 3d20 7365 6c66 2e73 7562 6d69  .ok = self.submi
+00000bf0: 745f 7265 7375 6c74 2e6f 6b0a 2020 2020  t_result.ok.    
+00000c00: 2020 2020 7365 6c66 2e6a 6f62 5f73 7461      self.job_sta
+00000c10: 7465 203d 204e 6f6e 650a 2020 2020 2020  te = None.      
+00000c20: 2020 7365 6c66 2e65 7272 6f72 5f6d 6573    self.error_mes
+00000c30: 7361 6765 203d 2073 656c 662e 7375 626d  sage = self.subm
+00000c40: 6974 5f72 6573 756c 742e 7374 6465 7272  it_result.stderr
+00000c50: 2069 6620 6861 7361 7474 7228 7365 6c66   if hasattr(self
+00000c60: 2e73 7562 6d69 745f 7265 7375 6c74 2c20  .submit_result, 
+00000c70: 2773 7464 6572 7227 2920 656c 7365 2027  'stderr') else '
+00000c80: 270a 0a20 2020 2064 6566 2077 6169 745f  '..    def wait_
+00000c90: 666f 725f 636f 6d70 6c65 7469 6f6e 2873  for_completion(s
+00000ca0: 656c 662c 2073 6c75 726d 436c 6965 6e74  elf, slurmClient
+00000cb0: 2c20 6f6d 6572 6f43 6f6e 6e29 202d 3e20  , omeroConn) -> 
+00000cc0: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
+00000cd0: 0a20 2020 2020 2020 2057 6169 7420 666f  .        Wait fo
+00000ce0: 7220 7468 6520 536c 7572 6d20 6a6f 6220  r the Slurm job 
+00000cf0: 746f 2072 6561 6368 2063 6f6d 706c 6574  to reach complet
+00000d00: 696f 6e2c 2063 616e 6365 6c6c 6174 696f  ion, cancellatio
+00000d10: 6e2c 2066 6169 6c75 7265 2c20 6f72 2074  n, failure, or t
+00000d20: 696d 656f 7574 2e0a 0a20 2020 2020 2020  imeout...       
+00000d30: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00000d40: 2020 2073 6c75 726d 436c 6965 6e74 3a20     slurmClient: 
+00000d50: 5468 6520 536c 7572 6d20 636c 6965 6e74  The Slurm client
+00000d60: 2e0a 2020 2020 2020 2020 2020 2020 6f6d  ..            om
+00000d70: 6572 6f43 6f6e 6e3a 2054 6865 204f 4d45  eroConn: The OME
+00000d80: 524f 2063 6f6e 6e65 6374 696f 6e2e 0a0a  RO connection...
+00000d90: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00000da0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00000db0: 3a20 5468 6520 6669 6e61 6c20 7374 6174  : The final stat
+00000dc0: 6520 6f66 2074 6865 2053 6c75 726d 206a  e of the Slurm j
+00000dd0: 6f62 2e0a 2020 2020 2020 2020 2222 220a  ob..        """.
+00000de0: 2020 2020 2020 2020 7768 696c 6520 7365          while se
+00000df0: 6c66 2e6a 6f62 5f73 7461 7465 206e 6f74  lf.job_state not
+00000e00: 2069 6e20 2822 4641 494c 4544 222c 200a   in ("FAILED", .
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e30: 2020 2020 2022 434f 4d50 4c45 5445 4422       "COMPLETED"
+00000e40: 2c20 0a20 2020 2020 2020 2020 2020 2020  , .             
+00000e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e60: 2020 2020 2020 2020 2243 414e 4345 4c4c          "CANCELL
+00000e70: 4544 222c 0a20 2020 2020 2020 2020 2020  ED",.           
+00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e90: 2020 2020 2020 2020 2020 2254 494d 454f            "TIMEO
+00000ea0: 5554 222c 0a20 2020 2020 2020 2020 2020  UT",.           
+00000eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ec0: 2020 2020 2020 2020 2020 2246 4149 4c45            "FAILE
+00000ed0: 442b 222c 200a 2020 2020 2020 2020 2020  D+", .          
+00000ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ef0: 2020 2020 2020 2020 2020 2022 434f 4d50             "COMP
+00000f00: 4c45 5445 442b 222c 200a 2020 2020 2020  LETED+", .      
+00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00000f30: 4341 4e43 454c 4c45 442b 222c 0a20 2020  CANCELLED+",.   
+00000f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f60: 2020 2254 494d 454f 5554 2b22 293a 0a20    "TIMEOUT+"):. 
+00000f70: 2020 2020 2020 2020 2020 206a 6f62 5f73             job_s
+00000f80: 7461 7475 735f 6469 6374 2c20 706f 6c6c  tatus_dict, poll
+00000f90: 5f72 6573 756c 7420 3d20 736c 7572 6d43  _result = slurmC
+00000fa0: 6c69 656e 742e 6368 6563 6b5f 6a6f 625f  lient.check_job_
+00000fb0: 7374 6174 7573 280a 2020 2020 2020 2020  status(.        
+00000fc0: 2020 2020 2020 2020 5b73 656c 662e 6a6f          [self.jo
+00000fd0: 625f 6964 5d29 0a20 2020 2020 2020 2020  b_id]).         
+00000fe0: 2020 2069 6620 6e6f 7420 706f 6c6c 5f72     if not poll_r
+00000ff0: 6573 756c 742e 6f6b 3a0a 2020 2020 2020  esult.ok:.      
+00001000: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+00001010: 2e77 6172 6e69 6e67 280a 2020 2020 2020  .warning(.      
+00001020: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+00001030: 4572 726f 7220 6368 6563 6b69 6e67 206a  Error checking j
+00001040: 6f62 2073 7461 7475 733a 7b70 6f6c 6c5f  ob status:{poll_
+00001050: 7265 7375 6c74 2e73 7464 6572 727d 2229  result.stderr}")
+00001060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001070: 2073 656c 662e 6a6f 625f 7374 6174 6520   self.job_state 
+00001080: 3d20 2246 4149 4c45 4422 0a20 2020 2020  = "FAILED".     
+00001090: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000010a0: 6572 726f 725f 6d65 7373 6167 6520 3d20  error_message = 
+000010b0: 706f 6c6c 5f72 6573 756c 742e 7374 6465  poll_result.stde
+000010c0: 7272 0a20 2020 2020 2020 2020 2020 2073  rr.            s
+000010d0: 656c 662e 6a6f 625f 7374 6174 6520 3d20  elf.job_state = 
+000010e0: 6a6f 625f 7374 6174 7573 5f64 6963 745b  job_status_dict[
+000010f0: 7365 6c66 2e6a 6f62 5f69 645d 0a20 2020  self.job_id].   
+00001100: 2020 2020 2020 2020 2023 2077 6169 7420           # wait 
+00001110: 666f 7220 3130 2073 6563 6f6e 6473 2062  for 10 seconds b
+00001120: 6566 6f72 6520 6368 6563 6b69 6e67 2061  efore checking a
+00001130: 6761 696e 0a20 2020 2020 2020 2020 2020  gain.           
+00001140: 206f 6d65 726f 436f 6e6e 2e6b 6565 7041   omeroConn.keepA
+00001150: 6c69 7665 2829 2020 2320 6b65 6570 2074  live()  # keep t
+00001160: 6865 204f 4d45 524f 2063 6f6e 6e65 6374  he OMERO connect
+00001170: 696f 6e20 616c 6976 650a 2020 2020 2020  ion alive.      
+00001180: 2020 2020 2020 7469 6d65 736c 6565 702e        timesleep.
+00001190: 736c 6565 7028 3130 290a 2020 2020 2020  sleep(10).      
+000011a0: 2020 6c6f 6767 6572 2e69 6e66 6f28 6622    logger.info(f"
+000011b0: 4a6f 6220 7b73 656c 662e 6a6f 625f 6964  Job {self.job_id
+000011c0: 7d20 6669 6e69 7368 6564 3a20 7b73 656c  } finished: {sel
+000011d0: 662e 6a6f 625f 7374 6174 657d 2229 0a20  f.job_state}"). 
+000011e0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+000011f0: 666f 280a 2020 2020 2020 2020 2020 2020  fo(.            
+00001200: 6622 596f 7520 6361 6e20 6765 7420 7468  f"You can get th
+00001210: 6520 6c6f 6766 696c 6520 7573 696e 6720  e logfile using 
+00001220: 6053 6c75 726d 2047 6574 2055 7064 6174  `Slurm Get Updat
+00001230: 6560 206f 6e20 6a6f 6220 7b73 656c 662e  e` on job {self.
+00001240: 6a6f 625f 6964 7d22 290a 2020 2020 2020  job_id}").      
+00001250: 2020 7265 7475 726e 2073 656c 662e 6a6f    return self.jo
+00001260: 625f 7374 6174 650a 2020 2020 0a20 2020  b_state.    .   
+00001270: 2064 6566 2063 6c65 616e 7570 2873 656c   def cleanup(sel
+00001280: 662c 2073 6c75 726d 436c 6965 6e74 2920  f, slurmClient) 
+00001290: 2d3e 2052 6573 756c 743a 0a20 2020 2020  -> Result:.     
+000012a0: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+000012b0: 6c65 616e 7570 2072 656d 6169 6e69 6e67  leanup remaining
+000012c0: 206c 6f67 2066 696c 6573 2e0a 0a20 2020   log files...   
+000012d0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+000012e0: 2020 2020 2020 2073 6c75 726d 436c 6965         slurmClie
+000012f0: 6e74 3a20 5468 6520 536c 7572 6d20 636c  nt: The Slurm cl
+00001300: 6965 6e74 2e0a 0a20 2020 2020 2020 2052  ient...        R
+00001310: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00001320: 2020 2020 5265 7375 6c74 3a20 5468 6520      Result: The 
+00001330: 7265 7375 6c74 206f 6620 7468 6520 636c  result of the cl
+00001340: 6561 6e75 7020 6f70 6572 6174 696f 6e2e  eanup operation.
+00001350: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00001360: 2020 2020 2072 6574 7572 6e20 736c 7572       return slur
+00001370: 6d43 6c69 656e 742e 636c 6561 6e75 705f  mClient.cleanup_
+00001380: 746d 705f 6669 6c65 7328 7365 6c66 2e6a  tmp_files(self.j
+00001390: 6f62 5f69 6429 0a0a 2020 2020 6465 6620  ob_id)..    def 
+000013a0: 636f 6d70 6c65 7465 6428 7365 6c66 293a  completed(self):
+000013b0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000013c0: 2020 2020 2043 6865 636b 2069 6620 7468       Check if th
+000013d0: 6520 536c 7572 6d20 6a6f 6220 6861 7320  e Slurm job has 
+000013e0: 636f 6d70 6c65 7465 6420 7375 6363 6573  completed succes
+000013f0: 7366 756c 6c79 2e0a 0a20 2020 2020 2020  sfully...       
+00001400: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00001410: 2020 2020 2020 626f 6f6c 3a20 5472 7565        bool: True
+00001420: 2069 6620 7468 6520 6a6f 6220 6861 7320   if the job has 
+00001430: 636f 6d70 6c65 7465 643b 2046 616c 7365  completed; False
+00001440: 206f 7468 6572 7769 7365 2e0a 2020 2020   otherwise..    
+00001450: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00001460: 7265 7475 726e 2073 656c 662e 6a6f 625f  return self.job_
+00001470: 7374 6174 6520 3d3d 2022 434f 4d50 4c45  state == "COMPLE
+00001480: 5445 4422 206f 7220 7365 6c66 2e6a 6f62  TED" or self.job
+00001490: 5f73 7461 7465 203d 3d20 2243 4f4d 504c  _state == "COMPL
+000014a0: 4554 4544 2b22 0a20 2020 200a 2020 2020  ETED+".    .    
+000014b0: 6465 6620 6765 745f 6572 726f 7228 7365  def get_error(se
+000014c0: 6c66 2920 2d3e 2073 7472 3a0a 2020 2020  lf) -> str:.    
+000014d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000014e0: 4765 7420 7468 6520 6572 726f 7220 6d65  Get the error me
+000014f0: 7373 6167 6520 6173 736f 6369 6174 6564  ssage associated
+00001500: 2077 6974 6820 7468 6520 536c 7572 6d20   with the Slurm 
+00001510: 6a6f 6220 7375 626d 6973 7369 6f6e 2e0a  job submission..
+00001520: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00001530: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
+00001540: 723a 2054 6865 2065 7272 6f72 206d 6573  r: The error mes
+00001550: 7361 6765 2c20 6f72 2061 6e20 656d 7074  sage, or an empt
+00001560: 7920 7374 7269 6e67 2069 6620 6e6f 2065  y string if no e
+00001570: 7272 6f72 206f 6363 7572 7265 642e 0a20  rror occurred.. 
+00001580: 2020 2020 2020 2022 2222 2020 2020 2020         """      
+00001590: 2020 0a20 2020 2020 2020 2072 6574 7572    .        retur
+000015a0: 6e20 7365 6c66 2e65 7272 6f72 5f6d 6573  n self.error_mes
+000015b0: 7361 6765 0a20 2020 2020 2020 200a 2020  sage.        .  
+000015c0: 2020 6465 6620 5f5f 7374 725f 5f28 7365    def __str__(se
+000015d0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000015e0: 0a20 2020 2020 2020 2052 6574 7572 6e20  .        Return 
+000015f0: 6120 7374 7269 6e67 2072 6570 7265 7365  a string represe
+00001600: 6e74 6174 696f 6e20 6f66 2074 6865 2053  ntation of the S
+00001610: 6c75 726d 4a6f 6220 696e 7374 616e 6365  lurmJob instance
+00001620: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00001630: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00001640: 7374 723a 2053 7472 696e 6720 7265 7072  str: String repr
+00001650: 6573 656e 7461 7469 6f6e 2e0a 2020 2020  esentation..    
+00001660: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00001670: 7072 6f70 6572 7469 6573 203d 2027 2c20  properties = ', 
+00001680: 272e 6a6f 696e 280a 2020 2020 2020 2020  '.join(.        
+00001690: 2020 2020 6622 7b6b 6579 7d3d 7b76 616c      f"{key}={val
+000016a0: 7565 7d22 2066 6f72 206b 6579 2c20 7661  ue}" for key, va
+000016b0: 6c75 6520 696e 2073 656c 662e 5f5f 6469  lue in self.__di
+000016c0: 6374 5f5f 2e69 7465 6d73 2829 290a 2020  ct__.items()).  
+000016d0: 2020 2020 2020 7265 7475 726e 2066 2253        return f"S
+000016e0: 6c75 726d 4a6f 6228 7b70 726f 7065 7274  lurmJob({propert
+000016f0: 6965 737d 2922 0a0a 0a63 6c61 7373 2053  ies})"...class S
+00001700: 6c75 726d 436c 6965 6e74 2843 6f6e 6e65  lurmClient(Conne
+00001710: 6374 696f 6e29 3a0a 2020 2020 2222 2241  ction):.    """A
+00001720: 2063 6c69 656e 7420 666f 7220 636f 6e6e   client for conn
+00001730: 6563 7469 6e67 2074 6f20 616e 6420 696e  ecting to and in
+00001740: 7465 7261 6374 696e 6720 7769 7468 2061  teracting with a
+00001750: 2053 6c75 726d 2063 6c75 7374 6572 206f   Slurm cluster o
+00001760: 7665 720a 2020 2020 5353 482e 0a0a 2020  ver.    SSH...  
+00001770: 2020 5468 6973 2063 6c61 7373 2065 7874    This class ext
+00001780: 656e 6473 2074 6865 2043 6f6e 6e65 6374  ends the Connect
+00001790: 696f 6e20 636c 6173 732c 2061 6464 696e  ion class, addin
+000017a0: 6720 6d65 7468 6f64 7320 616e 640a 2020  g methods and.  
+000017b0: 2020 6174 7472 6962 7574 6573 2073 7065    attributes spe
+000017c0: 6369 6669 6320 746f 2077 6f72 6b69 6e67  cific to working
+000017d0: 2077 6974 6820 536c 7572 6d2e 0a0a 2020   with Slurm...  
+000017e0: 2020 536c 7572 6d43 6c69 656e 7420 6163    SlurmClient ac
+000017f0: 6365 7074 7320 7468 6520 7361 6d65 2061  cepts the same a
+00001800: 7267 756d 656e 7473 2061 7320 436f 6e6e  rguments as Conn
+00001810: 6563 7469 6f6e 2e20 4265 6c6f 7720 6f6e  ection. Below on
+00001820: 6c79 0a20 2020 206d 656e 7469 6f6e 7320  ly.    mentions 
+00001830: 7468 6520 6164 6465 6420 6f6e 6573 3a0a  the added ones:.
+00001840: 0a20 2020 2054 6865 2065 6173 6965 7374  .    The easiest
+00001850: 2077 6179 2074 6f20 7365 7420 7468 6973   way to set this
+00001860: 2063 6c69 656e 7420 7570 2069 7320 6279   client up is by
+00001870: 2075 7369 6e67 2061 2073 6c75 726d 2d63   using a slurm-c
+00001880: 6f6e 6669 672e 696e 690a 2020 2020 616e  onfig.ini.    an
+00001890: 6420 7468 6520 6672 6f6d 5f63 6f6e 6669  d the from_confi
+000018a0: 6728 2920 6d65 7468 6f64 2e0a 0a20 2020  g() method...   
+000018b0: 2041 7474 7269 6275 7465 733a 0a20 2020   Attributes:.   
+000018c0: 2020 2020 2073 6c75 726d 5f64 6174 615f       slurm_data_
+000018d0: 7061 7468 2028 7374 7229 3a20 5468 6520  path (str): The 
+000018e0: 7061 7468 2074 6f20 7468 6520 6469 7265  path to the dire
+000018f0: 6374 6f72 7920 636f 6e74 6169 6e69 6e67  ctory containing
+00001900: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
+00001910: 2064 6174 6120 6669 6c65 7320 666f 7220   data files for 
+00001920: 536c 7572 6d20 6a6f 6273 2e0a 2020 2020  Slurm jobs..    
+00001930: 2020 2020 736c 7572 6d5f 696d 6167 6573      slurm_images
+00001940: 5f70 6174 6820 2873 7472 293a 2054 6865  _path (str): The
+00001950: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
+00001960: 6563 746f 7279 2063 6f6e 7461 696e 696e  ectory containin
+00001970: 670a 2020 2020 2020 2020 2020 2020 7468  g.            th
+00001980: 6520 5369 6e67 756c 6172 6974 7920 696d  e Singularity im
+00001990: 6167 6573 2066 6f72 2053 6c75 726d 206a  ages for Slurm j
+000019a0: 6f62 732e 0a20 2020 2020 2020 2073 6c75  obs..        slu
+000019b0: 726d 5f63 6f6e 7665 7274 6572 735f 7061  rm_converters_pa
+000019c0: 7468 2028 7374 7229 3a20 5468 6520 7061  th (str): The pa
+000019d0: 7468 2074 6f20 7468 6520 6469 7265 6374  th to the direct
+000019e0: 6f72 7920 636f 6e74 6169 6e69 6e67 0a20  ory containing. 
+000019f0: 2020 2020 2020 2020 2020 2074 6865 2053             the S
+00001a00: 696e 6775 6c61 7269 7479 2069 6d61 6765  ingularity image
+00001a10: 7320 666f 7220 6669 6c65 2063 6f6e 7665  s for file conve
+00001a20: 7274 6572 732e 0a20 2020 2020 2020 2073  rters..        s
+00001a30: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
+00001a40: 2028 6469 6374 293a 2041 2064 6963 7469   (dict): A dicti
+00001a50: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+00001a60: 2074 6865 2070 6174 6873 2074 6f0a 2020   the paths to.  
+00001a70: 2020 2020 2020 2020 2020 7468 6520 5369            the Si
+00001a80: 6e67 756c 6172 6974 7920 696d 6167 6573  ngularity images
+00001a90: 2066 6f72 2073 7065 6369 6669 6320 536c   for specific Sl
+00001aa0: 7572 6d20 6a6f 6220 6d6f 6465 6c73 2e0a  urm job models..
+00001ab0: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
+00001ac0: 6465 6c5f 7265 706f 7320 2864 6963 7429  del_repos (dict)
+00001ad0: 3a20 4120 6469 6374 696f 6e61 7279 2063  : A dictionary c
+00001ae0: 6f6e 7461 696e 696e 6720 7468 6520 6769  ontaining the gi
+00001af0: 740a 2020 2020 2020 2020 2020 2020 7265  t.            re
+00001b00: 706f 7369 746f 7269 6573 206f 6620 5369  positories of Si
+00001b10: 6e67 756c 6172 6974 7920 696d 6167 6573  ngularity images
+00001b20: 2066 6f72 2073 7065 6369 6669 6320 536c   for specific Sl
+00001b30: 7572 6d20 6a6f 6220 6d6f 6465 6c73 2e0a  urm job models..
+00001b40: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
+00001b50: 6465 6c5f 696d 6167 6573 2028 6469 6374  del_images (dict
+00001b60: 293a 2041 2064 6963 7469 6f6e 6172 7920  ): A dictionary 
+00001b70: 636f 6e74 6169 6e69 6e67 2074 6865 2064  containing the d
+00001b80: 6f63 6b65 7268 7562 0a20 2020 2020 2020  ockerhub.       
+00001b90: 2020 2020 206f 6620 7468 6520 5369 6e67       of the Sing
+00001ba0: 756c 6172 6974 7920 696d 6167 6573 2066  ularity images f
+00001bb0: 6f72 2073 7065 6369 6669 6320 536c 7572  or specific Slur
+00001bc0: 6d20 6a6f 6220 6d6f 6465 6c73 2e0a 2020  m job models..  
+00001bd0: 2020 2020 2020 2020 2020 5769 6c6c 2066            Will f
+00001be0: 696c 6c20 6175 746f 6d61 7469 6361 6c6c  ill automaticall
+00001bf0: 7920 6672 6f6d 2074 6865 2064 6174 6120  y from the data 
+00001c00: 696e 2074 6865 2067 6974 2072 6570 6f73  in the git repos
+00001c10: 6974 6f72 792c 0a20 2020 2020 2020 2020  itory,.         
+00001c20: 2020 2069 6620 796f 7520 7365 7420 696e     if you set in
+00001c30: 6974 5f73 6c75 726d 2e0a 2020 2020 2020  it_slurm..      
+00001c40: 2020 736c 7572 6d5f 7363 7269 7074 5f70    slurm_script_p
+00001c50: 6174 6820 2873 7472 293a 2054 6865 2070  ath (str): The p
+00001c60: 6174 6820 746f 2074 6865 2064 6972 6563  ath to the direc
+00001c70: 746f 7279 2063 6f6e 7461 696e 696e 670a  tory containing.
+00001c80: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00001c90: 536c 7572 6d20 6a6f 6220 7375 626d 6973  Slurm job submis
+00001ca0: 7369 6f6e 2073 6372 6970 7473 206f 6e20  sion scripts on 
+00001cb0: 536c 7572 6d2e 0a20 2020 2020 2020 2073  Slurm..        s
+00001cc0: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
+00001cd0: 2028 7374 7229 3a20 5468 6520 6769 7420   (str): The git 
+00001ce0: 6874 7470 7320 5552 4c20 666f 7220 636c  https URL for cl
+00001cf0: 6f6e 696e 6720 7468 6520 7265 706f 0a20  oning the repo. 
+00001d00: 2020 2020 2020 2020 2020 2063 6f6e 7461             conta
+00001d10: 696e 696e 6720 7468 6520 536c 7572 6d20  ining the Slurm 
+00001d20: 6a6f 6220 7375 626d 6973 7369 6f6e 2073  job submission s
+00001d30: 6372 6970 7473 2e20 4f70 7469 6f6e 616c  cripts. Optional
+00001d40: 2e0a 0a20 2020 2045 7861 6d70 6c65 3a0a  ...    Example:.
+00001d50: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+00001d60: 2061 2053 6c75 726d 436c 6965 6e74 206f   a SlurmClient o
+00001d70: 626a 6563 7420 6173 2063 6f6e 7465 7874  bject as context
+00001d80: 6d61 6e61 6765 720a 0a20 2020 2020 2020  manager..       
+00001d90: 2077 6974 6820 536c 7572 6d43 6c69 656e   with SlurmClien
+00001da0: 742e 6672 6f6d 5f63 6f6e 6669 6728 2920  t.from_config() 
+00001db0: 6173 2063 6c69 656e 743a 0a0a 2020 2020  as client:..    
+00001dc0: 2020 2020 2020 2020 2320 5275 6e20 6120          # Run a 
+00001dd0: 636f 6d6d 616e 6420 6f6e 2074 6865 2072  command on the r
+00001de0: 656d 6f74 6520 686f 7374 0a0a 2020 2020  emote host..    
+00001df0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00001e00: 2063 6c69 656e 742e 7275 6e28 2773 6261   client.run('sba
+00001e10: 7463 6820 6d79 6a6f 622e 7368 2729 0a0a  tch myjob.sh')..
+00001e20: 2020 2020 2020 2020 2020 2020 2320 4368              # Ch
+00001e30: 6563 6b20 7768 6574 6865 7220 7468 6520  eck whether the 
+00001e40: 636f 6d6d 616e 6420 7375 6363 6565 6465  command succeede
+00001e50: 640a 0a20 2020 2020 2020 2020 2020 2069  d..            i
+00001e60: 6620 7265 7375 6c74 2e6f 6b3a 0a20 2020  f result.ok:.   
+00001e70: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00001e80: 6e74 2827 4a6f 6220 7375 626d 6974 7465  nt('Job submitte
+00001e90: 6420 7375 6363 6573 7366 756c 6c79 2127  d successfully!'
+00001ea0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
+00001eb0: 2050 7269 6e74 2074 6865 206f 7574 7075   Print the outpu
+00001ec0: 7420 6f66 2074 6865 2063 6f6d 6d61 6e64  t of the command
+00001ed0: 0a0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00001ee0: 696e 7428 7265 7375 6c74 2e73 7464 6f75  int(result.stdou
+00001ef0: 7429 0a0a 2020 2020 4578 616d 706c 6520  t)..    Example 
+00001f00: 323a 0a20 2020 2020 2020 2023 2043 7265  2:.        # Cre
+00001f10: 6174 6520 6120 536c 7572 6d43 6c69 656e  ate a SlurmClien
+00001f20: 7420 616e 6420 7365 7475 7020 536c 7572  t and setup Slur
+00001f30: 6d20 2864 6f77 6e6c 6f61 6420 636f 6e74  m (download cont
+00001f40: 6169 6e65 7273 2065 7463 2e29 0a0a 2020  ainers etc.)..  
+00001f50: 2020 2020 2020 7769 7468 2053 6c75 726d        with Slurm
+00001f60: 436c 6965 6e74 2e66 726f 6d5f 636f 6e66  Client.from_conf
+00001f70: 6967 2869 6e69 745f 736c 7572 6d3d 5472  ig(init_slurm=Tr
+00001f80: 7565 2920 6173 2063 6c69 656e 743a 0a0a  ue) as client:..
+00001f90: 2020 2020 2020 2020 2020 2020 636c 6965              clie
+00001fa0: 6e74 2e72 756e 5f77 6f72 6b66 6c6f 7728  nt.run_workflow(
+00001fb0: 2e2e 2e29 0a0a 2020 2020 2222 220a 2020  ...)..    """.  
+00001fc0: 2020 5f44 4546 4155 4c54 5f43 4f4e 4649    _DEFAULT_CONFI
+00001fd0: 475f 5041 5448 5f31 203d 2022 2f65 7463  G_PATH_1 = "/etc
+00001fe0: 2f73 6c75 726d 2d63 6f6e 6669 672e 696e  /slurm-config.in
+00001ff0: 6922 0a20 2020 205f 4445 4641 554c 545f  i".    _DEFAULT_
+00002000: 434f 4e46 4947 5f50 4154 485f 3220 3d20  CONFIG_PATH_2 = 
+00002010: 227e 2f73 6c75 726d 2d63 6f6e 6669 672e  "~/slurm-config.
+00002020: 696e 6922 0a20 2020 205f 4445 4641 554c  ini".    _DEFAUL
+00002030: 545f 484f 5354 203d 2022 736c 7572 6d22  T_HOST = "slurm"
+00002040: 0a20 2020 205f 4445 4641 554c 545f 494e  .    _DEFAULT_IN
+00002050: 4c49 4e45 5f53 5348 5f45 4e56 203d 2054  LINE_SSH_ENV = T
+00002060: 7275 650a 2020 2020 5f44 4546 4155 4c54  rue.    _DEFAULT
+00002070: 5f53 4c55 524d 5f44 4154 415f 5041 5448  _SLURM_DATA_PATH
+00002080: 203d 2022 6d79 2d73 6372 6174 6368 2f64   = "my-scratch/d
+00002090: 6174 6122 0a20 2020 205f 4445 4641 554c  ata".    _DEFAUL
+000020a0: 545f 534c 5552 4d5f 494d 4147 4553 5f50  T_SLURM_IMAGES_P
+000020b0: 4154 4820 3d20 226d 792d 7363 7261 7463  ATH = "my-scratc
+000020c0: 682f 7369 6e67 756c 6172 6974 795f 696d  h/singularity_im
+000020d0: 6167 6573 2f77 6f72 6b66 6c6f 7773 220a  ages/workflows".
+000020e0: 2020 2020 5f44 4546 4155 4c54 5f53 4c55      _DEFAULT_SLU
+000020f0: 524d 5f43 4f4e 5645 5254 4552 535f 5041  RM_CONVERTERS_PA
+00002100: 5448 203d 2022 6d79 2d73 6372 6174 6368  TH = "my-scratch
+00002110: 2f73 696e 6775 6c61 7269 7479 5f69 6d61  /singularity_ima
+00002120: 6765 732f 636f 6e76 6572 7465 7273 220a  ges/converters".
+00002130: 2020 2020 5f44 4546 4155 4c54 5f53 4c55      _DEFAULT_SLU
+00002140: 524d 5f47 4954 5f53 4352 4950 545f 5041  RM_GIT_SCRIPT_PA
+00002150: 5448 203d 2022 736c 7572 6d2d 7363 7269  TH = "slurm-scri
+00002160: 7074 7322 0a20 2020 205f 4f55 545f 5345  pts".    _OUT_SE
+00002170: 5020 3d20 222d 2d73 706c 6974 2d2d 220a  P = "--split--".
+00002180: 2020 2020 5f56 4552 5349 4f4e 5f43 4d44      _VERSION_CMD
+00002190: 203d 2022 6c73 202d 6820 5c22 7b73 6c75   = "ls -h \"{slu
+000021a0: 726d 5f69 6d61 6765 735f 7061 7468 7d2f  rm_images_path}/
+000021b0: 7b69 6d61 6765 5f70 6174 687d 5c22 207c  {image_path}\" |
+000021c0: 2067 7265 7020 2d6f 5020 2728 3f3c 3d5c   grep -oP '(?<=\
+000021d0: 2d7c 5c5f 2928 762e 2b7c 6c61 7465 7374  -|\_)(v.+|latest
+000021e0: 2928 3f3d 2e73 696d 677c 2e73 6966 2927  )(?=.simg|.sif)'
+000021f0: 220a 2020 2020 2320 4e6f 7465 2c20 6772  ".    # Note, gr
+00002200: 6570 2072 6574 7572 6e73 2065 7869 7463  ep returns exitc
+00002210: 6f64 6520 3120 6966 206e 6f20 6d61 7463  ode 1 if no matc
+00002220: 6820 6973 2066 6f75 6e64 210a 2020 2020  h is found!.    
+00002230: 2320 5468 6973 2077 696c 6c20 7472 616e  # This will tran
+00002240: 736c 6174 6520 696e 746f 2061 2055 6e65  slate into a Une
+00002250: 7870 6563 7465 6445 7869 7420 6572 726f  xpectedExit erro
+00002260: 722c 2073 6f20 6d75 7465 2074 6861 7420  r, so mute that 
+00002270: 6966 2079 6f75 0a20 2020 2023 2064 6f6e  if you.    # don
+00002280: 2774 2063 6172 6520 6162 6f75 7420 656d  't care about em
+00002290: 7074 792e 0a20 2020 2023 204c 696b 6520  pty..    # Like 
+000022a0: 6265 6c6f 7720 7769 7468 2074 6865 2022  below with the "
+000022b0: 7c7c 203a 222e 0a20 2020 2023 2044 6174  || :"..    # Dat
+000022c0: 6120 636f 756c 6420 6c65 6769 7420 6265  a could legit be
+000022d0: 2065 6d70 7479 2e0a 2020 2020 5f44 4154   empty..    _DAT
+000022e0: 415f 434d 4420 3d20 226c 7320 2d68 205c  A_CMD = "ls -h \
+000022f0: 227b 736c 7572 6d5f 6461 7461 5f70 6174  "{slurm_data_pat
+00002300: 687d 5c22 207c 2067 7265 7020 2d6f 5020  h}\" | grep -oP 
+00002310: 272e 2b28 3f3d 2e7a 6970 2927 207c 7c20  '.+(?=.zip)' || 
+00002320: 3a22 0a20 2020 205f 414c 4c5f 4a4f 4253  :".    _ALL_JOBS
+00002330: 5f43 4d44 203d 2022 7361 6363 7420 2d2d  _CMD = "sacct --
+00002340: 7374 6172 7474 696d 6520 7b73 7461 7274  starttime {start
+00002350: 5f74 696d 657d 202d 2d65 6e64 7469 6d65  _time} --endtime
+00002360: 207b 656e 645f 7469 6d65 7d20 2d2d 7374   {end_time} --st
+00002370: 6174 6520 7b73 7461 7465 737d 202d 6f20  ate {states} -o 
+00002380: 7b63 6f6c 756d 6e73 7d20 2d6e 202d 5820  {columns} -n -X 
+00002390: 220a 2020 2020 5f5a 4950 5f43 4d44 203d  ".    _ZIP_CMD =
+000023a0: 2022 377a 2061 202d 7920 5c22 7b66 696c   "7z a -y \"{fil
+000023b0: 656e 616d 657d 5c22 202d 747a 6970 205c  ename}\" -tzip \
+000023c0: 227b 6461 7461 5f6c 6f63 6174 696f 6e7d  "{data_location}
+000023d0: 2f64 6174 612f 6f75 745c 2222 0a20 2020  /data/out\"".   
+000023e0: 205f 4143 5449 5645 5f4a 4f42 535f 434d   _ACTIVE_JOBS_CM
+000023f0: 4420 3d20 2273 7175 6575 6520 2d75 2024  D = "squeue -u $
+00002400: 5553 4552 202d 2d6e 6f68 6561 6420 2d2d  USER --nohead --
+00002410: 666f 726d 6174 2025 4622 0a20 2020 205f  format %F".    _
+00002420: 4a4f 425f 5354 4154 5553 5f43 4d44 203d  JOB_STATUS_CMD =
+00002430: 2022 7361 6363 7420 2d6e 202d 6f20 4a6f   "sacct -n -o Jo
+00002440: 6249 642c 5374 6174 652c 456e 6420 2d58  bId,State,End -X
+00002450: 202d 6a20 7b73 6c75 726d 5f6a 6f62 5f69   -j {slurm_job_i
+00002460: 647d 220a 2020 2020 2320 544f 444f 206d  d}".    # TODO m
+00002470: 6f76 6520 616c 6c20 636f 6d6d 616e 6473  ove all commands
+00002480: 2074 6f20 6120 7369 6d69 6c61 7220 666f   to a similar fo
+00002490: 726d 6174 2e0a 2020 2020 2320 5468 656e  rmat..    # Then
+000024a0: 206d 6179 6265 2061 6c6c 6f77 206f 7665   maybe allow ove
+000024b0: 7277 7269 7465 2066 726f 6d20 736c 7572  rwrite from slur
+000024c0: 6d2d 636f 6e66 6967 2e69 6e69 0a20 2020  m-config.ini.   
+000024d0: 205f 4c4f 4746 494c 4520 3d20 226f 6d65   _LOGFILE = "ome
+000024e0: 726f 2d7b 736c 7572 6d5f 6a6f 625f 6964  ro-{slurm_job_id
+000024f0: 7d2e 6c6f 6722 0a20 2020 205f 434f 4e56  }.log".    _CONV
+00002500: 4552 5445 525f 4c4f 4746 494c 4520 3d20  ERTER_LOGFILE = 
+00002510: 225c 2273 6c75 726d 2d7b 736c 7572 6d5f  "\"slurm-{slurm_
+00002520: 6a6f 625f 6964 7d5c 225f 2a2e 6f75 7422  job_id}\"_*.out"
+00002530: 0a20 2020 205f 5441 494c 5f4c 4f47 5f43  .    _TAIL_LOG_C
+00002540: 4d44 203d 2022 7461 696c 202d 6e20 7b6e  MD = "tail -n {n
+00002550: 7d20 5c22 7b6c 6f67 5f66 696c 657d 5c22  } \"{log_file}\"
+00002560: 207c 2073 7472 696e 6773 220a 2020 2020   | strings".    
+00002570: 5f4c 4f47 4649 4c45 5f44 4154 415f 434d  _LOGFILE_DATA_CM
+00002580: 4420 3d20 2263 6174 205c 227b 6c6f 675f  D = "cat \"{log_
+00002590: 6669 6c65 7d5c 2220 7c20 7065 726c 202d  file}\" | perl -
+000025a0: 776e 6520 272f 5275 6e6e 696e 6720 5b5c  wne '/Running [\
+000025b0: 772d 5d2b 3f20 4a6f 6220 775c 2f20 2e2b  w-]+? Job w\/ .+
+000025c0: 3f20 5c7c 202e 2b3f 205c 7c20 282e 2b3f  ? \| .+? \| (.+?
+000025d0: 2920 5c7c 2e2a 2f69 2061 6e64 2070 7269  ) \|.*/i and pri
+000025e0: 6e74 2431 2722 0a0a 2020 2020 6465 6620  nt$1'"..    def 
+000025f0: 5f5f 696e 6974 5f5f 2873 656c 662c 0a20  __init__(self,. 
+00002600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002610: 686f 7374 3d5f 4445 4641 554c 545f 484f  host=_DEFAULT_HO
+00002620: 5354 2c0a 2020 2020 2020 2020 2020 2020  ST,.            
+00002630: 2020 2020 2075 7365 723d 4e6f 6e65 2c0a       user=None,.
+00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002650: 2070 6f72 743d 4e6f 6e65 2c0a 2020 2020   port=None,.    
+00002660: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00002670: 6669 673d 4e6f 6e65 2c0a 2020 2020 2020  fig=None,.      
+00002680: 2020 2020 2020 2020 2020 2067 6174 6577             gatew
+00002690: 6179 3d4e 6f6e 652c 0a20 2020 2020 2020  ay=None,.       
+000026a0: 2020 2020 2020 2020 2020 666f 7277 6172            forwar
+000026b0: 645f 6167 656e 743d 4e6f 6e65 2c0a 2020  d_agent=None,.  
+000026c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000026d0: 6f6e 6e65 6374 5f74 696d 656f 7574 3d4e  onnect_timeout=N
+000026e0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+000026f0: 2020 2020 2020 636f 6e6e 6563 745f 6b77        connect_kw
+00002700: 6172 6773 3d4e 6f6e 652c 0a20 2020 2020  args=None,.     
+00002710: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
+00002720: 6e65 5f73 7368 5f65 6e76 3d5f 4445 4641  ne_ssh_env=_DEFA
+00002730: 554c 545f 494e 4c49 4e45 5f53 5348 5f45  ULT_INLINE_SSH_E
+00002740: 4e56 2c0a 2020 2020 2020 2020 2020 2020  NV,.            
+00002750: 2020 2020 2073 6c75 726d 5f64 6174 615f       slurm_data_
+00002760: 7061 7468 3a20 7374 7220 3d20 5f44 4546  path: str = _DEF
+00002770: 4155 4c54 5f53 4c55 524d 5f44 4154 415f  AULT_SLURM_DATA_
+00002780: 5041 5448 2c0a 2020 2020 2020 2020 2020  PATH,.          
+00002790: 2020 2020 2020 2073 6c75 726d 5f69 6d61         slurm_ima
+000027a0: 6765 735f 7061 7468 3a20 7374 7220 3d20  ges_path: str = 
+000027b0: 5f44 4546 4155 4c54 5f53 4c55 524d 5f49  _DEFAULT_SLURM_I
+000027c0: 4d41 4745 535f 5041 5448 2c0a 2020 2020  MAGES_PATH,.    
+000027d0: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
+000027e0: 726d 5f63 6f6e 7665 7274 6572 735f 7061  rm_converters_pa
+000027f0: 7468 3a20 7374 7220 3d20 5f44 4546 4155  th: str = _DEFAU
+00002800: 4c54 5f53 4c55 524d 5f43 4f4e 5645 5254  LT_SLURM_CONVERT
+00002810: 4552 535f 5041 5448 2c0a 2020 2020 2020  ERS_PATH,.      
+00002820: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+00002830: 5f6d 6f64 656c 5f70 6174 6873 3a20 6469  _model_paths: di
+00002840: 6374 203d 204e 6f6e 652c 0a20 2020 2020  ct = None,.     
+00002850: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+00002860: 6d5f 6d6f 6465 6c5f 7265 706f 733a 2064  m_model_repos: d
+00002870: 6963 7420 3d20 4e6f 6e65 2c0a 2020 2020  ict = None,.    
+00002880: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
+00002890: 726d 5f6d 6f64 656c 5f69 6d61 6765 733a  rm_model_images:
+000028a0: 2064 6963 7420 3d20 4e6f 6e65 2c0a 2020   dict = None,.  
+000028b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000028c0: 6c75 726d 5f6d 6f64 656c 5f6a 6f62 733a  lurm_model_jobs:
+000028d0: 2064 6963 7420 3d20 4e6f 6e65 2c0a 2020   dict = None,.  
+000028e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000028f0: 6c75 726d 5f6d 6f64 656c 5f6a 6f62 735f  lurm_model_jobs_
+00002900: 7061 7261 6d73 3a20 6469 6374 203d 204e  params: dict = N
+00002910: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
+00002920: 2020 2020 2020 736c 7572 6d5f 7363 7269        slurm_scri
+00002930: 7074 5f70 6174 683a 2073 7472 203d 205f  pt_path: str = _
+00002940: 4445 4641 554c 545f 534c 5552 4d5f 4749  DEFAULT_SLURM_GI
+00002950: 545f 5343 5249 5054 5f50 4154 482c 0a20  T_SCRIPT_PATH,. 
+00002960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002970: 736c 7572 6d5f 7363 7269 7074 5f72 6570  slurm_script_rep
+00002980: 6f3a 2073 7472 203d 204e 6f6e 652c 0a20  o: str = None,. 
+00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000029a0: 696e 6974 5f73 6c75 726d 3a20 626f 6f6c  init_slurm: bool
+000029b0: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
+000029c0: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
+000029d0: 2020 2020 2020 2222 2249 6e69 7469 616c        """Initial
+000029e0: 697a 6573 2061 206e 6577 2069 6e73 7461  izes a new insta
+000029f0: 6e63 6520 6f66 2074 6865 2053 6c75 726d  nce of the Slurm
+00002a00: 436c 6965 6e74 2063 6c61 7373 2e0a 0a20  Client class... 
+00002a10: 2020 2020 2020 2049 7420 6973 2070 7265         It is pre
+00002a20: 6665 7261 626c 6520 746f 2075 7365 2023  ferable to use #
+00002a30: 6672 6f6d 5f63 6f6e 6669 6728 2e2e 2e29  from_config(...)
+00002a40: 206d 6574 686f 6420 746f 2069 6e69 7469   method to initi
+00002a50: 616c 697a 650a 2020 2020 2020 2020 7061  alize.        pa
+00002a60: 7261 6d65 7465 7273 2066 726f 6d20 6120  rameters from a 
+00002a70: 636f 6e66 6967 2066 696c 652e 0a0a 2020  config file...  
+00002a80: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00002a90: 2020 2020 2020 2020 686f 7374 2028 7374          host (st
+00002aa0: 722c 206f 7074 696f 6e61 6c29 3a20 5468  r, optional): Th
+00002ab0: 6520 686f 7374 6e61 6d65 206f 7220 4950  e hostname or IP
+00002ac0: 2061 6464 7265 7373 206f 6620 7468 6520   address of the 
+00002ad0: 7265 6d6f 7465 0a20 2020 2020 2020 2020  remote.         
+00002ae0: 2020 2020 2020 2073 6572 7665 722e 2044         server. D
+00002af0: 6566 6175 6c74 7320 746f 205f 4445 4641  efaults to _DEFA
+00002b00: 554c 545f 484f 5354 2e0a 2020 2020 2020  ULT_HOST..      
+00002b10: 2020 2020 2020 7573 6572 2028 7374 722c        user (str,
+00002b20: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00002b30: 7573 6572 6e61 6d65 2074 6f20 7573 6520  username to use 
+00002b40: 7768 656e 2063 6f6e 6e65 6374 696e 6720  when connecting 
+00002b50: 746f 200a 2020 2020 2020 2020 2020 2020  to .            
+00002b60: 2020 2020 7468 6520 7265 6d6f 7465 2073      the remote s
+00002b70: 6572 7665 722e 2044 6566 6175 6c74 7320  erver. Defaults 
+00002b80: 746f 204e 6f6e 652c 2077 6869 6368 2064  to None, which d
+00002b90: 6566 6175 6c74 7320 0a20 2020 2020 2020  efaults .       
+00002ba0: 2020 2020 2020 2020 2074 6f20 636f 6e66           to conf
+00002bb0: 6967 2e75 7365 722e 0a20 2020 2020 2020  ig.user..       
+00002bc0: 2020 2020 2070 6f72 7420 2869 6e74 2c20       port (int, 
+00002bd0: 6f70 7469 6f6e 616c 293a 2054 6865 2053  optional): The S
+00002be0: 5348 2070 6f72 7420 746f 2075 7365 2077  SH port to use w
+00002bf0: 6865 6e20 636f 6e6e 6563 7469 6e67 2e0a  hen connecting..
+00002c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c10: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
+00002c20: 2c20 7768 6963 6820 6465 6661 756c 7473  , which defaults
+00002c30: 2074 6f20 636f 6e66 6967 2e70 6f72 742e   to config.port.
+00002c40: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00002c50: 6669 6720 2873 7472 2c20 6f70 7469 6f6e  fig (str, option
+00002c60: 616c 293a 2050 6174 6820 746f 2074 6865  al): Path to the
+00002c70: 2053 5348 2063 6f6e 6669 6720 6669 6c65   SSH config file
+00002c80: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00002c90: 2020 4465 6661 756c 7473 2074 6f20 4e6f    Defaults to No
+00002ca0: 6e65 2c20 7768 6963 6820 6465 6661 756c  ne, which defaul
+00002cb0: 7473 2074 6f20 796f 7572 2053 5348 2063  ts to your SSH c
+00002cc0: 6f6e 6669 6720 6669 6c65 2e0a 2020 2020  onfig file..    
+00002cd0: 2020 2020 2020 2020 6761 7465 7761 7920          gateway 
+00002ce0: 2843 6f6e 6e65 6374 696f 6e2c 206f 7074  (Connection, opt
+00002cf0: 696f 6e61 6c29 3a20 416e 206f 7074 696f  ional): An optio
+00002d00: 6e61 6c20 6761 7465 7761 7920 666f 7220  nal gateway for 
+00002d10: 636f 6e6e 6563 7469 6e67 200a 2020 2020  connecting .    
+00002d20: 2020 2020 2020 2020 2020 2020 7468 726f              thro
+00002d30: 7567 6820 6120 6a75 6d70 2068 6f73 742e  ugh a jump host.
+00002d40: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+00002d50: 652e 0a20 2020 2020 2020 2020 2020 2066  e..            f
+00002d60: 6f72 7761 7264 5f61 6765 6e74 2028 626f  orward_agent (bo
+00002d70: 6f6c 2c20 6f70 7469 6f6e 616c 293a 2057  ol, optional): W
+00002d80: 6865 7468 6572 2074 6f20 666f 7277 6172  hether to forwar
+00002d90: 6420 7468 6520 6c6f 6361 6c20 5353 4820  d the local SSH 
+00002da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002db0: 2061 6765 6e74 2074 6f20 7468 6520 7265   agent to the re
+00002dc0: 6d6f 7465 2073 6572 7665 722e 2044 6566  mote server. Def
+00002dd0: 6175 6c74 7320 746f 204e 6f6e 652c 2077  aults to None, w
+00002de0: 6869 6368 200a 2020 2020 2020 2020 2020  hich .          
+00002df0: 2020 2020 2020 6465 6661 756c 7473 2074        defaults t
+00002e00: 6f20 636f 6e66 6967 2e66 6f72 7761 7264  o config.forward
+00002e10: 5f61 6765 6e74 2e0a 2020 2020 2020 2020  _agent..        
+00002e20: 2020 2020 636f 6e6e 6563 745f 7469 6d65      connect_time
+00002e30: 6f75 7420 2869 6e74 2c20 6f70 7469 6f6e  out (int, option
+00002e40: 616c 293a 2054 696d 656f 7574 2066 6f72  al): Timeout for
+00002e50: 2065 7374 6162 6c69 7368 696e 6720 7468   establishing th
+00002e60: 6520 5353 4820 0a20 2020 2020 2020 2020  e SSH .         
+00002e70: 2020 2020 2020 2063 6f6e 6e65 6374 696f         connectio
+00002e80: 6e2e 2044 6566 6175 6c74 7320 746f 204e  n. Defaults to N
+00002e90: 6f6e 652c 2077 6869 6368 2064 6566 6175  one, which defau
+00002ea0: 6c74 7320 0a20 2020 2020 2020 2020 2020  lts .           
+00002eb0: 2020 2020 2074 6f20 636f 6e66 6967 2e74       to config.t
+00002ec0: 696d 656f 7574 732e 636f 6e6e 6563 742e  imeouts.connect.
+00002ed0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00002ee0: 6e65 6374 5f6b 7761 7267 7320 2864 6963  nect_kwargs (dic
+00002ef0: 742c 206f 7074 696f 6e61 6c29 3a20 4164  t, optional): Ad
+00002f00: 6469 7469 6f6e 616c 206b 6579 776f 7264  ditional keyword
+00002f10: 2061 7267 756d 656e 7473 2066 6f72 200a   arguments for .
+00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002f30: 7468 6520 756e 6465 726c 7969 6e67 2053  the underlying S
+00002f40: 5348 2063 6f6e 6e65 6374 696f 6e2e 2048  SH connection. H
+00002f50: 616e 6465 6420 7665 7262 6174 696d 2074  anded verbatim t
+00002f60: 6f20 0a20 2020 2020 2020 2020 2020 2020  o .             
+00002f70: 2020 2060 5353 4843 6c69 656e 742e 636f     `SSHClient.co
+00002f80: 6e6e 6563 7420 3c70 6172 616d 696b 6f2e  nnect <paramiko.
+00002f90: 636c 6965 6e74 2e53 5348 436c 6965 6e74  client.SSHClient
+00002fa0: 2e63 6f6e 6e65 6374 3e60 2e20 0a20 2020  .connect>`. .   
+00002fb0: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+00002fc0: 6175 6c74 7320 746f 204e 6f6e 652e 200a  aults to None. .
+00002fd0: 2020 2020 2020 2020 2020 2020 696e 6c69              inli
+00002fe0: 6e65 5f73 7368 5f65 6e76 2028 626f 6f6c  ne_ssh_env (bool
+00002ff0: 2c20 6f70 7469 6f6e 616c 293a 2057 6865  , optional): Whe
+00003000: 7468 6572 2074 6f20 7573 6520 696e 6c69  ther to use inli
+00003010: 6e65 2053 5348 0a20 2020 2020 2020 2020  ne SSH.         
+00003020: 2020 2020 2020 2065 6e76 6972 6f6e 6d65         environme
+00003030: 6e74 2e20 5468 6973 2069 7320 6e65 6365  nt. This is nece
+00003040: 7373 6172 7920 6966 2074 6865 2072 656d  ssary if the rem
+00003050: 6f74 6520 7365 7276 6572 2068 6173 200a  ote server has .
+00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003070: 6120 7265 7374 7269 6374 6564 2060 6041  a restricted ``A
+00003080: 6363 6570 7445 6e76 6060 2073 6574 7469  cceptEnv`` setti
+00003090: 6e67 2028 7768 6963 6820 6973 2074 6865  ng (which is the
+000030a0: 2063 6f6d 6d6f 6e20 0a20 2020 2020 2020   common .       
+000030b0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+000030c0: 292e 2044 6566 6175 6c74 7320 746f 205f  ). Defaults to _
+000030d0: 4445 4641 554c 545f 494e 4c49 4e45 5f53  DEFAULT_INLINE_S
+000030e0: 5348 5f45 4e56 2e0a 2020 2020 2020 2020  SH_ENV..        
+000030f0: 2020 2020 736c 7572 6d5f 6461 7461 5f70      slurm_data_p
+00003100: 6174 6820 2873 7472 2c20 6f70 7469 6f6e  ath (str, option
+00003110: 616c 293a 2054 6865 2070 6174 6820 746f  al): The path to
+00003120: 2074 6865 2064 6972 6563 746f 7279 0a20   the directory. 
+00003130: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00003140: 6f6e 7461 696e 696e 6720 7468 6520 6461  ontaining the da
+00003150: 7461 2066 696c 6573 2066 6f72 2053 6c75  ta files for Slu
+00003160: 726d 206a 6f62 732e 0a20 2020 2020 2020  rm jobs..       
+00003170: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+00003180: 7320 746f 205f 4445 4641 554c 545f 534c  s to _DEFAULT_SL
+00003190: 5552 4d5f 4441 5441 5f50 4154 482e 0a20  URM_DATA_PATH.. 
+000031a0: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+000031b0: 5f69 6d61 6765 735f 7061 7468 2028 7374  _images_path (st
+000031c0: 722c 206f 7074 696f 6e61 6c29 3a20 5468  r, optional): Th
+000031d0: 6520 7061 7468 2074 6f20 7468 6520 6469  e path to the di
+000031e0: 7265 6374 6f72 790a 2020 2020 2020 2020  rectory.        
+000031f0: 2020 2020 2020 2020 636f 6e74 6169 6e69          containi
+00003200: 6e67 2074 6865 2053 696e 6775 6c61 7269  ng the Singulari
+00003210: 7479 2069 6d61 6765 7320 666f 7220 536c  ty images for Sl
+00003220: 7572 6d20 6a6f 6273 2e0a 2020 2020 2020  urm jobs..      
+00003230: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00003240: 7473 2074 6f20 5f44 4546 4155 4c54 5f53  ts to _DEFAULT_S
+00003250: 4c55 524d 5f49 4d41 4745 535f 5041 5448  LURM_IMAGES_PATH
+00003260: 2e0a 2020 2020 2020 2020 2020 2020 736c  ..            sl
+00003270: 7572 6d5f 636f 6e76 6572 7465 7273 5f70  urm_converters_p
+00003280: 6174 6820 2873 7472 2c20 6f70 7469 6f6e  ath (str, option
+00003290: 616c 293a 2054 6865 2070 6174 6820 746f  al): The path to
+000032a0: 2074 6865 2064 6972 6563 746f 7279 0a20   the directory. 
+000032b0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+000032c0: 6f6e 7461 696e 696e 6720 7468 6520 5369  ontaining the Si
+000032d0: 6e67 756c 6172 6974 7920 696d 6167 6573  ngularity images
+000032e0: 2066 6f72 2066 696c 6520 636f 6e76 6572   for file conver
+000032f0: 7465 7273 2e0a 2020 2020 2020 2020 2020  ters..          
+00003300: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
+00003310: 6f20 5f44 4546 4155 4c54 5f53 4c55 524d  o _DEFAULT_SLURM
+00003320: 5f43 4f4e 5645 5254 4552 535f 5041 5448  _CONVERTERS_PATH
+00003330: 2e0a 2020 2020 2020 2020 2020 2020 736c  ..            sl
+00003340: 7572 6d5f 6d6f 6465 6c5f 7061 7468 7320  urm_model_paths 
+00003350: 2864 6963 742c 206f 7074 696f 6e61 6c29  (dict, optional)
+00003360: 3a20 4120 6469 6374 696f 6e61 7279 2063  : A dictionary c
+00003370: 6f6e 7461 696e 696e 6720 7468 6520 0a20  ontaining the . 
+00003380: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00003390: 6174 6873 2074 6f20 7468 6520 5369 6e67  aths to the Sing
+000033a0: 756c 6172 6974 7920 696d 6167 6573 2066  ularity images f
+000033b0: 6f72 2073 7065 6369 6669 6320 536c 7572  or specific Slur
+000033c0: 6d20 6a6f 6220 6d6f 6465 6c73 2e0a 2020  m job models..  
+000033d0: 2020 2020 2020 2020 2020 2020 2020 4465                De
+000033e0: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
+000033f0: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+00003400: 6d5f 6d6f 6465 6c5f 7265 706f 7320 2864  m_model_repos (d
+00003410: 6963 742c 206f 7074 696f 6e61 6c29 3a20  ict, optional): 
+00003420: 4120 6469 6374 696f 6e61 7279 2063 6f6e  A dictionary con
+00003430: 7461 696e 696e 6720 7468 6520 0a20 2020  taining the .   
+00003440: 2020 2020 2020 2020 2020 2020 2067 6974               git
+00003450: 2072 6570 6f73 6974 6f72 6965 7320 6f66   repositories of
+00003460: 2053 696e 6775 6c61 7269 7479 2069 6d61   Singularity ima
+00003470: 6765 7320 666f 7220 7370 6563 6966 6963  ges for specific
+00003480: 2053 6c75 726d 200a 2020 2020 2020 2020   Slurm .        
+00003490: 2020 2020 2020 2020 6a6f 6220 6d6f 6465          job mode
+000034a0: 6c73 2e0a 2020 2020 2020 2020 2020 2020  ls..            
+000034b0: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+000034c0: 4e6f 6e65 2e0a 2020 2020 2020 2020 2020  None..          
+000034d0: 2020 736c 7572 6d5f 6d6f 6465 6c5f 696d    slurm_model_im
+000034e0: 6167 6573 2028 6469 6374 2c20 6f70 7469  ages (dict, opti
+000034f0: 6f6e 616c 293a 2041 2064 6963 7469 6f6e  onal): A diction
+00003500: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
+00003510: 6865 200a 2020 2020 2020 2020 2020 2020  he .            
+00003520: 2020 2020 646f 636b 6572 6875 6220 6f66      dockerhub of
+00003530: 2074 6865 2053 696e 6775 6c61 7269 7479   the Singularity
+00003540: 2069 6d61 6765 7320 666f 7220 7370 6563   images for spec
+00003550: 6966 6963 2053 6c75 726d 200a 2020 2020  ific Slurm .    
+00003560: 2020 2020 2020 2020 2020 2020 6a6f 6220              job 
+00003570: 6d6f 6465 6c73 2e20 5769 6c6c 2066 696c  models. Will fil
+00003580: 6c20 6175 746f 6d61 7469 6361 6c6c 7920  l automatically 
+00003590: 6672 6f6d 2074 6865 2064 6174 6120 696e  from the data in
+000035a0: 2074 6865 2067 6974 200a 2020 2020 2020   the git .      
+000035b0: 2020 2020 2020 2020 2020 7265 706f 7369            reposi
+000035c0: 746f 7279 2069 6620 796f 7520 7365 7420  tory if you set 
+000035d0: 696e 6974 5f73 6c75 726d 2e0a 2020 2020  init_slurm..    
+000035e0: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+000035f0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
+00003600: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
+00003610: 6d6f 6465 6c5f 6a6f 6273 2028 6469 6374  model_jobs (dict
+00003620: 2c20 6f70 7469 6f6e 616c 293a 2041 2064  , optional): A d
+00003630: 6963 7469 6f6e 6172 7920 636f 6e74 6169  ictionary contai
+00003640: 6e69 6e67 0a20 2020 2020 2020 2020 2020  ning.           
+00003650: 2020 2020 2069 6e66 6f72 6d61 7469 6f6e       information
+00003660: 2061 626f 7574 2073 7065 6369 6669 6320   about specific 
+00003670: 536c 7572 6d20 6a6f 6220 6d6f 6465 6c73  Slurm job models
+00003680: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00003690: 2020 4465 6661 756c 7473 2074 6f20 4e6f    Defaults to No
+000036a0: 6e65 2e0a 2020 2020 2020 2020 2020 2020  ne..            
+000036b0: 736c 7572 6d5f 6d6f 6465 6c5f 6a6f 6273  slurm_model_jobs
+000036c0: 5f70 6172 616d 7320 2864 6963 742c 206f  _params (dict, o
+000036d0: 7074 696f 6e61 6c29 3a20 4120 6469 6374  ptional): A dict
+000036e0: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+000036f0: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
+00003700: 2020 7061 7261 6d65 7465 7273 2066 6f72    parameters for
+00003710: 2073 7065 6369 6669 6320 536c 7572 6d20   specific Slurm 
+00003720: 6a6f 6220 6d6f 6465 6c73 2e0a 2020 2020  job models..    
+00003730: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00003740: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
+00003750: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
+00003760: 7363 7269 7074 5f70 6174 6820 2873 7472  script_path (str
+00003770: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+00003780: 2070 6174 6820 746f 2074 6865 2064 6972   path to the dir
+00003790: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
+000037a0: 2020 2020 2020 2063 6f6e 7461 696e 696e         containin
+000037b0: 6720 7468 6520 536c 7572 6d20 6a6f 6220  g the Slurm job 
+000037c0: 7375 626d 6973 7369 6f6e 2073 6372 6970  submission scrip
+000037d0: 7473 206f 6e20 536c 7572 6d2e 0a20 2020  ts on Slurm..   
+000037e0: 2020 2020 2020 2020 2020 2020 2044 6566               Def
+000037f0: 6175 6c74 7320 746f 205f 4445 4641 554c  aults to _DEFAUL
+00003800: 545f 534c 5552 4d5f 4749 545f 5343 5249  T_SLURM_GIT_SCRI
+00003810: 5054 5f50 4154 482e 0a20 2020 2020 2020  PT_PATH..       
+00003820: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
+00003830: 745f 7265 706f 2028 7374 722c 206f 7074  t_repo (str, opt
+00003840: 696f 6e61 6c29 3a20 5468 6520 6769 7420  ional): The git 
+00003850: 6874 7470 7320 5552 4c20 666f 7220 636c  https URL for cl
+00003860: 6f6e 696e 670a 2020 2020 2020 2020 2020  oning.          
+00003870: 2020 2020 2020 7468 6520 7265 706f 2063        the repo c
+00003880: 6f6e 7461 696e 696e 6720 7468 6520 536c  ontaining the Sl
+00003890: 7572 6d20 6a6f 6220 7375 626d 6973 7369  urm job submissi
+000038a0: 6f6e 2073 6372 6970 7473 2e0a 2020 2020  on scripts..    
+000038b0: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+000038c0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 2020  ults to None..  
+000038d0: 2020 2020 2020 2020 2020 696e 6974 5f73            init_s
+000038e0: 6c75 726d 2028 626f 6f6c 293a 2057 6865  lurm (bool): Whe
+000038f0: 7468 6572 2074 6f20 7365 7420 7570 2074  ther to set up t
+00003900: 6865 2072 6571 7569 7265 6420 7374 7275  he required stru
+00003910: 6374 7572 6573 200a 2020 2020 2020 2020  ctures .        
+00003920: 2020 2020 2020 2020 6f6e 2053 6c75 726d          on Slurm
+00003930: 2061 6674 6572 2069 6e69 7469 6174 696e   after initiatin
+00003940: 6720 7468 6973 2063 6c69 656e 742e 2054  g this client. T
+00003950: 6869 7320 696e 636c 7564 6573 2063 7265  his includes cre
+00003960: 6174 696e 6720 0a20 2020 2020 2020 2020  ating .         
+00003970: 2020 2020 2020 206d 6973 7369 6e67 2066         missing f
+00003980: 6f6c 6465 7273 2c20 646f 776e 6c6f 6164  olders, download
+00003990: 696e 6720 636f 6e74 6169 6e65 7220 696d  ing container im
+000039a0: 6167 6573 2c20 636c 6f6e 696e 6720 6769  ages, cloning gi
+000039b0: 742c 6574 632e 0a20 2020 2020 2020 2020  t,etc..         
+000039c0: 2020 2020 2020 2054 6869 7320 7769 6c6c         This will
+000039d0: 2074 616b 6520 6120 7768 696c 6520 6174   take a while at
+000039e0: 2066 6972 7374 2062 7574 2077 696c 6c20   first but will 
+000039f0: 7661 6c69 6461 7465 2079 6f75 7220 7365  validate your se
+00003a00: 7475 702e 0a20 2020 2020 2020 2020 2020  tup..           
+00003a10: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+00003a20: 2046 616c 7365 2074 6f20 7361 7665 2074   False to save t
+00003a30: 696d 652e 0a20 2020 2020 2020 2022 2222  ime..        """
+00003a40: 0a20 2020 2020 2020 2073 7570 6572 2853  .        super(S
+00003a50: 6c75 726d 436c 6965 6e74 2c20 7365 6c66  lurmClient, self
+00003a60: 292e 5f5f 696e 6974 5f5f 2868 6f73 742c  ).__init__(host,
+00003a70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a90: 2020 2020 2020 2020 2020 2075 7365 722c             user,
+00003aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ac0: 2020 2020 2020 2020 2020 2070 6f72 742c             port,
+00003ad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003af0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00003b00: 672c 0a20 2020 2020 2020 2020 2020 2020  g,.             
+00003b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b20: 2020 2020 2020 2020 2020 2020 2067 6174               gat
+00003b30: 6577 6179 2c0a 2020 2020 2020 2020 2020  eway,.          
+00003b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b60: 666f 7277 6172 645f 6167 656e 742c 0a20  forward_agent,. 
+00003b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b90: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
+00003ba0: 5f74 696d 656f 7574 2c0a 2020 2020 2020  _timeout,.      
+00003bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003bd0: 2020 2020 636f 6e6e 6563 745f 6b77 6172      connect_kwar
+00003be0: 6773 2c0a 2020 2020 2020 2020 2020 2020  gs,.            
+00003bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003c00: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00003c10: 6c69 6e65 5f73 7368 5f65 6e76 290a 2020  line_ssh_env).  
+00003c20: 2020 2020 2020 7365 6c66 2e73 6c75 726d        self.slurm
+00003c30: 5f64 6174 615f 7061 7468 203d 2073 6c75  _data_path = slu
+00003c40: 726d 5f64 6174 615f 7061 7468 0a20 2020  rm_data_path.   
+00003c50: 2020 2020 2073 656c 662e 736c 7572 6d5f       self.slurm_
+00003c60: 696d 6167 6573 5f70 6174 6820 3d20 736c  images_path = sl
+00003c70: 7572 6d5f 696d 6167 6573 5f70 6174 680a  urm_images_path.
+00003c80: 2020 2020 2020 2020 7365 6c66 2e73 6c75          self.slu
+00003c90: 726d 5f63 6f6e 7665 7274 6572 735f 7061  rm_converters_pa
+00003ca0: 7468 203d 2073 6c75 726d 5f63 6f6e 7665  th = slurm_conve
+00003cb0: 7274 6572 735f 7061 7468 0a20 2020 2020  rters_path.     
+00003cc0: 2020 2073 656c 662e 736c 7572 6d5f 6d6f     self.slurm_mo
+00003cd0: 6465 6c5f 7061 7468 7320 3d20 736c 7572  del_paths = slur
+00003ce0: 6d5f 6d6f 6465 6c5f 7061 7468 730a 2020  m_model_paths.  
+00003cf0: 2020 2020 2020 7365 6c66 2e73 6c75 726d        self.slurm
+00003d00: 5f73 6372 6970 745f 7061 7468 203d 2073  _script_path = s
+00003d10: 6c75 726d 5f73 6372 6970 745f 7061 7468  lurm_script_path
+00003d20: 0a20 2020 2020 2020 2073 656c 662e 736c  .        self.sl
+00003d30: 7572 6d5f 7363 7269 7074 5f72 6570 6f20  urm_script_repo 
+00003d40: 3d20 736c 7572 6d5f 7363 7269 7074 5f72  = slurm_script_r
+00003d50: 6570 6f0a 2020 2020 2020 2020 7365 6c66  epo.        self
+00003d60: 2e73 6c75 726d 5f6d 6f64 656c 5f72 6570  .slurm_model_rep
+00003d70: 6f73 203d 2073 6c75 726d 5f6d 6f64 656c  os = slurm_model
+00003d80: 5f72 6570 6f73 0a20 2020 2020 2020 2073  _repos.        s
+00003d90: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
+00003da0: 696d 6167 6573 203d 2073 6c75 726d 5f6d  images = slurm_m
+00003db0: 6f64 656c 5f69 6d61 6765 730a 2020 2020  odel_images.    
+00003dc0: 2020 2020 7365 6c66 2e73 6c75 726d 5f6d      self.slurm_m
+00003dd0: 6f64 656c 5f6a 6f62 7320 3d20 736c 7572  odel_jobs = slur
+00003de0: 6d5f 6d6f 6465 6c5f 6a6f 6273 0a20 2020  m_model_jobs.   
+00003df0: 2020 2020 2073 656c 662e 736c 7572 6d5f       self.slurm_
+00003e00: 6d6f 6465 6c5f 6a6f 6273 5f70 6172 616d  model_jobs_param
+00003e10: 7320 3d20 736c 7572 6d5f 6d6f 6465 6c5f  s = slurm_model_
+00003e20: 6a6f 6273 5f70 6172 616d 730a 0a20 2020  jobs_params..   
+00003e30: 2020 2020 2023 2049 6e69 7420 6361 6368       # Init cach
+00003e40: 652e 204b 6565 7020 7265 7370 6f6e 7365  e. Keep response
+00003e50: 7320 666f 7220 3336 3020 7365 636f 6e64  s for 360 second
+00003e60: 730a 2020 2020 2020 2020 7365 6c66 2e63  s.        self.c
+00003e70: 6163 6865 203d 2072 6571 7565 7374 735f  ache = requests_
+00003e80: 6361 6368 652e 6261 636b 656e 6473 2e73  cache.backends.s
+00003e90: 716c 6974 652e 5351 4c69 7465 4361 6368  qlite.SQLiteCach
+00003ea0: 6528 0a20 2020 2020 2020 2020 2020 2064  e(.            d
+00003eb0: 625f 7061 7468 3d22 6769 7468 7562 5f63  b_path="github_c
+00003ec0: 6163 6865 222c 2075 7365 5f74 656d 703d  ache", use_temp=
+00003ed0: 5472 7565 290a 2020 2020 2020 2020 7365  True).        se
+00003ee0: 6c66 2e67 6574 5f6f 725f 6372 6561 7465  lf.get_or_create
+00003ef0: 5f67 6974 6875 625f 7365 7373 696f 6e28  _github_session(
+00003f00: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00003f10: 696e 6974 5f77 6f72 6b66 6c6f 7773 2829  init_workflows()
+00003f20: 0a20 2020 2020 2020 2073 656c 662e 7661  .        self.va
+00003f30: 6c69 6461 7465 2876 616c 6964 6174 655f  lidate(validate_
+00003f40: 736c 7572 6d5f 7365 7475 703d 696e 6974  slurm_setup=init
+00003f50: 5f73 6c75 726d 290a 0a20 2020 2064 6566  _slurm)..    def
+00003f60: 2069 6e69 745f 776f 726b 666c 6f77 7328   init_workflows(
+00003f70: 7365 6c66 2c20 666f 7263 655f 7570 6461  self, force_upda
+00003f80: 7465 3a20 626f 6f6c 203d 2046 616c 7365  te: bool = False
+00003f90: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00003fa0: 2020 2020 2020 2052 6574 7269 6576 6573         Retrieves
+00003fb0: 2074 6865 2072 6571 7569 7265 6420 696e   the required in
+00003fc0: 666f 2066 6f72 2074 6865 2063 6f6e 6669  fo for the confi
+00003fd0: 6775 7265 6420 776f 726b 666c 6f77 7320  gured workflows 
+00003fe0: 6672 6f6d 2067 6974 6875 622e 0a20 2020  from github..   
+00003ff0: 2020 2020 2049 7420 7769 6c6c 2066 696c       It will fil
+00004000: 6c20 6073 6c75 726d 5f6d 6f64 656c 5f69  l `slurm_model_i
+00004010: 6d61 6765 7360 2077 6974 6820 646f 636b  mages` with dock
+00004020: 6572 6875 6220 6c69 6e6b 732e 0a0a 2020  erhub links...  
+00004030: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00004040: 2020 2020 2020 2020 666f 7263 655f 7570          force_up
+00004050: 6461 7465 2028 626f 6f6c 293a 2057 696c  date (bool): Wil
+00004060: 6c20 6f76 6572 7772 6974 6520 616c 7265  l overwrite alre
+00004070: 6164 7920 6769 7665 6e20 7061 7468 730a  ady given paths.
+00004080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004090: 696e 2060 736c 7572 6d5f 6d6f 6465 6c5f  in `slurm_model_
+000040a0: 696d 6167 6573 600a 0a20 2020 2020 2020  images`..       
+000040b0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+000040c0: 6e6f 7420 7365 6c66 2e73 6c75 726d 5f6d  not self.slurm_m
+000040d0: 6f64 656c 5f69 6d61 6765 733a 0a20 2020  odel_images:.   
+000040e0: 2020 2020 2020 2020 2073 656c 662e 736c           self.sl
+000040f0: 7572 6d5f 6d6f 6465 6c5f 696d 6167 6573  urm_model_images
+00004100: 203d 207b 7d0a 2020 2020 2020 2020 6966   = {}.        if
+00004110: 206e 6f74 2073 656c 662e 736c 7572 6d5f   not self.slurm_
+00004120: 6d6f 6465 6c5f 7265 706f 733a 0a20 2020  model_repos:.   
+00004130: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00004140: 7761 726e 696e 6728 224e 6f20 776f 726b  warning("No work
+00004150: 666c 6f77 7320 636f 6e66 6967 7572 6564  flows configured
+00004160: 2122 290a 2020 2020 2020 2020 2020 2020  !").            
+00004170: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+00004180: 5f72 6570 6f73 203d 207b 7d0a 2020 2020  _repos = {}.    
+00004190: 2020 2020 2020 2020 2320 736b 6970 7320          # skips 
+000041a0: 7468 6520 7365 7475 700a 2020 2020 2020  the setup.      
+000041b0: 2020 666f 7220 776f 726b 666c 6f77 2069    for workflow i
+000041c0: 6e20 7365 6c66 2e73 6c75 726d 5f6d 6f64  n self.slurm_mod
+000041d0: 656c 5f72 6570 6f73 2e6b 6579 7328 293a  el_repos.keys():
+000041e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000041f0: 776f 726b 666c 6f77 206e 6f74 2069 6e20  workflow not in 
+00004200: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+00004210: 5f69 6d61 6765 7320 6f72 2066 6f72 6365  _images or force
+00004220: 5f75 7064 6174 653a 0a20 2020 2020 2020  _update:.       
+00004230: 2020 2020 2020 2020 206a 736f 6e5f 6465           json_de
+00004240: 7363 7269 7074 6f72 203d 2073 656c 662e  scriptor = self.
+00004250: 7075 6c6c 5f64 6573 6372 6970 746f 725f  pull_descriptor_
+00004260: 6672 6f6d 5f67 6974 6875 6228 776f 726b  from_github(work
+00004270: 666c 6f77 290a 2020 2020 2020 2020 2020  flow).          
+00004280: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+00004290: 7567 2827 2573 3a20 2573 272c 2077 6f72  ug('%s: %s', wor
+000042a0: 6b66 6c6f 772c 206a 736f 6e5f 6465 7363  kflow, json_desc
+000042b0: 7269 7074 6f72 290a 2020 2020 2020 2020  riptor).        
+000042c0: 2020 2020 2020 2020 696d 6167 6520 3d20          image = 
+000042d0: 6a73 6f6e 5f64 6573 6372 6970 746f 725b  json_descriptor[
+000042e0: 2763 6f6e 7461 696e 6572 2d69 6d61 6765  'container-image
+000042f0: 275d 5b27 696d 6167 6527 5d0a 2020 2020  ']['image'].    
+00004300: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004310: 2e73 6c75 726d 5f6d 6f64 656c 5f69 6d61  .slurm_model_ima
+00004320: 6765 735b 776f 726b 666c 6f77 5d20 3d20  ges[workflow] = 
+00004330: 696d 6167 650a 0a20 2020 2064 6566 2073  image..    def s
+00004340: 6574 7570 5f73 6c75 726d 2873 656c 6629  etup_slurm(self)
+00004350: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00004360: 2020 2020 2020 5661 6c69 6461 7465 7320        Validates 
+00004370: 6f72 2063 7265 6174 6573 2074 6865 2072  or creates the r
+00004380: 6571 7569 7265 6420 7365 7475 7020 6f6e  equired setup on
+00004390: 2074 6865 2053 6c75 726d 2063 6c75 7374   the Slurm clust
+000043a0: 6572 2e0a 0a20 2020 2020 2020 2052 6169  er...        Rai
+000043b0: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+000043c0: 2053 5348 4578 6365 7074 696f 6e3a 2069   SSHException: i
+000043d0: 6620 6974 2063 616e 6e6f 7420 636f 6e6e  f it cannot conn
+000043e0: 6563 7420 746f 2053 6c75 726d 2c20 6f72  ect to Slurm, or
+000043f0: 2072 756e 7320 696e 746f 2061 6e20 6572   runs into an er
+00004400: 726f 720a 2020 2020 2020 2020 2222 220a  ror.        """.
+00004410: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00004420: 7661 6c69 6461 7465 2829 3a0a 2020 2020  validate():.    
+00004430: 2020 2020 2020 2020 2320 312e 2043 7265          # 1. Cre
+00004440: 6174 6520 6469 7265 6374 6f72 6965 730a  ate directories.
+00004450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00004460: 2e73 6574 7570 5f64 6972 6563 746f 7269  .setup_directori
+00004470: 6573 2829 0a0a 2020 2020 2020 2020 2020  es()..          
+00004480: 2020 2320 322e 2043 6c6f 6e65 2067 6974    # 2. Clone git
+00004490: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000044a0: 662e 7365 7475 705f 6a6f 625f 7363 7269  f.setup_job_scri
+000044b0: 7074 7328 290a 0a20 2020 2020 2020 2020  pts()..         
+000044c0: 2020 2023 2033 2e20 5365 7475 7020 636f     # 3. Setup co
+000044d0: 6e76 6572 7465 7273 0a20 2020 2020 2020  nverters.       
+000044e0: 2020 2020 2073 656c 662e 7365 7475 705f       self.setup_
+000044f0: 636f 6e76 6572 7465 7273 2829 0a0a 2020  converters()..  
+00004500: 2020 2020 2020 2020 2020 2320 342e 2044            # 4. D
+00004510: 6f77 6e6c 6f61 6420 776f 726b 666c 6f77  ownload workflow
+00004520: 2069 6d61 6765 730a 2020 2020 2020 2020   images.        
+00004530: 2020 2020 7365 6c66 2e73 6574 7570 5f63      self.setup_c
+00004540: 6f6e 7461 696e 6572 5f69 6d61 6765 7328  ontainer_images(
+00004550: 290a 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+00004560: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00004570: 7365 2053 5348 4578 6365 7074 696f 6e28  se SSHException(
+00004580: 2246 6169 6c75 7265 2069 6e20 636f 6e6e  "Failure in conn
+00004590: 6563 7469 6e67 2074 6f20 536c 7572 6d20  ecting to Slurm 
+000045a0: 636c 7573 7465 7222 290a 0a20 2020 2064  cluster")..    d
+000045b0: 6566 2073 6574 7570 5f63 6f6e 7461 696e  ef setup_contain
+000045c0: 6572 5f69 6d61 6765 7328 7365 6c66 293a  er_images(self):
+000045d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000045e0: 2020 2020 2053 6574 7320 7570 2063 6f6e       Sets up con
+000045f0: 7461 696e 6572 2069 6d61 6765 7320 666f  tainer images fo
+00004600: 7220 536c 7572 6d20 6f70 6572 6174 696f  r Slurm operatio
+00004610: 6e73 2e0a 0a20 2020 2020 2020 2054 6869  ns...        Thi
+00004620: 7320 6675 6e63 7469 6f6e 2063 7265 6174  s function creat
+00004630: 6573 2073 7065 6369 6669 6320 6469 7265  es specific dire
+00004640: 6374 6f72 6965 7320 666f 7220 636f 6e74  ctories for cont
+00004650: 6169 6e65 7220 696d 6167 6573 2061 6e64  ainer images and
+00004660: 2070 756c 6c73 0a20 2020 2020 2020 206e   pulls.        n
+00004670: 6563 6573 7361 7279 2069 6d61 6765 7320  ecessary images 
+00004680: 6672 6f6d 2044 6f63 6b65 7220 7265 706f  from Docker repo
+00004690: 7369 746f 7269 6573 2e20 4974 2067 656e  sitories. It gen
+000046a0: 6572 6174 6573 2061 6e64 2065 7865 6375  erates and execu
+000046b0: 7465 730a 2020 2020 2020 2020 6120 7363  tes.        a sc
+000046c0: 7269 7074 2074 6f20 7075 6c6c 2069 6d61  ript to pull ima
+000046d0: 6765 7320 616e 6420 636f 7069 6573 2069  ges and copies i
+000046e0: 7420 746f 2074 6865 2072 656d 6f74 6520  t to the remote 
+000046f0: 6c6f 6361 7469 6f6e 2e0a 0a20 2020 2020  location...     
+00004700: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+00004710: 2020 2020 2020 2053 5348 4578 6365 7074         SSHExcept
+00004720: 696f 6e3a 2049 6620 7468 6572 6520 6973  ion: If there is
+00004730: 2061 6e20 6973 7375 6520 6578 6563 7574   an issue execut
+00004740: 696e 6720 636f 6d6d 616e 6473 206f 7220  ing commands or 
+00004750: 636f 7079 696e 6720 6669 6c65 732e 0a20  copying files.. 
+00004760: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00004770: 2020 2023 2043 7265 6174 6520 7370 6563     # Create spec
+00004780: 6966 6963 2077 6f72 6b66 6c6f 7720 6469  ific workflow di
+00004790: 7273 0a20 2020 2020 2020 2077 6974 6820  rs.        with 
+000047a0: 7365 6c66 2e63 6428 7365 6c66 2e73 6c75  self.cd(self.slu
+000047b0: 726d 5f69 6d61 6765 735f 7061 7468 293a  rm_images_path):
+000047c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000047d0: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+000047e0: 5f70 6174 6873 3a0a 2020 2020 2020 2020  _paths:.        
+000047f0: 2020 2020 2020 2020 6d6f 6465 6c70 6174          modelpat
+00004800: 6873 203d 2022 2022 2e6a 6f69 6e28 7365  hs = " ".join(se
+00004810: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f70  lf.slurm_model_p
+00004820: 6174 6873 2e76 616c 7565 7328 2929 0a20  aths.values()). 
+00004830: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00004840: 206d 6b64 6972 2063 656c 6c70 726f 6669   mkdir cellprofi
+00004850: 6c65 7220 696d 6167 656a 202e 2e2e 0a20  ler imagej .... 
+00004860: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004870: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
+00004880: 616e 6473 285b 6622 6d6b 6469 7220 2d70  ands([f"mkdir -p
+00004890: 205c 227b 6d6f 6465 6c70 6174 6873 7d5c   \"{modelpaths}\
+000048a0: 2222 5d29 0a20 2020 2020 2020 2020 2020  ""]).           
+000048b0: 2020 2020 2069 6620 6e6f 7420 722e 6f6b       if not r.ok
+000048c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000048d0: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
+000048e0: 7863 6570 7469 6f6e 2872 290a 0a20 2020  xception(r)..   
+000048f0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00004900: 2e73 6c75 726d 5f6d 6f64 656c 5f69 6d61  .slurm_model_ima
+00004910: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
+00004920: 2020 2020 2070 756c 6c5f 636f 6d6d 616e       pull_comman
+00004930: 6473 203d 205b 5d0a 2020 2020 2020 2020  ds = [].        
+00004940: 2020 2020 2020 2020 666f 7220 7766 2c20          for wf, 
+00004950: 696d 6167 6520 696e 2073 656c 662e 736c  image in self.sl
+00004960: 7572 6d5f 6d6f 6465 6c5f 696d 6167 6573  urm_model_images
+00004970: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00004980: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00004990: 706f 203d 2073 656c 662e 736c 7572 6d5f  po = self.slurm_
+000049a0: 6d6f 6465 6c5f 7265 706f 735b 7766 5d0a  model_repos[wf].
+000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049c0: 2020 2020 7061 7468 203d 2073 656c 662e      path = self.
+000049d0: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
+000049e0: 735b 7766 5d0a 2020 2020 2020 2020 2020  s[wf].          
+000049f0: 2020 2020 2020 2020 2020 5f2c 2076 6572            _, ver
+00004a00: 7369 6f6e 203d 2073 656c 662e 6578 7472  sion = self.extr
+00004a10: 6163 745f 7061 7274 735f 6672 6f6d 5f75  act_parts_from_u
+00004a20: 726c 2872 6570 6f29 0a20 2020 2020 2020  rl(repo).       
+00004a30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00004a40: 7665 7273 696f 6e20 3d3d 2022 6d61 7374  version == "mast
+00004a50: 6572 223a 0a20 2020 2020 2020 2020 2020  er":.           
+00004a60: 2020 2020 2020 2020 2020 2020 2076 6572               ver
+00004a70: 7369 6f6e 203d 2022 6c61 7465 7374 220a  sion = "latest".
+00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a90: 2020 2020 7075 6c6c 5f74 656d 706c 6174      pull_templat
+00004aa0: 6520 3d20 2265 6368 6f20 2773 7461 7274  e = "echo 'start
+00004ab0: 696e 6720 2470 6174 6820 2476 6572 7369  ing $path $versi
+00004ac0: 6f6e 2720 3e3e 2073 696e 672e 6c6f 675c  on' >> sing.log\
+00004ad0: 6e6e 6f68 7570 2073 6820 2d63 205c 2273  nnohup sh -c \"s
+00004ae0: 696e 6775 6c61 7269 7479 2070 756c 6c20  ingularity pull 
+00004af0: 2d2d 6469 7361 626c 652d 6361 6368 6520  --disable-cache 
+00004b00: 2d2d 6469 7220 2470 6174 6820 646f 636b  --dir $path dock
+00004b10: 6572 3a2f 2f24 696d 6167 653a 2476 6572  er://$image:$ver
+00004b20: 7369 6f6e 3b20 6563 686f 2027 6669 6e69  sion; echo 'fini
+00004b30: 7368 6564 2024 7061 7468 2024 7665 7273  shed $path $vers
+00004b40: 696f 6e27 5c22 203e 3e20 7369 6e67 2e6c  ion'\" >> sing.l
+00004b50: 6f67 2032 3e26 3120 2620 6469 736f 776e  og 2>&1 & disown
+00004b60: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00004b70: 2020 2020 2020 7420 3d20 5465 6d70 6c61        t = Templa
+00004b80: 7465 2870 756c 6c5f 7465 6d70 6c61 7465  te(pull_template
+00004b90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00004ba0: 2020 2020 2020 7375 6273 7469 7475 7465        substitute
+00004bb0: 7320 3d20 7b7d 0a20 2020 2020 2020 2020  s = {}.         
+00004bc0: 2020 2020 2020 2020 2020 2073 7562 7374             subst
+00004bd0: 6974 7574 6573 5b27 7061 7468 275d 203d  itutes['path'] =
+00004be0: 2070 6174 680a 2020 2020 2020 2020 2020   path.          
+00004bf0: 2020 2020 2020 2020 2020 7375 6273 7469            substi
+00004c00: 7475 7465 735b 2769 6d61 6765 275d 203d  tutes['image'] =
+00004c10: 2069 6d61 6765 0a20 2020 2020 2020 2020   image.         
+00004c20: 2020 2020 2020 2020 2020 2073 7562 7374             subst
+00004c30: 6974 7574 6573 5b27 7665 7273 696f 6e27  itutes['version'
+00004c40: 5d20 3d20 7665 7273 696f 6e0a 2020 2020  ] = version.    
+00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004c60: 636d 6420 3d20 742e 7361 6665 5f73 7562  cmd = t.safe_sub
+00004c70: 7374 6974 7574 6528 7375 6273 7469 7475  stitute(substitu
+00004c80: 7465 7329 0a20 2020 2020 2020 2020 2020  tes).           
+00004c90: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00004ca0: 6465 6275 6728 6622 7375 6273 7469 7475  debug(f"substitu
+00004cb0: 7465 643a 207b 636d 647d 2229 0a20 2020  ted: {cmd}").   
+00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004cd0: 2070 756c 6c5f 636f 6d6d 616e 6473 2e61   pull_commands.a
+00004ce0: 7070 656e 6428 636d 6429 0a20 2020 2020  ppend(cmd).     
+00004cf0: 2020 2020 2020 2020 2020 2073 6372 6970             scrip
+00004d00: 745f 6e61 6d65 203d 2022 7075 6c6c 5f69  t_name = "pull_i
+00004d10: 6d61 6765 732e 7368 220a 2020 2020 2020  mages.sh".      
+00004d20: 2020 2020 2020 2020 2020 7465 6d70 6c61            templa
+00004d30: 7465 5f73 6372 6970 7420 3d20 6669 6c65  te_script = file
+00004d40: 7328 2272 6573 6f75 7263 6573 2229 2e6a  s("resources").j
+00004d50: 6f69 6e70 6174 6828 7363 7269 7074 5f6e  oinpath(script_n
+00004d60: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+00004d70: 2020 2020 2077 6974 6820 7465 6d70 6c61       with templa
+00004d80: 7465 5f73 6372 6970 742e 6f70 656e 2827  te_script.open('
+00004d90: 7227 2920 6173 2066 3a0a 2020 2020 2020  r') as f:.      
+00004da0: 2020 2020 2020 2020 2020 2020 2020 7372                sr
+00004db0: 6320 3d20 5465 6d70 6c61 7465 2866 2e72  c = Template(f.r
+00004dc0: 6561 6428 2929 0a20 2020 2020 2020 2020  ead()).         
+00004dd0: 2020 2020 2020 2020 2020 2073 7562 7374             subst
+00004de0: 6974 7574 6520 3d20 7b27 7075 6c6c 636f  itute = {'pullco
+00004df0: 6d6d 616e 6473 273a 2022 5c6e 222e 6a6f  mmands': "\n".jo
+00004e00: 696e 2870 756c 6c5f 636f 6d6d 616e 6473  in(pull_commands
+00004e10: 297d 0a20 2020 2020 2020 2020 2020 2020  )}.             
+00004e20: 2020 2020 2020 206a 6f62 5f73 6372 6970         job_scrip
+00004e30: 7420 3d20 7372 632e 7361 6665 5f73 7562  t = src.safe_sub
+00004e40: 7374 6974 7574 6528 7375 6273 7469 7475  stitute(substitu
+00004e50: 7465 290a 2020 2020 2020 2020 2020 2020  te).            
+00004e60: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+00004e70: 2866 2273 7562 7374 6974 7574 6564 3a5c  (f"substituted:\
+00004e80: 6e20 7b6a 6f62 5f73 6372 6970 747d 2229  n {job_script}")
+00004e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004ea0: 2023 2063 6f70 7920 746f 2072 656d 6f74   # copy to remot
+00004eb0: 6520 6669 6c65 0a20 2020 2020 2020 2020  e file.         
+00004ec0: 2020 2020 2020 2066 756c 6c5f 7061 7468         full_path
+00004ed0: 203d 2073 656c 662e 736c 7572 6d5f 696d   = self.slurm_im
+00004ee0: 6167 6573 5f70 6174 682b 222f 222b 7363  ages_path+"/"+sc
+00004ef0: 7269 7074 5f6e 616d 650a 2020 2020 2020  ript_name.      
+00004f00: 2020 2020 2020 2020 2020 5f20 3d20 7365            _ = se
+00004f10: 6c66 2e70 7574 286c 6f63 616c 3d69 6f2e  lf.put(local=io.
+00004f20: 5374 7269 6e67 494f 286a 6f62 5f73 6372  StringIO(job_scr
+00004f30: 6970 7429 2c0a 2020 2020 2020 2020 2020  ipt),.          
+00004f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f50: 2020 2072 656d 6f74 653d 6675 6c6c 5f70     remote=full_p
+00004f60: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+00004f70: 2020 2020 2063 6d64 203d 2066 2274 696d       cmd = f"tim
+00004f80: 6520 7368 207b 7363 7269 7074 5f6e 616d  e sh {script_nam
+00004f90: 657d 220a 2020 2020 2020 2020 2020 2020  e}".            
+00004fa0: 2020 2020 7220 3d20 7365 6c66 2e72 756e      r = self.run
+00004fb0: 5f63 6f6d 6d61 6e64 7328 5b63 6d64 5d29  _commands([cmd])
+00004fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004fd0: 2069 6620 6e6f 7420 722e 6f6b 3a0a 2020   if not r.ok:.  
+00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ff0: 2020 7261 6973 6520 5353 4845 7863 6570    raise SSHExcep
+00005000: 7469 6f6e 2872 290a 2020 2020 2020 2020  tion(r).        
+00005010: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+00005020: 6e66 6f28 722e 7374 646f 7574 290a 2020  nfo(r.stdout).  
+00005030: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+00005040: 6767 6572 2e69 6e66 6f28 2249 6e69 7469  gger.info("Initi
+00005050: 6174 6564 2064 6f77 6e6c 6f61 6469 6e67  ated downloading
+00005060: 2061 6e64 2062 7569 6c64 696e 6722 202b   and building" +
+00005070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005080: 2020 2020 2020 2020 2020 2020 2022 2063               " c
+00005090: 6f6e 7461 696e 6572 2069 6d61 6765 7320  ontainer images 
+000050a0: 6f6e 2053 6c75 726d 2e22 202b 0a20 2020  on Slurm." +.   
+000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000050c0: 2020 2020 2020 2020 2022 2054 6869 7320           " This 
+000050d0: 7769 6c6c 2070 726f 6261 626c 7920 7461  will probably ta
+000050e0: 6b65 2061 2077 6869 6c65 2069 6e20 7468  ke a while in th
+000050f0: 6520 6261 636b 6772 6f75 6e64 2e22 202b  e background." +
+00005100: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00005110: 2020 2020 2020 2020 2020 2020 2020 2220                " 
+00005120: 4368 6563 6b20 2773 696e 672e 6c6f 6727  Check 'sing.log'
+00005130: 206f 6e20 536c 7572 6d20 666f 7220 7072   on Slurm for pr
+00005140: 6f67 7265 7373 2e22 290a 2020 2020 2020  ogress.").      
+00005150: 2020 2020 2020 2020 2020 2320 2320 636c            # # cl
+00005160: 6561 6e75 7020 6769 616e 7420 7369 6e67  eanup giant sing
+00005170: 756c 6172 6974 7920 6361 6368 6521 0a20  ularity cache!. 
+00005180: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00005190: 2075 7369 6e67 202d 2d64 6973 6162 6c65   using --disable
+000051a0: 2d63 6163 6865 2062 6563 6175 7365 2077  -cache because w
+000051b0: 6520 7275 6e20 696e 2074 6865 2062 6163  e run in the bac
+000051c0: 6b67 726f 756e 640a 2020 2020 2020 2020  kground.        
+000051d0: 2020 2020 2020 2020 2320 636d 6420 3d20          # cmd = 
+000051e0: 2273 696e 6775 6c61 7269 7479 2063 6163  "singularity cac
+000051f0: 6865 2063 6c65 616e 202d 6622 0a20 2020  he clean -f".   
+00005200: 2020 2020 2020 2020 2020 2020 2023 2072               # r
+00005210: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
+00005220: 616e 6473 285b 636d 645d 290a 0a20 2020  ands([cmd])..   
+00005230: 2064 6566 2073 6574 7570 5f63 6f6e 7665   def setup_conve
+00005240: 7274 6572 7328 7365 6c66 293a 0a20 2020  rters(self):.   
+00005250: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00005260: 2053 6574 7320 7570 2063 6f6e 7665 7274   Sets up convert
+00005270: 6572 7320 666f 7220 536c 7572 6d20 6f70  ers for Slurm op
+00005280: 6572 6174 696f 6e73 2e0a 0a20 2020 2020  erations...     
+00005290: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
+000052a0: 2063 7265 6174 6573 206e 6563 6573 7361   creates necessa
+000052b0: 7279 2064 6972 6563 746f 7269 6573 2066  ry directories f
+000052c0: 6f72 2063 6f6e 7665 7274 6572 7320 616e  or converters an
+000052d0: 6420 636f 7069 6573 0a20 2020 2020 2020  d copies.       
+000052e0: 2063 6f6e 7665 7274 6572 2073 6372 6970   converter scrip
+000052f0: 7473 2061 6e64 2064 6566 696e 6974 696f  ts and definitio
+00005300: 6e73 2074 6f20 7468 6520 6170 7072 6f70  ns to the approp
+00005310: 7269 6174 6520 6c6f 6361 7469 6f6e 732e  riate locations.
+00005320: 2049 7420 616c 736f 0a20 2020 2020 2020   It also.       
+00005330: 2062 7569 6c64 7320 5369 6e67 756c 6172   builds Singular
+00005340: 6974 7920 636f 6e74 6169 6e65 7273 2066  ity containers f
+00005350: 726f 6d20 7468 6520 7072 6f76 6964 6564  rom the provided
+00005360: 2064 6566 696e 6974 696f 6e73 2e0a 0a20   definitions... 
+00005370: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
+00005380: 2020 2020 2020 2020 2020 2053 5348 4578             SSHEx
+00005390: 6365 7074 696f 6e3a 2049 6620 7468 6572  ception: If ther
+000053a0: 6520 6973 2061 6e20 6973 7375 6520 6578  e is an issue ex
+000053b0: 6563 7574 696e 6720 636f 6d6d 616e 6473  ecuting commands
+000053c0: 206f 7220 636f 7079 696e 6720 6669 6c65   or copying file
+000053d0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+000053e0: 2020 2020 2020 2063 6f6e 7665 7274 5f63         convert_c
+000053f0: 6d64 7320 3d20 5b5d 0a20 2020 2020 2020  mds = [].       
+00005400: 2069 6620 7365 6c66 2e73 6c75 726d 5f63   if self.slurm_c
+00005410: 6f6e 7665 7274 6572 735f 7061 7468 3a0a  onverters_path:.
+00005420: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
+00005430: 6572 745f 636d 6473 2e61 7070 656e 6428  ert_cmds.append(
+00005440: 6622 6d6b 6469 7220 2d70 205c 227b 7365  f"mkdir -p \"{se
+00005450: 6c66 2e73 6c75 726d 5f63 6f6e 7665 7274  lf.slurm_convert
+00005460: 6572 735f 7061 7468 7d5c 2222 290a 2020  ers_path}\"").  
+00005470: 2020 2020 2020 7220 3d20 7365 6c66 2e72        r = self.r
+00005480: 756e 5f63 6f6d 6d61 6e64 7328 636f 6e76  un_commands(conv
+00005490: 6572 745f 636d 6473 290a 2020 2020 2020  ert_cmds).      
+000054a0: 2020 2320 636f 7079 2067 656e 6572 6963    # copy generic
+000054b0: 206a 6f62 2061 7272 6179 2073 6372 6970   job array scrip
+000054c0: 7420 6f76 6572 2074 6f20 736c 7572 6d0a  t over to slurm.
+000054d0: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
+000054e0: 6a6f 625f 6c6f 6361 6c20 3d20 6669 6c65  job_local = file
+000054f0: 7328 2272 6573 6f75 7263 6573 2229 2e6a  s("resources").j
+00005500: 6f69 6e70 6174 6828 0a20 2020 2020 2020  oinpath(.       
+00005510: 2020 2020 2022 636f 6e76 6572 745f 6a6f       "convert_jo
+00005520: 625f 6172 7261 792e 7368 2229 0a20 2020  b_array.sh").   
+00005530: 2020 2020 205f 203d 2073 656c 662e 7075       _ = self.pu
+00005540: 7428 6c6f 6361 6c3d 636f 6e76 6572 745f  t(local=convert_
+00005550: 6a6f 625f 6c6f 6361 6c2c 0a20 2020 2020  job_local,.     
+00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005570: 7265 6d6f 7465 3d73 656c 662e 736c 7572  remote=self.slur
+00005580: 6d5f 7363 7269 7074 5f70 6174 6829 0a20  m_script_path). 
+00005590: 2020 2020 2020 2023 2063 7572 7265 6e74         # current
+000055a0: 6c79 206b 6e6f 776e 2063 6f6e 7665 7274  ly known convert
+000055b0: 6572 730a 2020 2020 2020 2020 2320 3361  ers.        # 3a
+000055c0: 2e20 5a41 5252 2074 6f20 5449 4646 0a20  . ZARR to TIFF. 
+000055d0: 2020 2020 2020 2023 2054 4f44 4f20 6578         # TODO ex
+000055e0: 7472 6163 7420 7468 6573 6520 7661 6c75  tract these valu
+000055f0: 6573 2074 6f20 652e 672e 2063 6f6e 6669  es to e.g. confi
+00005600: 6720 6966 2077 6520 6861 7665 206d 6f72  g if we have mor
+00005610: 650a 2020 2020 2020 2020 636f 6e76 6572  e.        conver
+00005620: 745f 6e61 6d65 203d 2022 636f 6e76 6572  t_name = "conver
+00005630: 745f 7a61 7272 5f74 6f5f 7469 6666 220a  t_zarr_to_tiff".
+00005640: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
+00005650: 7079 203d 2066 227b 636f 6e76 6572 745f  py = f"{convert_
+00005660: 6e61 6d65 7d2e 7079 220a 2020 2020 2020  name}.py".      
+00005670: 2020 636f 6e76 6572 745f 7363 7269 7074    convert_script
+00005680: 5f6c 6f63 616c 203d 2066 696c 6573 2822  _local = files("
+00005690: 7265 736f 7572 6365 7322 292e 6a6f 696e  resources").join
+000056a0: 7061 7468 280a 2020 2020 2020 2020 2020  path(.          
+000056b0: 2020 636f 6e76 6572 745f 7079 290a 2020    convert_py).  
+000056c0: 2020 2020 2020 636f 6e76 6572 745f 6465        convert_de
+000056d0: 6620 3d20 6622 7b63 6f6e 7665 7274 5f6e  f = f"{convert_n
+000056e0: 616d 657d 2e64 6566 220a 2020 2020 2020  ame}.def".      
+000056f0: 2020 636f 6e76 6572 745f 6465 665f 6c6f    convert_def_lo
+00005700: 6361 6c20 3d20 6669 6c65 7328 2272 6573  cal = files("res
+00005710: 6f75 7263 6573 2229 2e6a 6f69 6e70 6174  ources").joinpat
+00005720: 6828 0a20 2020 2020 2020 2020 2020 2063  h(.            c
+00005730: 6f6e 7665 7274 5f64 6566 290a 2020 2020  onvert_def).    
+00005740: 2020 2020 5f20 3d20 7365 6c66 2e70 7574      _ = self.put
+00005750: 286c 6f63 616c 3d63 6f6e 7665 7274 5f73  (local=convert_s
+00005760: 6372 6970 745f 6c6f 6361 6c2c 0a20 2020  cript_local,.   
+00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005780: 2020 7265 6d6f 7465 3d73 656c 662e 736c    remote=self.sl
+00005790: 7572 6d5f 636f 6e76 6572 7465 7273 5f70  urm_converters_p
+000057a0: 6174 6829 0a20 2020 2020 2020 205f 203d  ath).        _ =
+000057b0: 2073 656c 662e 7075 7428 6c6f 6361 6c3d   self.put(local=
+000057c0: 636f 6e76 6572 745f 6465 665f 6c6f 6361  convert_def_loca
+000057d0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
+000057e0: 2020 2020 2020 2020 7265 6d6f 7465 3d73          remote=s
+000057f0: 656c 662e 736c 7572 6d5f 636f 6e76 6572  elf.slurm_conver
+00005800: 7465 7273 5f70 6174 6829 0a20 2020 2020  ters_path).     
+00005810: 2020 2023 2042 7569 6c64 2073 696e 6775     # Build singu
+00005820: 6c61 7269 7479 2063 6f6e 7461 696e 6572  larity container
+00005830: 2066 726f 6d20 6465 6669 6e69 7469 6f6e   from definition
+00005840: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
+00005850: 6c66 2e63 6428 7365 6c66 2e73 6c75 726d  lf.cd(self.slurm
+00005860: 5f63 6f6e 7665 7274 6572 735f 7061 7468  _converters_path
+00005870: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+00005880: 6f6e 7665 7274 5f63 6d64 7320 3d20 5b5d  onvert_cmds = []
+00005890: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000058a0: 7365 6c66 2e73 6c75 726d 5f69 6d61 6765  self.slurm_image
+000058b0: 735f 7061 7468 3a0a 2020 2020 2020 2020  s_path:.        
+000058c0: 2020 2020 2020 2020 2320 544f 444f 2043          # TODO C
+000058d0: 6861 6e67 6520 7468 6520 746d 7020 6469  hange the tmp di
+000058e0: 723f 0a20 2020 2020 2020 2020 2020 2020  r?.             
+000058f0: 2020 2023 2065 7870 6f72 7420 5349 4e47     # export SING
+00005900: 554c 4152 4954 595f 544d 5044 4952 3d7e  ULARITY_TMPDIR=~
+00005910: 2f6d 792d 7363 7261 7463 682f 746d 703b  /my-scratch/tmp;
+00005920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005930: 2023 206f 6e6c 7920 6966 2066 696c 6520   # only if file 
+00005940: 646f 6573 206e 6f74 2065 7869 7374 2079  does not exist y
+00005950: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
+00005960: 2020 2023 2063 6f6e 7665 7274 5f63 6d64     # convert_cmd
+00005970: 732e 6170 7065 6e64 2866 225b 2021 202d  s.append(f"[ ! -
+00005980: 6620 7b63 6f6e 7665 7274 5f6e 616d 657d  f {convert_name}
+00005990: 2e73 6966 205d 2229 0a20 2020 2020 2020  .sif ]").       
+000059a0: 2020 2020 2020 2020 2023 2045 4449 5420           # EDIT 
+000059b0: 2d2d 204e 4f2c 2074 6865 6e20 7765 2063  -- NO, then we c
+000059c0: 616e 2774 2075 7064 6174 6521 2046 6f72  an't update! For
+000059d0: 6365 2072 6562 7569 6c64 210a 2020 2020  ce rebuild!.    
+000059e0: 2020 2020 2020 2020 2020 2020 2320 646f              # do
+000059f0: 776e 6c6f 6164 202f 6275 696c 6420 6e65  wnload /build ne
+00005a00: 7720 636f 6e74 6169 6e65 720a 2020 2020  w container.    
+00005a10: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
+00005a20: 6572 745f 636d 6473 2e61 7070 656e 6428  ert_cmds.append(
+00005a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005a40: 2020 2020 2066 2273 696e 6775 6c61 7269       f"singulari
+00005a50: 7479 2062 7569 6c64 202d 4620 5c22 7b63  ty build -F \"{c
+00005a60: 6f6e 7665 7274 5f6e 616d 657d 2e73 6966  onvert_name}.sif
+00005a70: 5c22 207b 636f 6e76 6572 745f 6465 667d  \" {convert_def}
+00005a80: 203e 3e20 7369 6e67 2e6c 6f67 2032 3e26   >> sing.log 2>&
+00005a90: 3120 3b20 6563 686f 2027 6669 6e69 7368  1 ; echo 'finish
+00005aa0: 6564 207b 636f 6e76 6572 745f 6e61 6d65  ed {convert_name
+00005ab0: 7d2e 7369 6627 2026 2229 0a20 2020 2020  }.sif' &").     
+00005ac0: 2020 2020 2020 205f 203d 2073 656c 662e         _ = self.
+00005ad0: 7275 6e5f 636f 6d6d 616e 6473 2863 6f6e  run_commands(con
+00005ae0: 7665 7274 5f63 6d64 7329 0a0a 2020 2020  vert_cmds)..    
+00005af0: 6465 6620 7365 7475 705f 6a6f 625f 7363  def setup_job_sc
+00005b00: 7269 7074 7328 7365 6c66 293a 0a20 2020  ripts(self):.   
+00005b10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00005b20: 2053 6574 7320 7570 206a 6f62 2073 6372   Sets up job scr
+00005b30: 6970 7473 2066 6f72 2053 6c75 726d 206f  ipts for Slurm o
+00005b40: 7065 7261 7469 6f6e 732e 0a0a 2020 2020  perations...    
+00005b50: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
+00005b60: 6e20 6569 7468 6572 2063 6c6f 6e65 7320  n either clones 
+00005b70: 6120 4769 7420 7265 706f 7369 746f 7279  a Git repository
+00005b80: 2063 6f6e 7461 696e 696e 6720 6a6f 6220   containing job 
+00005b90: 7363 7269 7074 730a 2020 2020 2020 2020  scripts.        
+00005ba0: 696e 746f 2074 6865 2073 7065 6369 6669  into the specifi
+00005bb0: 6564 2073 6372 6970 7420 7061 7468 206f  ed script path o
+00005bc0: 7220 6765 6e65 7261 7465 7320 7363 7269  r generates scri
+00005bd0: 7074 7320 6c6f 6361 6c6c 7920 6966 206e  pts locally if n
+00005be0: 6f20 7265 706f 7369 746f 7279 0a20 2020  o repository.   
+00005bf0: 2020 2020 2069 7320 7072 6f76 6964 6564       is provided
+00005c00: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00005c10: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
+00005c20: 5348 4578 6365 7074 696f 6e3a 2049 6620  SHException: If 
+00005c30: 7468 6572 6520 6973 2061 6e20 6973 7375  there is an issu
+00005c40: 6520 6578 6563 7574 696e 6720 4769 7420  e executing Git 
+00005c50: 636f 6d6d 616e 6473 206f 7220 6765 6e65  commands or gene
+00005c60: 7261 7469 6e67 2073 6372 6970 7473 2e0a  rating scripts..
+00005c70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00005c80: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
+00005c90: 6d5f 7363 7269 7074 5f72 6570 6f20 616e  m_script_repo an
+00005ca0: 6420 7365 6c66 2e73 6c75 726d 5f73 6372  d self.slurm_scr
+00005cb0: 6970 745f 7061 7468 3a0a 2020 2020 2020  ipt_path:.      
+00005cc0: 2020 2020 2020 2320 6769 7420 636c 6f6e        # git clon
+00005cd0: 6520 696e 746f 2073 6372 6970 7420 7061  e into script pa
+00005ce0: 7468 0a20 2020 2020 2020 2020 2020 2065  th.            e
+00005cf0: 6e76 203d 207b 0a20 2020 2020 2020 2020  nv = {.         
+00005d00: 2020 2020 2020 2022 5245 504f 5352 4322         "REPOSRC"
+00005d10: 3a20 6622 5c22 7b73 656c 662e 736c 7572  : f"\"{self.slur
+00005d20: 6d5f 7363 7269 7074 5f72 6570 6f7d 5c22  m_script_repo}\"
+00005d30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00005d40: 2020 2022 4c4f 4341 4c52 4550 4f22 3a20     "LOCALREPO": 
+00005d50: 6622 5c22 7b73 656c 662e 736c 7572 6d5f  f"\"{self.slurm_
+00005d60: 7363 7269 7074 5f70 6174 687d 5c22 220a  script_path}\"".
+00005d70: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00005d80: 2020 2020 2020 2020 2020 2320 436c 6561            # Clea
+00005d90: 6e75 7020 7468 6520 6578 6973 7469 6e67  nup the existing
+00005da0: 2066 6f6c 6465 7220 6669 7273 740a 2020   folder first.  
+00005db0: 2020 2020 2020 2020 2020 636c 6561 6e75            cleanu
+00005dc0: 705f 6669 7273 7420 3d20 2772 6d20 2d72  p_first = 'rm -r
+00005dd0: 6620 2224 4c4f 4341 4c52 4550 4f22 270a  f "$LOCALREPO"'.
+00005de0: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
+00005df0: 3d20 2767 6974 2063 6c6f 6e65 2022 2452  = 'git clone "$R
+00005e00: 4550 4f53 5243 2220 2224 4c4f 4341 4c52  EPOSRC" "$LOCALR
+00005e10: 4550 4f22 2032 3e20 2f64 6576 2f6e 756c  EPO" 2> /dev/nul
+00005e20: 6c27 0a20 2020 2020 2020 2020 2020 2072  l'.            r
+00005e30: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
+00005e40: 616e 6473 285b 636c 6561 6e75 705f 6669  ands([cleanup_fi
+00005e50: 7273 742c 2063 6d64 5d2c 2065 6e76 290a  rst, cmd], env).
+00005e60: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00005e70: 6f74 2072 2e6f 6b3a 0a20 2020 2020 2020  ot r.ok:.       
+00005e80: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
+00005e90: 5348 4578 6365 7074 696f 6e28 7229 0a20  SHException(r). 
+00005ea0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
+00005eb0: 2e73 6c75 726d 5f73 6372 6970 745f 7061  .slurm_script_pa
+00005ec0: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
+00005ed0: 2320 6765 6e65 7261 7465 2073 6372 6970  # generate scrip
+00005ee0: 7473 0a20 2020 2020 2020 2020 2020 2073  ts.            s
+00005ef0: 656c 662e 7570 6461 7465 5f73 6c75 726d  elf.update_slurm
+00005f00: 5f73 6372 6970 7473 2867 656e 6572 6174  _scripts(generat
+00005f10: 655f 6a6f 6273 3d54 7275 6529 0a0a 2020  e_jobs=True)..  
+00005f20: 2020 6465 6620 7365 7475 705f 6469 7265    def setup_dire
+00005f30: 6374 6f72 6965 7328 7365 6c66 293a 0a20  ctories(self):. 
+00005f40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005f50: 2020 2043 7265 6174 6573 206e 6563 6573     Creates neces
+00005f60: 7361 7279 2064 6972 6563 746f 7269 6573  sary directories
+00005f70: 2066 6f72 2053 6c75 726d 206f 7065 7261   for Slurm opera
+00005f80: 7469 6f6e 732e 0a0a 2020 2020 2020 2020  tions...        
+00005f90: 5468 6973 2066 756e 6374 696f 6e20 6372  This function cr
+00005fa0: 6561 7465 7320 6469 7265 6374 6f72 6965  eates directorie
+00005fb0: 7320 666f 7220 6461 7461 2073 746f 7261  s for data stora
+00005fc0: 6765 2c20 7363 7269 7074 732c 2061 6e64  ge, scripts, and
+00005fd0: 2077 6f72 6b66 6c6f 7773 0a20 2020 2020   workflows.     
+00005fe0: 2020 2061 7320 7370 6563 6966 6965 6420     as specified 
+00005ff0: 696e 2074 6865 2053 6c75 726d 436c 6965  in the SlurmClie
+00006000: 6e74 206f 626a 6563 742e 0a0a 2020 2020  nt object...    
+00006010: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
+00006020: 2020 2020 2020 2020 5353 4845 7863 6570          SSHExcep
+00006030: 7469 6f6e 3a20 4966 2074 6865 7265 2069  tion: If there i
+00006040: 7320 616e 2069 7373 7565 2065 7865 6375  s an issue execu
+00006050: 7469 6e67 2064 6972 6563 746f 7279 2063  ting directory c
+00006060: 7265 6174 696f 6e20 636f 6d6d 616e 6473  reation commands
+00006070: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00006080: 2020 2020 2020 6469 725f 636d 6473 203d        dir_cmds =
+00006090: 205b 5d0a 2020 2020 2020 2020 2320 612e   [].        # a.
+000060a0: 2064 6174 610a 2020 2020 2020 2020 6966   data.        if
+000060b0: 2073 656c 662e 736c 7572 6d5f 6461 7461   self.slurm_data
+000060c0: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
+000060d0: 2020 2064 6972 5f63 6d64 732e 6170 7065     dir_cmds.appe
+000060e0: 6e64 2866 226d 6b64 6972 202d 7020 5c22  nd(f"mkdir -p \"
+000060f0: 7b73 656c 662e 736c 7572 6d5f 6461 7461  {self.slurm_data
+00006100: 5f70 6174 687d 5c22 2229 0a20 2020 2020  _path}\"").     
+00006110: 2020 2020 2020 2023 2062 2e20 7363 7269         # b. scri
+00006120: 7074 730a 2020 2020 2020 2020 6966 2073  pts.        if s
+00006130: 656c 662e 736c 7572 6d5f 7363 7269 7074  elf.slurm_script
+00006140: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
+00006150: 2020 2064 6972 5f63 6d64 732e 6170 7065     dir_cmds.appe
+00006160: 6e64 2866 226d 6b64 6972 202d 7020 5c22  nd(f"mkdir -p \"
+00006170: 7b73 656c 662e 736c 7572 6d5f 7363 7269  {self.slurm_scri
+00006180: 7074 5f70 6174 687d 5c22 2229 0a20 2020  pt_path}\"").   
+00006190: 2020 2020 2020 2020 2023 2063 2e20 776f           # c. wo
+000061a0: 726b 666c 6f77 730a 2020 2020 2020 2020  rkflows.        
+000061b0: 6966 2073 656c 662e 736c 7572 6d5f 696d  if self.slurm_im
+000061c0: 6167 6573 5f70 6174 683a 0a20 2020 2020  ages_path:.     
+000061d0: 2020 2020 2020 2064 6972 5f63 6d64 732e         dir_cmds.
+000061e0: 6170 7065 6e64 2866 226d 6b64 6972 202d  append(f"mkdir -
+000061f0: 7020 5c22 7b73 656c 662e 736c 7572 6d5f  p \"{self.slurm_
+00006200: 696d 6167 6573 5f70 6174 687d 5c22 2229  images_path}\"")
+00006210: 0a20 2020 2020 2020 2072 203d 2073 656c  .        r = sel
+00006220: 662e 7275 6e5f 636f 6d6d 616e 6473 2864  f.run_commands(d
+00006230: 6972 5f63 6d64 7329 0a20 2020 2020 2020  ir_cmds).       
+00006240: 2069 6620 6e6f 7420 722e 6f6b 3a0a 2020   if not r.ok:.  
+00006250: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00006260: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
+00006270: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+00006280: 640a 2020 2020 6465 6620 6672 6f6d 5f63  d.    def from_c
+00006290: 6f6e 6669 6728 636c 732c 2063 6f6e 6669  onfig(cls, confi
+000062a0: 6766 696c 653a 2073 7472 203d 2027 272c  gfile: str = '',
+000062b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000062c0: 2020 2020 2069 6e69 745f 736c 7572 6d3a       init_slurm:
+000062d0: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
+000062e0: 3e20 2753 6c75 726d 436c 6965 6e74 273a  > 'SlurmClient':
+000062f0: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
+00006300: 7465 7320 6120 6e65 7720 536c 7572 6d43  tes a new SlurmC
+00006310: 6c69 656e 7420 6f62 6a65 6374 2075 7369  lient object usi
+00006320: 6e67 2074 6865 2070 6172 616d 6574 6572  ng the parameter
+00006330: 7320 7265 6164 2066 726f 6d20 610a 2020  s read from a.  
+00006340: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
+00006350: 696f 6e20 6669 6c65 2028 2e69 6e69 292e  ion file (.ini).
+00006360: 0a0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
+00006370: 7473 2070 6174 6873 2074 6f20 6c6f 6f6b  ts paths to look
+00006380: 2066 6f72 2063 6f6e 6669 6720 6669 6c65   for config file
+00006390: 7320 6172 653a 0a20 2020 2020 2020 2020  s are:.         
+000063a0: 2020 202d 202f 6574 632f 736c 7572 6d2d     - /etc/slurm-
+000063b0: 636f 6e66 6967 2e69 6e69 0a20 2020 2020  config.ini.     
+000063c0: 2020 2020 2020 202d 207e 2f73 6c75 726d         - ~/slurm
+000063d0: 2d63 6f6e 6669 672e 696e 690a 0a20 2020  -config.ini..   
+000063e0: 2020 2020 204e 6f74 6520 7468 6174 2074       Note that t
+000063f0: 6869 7320 6973 206f 6e6c 7920 666f 7220  his is only for 
+00006400: 7468 6520 534c 5552 4d20 7370 6563 6966  the SLURM specif
+00006410: 6963 2076 616c 7565 7320 7468 6174 2077  ic values that w
+00006420: 6520 6164 6465 642e 0a20 2020 2020 2020  e added..       
+00006430: 204d 6f73 7420 636f 6e66 6967 7572 6174   Most configurat
+00006440: 696f 6e20 7661 6c75 6573 2061 7265 2073  ion values are s
+00006450: 6574 2076 6961 2063 6f6e 6669 6775 7261  et via configura
+00006460: 7469 6f6e 206d 6563 6861 6e69 736d 7320  tion mechanisms 
+00006470: 6672 6f6d 0a20 2020 2020 2020 2046 6162  from.        Fab
+00006480: 7269 6320 6c69 6272 6172 792c 0a20 2020  ric library,.   
+00006490: 2020 2020 206c 696b 6520 5353 4820 7365       like SSH se
+000064a0: 7474 696e 6773 2062 6569 6e67 206c 6f61  ttings being loa
+000064b0: 6465 6420 6672 6f6d 2053 5348 2063 6f6e  ded from SSH con
+000064c0: 6669 672c 202f 6574 632f 6661 6272 6963  fig, /etc/fabric
+000064d0: 2e79 6d6c 206f 720a 2020 2020 2020 2020  .yml or.        
+000064e0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+000064f0: 6162 6c65 732e 0a20 2020 2020 2020 2053  ables..        S
+00006500: 6565 2046 6162 7269 6327 7320 646f 6375  ee Fabric's docu
+00006510: 6d65 6e74 6174 696f 6e20 666f 7220 6d6f  mentation for mo
+00006520: 7265 2069 6e66 6f20 6f6e 2063 6f6e 6669  re info on confi
+00006530: 6775 7261 7469 6f6e 2069 6620 6e65 6564  guration if need
+00006540: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
+00006550: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+00006560: 6f6e 6669 6766 696c 6520 2873 7472 293a  onfigfile (str):
+00006570: 2054 6865 2070 6174 6820 746f 2079 6f75   The path to you
+00006580: 7220 636f 6e66 6967 7572 6174 696f 6e20  r configuration 
+00006590: 6669 6c65 2e20 4f70 7469 6f6e 616c 2e0a  file. Optional..
+000065a0: 2020 2020 2020 2020 2020 2020 696e 6974              init
+000065b0: 5f73 6c75 726d 2028 626f 6f6c 293a 2049  _slurm (bool): I
+000065c0: 6e69 7469 6174 6520 2f20 7661 6c69 6461  nitiate / valida
+000065d0: 7465 2073 6c75 726d 2073 6574 7570 2e20  te slurm setup. 
+000065e0: 4f70 7469 6f6e 616c 0a20 2020 2020 2020  Optional.       
+000065f0: 2020 2020 2020 2020 204d 6967 6874 2074           Might t
+00006600: 616b 6520 736f 6d65 2074 696d 6520 7468  ake some time th
+00006610: 6520 6669 7273 7420 7469 6d65 2077 6974  e first time wit
+00006620: 6820 646f 776e 6c6f 6164 696e 6720 6574  h downloading et
+00006630: 632e 0a0a 2020 2020 2020 2020 5265 7475  c...        Retu
+00006640: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00006650: 2053 6c75 726d 436c 6965 6e74 3a20 4120   SlurmClient: A 
+00006660: 6e65 7720 536c 7572 6d43 6c69 656e 7420  new SlurmClient 
+00006670: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
+00006680: 2222 220a 2020 2020 2020 2020 2320 4c6f  """.        # Lo
+00006690: 6164 2074 6865 2063 6f6e 6669 6775 7261  ad the configura
+000066a0: 7469 6f6e 2066 696c 650a 2020 2020 2020  tion file.      
+000066b0: 2020 636f 6e66 6967 7320 3d20 636f 6e66    configs = conf
+000066c0: 6967 7061 7273 6572 2e43 6f6e 6669 6750  igparser.ConfigP
+000066d0: 6172 7365 7228 616c 6c6f 775f 6e6f 5f76  arser(allow_no_v
+000066e0: 616c 7565 3d54 7275 6529 0a20 2020 2020  alue=True).     
+000066f0: 2020 2023 204c 6f61 6473 2066 726f 6d20     # Loads from 
+00006700: 6465 6661 756c 7420 6c6f 6361 7469 6f6e  default location
+00006710: 7320 616e 6420 6769 7665 6e20 6c6f 6361  s and given loca
+00006720: 7469 6f6e 2c20 6d69 7373 696e 6720 6669  tion, missing fi
+00006730: 6c65 7320 6172 6520 6f6b 0a20 2020 2020  les are ok.     
+00006740: 2020 2063 6f6e 6669 6773 2e72 6561 6428     configs.read(
+00006750: 5b63 6c73 2e5f 4445 4641 554c 545f 434f  [cls._DEFAULT_CO
+00006760: 4e46 4947 5f50 4154 485f 312c 0a20 2020  NFIG_PATH_1,.   
+00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006780: 2020 636c 732e 5f44 4546 4155 4c54 5f43    cls._DEFAULT_C
+00006790: 4f4e 4649 475f 5041 5448 5f32 2c0a 2020  ONFIG_PATH_2,.  
+000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067b0: 2020 2063 6f6e 6669 6766 696c 655d 290a     configfile]).
+000067c0: 2020 2020 2020 2020 2320 5265 6164 2074          # Read t
+000067d0: 6865 2072 6571 7569 7265 6420 7061 7261  he required para
+000067e0: 6d65 7465 7273 2066 726f 6d20 7468 6520  meters from the 
+000067f0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00006800: 6c65 2c0a 2020 2020 2020 2020 2320 6661  le,.        # fa
+00006810: 6c6c 6261 636b 2074 6f20 6465 6661 756c  llback to defaul
+00006820: 7473 0a20 2020 2020 2020 2068 6f73 7420  ts.        host 
+00006830: 3d20 636f 6e66 6967 732e 6765 7428 2253  = configs.get("S
+00006840: 5348 222c 2022 686f 7374 222c 2066 616c  SH", "host", fal
+00006850: 6c62 6163 6b3d 636c 732e 5f44 4546 4155  lback=cls._DEFAU
+00006860: 4c54 5f48 4f53 5429 0a20 2020 2020 2020  LT_HOST).       
+00006870: 2069 6e6c 696e 655f 7373 685f 656e 7620   inline_ssh_env 
+00006880: 3d20 636f 6e66 6967 732e 6765 7462 6f6f  = configs.getboo
+00006890: 6c65 616e 280a 2020 2020 2020 2020 2020  lean(.          
+000068a0: 2020 2253 5348 222c 2022 696e 6c69 6e65    "SSH", "inline
+000068b0: 5f73 7368 5f65 6e76 222c 2066 616c 6c62  _ssh_env", fallb
+000068c0: 6163 6b3d 636c 732e 5f44 4546 4155 4c54  ack=cls._DEFAULT
+000068d0: 5f49 4e4c 494e 455f 5353 485f 454e 5629  _INLINE_SSH_ENV)
+000068e0: 0a20 2020 2020 2020 2073 6c75 726d 5f64  .        slurm_d
+000068f0: 6174 615f 7061 7468 203d 2063 6f6e 6669  ata_path = confi
+00006900: 6773 2e67 6574 280a 2020 2020 2020 2020  gs.get(.        
+00006910: 2020 2020 2253 4c55 524d 222c 2022 736c      "SLURM", "sl
+00006920: 7572 6d5f 6461 7461 5f70 6174 6822 2c20  urm_data_path", 
+00006930: 6661 6c6c 6261 636b 3d63 6c73 2e5f 4445  fallback=cls._DE
+00006940: 4641 554c 545f 534c 5552 4d5f 4441 5441  FAULT_SLURM_DATA
+00006950: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
+00006960: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
+00006970: 203d 2063 6f6e 6669 6773 2e67 6574 280a   = configs.get(.
+00006980: 2020 2020 2020 2020 2020 2020 2253 4c55              "SLU
+00006990: 524d 222c 2022 736c 7572 6d5f 696d 6167  RM", "slurm_imag
+000069a0: 6573 5f70 6174 6822 2c0a 2020 2020 2020  es_path",.      
+000069b0: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
+000069c0: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
+000069d0: 4d5f 494d 4147 4553 5f50 4154 4829 0a20  M_IMAGES_PATH). 
+000069e0: 2020 2020 2020 2073 6c75 726d 5f63 6f6e         slurm_con
+000069f0: 7665 7274 6572 735f 7061 7468 203d 2063  verters_path = c
+00006a00: 6f6e 6669 6773 2e67 6574 280a 2020 2020  onfigs.get(.    
+00006a10: 2020 2020 2020 2020 2253 4c55 524d 222c          "SLURM",
+00006a20: 2022 736c 7572 6d5f 636f 6e76 6572 7465   "slurm_converte
+00006a30: 7273 5f70 6174 6822 2c0a 2020 2020 2020  rs_path",.      
+00006a40: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
+00006a50: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
+00006a60: 4d5f 434f 4e56 4552 5445 5253 5f50 4154  M_CONVERTERS_PAT
+00006a70: 4829 0a0a 2020 2020 2020 2020 2320 5370  H)..        # Sp
+00006a80: 6c69 7420 7468 6520 4d4f 4445 4c53 2069  lit the MODELS i
+00006a90: 6e74 6f20 7061 7468 732c 2072 6570 6f73  nto paths, repos
+00006aa0: 2061 6e64 2069 6d61 6765 730a 2020 2020   and images.    
+00006ab0: 2020 2020 6d6f 6465 6c73 5f64 6963 7420      models_dict 
+00006ac0: 3d20 6469 6374 2863 6f6e 6669 6773 2e69  = dict(configs.i
+00006ad0: 7465 6d73 2822 4d4f 4445 4c53 2229 290a  tems("MODELS")).
+00006ae0: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
+00006af0: 6465 6c5f 7061 7468 7320 3d20 7b7d 0a20  del_paths = {}. 
+00006b00: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00006b10: 656c 5f72 6570 6f73 203d 207b 7d0a 2020  el_repos = {}.  
+00006b20: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+00006b30: 6c5f 6a6f 6273 203d 207b 7d0a 2020 2020  l_jobs = {}.    
+00006b40: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
+00006b50: 6a6f 6273 5f70 6172 616d 7320 3d20 7b7d  jobs_params = {}
+00006b60: 0a20 2020 2020 2020 2066 6f72 206b 2c20  .        for k, 
+00006b70: 7620 696e 206d 6f64 656c 735f 6469 6374  v in models_dict
+00006b80: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
+00006b90: 2020 2020 2020 7375 6666 6978 5f72 6570        suffix_rep
+00006ba0: 6f20 3d20 275f 7265 706f 270a 2020 2020  o = '_repo'.    
+00006bb0: 2020 2020 2020 2020 7375 6666 6978 5f6a          suffix_j
+00006bc0: 6f62 203d 2027 5f6a 6f62 270a 2020 2020  ob = '_job'.    
+00006bd0: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
+00006be0: 6d5f 7061 7474 6572 6e20 3d20 2228 2e2b  m_pattern = "(.+
+00006bf0: 295f 6a6f 625f 282e 2b29 220a 2020 2020  )_job_(.+)".    
+00006c00: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
+00006c10: 6d5f 6d61 7463 6820 3d20 7265 2e6d 6174  m_match = re.mat
+00006c20: 6368 286a 6f62 5f70 6172 616d 5f70 6174  ch(job_param_pat
+00006c30: 7465 726e 2c20 6b29 0a20 2020 2020 2020  tern, k).       
+00006c40: 2020 2020 2069 6620 6b2e 656e 6473 7769       if k.endswi
+00006c50: 7468 2873 7566 6669 785f 7265 706f 293a  th(suffix_repo):
+00006c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006c70: 2073 6c75 726d 5f6d 6f64 656c 5f72 6570   slurm_model_rep
+00006c80: 6f73 5b6b 5b3a 2d6c 656e 2873 7566 6669  os[k[:-len(suffi
+00006c90: 785f 7265 706f 295d 5d20 3d20 760a 2020  x_repo)]] = v.  
+00006ca0: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
+00006cb0: 2e65 6e64 7377 6974 6828 7375 6666 6978  .endswith(suffix
+00006cc0: 5f6a 6f62 293a 0a20 2020 2020 2020 2020  _job):.         
+00006cd0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00006ce0: 656c 5f6a 6f62 735b 6b5b 3a2d 6c65 6e28  el_jobs[k[:-len(
+00006cf0: 7375 6666 6978 5f6a 6f62 295d 5d20 3d20  suffix_job)]] = 
+00006d00: 760a 2020 2020 2020 2020 2020 2020 2020  v.              
+00006d10: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
+00006d20: 6273 5f70 6172 616d 735b 6b5b 3a2d 6c65  bs_params[k[:-le
+00006d30: 6e28 7375 6666 6978 5f6a 6f62 295d 5d20  n(suffix_job)]] 
+00006d40: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00006d50: 2065 6c69 6620 6a6f 625f 7061 7261 6d5f   elif job_param_
+00006d60: 6d61 7463 683a 0a20 2020 2020 2020 2020  match:.         
+00006d70: 2020 2020 2020 2070 7269 6e74 2866 224d         print(f"M
+00006d80: 6174 6368 3a20 7b73 6c75 726d 5f6d 6f64  atch: {slurm_mod
+00006d90: 656c 5f6a 6f62 735f 7061 7261 6d73 7d22  el_jobs_params}"
+00006da0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00006db0: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
+00006dc0: 6273 5f70 6172 616d 735b 6a6f 625f 7061  bs_params[job_pa
+00006dd0: 7261 6d5f 6d61 7463 682e 6772 6f75 7028  ram_match.group(
+00006de0: 3129 5d2e 6170 7065 6e64 280a 2020 2020  1)].append(.    
+00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006e00: 6622 202d 2d7b 6a6f 625f 7061 7261 6d5f  f" --{job_param_
+00006e10: 6d61 7463 682e 6772 6f75 7028 3229 7d3d  match.group(2)}=
+00006e20: 7b76 7d22 290a 2020 2020 2020 2020 2020  {v}").          
+00006e30: 2020 2020 2020 7072 696e 7428 6622 4164        print(f"Ad
+00006e40: 6465 643a 207b 736c 7572 6d5f 6d6f 6465  ded: {slurm_mode
+00006e50: 6c5f 6a6f 6273 5f70 6172 616d 737d 2229  l_jobs_params}")
+00006e60: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00006e70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00006e80: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
+00006e90: 6174 6873 5b6b 5d20 3d20 760a 0a20 2020  aths[k] = v..   
+00006ea0: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
+00006eb0: 745f 7061 7468 203d 2063 6f6e 6669 6773  t_path = configs
+00006ec0: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
+00006ed0: 2020 2253 4c55 524d 222c 2022 736c 7572    "SLURM", "slur
+00006ee0: 6d5f 7363 7269 7074 5f70 6174 6822 2c0a  m_script_path",.
+00006ef0: 2020 2020 2020 2020 2020 2020 6661 6c6c              fall
+00006f00: 6261 636b 3d63 6c73 2e5f 4445 4641 554c  back=cls._DEFAUL
+00006f10: 545f 534c 5552 4d5f 4749 545f 5343 5249  T_SLURM_GIT_SCRI
+00006f20: 5054 5f50 4154 4829 0a20 2020 2020 2020  PT_PATH).       
+00006f30: 2073 6c75 726d 5f73 6372 6970 745f 7265   slurm_script_re
+00006f40: 706f 203d 2063 6f6e 6669 6773 2e67 6574  po = configs.get
+00006f50: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
+00006f60: 4c55 524d 222c 2022 736c 7572 6d5f 7363  LURM", "slurm_sc
+00006f70: 7269 7074 5f72 6570 6f22 2c0a 2020 2020  ript_repo",.    
+00006f80: 2020 2020 2020 2020 6661 6c6c 6261 636b          fallback
+00006f90: 3d4e 6f6e 650a 2020 2020 2020 2020 290a  =None.        ).
+00006fa0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
+00006fb0: 2074 6865 2053 6c75 726d 436c 6965 6e74   the SlurmClient
+00006fc0: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
+00006fd0: 2070 6172 616d 6574 6572 7320 7265 6164   parameters read
+00006fe0: 2066 726f 6d0a 2020 2020 2020 2020 2320   from.        # 
+00006ff0: 7468 6520 636f 6e66 6967 2066 696c 650a  the config file.
+00007000: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00007010: 6c73 2868 6f73 743d 686f 7374 2c0a 2020  ls(host=host,.  
+00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007030: 2069 6e6c 696e 655f 7373 685f 656e 763d   inline_ssh_env=
+00007040: 696e 6c69 6e65 5f73 7368 5f65 6e76 2c0a  inline_ssh_env,.
+00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007060: 2020 2073 6c75 726d 5f64 6174 615f 7061     slurm_data_pa
+00007070: 7468 3d73 6c75 726d 5f64 6174 615f 7061  th=slurm_data_pa
+00007080: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00007090: 2020 2020 2020 2073 6c75 726d 5f69 6d61         slurm_ima
+000070a0: 6765 735f 7061 7468 3d73 6c75 726d 5f69  ges_path=slurm_i
+000070b0: 6d61 6765 735f 7061 7468 2c0a 2020 2020  mages_path,.    
+000070c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000070d0: 6c75 726d 5f63 6f6e 7665 7274 6572 735f  lurm_converters_
+000070e0: 7061 7468 3d73 6c75 726d 5f63 6f6e 7665  path=slurm_conve
+000070f0: 7274 6572 735f 7061 7468 2c0a 2020 2020  rters_path,.    
+00007100: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007110: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
+00007120: 3d73 6c75 726d 5f6d 6f64 656c 5f70 6174  =slurm_model_pat
+00007130: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
+00007140: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00007150: 656c 5f72 6570 6f73 3d73 6c75 726d 5f6d  el_repos=slurm_m
+00007160: 6f64 656c 5f72 6570 6f73 2c0a 2020 2020  odel_repos,.    
+00007170: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00007180: 6c75 726d 5f6d 6f64 656c 5f69 6d61 6765  lurm_model_image
+00007190: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+000071a0: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+000071b0: 5f6d 6f64 656c 5f6a 6f62 733d 736c 7572  _model_jobs=slur
+000071c0: 6d5f 6d6f 6465 6c5f 6a6f 6273 2c0a 2020  m_model_jobs,.  
+000071d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000071e0: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
+000071f0: 735f 7061 7261 6d73 3d73 6c75 726d 5f6d  s_params=slurm_m
+00007200: 6f64 656c 5f6a 6f62 735f 7061 7261 6d73  odel_jobs_params
+00007210: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007220: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
+00007230: 745f 7061 7468 3d73 6c75 726d 5f73 6372  t_path=slurm_scr
+00007240: 6970 745f 7061 7468 2c0a 2020 2020 2020  ipt_path,.      
+00007250: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
+00007260: 726d 5f73 6372 6970 745f 7265 706f 3d73  rm_script_repo=s
+00007270: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
+00007280: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007290: 2020 2020 2069 6e69 745f 736c 7572 6d3d       init_slurm=
+000072a0: 696e 6974 5f73 6c75 726d 290a 0a20 2020  init_slurm)..   
+000072b0: 2064 6566 2063 6c65 616e 7570 5f74 6d70   def cleanup_tmp
+000072c0: 5f66 696c 6573 2873 656c 662c 0a20 2020  _files(self,.   
+000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000072e0: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
+000072f0: 5f69 643a 2073 7472 2c0a 2020 2020 2020  _id: str,.      
+00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007310: 2020 2020 6669 6c65 6e61 6d65 3a20 7374      filename: st
+00007320: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007340: 2020 2020 6461 7461 5f6c 6f63 6174 696f      data_locatio
+00007350: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
+00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007370: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
+00007380: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
+00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000073a0: 2020 2020 2020 2020 2920 2d3e 2052 6573          ) -> Res
+000073b0: 756c 743a 0a20 2020 2020 2020 2022 2222  ult:.        """
+000073c0: 0a20 2020 2020 2020 2043 6c65 616e 7570  .        Cleanup
+000073d0: 207a 6970 2061 6e64 2075 6e7a 6970 7065   zip and unzippe
+000073e0: 6420 6669 6c65 732f 666f 6c64 6572 7320  d files/folders 
+000073f0: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+00007400: 6120 536c 7572 6d20 6a6f 622e 0a0a 2020  a Slurm job...  
+00007410: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00007420: 2020 2020 2020 2020 736c 7572 6d5f 6a6f          slurm_jo
+00007430: 625f 6964 2028 7374 7229 3a20 5468 6520  b_id (str): The 
+00007440: 6a6f 6220 4944 206f 6620 7468 6520 536c  job ID of the Sl
+00007450: 7572 6d20 7363 7269 7074 2e0a 2020 2020  urm script..    
+00007460: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+00007470: 2028 7374 7229 3a20 5468 6520 7a69 7020   (str): The zip 
+00007480: 6669 6c65 6e61 6d65 206f 6e20 536c 7572  filename on Slur
+00007490: 6d2e 0a20 2020 2020 2020 2020 2020 2064  m..            d
+000074a0: 6174 615f 6c6f 6361 7469 6f6e 2028 7374  ata_location (st
+000074b0: 722c 206f 7074 696f 6e61 6c29 3a20 5468  r, optional): Th
+000074c0: 6520 6c6f 6361 7469 6f6e 206f 6620 6461  e location of da
+000074d0: 7461 2066 696c 6573 206f 6e20 536c 7572  ta files on Slur
+000074e0: 6d2e 0a20 2020 2020 2020 2020 2020 2020  m..             
+000074f0: 2020 2049 6620 6e6f 7420 7072 6f76 6964     If not provid
+00007500: 6564 2c20 6974 2077 696c 6c20 6265 2065  ed, it will be e
+00007510: 7874 7261 6374 6564 2066 726f 6d20 7468  xtracted from th
+00007520: 6520 6c6f 6720 6669 6c65 2e0a 2020 2020  e log file..    
+00007530: 2020 2020 2020 2020 6c6f 6766 696c 6520          logfile 
+00007540: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00007550: 2054 6865 206c 6f67 2066 696c 6520 6f66   The log file of
+00007560: 2074 6865 2053 6c75 726d 206a 6f62 2e20   the Slurm job. 
+00007570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007580: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
+00007590: 2c20 6120 6465 6661 756c 7420 6c6f 6720  , a default log 
+000075a0: 6669 6c65 2077 696c 6c20 6265 2075 7365  file will be use
+000075b0: 642e 0a0a 2020 2020 2020 2020 5265 7475  d...        Retu
+000075c0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+000075d0: 2052 6573 756c 743a 2054 6865 2072 6573   Result: The res
+000075e0: 756c 7420 6f66 2074 6865 2063 6c65 616e  ult of the clean
+000075f0: 7570 206f 7065 7261 7469 6f6e 2e0a 0a20  up operation... 
+00007600: 2020 2020 2020 204e 6f74 653a 0a20 2020         Note:.   
+00007610: 2020 2020 2020 2020 2054 6865 2063 6c65           The cle
+00007620: 616e 7570 2070 726f 6365 7373 2069 6e76  anup process inv
+00007630: 6f6c 7665 7320 7265 6d6f 7669 6e67 2074  olves removing t
+00007640: 6865 2073 7065 6369 6669 6564 207a 6970  he specified zip
+00007650: 2066 696c 652c 200a 2020 2020 2020 2020   file, .        
+00007660: 2020 2020 7468 6520 6c6f 6720 6669 6c65      the log file
+00007670: 2c20 616e 6420 6173 736f 6369 6174 6564  , and associated
+00007680: 2064 6174 6120 6669 6c65 7320 616e 6420   data files and 
+00007690: 666f 6c64 6572 732e 0a0a 2020 2020 2020  folders...      
+000076a0: 2020 4578 616d 706c 653a 0a20 2020 2020    Example:.     
+000076b0: 2020 2020 2020 2023 2043 6c65 616e 7570         # Cleanup
+000076c0: 2074 656d 706f 7261 7279 2066 696c 6573   temporary files
+000076d0: 2066 6f72 2061 2053 6c75 726d 206a 6f62   for a Slurm job
+000076e0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
+000076f0: 656e 742e 636c 6561 6e75 705f 746d 705f  ent.cleanup_tmp_
+00007700: 6669 6c65 7328 2231 3233 3435 222c 2022  files("12345", "
+00007710: 6f75 7470 7574 2e7a 6970 2229 0a20 2020  output.zip").   
+00007720: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007730: 2063 6d64 7320 3d20 5b5d 0a20 2020 2020   cmds = [].     
+00007740: 2020 2023 207a 6970 0a20 2020 2020 2020     # zip.       
+00007750: 2069 6620 6669 6c65 6e61 6d65 3a0a 2020   if filename:.  
+00007760: 2020 2020 2020 2020 2020 726d 7a69 7020            rmzip 
+00007770: 3d20 6622 726d 205c 227b 6669 6c65 6e61  = f"rm \"{filena
+00007780: 6d65 7d5c 222e 2a22 0a20 2020 2020 2020  me}\".*".       
+00007790: 2020 2020 2063 6d64 732e 6170 7065 6e64       cmds.append
+000077a0: 2872 6d7a 6970 290a 2020 2020 2020 2020  (rmzip).        
+000077b0: 2320 6c6f 670a 2020 2020 2020 2020 6966  # log.        if
+000077c0: 206c 6f67 6669 6c65 2069 7320 4e6f 6e65   logfile is None
+000077d0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
+000077e0: 6766 696c 6520 3d20 7365 6c66 2e5f 4c4f  gfile = self._LO
+000077f0: 4746 494c 450a 2020 2020 2020 2020 2020  GFILE.          
+00007800: 2020 6c6f 6766 696c 6520 3d20 6c6f 6766    logfile = logf
+00007810: 696c 652e 666f 726d 6174 2873 6c75 726d  ile.format(slurm
+00007820: 5f6a 6f62 5f69 643d 736c 7572 6d5f 6a6f  _job_id=slurm_jo
+00007830: 625f 6964 290a 2020 2020 2020 2020 726d  b_id).        rm
+00007840: 6c6f 6720 3d20 6622 726d 205c 227b 6c6f  log = f"rm \"{lo
+00007850: 6766 696c 657d 5c22 220a 2020 2020 2020  gfile}\"".      
+00007860: 2020 636d 6473 2e61 7070 656e 6428 726d    cmds.append(rm
+00007870: 6c6f 6729 0a20 2020 2020 2020 2023 2063  log).        # c
+00007880: 6f6e 7665 7274 6572 206c 6f67 730a 2020  onverter logs.  
+00007890: 2020 2020 2020 636c 6f67 203d 2073 656c        clog = sel
+000078a0: 662e 5f43 4f4e 5645 5254 4552 5f4c 4f47  f._CONVERTER_LOG
+000078b0: 4649 4c45 0a20 2020 2020 2020 2063 6c6f  FILE.        clo
+000078c0: 6720 3d20 636c 6f67 2e66 6f72 6d61 7428  g = clog.format(
+000078d0: 736c 7572 6d5f 6a6f 625f 6964 3d73 6c75  slurm_job_id=slu
+000078e0: 726d 5f6a 6f62 5f69 6429 0a20 2020 2020  rm_job_id).     
+000078f0: 2020 2072 6d63 6c6f 6720 3d20 6622 726d     rmclog = f"rm
+00007900: 207b 636c 6f67 7d22 0a20 2020 2020 2020   {clog}".       
+00007910: 2063 6d64 732e 6170 7065 6e64 2872 6d63   cmds.append(rmc
+00007920: 6c6f 6729 0a20 2020 2020 2020 200a 2020  log).        .  
+00007930: 2020 2020 2020 2320 6461 7461 0a20 2020        # data.   
+00007940: 2020 2020 2069 6620 6461 7461 5f6c 6f63       if data_loc
+00007950: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
+00007960: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+00007970: 6c6f 6361 7469 6f6e 203d 2073 656c 662e  location = self.
+00007980: 6578 7472 6163 745f 6461 7461 5f6c 6f63  extract_data_loc
+00007990: 6174 696f 6e5f 6672 6f6d 5f6c 6f67 286c  ation_from_log(l
+000079a0: 6f67 6669 6c65 290a 2020 2020 2020 2020  ogfile).        
+000079b0: 2020 2020 0a20 2020 2020 2020 2069 6620      .        if 
+000079c0: 6461 7461 5f6c 6f63 6174 696f 6e3a 0a20  data_location:. 
+000079d0: 2020 2020 2020 2020 2020 2072 6d64 6174             rmdat
+000079e0: 6120 3d20 6622 726d 202d 7266 205c 227b  a = f"rm -rf \"{
+000079f0: 6461 7461 5f6c 6f63 6174 696f 6e7d 5c22  data_location}\"
+00007a00: 205c 227b 6461 7461 5f6c 6f63 6174 696f   \"{data_locatio
+00007a10: 6e7d 5c22 2e2a 220a 2020 2020 2020 2020  n}\".*".        
+00007a20: 2020 2020 636d 6473 2e61 7070 656e 6428      cmds.append(
+00007a30: 726d 6461 7461 290a 2020 2020 2020 2020  rmdata).        
+00007a40: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00007a50: 2023 2063 6f6e 7665 7274 2063 6f6e 6669   # convert confi
+00007a60: 6720 6669 6c65 0a20 2020 2020 2020 2020  g file.         
+00007a70: 2020 2063 6f6e 6669 675f 6669 6c65 203d     config_file =
+00007a80: 2066 2263 6f6e 6669 675f 7b6f 732e 7061   f"config_{os.pa
+00007a90: 7468 2e62 6173 656e 616d 6528 6461 7461  th.basename(data
+00007aa0: 5f6c 6f63 6174 696f 6e29 7d2e 7478 7422  _location)}.txt"
+00007ab0: 0a20 2020 2020 2020 2020 2020 2072 6d63  .            rmc
+00007ac0: 6f6e 6669 6720 3d20 6622 726d 205c 227b  onfig = f"rm \"{
+00007ad0: 636f 6e66 6967 5f66 696c 657d 5c22 220a  config_file}\"".
+00007ae0: 2020 2020 2020 2020 2020 2020 636d 6473              cmds
+00007af0: 2e61 7070 656e 6428 726d 636f 6e66 6967  .append(rmconfig
+00007b00: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00007b10: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00007b20: 6572 2e77 6172 6e69 6e67 2866 2243 6f75  er.warning(f"Cou
+00007b30: 6c64 206e 6f74 2065 7874 7261 6374 2064  ld not extract d
+00007b40: 6174 6120 6c6f 6361 7469 6f6e 2066 726f  ata location fro
+00007b50: 6d20 6c6f 6720 7b6c 6f67 6669 6c65 7d2e  m log {logfile}.
+00007b60: 2053 6b69 7070 696e 6720 636c 6561 6e75   Skipping cleanu
+00007b70: 702e 2229 0a0a 2020 2020 2020 2020 7472  p.")..        tr
+00007b80: 793a 0a20 2020 2020 2020 2020 2020 2023  y:.            #
+00007b90: 2064 6f20 6173 206d 7563 6820 6173 2070   do as much as p
+00007ba0: 6f73 7369 626c 652c 206e 6f74 2063 6f6e  ossible, not con
+00007bb0: 6469 7469 6f6e 616c 2072 656d 6f76 616c  ditional removal
+00007bc0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00007bd0: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
+00007be0: 6f6d 6d61 6e64 7328 636d 6473 2c20 7365  ommands(cmds, se
+00007bf0: 703d 2720 3b20 2729 0a20 2020 2020 2020  p=' ; ').       
+00007c00: 2065 7863 6570 7420 556e 6578 7065 6374   except Unexpect
+00007c10: 6564 4578 6974 2061 7320 653a 0a20 2020  edExit as e:.   
+00007c20: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00007c30: 7761 726e 696e 6728 6529 0a20 2020 2020  warning(e).     
+00007c40: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00007c50: 652e 7265 7375 6c74 0a20 2020 2020 2020  e.result.       
+00007c60: 2072 6574 7572 6e20 7265 7375 6c74 206f   return result o
+00007c70: 7220 4e6f 6e65 0a0a 2020 2020 6465 6620  r None..    def 
+00007c80: 7661 6c69 6461 7465 2873 656c 662c 2076  validate(self, v
+00007c90: 616c 6964 6174 655f 736c 7572 6d5f 7365  alidate_slurm_se
+00007ca0: 7475 703a 2062 6f6f 6c20 3d20 4661 6c73  tup: bool = Fals
+00007cb0: 6529 3a0a 2020 2020 2020 2020 2222 2256  e):.        """V
+00007cc0: 616c 6964 6174 6520 7468 6520 636f 6e6e  alidate the conn
+00007cd0: 6563 7469 6f6e 2074 6f20 7468 6520 536c  ection to the Sl
+00007ce0: 7572 6d20 636c 7573 7465 7220 6279 2072  urm cluster by r
+00007cf0: 756e 6e69 6e67 0a20 2020 2020 2020 2061  unning.        a
+00007d00: 2073 696d 706c 6520 636f 6d6d 616e 642e   simple command.
+00007d10: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00007d20: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
+00007d30: 6461 7465 5f73 6c75 726d 5f73 6574 7570  date_slurm_setup
+00007d40: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
+00007d50: 2074 6f20 616c 736f 2063 6865 636b 0a20   to also check. 
+00007d60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00007d70: 6e64 2066 6978 2074 6865 2053 6c75 726d  nd fix the Slurm
+00007d80: 2073 6574 7570 2028 666f 6c64 6572 732c   setup (folders,
+00007d90: 2069 6d61 6765 732c 2065 7463 2e29 0a0a   images, etc.)..
+00007da0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00007db0: 0a20 2020 2020 2020 2020 2020 2062 6f6f  .            boo
+00007dc0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+00007dd0: 2020 2054 7275 6520 6966 2074 6865 2076     True if the v
+00007de0: 616c 6964 6174 696f 6e20 6973 2073 7563  alidation is suc
+00007df0: 6365 7373 6675 6c2c 0a20 2020 2020 2020  cessful,.       
+00007e00: 2020 2020 2020 2020 2046 616c 7365 206f           False o
+00007e10: 7468 6572 7769 7365 2e0a 2020 2020 2020  therwise..      
+00007e20: 2020 2222 220a 2020 2020 2020 2020 636f    """.        co
+00007e30: 6e6e 6563 7465 6420 3d20 7365 6c66 2e72  nnected = self.r
+00007e40: 756e 2827 6563 686f 2022 2022 2729 2e6f  un('echo " "').o
+00007e50: 6b0a 2020 2020 2020 2020 6966 2063 6f6e  k.        if con
+00007e60: 6e65 6374 6564 2061 6e64 2076 616c 6964  nected and valid
+00007e70: 6174 655f 736c 7572 6d5f 7365 7475 703a  ate_slurm_setup:
+00007e80: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
+00007e90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00007ea0: 2020 7365 6c66 2e73 6574 7570 5f73 6c75    self.setup_slu
+00007eb0: 726d 2829 0a20 2020 2020 2020 2020 2020  rm().           
+00007ec0: 2065 7863 6570 7420 5353 4845 7863 6570   except SSHExcep
+00007ed0: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+00007ee0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00007ef0: 722e 6572 726f 7228 6529 0a20 2020 2020  r.error(e).     
+00007f00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00007f10: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+00007f20: 7265 7475 726e 2063 6f6e 6e65 6374 6564  return connected
+00007f30: 0a0a 2020 2020 6465 6620 6765 745f 7265  ..    def get_re
+00007f40: 6365 6e74 5f6c 6f67 5f63 6f6d 6d61 6e64  cent_log_command
+00007f50: 2873 656c 662c 206c 6f67 5f66 696c 653a  (self, log_file:
+00007f60: 2073 7472 2c20 6e3a 2069 6e74 203d 2031   str, n: int = 1
+00007f70: 3029 202d 3e20 7374 723a 0a20 2020 2020  0) -> str:.     
+00007f80: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+00007f90: 6574 2074 6865 2063 6f6d 6d61 6e64 2074  et the command t
+00007fa0: 6f20 7265 7472 6965 7665 2074 6865 2072  o retrieve the r
+00007fb0: 6563 656e 7420 6c6f 6720 656e 7472 6965  ecent log entrie
+00007fc0: 7320 6672 6f6d 2061 0a20 2020 2020 2020  s from a.       
+00007fd0: 2073 7065 6369 6669 6564 206c 6f67 2066   specified log f
+00007fe0: 696c 652e 0a0a 2020 2020 2020 2020 4172  ile...        Ar
+00007ff0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00008000: 6c6f 675f 6669 6c65 2028 7374 7229 3a20  log_file (str): 
+00008010: 5468 6520 7061 7468 2074 6f20 7468 6520  The path to the 
+00008020: 6c6f 6720 6669 6c65 2e0a 2020 2020 2020  log file..      
+00008030: 2020 2020 2020 6e20 2869 6e74 2c20 6f70        n (int, op
+00008040: 7469 6f6e 616c 293a 2054 6865 206e 756d  tional): The num
+00008050: 6265 7220 6f66 2072 6563 656e 7420 6c6f  ber of recent lo
+00008060: 6720 656e 7472 6965 7320 746f 2072 6574  g entries to ret
+00008070: 7269 6576 652e 0a20 2020 2020 2020 2020  rieve..         
+00008080: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00008090: 746f 2031 302e 0a0a 2020 2020 2020 2020  to 10...        
+000080a0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+000080b0: 2020 2020 2073 7472 3a20 5468 6520 636f       str: The co
+000080c0: 6d6d 616e 6420 746f 2072 6574 7269 6576  mmand to retriev
+000080d0: 6520 7468 6520 7265 6365 6e74 206c 6f67  e the recent log
+000080e0: 2065 6e74 7269 6573 2e0a 2020 2020 2020   entries..      
+000080f0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00008100: 7475 726e 2073 656c 662e 5f54 4149 4c5f  turn self._TAIL_
+00008110: 4c4f 475f 434d 442e 666f 726d 6174 286e  LOG_CMD.format(n
+00008120: 3d6e 2c20 6c6f 675f 6669 6c65 3d6c 6f67  =n, log_file=log
+00008130: 5f66 696c 6529 0a0a 2020 2020 6465 6620  _file)..    def 
+00008140: 6765 745f 6163 7469 7665 5f6a 6f62 5f70  get_active_job_p
+00008150: 726f 6772 6573 7328 7365 6c66 2c0a 2020  rogress(self,.  
+00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008170: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+00008180: 7572 6d5f 6a6f 625f 6964 3a20 7374 722c  urm_job_id: str,
+00008190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081b0: 2070 6174 7465 726e 3a20 7374 7220 3d20   pattern: str = 
+000081c0: 7222 5c64 2b25 222c 0a20 2020 2020 2020  r"\d+%",.       
+000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081e0: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
+000081f0: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00008200: 2073 7472 5d5d 203d 204e 6f6e 6529 202d   str]] = None) -
+00008210: 3e20 7374 723a 0a20 2020 2020 2020 2022  > str:.        "
+00008220: 2222 0a20 2020 2020 2020 2047 6574 2074  "".        Get t
+00008230: 6865 2070 726f 6772 6573 7320 6f66 2061  he progress of a
+00008240: 6e20 6163 7469 7665 2053 6c75 726d 206a  n active Slurm j
+00008250: 6f62 2066 726f 6d20 6974 7320 6c6f 6766  ob from its logf
+00008260: 696c 6573 2e0a 0a20 2020 2020 2020 2041  iles...        A
+00008270: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00008280: 2073 6c75 726d 5f6a 6f62 5f69 6420 2873   slurm_job_id (s
+00008290: 7472 293a 2054 6865 2049 4420 6f66 2074  tr): The ID of t
+000082a0: 6865 2053 6c75 726d 206a 6f62 2e0a 2020  he Slurm job..  
+000082b0: 2020 2020 2020 2020 2020 7061 7474 6572            patter
+000082c0: 6e20 2873 7472 293a 2054 6865 2070 6174  n (str): The pat
+000082d0: 7465 726e 2074 6f20 6d61 7463 6820 696e  tern to match in
+000082e0: 2074 6865 206a 6f62 206c 6f67 2074 6f20   the job log to 
+000082f0: 6578 7472 6163 740a 2020 2020 2020 2020  extract.        
+00008300: 2020 2020 2020 2020 7468 6520 7072 6f67          the prog
+00008310: 7265 7373 2028 6465 6661 756c 743a 2072  ress (default: r
+00008320: 225c 642b 2522 292e 0a0a 2020 2020 2020  "\d+%")...      
+00008330: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
+00008340: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
+00008350: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
+00008360: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00008370: 626c 6573 200a 2020 2020 2020 2020 2020  bles .          
+00008380: 2020 2020 2020 746f 2073 6574 2077 6865        to set whe
+00008390: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
+000083a0: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
+000083b0: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
+000083c0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+000083d0: 2020 2020 2020 2073 7472 3a20 5468 6520         str: The 
+000083e0: 7072 6f67 7265 7373 206f 6620 7468 6520  progress of the 
+000083f0: 536c 7572 6d20 6a6f 622e 0a20 2020 2020  Slurm job..     
+00008400: 2020 2022 2222 0a20 2020 2020 2020 2063     """.        c
+00008410: 6d64 6c69 7374 203d 205b 5d0a 2020 2020  mdlist = [].    
+00008420: 2020 2020 636d 6420 3d20 7365 6c66 2e67      cmd = self.g
+00008430: 6574 5f72 6563 656e 745f 6c6f 675f 636f  et_recent_log_co
+00008440: 6d6d 616e 6428 0a20 2020 2020 2020 2020  mmand(.         
+00008450: 2020 206c 6f67 5f66 696c 653d 7365 6c66     log_file=self
+00008460: 2e5f 4c4f 4746 494c 452e 666f 726d 6174  ._LOGFILE.format
+00008470: 2873 6c75 726d 5f6a 6f62 5f69 643d 736c  (slurm_job_id=sl
+00008480: 7572 6d5f 6a6f 625f 6964 2929 0a20 2020  urm_job_id)).   
+00008490: 2020 2020 2063 6d64 6c69 7374 2e61 7070       cmdlist.app
+000084a0: 656e 6428 636d 6429 0a20 2020 2020 2020  end(cmd).       
+000084b0: 2069 6620 656e 7620 6973 204e 6f6e 653a   if env is None:
+000084c0: 0a20 2020 2020 2020 2020 2020 2065 6e76  .            env
+000084d0: 203d 207b 7d0a 2020 2020 2020 2020 7472   = {}.        tr
+000084e0: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
+000084f0: 6573 756c 7420 3d20 7365 6c66 2e72 756e  esult = self.run
+00008500: 5f63 6f6d 6d61 6e64 7328 636d 646c 6973  _commands(cmdlis
+00008510: 742c 2065 6e76 3d65 6e76 290a 2020 2020  t, env=env).    
+00008520: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
+00008530: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
+00008540: 2020 2020 2020 206c 6f67 6765 722e 6572         logger.er
+00008550: 726f 7228 6622 4973 7375 6520 7769 7468  ror(f"Issue with
+00008560: 2072 756e 2063 6f6d 6d61 6e64 3a20 7b65   run command: {e
+00008570: 7d22 290a 2020 2020 2020 2020 2320 4d61  }").        # Ma
+00008580: 7463 6820 7468 6520 7370 6563 6966 6965  tch the specifie
+00008590: 6420 7061 7474 6572 6e20 696e 2074 6865  d pattern in the
+000085a0: 2072 6573 756c 7427 7320 7374 646f 7574   result's stdout
+000085b0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+000085c0: 2020 2020 2020 2020 2020 6c61 7465 7374            latest
+000085d0: 5f70 726f 6772 6573 7320 3d20 7265 2e66  _progress = re.f
+000085e0: 696e 6461 6c6c 280a 2020 2020 2020 2020  indall(.        
+000085f0: 2020 2020 2020 2020 7061 7474 6572 6e2c          pattern,
+00008600: 2072 6573 756c 742e 7374 646f 7574 295b   result.stdout)[
+00008610: 2d31 5d0a 2020 2020 2020 2020 6578 6365  -1].        exce
+00008620: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
+00008630: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
+00008640: 6f67 6765 722e 6572 726f 7228 6622 4973  ogger.error(f"Is
+00008650: 7375 6520 7769 7468 2065 7874 7261 6374  sue with extract
+00008660: 696e 6720 7072 6f67 7265 7373 3a20 7b65  ing progress: {e
+00008670: 7d22 290a 0a20 2020 2020 2020 2072 6574  }")..        ret
+00008680: 7572 6e20 6622 5072 6f67 7265 7373 3a20  urn f"Progress: 
+00008690: 7b6c 6174 6573 745f 7072 6f67 7265 7373  {latest_progress
+000086a0: 7d5c 6e22 0a0a 2020 2020 6465 6620 7275  }\n"..    def ru
+000086b0: 6e5f 636f 6d6d 616e 6473 2873 656c 662c  n_commands(self,
+000086c0: 2063 6d64 6c69 7374 3a20 4c69 7374 5b73   cmdlist: List[s
+000086d0: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
+000086e0: 2020 2020 2020 2020 2020 656e 763a 204f            env: O
+000086f0: 7074 696f 6e61 6c5b 4469 6374 5b73 7472  ptional[Dict[str
+00008700: 2c20 7374 725d 5d20 3d20 4e6f 6e65 2c0a  , str]] = None,.
+00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008720: 2020 2020 2073 6570 3a20 7374 7220 3d20       sep: str = 
+00008730: 2720 2626 2027 2c0a 2020 2020 2020 2020  ' && ',.        
+00008740: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
+00008750: 7761 7267 7329 202d 3e20 5265 7375 6c74  wargs) -> Result
+00008760: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00008770: 2020 2020 2020 5275 6e20 6120 6c69 7374        Run a list
+00008780: 206f 6620 7368 656c 6c20 636f 6d6d 616e   of shell comman
+00008790: 6473 2063 6f6e 7365 6375 7469 7665 6c79  ds consecutively
+000087a0: 206f 6e20 7468 6520 536c 7572 6d20 636c   on the Slurm cl
+000087b0: 7573 7465 722c 0a20 2020 2020 2020 2065  uster,.        e
+000087c0: 6e73 7572 696e 6720 7468 6520 7375 6363  nsuring the succ
+000087d0: 6573 7320 6f66 2065 6163 6820 6265 666f  ess of each befo
+000087e0: 7265 2070 726f 6365 6564 696e 6720 746f  re proceeding to
+000087f0: 2074 6865 206e 6578 742e 0a0a 2020 2020   the next...    
+00008800: 2020 2020 5468 6520 656e 7669 726f 6e6d      The environm
+00008810: 656e 7420 7661 7269 6162 6c65 7320 6361  ent variables ca
+00008820: 6e20 6265 2073 6574 2075 7369 6e67 2074  n be set using t
+00008830: 6865 2060 656e 7660 2061 7267 756d 656e  he `env` argumen
+00008840: 742e 0a20 2020 2020 2020 2054 6865 7365  t..        These
+00008850: 2063 6f6d 6d61 6e64 7320 7265 7461 696e   commands retain
+00008860: 2074 6865 2073 616d 6520 7365 7373 696f   the same sessio
+00008870: 6e20 2865 6e76 6972 6f6e 6d65 6e74 2076  n (environment v
+00008880: 6172 6961 626c 6573 0a20 2020 2020 2020  ariables.       
+00008890: 2065 7463 2e29 2c20 756e 6c69 6b65 2072   etc.), unlike r
+000088a0: 756e 6e69 6e67 2074 6865 6d20 7365 7061  unning them sepa
+000088b0: 7261 7465 6c79 2e0a 0a20 2020 2020 2020  rately...       
+000088c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+000088d0: 2020 2063 6d64 6c69 7374 2028 4c69 7374     cmdlist (List
+000088e0: 5b73 7472 5d29 3a20 4120 6c69 7374 206f  [str]): A list o
+000088f0: 6620 7368 656c 6c20 636f 6d6d 616e 6473  f shell commands
+00008900: 2074 6f20 7275 6e20 6f6e 2053 6c75 726d   to run on Slurm
+00008910: 2e0a 2020 2020 2020 2020 2020 2020 656e  ..            en
+00008920: 7620 2844 6963 745b 7374 722c 2073 7472  v (Dict[str, str
+00008930: 5d2c 206f 7074 696f 6e61 6c29 3a20 4f70  ], optional): Op
+00008940: 7469 6f6e 616c 2065 6e76 6972 6f6e 6d65  tional environme
+00008950: 6e74 2076 6172 6961 626c 6573 2074 6f0a  nt variables to.
+00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008970: 7365 7420 7768 656e 2072 756e 6e69 6e67  set when running
+00008980: 2074 6865 2063 6f6d 6d61 6e64 2e20 4465   the command. De
+00008990: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
+000089a0: 2020 2020 2020 2020 2020 2020 7365 7020              sep 
+000089b0: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+000089c0: 2054 6865 2073 6570 6172 6174 6f72 2075   The separator u
+000089d0: 7365 6420 746f 2063 6f6e 6361 7465 6e61  sed to concatena
+000089e0: 7465 2074 6865 200a 2020 2020 2020 2020  te the .        
+000089f0: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
+00008a00: 2e20 4465 6661 756c 7473 2074 6f20 2720  . Defaults to ' 
+00008a10: 2626 2027 2e0a 2020 2020 2020 2020 2020  && '..          
+00008a20: 2020 2a2a 6b77 6172 6773 3a20 4164 6469    **kwargs: Addi
+00008a30: 7469 6f6e 616c 206b 6579 776f 7264 2061  tional keyword a
+00008a40: 7267 756d 656e 7473 2e0a 0a20 2020 2020  rguments...     
+00008a50: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00008a60: 2020 2020 2020 2020 5265 7375 6c74 3a20          Result: 
+00008a70: 5468 6520 7265 7375 6c74 206f 6620 7468  The result of th
+00008a80: 6520 6c61 7374 2063 6f6d 6d61 6e64 2069  e last command i
+00008a90: 6e20 7468 6520 6c69 7374 2e0a 2020 2020  n the list..    
+00008aa0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008ab0: 6966 2065 6e76 2069 7320 4e6f 6e65 3a0a  if env is None:.
+00008ac0: 2020 2020 2020 2020 2020 2020 656e 7620              env 
+00008ad0: 3d20 7b7d 0a20 2020 2020 2020 2063 6d64  = {}.        cmd
+00008ae0: 203d 2073 6570 2e6a 6f69 6e28 636d 646c   = sep.join(cmdl
+00008af0: 6973 7429 0a20 2020 2020 2020 206c 6f67  ist).        log
+00008b00: 6765 722e 696e 666f 280a 2020 2020 2020  ger.info(.      
+00008b10: 2020 2020 2020 6622 5275 6e6e 696e 6720        f"Running 
+00008b20: 636f 6d6d 616e 6473 2c20 7769 7468 2065  commands, with e
+00008b30: 6e76 207b 656e 767d 2061 6e64 2073 6570  nv {env} and sep
+00008b40: 207b 7365 707d 205c 0a20 2020 2020 2020   {sep} \.       
+00008b50: 2020 2020 2020 2020 2061 6e64 207b 6b77           and {kw
+00008b60: 6172 6773 7d3a 207b 636d 647d 2229 0a20  args}: {cmd}"). 
+00008b70: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00008b80: 7365 6c66 2e72 756e 2863 6d64 2c20 656e  self.run(cmd, en
+00008b90: 763d 656e 762c 202a 2a6b 7761 7267 7329  v=env, **kwargs)
+00008ba0: 2020 2320 6f75 745f 7374 7265 616d 3d6f    # out_stream=o
+00008bb0: 7574 5f73 7472 6561 6d2c 0a0a 2020 2020  ut_stream,..    
+00008bc0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+00008bd0: 2020 2020 2023 2057 6174 6368 206f 7574       # Watch out
+00008be0: 2066 6f72 2055 6e69 636f 6465 456e 636f   for UnicodeEnco
+00008bf0: 6465 4572 726f 7220 7768 656e 2079 6f75  deError when you
+00008c00: 2073 7472 2829 2074 6869 732e 0a20 2020   str() this..   
+00008c10: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00008c20: 696e 666f 2866 227b 7265 7375 6c74 2e73  info(f"{result.s
+00008c30: 7464 6f75 747d 2229 0a20 2020 2020 2020  tdout}").       
+00008c40: 2065 7863 6570 7420 556e 6963 6f64 6545   except UnicodeE
+00008c50: 6e63 6f64 6545 7272 6f72 2061 7320 653a  ncodeError as e:
+00008c60: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00008c70: 6765 722e 6572 726f 7228 6622 556e 6963  ger.error(f"Unic
+00008c80: 6f64 6520 6572 726f 723a 207b 657d 2229  ode error: {e}")
+00008c90: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00008ca0: 4f44 4f3a 204f 4e4c 5920 7374 646f 7574  ODO: ONLY stdout
+00008cb0: 2052 4543 4f44 4520 4e45 4544 4544 3f3f   RECODE NEEDED??
+00008cc0: 206f 7220 616c 736f 2065 7272 6f72 3f0a   or also error?.
+00008cd0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00008ce0: 6c74 2e73 7464 6f75 7420 3d20 7265 7375  lt.stdout = resu
+00008cf0: 6c74 2e73 7464 6f75 742e 656e 636f 6465  lt.stdout.encode
+00008d00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00008d10: 2020 2775 7466 2d38 272c 2027 6967 6e6f    'utf-8', 'igno
+00008d20: 7265 2729 2e64 6563 6f64 6528 2775 7466  re').decode('utf
+00008d30: 2d38 2729 0a20 2020 2020 2020 2072 6574  -8').        ret
+00008d40: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
+00008d50: 6465 6620 7374 725f 746f 5f63 6c61 7373  def str_to_class
+00008d60: 2873 656c 662c 206d 6f64 756c 655f 6e61  (self, module_na
+00008d70: 6d65 3a20 7374 722c 2063 6c61 7373 5f6e  me: str, class_n
+00008d80: 616d 653a 2073 7472 2c20 2a61 7267 732c  ame: str, *args,
+00008d90: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
+00008da0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00008db0: 5265 7475 726e 2061 2063 6c61 7373 2069  Return a class i
+00008dc0: 6e73 7461 6e63 6520 6672 6f6d 2061 2073  nstance from a s
+00008dd0: 7472 696e 6720 7265 6665 7265 6e63 652e  tring reference.
+00008de0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00008df0: 2020 2020 2020 2020 2020 2020 6d6f 6475              modu
+00008e00: 6c65 5f6e 616d 6520 2873 7472 293a 2054  le_name (str): T
+00008e10: 6865 206e 616d 6520 6f66 2074 6865 206d  he name of the m
+00008e20: 6f64 756c 652e 0a20 2020 2020 2020 2020  odule..         
+00008e30: 2020 2063 6c61 7373 5f6e 616d 6520 2873     class_name (s
+00008e40: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
+00008e50: 2074 6865 2063 6c61 7373 2e0a 2020 2020   the class..    
+00008e60: 2020 2020 2020 2020 2a61 7267 733a 2041          *args: A
+00008e70: 6464 6974 696f 6e61 6c20 706f 7369 7469  dditional positi
+00008e80: 6f6e 616c 2061 7267 756d 656e 7473 2066  onal arguments f
+00008e90: 6f72 2074 6865 2063 6c61 7373 2063 6f6e  or the class con
+00008ea0: 7374 7275 6374 6f72 2e0a 2020 2020 2020  structor..      
+00008eb0: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
+00008ec0: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
+00008ed0: 7264 2061 7267 756d 656e 7473 2066 6f72  rd arguments for
+00008ee0: 2074 6865 2063 6c61 7373 2063 6f6e 7374   the class const
+00008ef0: 7275 6374 6f72 2e0a 0a20 2020 2020 2020  ructor...       
+00008f00: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00008f10: 2020 2020 2020 6f62 6a65 6374 3a20 416e        object: An
+00008f20: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
+00008f30: 2073 7065 6369 6669 6564 2063 6c61 7373   specified class
+00008f40: 2c20 6f72 204e 6f6e 6520 6966 2074 6865  , or None if the
+00008f50: 2063 6c61 7373 206f 720a 2020 2020 2020   class or.      
+00008f60: 2020 2020 2020 2020 2020 6d6f 6475 6c65            module
+00008f70: 2064 6f65 7320 6e6f 7420 6578 6973 742e   does not exist.
+00008f80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00008f90: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00008fa0: 2020 2020 2020 6d6f 6475 6c65 5f20 3d20        module_ = 
+00008fb0: 696d 706f 7274 6c69 622e 696d 706f 7274  importlib.import
+00008fc0: 5f6d 6f64 756c 6528 6d6f 6475 6c65 5f6e  _module(module_n
+00008fd0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
+00008fe0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00008ff0: 2020 2020 2020 636c 6173 735f 203d 2067        class_ = g
+00009000: 6574 6174 7472 286d 6f64 756c 655f 2c20  etattr(module_, 
+00009010: 636c 6173 735f 6e61 6d65 2928 2a61 7267  class_name)(*arg
+00009020: 732c 202a 2a6b 7761 7267 7329 0a20 2020  s, **kwargs).   
+00009030: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00009040: 4174 7472 6962 7574 6545 7272 6f72 3a0a  AttributeError:.
+00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009060: 6c6f 6767 6572 2e65 7272 6f72 2827 436c  logger.error('Cl
+00009070: 6173 7320 646f 6573 206e 6f74 2065 7869  ass does not exi
+00009080: 7374 2729 0a20 2020 2020 2020 2065 7863  st').        exc
+00009090: 6570 7420 496d 706f 7274 4572 726f 723a  ept ImportError:
+000090a0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+000090b0: 6765 722e 6572 726f 7228 274d 6f64 756c  ger.error('Modul
+000090c0: 6520 646f 6573 206e 6f74 2065 7869 7374  e does not exist
+000090d0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
+000090e0: 6e20 636c 6173 735f 206f 7220 4e6f 6e65  n class_ or None
+000090f0: 0a0a 2020 2020 6465 6620 7275 6e5f 636f  ..    def run_co
+00009100: 6d6d 616e 6473 5f73 706c 6974 5f6f 7574  mmands_split_out
+00009110: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+00009120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009130: 2020 2020 2020 636d 646c 6973 743a 204c        cmdlist: L
+00009140: 6973 745b 7374 725d 2c0a 2020 2020 2020  ist[str],.      
+00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009160: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
+00009170: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00009180: 2073 7472 5d5d 203d 204e 6f6e 650a 2020   str]] = None.  
+00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091a0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+000091b0: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
+000091c0: 2020 2020 2022 2222 5275 6e20 6120 6c69       """Run a li
+000091d0: 7374 206f 6620 7368 656c 6c20 636f 6d6d  st of shell comm
+000091e0: 616e 6473 2063 6f6e 7365 6375 7469 7665  ands consecutive
+000091f0: 6c79 2061 6e64 2073 706c 6974 2074 6865  ly and split the
+00009200: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
+00009210: 6f66 2065 6163 6820 636f 6d6d 616e 642e  of each command.
+00009220: 0a0a 2020 2020 2020 2020 4561 6368 2063  ..        Each c
+00009230: 6f6d 6d61 6e64 2069 6e20 7468 6520 6c69  ommand in the li
+00009240: 7374 2069 7320 6578 6563 7574 6564 2077  st is executed w
+00009250: 6974 6820 6120 7365 7061 7261 746f 7220  ith a separator 
+00009260: 696e 2062 6574 7765 656e 0a20 2020 2020  in between.     
+00009270: 2020 2074 6861 7420 6973 2075 6e69 7175     that is uniqu
+00009280: 6520 616e 6420 6361 6e20 6265 2075 7365  e and can be use
+00009290: 6420 746f 2073 706c 6974 0a20 2020 2020  d to split.     
+000092a0: 2020 2074 6865 206f 7574 7075 7420 6f66     the output of
+000092b0: 2065 6163 6820 636f 6d6d 616e 6420 6c61   each command la
+000092c0: 7465 722e 2054 6865 2073 6570 6172 6174  ter. The separat
+000092d0: 6f72 2075 7365 6420 6973 2073 7065 6369  or used is speci
+000092e0: 6669 6564 0a20 2020 2020 2020 2062 7920  fied.        by 
+000092f0: 7468 6520 605f 4f55 545f 5345 5060 2061  the `_OUT_SEP` a
+00009300: 7474 7269 6275 7465 206f 6620 7468 650a  ttribute of the.
+00009310: 2020 2020 2020 2020 536c 7572 6d43 6c69          SlurmCli
+00009320: 656e 7420 696e 7374 616e 6365 2e0a 0a20  ent instance... 
+00009330: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00009340: 2020 2020 2020 2020 2063 6d64 6c69 7374           cmdlist
+00009350: 2028 4c69 7374 5b73 7472 5d29 3a20 4120   (List[str]): A 
+00009360: 6c69 7374 206f 6620 7368 656c 6c20 636f  list of shell co
+00009370: 6d6d 616e 6473 2074 6f20 7275 6e2e 0a20  mmands to run.. 
+00009380: 2020 2020 2020 2020 2020 2065 6e76 2028             env (
+00009390: 4469 6374 5b73 7472 2c20 7374 725d 2c20  Dict[str, str], 
+000093a0: 6f70 7469 6f6e 616c 293a 204f 7074 696f  optional): Optio
+000093b0: 6e61 6c20 656e 7669 726f 6e6d 656e 7420  nal environment 
+000093c0: 7661 7269 6162 6c65 7320 0a20 2020 2020  variables .     
+000093d0: 2020 2020 2020 2020 2020 2074 6f20 7365             to se
+000093e0: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
+000093f0: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
+00009400: 756c 7473 2074 6f20 4e6f 6e65 2e0a 0a20  ults to None... 
+00009410: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00009420: 2020 2020 2020 2020 2020 2020 4c69 7374              List
+00009430: 5b73 7472 5d3a 0a20 2020 2020 2020 2020  [str]:.         
+00009440: 2020 2020 2020 2041 206c 6973 7420 6f66         A list of
+00009450: 2073 7472 696e 6773 2c20 7768 6572 6520   strings, where 
+00009460: 6561 6368 2073 7472 696e 6720 636f 7272  each string corr
+00009470: 6573 706f 6e64 7320 746f 0a20 2020 2020  esponds to.     
+00009480: 2020 2020 2020 2020 2020 2074 6865 206f             the o
+00009490: 7574 7075 7420 6f66 2061 2073 696e 676c  utput of a singl
+000094a0: 6520 636f 6d6d 616e 6420 696e 2060 636d  e command in `cm
+000094b0: 646c 6973 7460 2073 706c 6974 0a20 2020  dlist` split.   
+000094c0: 2020 2020 2020 2020 2020 2020 2062 7920               by 
+000094d0: 7468 6520 7365 7061 7261 746f 7220 605f  the separator `_
+000094e0: 4f55 545f 5345 5060 2e0a 0a20 2020 2020  OUT_SEP`...     
+000094f0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
+00009500: 2020 2020 2020 2053 5348 4578 6365 7074         SSHExcept
+00009510: 696f 6e3a 2049 6620 616e 7920 6f66 2074  ion: If any of t
+00009520: 6865 2063 6f6d 6d61 6e64 7320 6661 696c  he commands fail
+00009530: 2074 6f20 6578 6563 7574 6520 7375 6363   to execute succ
+00009540: 6573 7366 756c 6c79 2e0a 2020 2020 2020  essfully..      
+00009550: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
+00009560: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
+00009570: 6573 756c 7420 3d20 7365 6c66 2e72 756e  esult = self.run
+00009580: 5f63 6f6d 6d61 6e64 7328 636d 646c 6973  _commands(cmdlis
+00009590: 743d 636d 646c 6973 742c 0a20 2020 2020  t=cmdlist,.     
+000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095c0: 2020 656e 763d 656e 762c 0a20 2020 2020    env=env,.     
+000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000095f0: 2020 7365 703d 6622 203b 2065 6368 6f20    sep=f" ; echo 
+00009600: 7b73 656c 662e 5f4f 5554 5f53 4550 7d20  {self._OUT_SEP} 
+00009610: 3b20 2229 0a20 2020 2020 2020 2065 7863  ; ").        exc
+00009620: 6570 7420 556e 6578 7065 6374 6564 4578  ept UnexpectedEx
+00009630: 6974 2061 7320 653a 0a20 2020 2020 2020  it as e:.       
+00009640: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
+00009650: 696e 6728 6529 0a20 2020 2020 2020 2020  ing(e).         
+00009660: 2020 2072 6573 756c 7420 3d20 652e 7265     result = e.re
+00009670: 7375 6c74 0a20 2020 2020 2020 2069 6620  sult.        if 
+00009680: 7265 7375 6c74 2e6f 6b3a 0a20 2020 2020  result.ok:.     
+00009690: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
+000096a0: 3d20 7265 7375 6c74 2e73 7464 6f75 740a  = result.stdout.
+000096b0: 2020 2020 2020 2020 2020 2020 7370 6c69              spli
+000096c0: 745f 7265 7370 6f6e 7365 7320 3d20 7265  t_responses = re
+000096d0: 7370 6f6e 7365 2e73 706c 6974 2873 656c  sponse.split(sel
+000096e0: 662e 5f4f 5554 5f53 4550 290a 2020 2020  f._OUT_SEP).    
+000096f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00009700: 706c 6974 5f72 6573 706f 6e73 6573 0a20  plit_responses. 
+00009710: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00009720: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
+00009730: 6520 7265 7375 6c74 2069 7320 6e6f 7420  e result is not 
+00009740: 6f6b 2c20 6c6f 6720 7468 6520 6572 726f  ok, log the erro
+00009750: 7220 616e 6420 7261 6973 6520 616e 2053  r and raise an S
+00009760: 5348 4578 6365 7074 696f 6e0a 2020 2020  SHException.    
+00009770: 2020 2020 2020 2020 6572 726f 7220 3d20          error = 
+00009780: 6622 5265 7375 6c74 2069 7320 6e6f 7420  f"Result is not 
+00009790: 6f6b 3a20 7b72 6573 756c 747d 220a 2020  ok: {result}".  
+000097a0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+000097b0: 2e65 7272 6f72 2865 7272 6f72 290a 2020  .error(error).  
+000097c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000097d0: 5353 4845 7863 6570 7469 6f6e 2865 7272  SSHException(err
+000097e0: 6f72 290a 0a20 2020 2064 6566 206c 6973  or)..    def lis
+000097f0: 745f 6163 7469 7665 5f6a 6f62 7328 7365  t_active_jobs(se
+00009800: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+00009810: 2020 2020 2020 2020 2020 2020 2065 6e76               env
+00009820: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
+00009830: 7374 722c 2073 7472 5d5d 203d 204e 6f6e  str, str]] = Non
+00009840: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
+00009850: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00009860: 2020 2020 2047 6574 2061 206c 6973 7420       Get a list 
+00009870: 6f66 2061 6374 6976 6520 6a6f 6273 2066  of active jobs f
+00009880: 726f 6d20 534c 5552 4d2e 0a0a 2020 2020  rom SLURM...    
+00009890: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+000098a0: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
+000098b0: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
+000098c0: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
+000098d0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+000098e0: 626c 6573 2074 6f20 0a20 2020 2020 2020  bles to .       
+000098f0: 2020 2020 2020 2020 2073 6574 2077 6865           set whe
+00009900: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
+00009910: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
+00009920: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
+00009930: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00009940: 2020 2020 2020 204c 6973 745b 7374 725d         List[str]
+00009950: 3a20 4120 6c69 7374 206f 6620 6a6f 6220  : A list of job 
+00009960: 4944 732e 0a20 2020 2020 2020 2022 2222  IDs..        """
+00009970: 0a20 2020 2020 2020 2023 2063 6d64 203d  .        # cmd =
+00009980: 2073 656c 662e 5f41 4354 4956 455f 4a4f   self._ACTIVE_JO
+00009990: 4253 5f43 4d44 0a20 2020 2020 2020 2063  BS_CMD.        c
+000099a0: 6d64 203d 2073 656c 662e 6765 745f 6a6f  md = self.get_jo
+000099b0: 6273 5f69 6e66 6f5f 636f 6d6d 616e 6428  bs_info_command(
+000099c0: 7374 6172 745f 7469 6d65 3d22 6e6f 7722  start_time="now"
+000099d0: 2c20 7374 6174 6573 3d22 7222 290a 2020  , states="r").  
+000099e0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+000099f0: 6f28 2252 6574 7269 6576 696e 6720 6c69  o("Retrieving li
+00009a00: 7374 206f 6620 6163 7469 7665 206a 6f62  st of active job
+00009a10: 7320 6672 6f6d 2053 6c75 726d 2229 0a20  s from Slurm"). 
+00009a20: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00009a30: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
+00009a40: 7328 5b63 6d64 5d2c 2065 6e76 3d65 6e76  s([cmd], env=env
+00009a50: 290a 2020 2020 2020 2020 6a6f 625f 6c69  ).        job_li
+00009a60: 7374 203d 2072 6573 756c 742e 7374 646f  st = result.stdo
+00009a70: 7574 2e73 7472 6970 2829 2e73 706c 6974  ut.strip().split
+00009a80: 2827 5c6e 2729 0a20 2020 2020 2020 206a  ('\n').        j
+00009a90: 6f62 5f6c 6973 742e 7265 7665 7273 6528  ob_list.reverse(
+00009aa0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00009ab0: 206a 6f62 5f6c 6973 740a 0a20 2020 2064   job_list..    d
+00009ac0: 6566 206c 6973 745f 636f 6d70 6c65 7465  ef list_complete
+00009ad0: 645f 6a6f 6273 2873 656c 662c 0a20 2020  d_jobs(self,.   
+00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009af0: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
+00009b00: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00009b10: 2073 7472 5d5d 203d 204e 6f6e 6529 202d   str]] = None) -
+00009b20: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
+00009b30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00009b40: 2047 6574 2061 206c 6973 7420 6f66 2063   Get a list of c
+00009b50: 6f6d 706c 6574 6564 206a 6f62 7320 6672  ompleted jobs fr
+00009b60: 6f6d 2053 4c55 524d 2e0a 0a20 2020 2020  om SLURM...     
+00009b70: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00009b80: 2020 2020 2065 6e76 2028 4469 6374 5b73       env (Dict[s
+00009b90: 7472 2c20 7374 725d 2c20 6f70 7469 6f6e  tr, str], option
+00009ba0: 616c 293a 204f 7074 696f 6e61 6c20 656e  al): Optional en
+00009bb0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00009bc0: 6c65 7320 746f 0a20 2020 2020 2020 2020  les to.         
+00009bd0: 2020 2020 2020 2073 6574 2077 6865 6e20         set when 
+00009be0: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
+00009bf0: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
+00009c00: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
+00009c10: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00009c20: 2020 2020 204c 6973 745b 7374 725d 3a20       List[str]: 
+00009c30: 4120 6c69 7374 206f 6620 6a6f 6220 4944  A list of job ID
+00009c40: 732e 0a20 2020 2020 2020 2022 2222 0a0a  s..        """..
+00009c50: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
+00009c60: 6c66 2e67 6574 5f6a 6f62 735f 696e 666f  lf.get_jobs_info
+00009c70: 5f63 6f6d 6d61 6e64 2873 7461 7465 733d  _command(states=
+00009c80: 2263 6422 290a 2020 2020 2020 2020 6c6f  "cd").        lo
+00009c90: 6767 6572 2e69 6e66 6f28 2252 6574 7269  gger.info("Retri
+00009ca0: 6576 696e 6720 6120 6c69 7374 206f 6620  eving a list of 
+00009cb0: 636f 6d70 6c65 7465 6420 6a6f 6273 2066  completed jobs f
+00009cc0: 726f 6d20 536c 7572 6d22 290a 2020 2020  rom Slurm").    
+00009cd0: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
+00009ce0: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
+00009cf0: 636d 645d 2c20 656e 763d 656e 7629 0a20  cmd], env=env). 
+00009d00: 2020 2020 2020 206a 6f62 5f6c 6973 7420         job_list 
+00009d10: 3d20 5b6a 6f62 2e73 7472 6970 2829 2066  = [job.strip() f
+00009d20: 6f72 206a 6f62 2069 6e20 7265 7375 6c74  or job in result
+00009d30: 2e73 7464 6f75 742e 7374 7269 7028 292e  .stdout.strip().
+00009d40: 7370 6c69 7428 275c 6e27 295d 0a20 2020  split('\n')].   
+00009d50: 2020 2020 206a 6f62 5f6c 6973 742e 7265       job_list.re
+00009d60: 7665 7273 6528 290a 2020 2020 2020 2020  verse().        
+00009d70: 7265 7475 726e 206a 6f62 5f6c 6973 740a  return job_list.
+00009d80: 0a20 2020 2064 6566 206c 6973 745f 616c  .    def list_al
+00009d90: 6c5f 6a6f 6273 2873 656c 662c 2065 6e76  l_jobs(self, env
+00009da0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
+00009db0: 7374 722c 2073 7472 5d5d 203d 204e 6f6e  str, str]] = Non
+00009dc0: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
+00009dd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00009de0: 2020 2020 2047 6574 2061 206c 6973 7420       Get a list 
+00009df0: 6f66 2061 6c6c 206a 6f62 7320 6672 6f6d  of all jobs from
+00009e00: 2053 4c55 524d 2e0a 0a20 2020 2020 2020   SLURM...       
+00009e10: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00009e20: 2020 2065 6e76 2028 4469 6374 5b73 7472     env (Dict[str
+00009e30: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
+00009e40: 293a 204f 7074 696f 6e61 6c20 656e 7669  ): Optional envi
+00009e50: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00009e60: 7320 0a20 2020 2020 2020 2020 2020 2020  s .             
+00009e70: 2020 2074 6f20 7365 7420 7768 656e 2072     to set when r
+00009e80: 756e 6e69 6e67 2074 6865 2063 6f6d 6d61  unning the comma
+00009e90: 6e64 2e20 4465 6661 756c 7473 2074 6f20  nd. Defaults to 
+00009ea0: 4e6f 6e65 2e0a 0a20 2020 2020 2020 2052  None...        R
+00009eb0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00009ec0: 2020 2020 4c69 7374 5b73 7472 5d3a 2041      List[str]: A
+00009ed0: 206c 6973 7420 6f66 206a 6f62 2049 4473   list of job IDs
+00009ee0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
+00009ef0: 2020 2020 2020 2063 6d64 203d 2073 656c         cmd = sel
+00009f00: 662e 6765 745f 6a6f 6273 5f69 6e66 6f5f  f.get_jobs_info_
+00009f10: 636f 6d6d 616e 6428 290a 2020 2020 2020  command().      
+00009f20: 2020 6c6f 6767 6572 2e69 6e66 6f28 2252    logger.info("R
+00009f30: 6574 7269 6576 696e 6720 6120 6c69 7374  etrieving a list
+00009f40: 206f 6620 616c 6c20 6a6f 6273 2066 726f   of all jobs fro
+00009f50: 6d20 536c 7572 6d22 290a 2020 2020 2020  m Slurm").      
+00009f60: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
+00009f70: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
+00009f80: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
+00009f90: 2020 2020 206a 6f62 5f6c 6973 7420 3d20       job_list = 
+00009fa0: 7265 7375 6c74 2e73 7464 6f75 742e 7374  result.stdout.st
+00009fb0: 7269 7028 292e 7370 6c69 7428 275c 6e27  rip().split('\n'
+00009fc0: 290a 2020 2020 2020 2020 6a6f 625f 6c69  ).        job_li
+00009fd0: 7374 2e72 6576 6572 7365 2829 0a20 2020  st.reverse().   
+00009fe0: 2020 2020 2072 6574 7572 6e20 6a6f 625f       return job_
+00009ff0: 6c69 7374 0a0a 2020 2020 6465 6620 6765  list..    def ge
+0000a000: 745f 6a6f 6273 5f69 6e66 6f5f 636f 6d6d  t_jobs_info_comm
+0000a010: 616e 6428 7365 6c66 2c20 7374 6172 745f  and(self, start_
+0000a020: 7469 6d65 3a20 7374 7220 3d20 2232 3032  time: str = "202
+0000a030: 332d 3031 2d30 3122 2c0a 2020 2020 2020  3-01-01",.      
+0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a050: 2020 2020 2020 2020 656e 645f 7469 6d65          end_time
+0000a060: 3a20 7374 7220 3d20 226e 6f77 222c 0a20  : str = "now",. 
+0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a080: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+0000a090: 756d 6e73 3a20 7374 7220 3d20 224a 6f62  umns: str = "Job
+0000a0a0: 4964 222c 0a20 2020 2020 2020 2020 2020  Id",.           
+0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0c0: 2020 2073 7461 7465 733a 2073 7472 203d     states: str =
+0000a0d0: 2022 722c 6364 2c66 2c74 6f2c 7273 2c64   "r,cd,f,to,rs,d
+0000a0e0: 6c2c 6e66 2229 202d 3e20 7374 723a 0a20  l,nf") -> str:. 
+0000a0f0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+0000a100: 2074 6865 2053 6c75 726d 2063 6f6d 6d61   the Slurm comma
+0000a110: 6e64 2074 6f20 7265 7472 6965 7665 2069  nd to retrieve i
+0000a120: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+0000a130: 206f 6c64 206a 6f62 732e 0a0a 2020 2020   old jobs...    
+0000a140: 2020 2020 5468 6520 636f 6d6d 616e 6420      The command 
+0000a150: 7769 6c6c 2062 6520 666f 726d 6174 7465  will be formatte
+0000a160: 6420 7769 7468 2074 6865 2073 7065 6369  d with the speci
+0000a170: 6669 6564 2073 7461 7274 2074 696d 652c  fied start time,
+0000a180: 2077 6869 6368 2069 730a 2020 2020 2020   which is.      
+0000a190: 2020 6578 7065 6374 6564 2074 6f20 6265    expected to be
+0000a1a0: 2069 6e20 7468 6520 4953 4f20 666f 726d   in the ISO form
+0000a1b0: 6174 2022 5959 5959 2d4d 4d2d 4444 222e  at "YYYY-MM-DD".
+0000a1c0: 0a20 2020 2020 2020 2054 6865 2063 6f6d  .        The com
+0000a1d0: 6d61 6e64 2077 696c 6c20 7573 6520 7468  mand will use th
+0000a1e0: 6520 2273 6163 6374 2220 746f 6f6c 2074  e "sacct" tool t
+0000a1f0: 6f20 7175 6572 7920 7468 650a 2020 2020  o query the.    
+0000a200: 2020 2020 536c 7572 6d20 6163 636f 756e      Slurm accoun
+0000a210: 7469 6e67 2064 6174 6162 6173 6520 666f  ting database fo
+0000a220: 7220 6a6f 6273 2074 6861 7420 7374 6172  r jobs that star
+0000a230: 7465 6420 6f6e 206f 7220 6166 7465 7220  ted on or after 
+0000a240: 7468 650a 2020 2020 2020 2020 7370 6563  the.        spec
+0000a250: 6966 6965 6420 7374 6172 7420 7469 6d65  ified start time
+0000a260: 2c20 616e 6420 7769 6c6c 206f 7574 7075  , and will outpu
+0000a270: 7420 6f6e 6c79 2074 6865 206a 6f62 2049  t only the job I
+0000a280: 4473 2028 2d6f 204a 6f62 4964 290a 2020  Ds (-o JobId).  
+0000a290: 2020 2020 2020 7769 7468 6f75 7420 6865        without he
+0000a2a0: 6164 6572 206f 7220 7472 6169 6c65 7220  ader or trailer 
+0000a2b0: 6c69 6e65 7320 282d 6e20 2d58 292e 0a0a  lines (-n -X)...
+0000a2c0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000a2d0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+0000a2e0: 7469 6d65 2028 7374 7229 3a20 5468 6520  time (str): The 
+0000a2f0: 7374 6172 7420 7469 6d65 2066 726f 6d20  start time from 
+0000a300: 7768 6963 6820 746f 2072 6574 7269 6576  which to retriev
+0000a310: 6520 6a6f 620a 2020 2020 2020 2020 2020  e job.          
+0000a320: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
+0000a330: 6e2e 2044 6566 6175 6c74 7320 746f 2022  n. Defaults to "
+0000a340: 3230 3233 2d30 312d 3031 222e 0a20 2020  2023-01-01"..   
+0000a350: 2020 2020 2020 2020 2065 6e64 5f74 696d           end_tim
+0000a360: 6520 2873 7472 293a 2054 6865 2065 6e64  e (str): The end
+0000a370: 2074 696d 6520 756e 7469 6c20 7768 6963   time until whic
+0000a380: 6820 746f 2072 6574 7269 6576 6520 6a6f  h to retrieve jo
+0000a390: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
+0000a3a0: 2020 696e 666f 726d 6174 696f 6e2e 2044    information. D
+0000a3b0: 6566 6175 6c74 7320 746f 2022 6e6f 7722  efaults to "now"
+0000a3c0: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+0000a3d0: 6c75 6d6e 7320 2873 7472 293a 2054 6865  lumns (str): The
+0000a3e0: 2063 6f6c 756d 6e73 2074 6f20 7265 7472   columns to retr
+0000a3f0: 6965 7665 2066 726f 6d20 7468 6520 6a6f  ieve from the jo
+0000a400: 6220 696e 666f 726d 6174 696f 6e2e 0a20  b information.. 
+0000a410: 2020 2020 2020 2020 2020 2020 2020 2044                 D
+0000a420: 6566 6175 6c74 7320 746f 2022 4a6f 6249  efaults to "JobI
+0000a430: 6422 2e20 4974 2069 7320 636f 6d6d 6120  d". It is comma 
+0000a440: 7365 7061 7261 7465 642c 2065 2e67 2e20  separated, e.g. 
+0000a450: 224a 6f62 4964 2c53 7461 7465 222e 0a20  "JobId,State".. 
+0000a460: 2020 2020 2020 2020 2020 2073 7461 7465             state
+0000a470: 7320 2873 7472 293a 2054 6865 206a 6f62  s (str): The job
+0000a480: 2073 7461 7465 7320 746f 2069 6e63 6c75   states to inclu
+0000a490: 6465 2069 6e20 7468 6520 7175 6572 792e  de in the query.
+0000a4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a4b0: 2044 6566 6175 6c74 7320 746f 2022 722c   Defaults to "r,
+0000a4c0: 6364 2c66 2c74 6f2c 7273 2c64 6c2c 6e66  cd,f,to,rs,dl,nf
+0000a4d0: 222e 0a0a 2020 2020 2020 2020 5265 7475  "...        Retu
+0000a4e0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000a4f0: 2073 7472 3a0a 2020 2020 2020 2020 2020   str:.          
+0000a500: 2020 2020 2020 4120 7374 7269 6e67 2072        A string r
+0000a510: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
+0000a520: 536c 7572 6d20 636f 6d6d 616e 6420 746f  Slurm command to
+0000a530: 2072 6574 7269 6576 650a 2020 2020 2020   retrieve.      
+0000a540: 2020 2020 2020 2020 2020 696e 666f 726d            inform
+0000a550: 6174 696f 6e20 6162 6f75 7420 6f6c 6420  ation about old 
+0000a560: 6a6f 6273 2e0a 2020 2020 2020 2020 2222  jobs..        ""
+0000a570: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+0000a580: 2073 656c 662e 5f41 4c4c 5f4a 4f42 535f   self._ALL_JOBS_
+0000a590: 434d 442e 666f 726d 6174 2873 7461 7274  CMD.format(start
+0000a5a0: 5f74 696d 653d 7374 6172 745f 7469 6d65  _time=start_time
+0000a5b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5d0: 2020 2020 2020 2020 2020 2065 6e64 5f74             end_t
+0000a5e0: 696d 653d 656e 645f 7469 6d65 2c0a 2020  ime=end_time,.  
 0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a600: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000a610: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-0000a620: 2022 2222 0a20 2020 2020 2020 2047 656e   """.        Gen
-0000a630: 6572 6174 6520 6120 536c 7572 6d20 6a6f  erate a Slurm jo
-0000a640: 6220 7363 7269 7074 2066 6f72 2061 2073  b script for a s
-0000a650: 7065 6369 6669 6320 776f 726b 666c 6f77  pecific workflow
-0000a660: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-0000a670: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
-0000a680: 6b66 6c6f 7720 2873 7472 293a 2054 6865  kflow (str): The
-0000a690: 206e 616d 6520 6f66 2074 6865 2077 6f72   name of the wor
-0000a6a0: 6b66 6c6f 772e 0a20 2020 2020 2020 2020  kflow..         
-0000a6b0: 2020 2073 7562 7374 6974 7574 6573 2028     substitutes (
-0000a6c0: 4469 6374 5b73 7472 2c20 7374 725d 293a  Dict[str, str]):
-0000a6d0: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
-0000a6e0: 6e74 6169 6e69 6e67 206b 6579 2d76 616c  ntaining key-val
-0000a6f0: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-0000a700: 2020 2070 6169 7273 2066 6f72 2073 7562     pairs for sub
-0000a710: 7374 6974 7574 696e 6720 706c 6163 6568  stituting placeh
-0000a720: 6f6c 6465 7273 2069 6e20 7468 6520 6a6f  olders in the jo
-0000a730: 6220 7465 6d70 6c61 7465 2e0a 2020 2020  b template..    
-0000a740: 2020 2020 2020 2020 7465 6d70 6c61 7465          template
-0000a750: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-0000a760: 3a20 5468 6520 6669 6c65 6e61 6d65 206f  : The filename o
-0000a770: 6620 7468 6520 6a6f 6220 7465 6d70 6c61  f the job templa
-0000a780: 7465 2e0a 2020 2020 2020 2020 2020 2020  te..            
-0000a790: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-0000a7a0: 226a 6f62 5f74 656d 706c 6174 652e 7368  "job_template.sh
-0000a7b0: 222e 0a0a 2020 2020 2020 2020 5265 7475  "...        Retu
-0000a7c0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000a7d0: 2073 7472 3a20 5468 6520 6765 6e65 7261   str: The genera
-0000a7e0: 7465 6420 536c 7572 6d20 6a6f 6220 7363  ted Slurm job sc
-0000a7f0: 7269 7074 2061 7320 6120 7374 7269 6e67  ript as a string
-0000a800: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000a810: 2020 2020 2020 2320 6164 6420 776f 726b        # add work
-0000a820: 666c 6f77 2074 6f20 7375 6273 7469 7475  flow to substitu
-0000a830: 7465 730a 2020 2020 2020 2020 7375 6273  tes.        subs
-0000a840: 7469 7475 7465 735b 276a 6f62 6e61 6d65  titutes['jobname
-0000a850: 275d 203d 2077 6f72 6b66 6c6f 770a 2020  '] = workflow.  
-0000a860: 2020 2020 2020 2320 6772 6162 206a 6f62        # grab job
-0000a870: 2074 656d 706c 6174 650a 2020 2020 2020   template.      
-0000a880: 2020 7465 6d70 6c61 7465 5f66 203d 2066    template_f = f
-0000a890: 696c 6573 2822 7265 736f 7572 6365 7322  iles("resources"
-0000a8a0: 292e 6a6f 696e 7061 7468 2874 656d 706c  ).joinpath(templ
-0000a8b0: 6174 6529 0a20 2020 2020 2020 2077 6974  ate).        wit
-0000a8c0: 6820 7465 6d70 6c61 7465 5f66 2e6f 7065  h template_f.ope
-0000a8d0: 6e28 2772 2729 2061 7320 663a 0a20 2020  n('r') as f:.   
-0000a8e0: 2020 2020 2020 2020 2073 7263 203d 2054           src = T
-0000a8f0: 656d 706c 6174 6528 662e 7265 6164 2829  emplate(f.read()
-0000a900: 290a 2020 2020 2020 2020 2020 2020 6a6f  ).            jo
-0000a910: 625f 7363 7269 7074 203d 2073 7263 2e73  b_script = src.s
-0000a920: 6166 655f 7375 6273 7469 7475 7465 2873  afe_substitute(s
-0000a930: 7562 7374 6974 7574 6573 290a 2020 2020  ubstitutes).    
-0000a940: 2020 2020 7265 7475 726e 206a 6f62 5f73      return job_s
-0000a950: 6372 6970 740a 0a20 2020 2064 6566 2077  cript..    def w
-0000a960: 6f72 6b66 6c6f 775f 7061 7261 6d73 5f74  orkflow_params_t
-0000a970: 6f5f 7375 6273 2873 656c 662c 2070 6172  o_subs(self, par
-0000a980: 616d 7329 202d 3e20 4469 6374 5b73 7472  ams) -> Dict[str
-0000a990: 2c20 7374 725d 3a0a 2020 2020 2020 2020  , str]:.        
-0000a9a0: 2222 220a 2020 2020 2020 2020 436f 6e76  """.        Conv
-0000a9b0: 6572 7420 776f 726b 666c 6f77 2070 6172  ert workflow par
-0000a9c0: 616d 6574 6572 7320 746f 2073 7562 7374  ameters to subst
-0000a9d0: 6974 7574 696f 6e20 6469 6374 696f 6e61  itution dictiona
-0000a9e0: 7279 2066 6f72 206a 6f62 2073 6372 6970  ry for job scrip
-0000a9f0: 742e 0a0a 2020 2020 2020 2020 4172 6773  t...        Args
-0000aa00: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-0000aa10: 7261 6d73 3a20 4120 6469 6374 696f 6e61  rams: A dictiona
-0000aa20: 7279 2063 6f6e 7461 696e 696e 6720 776f  ry containing wo
-0000aa30: 726b 666c 6f77 2070 6172 616d 6574 6572  rkflow parameter
-0000aa40: 732e 0a0a 2020 2020 2020 2020 5265 7475  s...        Retu
-0000aa50: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000aa60: 2044 6963 745b 7374 722c 2073 7472 5d3a   Dict[str, str]:
-0000aa70: 2041 2064 6963 7469 6f6e 6172 7920 7769   A dictionary wi
-0000aa80: 7468 2070 6172 616d 6574 6572 206e 616d  th parameter nam
-0000aa90: 6573 2061 7320 6b65 7973 2061 6e64 0a20  es as keys and. 
-0000aaa0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000aab0: 6f72 7265 7370 6f6e 6469 6e67 2066 6c61  orresponding fla
-0000aac0: 6773 2077 6974 6820 706c 6163 6568 6f6c  gs with placehol
-0000aad0: 6465 7273 2061 7320 7661 6c75 6573 2e0a  ders as values..
-0000aae0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000aaf0: 2020 2020 7375 6273 203d 207b 7d0a 2020      subs = {}.  
-0000ab00: 2020 2020 2020 666c 6167 7320 3d20 5b5d        flags = []
-0000ab10: 0a20 2020 2020 2020 2066 6f72 205f 2c20  .        for _, 
-0000ab20: 7061 7261 6d20 696e 2070 6172 616d 732e  param in params.
-0000ab30: 6974 656d 7328 293a 0a20 2020 2020 2020  items():.       
-0000ab40: 2020 2020 2066 6c61 6720 3d20 7061 7261       flag = para
-0000ab50: 6d5b 2763 6d64 5f66 6c61 6727 5d0a 2020  m['cmd_flag'].  
-0000ab60: 2020 2020 2020 2020 2020 666c 6167 203d            flag =
-0000ab70: 2066 6c61 6720 2b20 2220 2422 202b 2070   flag + " $" + p
-0000ab80: 6172 616d 5b27 6e61 6d65 275d 2e75 7070  aram['name'].upp
-0000ab90: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-0000aba0: 2066 6c61 6773 2e61 7070 656e 6428 666c   flags.append(fl
-0000abb0: 6167 290a 2020 2020 2020 2020 7375 6273  ag).        subs
-0000abc0: 5b27 5041 5241 4d53 275d 203d 2022 2022  ['PARAMS'] = " "
-0000abd0: 2e6a 6f69 6e28 666c 6167 7329 0a20 2020  .join(flags).   
-0000abe0: 2020 2020 2072 6574 7572 6e20 7375 6273       return subs
-0000abf0: 0a0a 2020 2020 6465 6620 7570 6461 7465  ..    def update
-0000ac00: 5f73 6c75 726d 5f73 6372 6970 7473 2873  _slurm_scripts(s
-0000ac10: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
-0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac30: 2020 6765 6e65 7261 7465 5f6a 6f62 733a    generate_jobs:
-0000ac40: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac60: 2020 2020 2020 2020 2020 2020 656e 763a              env:
-0000ac70: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
-0000ac80: 7472 2c20 7374 725d 5d20 3d20 4e6f 6e65  tr, str]] = None
-0000ac90: 2920 2d3e 2052 6573 756c 743a 0a20 2020  ) -> Result:.   
-0000aca0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000acb0: 2055 7064 6174 6573 2074 6865 206c 6f63   Updates the loc
-0000acc0: 616c 2063 6f70 7920 6f66 2074 6865 2053  al copy of the S
-0000acd0: 6c75 726d 206a 6f62 2073 7562 6d69 7373  lurm job submiss
-0000ace0: 696f 6e20 7363 7269 7074 732e 0a0a 2020  ion scripts...  
-0000acf0: 2020 2020 2020 5468 6973 2066 756e 6374        This funct
-0000ad00: 696f 6e20 7075 6c6c 7320 7468 6520 6c61  ion pulls the la
-0000ad10: 7465 7374 2076 6572 7369 6f6e 206f 6620  test version of 
-0000ad20: 7468 6520 7363 7269 7074 7320 6672 6f6d  the scripts from
-0000ad30: 2074 6865 2047 6974 0a20 2020 2020 2020   the Git.       
-0000ad40: 2072 6570 6f73 6974 6f72 7920 616e 6420   repository and 
-0000ad50: 636f 7069 6573 2074 6865 6d20 746f 2074  copies them to t
-0000ad60: 6865 2073 6c75 726d 5f73 6372 6970 745f  he slurm_script_
-0000ad70: 7061 7468 2064 6972 6563 746f 7279 2e0a  path directory..
-0000ad80: 2020 2020 2020 2020 416c 7465 726e 6174          Alternat
-0000ad90: 6976 656c 792c 2069 7420 6361 6e20 6765  ively, it can ge
-0000ada0: 6e65 7261 7465 2073 6372 6970 7473 2066  nerate scripts f
-0000adb0: 726f 6d20 6120 7465 6d70 6c61 7465 2e20  rom a template. 
-0000adc0: 5468 6973 2069 7320 7468 650a 2020 2020  This is the.    
-0000add0: 2020 2020 6465 6661 756c 7420 6265 6861      default beha
-0000ade0: 7669 6f72 2069 6620 6e6f 2047 6974 2072  vior if no Git r
-0000adf0: 6570 6f20 6973 2070 726f 7669 6465 6420  epo is provided 
-0000ae00: 6f72 2063 616e 2062 6520 666f 7263 6564  or can be forced
-0000ae10: 2076 6961 2074 6865 0a20 2020 2020 2020   via the.       
-0000ae20: 2060 6765 6e65 7261 7465 5f6a 6f62 7360   `generate_jobs`
-0000ae30: 2070 6172 616d 6574 6572 2e0a 0a20 2020   parameter...   
-0000ae40: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000ae50: 2020 2020 2020 2067 656e 6572 6174 655f         generate_
-0000ae60: 6a6f 6273 2028 626f 6f6c 293a 2057 6865  jobs (bool): Whe
-0000ae70: 7468 6572 2074 6f20 6765 6e65 7261 7465  ther to generate
-0000ae80: 206e 6577 2073 6c75 726d 206a 6f62 2073   new slurm job s
-0000ae90: 6372 6970 7473 0a20 2020 2020 2020 2020  cripts.         
-0000aea0: 2020 2020 2020 2049 4e53 5445 4144 2028         INSTEAD (
-0000aeb0: 6f66 2070 756c 6c69 6e67 2066 726f 6d20  of pulling from 
-0000aec0: 6769 7429 2e20 4465 6661 756c 7473 2074  git). Defaults t
-0000aed0: 6f20 4661 6c73 652c 2065 7863 6570 740a  o False, except.
-0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aef0: 6966 206e 6f20 736c 7572 6d5f 7363 7269  if no slurm_scri
-0000af00: 7074 5f72 6570 6f20 6973 2063 6f6e 6669  pt_repo is confi
-0000af10: 6775 7265 642e 0a20 2020 2020 2020 2020  gured..         
-0000af20: 2020 2065 6e76 2028 4469 6374 5b73 7472     env (Dict[str
-0000af30: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
-0000af40: 293a 204f 7074 696f 6e61 6c20 656e 7669  ): Optional envi
-0000af50: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-0000af60: 7320 0a20 2020 2020 2020 2020 2020 2020  s .             
-0000af70: 2020 2074 6f20 7365 7420 7768 656e 2072     to set when r
-0000af80: 756e 6e69 6e67 2074 6865 2063 6f6d 6d61  unning the comma
-0000af90: 6e64 2e20 4465 6661 756c 7473 2074 6f20  nd. Defaults to 
-0000afa0: 4e6f 6e65 2e0a 0a20 2020 2020 2020 2052  None...        R
-0000afb0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0000afc0: 2020 2020 5265 7375 6c74 3a20 5468 6520      Result: The 
-0000afd0: 7265 7375 6c74 206f 6620 7468 6520 636f  result of the co
-0000afe0: 6d6d 616e 642e 0a20 2020 2020 2020 2022  mmand..        "
-0000aff0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-0000b000: 7420 7365 6c66 2e73 6c75 726d 5f73 6372  t self.slurm_scr
-0000b010: 6970 745f 7265 706f 3a0a 2020 2020 2020  ipt_repo:.      
-0000b020: 2020 2020 2020 6765 6e65 7261 7465 5f6a        generate_j
-0000b030: 6f62 7320 3d20 5472 7565 0a0a 2020 2020  obs = True..    
-0000b040: 2020 2020 6966 2067 656e 6572 6174 655f      if generate_
-0000b050: 6a6f 6273 3a0a 2020 2020 2020 2020 2020  jobs:.          
-0000b060: 2020 6c6f 6767 6572 2e69 6e66 6f28 2247    logger.info("G
-0000b070: 656e 6572 6174 696e 6720 536c 7572 6d20  enerating Slurm 
-0000b080: 6a6f 6220 7363 7269 7074 7322 290a 2020  job scripts").  
-0000b090: 2020 2020 2020 2020 2020 666f 7220 7766            for wf
-0000b0a0: 2c20 6a6f 625f 7061 7468 2069 6e20 7365  , job_path in se
-0000b0b0: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f6a  lf.slurm_model_j
-0000b0c0: 6f62 732e 6974 656d 7328 293a 0a20 2020  obs.items():.   
-0000b0d0: 2020 2020 2020 2020 2020 2020 2023 2067               # g
-0000b0e0: 656e 6572 6174 6520 6a6f 6220 7363 7269  enerate job scri
-0000b0f0: 7074 0a20 2020 2020 2020 2020 2020 2020  pt.             
-0000b100: 2020 2070 6172 616d 7320 3d20 7365 6c66     params = self
-0000b110: 2e67 6574 5f77 6f72 6b66 6c6f 775f 7061  .get_workflow_pa
-0000b120: 7261 6d65 7465 7273 2877 6629 0a20 2020  rameters(wf).   
-0000b130: 2020 2020 2020 2020 2020 2020 2073 7562               sub
-0000b140: 7320 3d20 7365 6c66 2e77 6f72 6b66 6c6f  s = self.workflo
-0000b150: 775f 7061 7261 6d73 5f74 6f5f 7375 6273  w_params_to_subs
-0000b160: 2870 6172 616d 7329 0a20 2020 2020 2020  (params).       
-0000b170: 2020 2020 2020 2020 206a 6f62 5f73 6372           job_scr
-0000b180: 6970 7420 3d20 7365 6c66 2e67 656e 6572  ipt = self.gener
-0000b190: 6174 655f 736c 7572 6d5f 6a6f 625f 666f  ate_slurm_job_fo
-0000b1a0: 725f 776f 726b 666c 6f77 2877 662c 2073  r_workflow(wf, s
-0000b1b0: 7562 7329 0a20 2020 2020 2020 2020 2020  ubs).           
-0000b1c0: 2020 2020 2023 2065 6e73 7572 6520 616c       # ensure al
-0000b1d0: 6c20 6469 7273 2065 7869 7374 2072 656d  l dirs exist rem
-0000b1e0: 6f74 656c 790a 2020 2020 2020 2020 2020  otely.          
-0000b1f0: 2020 2020 2020 6675 6c6c 5f70 6174 6820        full_path 
-0000b200: 3d20 7365 6c66 2e73 6c75 726d 5f73 6372  = self.slurm_scr
-0000b210: 6970 745f 7061 7468 2b22 2f22 2b6a 6f62  ipt_path+"/"+job
-0000b220: 5f70 6174 680a 2020 2020 2020 2020 2020  _path.          
-0000b230: 2020 2020 2020 6a6f 625f 6469 722c 205f        job_dir, _
-0000b240: 203d 206f 732e 7061 7468 2e73 706c 6974   = os.path.split
-0000b250: 2866 756c 6c5f 7061 7468 290a 2020 2020  (full_path).    
-0000b260: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000b270: 2e72 756e 2866 226d 6b64 6972 202d 7020  .run(f"mkdir -p 
-0000b280: 7b6a 6f62 5f64 6972 7d22 290a 2020 2020  {job_dir}").    
-0000b290: 2020 2020 2020 2020 2020 2020 2320 636f              # co
-0000b2a0: 7079 2074 6f20 7265 6d6f 7465 2066 696c  py to remote fil
-0000b2b0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000b2c0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-0000b2d0: 7075 7428 6c6f 6361 6c3d 696f 2e53 7472  put(local=io.Str
-0000b2e0: 696e 6749 4f28 6a6f 625f 7363 7269 7074  ingIO(job_script
-0000b2f0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000b300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b310: 2020 2020 2072 656d 6f74 653d 6675 6c6c       remote=full
-0000b320: 5f70 6174 6829 0a20 2020 2020 2020 2065  _path).        e
-0000b330: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000b340: 2063 6d64 203d 2073 656c 662e 6765 745f   cmd = self.get_
-0000b350: 7570 6461 7465 5f73 6c75 726d 5f73 6372  update_slurm_scr
-0000b360: 6970 7473 5f63 6f6d 6d61 6e64 2829 0a20  ipts_command(). 
-0000b370: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000b380: 722e 696e 666f 2822 5570 6461 7469 6e67  r.info("Updating
-0000b390: 2053 6c75 726d 206a 6f62 2073 6372 6970   Slurm job scrip
-0000b3a0: 7473 206f 6e20 536c 7572 6d22 290a 2020  ts on Slurm").  
-0000b3b0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000b3c0: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
-0000b3d0: 616e 6473 285b 636d 645d 2c20 656e 763d  ands([cmd], env=
-0000b3e0: 656e 7629 0a20 2020 2020 2020 2072 6574  env).        ret
-0000b3f0: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-0000b400: 6465 6620 7275 6e5f 776f 726b 666c 6f77  def run_workflow
-0000b410: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-0000b420: 2020 2020 2020 2020 2020 2020 776f 726b              work
-0000b430: 666c 6f77 5f6e 616d 653a 2073 7472 2c0a  flow_name: str,.
-0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b450: 2020 2020 2077 6f72 6b66 6c6f 775f 7665       workflow_ve
-0000b460: 7273 696f 6e3a 2073 7472 2c0a 2020 2020  rsion: str,.    
-0000b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b480: 2069 6e70 7574 5f64 6174 613a 2073 7472   input_data: str
-0000b490: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000b4a0: 2020 2020 2020 2065 6d61 696c 3a20 4f70         email: Op
-0000b4b0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-0000b4c0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
-0000b4d0: 2020 2020 2020 2020 2074 696d 653a 204f           time: O
-0000b4e0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-0000b4f0: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
-0000b500: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000b510: 6773 0a20 2020 2020 2020 2020 2020 2020  gs.             
-0000b520: 2020 2020 2020 2020 2920 2d3e 2054 7570          ) -> Tup
-0000b530: 6c65 5b52 6573 756c 742c 2069 6e74 5d3a  le[Result, int]:
-0000b540: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000b550: 2020 2020 2052 756e 2061 2073 7065 6369       Run a speci
-0000b560: 6669 6564 2077 6f72 6b66 6c6f 7720 6f6e  fied workflow on
-0000b570: 2053 6c75 726d 2075 7369 6e67 2074 6865   Slurm using the
-0000b580: 2067 6976 656e 2070 6172 616d 6574 6572   given parameter
-0000b590: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
-0000b5a0: 3a0a 2020 2020 2020 2020 2020 2020 776f  :.            wo
-0000b5b0: 726b 666c 6f77 5f6e 616d 6520 2873 7472  rkflow_name (str
-0000b5c0: 293a 204e 616d 6520 6f66 2074 6865 2077  ): Name of the w
-0000b5d0: 6f72 6b66 6c6f 7720 746f 2065 7865 6375  orkflow to execu
-0000b5e0: 7465 2e0a 2020 2020 2020 2020 2020 2020  te..            
-0000b5f0: 776f 726b 666c 6f77 5f76 6572 7369 6f6e  workflow_version
-0000b600: 2028 7374 7229 3a20 5665 7273 696f 6e20   (str): Version 
-0000b610: 6f66 2074 6865 2077 6f72 6b66 6c6f 7720  of the workflow 
-0000b620: 2869 6d61 6765 2076 6572 7369 6f6e 200a  (image version .
-0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 6f6e 2053 6c75 726d 292e 0a20 2020 2020  on Slurm)..     
-0000b650: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
-0000b660: 6120 2873 7472 293a 204e 616d 6520 6f66  a (str): Name of
-0000b670: 2074 6865 2069 6e70 7574 2064 6174 6120   the input data 
-0000b680: 666f 6c64 6572 2063 6f6e 7461 696e 696e  folder containin
-0000b690: 6720 696e 7075 740a 2020 2020 2020 2020  g input.        
-0000b6a0: 2020 2020 2020 2020 696d 6167 6520 6669          image fi
-0000b6b0: 6c65 732e 0a20 2020 2020 2020 2020 2020  les..           
-0000b6c0: 2065 6d61 696c 2028 7374 722c 206f 7074   email (str, opt
-0000b6d0: 696f 6e61 6c29 3a20 456d 6169 6c20 6164  ional): Email ad
-0000b6e0: 6472 6573 7320 666f 7220 536c 7572 6d20  dress for Slurm 
-0000b6f0: 6a6f 6220 6e6f 7469 6669 6361 7469 6f6e  job notification
-0000b700: 732e 0a20 2020 2020 2020 2020 2020 2074  s..            t
-0000b710: 696d 6520 2873 7472 2c20 6f70 7469 6f6e  ime (str, option
-0000b720: 616c 293a 2054 696d 6520 6c69 6d69 7420  al): Time limit 
-0000b730: 666f 7220 7468 6520 536c 7572 6d20 6a6f  for the Slurm jo
-0000b740: 6220 696e 2074 6865 200a 2020 2020 2020  b in the .      
-0000b750: 2020 2020 2020 2020 2020 666f 726d 6174            format
-0000b760: 2048 483a 4d4d 3a53 532e 0a20 2020 2020   HH:MM:SS..     
-0000b770: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
-0000b780: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
-0000b790: 6f72 6420 6172 6775 6d65 6e74 7320 666f  ord arguments fo
-0000b7a0: 7220 7468 6520 776f 726b 666c 6f77 2e0a  r the workflow..
-0000b7b0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000b7c0: 3a0a 2020 2020 2020 2020 2020 2020 5475  :.            Tu
-0000b7d0: 706c 655b 5265 7375 6c74 2c20 696e 745d  ple[Result, int]
-0000b7e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000b7f0: 2020 4120 7475 706c 6520 636f 6e74 6169    A tuple contai
-0000b800: 6e69 6e67 2074 6865 2072 6573 756c 7420  ning the result 
-0000b810: 6f66 2073 7461 7274 696e 6720 7468 6520  of starting the 
-0000b820: 776f 726b 666c 6f77 206a 6f62 2061 6e64  workflow job and
-0000b830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b840: 2074 6865 2053 6c75 726d 206a 6f62 2049   the Slurm job I
-0000b850: 442c 206f 7220 2d31 2069 6620 7468 6520  D, or -1 if the 
-0000b860: 6a6f 6220 4944 2063 6f75 6c64 206e 6f74  job ID could not
-0000b870: 2062 6520 6578 7472 6163 7465 642e 0a0a   be extracted...
-0000b880: 2020 2020 2020 2020 4e6f 7465 3a0a 2020          Note:.  
-0000b890: 2020 2020 2020 2020 2020 5468 6520 536c            The Sl
-0000b8a0: 7572 6d20 6a6f 6220 4944 2069 7320 6578  urm job ID is ex
-0000b8b0: 7472 6163 7465 6420 6672 6f6d 2074 6865  tracted from the
-0000b8c0: 2072 6573 756c 7420 6f66 2074 6865 200a   result of the .
-0000b8d0: 2020 2020 2020 2020 2020 2020 6072 756e              `run
-0000b8e0: 5f63 6f6d 6d61 6e64 7360 206d 6574 686f  _commands` metho
-0000b8f0: 642e 0a20 2020 2020 2020 2022 2222 0a20  d..        """. 
-0000b900: 2020 2020 2020 2073 6261 7463 685f 636d         sbatch_cm
-0000b910: 642c 2073 6261 7463 685f 656e 7620 3d20  d, sbatch_env = 
-0000b920: 7365 6c66 2e67 6574 5f77 6f72 6b66 6c6f  self.get_workflo
-0000b930: 775f 636f 6d6d 616e 6428 0a20 2020 2020  w_command(.     
-0000b940: 2020 2020 2020 2077 6f72 6b66 6c6f 775f         workflow_
-0000b950: 6e61 6d65 2c20 776f 726b 666c 6f77 5f76  name, workflow_v
-0000b960: 6572 7369 6f6e 2c20 696e 7075 745f 6461  ersion, input_da
-0000b970: 7461 2c20 656d 6169 6c2c 2074 696d 652c  ta, email, time,
-0000b980: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-0000b990: 2020 2070 7269 6e74 2866 2252 756e 6e69     print(f"Runni
-0000b9a0: 6e67 207b 776f 726b 666c 6f77 5f6e 616d  ng {workflow_nam
-0000b9b0: 657d 206a 6f62 206f 6e20 7b69 6e70 7574  e} job on {input
-0000b9c0: 5f64 6174 617d 206f 6e20 536c 7572 6d3a  _data} on Slurm:
-0000b9d0: 5c0a 2020 2020 2020 2020 2020 2020 7b73  \.            {s
-0000b9e0: 6261 7463 685f 636d 647d 2077 2f20 7b73  batch_cmd} w/ {s
-0000b9f0: 6261 7463 685f 656e 767d 2229 0a20 2020  batch_env}").   
-0000ba00: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-0000ba10: 2866 2252 756e 6e69 6e67 207b 776f 726b  (f"Running {work
-0000ba20: 666c 6f77 5f6e 616d 657d 206a 6f62 206f  flow_name} job o
-0000ba30: 6e20 7b69 6e70 7574 5f64 6174 617d 206f  n {input_data} o
-0000ba40: 6e20 536c 7572 6d22 290a 2020 2020 2020  n Slurm").      
-0000ba50: 2020 7265 7320 3d20 7365 6c66 2e72 756e    res = self.run
-0000ba60: 5f63 6f6d 6d61 6e64 7328 5b73 6261 7463  _commands([sbatc
-0000ba70: 685f 636d 645d 2c20 7362 6174 6368 5f65  h_cmd], sbatch_e
-0000ba80: 6e76 290a 2020 2020 2020 2020 7265 7475  nv).        retu
-0000ba90: 726e 2072 6573 2c20 7365 6c66 2e65 7874  rn res, self.ext
-0000baa0: 7261 6374 5f6a 6f62 5f69 6428 7265 7329  ract_job_id(res)
-0000bab0: 0a0a 2020 2020 6465 6620 7275 6e5f 776f  ..    def run_wo
-0000bac0: 726b 666c 6f77 5f6a 6f62 2873 656c 662c  rkflow_job(self,
-0000bad0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bae0: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000baf0: 6f77 5f6e 616d 653a 2073 7472 2c0a 2020  ow_name: str,.  
+0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a610: 2020 2020 2020 2073 7461 7465 733d 7374         states=st
+0000a620: 6174 6573 2c0a 2020 2020 2020 2020 2020  ates,.          
+0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a640: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000a650: 6f6c 756d 6e73 3d63 6f6c 756d 6e73 290a  olumns=columns).
+0000a660: 0a20 2020 2064 6566 2074 7261 6e73 6665  .    def transfe
+0000a670: 725f 6461 7461 2873 656c 662c 206c 6f63  r_data(self, loc
+0000a680: 616c 5f70 6174 683a 2073 7472 2920 2d3e  al_path: str) ->
+0000a690: 2052 6573 756c 743a 0a20 2020 2020 2020   Result:.       
+0000a6a0: 2022 2222 0a20 2020 2020 2020 2054 7261   """.        Tra
+0000a6b0: 6e73 6665 7273 2061 2066 696c 6520 6f72  nsfers a file or
+0000a6c0: 2064 6972 6563 746f 7279 2066 726f 6d20   directory from 
+0000a6d0: 7468 6520 6c6f 6361 6c20 6d61 6368 696e  the local machin
+0000a6e0: 6520 746f 2074 6865 2072 656d 6f74 650a  e to the remote.
+0000a6f0: 2020 2020 2020 2020 536c 7572 6d20 636c          Slurm cl
+0000a700: 7573 7465 722e 0a0a 2020 2020 2020 2020  uster...        
+0000a710: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+0000a720: 2020 6c6f 6361 6c5f 7061 7468 2028 7374    local_path (st
+0000a730: 7229 3a20 5468 6520 6c6f 6361 6c20 7061  r): The local pa
+0000a740: 7468 2074 6f20 7468 6520 6669 6c65 206f  th to the file o
+0000a750: 7220 6469 7265 6374 6f72 7920 746f 0a20  r directory to. 
+0000a760: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000a770: 7261 6e73 6665 722e 0a0a 2020 2020 2020  ransfer...      
+0000a780: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000a790: 2020 2020 2020 2052 6573 756c 743a 2054         Result: T
+0000a7a0: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
+0000a7b0: 2066 696c 6520 7472 616e 7366 6572 206f   file transfer o
+0000a7c0: 7065 7261 7469 6f6e 2e0a 2020 2020 2020  peration..      
+0000a7d0: 2020 2222 220a 2020 2020 2020 2020 6c6f    """.        lo
+0000a7e0: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
+0000a7f0: 2020 2020 2020 2066 2254 7261 6e73 6665         f"Transfe
+0000a800: 7269 6e67 2066 696c 6520 7b6c 6f63 616c  ring file {local
+0000a810: 5f70 6174 687d 2074 6f20 7b73 656c 662e  _path} to {self.
+0000a820: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
+0000a830: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
+0000a840: 6e20 7365 6c66 2e70 7574 286c 6f63 616c  n self.put(local
+0000a850: 3d6c 6f63 616c 5f70 6174 682c 2072 656d  =local_path, rem
+0000a860: 6f74 653d 7365 6c66 2e73 6c75 726d 5f64  ote=self.slurm_d
+0000a870: 6174 615f 7061 7468 290a 0a20 2020 2064  ata_path)..    d
+0000a880: 6566 2075 6e70 6163 6b5f 6461 7461 2873  ef unpack_data(s
+0000a890: 656c 662c 207a 6970 6669 6c65 3a20 7374  elf, zipfile: st
+0000a8a0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
+0000a8b0: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
+0000a8c0: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
+0000a8d0: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
+0000a8e0: 5265 7375 6c74 3a0a 2020 2020 2020 2020  Result:.        
+0000a8f0: 2222 220a 2020 2020 2020 2020 556e 7061  """.        Unpa
+0000a900: 636b 7320 6120 7a69 7070 6564 2066 696c  cks a zipped fil
+0000a910: 6520 6f6e 2074 6865 2072 656d 6f74 6520  e on the remote 
+0000a920: 536c 7572 6d20 636c 7573 7465 722e 0a0a  Slurm cluster...
+0000a930: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000a940: 2020 2020 2020 2020 2020 7a69 7066 696c            zipfil
+0000a950: 6520 2873 7472 293a 2054 6865 206e 616d  e (str): The nam
+0000a960: 6520 6f66 2074 6865 207a 6970 7065 6420  e of the zipped 
+0000a970: 6669 6c65 2074 6f20 6265 2075 6e70 6163  file to be unpac
+0000a980: 6b65 642e 0a0a 2020 2020 2020 2020 2020  ked...          
+0000a990: 2020 656e 7620 2844 6963 745b 7374 722c    env (Dict[str,
+0000a9a0: 2073 7472 5d2c 206f 7074 696f 6e61 6c29   str], optional)
+0000a9b0: 3a20 4f70 7469 6f6e 616c 2065 6e76 6972  : Optional envir
+0000a9c0: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
+0000a9d0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000a9e0: 2020 746f 2073 6574 2077 6865 6e20 7275    to set when ru
+0000a9f0: 6e6e 696e 6720 7468 6520 636f 6d6d 616e  nning the comman
+0000aa00: 642e 2044 6566 6175 6c74 7320 746f 204e  d. Defaults to N
+0000aa10: 6f6e 652e 0a0a 2020 2020 2020 2020 5265  one...        Re
+0000aa20: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0000aa30: 2020 2052 6573 756c 743a 2054 6865 2072     Result: The r
+0000aa40: 6573 756c 7420 6f66 2074 6865 2063 6f6d  esult of the com
+0000aa50: 6d61 6e64 2e0a 2020 2020 2020 2020 2222  mand..        ""
+0000aa60: 220a 2020 2020 2020 2020 636d 6420 3d20  ".        cmd = 
+0000aa70: 7365 6c66 2e67 6574 5f75 6e7a 6970 5f63  self.get_unzip_c
+0000aa80: 6f6d 6d61 6e64 287a 6970 6669 6c65 290a  ommand(zipfile).
+0000aa90: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
+0000aaa0: 6e66 6f28 6622 556e 7061 636b 696e 6720  nfo(f"Unpacking 
+0000aab0: 7b7a 6970 6669 6c65 7d20 6f6e 2053 6c75  {zipfile} on Slu
+0000aac0: 726d 2229 0a20 2020 2020 2020 2072 6574  rm").        ret
+0000aad0: 7572 6e20 7365 6c66 2e72 756e 5f63 6f6d  urn self.run_com
+0000aae0: 6d61 6e64 7328 5b63 6d64 5d2c 2065 6e76  mands([cmd], env
+0000aaf0: 3d65 6e76 290a 0a20 2020 2064 6566 2067  =env)..    def g
+0000ab00: 656e 6572 6174 655f 736c 7572 6d5f 6a6f  enerate_slurm_jo
+0000ab10: 625f 666f 725f 776f 726b 666c 6f77 2873  b_for_workflow(s
+0000ab20: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab40: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
+0000ab50: 6b66 6c6f 773a 2073 7472 2c0a 2020 2020  kflow: str,.    
+0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab80: 2020 2020 7375 6273 7469 7475 7465 733a      substitutes:
+0000ab90: 2044 6963 745b 7374 722c 2073 7472 5d2c   Dict[str, str],
+0000aba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abc0: 2020 2020 2020 2020 2074 656d 706c 6174           templat
+0000abd0: 653a 2073 7472 203d 2022 6a6f 625f 7465  e: str = "job_te
+0000abe0: 6d70 6c61 7465 2e73 6822 0a20 2020 2020  mplate.sh".     
+0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac10: 2020 2029 202d 3e20 7374 723a 0a20 2020     ) -> str:.   
+0000ac20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ac30: 2047 656e 6572 6174 6520 6120 536c 7572   Generate a Slur
+0000ac40: 6d20 6a6f 6220 7363 7269 7074 2066 6f72  m job script for
+0000ac50: 2061 2073 7065 6369 6669 6320 776f 726b   a specific work
+0000ac60: 666c 6f77 2e0a 0a20 2020 2020 2020 2041  flow...        A
+0000ac70: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000ac80: 2077 6f72 6b66 6c6f 7720 2873 7472 293a   workflow (str):
+0000ac90: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+0000aca0: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
+0000acb0: 2020 2020 2020 2073 7562 7374 6974 7574         substitut
+0000acc0: 6573 2028 4469 6374 5b73 7472 2c20 7374  es (Dict[str, st
+0000acd0: 725d 293a 2041 2064 6963 7469 6f6e 6172  r]): A dictionar
+0000ace0: 7920 636f 6e74 6169 6e69 6e67 206b 6579  y containing key
+0000acf0: 2d76 616c 7565 0a20 2020 2020 2020 2020  -value.         
+0000ad00: 2020 2020 2020 2070 6169 7273 2066 6f72         pairs for
+0000ad10: 2073 7562 7374 6974 7574 696e 6720 706c   substituting pl
+0000ad20: 6163 6568 6f6c 6465 7273 2069 6e20 7468  aceholders in th
+0000ad30: 6520 6a6f 6220 7465 6d70 6c61 7465 2e0a  e job template..
+0000ad40: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
+0000ad50: 6c61 7465 2028 7374 722c 206f 7074 696f  late (str, optio
+0000ad60: 6e61 6c29 3a20 5468 6520 6669 6c65 6e61  nal): The filena
+0000ad70: 6d65 206f 6620 7468 6520 6a6f 6220 7465  me of the job te
+0000ad80: 6d70 6c61 7465 2e0a 2020 2020 2020 2020  mplate..        
+0000ad90: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+0000ada0: 2074 6f20 226a 6f62 5f74 656d 706c 6174   to "job_templat
+0000adb0: 652e 7368 222e 0a0a 2020 2020 2020 2020  e.sh"...        
+0000adc0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000add0: 2020 2020 2073 7472 3a20 5468 6520 6765       str: The ge
+0000ade0: 6e65 7261 7465 6420 536c 7572 6d20 6a6f  nerated Slurm jo
+0000adf0: 6220 7363 7269 7074 2061 7320 6120 7374  b script as a st
+0000ae00: 7269 6e67 2e0a 2020 2020 2020 2020 2222  ring..        ""
+0000ae10: 220a 2020 2020 2020 2020 2320 6164 6420  ".        # add 
+0000ae20: 776f 726b 666c 6f77 2074 6f20 7375 6273  workflow to subs
+0000ae30: 7469 7475 7465 730a 2020 2020 2020 2020  titutes.        
+0000ae40: 7375 6273 7469 7475 7465 735b 276a 6f62  substitutes['job
+0000ae50: 6e61 6d65 275d 203d 2077 6f72 6b66 6c6f  name'] = workflo
+0000ae60: 770a 2020 2020 2020 2020 2320 6772 6162  w.        # grab
+0000ae70: 206a 6f62 2074 656d 706c 6174 650a 2020   job template.  
+0000ae80: 2020 2020 2020 7465 6d70 6c61 7465 5f66        template_f
+0000ae90: 203d 2066 696c 6573 2822 7265 736f 7572   = files("resour
+0000aea0: 6365 7322 292e 6a6f 696e 7061 7468 2874  ces").joinpath(t
+0000aeb0: 656d 706c 6174 6529 0a20 2020 2020 2020  emplate).       
+0000aec0: 2077 6974 6820 7465 6d70 6c61 7465 5f66   with template_f
+0000aed0: 2e6f 7065 6e28 2772 2729 2061 7320 663a  .open('r') as f:
+0000aee0: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
+0000aef0: 203d 2054 656d 706c 6174 6528 662e 7265   = Template(f.re
+0000af00: 6164 2829 290a 2020 2020 2020 2020 2020  ad()).          
+0000af10: 2020 6a6f 625f 7363 7269 7074 203d 2073    job_script = s
+0000af20: 7263 2e73 6166 655f 7375 6273 7469 7475  rc.safe_substitu
+0000af30: 7465 2873 7562 7374 6974 7574 6573 290a  te(substitutes).
+0000af40: 2020 2020 2020 2020 7265 7475 726e 206a          return j
+0000af50: 6f62 5f73 6372 6970 740a 0a20 2020 2064  ob_script..    d
+0000af60: 6566 2077 6f72 6b66 6c6f 775f 7061 7261  ef workflow_para
+0000af70: 6d73 5f74 6f5f 7375 6273 2873 656c 662c  ms_to_subs(self,
+0000af80: 2070 6172 616d 7329 202d 3e20 4469 6374   params) -> Dict
+0000af90: 5b73 7472 2c20 7374 725d 3a0a 2020 2020  [str, str]:.    
+0000afa0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000afb0: 436f 6e76 6572 7420 776f 726b 666c 6f77  Convert workflow
+0000afc0: 2070 6172 616d 6574 6572 7320 746f 2073   parameters to s
+0000afd0: 7562 7374 6974 7574 696f 6e20 6469 6374  ubstitution dict
+0000afe0: 696f 6e61 7279 2066 6f72 206a 6f62 2073  ionary for job s
+0000aff0: 6372 6970 742e 0a0a 2020 2020 2020 2020  cript...        
+0000b000: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+0000b010: 2020 7061 7261 6d73 3a20 4120 6469 6374    params: A dict
+0000b020: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+0000b030: 6720 776f 726b 666c 6f77 2070 6172 616d  g workflow param
+0000b040: 6574 6572 732e 0a0a 2020 2020 2020 2020  eters...        
+0000b050: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000b060: 2020 2020 2044 6963 745b 7374 722c 2073       Dict[str, s
+0000b070: 7472 5d3a 2041 2064 6963 7469 6f6e 6172  tr]: A dictionar
+0000b080: 7920 7769 7468 2070 6172 616d 6574 6572  y with parameter
+0000b090: 206e 616d 6573 2061 7320 6b65 7973 2061   names as keys a
+0000b0a0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+0000b0b0: 2020 2063 6f72 7265 7370 6f6e 6469 6e67     corresponding
+0000b0c0: 2066 6c61 6773 2077 6974 6820 706c 6163   flags with plac
+0000b0d0: 6568 6f6c 6465 7273 2061 7320 7661 6c75  eholders as valu
+0000b0e0: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
+0000b0f0: 2020 2020 2020 2020 7375 6273 203d 207b          subs = {
+0000b100: 7d0a 2020 2020 2020 2020 666c 6167 7320  }.        flags 
+0000b110: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
+0000b120: 205f 2c20 7061 7261 6d20 696e 2070 6172   _, param in par
+0000b130: 616d 732e 6974 656d 7328 293a 0a20 2020  ams.items():.   
+0000b140: 2020 2020 2020 2020 2066 6c61 6720 3d20           flag = 
+0000b150: 7061 7261 6d5b 2763 6d64 5f66 6c61 6727  param['cmd_flag'
+0000b160: 5d0a 2020 2020 2020 2020 2020 2020 666c  ].            fl
+0000b170: 6167 203d 2066 6c61 6720 2b20 2220 2422  ag = flag + " $"
+0000b180: 202b 2070 6172 616d 5b27 6e61 6d65 275d   + param['name']
+0000b190: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
+0000b1a0: 2020 2020 2066 6c61 6773 2e61 7070 656e       flags.appen
+0000b1b0: 6428 666c 6167 290a 2020 2020 2020 2020  d(flag).        
+0000b1c0: 7375 6273 5b27 5041 5241 4d53 275d 203d  subs['PARAMS'] =
+0000b1d0: 2022 2022 2e6a 6f69 6e28 666c 6167 7329   " ".join(flags)
+0000b1e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000b1f0: 7375 6273 0a0a 2020 2020 6465 6620 7570  subs..    def up
+0000b200: 6461 7465 5f73 6c75 726d 5f73 6372 6970  date_slurm_scrip
+0000b210: 7473 2873 656c 662c 0a20 2020 2020 2020  ts(self,.       
+0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b230: 2020 2020 2020 6765 6e65 7261 7465 5f6a        generate_j
+0000b240: 6f62 733a 2062 6f6f 6c20 3d20 4661 6c73  obs: bool = Fals
+0000b250: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b270: 656e 763a 204f 7074 696f 6e61 6c5b 4469  env: Optional[Di
+0000b280: 6374 5b73 7472 2c20 7374 725d 5d20 3d20  ct[str, str]] = 
+0000b290: 4e6f 6e65 2920 2d3e 2052 6573 756c 743a  None) -> Result:
+0000b2a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000b2b0: 2020 2020 2055 7064 6174 6573 2074 6865       Updates the
+0000b2c0: 206c 6f63 616c 2063 6f70 7920 6f66 2074   local copy of t
+0000b2d0: 6865 2053 6c75 726d 206a 6f62 2073 7562  he Slurm job sub
+0000b2e0: 6d69 7373 696f 6e20 7363 7269 7074 732e  mission scripts.
+0000b2f0: 0a0a 2020 2020 2020 2020 5468 6973 2066  ..        This f
+0000b300: 756e 6374 696f 6e20 7075 6c6c 7320 7468  unction pulls th
+0000b310: 6520 6c61 7465 7374 2076 6572 7369 6f6e  e latest version
+0000b320: 206f 6620 7468 6520 7363 7269 7074 7320   of the scripts 
+0000b330: 6672 6f6d 2074 6865 2047 6974 0a20 2020  from the Git.   
+0000b340: 2020 2020 2072 6570 6f73 6974 6f72 7920       repository 
+0000b350: 616e 6420 636f 7069 6573 2074 6865 6d20  and copies them 
+0000b360: 746f 2074 6865 2073 6c75 726d 5f73 6372  to the slurm_scr
+0000b370: 6970 745f 7061 7468 2064 6972 6563 746f  ipt_path directo
+0000b380: 7279 2e0a 2020 2020 2020 2020 416c 7465  ry..        Alte
+0000b390: 726e 6174 6976 656c 792c 2069 7420 6361  rnatively, it ca
+0000b3a0: 6e20 6765 6e65 7261 7465 2073 6372 6970  n generate scrip
+0000b3b0: 7473 2066 726f 6d20 6120 7465 6d70 6c61  ts from a templa
+0000b3c0: 7465 2e20 5468 6973 2069 7320 7468 650a  te. This is the.
+0000b3d0: 2020 2020 2020 2020 6465 6661 756c 7420          default 
+0000b3e0: 6265 6861 7669 6f72 2069 6620 6e6f 2047  behavior if no G
+0000b3f0: 6974 2072 6570 6f20 6973 2070 726f 7669  it repo is provi
+0000b400: 6465 6420 6f72 2063 616e 2062 6520 666f  ded or can be fo
+0000b410: 7263 6564 2076 6961 2074 6865 0a20 2020  rced via the.   
+0000b420: 2020 2020 2060 6765 6e65 7261 7465 5f6a       `generate_j
+0000b430: 6f62 7360 2070 6172 616d 6574 6572 2e0a  obs` parameter..
+0000b440: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0000b450: 2020 2020 2020 2020 2020 2067 656e 6572             gener
+0000b460: 6174 655f 6a6f 6273 2028 626f 6f6c 293a  ate_jobs (bool):
+0000b470: 2057 6865 7468 6572 2074 6f20 6765 6e65   Whether to gene
+0000b480: 7261 7465 206e 6577 2073 6c75 726d 206a  rate new slurm j
+0000b490: 6f62 2073 6372 6970 7473 0a20 2020 2020  ob scripts.     
+0000b4a0: 2020 2020 2020 2020 2020 2049 4e53 5445             INSTE
+0000b4b0: 4144 2028 6f66 2070 756c 6c69 6e67 2066  AD (of pulling f
+0000b4c0: 726f 6d20 6769 7429 2e20 4465 6661 756c  rom git). Defaul
+0000b4d0: 7473 2074 6f20 4661 6c73 652c 2065 7863  ts to False, exc
+0000b4e0: 6570 740a 2020 2020 2020 2020 2020 2020  ept.            
+0000b4f0: 2020 2020 6966 206e 6f20 736c 7572 6d5f      if no slurm_
+0000b500: 7363 7269 7074 5f72 6570 6f20 6973 2063  script_repo is c
+0000b510: 6f6e 6669 6775 7265 642e 0a20 2020 2020  onfigured..     
+0000b520: 2020 2020 2020 2065 6e76 2028 4469 6374         env (Dict
+0000b530: 5b73 7472 2c20 7374 725d 2c20 6f70 7469  [str, str], opti
+0000b540: 6f6e 616c 293a 204f 7074 696f 6e61 6c20  onal): Optional 
+0000b550: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+0000b560: 6162 6c65 7320 0a20 2020 2020 2020 2020  ables .         
+0000b570: 2020 2020 2020 2074 6f20 7365 7420 7768         to set wh
+0000b580: 656e 2072 756e 6e69 6e67 2074 6865 2063  en running the c
+0000b590: 6f6d 6d61 6e64 2e20 4465 6661 756c 7473  ommand. Defaults
+0000b5a0: 2074 6f20 4e6f 6e65 2e0a 0a20 2020 2020   to None...     
+0000b5b0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000b5c0: 2020 2020 2020 2020 5265 7375 6c74 3a20          Result: 
+0000b5d0: 5468 6520 7265 7375 6c74 206f 6620 7468  The result of th
+0000b5e0: 6520 636f 6d6d 616e 642e 0a20 2020 2020  e command..     
+0000b5f0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+0000b600: 6620 6e6f 7420 7365 6c66 2e73 6c75 726d  f not self.slurm
+0000b610: 5f73 6372 6970 745f 7265 706f 3a0a 2020  _script_repo:.  
+0000b620: 2020 2020 2020 2020 2020 6765 6e65 7261            genera
+0000b630: 7465 5f6a 6f62 7320 3d20 5472 7565 0a0a  te_jobs = True..
+0000b640: 2020 2020 2020 2020 6966 2067 656e 6572          if gener
+0000b650: 6174 655f 6a6f 6273 3a0a 2020 2020 2020  ate_jobs:.      
+0000b660: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+0000b670: 6f28 2247 656e 6572 6174 696e 6720 536c  o("Generating Sl
+0000b680: 7572 6d20 6a6f 6220 7363 7269 7074 7322  urm job scripts"
+0000b690: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
+0000b6a0: 7220 7766 2c20 6a6f 625f 7061 7468 2069  r wf, job_path i
+0000b6b0: 6e20 7365 6c66 2e73 6c75 726d 5f6d 6f64  n self.slurm_mod
+0000b6c0: 656c 5f6a 6f62 732e 6974 656d 7328 293a  el_jobs.items():
+0000b6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b6e0: 2023 2067 656e 6572 6174 6520 6a6f 6220   # generate job 
+0000b6f0: 7363 7269 7074 0a20 2020 2020 2020 2020  script.         
+0000b700: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
+0000b710: 7365 6c66 2e67 6574 5f77 6f72 6b66 6c6f  self.get_workflo
+0000b720: 775f 7061 7261 6d65 7465 7273 2877 6629  w_parameters(wf)
+0000b730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b740: 2073 7562 7320 3d20 7365 6c66 2e77 6f72   subs = self.wor
+0000b750: 6b66 6c6f 775f 7061 7261 6d73 5f74 6f5f  kflow_params_to_
+0000b760: 7375 6273 2870 6172 616d 7329 0a20 2020  subs(params).   
+0000b770: 2020 2020 2020 2020 2020 2020 206a 6f62               job
+0000b780: 5f73 6372 6970 7420 3d20 7365 6c66 2e67  _script = self.g
+0000b790: 656e 6572 6174 655f 736c 7572 6d5f 6a6f  enerate_slurm_jo
+0000b7a0: 625f 666f 725f 776f 726b 666c 6f77 2877  b_for_workflow(w
+0000b7b0: 662c 2073 7562 7329 0a20 2020 2020 2020  f, subs).       
+0000b7c0: 2020 2020 2020 2020 2023 2065 6e73 7572           # ensur
+0000b7d0: 6520 616c 6c20 6469 7273 2065 7869 7374  e all dirs exist
+0000b7e0: 2072 656d 6f74 656c 790a 2020 2020 2020   remotely.      
+0000b7f0: 2020 2020 2020 2020 2020 6675 6c6c 5f70            full_p
+0000b800: 6174 6820 3d20 7365 6c66 2e73 6c75 726d  ath = self.slurm
+0000b810: 5f73 6372 6970 745f 7061 7468 2b22 2f22  _script_path+"/"
+0000b820: 2b6a 6f62 5f70 6174 680a 2020 2020 2020  +job_path.      
+0000b830: 2020 2020 2020 2020 2020 6a6f 625f 6469            job_di
+0000b840: 722c 205f 203d 206f 732e 7061 7468 2e73  r, _ = os.path.s
+0000b850: 706c 6974 2866 756c 6c5f 7061 7468 290a  plit(full_path).
+0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b870: 7365 6c66 2e72 756e 2866 226d 6b64 6972  self.run(f"mkdir
+0000b880: 202d 7020 5c22 7b6a 6f62 5f64 6972 7d5c   -p \"{job_dir}\
+0000b890: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
+0000b8a0: 2020 2020 2320 636f 7079 2074 6f20 7265      # copy to re
+0000b8b0: 6d6f 7465 2066 696c 650a 2020 2020 2020  mote file.      
+0000b8c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000b8d0: 203d 2073 656c 662e 7075 7428 6c6f 6361   = self.put(loca
+0000b8e0: 6c3d 696f 2e53 7472 696e 6749 4f28 6a6f  l=io.StringIO(jo
+0000b8f0: 625f 7363 7269 7074 292c 0a20 2020 2020  b_script),.     
+0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b910: 2020 2020 2020 2020 2020 2020 2072 656d               rem
+0000b920: 6f74 653d 6675 6c6c 5f70 6174 6829 0a20  ote=full_path). 
+0000b930: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000b940: 2020 2020 2020 2020 2063 6d64 203d 2073           cmd = s
+0000b950: 656c 662e 6765 745f 7570 6461 7465 5f73  elf.get_update_s
+0000b960: 6c75 726d 5f73 6372 6970 7473 5f63 6f6d  lurm_scripts_com
+0000b970: 6d61 6e64 2829 0a20 2020 2020 2020 2020  mand().         
+0000b980: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
+0000b990: 5570 6461 7469 6e67 2053 6c75 726d 206a  Updating Slurm j
+0000b9a0: 6f62 2073 6372 6970 7473 206f 6e20 536c  ob scripts on Sl
+0000b9b0: 7572 6d22 290a 2020 2020 2020 2020 2020  urm").          
+0000b9c0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
+0000b9d0: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
+0000b9e0: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
+0000b9f0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+0000ba00: 6c74 0a0a 2020 2020 6465 6620 7275 6e5f  lt..    def run_
+0000ba10: 776f 726b 666c 6f77 2873 656c 662c 0a20  workflow(self,. 
+0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba30: 2020 2020 776f 726b 666c 6f77 5f6e 616d      workflow_nam
+0000ba40: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
+0000ba50: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
+0000ba60: 6b66 6c6f 775f 7665 7273 696f 6e3a 2073  kflow_version: s
+0000ba70: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+0000ba80: 2020 2020 2020 2020 2069 6e70 7574 5f64           input_d
+0000ba90: 6174 613a 2073 7472 2c0a 2020 2020 2020  ata: str,.      
+0000baa0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000bab0: 6d61 696c 3a20 4f70 7469 6f6e 616c 5b73  mail: Optional[s
+0000bac0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bae0: 2074 696d 653a 204f 7074 696f 6e61 6c5b   time: Optional[
+0000baf0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
 0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb10: 2020 2020 2020 2077 6f72 6b66 6c6f 775f         workflow_
-0000bb20: 7665 7273 696f 6e3a 2073 7472 2c0a 2020  version: str,.  
-0000bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb40: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
-0000bb50: 613a 2073 7472 2c0a 2020 2020 2020 2020  a: str,.        
-0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb70: 2065 6d61 696c 3a20 4f70 7469 6f6e 616c   email: Optional
-0000bb80: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-0000bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bba0: 2020 2020 2020 2074 696d 653a 204f 7074         time: Opt
-0000bbb0: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000bbc0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000bbd0: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
-0000bbe0: 6172 6773 0a20 2020 2020 2020 2020 2020  args.           
-0000bbf0: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
-0000bc00: 2d3e 2053 6c75 726d 4a6f 623a 0a20 2020  -> SlurmJob:.   
-0000bc10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000bc20: 2052 756e 2061 2073 7065 6369 6669 6564   Run a specified
-0000bc30: 2077 6f72 6b66 6c6f 7720 6f6e 2053 6c75   workflow on Slu
-0000bc40: 726d 2075 7369 6e67 2074 6865 2067 6976  rm using the giv
-0000bc50: 656e 2070 6172 616d 6574 6572 7320 616e  en parameters an
-0000bc60: 6420 7265 7475 726e 2061 2053 6c75 726d  d return a Slurm
-0000bc70: 4a6f 6220 696e 7374 616e 6365 2e0a 0a20  Job instance... 
-0000bc80: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000bc90: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
-0000bca0: 775f 6e61 6d65 2028 7374 7229 3a20 4e61  w_name (str): Na
-0000bcb0: 6d65 206f 6620 7468 6520 776f 726b 666c  me of the workfl
-0000bcc0: 6f77 2074 6f20 6578 6563 7574 652e 0a20  ow to execute.. 
-0000bcd0: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
-0000bce0: 6c6f 775f 7665 7273 696f 6e20 2873 7472  low_version (str
-0000bcf0: 293a 2056 6572 7369 6f6e 206f 6620 7468  ): Version of th
-0000bd00: 6520 776f 726b 666c 6f77 2028 696d 6167  e workflow (imag
-0000bd10: 6520 7665 7273 696f 6e20 6f6e 2053 6c75  e version on Slu
-0000bd20: 726d 292e 0a20 2020 2020 2020 2020 2020  rm)..           
-0000bd30: 2069 6e70 7574 5f64 6174 6120 2873 7472   input_data (str
-0000bd40: 293a 204e 616d 6520 6f66 2074 6865 2069  ): Name of the i
-0000bd50: 6e70 7574 2064 6174 6120 666f 6c64 6572  nput data folder
-0000bd60: 2063 6f6e 7461 696e 696e 6720 696e 7075   containing inpu
-0000bd70: 7420 696d 6167 6520 6669 6c65 732e 0a20  t image files.. 
-0000bd80: 2020 2020 2020 2020 2020 2065 6d61 696c             email
-0000bd90: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
-0000bda0: 3a20 456d 6169 6c20 6164 6472 6573 7320  : Email address 
-0000bdb0: 666f 7220 536c 7572 6d20 6a6f 6220 6e6f  for Slurm job no
-0000bdc0: 7469 6669 6361 7469 6f6e 732e 0a20 2020  tifications..   
-0000bdd0: 2020 2020 2020 2020 2074 696d 6520 2873           time (s
-0000bde0: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
-0000bdf0: 696d 6520 6c69 6d69 7420 666f 7220 7468  ime limit for th
-0000be00: 6520 536c 7572 6d20 6a6f 6220 696e 2074  e Slurm job in t
-0000be10: 6865 2066 6f72 6d61 7420 4848 3a4d 4d3a  he format HH:MM:
-0000be20: 5353 2e0a 2020 2020 2020 2020 2020 2020  SS..            
-0000be30: 2a2a 6b77 6172 6773 3a20 4164 6469 7469  **kwargs: Additi
-0000be40: 6f6e 616c 206b 6579 776f 7264 2061 7267  onal keyword arg
-0000be50: 756d 656e 7473 2066 6f72 2074 6865 2077  uments for the w
-0000be60: 6f72 6b66 6c6f 772e 0a0a 2020 2020 2020  orkflow...      
-0000be70: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000be80: 2020 2020 2020 2053 6c75 726d 4a6f 623a         SlurmJob:
-0000be90: 2041 2053 6c75 726d 4a6f 6220 696e 7374   A SlurmJob inst
-0000bea0: 616e 6365 2072 6570 7265 7365 6e74 696e  ance representin
-0000beb0: 6720 7468 6520 7374 6172 7465 6420 776f  g the started wo
-0000bec0: 726b 666c 6f77 206a 6f62 2e0a 2020 2020  rkflow job..    
-0000bed0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000bee0: 7265 7375 6c74 2c20 6a6f 625f 6964 203d  result, job_id =
-0000bef0: 2073 656c 662e 7275 6e5f 776f 726b 666c   self.run_workfl
-0000bf00: 6f77 280a 2020 2020 2020 2020 2020 2020  ow(.            
-0000bf10: 776f 726b 666c 6f77 5f6e 616d 652c 2077  workflow_name, w
-0000bf20: 6f72 6b66 6c6f 775f 7665 7273 696f 6e2c  orkflow_version,
-0000bf30: 2069 6e70 7574 5f64 6174 612c 2065 6d61   input_data, ema
-0000bf40: 696c 2c20 7469 6d65 2c20 2a2a 6b77 6172  il, time, **kwar
-0000bf50: 6773 290a 2020 2020 2020 2020 7265 7475  gs).        retu
-0000bf60: 726e 2053 6c75 726d 4a6f 6228 7265 7375  rn SlurmJob(resu
-0000bf70: 6c74 2c20 6a6f 625f 6964 290a 0a20 2020  lt, job_id)..   
-0000bf80: 2064 6566 2072 756e 5f63 6f6e 7665 7273   def run_convers
-0000bf90: 696f 6e5f 776f 726b 666c 6f77 5f6a 6f62  ion_workflow_job
-0000bfa0: 2873 656c 662c 2066 6f6c 6465 725f 6e61  (self, folder_na
-0000bfb0: 6d65 3a20 7374 722c 0a20 2020 2020 2020  me: str,.       
-0000bfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfd0: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
-0000bfe0: 7263 655f 666f 726d 6174 3a20 7374 7220  rce_format: str 
-0000bff0: 3d20 277a 6172 7227 2c0a 2020 2020 2020  = 'zarr',.      
-0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c010: 2020 2020 2020 2020 2020 2020 2020 7461                ta
-0000c020: 7267 6574 5f66 6f72 6d61 743a 2073 7472  rget_format: str
-0000c030: 203d 2027 7469 6666 270a 2020 2020 2020   = 'tiff'.      
-0000c040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c050: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
-0000c060: 2d3e 2054 7570 6c65 5b52 6573 756c 742c  -> Tuple[Result,
-0000c070: 2069 6e74 5d3a 0a20 2020 2020 2020 2022   int]:.        "
-0000c080: 2222 0a20 2020 2020 2020 2052 756e 2074  "".        Run t
-0000c090: 6865 2064 6174 6120 636f 6e76 6572 7369  he data conversi
-0000c0a0: 6f6e 2077 6f72 6b66 6c6f 7720 6f6e 2053  on workflow on S
-0000c0b0: 6c75 726d 2075 7369 6e67 2074 6865 2067  lurm using the g
-0000c0c0: 6976 656e 2064 6174 6120 666f 6c64 6572  iven data folder
-0000c0d0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-0000c0e0: 0a20 2020 2020 2020 2020 2020 2066 6f6c  .            fol
-0000c0f0: 6465 725f 6e61 6d65 2028 7374 7229 3a20  der_name (str): 
-0000c100: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-0000c110: 6461 7461 2066 6f6c 6465 7220 636f 6e74  data folder cont
-0000c120: 6169 6e69 6e67 2073 6f75 7263 6520 666f  aining source fo
-0000c130: 726d 6174 2066 696c 6573 2e0a 2020 2020  rmat files..    
-0000c140: 2020 2020 2020 2020 736f 7572 6365 5f66          source_f
-0000c150: 6f72 6d61 7420 2873 7472 293a 2053 6f75  ormat (str): Sou
-0000c160: 7263 6520 6461 7461 2066 6f72 6d61 7420  rce data format 
-0000c170: 666f 7220 636f 6e76 6572 7369 6f6e 2028  for conversion (
-0000c180: 6465 6661 756c 7420 6973 2027 7a61 7272  default is 'zarr
-0000c190: 2729 2e0a 2020 2020 2020 2020 2020 2020  ')..            
-0000c1a0: 7461 7267 6574 5f66 6f72 6d61 7420 2873  target_format (s
-0000c1b0: 7472 293a 2054 6172 6765 7420 6461 7461  tr): Target data
-0000c1c0: 2066 6f72 6d61 7420 6166 7465 7220 636f   format after co
-0000c1d0: 6e76 6572 7369 6f6e 2028 6465 6661 756c  nversion (defaul
-0000c1e0: 7420 6973 2027 7469 6666 2729 2e0a 0a20  t is 'tiff')... 
-0000c1f0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000c200: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
-0000c210: 655b 5265 7375 6c74 2c20 696e 745d 3a0a  e[Result, int]:.
-0000c220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c230: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
-0000c240: 6e67 2074 6865 2072 6573 756c 7420 6f66  ng the result of
-0000c250: 2073 7461 7274 696e 6720 7468 6520 636f   starting the co
-0000c260: 6e76 6572 7369 6f6e 206a 6f62 2061 6e64  nversion job and
-0000c270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c280: 2074 6865 2053 6c75 726d 206a 6f62 2049   the Slurm job I
-0000c290: 442c 206f 7220 2d31 2069 6620 7468 6520  D, or -1 if the 
-0000c2a0: 6a6f 6220 4944 2063 6f75 6c64 206e 6f74  job ID could not
-0000c2b0: 2062 6520 6578 7472 6163 7465 642e 0a0a   be extracted...
-0000c2c0: 2020 2020 2020 2020 5761 726e 696e 673a          Warning:
-0000c2d0: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
-0000c2e0: 2064 6566 6175 6c74 2069 6d70 6c65 6d65   default impleme
-0000c2f0: 6e74 6174 696f 6e20 6f6e 6c79 2073 7570  ntation only sup
-0000c300: 706f 7274 7320 636f 6e76 6572 7369 6f6e  ports conversion
-0000c310: 2066 726f 6d20 277a 6172 7227 2074 6f20   from 'zarr' to 
-0000c320: 2774 6966 6627 2e0a 2020 2020 2020 2020  'tiff'..        
-0000c330: 2020 2020 4966 2075 7369 6e67 206f 7468      If using oth
-0000c340: 6572 2073 6f75 7263 6520 6f72 2074 6172  er source or tar
-0000c350: 6765 7420 666f 726d 6174 732c 2075 7365  get formats, use
-0000c360: 7273 206d 7573 7420 696d 706c 656d 656e  rs must implemen
-0000c370: 7420 616e 6420 636f 6e66 6967 7572 650a  t and configure.
-0000c380: 2020 2020 2020 2020 2020 2020 6164 6469              addi
-0000c390: 7469 6f6e 616c 2063 6f6e 7665 7274 6572  tional converter
-0000c3a0: 7320 7468 656d 7365 6c76 6573 2e0a 2020  s themselves..  
-0000c3b0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000c3c0: 2020 2320 4765 6e65 7261 7465 2061 2075    # Generate a u
-0000c3d0: 6e69 7175 6520 636f 6e66 6967 2066 696c  nique config fil
-0000c3e0: 6520 6e61 6d65 0a20 2020 2020 2020 2063  e name.        c
-0000c3f0: 6f6e 6669 675f 6669 6c65 203d 2066 2263  onfig_file = f"c
-0000c400: 6f6e 6669 675f 7b66 6f6c 6465 725f 6e61  onfig_{folder_na
-0000c410: 6d65 7d2e 7478 7422 0a0a 2020 2020 2020  me}.txt"..      
-0000c420: 2020 2320 436f 6e73 7472 7563 7420 616c    # Construct al
-0000c430: 6c20 636f 6d6d 616e 6473 2074 6f20 7275  l commands to ru
-0000c440: 6e20 636f 6e73 6563 7574 6976 656c 790a  n consecutively.
-0000c450: 2020 2020 2020 2020 6461 7461 5f70 6174          data_pat
-0000c460: 6820 3d20 6622 7b73 656c 662e 736c 7572  h = f"{self.slur
-0000c470: 6d5f 6461 7461 5f70 6174 687d 2f7b 666f  m_data_path}/{fo
-0000c480: 6c64 6572 5f6e 616d 657d 220a 2020 2020  lder_name}".    
-0000c490: 2020 2020 636f 6e76 6572 7369 6f6e 5f63      conversion_c
-0000c4a0: 6d64 2c20 7362 6174 6368 5f65 6e76 203d  md, sbatch_env =
-0000c4b0: 2073 656c 662e 6765 745f 636f 6e76 6572   self.get_conver
-0000c4c0: 7369 6f6e 5f63 6f6d 6d61 6e64 280a 2020  sion_command(.  
-0000c4d0: 2020 2020 2020 2020 2020 6461 7461 5f70            data_p
-0000c4e0: 6174 682c 2063 6f6e 6669 675f 6669 6c65  ath, config_file
-0000c4f0: 2c20 736f 7572 6365 5f66 6f72 6d61 742c  , source_format,
-0000c500: 2074 6172 6765 745f 666f 726d 6174 290a   target_format).
-0000c510: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
-0000c520: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-0000c530: 2066 2266 696e 6420 7b64 6174 615f 7061   f"find {data_pa
-0000c540: 7468 7d2f 6461 7461 2f69 6e20 2d6e 616d  th}/data/in -nam
-0000c550: 6520 272a 2e7b 736f 7572 6365 5f66 6f72  e '*.{source_for
-0000c560: 6d61 747d 2720 7c20 6177 6b20 277b 7b70  mat}' | awk '{{p
-0000c570: 7269 6e74 204e 522c 2024 307d 7d27 203e  rint NR, $0}}' >
-0000c580: 207b 636f 6e66 6967 5f66 696c 657d 222c   {config_file}",
-0000c590: 0a20 2020 2020 2020 2020 2020 2066 224e  .            f"N
-0000c5a0: 3d24 2877 6320 2d6c 203c 205c 227b 636f  =$(wc -l < \"{co
-0000c5b0: 6e66 6967 5f66 696c 657d 5c22 2922 2c0a  nfig_file}\")",.
-0000c5c0: 2020 2020 2020 2020 2020 2020 6622 6563              f"ec
-0000c5d0: 686f 205c 224e 756d 6265 7220 6f66 202e  ho \"Number of .
-0000c5e0: 7b73 6f75 7263 655f 666f 726d 6174 7d20  {source_format} 
-0000c5f0: 6669 6c65 733a 2024 4e5c 2222 2c0a 2020  files: $N\"",.  
-0000c600: 2020 2020 2020 2020 2020 636f 6e76 6572            conver
-0000c610: 7369 6f6e 5f63 6d64 0a20 2020 2020 2020  sion_cmd.       
-0000c620: 205d 0a0a 2020 2020 2020 2020 2320 5275   ]..        # Ru
-0000c630: 6e20 616c 6c20 636f 6d6d 616e 6473 2063  n all commands c
-0000c640: 6f6e 7365 6375 7469 7665 6c79 0a20 2020  onsecutively.   
-0000c650: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
-0000c660: 7275 6e5f 636f 6d6d 616e 6473 2863 6f6d  run_commands(com
-0000c670: 6d61 6e64 732c 2073 6261 7463 685f 656e  mands, sbatch_en
-0000c680: 7629 0a0a 2020 2020 2020 2020 7265 7475  v)..        retu
-0000c690: 726e 2053 6c75 726d 4a6f 6228 7265 732c  rn SlurmJob(res,
-0000c6a0: 2073 656c 662e 6578 7472 6163 745f 6a6f   self.extract_jo
-0000c6b0: 625f 6964 2872 6573 2929 0a0a 2020 2020  b_id(res))..    
-0000c6c0: 6465 6620 6578 7472 6163 745f 6a6f 625f  def extract_job_
-0000c6d0: 6964 2873 656c 662c 2072 6573 756c 743a  id(self, result:
-0000c6e0: 2052 6573 756c 7429 202d 3e20 696e 743a   Result) -> int:
-0000c6f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c700: 2020 2020 2045 7874 7261 6374 2074 6865       Extract the
-0000c710: 2053 6c75 726d 206a 6f62 2049 4420 6672   Slurm job ID fr
-0000c720: 6f6d 2074 6865 2072 6573 756c 7420 6f66  om the result of
-0000c730: 2061 2063 6f6d 6d61 6e64 2e0a 0a20 2020   a command...   
-0000c740: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000c750: 2020 2020 2020 2072 6573 756c 7420 2852         result (R
-0000c760: 6573 756c 7429 3a20 5468 6520 7265 7375  esult): The resu
-0000c770: 6c74 206f 6620 6120 636f 6d6d 616e 6420  lt of a command 
-0000c780: 6578 6563 7574 696f 6e2e 0a0a 2020 2020  execution...    
-0000c790: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0000c7a0: 2020 2020 2020 2020 2069 6e74 3a0a 2020           int:.  
-0000c7b0: 2020 2020 2020 2020 2020 2020 2020 5468                Th
-0000c7c0: 6520 536c 7572 6d20 6a6f 6220 4944 2065  e Slurm job ID e
-0000c7d0: 7874 7261 6374 6564 2066 726f 6d20 7468  xtracted from th
-0000c7e0: 6520 7265 7375 6c74 2c0a 2020 2020 2020  e result,.      
-0000c7f0: 2020 2020 2020 2020 2020 6f72 202d 3120            or -1 
-0000c800: 6966 206e 6f74 2066 6f75 6e64 2e0a 2020  if not found..  
-0000c810: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000c820: 2020 736c 7572 6d5f 6a6f 625f 6964 203d    slurm_job_id =
-0000c830: 206e 6578 7428 2869 6e74 2873 2e73 7472   next((int(s.str
-0000c840: 6970 2829 2920 666f 7220 7320 696e 2072  ip()) for s in r
-0000c850: 6573 756c 742e 7374 646f 7574 2e73 706c  esult.stdout.spl
-0000c860: 6974 280a 2020 2020 2020 2020 2020 2020  it(.            
-0000c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c880: 2253 7562 6d69 7474 6564 2062 6174 6368  "Submitted batch
-0000c890: 206a 6f62 2229 2069 6620 732e 7374 7269   job") if s.stri
-0000c8a0: 7028 292e 6973 6469 6769 7428 2929 2c20  p().isdigit()), 
-0000c8b0: 2d31 290a 2020 2020 2020 2020 7265 7475  -1).        retu
-0000c8c0: 726e 2073 6c75 726d 5f6a 6f62 5f69 640a  rn slurm_job_id.
-0000c8d0: 0a20 2020 2064 6566 2067 6574 5f75 7064  .    def get_upd
-0000c8e0: 6174 655f 736c 7572 6d5f 7363 7269 7074  ate_slurm_script
-0000c8f0: 735f 636f 6d6d 616e 6428 7365 6c66 2920  s_command(self) 
-0000c900: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
-0000c910: 2222 2247 656e 6572 6174 6520 7468 6520  """Generate the 
-0000c920: 636f 6d6d 616e 6420 746f 2075 7064 6174  command to updat
-0000c930: 6520 7468 6520 4769 7420 7265 706f 7369  e the Git reposi
-0000c940: 746f 7279 2063 6f6e 7461 696e 696e 670a  tory containing.
-0000c950: 2020 2020 2020 2020 7468 6520 536c 7572          the Slur
-0000c960: 6d20 7363 7269 7074 732c 2069 6620 6e65  m scripts, if ne
-0000c970: 6365 7373 6172 792e 0a0a 2020 2020 2020  cessary...      
-0000c980: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000c990: 2020 2020 2020 2073 7472 3a0a 2020 2020         str:.    
-0000c9a0: 2020 2020 2020 2020 2020 2020 4120 7374              A st
-0000c9b0: 7269 6e67 2063 6f6e 7461 696e 696e 6720  ring containing 
-0000c9c0: 7468 6520 4769 7420 636f 6d6d 616e 640a  the Git command.
-0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9e0: 746f 2075 7064 6174 6520 7468 6520 536c  to update the Sl
-0000c9f0: 7572 6d20 7363 7269 7074 732e 0a20 2020  urm scripts..   
-0000ca00: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000ca10: 2075 7064 6174 655f 636d 6420 3d20 6622   update_cmd = f"
-0000ca20: 6769 7420 2d43 207b 7365 6c66 2e73 6c75  git -C {self.slu
-0000ca30: 726d 5f73 6372 6970 745f 7061 7468 7d20  rm_script_path} 
-0000ca40: 7075 6c6c 220a 2020 2020 2020 2020 7265  pull".        re
-0000ca50: 7475 726e 2075 7064 6174 655f 636d 640a  turn update_cmd.
-0000ca60: 0a20 2020 2064 6566 2063 6865 636b 5f6a  .    def check_j
-0000ca70: 6f62 5f73 7461 7475 7328 7365 6c66 2c0a  ob_status(self,.
-0000ca80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca90: 2020 2020 2020 2020 2073 6c75 726d 5f6a           slurm_j
-0000caa0: 6f62 5f69 6473 3a20 4c69 7374 5b69 6e74  ob_ids: List[int
-0000cab0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
-0000cac0: 2020 2020 2020 2020 2020 2020 656e 763a              env:
-0000cad0: 204f 7074 696f 6e61 6c5b 4469 6374 5b73   Optional[Dict[s
-0000cae0: 7472 2c20 7374 725d 5d20 3d20 4e6f 6e65  tr, str]] = None
-0000caf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cb00: 2020 2020 2020 2020 2020 2920 2d3e 2054            ) -> T
-0000cb10: 7570 6c65 5b44 6963 745b 696e 742c 2073  uple[Dict[int, s
-0000cb20: 7472 5d2c 2052 6573 756c 745d 3a0a 2020  tr], Result]:.  
-0000cb30: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000cb40: 2020 4368 6563 6b20 7468 6520 7374 6174    Check the stat
-0000cb50: 7573 206f 6620 536c 7572 6d20 6a6f 6273  us of Slurm jobs
-0000cb60: 2077 6974 6820 7468 6520 6769 7665 6e20   with the given 
-0000cb70: 6a6f 6220 4944 732e 0a0a 2020 2020 2020  job IDs...      
-0000cb80: 2020 4e6f 7465 3a20 5468 6973 2064 6f65    Note: This doe
-0000cb90: 736e 2774 2072 6574 7572 6e20 6a6f 6220  sn't return job 
-0000cba0: 6172 7261 7973 2069 6e64 6976 6964 7561  arrays individua
-0000cbb0: 6c6c 792e 0a20 2020 2020 2020 2049 7420  lly..        It 
-0000cbc0: 7461 6b65 7320 7468 6520 6c61 7374 2076  takes the last v
-0000cbd0: 616c 7565 2072 6574 7572 6e65 6420 666f  alue returned fo
-0000cbe0: 7220 7468 6f73 6520 7375 6220 6964 7320  r those sub ids 
-0000cbf0: 0a20 2020 2020 2020 2028 6765 6e65 7261  .        (genera
-0000cc00: 6c6c 7920 7468 6520 6f6e 6520 7374 696c  lly the one stil
-0000cc10: 6c20 5045 4e44 494e 4729 2e0a 0a20 2020  l PENDING)...   
-0000cc20: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000cc30: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
-0000cc40: 5f69 6473 2028 4c69 7374 5b69 6e74 5d29  _ids (List[int])
-0000cc50: 3a20 5468 6520 6a6f 6220 4944 7320 6f66  : The job IDs of
-0000cc60: 2074 6865 2053 6c75 726d 206a 6f62 7320   the Slurm jobs 
-0000cc70: 746f 2063 6865 636b 2e0a 2020 2020 2020  to check..      
-0000cc80: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
-0000cc90: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
-0000cca0: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
-0000ccb0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-0000ccc0: 626c 6573 2074 6f0a 2020 2020 2020 2020  bles to.        
-0000ccd0: 2020 2020 2020 2020 7365 7420 7768 656e          set when
-0000cce0: 2072 756e 6e69 6e67 2074 6865 2063 6f6d   running the com
-0000ccf0: 6d61 6e64 2e20 4465 6661 756c 7473 2074  mand. Defaults t
-0000cd00: 6f20 4e6f 6e65 2e0a 0a20 2020 2020 2020  o None...       
-0000cd10: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0000cd20: 2020 2020 2020 5475 706c 655b 4469 6374        Tuple[Dict
-0000cd30: 5b69 6e74 2c20 7374 725d 2c20 5265 7375  [int, str], Resu
-0000cd40: 6c74 5d3a 0a20 2020 2020 2020 2020 2020  lt]:.           
-0000cd50: 2020 2020 2041 2074 7570 6c65 2063 6f6e       A tuple con
-0000cd60: 7461 696e 696e 6720 7468 6520 7374 6174  taining the stat
-0000cd70: 7573 2070 6572 2069 6e70 7574 2049 4420  us per input ID 
-0000cd80: 616e 6420 7468 6520 7265 7375 6c74 206f  and the result o
-0000cd90: 6620 0a20 2020 2020 2020 2020 2020 2020  f .             
-0000cda0: 2020 2074 6865 2063 6f6d 6d61 6e64 2065     the command e
-0000cdb0: 7865 6375 7469 6f6e 2e0a 0a20 2020 2020  xecution...     
-0000cdc0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-0000cdd0: 2020 2020 2020 2053 5348 4578 6365 7074         SSHExcept
-0000cde0: 696f 6e3a 2049 6620 7468 6520 636f 6d6d  ion: If the comm
-0000cdf0: 616e 6420 6578 6563 7574 696f 6e20 6661  and execution fa
-0000ce00: 696c 7320 6f72 206e 6f20 7265 7370 6f6e  ils or no respon
-0000ce10: 7365 2069 730a 2020 2020 2020 2020 2020  se is.          
-0000ce20: 2020 2020 2020 7265 6365 6976 6564 2061        received a
-0000ce30: 6674 6572 206d 756c 7469 706c 6520 7265  fter multiple re
-0000ce40: 7472 6965 732e 0a20 2020 2020 2020 2022  tries..        "
-0000ce50: 2222 0a20 2020 2020 2020 2063 6d64 203d  "".        cmd =
-0000ce60: 2073 656c 662e 6765 745f 6a6f 625f 7374   self.get_job_st
-0000ce70: 6174 7573 5f63 6f6d 6d61 6e64 2873 6c75  atus_command(slu
-0000ce80: 726d 5f6a 6f62 5f69 6473 290a 2020 2020  rm_job_ids).    
-0000ce90: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
-0000cea0: 6622 4765 7474 696e 6720 7374 6174 7573  f"Getting status
-0000ceb0: 206f 6620 7b73 6c75 726d 5f6a 6f62 5f69   of {slurm_job_i
-0000cec0: 6473 7d20 6f6e 2053 6c75 726d 2229 0a20  ds} on Slurm"). 
-0000ced0: 2020 2020 2020 2072 6574 7279 5f73 7461         retry_sta
-0000cee0: 7475 7320 3d20 300a 2020 2020 2020 2020  tus = 0.        
-0000cef0: 7768 696c 6520 7265 7472 795f 7374 6174  while retry_stat
-0000cf00: 7573 203c 2033 3a0a 2020 2020 2020 2020  us < 3:.        
-0000cf10: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-0000cf20: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
-0000cf30: 636d 645d 2c20 656e 763d 656e 7629 0a20  cmd], env=env). 
-0000cf40: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000cf50: 722e 696e 666f 2872 6573 756c 7429 0a20  r.info(result). 
-0000cf60: 2020 2020 2020 2020 2020 2069 6620 7265             if re
-0000cf70: 7375 6c74 2e6f 6b3a 0a20 2020 2020 2020  sult.ok:.       
-0000cf80: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
-0000cf90: 7265 7375 6c74 2e73 7464 6f75 743a 0a20  result.stdout:. 
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfb0: 2020 2023 2077 6169 7420 666f 7220 3320     # wait for 3 
-0000cfc0: 7365 636f 6e64 7320 6265 666f 7265 2063  seconds before c
-0000cfd0: 6865 636b 696e 6720 6167 6169 6e0a 2020  hecking again.  
-0000cfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cff0: 2020 7469 6d65 736c 6565 702e 736c 6565    timesleep.slee
-0000d000: 7028 3329 0a20 2020 2020 2020 2020 2020  p(3).           
-0000d010: 2020 2020 2020 2020 2023 2072 6574 7279           # retry
-0000d020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d030: 2020 2020 2072 6574 7279 5f73 7461 7475       retry_statu
-0000d040: 7320 2b3d 2031 0a20 2020 2020 2020 2020  s += 1.         
-0000d050: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-0000d060: 722e 6465 6275 6728 0a20 2020 2020 2020  r.debug(.       
-0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d080: 2066 2252 6574 7279 207b 7265 7472 795f   f"Retry {retry_
-0000d090: 7374 6174 7573 7d20 6765 7474 696e 6720  status} getting 
-0000d0a0: 7374 6174 7573 205c 0a20 2020 2020 2020  status \.       
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 2020 2020 206f 6620 7b73 6c75 726d 5f6a       of {slurm_j
-0000d0d0: 6f62 5f69 6473 7d21 2229 0a20 2020 2020  ob_ids}!").     
-0000d0e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000d0f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d100: 2020 2020 2023 0a20 2020 2020 2020 2020       #.         
-0000d110: 2020 2020 2020 2020 2020 206a 6f62 5f73             job_s
-0000d120: 7461 7475 735f 6469 6374 203d 207b 696e  tatus_dict = {in
-0000d130: 7428 6c69 6e65 2e73 706c 6974 2829 5b30  t(line.split()[0
-0000d140: 5d2e 7370 6c69 7428 275f 2729 5b30 5d29  ].split('_')[0])
-0000d150: 3a20 6c69 6e65 2e73 706c 6974 280a 2020  : line.split(.  
-0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d170: 2020 295b 315d 2066 6f72 206c 696e 6520    )[1] for line 
-0000d180: 696e 2072 6573 756c 742e 7374 646f 7574  in result.stdout
-0000d190: 2e73 706c 6974 2822 5c6e 2229 2069 6620  .split("\n") if 
-0000d1a0: 6c69 6e65 7d0a 2020 2020 2020 2020 2020  line}.          
-0000d1b0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000d1c0: 2e64 6562 7567 2866 224a 6f62 2073 7461  .debug(f"Job sta
-0000d1d0: 7475 7365 733a 207b 6a6f 625f 7374 6174  tuses: {job_stat
-0000d1e0: 7573 5f64 6963 747d 2229 0a20 2020 2020  us_dict}").     
-0000d1f0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000d200: 6574 7572 6e20 6a6f 625f 7374 6174 7573  eturn job_status
-0000d210: 5f64 6963 742c 2072 6573 756c 740a 2020  _dict, result.  
-0000d220: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d240: 6572 726f 7220 3d20 6622 5265 7375 6c74  error = f"Result
-0000d250: 2069 7320 6e6f 7420 6f6b 3a20 7b72 6573   is not ok: {res
-0000d260: 756c 747d 220a 2020 2020 2020 2020 2020  ult}".          
-0000d270: 2020 2020 2020 6c6f 6767 6572 2e65 7272        logger.err
-0000d280: 6f72 2865 7272 6f72 290a 2020 2020 2020  or(error).      
-0000d290: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000d2a0: 5353 4845 7863 6570 7469 6f6e 2865 7272  SSHException(err
-0000d2b0: 6f72 290a 2020 2020 2020 2020 656c 7365  or).        else
-0000d2c0: 3a0a 2020 2020 2020 2020 2020 2020 6572  :.            er
-0000d2d0: 726f 7220 3d20 6622 4572 726f 723a 2052  ror = f"Error: R
-0000d2e0: 6574 7269 6564 207b 7265 7472 795f 7374  etried {retry_st
-0000d2f0: 6174 7573 7d20 7469 6d65 7320 746f 2067  atus} times to g
-0000d300: 6574 205c 0a20 2020 2020 2020 2020 2020  et \.           
-0000d310: 2020 2020 2073 7461 7475 7320 6f66 207b       status of {
-0000d320: 736c 7572 6d5f 6a6f 625f 6964 737d 2c20  slurm_job_ids}, 
-0000d330: 6275 7420 6e6f 2072 6573 706f 6e73 652e  but no response.
-0000d340: 220a 2020 2020 2020 2020 2020 2020 6c6f  ".            lo
-0000d350: 6767 6572 2e65 7272 6f72 2865 7272 6f72  gger.error(error
-0000d360: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
-0000d370: 6973 6520 5353 4845 7863 6570 7469 6f6e  ise SSHException
-0000d380: 2865 7272 6f72 290a 0a20 2020 2064 6566  (error)..    def
-0000d390: 2067 6574 5f6a 6f62 5f73 7461 7475 735f   get_job_status_
-0000d3a0: 636f 6d6d 616e 6428 7365 6c66 2c20 736c  command(self, sl
-0000d3b0: 7572 6d5f 6a6f 625f 6964 733a 204c 6973  urm_job_ids: Lis
-0000d3c0: 745b 696e 745d 2920 2d3e 2073 7472 3a0a  t[int]) -> str:.
-0000d3d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000d3e0: 2020 2020 5265 7475 726e 2074 6865 2053      Return the S
-0000d3f0: 6c75 726d 2063 6f6d 6d61 6e64 2074 6f20  lurm command to 
-0000d400: 6765 7420 7468 6520 7374 6174 7573 206f  get the status o
-0000d410: 6620 6a6f 6273 2077 6974 6820 7468 6520  f jobs with the 
-0000d420: 6769 7665 6e0a 2020 2020 2020 2020 6a6f  given.        jo
-0000d430: 6220 4944 732e 0a0a 2020 2020 2020 2020  b IDs...        
-0000d440: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000d450: 2020 736c 7572 6d5f 6a6f 625f 6964 7320    slurm_job_ids 
-0000d460: 284c 6973 745b 696e 745d 293a 2054 6865  (List[int]): The
-0000d470: 206a 6f62 2049 4473 206f 6620 7468 6520   job IDs of the 
-0000d480: 6a6f 6273 2074 6f20 6368 6563 6b2e 0a0a  jobs to check...
-0000d490: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0000d4a0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-0000d4b0: 3a20 0a20 2020 2020 2020 2020 2020 2020  : .             
-0000d4c0: 2020 2054 6865 2053 6c75 726d 2063 6f6d     The Slurm com
-0000d4d0: 6d61 6e64 2074 6f20 6765 7420 7468 6520  mand to get the 
-0000d4e0: 7374 6174 7573 206f 6620 7468 6520 6a6f  status of the jo
-0000d4f0: 6273 2e0a 2020 2020 2020 2020 2222 220a  bs..        """.
-0000d500: 2020 2020 2020 2020 2320 636f 6e63 6174          # concat
-0000d510: 206d 756c 7469 706c 6520 6a6f 6273 2069   multiple jobs i
-0000d520: 6620 6e65 6564 6564 0a20 2020 2020 2020  f needed.       
-0000d530: 2073 6c75 726d 5f6a 6f62 5f69 6420 3d20   slurm_job_id = 
-0000d540: 2220 2d6a 2022 2e6a 6f69 6e28 5b73 7472  " -j ".join([str
-0000d550: 2869 6429 2066 6f72 2069 6420 696e 2073  (id) for id in s
-0000d560: 6c75 726d 5f6a 6f62 5f69 6473 5d29 0a20  lurm_job_ids]). 
-0000d570: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000d580: 6c66 2e5f 4a4f 425f 5354 4154 5553 5f43  lf._JOB_STATUS_C
-0000d590: 4d44 2e66 6f72 6d61 7428 736c 7572 6d5f  MD.format(slurm_
-0000d5a0: 6a6f 625f 6964 3d73 6c75 726d 5f6a 6f62  job_id=slurm_job
-0000d5b0: 5f69 6429 0a0a 2020 2020 6465 6620 6578  _id)..    def ex
-0000d5c0: 7472 6163 745f 6461 7461 5f6c 6f63 6174  tract_data_locat
-0000d5d0: 696f 6e5f 6672 6f6d 5f6c 6f67 2873 656c  ion_from_log(sel
-0000d5e0: 662c 2073 6c75 726d 5f6a 6f62 5f69 643a  f, slurm_job_id:
-0000d5f0: 2073 7472 203d 204e 6f6e 652c 0a20 2020   str = None,.   
-0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d620: 2020 2020 6c6f 6766 696c 653a 2073 7472      logfile: str
-0000d630: 203d 204e 6f6e 6529 202d 3e20 7374 723a   = None) -> str:
-0000d640: 0a20 2020 2020 2020 2022 2222 5265 6164  .        """Read
-0000d650: 2053 4c55 524d 206a 6f62 206c 6f67 6669   SLURM job logfi
-0000d660: 6c65 2074 6f20 6669 6e64 206c 6f63 6174  le to find locat
-0000d670: 696f 6e20 6f66 2074 6865 2064 6174 612e  ion of the data.
-0000d680: 0a0a 2020 2020 2020 2020 4f6e 6520 6f66  ..        One of
-0000d690: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
-0000d6a0: 6973 2072 6571 7569 7265 642c 2065 6974  is required, eit
-0000d6b0: 6865 7220 6964 206f 7220 6669 6c65 2e0a  her id or file..
-0000d6c0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000d6d0: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
-0000d6e0: 5f6a 6f62 5f69 6420 2873 7472 293a 2049  _job_id (str): I
-0000d6f0: 6420 6f66 2074 6865 2073 6c75 726d 206a  d of the slurm j
-0000d700: 6f62 0a20 2020 2020 2020 2020 2020 206c  ob.            l
-0000d710: 6f67 6669 6c65 2028 7374 7229 3a20 5061  ogfile (str): Pa
-0000d720: 7468 2074 6f20 7468 6520 6c6f 6766 696c  th to the logfil
-0000d730: 650a 0a20 2020 2020 2020 2052 6574 7572  e..        Retur
-0000d740: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0000d750: 7374 723a 2044 6174 6120 6c6f 6361 7469  str: Data locati
-0000d760: 6f6e 2061 6363 6f72 6469 6e67 2074 6f20  on according to 
-0000d770: 7468 6520 6c6f 670a 0a20 2020 2020 2020  the log..       
-0000d780: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-0000d790: 2020 2020 2053 5348 4578 6365 7074 696f       SSHExceptio
-0000d7a0: 6e3a 2049 6620 7468 6572 6520 6973 2061  n: If there is a
-0000d7b0: 6e20 6973 7375 6520 7769 7468 2074 6865  n issue with the
-0000d7c0: 2063 6f6d 6d61 6e64 2065 7865 6375 7469   command executi
-0000d7d0: 6f6e 2e0a 2020 2020 2020 2020 2222 220a  on..        """.
-0000d7e0: 2020 2020 2020 2020 6966 206c 6f67 6669          if logfi
-0000d7f0: 6c65 2069 7320 4e6f 6e65 2061 6e64 2073  le is None and s
-0000d800: 6c75 726d 5f6a 6f62 5f69 6420 6973 206e  lurm_job_id is n
-0000d810: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
-0000d820: 2020 2020 206c 6f67 6669 6c65 203d 2073       logfile = s
-0000d830: 656c 662e 5f4c 4f47 4649 4c45 0a20 2020  elf._LOGFILE.   
-0000d840: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
-0000d850: 203d 206c 6f67 6669 6c65 2e66 6f72 6d61   = logfile.forma
-0000d860: 7428 736c 7572 6d5f 6a6f 625f 6964 3d73  t(slurm_job_id=s
-0000d870: 6c75 726d 5f6a 6f62 5f69 6429 0a20 2020  lurm_job_id).   
-0000d880: 2020 2020 2063 6d64 203d 2073 656c 662e       cmd = self.
-0000d890: 5f4c 4f47 4649 4c45 5f44 4154 415f 434d  _LOGFILE_DATA_CM
-0000d8a0: 442e 666f 726d 6174 286c 6f67 5f66 696c  D.format(log_fil
-0000d8b0: 653d 6c6f 6766 696c 6529 0a20 2020 2020  e=logfile).     
-0000d8c0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-0000d8d0: 2e72 756e 5f63 6f6d 6d61 6e64 7328 5b63  .run_commands([c
-0000d8e0: 6d64 5d29 0a20 2020 2020 2020 2069 6620  md]).        if 
-0000d8f0: 7265 7375 6c74 2e6f 6b3a 0a20 2020 2020  result.ok:.     
-0000d900: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0000d910: 7375 6c74 2e73 7464 6f75 740a 2020 2020  sult.stdout.    
-0000d920: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000d930: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
-0000d940: 7863 6570 7469 6f6e 2872 6573 756c 7429  xception(result)
-0000d950: 0a0a 2020 2020 6465 6620 6765 745f 776f  ..    def get_wo
-0000d960: 726b 666c 6f77 5f70 6172 616d 6574 6572  rkflow_parameter
-0000d970: 7328 7365 6c66 2c0a 2020 2020 2020 2020  s(self,.        
-0000d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d990: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
-0000d9a0: 3a20 7374 7229 202d 3e20 4469 6374 5b73  : str) -> Dict[s
-0000d9b0: 7472 2c20 4469 6374 5b73 7472 2c20 416e  tr, Dict[str, An
-0000d9c0: 795d 5d3a 0a20 2020 2020 2020 2022 2222  y]]:.        """
-0000d9d0: 0a20 2020 2020 2020 2052 6574 7269 6576  .        Retriev
-0000d9e0: 6520 7468 6520 7061 7261 6d65 7465 7273  e the parameters
-0000d9f0: 206f 6620 6120 776f 726b 666c 6f77 2e0a   of a workflow..
-0000da00: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000da10: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
-0000da20: 6c6f 7720 2873 7472 293a 2054 6865 2077  low (str): The w
-0000da30: 6f72 6b66 6c6f 7720 666f 7220 7768 6963  orkflow for whic
-0000da40: 6820 746f 2072 6574 7269 6576 6520 7468  h to retrieve th
-0000da50: 6520 7061 7261 6d65 7465 7273 2e0a 0a20  e parameters... 
-0000da60: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000da70: 2020 2020 2020 2020 2020 2020 4469 6374              Dict
-0000da80: 5b73 7472 2c20 4469 6374 5b73 7472 2c20  [str, Dict[str, 
-0000da90: 416e 795d 5d3a 0a20 2020 2020 2020 2020  Any]]:.         
-0000daa0: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
-0000dab0: 6172 7920 636f 6e74 6169 6e69 6e67 2074  ary containing t
-0000dac0: 6865 2077 6f72 6b66 6c6f 7720 7061 7261  he workflow para
-0000dad0: 6d65 7465 7273 2e0a 0a20 2020 2020 2020  meters...       
-0000dae0: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
-0000daf0: 2020 2020 2056 616c 7565 4572 726f 723a       ValueError:
-0000db00: 2049 6620 616e 2065 7272 6f72 206f 6363   If an error occ
-0000db10: 7572 7320 7768 696c 6520 7265 7472 6965  urs while retrie
-0000db20: 7669 6e67 2074 6865 2077 6f72 6b66 6c6f  ving the workflo
-0000db30: 770a 2020 2020 2020 2020 2020 2020 2020  w.              
-0000db40: 2020 7061 7261 6d65 7465 7273 2e0a 2020    parameters..  
-0000db50: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000db60: 2020 6a73 6f6e 5f64 6573 6372 6970 746f    json_descripto
-0000db70: 7220 3d20 7365 6c66 2e70 756c 6c5f 6465  r = self.pull_de
-0000db80: 7363 7269 7074 6f72 5f66 726f 6d5f 6769  scriptor_from_gi
-0000db90: 7468 7562 2877 6f72 6b66 6c6f 7729 0a20  thub(workflow). 
-0000dba0: 2020 2020 2020 2023 2063 6f6e 7665 7274         # convert
-0000dbb0: 2074 6f20 6f6d 6572 6f20 7479 7065 730a   to omero types.
-0000dbc0: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000dbd0: 6562 7567 286a 736f 6e5f 6465 7363 7269  ebug(json_descri
-0000dbe0: 7074 6f72 290a 2020 2020 2020 2020 776f  ptor).        wo
-0000dbf0: 726b 666c 6f77 5f64 6963 7420 3d20 7b7d  rkflow_dict = {}
-0000dc00: 0a20 2020 2020 2020 2066 6f72 2069 6e70  .        for inp
-0000dc10: 7574 2069 6e20 6a73 6f6e 5f64 6573 6372  ut in json_descr
-0000dc20: 6970 746f 725b 2769 6e70 7574 7327 5d3a  iptor['inputs']:
-0000dc30: 0a20 2020 2020 2020 2020 2020 2023 2066  .            # f
-0000dc40: 696c 7465 7220 6379 746f 6d69 6e65 2070  ilter cytomine p
-0000dc50: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0000dc60: 2020 2020 2020 6966 206e 6f74 2069 6e70        if not inp
-0000dc70: 7574 5b27 6964 275d 2e73 7461 7274 7377  ut['id'].startsw
-0000dc80: 6974 6828 2763 7974 6f6d 696e 6527 293a  ith('cytomine'):
-0000dc90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000dca0: 2077 6f72 6b66 6c6f 775f 7061 7261 6d73   workflow_params
-0000dcb0: 203d 207b 7d0a 2020 2020 2020 2020 2020   = {}.          
-0000dcc0: 2020 2020 2020 776f 726b 666c 6f77 5f70        workflow_p
-0000dcd0: 6172 616d 735b 276e 616d 6527 5d20 3d20  arams['name'] = 
-0000dce0: 696e 7075 745b 2769 6427 5d0a 2020 2020  input['id'].    
-0000dcf0: 2020 2020 2020 2020 2020 2020 776f 726b              work
-0000dd00: 666c 6f77 5f70 6172 616d 735b 2764 6566  flow_params['def
-0000dd10: 6175 6c74 275d 203d 2069 6e70 7574 5b27  ault'] = input['
-0000dd20: 6465 6661 756c 742d 7661 6c75 6527 5d0a  default-value'].
-0000dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd40: 776f 726b 666c 6f77 5f70 6172 616d 735b  workflow_params[
-0000dd50: 2763 7974 7970 6527 5d20 3d20 696e 7075  'cytype'] = inpu
-0000dd60: 745b 2774 7970 6527 5d0a 2020 2020 2020  t['type'].      
-0000dd70: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000dd80: 6f77 5f70 6172 616d 735b 276f 7074 696f  ow_params['optio
-0000dd90: 6e61 6c27 5d20 3d20 696e 7075 745b 276f  nal'] = input['o
-0000dda0: 7074 696f 6e61 6c27 5d0a 2020 2020 2020  ptional'].      
-0000ddb0: 2020 2020 2020 2020 2020 636d 645f 666c            cmd_fl
-0000ddc0: 6167 203d 2069 6e70 7574 5b27 636f 6d6d  ag = input['comm
-0000ddd0: 616e 642d 6c69 6e65 2d66 6c61 6727 5d0a  and-line-flag'].
-0000dde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddf0: 636d 645f 666c 6167 203d 2063 6d64 5f66  cmd_flag = cmd_f
-0000de00: 6c61 672e 7265 706c 6163 6528 2240 6964  lag.replace("@id
-0000de10: 222c 2069 6e70 7574 5b27 6964 275d 290a  ", input['id']).
-0000de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de30: 776f 726b 666c 6f77 5f70 6172 616d 735b  workflow_params[
-0000de40: 2763 6d64 5f66 6c61 6727 5d20 3d20 636d  'cmd_flag'] = cm
-0000de50: 645f 666c 6167 0a20 2020 2020 2020 2020  d_flag.         
-0000de60: 2020 2020 2020 2077 6f72 6b66 6c6f 775f         workflow_
-0000de70: 7061 7261 6d73 5b27 6465 7363 7269 7074  params['descript
-0000de80: 696f 6e27 5d20 3d20 696e 7075 745b 2764  ion'] = input['d
-0000de90: 6573 6372 6970 7469 6f6e 275d 0a20 2020  escription'].   
-0000dea0: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
-0000deb0: 6b66 6c6f 775f 6469 6374 5b69 6e70 7574  kflow_dict[input
-0000dec0: 5b27 6964 275d 5d20 3d20 776f 726b 666c  ['id']] = workfl
-0000ded0: 6f77 5f70 6172 616d 730a 2020 2020 2020  ow_params.      
-0000dee0: 2020 7265 7475 726e 2077 6f72 6b66 6c6f    return workflo
-0000def0: 775f 6469 6374 0a0a 2020 2020 6465 6620  w_dict..    def 
-0000df00: 636f 6e76 6572 745f 6379 7479 7065 5f74  convert_cytype_t
-0000df10: 6f5f 6f6d 7479 7065 2873 656c 662c 0a20  o_omtype(self,. 
-0000df20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df40: 6379 7479 7065 3a20 7374 722c 205f 6465  cytype: str, _de
-0000df50: 6661 756c 742c 202a 6172 6773 2c20 2a2a  fault, *args, **
-0000df60: 6b77 6172 6773 0a20 2020 2020 2020 2020  kwargs.         
-0000df70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df80: 2020 2020 2020 2020 2920 2d3e 2041 6e79          ) -> Any
-0000df90: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000dfa0: 2020 2020 2020 436f 6e76 6572 7420 6120        Convert a 
-0000dfb0: 4379 746f 6d69 6e65 2074 7970 6520 746f  Cytomine type to
-0000dfc0: 2061 6e20 4f4d 4552 4f20 7479 7065 2061   an OMERO type a
-0000dfd0: 6e64 2069 6e73 7461 6e74 6961 7465 7320  nd instantiates 
-0000dfe0: 6974 0a20 2020 2020 2020 2077 6974 6820  it.        with 
-0000dff0: 6172 6773 2f6b 7761 7267 732e 0a0a 2020  args/kwargs...  
-0000e000: 2020 2020 2020 4e6f 7465 2074 6861 7420        Note that 
-0000e010: 4379 746f 6d69 6e65 2068 6173 2061 2050  Cytomine has a P
-0000e020: 7974 686f 6e20 436c 6965 6e74 2c20 616e  ython Client, an
-0000e030: 6420 736f 6d65 2063 6f6e 7665 7273 696f  d some conversio
-0000e040: 6e20 6d65 7468 6f64 730a 2020 2020 2020  n methods.      
-0000e050: 2020 746f 2070 7974 686f 6e20 7479 7065    to python type
-0000e060: 732c 2062 7574 206e 6f74 6869 6e67 2070  s, but nothing p
-0000e070: 6172 7469 6375 6c61 726c 7920 776f 7274  articularly wort
-0000e080: 6820 6465 7065 6e64 696e 6720 6f6e 2074  h depending on t
-0000e090: 6861 740a 2020 2020 2020 2020 6c69 6272  hat.        libr
-0000e0a0: 6172 7920 666f 7220 7965 742e 204d 6967  ary for yet. Mig
-0000e0b0: 6874 2062 6520 7573 6566 756c 2069 6e20  ht be useful in 
-0000e0c0: 7468 6520 6675 7475 7265 2070 6572 6861  the future perha
-0000e0d0: 7073 2e0a 2020 2020 2020 2020 2865 2e67  ps..        (e.g
-0000e0e0: 2e20 6874 7470 733a 2f2f 6769 7468 7562  . https://github
-0000e0f0: 2e63 6f6d 2f43 7974 6f6d 696e 652d 554c  .com/Cytomine-UL
-0000e100: 6965 6765 2f43 7974 6f6d 696e 652d 7079  iege/Cytomine-py
-0000e110: 7468 6f6e 2d63 6c69 656e 742f 0a20 2020  thon-client/.   
-0000e120: 2020 2020 2062 6c6f 622f 6d61 7374 6572       blob/master
-0000e130: 2f63 7974 6f6d 696e 652f 6379 746f 6d69  /cytomine/cytomi
-0000e140: 6e65 5f6a 6f62 2e70 7929 0a0a 2020 2020  ne_job.py)..    
-0000e150: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000e160: 2020 2020 2020 6379 7479 7065 2028 7374        cytype (st
-0000e170: 7229 3a20 5468 6520 4379 746f 6d69 6e65  r): The Cytomine
-0000e180: 2074 7970 6520 746f 2063 6f6e 7665 7274   type to convert
-0000e190: 2e0a 2020 2020 2020 2020 2020 2020 5f64  ..            _d
-0000e1a0: 6566 6175 6c74 3a20 5468 6520 6465 6661  efault: The defa
-0000e1b0: 756c 7420 7661 6c75 652e 2052 6571 7569  ult value. Requi
-0000e1c0: 7265 6420 746f 2064 6973 7469 6e67 7569  red to distingui
-0000e1d0: 7368 2062 6574 7765 656e 2066 6c6f 6174  sh between float
-0000e1e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e1f0: 2061 6e64 2069 6e74 2e0a 2020 2020 2020   and int..      
-0000e200: 2020 2020 2020 2a61 7267 733a 2041 6464        *args: Add
-0000e210: 6974 696f 6e61 6c20 706f 7369 7469 6f6e  itional position
-0000e220: 616c 2061 7267 756d 656e 7473 2e0a 2020  al arguments..  
-0000e230: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
-0000e240: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
-0000e250: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
-0000e260: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0000e270: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0000e280: 416e 793a 0a20 2020 2020 2020 2020 2020  Any:.           
-0000e290: 2020 2020 2054 6865 2063 6f6e 7665 7274       The convert
-0000e2a0: 6564 204f 4d45 524f 2074 7970 6520 636c  ed OMERO type cl
-0000e2b0: 6173 7320 696e 7374 616e 6365 0a20 2020  ass instance.   
-0000e2c0: 2020 2020 2020 2020 2020 2020 206f 7220               or 
-0000e2d0: 4e6f 6e65 2069 6620 6572 726f 7273 206f  None if errors o
-0000e2e0: 6363 7572 6564 2e0a 0a20 2020 2020 2020  ccured...       
-0000e2f0: 2022 2222 0a20 2020 2020 2020 2023 2054   """.        # T
-0000e300: 4f44 4f20 6d61 6b65 2045 6e75 6d20 3f0a  ODO make Enum ?.
-0000e310: 2020 2020 2020 2020 6966 2063 7974 7970          if cytyp
-0000e320: 6520 3d3d 2027 4e75 6d62 6572 273a 0a20  e == 'Number':. 
-0000e330: 2020 2020 2020 2020 2020 2069 6620 6973             if is
-0000e340: 696e 7374 616e 6365 285f 6465 6661 756c  instance(_defaul
-0000e350: 742c 2066 6c6f 6174 293a 0a20 2020 2020  t, float):.     
-0000e360: 2020 2020 2020 2020 2020 2023 2066 6c6f             # flo
-0000e370: 6174 2069 6e73 7465 6164 0a20 2020 2020  at instead.     
-0000e380: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000e390: 6e20 7365 6c66 2e73 7472 5f74 6f5f 636c  n self.str_to_cl
-0000e3a0: 6173 7328 226f 6d65 726f 2e73 6372 6970  ass("omero.scrip
-0000e3b0: 7473 222c 2022 466c 6f61 7422 2c0a 2020  ts", "Float",.  
-0000e3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e3e0: 2020 2020 2020 202a 6172 6773 2c20 2a2a         *args, **
-0000e3f0: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
-0000e400: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000e410: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000e420: 2073 656c 662e 7374 725f 746f 5f63 6c61   self.str_to_cla
-0000e430: 7373 2822 6f6d 6572 6f2e 7363 7269 7074  ss("omero.script
-0000e440: 7322 2c20 2249 6e74 222c 0a20 2020 2020  s", "Int",.     
-0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e470: 2020 2020 2a61 7267 732c 202a 2a6b 7761      *args, **kwa
-0000e480: 7267 7329 0a20 2020 2020 2020 2065 6c69  rgs).        eli
-0000e490: 6620 6379 7479 7065 203d 3d20 2742 6f6f  f cytype == 'Boo
-0000e4a0: 6c65 616e 273a 0a20 2020 2020 2020 2020  lean':.         
-0000e4b0: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
-0000e4c0: 7472 5f74 6f5f 636c 6173 7328 226f 6d65  tr_to_class("ome
-0000e4d0: 726f 2e73 6372 6970 7473 222c 2022 426f  ro.scripts", "Bo
-0000e4e0: 6f6c 222c 0a20 2020 2020 2020 2020 2020  ol",.           
-0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e500: 2020 2020 2020 2020 2020 2a61 7267 732c            *args,
-0000e510: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-0000e520: 2020 2065 6c69 6620 6379 7479 7065 203d     elif cytype =
-0000e530: 3d20 2753 7472 696e 6727 3a0a 2020 2020  = 'String':.    
-0000e540: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-0000e550: 656c 662e 7374 725f 746f 5f63 6c61 7373  elf.str_to_class
-0000e560: 2822 6f6d 6572 6f2e 7363 7269 7074 7322  ("omero.scripts"
-0000e570: 2c20 2253 7472 696e 6722 2c0a 2020 2020  , "String",.    
-0000e580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5a0: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-0000e5b0: 290a 0a20 2020 2064 6566 2065 7874 7261  )..    def extra
-0000e5c0: 6374 5f70 6172 7473 5f66 726f 6d5f 7572  ct_parts_from_ur
-0000e5d0: 6c28 7365 6c66 2c20 696e 7075 745f 7572  l(self, input_ur
-0000e5e0: 6c3a 2073 7472 2920 2d3e 2054 7570 6c65  l: str) -> Tuple
-0000e5f0: 5b4c 6973 745b 7374 725d 2c20 7374 725d  [List[str], str]
-0000e600: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000e610: 2020 2020 2020 4578 7472 6163 7420 7468        Extract th
-0000e620: 6520 7265 706f 7369 746f 7279 2061 6e64  e repository and
-0000e630: 2062 7261 6e63 6820 696e 666f 726d 6174   branch informat
-0000e640: 696f 6e20 6672 6f6d 2074 6865 2069 6e70  ion from the inp
-0000e650: 7574 2055 524c 2e0a 0a20 2020 2020 2020  ut URL...       
-0000e660: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-0000e670: 2020 2069 6e70 7574 5f75 726c 2028 7374     input_url (st
-0000e680: 7229 3a20 5468 6520 696e 7075 7420 4769  r): The input Gi
-0000e690: 7448 7562 2055 524c 2e0a 0a20 2020 2020  tHub URL...     
-0000e6a0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000e6b0: 2020 2020 2020 2020 5475 706c 655b 4c69          Tuple[Li
-0000e6c0: 7374 5b73 7472 5d2c 2073 7472 5d3a 0a20  st[str], str]:. 
-0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2054                 T
-0000e6e0: 6865 206c 6973 7420 6f66 2075 726c 2070  he list of url p
-0000e6f0: 6172 7473 2061 6e64 2074 6865 2062 7261  arts and the bra
-0000e700: 6e63 682f 7665 7273 696f 6e2e 0a20 2020  nch/version..   
-0000e710: 2020 2020 2020 2020 2020 2020 2049 6620               If 
-0000e720: 6e6f 2062 7261 6e63 6820 6973 2066 6f75  no branch is fou
-0000e730: 6e64 2c20 6974 2077 696c 6c20 7265 7475  nd, it will retu
-0000e740: 726e 2022 6d61 7374 6572 220a 0a20 2020  rn "master"..   
-0000e750: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-0000e760: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
-0000e770: 726f 723a 2049 6620 7468 6520 696e 7075  ror: If the inpu
-0000e780: 7420 5552 4c20 6973 206e 6f74 2061 2076  t URL is not a v
-0000e790: 616c 6964 2047 6974 4875 6220 5552 4c2e  alid GitHub URL.
-0000e7a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000e7b0: 2020 2020 2075 726c 5f70 6172 7473 203d       url_parts =
-0000e7c0: 2069 6e70 7574 5f75 726c 2e73 706c 6974   input_url.split
-0000e7d0: 2822 2f22 290a 2020 2020 2020 2020 6966  ("/").        if
-0000e7e0: 206c 656e 2875 726c 5f70 6172 7473 2920   len(url_parts) 
-0000e7f0: 3c20 3520 6f72 2075 726c 5f70 6172 7473  < 5 or url_parts
-0000e800: 5b32 5d20 213d 2022 6769 7468 7562 2e63  [2] != "github.c
-0000e810: 6f6d 223a 0a20 2020 2020 2020 2020 2020  om":.           
-0000e820: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0000e830: 7228 2249 6e76 616c 6964 2047 6974 4875  r("Invalid GitHu
-0000e840: 6220 5552 4c22 290a 0a20 2020 2020 2020  b URL")..       
-0000e850: 2069 6620 2274 7265 6522 2069 6e20 7572   if "tree" in ur
-0000e860: 6c5f 7061 7274 733a 0a20 2020 2020 2020  l_parts:.       
-0000e870: 2020 2020 2023 2043 6173 653a 2055 524c       # Case: URL
-0000e880: 2063 6f6e 7461 696e 7320 6120 6272 616e   contains a bran
-0000e890: 6368 0a20 2020 2020 2020 2020 2020 2062  ch.            b
-0000e8a0: 7261 6e63 685f 696e 6465 7820 3d20 7572  ranch_index = ur
-0000e8b0: 6c5f 7061 7274 732e 696e 6465 7828 2274  l_parts.index("t
-0000e8c0: 7265 6522 2920 2b20 310a 2020 2020 2020  ree") + 1.      
-0000e8d0: 2020 2020 2020 6272 616e 6368 203d 2075        branch = u
-0000e8e0: 726c 5f70 6172 7473 5b62 7261 6e63 685f  rl_parts[branch_
-0000e8f0: 696e 6465 785d 0a20 2020 2020 2020 2065  index].        e
-0000e900: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000e910: 2023 2043 6173 653a 2055 524c 2064 6f65   # Case: URL doe
-0000e920: 7320 6e6f 7420 7370 6563 6966 7920 6120  s not specify a 
-0000e930: 6272 616e 6368 0a20 2020 2020 2020 2020  branch.         
-0000e940: 2020 2062 7261 6e63 6820 3d20 226d 6173     branch = "mas
-0000e950: 7465 7222 0a0a 2020 2020 2020 2020 7265  ter"..        re
-0000e960: 7475 726e 2075 726c 5f70 6172 7473 2c20  turn url_parts, 
-0000e970: 6272 616e 6368 0a0a 2020 2020 6465 6620  branch..    def 
-0000e980: 636f 6e76 6572 745f 7572 6c28 7365 6c66  convert_url(self
-0000e990: 2c20 696e 7075 745f 7572 6c3a 2073 7472  , input_url: str
-0000e9a0: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-0000e9b0: 2020 2222 220a 2020 2020 2020 2020 436f    """.        Co
-0000e9c0: 6e76 6572 7420 7468 6520 696e 7075 7420  nvert the input 
-0000e9d0: 4769 7448 7562 2055 524c 2074 6f20 616e  GitHub URL to an
-0000e9e0: 206f 7574 7075 7420 5552 4c20 7468 6174   output URL that
-0000e9f0: 2072 6574 7269 6576 6573 0a20 2020 2020   retrieves.     
-0000ea00: 2020 2074 6865 2027 6465 7363 7269 7074     the 'descript
-0000ea10: 6f72 2e6a 736f 6e27 2066 696c 6520 696e  or.json' file in
-0000ea20: 2072 6177 2066 6f72 6d61 742e 0a0a 2020   raw format...  
-0000ea30: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0000ea40: 2020 2020 2020 2020 696e 7075 745f 7572          input_ur
-0000ea50: 6c20 2873 7472 293a 2054 6865 2069 6e70  l (str): The inp
-0000ea60: 7574 2047 6974 4875 6220 5552 4c2e 0a0a  ut GitHub URL...
-0000ea70: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-0000ea80: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-0000ea90: 3a20 5468 6520 6f75 7470 7574 2055 524c  : The output URL
-0000eaa0: 2074 6f20 7468 6520 2764 6573 6372 6970   to the 'descrip
-0000eab0: 746f 722e 6a73 6f6e 2720 6669 6c65 2e0a  tor.json' file..
-0000eac0: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
-0000ead0: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-0000eae0: 7565 4572 726f 723a 2049 6620 7468 6520  ueError: If the 
-0000eaf0: 696e 7075 7420 5552 4c20 6973 206e 6f74  input URL is not
-0000eb00: 2061 2076 616c 6964 2047 6974 4875 6220   a valid GitHub 
-0000eb10: 5552 4c2e 0a20 2020 2020 2020 2022 2222  URL..        """
-0000eb20: 0a20 2020 2020 2020 2075 726c 5f70 6172  .        url_par
-0000eb30: 7473 2c20 6272 616e 6368 203d 2073 656c  ts, branch = sel
-0000eb40: 662e 6578 7472 6163 745f 7061 7274 735f  f.extract_parts_
-0000eb50: 6672 6f6d 5f75 726c 2869 6e70 7574 5f75  from_url(input_u
-0000eb60: 726c 290a 0a20 2020 2020 2020 2023 2043  rl)..        # C
-0000eb70: 6f6e 7374 7275 6374 2074 6865 206f 7574  onstruct the out
-0000eb80: 7075 7420 5552 4c20 6279 2063 6f6d 6269  put URL by combi
-0000eb90: 6e69 6e67 2074 6865 2065 7874 7261 6374  ning the extract
-0000eba0: 6564 2069 6e66 6f72 6d61 7469 6f6e 0a20  ed information. 
-0000ebb0: 2020 2020 2020 2023 2077 6974 6820 7468         # with th
-0000ebc0: 6520 6465 7369 7265 6420 6669 6c65 2070  e desired file p
-0000ebd0: 6174 680a 2020 2020 2020 2020 6f75 7470  ath.        outp
-0000ebe0: 7574 5f75 726c 203d 2066 2268 7474 7073  ut_url = f"https
-0000ebf0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7b75  ://github.com/{u
-0000ec00: 726c 5f70 6172 7473 5b33 5d7d 2f7b 7572  rl_parts[3]}/{ur
-0000ec10: 6c5f 7061 7274 735b 345d 7d2f 7261 772f  l_parts[4]}/raw/
-0000ec20: 7b62 7261 6e63 687d 2f64 6573 6372 6970  {branch}/descrip
-0000ec30: 746f 722e 6a73 6f6e 220a 0a20 2020 2020  tor.json"..     
-0000ec40: 2020 2072 6574 7572 6e20 6f75 7470 7574     return output
-0000ec50: 5f75 726c 0a0a 2020 2020 6465 6620 7075  _url..    def pu
-0000ec60: 6c6c 5f64 6573 6372 6970 746f 725f 6672  ll_descriptor_fr
-0000ec70: 6f6d 5f67 6974 6875 6228 7365 6c66 2c20  om_github(self, 
-0000ec80: 776f 726b 666c 6f77 3a20 7374 7229 202d  workflow: str) -
-0000ec90: 3e20 4469 6374 3a0a 2020 2020 2020 2020  > Dict:.        
-0000eca0: 2222 220a 2020 2020 2020 2020 5075 6c6c  """.        Pull
-0000ecb0: 2074 6865 2077 6f72 6b66 6c6f 7720 6465   the workflow de
-0000ecc0: 7363 7269 7074 6f72 2066 726f 6d20 4769  scriptor from Gi
-0000ecd0: 7448 7562 2e0a 0a20 2020 2020 2020 2041  tHub...        A
-0000ece0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000ecf0: 2077 6f72 6b66 6c6f 7720 2873 7472 293a   workflow (str):
-0000ed00: 2054 6865 2077 6f72 6b66 6c6f 7720 666f   The workflow fo
-0000ed10: 7220 7768 6963 6820 746f 2070 756c 6c20  r which to pull 
-0000ed20: 7468 6520 6465 7363 7269 7074 6f72 2e0a  the descriptor..
-0000ed30: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000ed40: 3a0a 2020 2020 2020 2020 2020 2020 4469  :.            Di
-0000ed50: 6374 3a20 5468 6520 4a53 4f4e 2064 6573  ct: The JSON des
-0000ed60: 6372 6970 746f 722e 0a0a 2020 2020 2020  criptor...      
-0000ed70: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-0000ed80: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
-0000ed90: 3a20 4966 2061 6e20 6572 726f 7220 6f63  : If an error oc
-0000eda0: 6375 7273 2077 6869 6c65 2070 756c 6c69  curs while pulli
-0000edb0: 6e67 2074 6865 2064 6573 6372 6970 746f  ng the descripto
-0000edc0: 7220 6669 6c65 2e0a 2020 2020 2020 2020  r file..        
-0000edd0: 2222 220a 2020 2020 2020 2020 6769 745f  """.        git_
-0000ede0: 7265 706f 203d 2073 656c 662e 736c 7572  repo = self.slur
-0000edf0: 6d5f 6d6f 6465 6c5f 7265 706f 735b 776f  m_model_repos[wo
-0000ee00: 726b 666c 6f77 5d0a 2020 2020 2020 2020  rkflow].        
-0000ee10: 2320 636f 6e76 6572 7420 6769 7420 7265  # convert git re
-0000ee20: 706f 2074 6f20 6a73 6f6e 2066 696c 650a  po to json file.
-0000ee30: 2020 2020 2020 2020 7261 775f 7572 6c20          raw_url 
-0000ee40: 3d20 7365 6c66 2e63 6f6e 7665 7274 5f75  = self.convert_u
-0000ee50: 726c 2867 6974 5f72 6570 6f29 0a20 2020  rl(git_repo).   
-0000ee60: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
-0000ee70: 6728 6622 5075 6c6c 2077 6f72 6b66 6c6f  g(f"Pull workflo
-0000ee80: 773a 207b 776f 726b 666c 6f77 7d3a 207b  w: {workflow}: {
-0000ee90: 6769 745f 7265 706f 7d20 3e3e 207b 7261  git_repo} >> {ra
-0000eea0: 775f 7572 6c7d 2229 0a20 2020 2020 2020  w_url}").       
-0000eeb0: 2023 2070 756c 6c20 776f 726b 666c 6f77   # pull workflow
-0000eec0: 2070 6172 616d 730a 2020 2020 2020 2020   params.        
-0000eed0: 6769 7468 7562 5f73 6573 7369 6f6e 203d  github_session =
-0000eee0: 2073 656c 662e 6765 745f 6f72 5f63 7265   self.get_or_cre
-0000eef0: 6174 655f 6769 7468 7562 5f73 6573 7369  ate_github_sessi
-0000ef00: 6f6e 2829 0a20 2020 2020 2020 2067 6866  on().        ghf
-0000ef10: 696c 6520 3d20 6769 7468 7562 5f73 6573  ile = github_ses
-0000ef20: 7369 6f6e 2e67 6574 2872 6177 5f75 726c  sion.get(raw_url
-0000ef30: 290a 2020 2020 2020 2020 6966 2067 6866  ).        if ghf
-0000ef40: 696c 652e 6f6b 3a0a 2020 2020 2020 2020  ile.ok:.        
-0000ef50: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-0000ef60: 2866 2243 6163 6865 643f 207b 6768 6669  (f"Cached? {ghfi
-0000ef70: 6c65 2e66 726f 6d5f 6361 6368 657d 2229  le.from_cache}")
-0000ef80: 0a20 2020 2020 2020 2020 2020 206a 736f  .            jso
-0000ef90: 6e5f 6465 7363 7269 7074 6f72 203d 2067  n_descriptor = g
-0000efa0: 6866 696c 652e 6a73 6f6e 2829 0a20 2020  hfile.json().   
-0000efb0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000efc0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-0000efd0: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-0000efe0: 2020 2020 2020 2020 2066 2745 7272 6f72           f'Error
-0000eff0: 2077 6869 6c65 2070 756c 6c69 6e67 2064   while pulling d
-0000f000: 6573 6372 6970 746f 7220 6669 6c65 2066  escriptor file f
-0000f010: 6f72 2077 6f72 6b66 6c6f 7720 7b77 6f72  or workflow {wor
-0000f020: 6b66 6c6f 777d 2c5c 0a20 2020 2020 2020  kflow},\.       
-0000f030: 2020 2020 2020 2020 2020 2020 2066 726f               fro
-0000f040: 6d20 7b72 6177 5f75 726c 7d3a 207b 6768  m {raw_url}: {gh
-0000f050: 6669 6c65 2e5f 5f64 6963 745f 5f7d 2729  file.__dict__}')
-0000f060: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000f070: 6a73 6f6e 5f64 6573 6372 6970 746f 720a  json_descriptor.
-0000f080: 0a20 2020 2064 6566 2067 6574 5f6f 725f  .    def get_or_
-0000f090: 6372 6561 7465 5f67 6974 6875 625f 7365  create_github_se
-0000f0a0: 7373 696f 6e28 7365 6c66 293a 0a20 2020  ssion(self):.   
-0000f0b0: 2020 2020 2023 204e 6f74 652c 2075 7369       # Note, usi
-0000f0c0: 6e67 2072 6571 7565 7374 735f 6361 6368  ng requests_cach
-0000f0d0: 6520 312e 312e 312c 2063 6f6e 6469 7469  e 1.1.1, conditi
-0000f0e0: 6f6e 616c 2071 7565 7269 6573 2061 7265  onal queries are
-0000f0f0: 2064 6566 6175 6c74 3a0a 2020 2020 2020   default:.      
-0000f100: 2020 2320 5468 6520 6361 6368 6564 2072    # The cached r
-0000f110: 6573 706f 6e73 6520 7769 6c6c 2073 7469  esponse will sti
-0000f120: 6c6c 2062 6520 7573 6564 2075 6e74 696c  ll be used until
-0000f130: 2074 6865 2072 656d 6f74 6520 636f 6e74   the remote cont
-0000f140: 656e 7420 6163 7475 616c 6c79 2063 6861  ent actually cha
-0000f150: 6e67 6573 0a20 2020 2020 2020 2023 2045  nges.        # E
-0000f160: 7665 6e20 6966 2074 6865 2027 6578 7069  ven if the 'expi
-0000f170: 7265 5f61 6674 6572 2720 6973 2074 7269  re_after' is tri
-0000f180: 6767 6572 6564 2e20 5468 6973 2069 7320  ggered. This is 
-0000f190: 6275 696c 7420 696e 746f 2047 6974 4875  built into GitHu
-0000f1a0: 622c 2077 6869 6368 2072 6574 7572 6e73  b, which returns
-0000f1b0: 0a20 2020 2020 2020 2023 2061 2045 7461  .        # a Eta
-0000f1c0: 6720 696e 2074 6865 2068 6561 6465 7220  g in the header 
-0000f1d0: 7468 6174 206f 6e6c 7920 6368 616e 6765  that only change
-0000f1e0: 7320 7768 656e 2074 6865 2063 6f6e 7465  s when the conte
-0000f1f0: 6e74 2028 652e 672e 2074 6865 2064 6573  nt (e.g. the des
-0000f200: 6372 6970 746f 7229 2063 6861 6e67 6573  criptor) changes
-0000f210: 2e0a 2020 2020 2020 2020 2320 4966 2079  ..        # If y
-0000f220: 6f75 2070 726f 7669 6465 2074 6869 7320  ou provide this 
-0000f230: 4574 6167 2077 6865 6e20 7175 6572 7969  Etag when queryi
-0000f240: 6e67 2c20 796f 7520 7769 6c6c 2067 6574  ng, you will get
-0000f250: 2061 2033 3034 2028 276e 6f20 6368 616e   a 304 ('no chan
-0000f260: 6765 2729 2061 6e64 2069 7420 7769 6c6c  ge') and it will
-0000f270: 0a20 2020 2020 2020 2023 204e 4f54 2063  .        # NOT c
-0000f280: 6f75 6e74 2074 6f77 6172 6473 2079 6f75  ount towards you
-0000f290: 7220 4769 7468 7562 206c 696d 6974 732e  r Github limits.
-0000f2a0: 2041 6e64 2072 6571 7565 7374 735f 6361   And requests_ca
-0000f2b0: 6368 6520 646f 6573 2074 6861 7420 666f  che does that fo
-0000f2c0: 7220 7573 206e 6f77 2e0a 2020 2020 2020  r us now..      
-0000f2d0: 2020 2320 4e6f 7420 6176 6169 6c61 626c    # Not availabl
-0000f2e0: 6520 696e 2050 7974 686f 6e33 2e36 2074  e in Python3.6 t
-0000f2f0: 686f 7567 682e 0a20 2020 2020 2020 2073  hough..        s
-0000f300: 203d 2072 6571 7565 7374 735f 6361 6368   = requests_cach
-0000f310: 652e 4361 6368 6564 5365 7373 696f 6e28  e.CachedSession(
-0000f320: 2767 6974 6875 625f 6361 6368 6527 2c0a  'github_cache',.
-0000f330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f350: 2020 2020 2020 2020 2062 6163 6b65 6e64           backend
-0000f360: 3d73 656c 662e 6361 6368 652c 0a20 2020  =self.cache,.   
-0000f370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f390: 2020 2020 2020 6578 7069 7265 5f61 6674        expire_aft
-0000f3a0: 6572 3d31 2c0a 2020 2020 2020 2020 2020  er=1,.          
-0000f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000f3d0: 6163 6865 5f63 6f6e 7472 6f6c 3d54 7275  ache_control=Tru
-0000f3e0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000f3f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f400: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-0000f410: 2020 2020 2023 204d 6967 6874 2068 6176       # Might hav
-0000f420: 6520 6269 6767 6572 2069 7373 7565 732c  e bigger issues,
-0000f430: 2074 6869 7320 6973 2072 656c 6174 6564   this is related
-0000f440: 2074 6f20 7261 7465 206c 696d 6974 7320   to rate limits 
-0000f450: 6f6e 2047 6974 4875 620a 2020 2020 2020  on GitHub.      
-0000f460: 2020 2320 6874 7470 733a 2f2f 646f 6373    # https://docs
-0000f470: 2e67 6974 6875 622e 636f 6d2f 656e 2f72  .github.com/en/r
-0000f480: 6573 742f 7573 696e 672d 7468 652d 7265  est/using-the-re
-0000f490: 7374 2d61 7069 2f72 6174 652d 6c69 6d69  st-api/rate-limi
-0000f4a0: 7473 2d66 6f72 2d74 6865 2d72 6573 742d  ts-for-the-rest-
-0000f4b0: 6170 690a 2020 2020 2020 2020 2320 4966  api.        # If
-0000f4c0: 2069 7420 7374 6179 7320 6120 7072 6f62   it stays a prob
-0000f4d0: 6c65 6d2c 2077 6520 6861 7665 2074 6f20  lem, we have to 
-0000f4e0: 6164 6420 616e 206f 7074 696f 6e20 746f  add an option to
-0000f4f0: 2061 6464 2061 2047 4820 6b65 7920 746f   add a GH key to
-0000f500: 2074 6865 2063 6f6e 6669 670a 2020 2020   the config.    
-0000f510: 2020 2020 2320 452e 672e 2073 6565 2068      # E.g. see h
-0000f520: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000f530: 6d2f 7265 7175 6573 7473 2d63 6163 6865  m/requests-cache
-0000f540: 2f72 6571 7565 7374 732d 6361 6368 652f  /requests-cache/
-0000f550: 626c 6f62 2f35 3331 3334 6566 3065 3939  blob/53134ef0e99
-0000f560: 6437 3133 6665 6436 3235 3135 6466 6237  d713fed62515dfb7
-0000f570: 6263 6661 6163 3566 3633 6639 642f 6578  bcfaac5f63f9d/ex
-0000f580: 616d 706c 6573 2f70 7967 6974 6875 622e  amples/pygithub.
-0000f590: 7079 0a20 2020 2020 2020 2023 2048 6572  py.        # Her
-0000f5a0: 6520 796f 7520 636f 756c 6420 6861 7665  e you could have
-0000f5b0: 2061 6e20 4143 4345 5353 5f54 4f4b 454e   an ACCESS_TOKEN
-0000f5c0: 2e0a 2020 2020 2020 2020 2320 416e 2041  ..        # An A
-0000f5d0: 4343 4553 535f 544f 4b45 4e20 636f 756c  CCESS_TOKEN coul
-0000f5e0: 6420 696d 7072 6f76 6520 6170 6920 6c69  d improve api li
-0000f5f0: 6d69 7473 2074 6f20 3530 3030 2f68 2028  mits to 5000/h (
-0000f600: 6672 6f6d 2036 302f 6829 2e0a 2020 2020  from 60/h)..    
-0000f610: 2020 2020 7265 7472 795f 7374 7261 7465      retry_strate
-0000f620: 6779 203d 2052 6574 7279 280a 2020 2020  gy = Retry(.    
-0000f630: 2020 2020 2020 2020 746f 7461 6c3d 352c          total=5,
-0000f640: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000f650: 204d 6178 696d 756d 206e 756d 6265 7220   Maximum number 
-0000f660: 6f66 2072 6574 7269 6573 0a20 2020 2020  of retries.     
-0000f670: 2020 2020 2020 2023 2045 7870 6f6e 656e         # Exponen
-0000f680: 7469 616c 2062 6163 6b6f 6666 2066 6163  tial backoff fac
-0000f690: 746f 7220 2864 656c 6179 2062 6574 7765  tor (delay betwe
-0000f6a0: 656e 2072 6574 7269 6573 290a 2020 2020  en retries).    
-0000f6b0: 2020 2020 2020 2020 6261 636b 6f66 665f          backoff_
-0000f6c0: 6661 6374 6f72 3d35 2c0a 2020 2020 2020  factor=5,.      
-0000f6d0: 2020 2020 2020 2320 5265 7472 7920 6f6e        # Retry on
-0000f6e0: 2074 6865 7365 2048 5454 5020 7374 6174   these HTTP stat
-0000f6f0: 7573 2063 6f64 6573 0a20 2020 2020 2020  us codes.       
-0000f700: 2020 2020 2073 7461 7475 735f 666f 7263       status_forc
-0000f710: 656c 6973 743d 5b35 3030 2c20 3530 322c  elist=[500, 502,
-0000f720: 2035 3033 2c20 3530 342c 2034 3033 2c20   503, 504, 403, 
-0000f730: 3432 395d 2c0a 2020 2020 2020 2020 2020  429],.          
-0000f740: 2020 616c 6c6f 7765 645f 6d65 7468 6f64    allowed_method
-0000f750: 733d 6672 6f7a 656e 7365 7428 5b27 4745  s=frozenset(['GE
-0000f760: 5427 5d29 2020 2320 4f6e 6c79 2072 6574  T'])  # Only ret
-0000f770: 7279 2066 6f72 2047 4554 2072 6571 7565  ry for GET reque
-0000f780: 7374 730a 2020 2020 2020 2020 290a 2020  sts.        ).  
-0000f790: 2020 2020 2020 732e 6d6f 756e 7428 2768        s.mount('h
-0000f7a0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000f7b0: 6d2f 272c 2048 5454 5041 6461 7074 6572  m/', HTTPAdapter
-0000f7c0: 286d 6178 5f72 6574 7269 6573 3d72 6574  (max_retries=ret
-0000f7d0: 7279 5f73 7472 6174 6567 7929 290a 2020  ry_strategy)).  
-0000f7e0: 2020 2020 2020 732e 6d6f 756e 7428 2768        s.mount('h
-0000f7f0: 7474 703a 2f2f 6769 7468 7562 2e63 6f6d  ttp://github.com
-0000f800: 2f27 2c20 4854 5450 4164 6170 7465 7228  /', HTTPAdapter(
-0000f810: 6d61 785f 7265 7472 6965 733d 7265 7472  max_retries=retr
-0000f820: 795f 7374 7261 7465 6779 2929 0a20 2020  y_strategy)).   
-0000f830: 2020 2020 2072 6574 7572 6e20 730a 0a20       return s.. 
-0000f840: 2020 2064 6566 2067 6574 5f77 6f72 6b66     def get_workf
-0000f850: 6c6f 775f 636f 6d6d 616e 6428 7365 6c66  low_command(self
-0000f860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f870: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000f880: 6f72 6b66 6c6f 773a 2073 7472 2c0a 2020  orkflow: str,.  
-0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f8a0: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
-0000f8b0: 6c6f 775f 7665 7273 696f 6e3a 2073 7472  low_version: str
-0000f8c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f8e0: 6e70 7574 5f64 6174 613a 2073 7472 2c0a  nput_data: str,.
-0000f8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f900: 2020 2020 2020 2020 2020 2020 2065 6d61               ema
-0000f910: 696c 3a20 4f70 7469 6f6e 616c 5b73 7472  il: Optional[str
-0000f920: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f940: 2020 2020 2020 2074 696d 653a 204f 7074         time: Opt
-0000f950: 696f 6e61 6c5b 7374 725d 203d 204e 6f6e  ional[str] = Non
-0000f960: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000f970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f980: 2a2a 6b77 6172 6773 2920 2d3e 2054 7570  **kwargs) -> Tup
-0000f990: 6c65 5b73 7472 2c20 4469 6374 5d3a 0a20  le[str, Dict]:. 
-0000f9a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000f9b0: 2020 2047 656e 6572 6174 6520 7468 6520     Generate the 
-0000f9c0: 536c 7572 6d20 776f 726b 666c 6f77 2063  Slurm workflow c
-0000f9d0: 6f6d 6d61 6e64 2061 6e64 2065 6e76 6972  ommand and envir
-0000f9e0: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-0000f9f0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-0000fa00: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
-0000fa10: 6b66 6c6f 7720 2873 7472 293a 2054 6865  kflow (str): The
-0000fa20: 206e 616d 6520 6f66 2074 6865 2077 6f72   name of the wor
-0000fa30: 6b66 6c6f 772e 0a20 2020 2020 2020 2020  kflow..         
-0000fa40: 2020 2077 6f72 6b66 6c6f 775f 7665 7273     workflow_vers
-0000fa50: 696f 6e20 2873 7472 293a 2054 6865 2076  ion (str): The v
-0000fa60: 6572 7369 6f6e 206f 6620 7468 6520 776f  ersion of the wo
-0000fa70: 726b 666c 6f77 2e0a 2020 2020 2020 2020  rkflow..        
-0000fa80: 2020 2020 696e 7075 745f 6461 7461 2028      input_data (
-0000fa90: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
-0000faa0: 6620 7468 6520 696e 7075 7420 6461 7461  f the input data
-0000fab0: 2066 6f6c 6465 7220 636f 6e74 6169 6e69   folder containi
-0000fac0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-0000fad0: 2020 2074 6865 2069 6e70 7574 2069 6d61     the input ima
-0000fae0: 6765 2066 696c 6573 2e0a 2020 2020 2020  ge files..      
-0000faf0: 2020 2020 2020 656d 6169 6c20 2873 7472        email (str
-0000fb00: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-0000fb10: 2065 6d61 696c 2061 6464 7265 7373 2066   email address f
-0000fb20: 6f72 206a 6f62 206e 6f74 6966 6963 6174  or job notificat
-0000fb30: 696f 6e73 2e0a 2020 2020 2020 2020 2020  ions..          
-0000fb40: 2020 2020 2020 4465 6661 756c 7473 2074        Defaults t
-0000fb50: 6f20 4e6f 6e65 2c20 7768 6963 6820 6465  o None, which de
-0000fb60: 6661 756c 7473 2074 6f20 7768 6174 2069  faults to what i
-0000fb70: 7320 696e 2074 6865 206a 6f62 2073 6372  s in the job scr
-0000fb80: 6970 742e 0a20 2020 2020 2020 2020 2020  ipt..           
-0000fb90: 2074 696d 6520 2873 7472 2c20 6f70 7469   time (str, opti
-0000fba0: 6f6e 616c 293a 2054 6865 2074 696d 6520  onal): The time 
-0000fbb0: 6c69 6d69 7420 666f 7220 7468 6520 6a6f  limit for the jo
-0000fbc0: 6220 696e 2074 6865 200a 2020 2020 2020  b in the .      
-0000fbd0: 2020 2020 2020 2020 2020 666f 726d 6174            format
-0000fbe0: 2048 483a 4d4d 3a53 532e 2044 6566 6175   HH:MM:SS. Defau
-0000fbf0: 6c74 7320 746f 204e 6f6e 652c 2077 6869  lts to None, whi
-0000fc00: 6368 2064 6566 6175 6c74 7320 746f 2077  ch defaults to w
-0000fc10: 6861 7420 0a20 2020 2020 2020 2020 2020  hat .           
-0000fc20: 2020 2020 2069 7320 696e 2074 6865 206a       is in the j
-0000fc30: 6f62 2073 6372 6970 742e 0a20 2020 2020  ob script..     
-0000fc40: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
-0000fc50: 2041 6464 6974 696f 6e61 6c20 6b65 7977   Additional keyw
-0000fc60: 6f72 6420 6172 6775 6d65 6e74 7320 666f  ord arguments fo
-0000fc70: 7220 7468 6520 776f 726b 666c 6f77 2e0a  r the workflow..
-0000fc80: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-0000fc90: 3a0a 2020 2020 2020 2020 2020 2020 5475  :.            Tu
-0000fca0: 706c 655b 7374 722c 2044 6963 745d 3a0a  ple[str, Dict]:.
-0000fcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fcc0: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
-0000fcd0: 6e67 2074 6865 2053 6c75 726d 2077 6f72  ng the Slurm wor
-0000fce0: 6b66 6c6f 7720 636f 6d6d 616e 6420 616e  kflow command an
-0000fcf0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0000fd00: 2020 7468 6520 656e 7669 726f 6e6d 656e    the environmen
-0000fd10: 7420 7661 7269 6162 6c65 732e 0a0a 2020  t variables...  
-0000fd20: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000fd30: 2020 6d6f 6465 6c5f 7061 7468 203d 2073    model_path = s
-0000fd40: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
-0000fd50: 7061 7468 735b 776f 726b 666c 6f77 2e6c  paths[workflow.l
-0000fd60: 6f77 6572 2829 5d0a 2020 2020 2020 2020  ower()].        
-0000fd70: 6a6f 625f 7363 7269 7074 203d 2073 656c  job_script = sel
-0000fd80: 662e 736c 7572 6d5f 6d6f 6465 6c5f 6a6f  f.slurm_model_jo
-0000fd90: 6273 5b77 6f72 6b66 6c6f 772e 6c6f 7765  bs[workflow.lowe
-0000fda0: 7228 295d 0a20 2020 2020 2020 206a 6f62  r()].        job
-0000fdb0: 5f70 6172 616d 7320 3d20 7365 6c66 2e73  _params = self.s
-0000fdc0: 6c75 726d 5f6d 6f64 656c 5f6a 6f62 735f  lurm_model_jobs_
-0000fdd0: 7061 7261 6d73 5b77 6f72 6b66 6c6f 772e  params[workflow.
-0000fde0: 6c6f 7765 7228 295d 0a20 2020 2020 2020  lower()].       
-0000fdf0: 2023 2067 7261 6220 6f6e 6c79 2074 6865   # grab only the
-0000fe00: 2069 6d61 6765 206e 616d 652c 206e 6f74   image name, not
-0000fe10: 2074 6865 2067 726f 7570 2f63 7265 6174   the group/creat
-0000fe20: 6f72 0a20 2020 2020 2020 2069 6d61 6765  or.        image
-0000fe30: 203d 2073 656c 662e 736c 7572 6d5f 6d6f   = self.slurm_mo
-0000fe40: 6465 6c5f 696d 6167 6573 5b77 6f72 6b66  del_images[workf
-0000fe50: 6c6f 772e 6c6f 7765 7228 295d 2e73 706c  low.lower()].spl
-0000fe60: 6974 2822 2f22 295b 315d 0a0a 2020 2020  it("/")[1]..    
-0000fe70: 2020 2020 7362 6174 6368 5f65 6e76 203d      sbatch_env =
-0000fe80: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-0000fe90: 4441 5441 5f50 4154 4822 3a20 6622 7b73  DATA_PATH": f"{s
-0000fea0: 656c 662e 736c 7572 6d5f 6461 7461 5f70  elf.slurm_data_p
-0000feb0: 6174 687d 2f7b 696e 7075 745f 6461 7461  ath}/{input_data
-0000fec0: 7d22 2c0a 2020 2020 2020 2020 2020 2020  }",.            
-0000fed0: 2249 4d41 4745 5f50 4154 4822 3a20 6622  "IMAGE_PATH": f"
-0000fee0: 7b73 656c 662e 736c 7572 6d5f 696d 6167  {self.slurm_imag
-0000fef0: 6573 5f70 6174 687d 2f7b 6d6f 6465 6c5f  es_path}/{model_
-0000ff00: 7061 7468 7d22 2c0a 2020 2020 2020 2020  path}",.        
-0000ff10: 2020 2020 2249 4d41 4745 5f56 4552 5349      "IMAGE_VERSI
-0000ff20: 4f4e 223a 2066 227b 776f 726b 666c 6f77  ON": f"{workflow
-0000ff30: 5f76 6572 7369 6f6e 7d22 2c0a 2020 2020  _version}",.    
-0000ff40: 2020 2020 2020 2020 2253 494e 4755 4c41          "SINGULA
-0000ff50: 5249 5459 5f49 4d41 4745 223a 2066 227b  RITY_IMAGE": f"{
-0000ff60: 696d 6167 657d 5f7b 776f 726b 666c 6f77  image}_{workflow
-0000ff70: 5f76 6572 7369 6f6e 7d2e 7369 6622 2c0a  _version}.sif",.
-0000ff80: 2020 2020 2020 2020 2020 2020 2253 4352              "SCR
-0000ff90: 4950 545f 5041 5448 223a 2066 227b 7365  IPT_PATH": f"{se
-0000ffa0: 6c66 2e73 6c75 726d 5f73 6372 6970 745f  lf.slurm_script_
-0000ffb0: 7061 7468 7d22 0a20 2020 2020 2020 207d  path}".        }
-0000ffc0: 0a20 2020 2020 2020 2077 6f72 6b66 6c6f  .        workflo
-0000ffd0: 775f 656e 7620 3d20 7365 6c66 2e77 6f72  w_env = self.wor
-0000ffe0: 6b66 6c6f 775f 7061 7261 6d73 5f74 6f5f  kflow_params_to_
-0000fff0: 656e 7676 6172 7328 2a2a 6b77 6172 6773  envvars(**kwargs
-00010000: 290a 2020 2020 2020 2020 656e 7620 3d20  ).        env = 
-00010010: 7b2a 2a73 6261 7463 685f 656e 762c 202a  {**sbatch_env, *
-00010020: 2a77 6f72 6b66 6c6f 775f 656e 767d 0a0a  *workflow_env}..
-00010030: 2020 2020 2020 2020 656d 6169 6c5f 7061          email_pa
-00010040: 7261 6d20 3d20 2222 2069 6620 656d 6169  ram = "" if emai
-00010050: 6c20 6973 204e 6f6e 6520 656c 7365 2066  l is None else f
-00010060: 2220 2d2d 6d61 696c 2d75 7365 723d 7b65  " --mail-user={e
-00010070: 6d61 696c 7d22 0a20 2020 2020 2020 2074  mail}".        t
-00010080: 696d 655f 7061 7261 6d20 3d20 2222 2069  ime_param = "" i
-00010090: 6620 7469 6d65 2069 7320 4e6f 6e65 2065  f time is None e
-000100a0: 6c73 6520 6622 202d 2d74 696d 653d 7b74  lse f" --time={t
-000100b0: 696d 657d 220a 2020 2020 2020 2020 6a6f  ime}".        jo
-000100c0: 625f 7061 7261 6d73 2e61 7070 656e 6428  b_params.append(
-000100d0: 7469 6d65 5f70 6172 616d 290a 2020 2020  time_param).    
-000100e0: 2020 2020 6a6f 625f 7061 7261 6d73 2e61      job_params.a
-000100f0: 7070 656e 6428 656d 6169 6c5f 7061 7261  ppend(email_para
-00010100: 6d29 0a20 2020 2020 2020 206a 6f62 5f70  m).        job_p
-00010110: 6172 616d 203d 2022 222e 6a6f 696e 286a  aram = "".join(j
-00010120: 6f62 5f70 6172 616d 7329 0a20 2020 2020  ob_params).     
-00010130: 2020 2073 6261 7463 685f 636d 6420 3d20     sbatch_cmd = 
-00010140: 6622 7362 6174 6368 7b6a 6f62 5f70 6172  f"sbatch{job_par
-00010150: 616d 7d20 2d2d 6f75 7470 7574 3d6f 6d65  am} --output=ome
-00010160: 726f 2d25 6a2e 6c6f 6720 5c0a 2020 2020  ro-%j.log \.    
-00010170: 2020 2020 2020 2020 7b73 656c 662e 736c          {self.sl
-00010180: 7572 6d5f 7363 7269 7074 5f70 6174 687d  urm_script_path}
-00010190: 2f7b 6a6f 625f 7363 7269 7074 7d22 0a0a  /{job_script}"..
-000101a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000101b0: 6261 7463 685f 636d 642c 2065 6e76 0a0a  batch_cmd, env..
-000101c0: 2020 2020 6465 6620 6765 745f 636f 6e76      def get_conv
-000101d0: 6572 7369 6f6e 5f63 6f6d 6d61 6e64 2873  ersion_command(s
-000101e0: 656c 662c 2064 6174 615f 7061 7468 3a20  elf, data_path: 
-000101f0: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
-00010200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010210: 2020 2020 636f 6e66 6967 5f66 696c 653a      config_file:
-00010220: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-00010230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010240: 2020 2020 2073 6f75 7263 655f 666f 726d       source_form
-00010250: 6174 3a20 7374 7220 3d20 277a 6172 7227  at: str = 'zarr'
-00010260: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00010270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010280: 2074 6172 6765 745f 666f 726d 6174 3a20   target_format: 
-00010290: 7374 7220 3d20 2774 6966 6627 2920 2d3e  str = 'tiff') ->
-000102a0: 2054 7570 6c65 5b73 7472 2c20 4469 6374   Tuple[str, Dict
-000102b0: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-000102c0: 2020 2020 2020 2047 656e 6572 6174 6520         Generate 
-000102d0: 536c 7572 6d20 636f 6e76 6572 7369 6f6e  Slurm conversion
-000102e0: 2063 6f6d 6d61 6e64 2061 6e64 2065 6e76   command and env
-000102f0: 6972 6f6e 6d65 6e74 2076 6172 6961 626c  ironment variabl
-00010300: 6573 2066 6f72 2064 6174 6120 636f 6e76  es for data conv
-00010310: 6572 7369 6f6e 2e0a 0a20 2020 2020 2020  ersion...       
-00010320: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00010330: 2020 2064 6174 615f 7061 7468 2028 7374     data_path (st
-00010340: 7229 3a20 5061 7468 2074 6f20 7468 6520  r): Path to the 
-00010350: 6461 7461 2066 6f6c 6465 722e 0a20 2020  data folder..   
-00010360: 2020 2020 2020 2020 2063 6f6e 6669 675f           config_
-00010370: 6669 6c65 2028 7374 7229 3a20 5061 7468  file (str): Path
-00010380: 2074 6f20 7468 6520 636f 6e66 6967 7572   to the configur
-00010390: 6174 696f 6e20 6669 6c65 2e0a 2020 2020  ation file..    
-000103a0: 2020 2020 2020 2020 736f 7572 6365 5f66          source_f
-000103b0: 6f72 6d61 7420 2873 7472 293a 2053 6f75  ormat (str): Sou
-000103c0: 7263 6520 6461 7461 2066 6f72 6d61 7420  rce data format 
-000103d0: 2864 6566 6175 6c74 2069 7320 277a 6172  (default is 'zar
-000103e0: 7227 292e 0a20 2020 2020 2020 2020 2020  r')..           
-000103f0: 2074 6172 6765 745f 666f 726d 6174 2028   target_format (
-00010400: 7374 7229 3a20 5461 7267 6574 2064 6174  str): Target dat
-00010410: 6120 666f 726d 6174 2028 6465 6661 756c  a format (defaul
-00010420: 7420 6973 2027 7469 6666 2729 2e0a 0a20  t is 'tiff')... 
-00010430: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00010440: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
-00010450: 655b 7374 722c 2044 6963 745d 3a0a 2020  e[str, Dict]:.  
-00010460: 2020 2020 2020 2020 2020 2020 2020 4120                A 
-00010470: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
-00010480: 2074 6865 2053 6c75 726d 2063 6f6e 7665   the Slurm conve
-00010490: 7273 696f 6e20 636f 6d6d 616e 6420 616e  rsion command an
-000104a0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-000104b0: 2020 7468 6520 656e 7669 726f 6e6d 656e    the environmen
-000104c0: 7420 7661 7269 6162 6c65 732e 0a0a 2020  t variables...  
-000104d0: 2020 2020 2020 5761 726e 696e 673a 0a20        Warning:. 
-000104e0: 2020 2020 2020 2020 2020 2054 6865 2064             The d
-000104f0: 6566 6175 6c74 2069 6d70 6c65 6d65 6e74  efault implement
-00010500: 6174 696f 6e20 6f6e 6c79 2073 7570 706f  ation only suppo
-00010510: 7274 7320 636f 6e76 6572 7369 6f6e 2066  rts conversion f
-00010520: 726f 6d20 277a 6172 7227 2074 6f20 2774  rom 'zarr' to 't
-00010530: 6966 6627 2e0a 2020 2020 2020 2020 2020  iff'..          
-00010540: 2020 4966 2075 7369 6e67 206f 7468 6572    If using other
-00010550: 2073 6f75 7263 6520 6f72 2074 6172 6765   source or targe
-00010560: 7420 666f 726d 6174 732c 2075 7365 7273  t formats, users
-00010570: 206d 7573 7420 696d 706c 656d 656e 7420   must implement 
-00010580: 616e 6420 636f 6e66 6967 7572 650a 2020  and configure.  
-00010590: 2020 2020 2020 2020 2020 6164 6469 7469            additi
-000105a0: 6f6e 616c 2063 6f6e 7665 7274 6572 7320  onal converters 
-000105b0: 7468 656d 7365 6c76 6573 2e0a 2020 2020  themselves..    
-000105c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000105d0: 6966 2073 6f75 7263 655f 666f 726d 6174  if source_format
-000105e0: 2021 3d20 227a 6172 7222 206f 7220 7461   != "zarr" or ta
-000105f0: 7267 6574 5f66 6f72 6d61 7420 213d 2022  rget_format != "
-00010600: 7469 6666 223a 0a20 2020 2020 2020 2020  tiff":.         
-00010610: 2020 2023 2057 6172 6e20 6162 6f75 7420     # Warn about 
-00010620: 756e 7375 7070 6f72 7465 6420 636f 6e76  unsupported conv
-00010630: 6572 7369 6f6e 3b20 6164 6469 7469 6f6e  ersion; addition
-00010640: 616c 2063 6f6e 7665 7274 6572 7320 6361  al converters ca
-00010650: 6e20 6265 0a20 2020 2020 2020 2020 2020  n be.           
-00010660: 2023 2061 6464 6564 206f 7574 7369 6465   # added outside
-00010670: 206f 7572 206b 6e6f 776c 6564 6765 2e0a   our knowledge..
-00010680: 2020 2020 2020 2020 2020 2020 2320 4368              # Ch
-00010690: 6563 6b69 6e67 2053 6c75 726d 2773 2060  ecking Slurm's `
-000106a0: 736c 7572 6d5f 636f 6e76 6572 7465 7273  slurm_converters
-000106b0: 5f70 6174 6860 2069 7320 736b 6970 7065  _path` is skippe
-000106c0: 6420 666f 720a 2020 2020 2020 2020 2020  d for.          
-000106d0: 2020 2320 7065 7266 6f72 6d61 6e63 6520    # performance 
-000106e0: 7265 6173 6f6e 732e 0a20 2020 2020 2020  reasons..       
-000106f0: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
-00010700: 696e 6728 0a20 2020 2020 2020 2020 2020  ing(.           
-00010710: 2020 2020 2066 2243 6f6e 7665 7273 696f       f"Conversio
-00010720: 6e20 6672 6f6d 207b 736f 7572 6365 5f66  n from {source_f
-00010730: 6f72 6d61 747d 2074 6f20 7b74 6172 6765  ormat} to {targe
-00010740: 745f 666f 726d 6174 7d20 6973 206e 6f74  t_format} is not
-00010750: 2073 7570 706f 7274 6564 2062 7920 6465   supported by de
-00010760: 6661 756c 7421 2229 0a0a 2020 2020 2020  fault!")..      
-00010770: 2020 6368 6f73 656e 5f63 6f6e 7665 7274    chosen_convert
-00010780: 6572 203d 2066 2263 6f6e 7665 7274 5f7b  er = f"convert_{
-00010790: 736f 7572 6365 5f66 6f72 6d61 747d 5f74  source_format}_t
-000107a0: 6f5f 7b74 6172 6765 745f 666f 726d 6174  o_{target_format
-000107b0: 7d2e 7369 6622 0a20 2020 2020 2020 2073  }.sif".        s
-000107c0: 6261 7463 685f 656e 7620 3d20 7b0a 2020  batch_env = {.  
-000107d0: 2020 2020 2020 2020 2020 2244 4154 415f            "DATA_
-000107e0: 5041 5448 223a 2066 227b 6461 7461 5f70  PATH": f"{data_p
-000107f0: 6174 687d 222c 0a20 2020 2020 2020 2020  ath}",.         
-00010800: 2020 2022 434f 4e56 4552 5349 4f4e 5f50     "CONVERSION_P
-00010810: 4154 4822 3a20 6622 7b73 656c 662e 736c  ATH": f"{self.sl
-00010820: 7572 6d5f 636f 6e76 6572 7465 7273 5f70  urm_converters_p
-00010830: 6174 687d 222c 0a20 2020 2020 2020 2020  ath}",.         
-00010840: 2020 2022 434f 4e56 4552 5445 525f 494d     "CONVERTER_IM
-00010850: 4147 4522 3a20 6368 6f73 656e 5f63 6f6e  AGE": chosen_con
-00010860: 7665 7274 6572 2c0a 2020 2020 2020 2020  verter,.        
-00010870: 2020 2020 2253 4352 4950 545f 5041 5448      "SCRIPT_PATH
-00010880: 223a 2066 227b 7365 6c66 2e73 6c75 726d  ": f"{self.slurm
-00010890: 5f73 6372 6970 745f 7061 7468 7d22 2c0a  _script_path}",.
-000108a0: 2020 2020 2020 2020 2020 2020 2243 4f4e              "CON
-000108b0: 4649 475f 4649 4c45 223a 2066 227b 636f  FIG_FILE": f"{co
-000108c0: 6e66 6967 5f66 696c 657d 220a 2020 2020  nfig_file}".    
-000108d0: 2020 2020 7d0a 0a20 2020 2020 2020 2063      }..        c
-000108e0: 6f6e 7665 7273 696f 6e5f 636d 6420 3d20  onversion_cmd = 
-000108f0: 2273 6261 7463 6820 2d2d 6a6f 622d 6e61  "sbatch --job-na
-00010900: 6d65 3d63 6f6e 7665 7273 696f 6e20 2d2d  me=conversion --
-00010910: 6578 706f 7274 3d41 4c4c 2c43 4f4e 4649  export=ALL,CONFI
-00010920: 475f 5041 5448 3d5c 2224 5057 442f 2443  G_PATH=\"$PWD/$C
-00010930: 4f4e 4649 475f 4649 4c45 5c22 202d 2d61  ONFIG_FILE\" --a
-00010940: 7272 6179 3d31 2d24 4e20 2453 4352 4950  rray=1-$N $SCRIP
-00010950: 545f 5041 5448 2f63 6f6e 7665 7274 5f6a  T_PATH/convert_j
-00010960: 6f62 5f61 7272 6179 2e73 6822 0a20 2020  ob_array.sh".   
-00010970: 2020 2020 2023 2063 6f6e 7665 7273 696f       # conversio
-00010980: 6e5f 636d 645f 7761 6974 696e 6720 3d20  n_cmd_waiting = 
-00010990: 2273 6261 7463 6820 2d2d 6a6f 622d 6e61  "sbatch --job-na
-000109a0: 6d65 3d63 6f6e 7665 7273 696f 6e20 2d2d  me=conversion --
-000109b0: 6578 706f 7274 3d41 4c4c 2c43 4f4e 4649  export=ALL,CONFI
-000109c0: 475f 5041 5448 3d5c 2224 5057 442f 2443  G_PATH=\"$PWD/$C
-000109d0: 4f4e 4649 475f 4649 4c45 5c22 202d 2d61  ONFIG_FILE\" --a
-000109e0: 7272 6179 3d31 2d24 4e20 2d2d 7761 6974  rray=1-$N --wait
-000109f0: 2024 5343 5249 5054 5f50 4154 482f 636f   $SCRIPT_PATH/co
-00010a00: 6e76 6572 745f 6a6f 625f 6172 7261 792e  nvert_job_array.
-00010a10: 7368 220a 0a20 2020 2020 2020 2072 6574  sh"..        ret
-00010a20: 7572 6e20 636f 6e76 6572 7369 6f6e 5f63  urn conversion_c
-00010a30: 6d64 2c20 7362 6174 6368 5f65 6e76 0a0a  md, sbatch_env..
-00010a40: 2020 2020 6465 6620 776f 726b 666c 6f77      def workflow
-00010a50: 5f70 6172 616d 735f 746f 5f65 6e76 7661  _params_to_envva
-00010a60: 7273 2873 656c 662c 202a 2a6b 7761 7267  rs(self, **kwarg
-00010a70: 7329 202d 3e20 4469 6374 3a0a 2020 2020  s) -> Dict:.    
-00010a80: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00010a90: 436f 6e76 6572 7420 776f 726b 666c 6f77  Convert workflow
-00010aa0: 2070 6172 616d 6574 6572 7320 746f 2065   parameters to e
-00010ab0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00010ac0: 626c 6573 2e0a 0a20 2020 2020 2020 2041  bles...        A
-00010ad0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00010ae0: 202a 2a6b 7761 7267 733a 2041 6464 6974   **kwargs: Addit
-00010af0: 696f 6e61 6c20 6b65 7977 6f72 6420 6172  ional keyword ar
-00010b00: 6775 6d65 6e74 7320 666f 7220 7468 6520  guments for the 
-00010b10: 776f 726b 666c 6f77 2e0a 0a20 2020 2020  workflow...     
-00010b20: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00010b30: 2020 2020 2020 2020 4469 6374 3a20 4120          Dict: A 
-00010b40: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
-00010b50: 696e 696e 6720 7468 6520 656e 7669 726f  ining the enviro
-00010b60: 6e6d 656e 7420 7661 7269 6162 6c65 732e  nment variables.
-00010b70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00010b80: 2020 2020 2077 6f72 6b66 6c6f 775f 656e       workflow_en
-00010b90: 7620 3d20 7b6b 6579 2e75 7070 6572 2829  v = {key.upper()
-00010ba0: 3a20 6622 7b76 616c 7565 7d22 2066 6f72  : f"{value}" for
-00010bb0: 206b 6579 2c0a 2020 2020 2020 2020 2020   key,.          
-00010bc0: 2020 2020 2020 2020 2020 2020 2020 7661                va
-00010bd0: 6c75 6520 696e 206b 7761 7267 732e 6974  lue in kwargs.it
-00010be0: 656d 7328 297d 0a20 2020 2020 2020 206c  ems()}.        l
-00010bf0: 6f67 6765 722e 6465 6275 6728 776f 726b  ogger.debug(work
-00010c00: 666c 6f77 5f65 6e76 290a 2020 2020 2020  flow_env).      
-00010c10: 2020 7265 7475 726e 2077 6f72 6b66 6c6f    return workflo
-00010c20: 775f 656e 760a 0a20 2020 2064 6566 2067  w_env..    def g
-00010c30: 6574 5f63 656c 6c70 6f73 655f 636f 6d6d  et_cellpose_comm
-00010c40: 616e 6428 7365 6c66 2c20 696d 6167 655f  and(self, image_
-00010c50: 7665 7273 696f 6e3a 2073 7472 2c0a 2020  version: str,.  
-00010c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c70: 2020 2020 2020 2020 2020 2069 6e70 7574             input
-00010c80: 5f64 6174 613a 2073 7472 2c0a 2020 2020  _data: str,.    
-00010c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010ca0: 2020 2020 2020 2020 2063 705f 6d6f 6465           cp_mode
-00010cb0: 6c3a 2073 7472 2c0a 2020 2020 2020 2020  l: str,.        
-00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cd0: 2020 2020 206e 7563 5f63 6861 6e6e 656c       nuc_channel
-00010ce0: 3a20 696e 742c 0a20 2020 2020 2020 2020  : int,.         
-00010cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d00: 2020 2020 7072 6f62 5f74 6872 6573 686f      prob_thresho
-00010d10: 6c64 3a20 666c 6f61 742c 0a20 2020 2020  ld: float,.     
-00010d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d30: 2020 2020 2020 2020 6365 6c6c 5f64 6961          cell_dia
-00010d40: 6d65 7465 723a 2066 6c6f 6174 2c0a 2020  meter: float,.  
-00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d60: 2020 2020 2020 2020 2020 2065 6d61 696c             email
-00010d70: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00010d80: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010da0: 2020 2020 2074 696d 653a 204f 7074 696f       time: Optio
-00010db0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00010dc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010dd0: 2020 2020 2020 2020 2020 2020 2020 7573                us
-00010de0: 655f 6770 753a 2062 6f6f 6c20 3d20 5472  e_gpu: bool = Tr
-00010df0: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00010e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010e10: 206d 6f64 656c 3a20 7374 7220 3d20 2263   model: str = "c
-00010e20: 656c 6c70 6f73 6522 2920 2d3e 2054 7570  ellpose") -> Tup
-00010e30: 6c65 5b73 7472 2c20 4469 6374 5d3a 0a20  le[str, Dict]:. 
-00010e40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00010e50: 2020 2052 6574 7572 6e20 7468 6520 636f     Return the co
-00010e60: 6d6d 616e 6420 616e 6420 656e 7669 726f  mmand and enviro
-00010e70: 6e6d 656e 7420 6469 6374 696f 6e61 7279  nment dictionary
-00010e80: 2074 6f20 7275 6e20 6120 4365 6c6c 506f   to run a CellPo
-00010e90: 7365 206a 6f62 0a20 2020 2020 2020 206f  se job.        o
-00010ea0: 6e20 7468 6520 536c 7572 6d20 776f 726b  n the Slurm work
-00010eb0: 6c6f 6164 206d 616e 6167 6572 2e0a 2020  load manager..  
-00010ec0: 2020 2020 2020 4120 7370 6563 6966 6963        A specific
-00010ed0: 2065 7861 6d70 6c65 206f 6620 7573 696e   example of usin
-00010ee0: 6720 7468 6520 6765 6e65 7269 6320 2767  g the generic 'g
-00010ef0: 6574 5f77 6f72 6b66 6c6f 775f 636f 6d6d  et_workflow_comm
-00010f00: 616e 6427 2e0a 0a20 2020 2020 2020 2041  and'...        A
-00010f10: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00010f20: 2069 6d61 6765 5f76 6572 7369 6f6e 2028   image_version (
-00010f30: 7374 7229 3a20 5468 6520 7665 7273 696f  str): The versio
-00010f40: 6e20 6f66 2074 6865 2053 696e 6775 6c61  n of the Singula
-00010f50: 7269 7479 2069 6d61 6765 2074 6f20 7573  rity image to us
-00010f60: 652e 0a20 2020 2020 2020 2020 2020 2069  e..            i
-00010f70: 6e70 7574 5f64 6174 6120 2873 7472 293a  nput_data (str):
-00010f80: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-00010f90: 2069 6e70 7574 2064 6174 6120 666f 6c64   input data fold
-00010fa0: 6572 206f 6e20 7468 6520 7368 6172 6564  er on the shared
-00010fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010fc0: 2066 696c 6520 7379 7374 656d 2e0a 2020   file system..  
-00010fd0: 2020 2020 2020 2020 2020 6370 5f6d 6f64            cp_mod
-00010fe0: 656c 2028 7374 7229 3a20 5468 6520 6e61  el (str): The na
-00010ff0: 6d65 206f 6620 7468 6520 4365 6c6c 506f  me of the CellPo
-00011000: 7365 206d 6f64 656c 2074 6f20 7573 652e  se model to use.
-00011010: 0a20 2020 2020 2020 2020 2020 206e 7563  .            nuc
-00011020: 5f63 6861 6e6e 656c 2028 696e 7429 3a20  _channel (int): 
-00011030: 5468 6520 696e 6465 7820 6f66 2074 6865  The index of the
-00011040: 206e 7563 6c65 6172 2063 6861 6e6e 656c   nuclear channel
-00011050: 2e0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00011060: 6f62 5f74 6872 6573 686f 6c64 2028 666c  ob_threshold (fl
-00011070: 6f61 7429 3a20 5468 6520 7072 6f62 6162  oat): The probab
-00011080: 696c 6974 7920 7468 7265 7368 6f6c 6420  ility threshold 
-00011090: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
-000110a0: 2020 2020 6e75 636c 6569 2064 6574 6563      nuclei detec
-000110b0: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
-000110c0: 2020 6365 6c6c 5f64 6961 6d65 7465 7220    cell_diameter 
-000110d0: 2866 6c6f 6174 293a 2054 6865 2065 7870  (float): The exp
-000110e0: 6563 7465 6420 6365 6c6c 2064 6961 6d65  ected cell diame
-000110f0: 7465 7220 696e 2070 6978 656c 732e 0a20  ter in pixels.. 
-00011100: 2020 2020 2020 2020 2020 2065 6d61 696c             email
-00011110: 2028 4f70 7469 6f6e 616c 5b73 7472 5d29   (Optional[str])
-00011120: 3a20 5468 6520 656d 6169 6c20 6164 6472  : The email addr
-00011130: 6573 7320 746f 2073 656e 6420 6e6f 7469  ess to send noti
-00011140: 6669 6361 7469 6f6e 7320 746f 2e0a 2020  fications to..  
-00011150: 2020 2020 2020 2020 2020 2020 2020 4465                De
-00011160: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
-00011170: 2020 2020 2020 2020 2020 2020 7469 6d65              time
-00011180: 2028 4f70 7469 6f6e 616c 5b73 7472 5d29   (Optional[str])
-00011190: 3a20 5468 6520 6d61 7869 6d75 6d20 7469  : The maximum ti
-000111a0: 6d65 2066 6f72 2074 6865 206a 6f62 2074  me for the job t
-000111b0: 6f20 7275 6e2e 0a20 2020 2020 2020 2020  o run..         
-000111c0: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-000111d0: 746f 204e 6f6e 652e 0a20 2020 2020 2020  to None..       
-000111e0: 2020 2020 2075 7365 5f67 7075 2028 626f       use_gpu (bo
-000111f0: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
-00011200: 7573 6520 4750 5520 666f 7220 7468 6520  use GPU for the 
-00011210: 4365 6c6c 506f 7365 206a 6f62 2e0a 2020  CellPose job..  
-00011220: 2020 2020 2020 2020 2020 2020 2020 4465                De
-00011230: 6661 756c 7473 2074 6f20 5472 7565 2e0a  faults to True..
-00011240: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
-00011250: 6c20 2873 7472 293a 2054 6865 206e 616d  l (str): The nam
-00011260: 6520 6f66 2074 6865 2066 6f6c 6465 7220  e of the folder 
-00011270: 6f66 2074 6865 2044 6f63 6b65 7220 696d  of the Docker im
-00011280: 6167 6520 746f 2075 7365 2e0a 2020 2020  age to use..    
-00011290: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
-000112a0: 756c 7473 2074 6f20 2263 656c 6c70 6f73  ults to "cellpos
-000112b0: 6522 2e0a 0a20 2020 2020 2020 2052 6574  e"...        Ret
-000112c0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-000112d0: 2020 5475 706c 655b 7374 722c 2064 6963    Tuple[str, dic
-000112e0: 745d 3a0a 2020 2020 2020 2020 2020 2020  t]:.            
-000112f0: 2020 2020 4120 7475 706c 6520 636f 6e74      A tuple cont
-00011300: 6169 6e69 6e67 2074 6865 2053 6c75 726d  aining the Slurm
-00011310: 2073 6261 7463 6820 636f 6d6d 616e 640a   sbatch command.
-00011320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011330: 616e 6420 7468 6520 656e 7669 726f 6e6d  and the environm
-00011340: 656e 7420 6469 6374 696f 6e61 7279 2e0a  ent dictionary..
-00011350: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011360: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00011370: 6765 745f 776f 726b 666c 6f77 5f63 6f6d  get_workflow_com
-00011380: 6d61 6e64 2877 6f72 6b66 6c6f 773d 6d6f  mand(workflow=mo
-00011390: 6465 6c2c 0a20 2020 2020 2020 2020 2020  del,.           
-000113a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113b0: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-000113c0: 726b 666c 6f77 5f76 6572 7369 6f6e 3d69  rkflow_version=i
-000113d0: 6d61 6765 5f76 6572 7369 6f6e 2c0a 2020  mage_version,.  
-000113e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000113f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011400: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
-00011410: 613d 696e 7075 745f 6461 7461 2c0a 2020  a=input_data,.  
-00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011440: 2020 2020 2020 2065 6d61 696c 3d65 6d61         email=ema
-00011450: 696c 2c0a 2020 2020 2020 2020 2020 2020  il,.            
-00011460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011470: 2020 2020 2020 2020 2020 2020 2074 696d               tim
-00011480: 653d 7469 6d65 2c0a 2020 2020 2020 2020  e=time,.        
-00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114b0: 2063 705f 6d6f 6465 6c3d 6370 5f6d 6f64   cp_model=cp_mod
-000114c0: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
-000114d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114e0: 2020 2020 2020 2020 2020 2020 206e 7563               nuc
-000114f0: 5f63 6861 6e6e 656c 3d6e 7563 5f63 6861  _channel=nuc_cha
-00011500: 6e6e 656c 2c0a 2020 2020 2020 2020 2020  nnel,.          
-00011510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011520: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00011530: 726f 625f 7468 7265 7368 6f6c 643d 7072  rob_threshold=pr
-00011540: 6f62 5f74 6872 6573 686f 6c64 2c0a 2020  ob_threshold,.  
-00011550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011570: 2020 2020 2020 2063 656c 6c5f 6469 616d         cell_diam
-00011580: 6574 6572 3d63 656c 6c5f 6469 616d 6574  eter=cell_diamet
-00011590: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-000115a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115b0: 2020 2020 2020 2020 2020 2020 2075 7365               use
-000115c0: 5f67 7075 3d75 7365 5f67 7075 290a 0a20  _gpu=use_gpu).. 
-000115d0: 2020 2064 6566 2063 6f70 795f 7a69 705f     def copy_zip_
-000115e0: 6c6f 6361 6c6c 7928 7365 6c66 2c20 6c6f  locally(self, lo
-000115f0: 6361 6c5f 746d 705f 7374 6f72 6167 653a  cal_tmp_storage:
-00011600: 2073 7472 2c20 6669 6c65 6e61 6d65 3a20   str, filename: 
-00011610: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-00011620: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-00011630: 3e20 5472 616e 7366 6572 5265 7375 6c74  > TransferResult
-00011640: 3a0a 2020 2020 2020 2020 2222 2220 436f  :.        """ Co
-00011650: 7079 2061 207a 6970 2066 696c 6520 6672  py a zip file fr
-00011660: 6f6d 2053 6c75 726d 2074 6f20 7468 6520  om Slurm to the 
-00011670: 6c6f 6361 6c20 7365 7276 6572 2e0a 0a20  local server... 
-00011680: 2020 2020 2020 204e 6f74 6520 6162 6f75         Note abou
-00011690: 7420 2854 7261 6e73 6665 7229 5265 7375  t (Transfer)Resu
-000116a0: 6c74 3a0a 0a20 2020 2020 2020 2055 6e6c  lt:..        Unl
-000116b0: 696b 6520 7369 6d69 6c61 7220 636c 6173  ike similar clas
-000116c0: 7365 7320 7375 6368 2061 7320 696e 766f  ses such as invo
-000116d0: 6b65 2e72 756e 6e65 7273 2e52 6573 756c  ke.runners.Resul
-000116e0: 7420 6f72 0a20 2020 2020 2020 2066 6162  t or.        fab
-000116f0: 7269 632e 7275 6e6e 6572 732e 5265 7375  ric.runners.Resu
-00011700: 6c74 0a20 2020 2020 2020 2028 7768 6963  lt.        (whic
-00011710: 6820 6861 7665 2061 2063 6f6e 6365 7074  h have a concept
-00011720: 206f 6620 e280 9c77 6172 6e20 616e 6420   of ...warn and 
-00011730: 7265 7475 726e 2061 6e79 7761 7973 206f  return anyways o
-00011740: 6e20 6661 696c 7572 65e2 809d 290a 2020  n failure...).  
-00011750: 2020 2020 2020 7468 6973 2063 6c61 7373        this class
-00011760: 2068 6173 206e 6f20 7573 6566 756c 2074   has no useful t
-00011770: 7275 7468 696e 6573 7320 6265 6861 7669  ruthiness behavi
-00011780: 6f72 2e0a 2020 2020 2020 2020 4966 2061  or..        If a
-00011790: 2066 696c 6520 7472 616e 7366 6572 2066   file transfer f
-000117a0: 6169 6c73 2c20 736f 6d65 2065 7863 6570  ails, some excep
-000117b0: 7469 6f6e 2077 696c 6c20 6265 2072 6169  tion will be rai
-000117c0: 7365 642c 0a20 2020 2020 2020 2065 6974  sed,.        eit
-000117d0: 6865 7220 616e 204f 5345 7272 6f72 206f  her an OSError o
-000117e0: 7220 616e 2065 7272 6f72 2066 726f 6d20  r an error from 
-000117f0: 7769 7468 696e 2050 6172 616d 696b 6f2e  within Paramiko.
-00011800: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00011810: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00011820: 6c5f 746d 705f 7374 6f72 6167 6520 2853  l_tmp_storage (S
-00011830: 7472 696e 6729 3a20 5061 7468 2074 6f20  tring): Path to 
-00011840: 7374 6f72 6520 7468 6520 7a69 7020 6669  store the zip fi
-00011850: 6c65 206c 6f63 616c 6c79 2e0a 2020 2020  le locally..    
-00011860: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
-00011870: 2028 5374 7269 6e67 293a 205a 6970 2066   (String): Zip f
-00011880: 696c 656e 616d 6520 6f6e 2053 6c75 726d  ilename on Slurm
-00011890: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-000118a0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-000118b0: 5472 616e 7366 6572 5265 7375 6c74 3a20  TransferResult: 
-000118c0: 5468 6520 7265 7375 6c74 206f 6620 7468  The result of th
-000118d0: 6520 7363 7020 6174 7465 6d70 742e 0a20  e scp attempt.. 
-000118e0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000118f0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
-00011900: 2243 6f70 7969 6e67 207a 6970 207b 6669  "Copying zip {fi
-00011910: 6c65 6e61 6d65 7d20 6672 6f6d 5c0a 2020  lename} from\.  
-00011920: 2020 2020 2020 2020 2020 536c 7572 6d20            Slurm 
-00011930: 746f 207b 6c6f 6361 6c5f 746d 705f 7374  to {local_tmp_st
-00011940: 6f72 6167 657d 2229 0a20 2020 2020 2020  orage}").       
-00011950: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
-00011960: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
-00011970: 6d6f 7465 3d66 227b 6669 6c65 6e61 6d65  mote=f"{filename
-00011980: 7d2e 7a69 7022 2c0a 2020 2020 2020 2020  }.zip",.        
-00011990: 2020 2020 6c6f 6361 6c3d 6c6f 6361 6c5f      local=local_
-000119a0: 746d 705f 7374 6f72 6167 6529 0a0a 2020  tmp_storage)..  
-000119b0: 2020 6465 6620 7a69 705f 6461 7461 5f6f    def zip_data_o
-000119c0: 6e5f 736c 7572 6d5f 7365 7276 6572 2873  n_slurm_server(s
-000119d0: 656c 662c 2064 6174 615f 6c6f 6361 7469  elf, data_locati
-000119e0: 6f6e 3a20 7374 722c 2066 696c 656e 616d  on: str, filenam
-000119f0: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
-00011a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a10: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
-00011a20: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-00011a30: 2073 7472 5d5d 203d 204e 6f6e 650a 2020   str]] = None.  
+0000bb10: 2020 2a2a 6b77 6172 6773 0a20 2020 2020    **kwargs.     
+0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb30: 2920 2d3e 2054 7570 6c65 5b52 6573 756c  ) -> Tuple[Resul
+0000bb40: 742c 2069 6e74 5d3a 0a20 2020 2020 2020  t, int]:.       
+0000bb50: 2022 2222 0a20 2020 2020 2020 2052 756e   """.        Run
+0000bb60: 2061 2073 7065 6369 6669 6564 2077 6f72   a specified wor
+0000bb70: 6b66 6c6f 7720 6f6e 2053 6c75 726d 2075  kflow on Slurm u
+0000bb80: 7369 6e67 2074 6865 2067 6976 656e 2070  sing the given p
+0000bb90: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
+0000bba0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000bbb0: 2020 2020 2020 776f 726b 666c 6f77 5f6e        workflow_n
+0000bbc0: 616d 6520 2873 7472 293a 204e 616d 6520  ame (str): Name 
+0000bbd0: 6f66 2074 6865 2077 6f72 6b66 6c6f 7720  of the workflow 
+0000bbe0: 746f 2065 7865 6375 7465 2e0a 2020 2020  to execute..    
+0000bbf0: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
+0000bc00: 5f76 6572 7369 6f6e 2028 7374 7229 3a20  _version (str): 
+0000bc10: 5665 7273 696f 6e20 6f66 2074 6865 2077  Version of the w
+0000bc20: 6f72 6b66 6c6f 7720 2869 6d61 6765 2076  orkflow (image v
+0000bc30: 6572 7369 6f6e 200a 2020 2020 2020 2020  ersion .        
+0000bc40: 2020 2020 2020 2020 6f6e 2053 6c75 726d          on Slurm
+0000bc50: 292e 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000bc60: 6e70 7574 5f64 6174 6120 2873 7472 293a  nput_data (str):
+0000bc70: 204e 616d 6520 6f66 2074 6865 2069 6e70   Name of the inp
+0000bc80: 7574 2064 6174 6120 666f 6c64 6572 2063  ut data folder c
+0000bc90: 6f6e 7461 696e 696e 6720 696e 7075 740a  ontaining input.
+0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcb0: 696d 6167 6520 6669 6c65 732e 0a20 2020  image files..   
+0000bcc0: 2020 2020 2020 2020 2065 6d61 696c 2028           email (
+0000bcd0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
+0000bce0: 456d 6169 6c20 6164 6472 6573 7320 666f  Email address fo
+0000bcf0: 7220 536c 7572 6d20 6a6f 6220 6e6f 7469  r Slurm job noti
+0000bd00: 6669 6361 7469 6f6e 732e 0a20 2020 2020  fications..     
+0000bd10: 2020 2020 2020 2074 696d 6520 2873 7472         time (str
+0000bd20: 2c20 6f70 7469 6f6e 616c 293a 2054 696d  , optional): Tim
+0000bd30: 6520 6c69 6d69 7420 666f 7220 7468 6520  e limit for the 
+0000bd40: 536c 7572 6d20 6a6f 6220 696e 2074 6865  Slurm job in the
+0000bd50: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000bd60: 2020 666f 726d 6174 2048 483a 4d4d 3a53    format HH:MM:S
+0000bd70: 532e 0a20 2020 2020 2020 2020 2020 202a  S..            *
+0000bd80: 2a6b 7761 7267 733a 2041 6464 6974 696f  *kwargs: Additio
+0000bd90: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
+0000bda0: 6d65 6e74 7320 666f 7220 7468 6520 776f  ments for the wo
+0000bdb0: 726b 666c 6f77 2e0a 0a20 2020 2020 2020  rkflow...       
+0000bdc0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000bdd0: 2020 2020 2020 5475 706c 655b 5265 7375        Tuple[Resu
+0000bde0: 6c74 2c20 696e 745d 3a0a 2020 2020 2020  lt, int]:.      
+0000bdf0: 2020 2020 2020 2020 2020 4120 7475 706c            A tupl
+0000be00: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
+0000be10: 2072 6573 756c 7420 6f66 2073 7461 7274   result of start
+0000be20: 696e 6720 7468 6520 776f 726b 666c 6f77  ing the workflow
+0000be30: 206a 6f62 2061 6e64 0a20 2020 2020 2020   job and.       
+0000be40: 2020 2020 2020 2020 2074 6865 2053 6c75           the Slu
+0000be50: 726d 206a 6f62 2049 442c 206f 7220 2d31  rm job ID, or -1
+0000be60: 2069 6620 7468 6520 6a6f 6220 4944 2063   if the job ID c
+0000be70: 6f75 6c64 206e 6f74 2062 6520 6578 7472  ould not be extr
+0000be80: 6163 7465 642e 0a0a 2020 2020 2020 2020  acted...        
+0000be90: 4e6f 7465 3a0a 2020 2020 2020 2020 2020  Note:.          
+0000bea0: 2020 5468 6520 536c 7572 6d20 6a6f 6220    The Slurm job 
+0000beb0: 4944 2069 7320 6578 7472 6163 7465 6420  ID is extracted 
+0000bec0: 6672 6f6d 2074 6865 2072 6573 756c 7420  from the result 
+0000bed0: 6f66 2074 6865 200a 2020 2020 2020 2020  of the .        
+0000bee0: 2020 2020 6072 756e 5f63 6f6d 6d61 6e64      `run_command
+0000bef0: 7360 206d 6574 686f 642e 0a20 2020 2020  s` method..     
+0000bf00: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
+0000bf10: 6261 7463 685f 636d 642c 2073 6261 7463  batch_cmd, sbatc
+0000bf20: 685f 656e 7620 3d20 7365 6c66 2e67 6574  h_env = self.get
+0000bf30: 5f77 6f72 6b66 6c6f 775f 636f 6d6d 616e  _workflow_comman
+0000bf40: 6428 0a20 2020 2020 2020 2020 2020 2077  d(.            w
+0000bf50: 6f72 6b66 6c6f 775f 6e61 6d65 2c20 776f  orkflow_name, wo
+0000bf60: 726b 666c 6f77 5f76 6572 7369 6f6e 2c20  rkflow_version, 
+0000bf70: 696e 7075 745f 6461 7461 2c20 656d 6169  input_data, emai
+0000bf80: 6c2c 2074 696d 652c 202a 2a6b 7761 7267  l, time, **kwarg
+0000bf90: 7329 0a20 2020 2020 2020 2070 7269 6e74  s).        print
+0000bfa0: 2866 2252 756e 6e69 6e67 207b 776f 726b  (f"Running {work
+0000bfb0: 666c 6f77 5f6e 616d 657d 206a 6f62 206f  flow_name} job o
+0000bfc0: 6e20 7b69 6e70 7574 5f64 6174 617d 206f  n {input_data} o
+0000bfd0: 6e20 536c 7572 6d3a 5c0a 2020 2020 2020  n Slurm:\.      
+0000bfe0: 2020 2020 2020 7b73 6261 7463 685f 636d        {sbatch_cm
+0000bff0: 647d 2077 2f20 7b73 6261 7463 685f 656e  d} w/ {sbatch_en
+0000c000: 767d 2229 0a20 2020 2020 2020 206c 6f67  v}").        log
+0000c010: 6765 722e 696e 666f 2866 2252 756e 6e69  ger.info(f"Runni
+0000c020: 6e67 207b 776f 726b 666c 6f77 5f6e 616d  ng {workflow_nam
+0000c030: 657d 206a 6f62 206f 6e20 7b69 6e70 7574  e} job on {input
+0000c040: 5f64 6174 617d 206f 6e20 536c 7572 6d22  _data} on Slurm"
+0000c050: 290a 2020 2020 2020 2020 7265 7320 3d20  ).        res = 
+0000c060: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
+0000c070: 7328 5b73 6261 7463 685f 636d 645d 2c20  s([sbatch_cmd], 
+0000c080: 7362 6174 6368 5f65 6e76 290a 2020 2020  sbatch_env).    
+0000c090: 2020 2020 7265 7475 726e 2072 6573 2c20      return res, 
+0000c0a0: 7365 6c66 2e65 7874 7261 6374 5f6a 6f62  self.extract_job
+0000c0b0: 5f69 6428 7265 7329 0a0a 2020 2020 6465  _id(res)..    de
+0000c0c0: 6620 7275 6e5f 776f 726b 666c 6f77 5f6a  f run_workflow_j
+0000c0d0: 6f62 2873 656c 662c 0a20 2020 2020 2020  ob(self,.       
+0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0f0: 2020 776f 726b 666c 6f77 5f6e 616d 653a    workflow_name:
+0000c100: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+0000c110: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000c120: 6f72 6b66 6c6f 775f 7665 7273 696f 6e3a  orkflow_version:
+0000c130: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+0000c140: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000c150: 6e70 7574 5f64 6174 613a 2073 7472 2c0a  nput_data: str,.
+0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c170: 2020 2020 2020 2020 2065 6d61 696c 3a20           email: 
+0000c180: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+0000c190: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
+0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000c1b0: 696d 653a 204f 7074 696f 6e61 6c5b 7374  ime: Optional[st
+0000c1c0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1e0: 2020 2020 2a2a 6b77 6172 6773 0a20 2020      **kwargs.   
+0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c200: 2020 2020 2020 2920 2d3e 2053 6c75 726d        ) -> Slurm
+0000c210: 4a6f 623a 0a20 2020 2020 2020 2022 2222  Job:.        """
+0000c220: 0a20 2020 2020 2020 2052 756e 2061 2073  .        Run a s
+0000c230: 7065 6369 6669 6564 2077 6f72 6b66 6c6f  pecified workflo
+0000c240: 7720 6f6e 2053 6c75 726d 2075 7369 6e67  w on Slurm using
+0000c250: 2074 6865 2067 6976 656e 2070 6172 616d   the given param
+0000c260: 6574 6572 7320 616e 6420 7265 7475 726e  eters and return
+0000c270: 2061 2053 6c75 726d 4a6f 6220 696e 7374   a SlurmJob inst
+0000c280: 616e 6365 2e0a 0a20 2020 2020 2020 2041  ance...        A
+0000c290: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000c2a0: 2077 6f72 6b66 6c6f 775f 6e61 6d65 2028   workflow_name (
+0000c2b0: 7374 7229 3a20 4e61 6d65 206f 6620 7468  str): Name of th
+0000c2c0: 6520 776f 726b 666c 6f77 2074 6f20 6578  e workflow to ex
+0000c2d0: 6563 7574 652e 0a20 2020 2020 2020 2020  ecute..         
+0000c2e0: 2020 2077 6f72 6b66 6c6f 775f 7665 7273     workflow_vers
+0000c2f0: 696f 6e20 2873 7472 293a 2056 6572 7369  ion (str): Versi
+0000c300: 6f6e 206f 6620 7468 6520 776f 726b 666c  on of the workfl
+0000c310: 6f77 2028 696d 6167 6520 7665 7273 696f  ow (image versio
+0000c320: 6e20 6f6e 2053 6c75 726d 292e 0a20 2020  n on Slurm)..   
+0000c330: 2020 2020 2020 2020 2069 6e70 7574 5f64           input_d
+0000c340: 6174 6120 2873 7472 293a 204e 616d 6520  ata (str): Name 
+0000c350: 6f66 2074 6865 2069 6e70 7574 2064 6174  of the input dat
+0000c360: 6120 666f 6c64 6572 2063 6f6e 7461 696e  a folder contain
+0000c370: 696e 6720 696e 7075 7420 696d 6167 6520  ing input image 
+0000c380: 6669 6c65 732e 0a20 2020 2020 2020 2020  files..         
+0000c390: 2020 2065 6d61 696c 2028 7374 722c 206f     email (str, o
+0000c3a0: 7074 696f 6e61 6c29 3a20 456d 6169 6c20  ptional): Email 
+0000c3b0: 6164 6472 6573 7320 666f 7220 536c 7572  address for Slur
+0000c3c0: 6d20 6a6f 6220 6e6f 7469 6669 6361 7469  m job notificati
+0000c3d0: 6f6e 732e 0a20 2020 2020 2020 2020 2020  ons..           
+0000c3e0: 2074 696d 6520 2873 7472 2c20 6f70 7469   time (str, opti
+0000c3f0: 6f6e 616c 293a 2054 696d 6520 6c69 6d69  onal): Time limi
+0000c400: 7420 666f 7220 7468 6520 536c 7572 6d20  t for the Slurm 
+0000c410: 6a6f 6220 696e 2074 6865 2066 6f72 6d61  job in the forma
+0000c420: 7420 4848 3a4d 4d3a 5353 2e0a 2020 2020  t HH:MM:SS..    
+0000c430: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+0000c440: 3a20 4164 6469 7469 6f6e 616c 206b 6579  : Additional key
+0000c450: 776f 7264 2061 7267 756d 656e 7473 2066  word arguments f
+0000c460: 6f72 2074 6865 2077 6f72 6b66 6c6f 772e  or the workflow.
+0000c470: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000c480: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
+0000c490: 6c75 726d 4a6f 623a 2041 2053 6c75 726d  lurmJob: A Slurm
+0000c4a0: 4a6f 6220 696e 7374 616e 6365 2072 6570  Job instance rep
+0000c4b0: 7265 7365 6e74 696e 6720 7468 6520 7374  resenting the st
+0000c4c0: 6172 7465 6420 776f 726b 666c 6f77 206a  arted workflow j
+0000c4d0: 6f62 2e0a 2020 2020 2020 2020 2222 220a  ob..        """.
+0000c4e0: 2020 2020 2020 2020 7265 7375 6c74 2c20          result, 
+0000c4f0: 6a6f 625f 6964 203d 2073 656c 662e 7275  job_id = self.ru
+0000c500: 6e5f 776f 726b 666c 6f77 280a 2020 2020  n_workflow(.    
+0000c510: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
+0000c520: 5f6e 616d 652c 2077 6f72 6b66 6c6f 775f  _name, workflow_
+0000c530: 7665 7273 696f 6e2c 2069 6e70 7574 5f64  version, input_d
+0000c540: 6174 612c 2065 6d61 696c 2c20 7469 6d65  ata, email, time
+0000c550: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+0000c560: 2020 2020 7265 7475 726e 2053 6c75 726d      return Slurm
+0000c570: 4a6f 6228 7265 7375 6c74 2c20 6a6f 625f  Job(result, job_
+0000c580: 6964 290a 0a20 2020 2064 6566 2072 756e  id)..    def run
+0000c590: 5f63 6f6e 7665 7273 696f 6e5f 776f 726b  _conversion_work
+0000c5a0: 666c 6f77 5f6a 6f62 2873 656c 662c 2066  flow_job(self, f
+0000c5b0: 6f6c 6465 725f 6e61 6d65 3a20 7374 722c  older_name: str,
+0000c5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5e0: 2020 2020 2073 6f75 7263 655f 666f 726d       source_form
+0000c5f0: 6174 3a20 7374 7220 3d20 277a 6172 7227  at: str = 'zarr'
+0000c600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c620: 2020 2020 2020 7461 7267 6574 5f66 6f72        target_for
+0000c630: 6d61 743a 2073 7472 203d 2027 7469 6666  mat: str = 'tiff
+0000c640: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000c650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c660: 2020 2020 2020 2920 2d3e 2054 7570 6c65        ) -> Tuple
+0000c670: 5b52 6573 756c 742c 2069 6e74 5d3a 0a20  [Result, int]:. 
+0000c680: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000c690: 2020 2052 756e 2074 6865 2064 6174 6120     Run the data 
+0000c6a0: 636f 6e76 6572 7369 6f6e 2077 6f72 6b66  conversion workf
+0000c6b0: 6c6f 7720 6f6e 2053 6c75 726d 2075 7369  low on Slurm usi
+0000c6c0: 6e67 2074 6865 2067 6976 656e 2064 6174  ng the given dat
+0000c6d0: 6120 666f 6c64 6572 2e0a 0a20 2020 2020  a folder...     
+0000c6e0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000c6f0: 2020 2020 2066 6f6c 6465 725f 6e61 6d65       folder_name
+0000c700: 2028 7374 7229 3a20 5468 6520 6e61 6d65   (str): The name
+0000c710: 206f 6620 7468 6520 6461 7461 2066 6f6c   of the data fol
+0000c720: 6465 7220 636f 6e74 6169 6e69 6e67 2073  der containing s
+0000c730: 6f75 7263 6520 666f 726d 6174 2066 696c  ource format fil
+0000c740: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+0000c750: 736f 7572 6365 5f66 6f72 6d61 7420 2873  source_format (s
+0000c760: 7472 293a 2053 6f75 7263 6520 6461 7461  tr): Source data
+0000c770: 2066 6f72 6d61 7420 666f 7220 636f 6e76   format for conv
+0000c780: 6572 7369 6f6e 2028 6465 6661 756c 7420  ersion (default 
+0000c790: 6973 2027 7a61 7272 2729 2e0a 2020 2020  is 'zarr')..    
+0000c7a0: 2020 2020 2020 2020 7461 7267 6574 5f66          target_f
+0000c7b0: 6f72 6d61 7420 2873 7472 293a 2054 6172  ormat (str): Tar
+0000c7c0: 6765 7420 6461 7461 2066 6f72 6d61 7420  get data format 
+0000c7d0: 6166 7465 7220 636f 6e76 6572 7369 6f6e  after conversion
+0000c7e0: 2028 6465 6661 756c 7420 6973 2027 7469   (default is 'ti
+0000c7f0: 6666 2729 2e0a 0a20 2020 2020 2020 2052  ff')...        R
+0000c800: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000c810: 2020 2020 5475 706c 655b 5265 7375 6c74      Tuple[Result
+0000c820: 2c20 696e 745d 3a0a 2020 2020 2020 2020  , int]:.        
+0000c830: 2020 2020 2020 2020 4120 7475 706c 6520          A tuple 
+0000c840: 636f 6e74 6169 6e69 6e67 2074 6865 2072  containing the r
+0000c850: 6573 756c 7420 6f66 2073 7461 7274 696e  esult of startin
+0000c860: 6720 7468 6520 636f 6e76 6572 7369 6f6e  g the conversion
+0000c870: 206a 6f62 2061 6e64 0a20 2020 2020 2020   job and.       
+0000c880: 2020 2020 2020 2020 2074 6865 2053 6c75           the Slu
+0000c890: 726d 206a 6f62 2049 442c 206f 7220 2d31  rm job ID, or -1
+0000c8a0: 2069 6620 7468 6520 6a6f 6220 4944 2063   if the job ID c
+0000c8b0: 6f75 6c64 206e 6f74 2062 6520 6578 7472  ould not be extr
+0000c8c0: 6163 7465 642e 0a0a 2020 2020 2020 2020  acted...        
+0000c8d0: 5761 726e 696e 673a 0a20 2020 2020 2020  Warning:.       
+0000c8e0: 2020 2020 2054 6865 2064 6566 6175 6c74       The default
+0000c8f0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
+0000c900: 6f6e 6c79 2073 7570 706f 7274 7320 636f  only supports co
+0000c910: 6e76 6572 7369 6f6e 2066 726f 6d20 277a  nversion from 'z
+0000c920: 6172 7227 2074 6f20 2774 6966 6627 2e0a  arr' to 'tiff'..
+0000c930: 2020 2020 2020 2020 2020 2020 4966 2075              If u
+0000c940: 7369 6e67 206f 7468 6572 2073 6f75 7263  sing other sourc
+0000c950: 6520 6f72 2074 6172 6765 7420 666f 726d  e or target form
+0000c960: 6174 732c 2075 7365 7273 206d 7573 7420  ats, users must 
+0000c970: 696d 706c 656d 656e 7420 616e 6420 636f  implement and co
+0000c980: 6e66 6967 7572 650a 2020 2020 2020 2020  nfigure.        
+0000c990: 2020 2020 6164 6469 7469 6f6e 616c 2063      additional c
+0000c9a0: 6f6e 7665 7274 6572 7320 7468 656d 7365  onverters themse
+0000c9b0: 6c76 6573 2e0a 2020 2020 2020 2020 2222  lves..        ""
+0000c9c0: 220a 2020 2020 2020 2020 2320 4765 6e65  ".        # Gene
+0000c9d0: 7261 7465 2061 2075 6e69 7175 6520 636f  rate a unique co
+0000c9e0: 6e66 6967 2066 696c 6520 6e61 6d65 0a20  nfig file name. 
+0000c9f0: 2020 2020 2020 2063 6f6e 6669 675f 6669         config_fi
+0000ca00: 6c65 203d 2066 2263 6f6e 6669 675f 7b66  le = f"config_{f
+0000ca10: 6f6c 6465 725f 6e61 6d65 7d2e 7478 7422  older_name}.txt"
+0000ca20: 0a0a 2020 2020 2020 2020 2320 436f 6e73  ..        # Cons
+0000ca30: 7472 7563 7420 616c 6c20 636f 6d6d 616e  truct all comman
+0000ca40: 6473 2074 6f20 7275 6e20 636f 6e73 6563  ds to run consec
+0000ca50: 7574 6976 656c 790a 2020 2020 2020 2020  utively.        
+0000ca60: 6461 7461 5f70 6174 6820 3d20 6622 7b73  data_path = f"{s
+0000ca70: 656c 662e 736c 7572 6d5f 6461 7461 5f70  elf.slurm_data_p
+0000ca80: 6174 687d 2f7b 666f 6c64 6572 5f6e 616d  ath}/{folder_nam
+0000ca90: 657d 220a 2020 2020 2020 2020 636f 6e76  e}".        conv
+0000caa0: 6572 7369 6f6e 5f63 6d64 2c20 7362 6174  ersion_cmd, sbat
+0000cab0: 6368 5f65 6e76 203d 2073 656c 662e 6765  ch_env = self.ge
+0000cac0: 745f 636f 6e76 6572 7369 6f6e 5f63 6f6d  t_conversion_com
+0000cad0: 6d61 6e64 280a 2020 2020 2020 2020 2020  mand(.          
+0000cae0: 2020 6461 7461 5f70 6174 682c 2063 6f6e    data_path, con
+0000caf0: 6669 675f 6669 6c65 2c20 736f 7572 6365  fig_file, source
+0000cb00: 5f66 6f72 6d61 742c 2074 6172 6765 745f  _format, target_
+0000cb10: 666f 726d 6174 290a 2020 2020 2020 2020  format).        
+0000cb20: 636f 6d6d 616e 6473 203d 205b 0a20 2020  commands = [.   
+0000cb30: 2020 2020 2020 2020 2066 2266 696e 6420           f"find 
+0000cb40: 5c22 7b64 6174 615f 7061 7468 7d2f 6461  \"{data_path}/da
+0000cb50: 7461 2f69 6e5c 2220 2d6e 616d 6520 5c22  ta/in\" -name \"
+0000cb60: 2a2e 7b73 6f75 7263 655f 666f 726d 6174  *.{source_format
+0000cb70: 7d5c 2220 7c20 6177 6b20 277b 7b70 7269  }\" | awk '{{pri
+0000cb80: 6e74 204e 522c 2024 307d 7d27 203e 205c  nt NR, $0}}' > \
+0000cb90: 227b 636f 6e66 6967 5f66 696c 657d 5c22  "{config_file}\"
+0000cba0: 222c 0a20 2020 2020 2020 2020 2020 2066  ",.            f
+0000cbb0: 224e 3d24 2877 6320 2d6c 203c 205c 227b  "N=$(wc -l < \"{
+0000cbc0: 636f 6e66 6967 5f66 696c 657d 5c22 2922  config_file}\")"
+0000cbd0: 2c0a 2020 2020 2020 2020 2020 2020 6622  ,.            f"
+0000cbe0: 6563 686f 205c 224e 756d 6265 7220 6f66  echo \"Number of
+0000cbf0: 202e 7b73 6f75 7263 655f 666f 726d 6174   .{source_format
+0000cc00: 7d20 6669 6c65 733a 2024 4e5c 2222 2c0a  } files: $N\"",.
+0000cc10: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
+0000cc20: 6572 7369 6f6e 5f63 6d64 0a20 2020 2020  ersion_cmd.     
+0000cc30: 2020 205d 0a0a 2020 2020 2020 2020 2320     ]..        # 
+0000cc40: 5275 6e20 616c 6c20 636f 6d6d 616e 6473  Run all commands
+0000cc50: 2063 6f6e 7365 6375 7469 7665 6c79 0a20   consecutively. 
+0000cc60: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
+0000cc70: 662e 7275 6e5f 636f 6d6d 616e 6473 2863  f.run_commands(c
+0000cc80: 6f6d 6d61 6e64 732c 2073 6261 7463 685f  ommands, sbatch_
+0000cc90: 656e 7629 0a0a 2020 2020 2020 2020 7265  env)..        re
+0000cca0: 7475 726e 2053 6c75 726d 4a6f 6228 7265  turn SlurmJob(re
+0000ccb0: 732c 2073 656c 662e 6578 7472 6163 745f  s, self.extract_
+0000ccc0: 6a6f 625f 6964 2872 6573 2929 0a0a 2020  job_id(res))..  
+0000ccd0: 2020 6465 6620 6578 7472 6163 745f 6a6f    def extract_jo
+0000cce0: 625f 6964 2873 656c 662c 2072 6573 756c  b_id(self, resul
+0000ccf0: 743a 2052 6573 756c 7429 202d 3e20 696e  t: Result) -> in
+0000cd00: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
+0000cd10: 2020 2020 2020 2045 7874 7261 6374 2074         Extract t
+0000cd20: 6865 2053 6c75 726d 206a 6f62 2049 4420  he Slurm job ID 
+0000cd30: 6672 6f6d 2074 6865 2072 6573 756c 7420  from the result 
+0000cd40: 6f66 2061 2063 6f6d 6d61 6e64 2e0a 0a20  of a command... 
+0000cd50: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000cd60: 2020 2020 2020 2020 2072 6573 756c 7420           result 
+0000cd70: 2852 6573 756c 7429 3a20 5468 6520 7265  (Result): The re
+0000cd80: 7375 6c74 206f 6620 6120 636f 6d6d 616e  sult of a comman
+0000cd90: 6420 6578 6563 7574 696f 6e2e 0a0a 2020  d execution...  
+0000cda0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+0000cdb0: 2020 2020 2020 2020 2020 2069 6e74 3a0a             int:.
+0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cdd0: 5468 6520 536c 7572 6d20 6a6f 6220 4944  The Slurm job ID
+0000cde0: 2065 7874 7261 6374 6564 2066 726f 6d20   extracted from 
+0000cdf0: 7468 6520 7265 7375 6c74 2c0a 2020 2020  the result,.    
+0000ce00: 2020 2020 2020 2020 2020 2020 6f72 202d              or -
+0000ce10: 3120 6966 206e 6f74 2066 6f75 6e64 2e0a  1 if not found..
+0000ce20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000ce30: 2020 2020 736c 7572 6d5f 6a6f 625f 6964      slurm_job_id
+0000ce40: 203d 206e 6578 7428 2869 6e74 2873 2e73   = next((int(s.s
+0000ce50: 7472 6970 2829 2920 666f 7220 7320 696e  trip()) for s in
+0000ce60: 2072 6573 756c 742e 7374 646f 7574 2e73   result.stdout.s
+0000ce70: 706c 6974 280a 2020 2020 2020 2020 2020  plit(.          
+0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce90: 2020 2253 7562 6d69 7474 6564 2062 6174    "Submitted bat
+0000cea0: 6368 206a 6f62 2229 2069 6620 732e 7374  ch job") if s.st
+0000ceb0: 7269 7028 292e 6973 6469 6769 7428 2929  rip().isdigit())
+0000cec0: 2c20 2d31 290a 2020 2020 2020 2020 7265  , -1).        re
+0000ced0: 7475 726e 2073 6c75 726d 5f6a 6f62 5f69  turn slurm_job_i
+0000cee0: 640a 0a20 2020 2064 6566 2067 6574 5f75  d..    def get_u
+0000cef0: 7064 6174 655f 736c 7572 6d5f 7363 7269  pdate_slurm_scri
+0000cf00: 7074 735f 636f 6d6d 616e 6428 7365 6c66  pts_command(self
+0000cf10: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
+0000cf20: 2020 2222 2247 656e 6572 6174 6520 7468    """Generate th
+0000cf30: 6520 636f 6d6d 616e 6420 746f 2075 7064  e command to upd
+0000cf40: 6174 6520 7468 6520 4769 7420 7265 706f  ate the Git repo
+0000cf50: 7369 746f 7279 2063 6f6e 7461 696e 696e  sitory containin
+0000cf60: 670a 2020 2020 2020 2020 7468 6520 536c  g.        the Sl
+0000cf70: 7572 6d20 7363 7269 7074 732c 2069 6620  urm scripts, if 
+0000cf80: 6e65 6365 7373 6172 792e 0a0a 2020 2020  necessary...    
+0000cf90: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0000cfa0: 2020 2020 2020 2020 2073 7472 3a0a 2020           str:.  
+0000cfb0: 2020 2020 2020 2020 2020 2020 2020 4120                A 
+0000cfc0: 7374 7269 6e67 2063 6f6e 7461 696e 696e  string containin
+0000cfd0: 6720 7468 6520 4769 7420 636f 6d6d 616e  g the Git comman
+0000cfe0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+0000cff0: 2020 746f 2075 7064 6174 6520 7468 6520    to update the 
+0000d000: 536c 7572 6d20 7363 7269 7074 732e 0a20  Slurm scripts.. 
+0000d010: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000d020: 2020 2075 7064 6174 655f 636d 6420 3d20     update_cmd = 
+0000d030: 6622 6769 7420 2d43 205c 227b 7365 6c66  f"git -C \"{self
+0000d040: 2e73 6c75 726d 5f73 6372 6970 745f 7061  .slurm_script_pa
+0000d050: 7468 7d5c 2220 7075 6c6c 220a 2020 2020  th}\" pull".    
+0000d060: 2020 2020 7265 7475 726e 2075 7064 6174      return updat
+0000d070: 655f 636d 640a 0a20 2020 2064 6566 2063  e_cmd..    def c
+0000d080: 6865 636b 5f6a 6f62 5f73 7461 7475 7328  heck_job_status(
+0000d090: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000d0b0: 6c75 726d 5f6a 6f62 5f69 6473 3a20 4c69  lurm_job_ids: Li
+0000d0c0: 7374 5b69 6e74 5d2c 0a20 2020 2020 2020  st[int],.       
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2020 656e 763a 204f 7074 696f 6e61 6c5b    env: Optional[
+0000d0f0: 4469 6374 5b73 7472 2c20 7374 725d 5d20  Dict[str, str]] 
+0000d100: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d120: 2920 2d3e 2054 7570 6c65 5b44 6963 745b  ) -> Tuple[Dict[
+0000d130: 696e 742c 2073 7472 5d2c 2052 6573 756c  int, str], Resul
+0000d140: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
+0000d150: 2020 2020 2020 2020 4368 6563 6b20 7468          Check th
+0000d160: 6520 7374 6174 7573 206f 6620 536c 7572  e status of Slur
+0000d170: 6d20 6a6f 6273 2077 6974 6820 7468 6520  m jobs with the 
+0000d180: 6769 7665 6e20 6a6f 6220 4944 732e 0a0a  given job IDs...
+0000d190: 2020 2020 2020 2020 4e6f 7465 3a20 5468          Note: Th
+0000d1a0: 6973 2064 6f65 736e 2774 2072 6574 7572  is doesn't retur
+0000d1b0: 6e20 6a6f 6220 6172 7261 7973 2069 6e64  n job arrays ind
+0000d1c0: 6976 6964 7561 6c6c 792e 0a20 2020 2020  ividually..     
+0000d1d0: 2020 2049 7420 7461 6b65 7320 7468 6520     It takes the 
+0000d1e0: 6c61 7374 2076 616c 7565 2072 6574 7572  last value retur
+0000d1f0: 6e65 6420 666f 7220 7468 6f73 6520 7375  ned for those su
+0000d200: 6220 6964 7320 0a20 2020 2020 2020 2028  b ids .        (
+0000d210: 6765 6e65 7261 6c6c 7920 7468 6520 6f6e  generally the on
+0000d220: 6520 7374 696c 6c20 5045 4e44 494e 4729  e still PENDING)
+0000d230: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+0000d240: 0a20 2020 2020 2020 2020 2020 2073 6c75  .            slu
+0000d250: 726d 5f6a 6f62 5f69 6473 2028 4c69 7374  rm_job_ids (List
+0000d260: 5b69 6e74 5d29 3a20 5468 6520 6a6f 6220  [int]): The job 
+0000d270: 4944 7320 6f66 2074 6865 2053 6c75 726d  IDs of the Slurm
+0000d280: 206a 6f62 7320 746f 2063 6865 636b 2e0a   jobs to check..
+0000d290: 2020 2020 2020 2020 2020 2020 656e 7620              env 
+0000d2a0: 2844 6963 745b 7374 722c 2073 7472 5d2c  (Dict[str, str],
+0000d2b0: 206f 7074 696f 6e61 6c29 3a20 4f70 7469   optional): Opti
+0000d2c0: 6f6e 616c 2065 6e76 6972 6f6e 6d65 6e74  onal environment
+0000d2d0: 2076 6172 6961 626c 6573 2074 6f0a 2020   variables to.  
+0000d2e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000d2f0: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
+0000d300: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
+0000d310: 756c 7473 2074 6f20 4e6f 6e65 2e0a 0a20  ults to None... 
+0000d320: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0000d330: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
+0000d340: 655b 4469 6374 5b69 6e74 2c20 7374 725d  e[Dict[int, str]
+0000d350: 2c20 5265 7375 6c74 5d3a 0a20 2020 2020  , Result]:.     
+0000d360: 2020 2020 2020 2020 2020 2041 2074 7570             A tup
+0000d370: 6c65 2063 6f6e 7461 696e 696e 6720 7468  le containing th
+0000d380: 6520 7374 6174 7573 2070 6572 2069 6e70  e status per inp
+0000d390: 7574 2049 4420 616e 6420 7468 6520 7265  ut ID and the re
+0000d3a0: 7375 6c74 206f 6620 0a20 2020 2020 2020  sult of .       
+0000d3b0: 2020 2020 2020 2020 2074 6865 2063 6f6d           the com
+0000d3c0: 6d61 6e64 2065 7865 6375 7469 6f6e 2e0a  mand execution..
+0000d3d0: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+0000d3e0: 0a20 2020 2020 2020 2020 2020 2053 5348  .            SSH
+0000d3f0: 4578 6365 7074 696f 6e3a 2049 6620 7468  Exception: If th
+0000d400: 6520 636f 6d6d 616e 6420 6578 6563 7574  e command execut
+0000d410: 696f 6e20 6661 696c 7320 6f72 206e 6f20  ion fails or no 
+0000d420: 7265 7370 6f6e 7365 2069 730a 2020 2020  response is.    
+0000d430: 2020 2020 2020 2020 2020 2020 7265 6365              rece
+0000d440: 6976 6564 2061 6674 6572 206d 756c 7469  ived after multi
+0000d450: 706c 6520 7265 7472 6965 732e 0a20 2020  ple retries..   
+0000d460: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000d470: 2063 6d64 203d 2073 656c 662e 6765 745f   cmd = self.get_
+0000d480: 6a6f 625f 7374 6174 7573 5f63 6f6d 6d61  job_status_comma
+0000d490: 6e64 2873 6c75 726d 5f6a 6f62 5f69 6473  nd(slurm_job_ids
+0000d4a0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+0000d4b0: 2e69 6e66 6f28 6622 4765 7474 696e 6720  .info(f"Getting 
+0000d4c0: 7374 6174 7573 206f 6620 7b73 6c75 726d  status of {slurm
+0000d4d0: 5f6a 6f62 5f69 6473 7d20 6f6e 2053 6c75  _job_ids} on Slu
+0000d4e0: 726d 2229 0a20 2020 2020 2020 2072 6574  rm").        ret
+0000d4f0: 7279 5f73 7461 7475 7320 3d20 300a 2020  ry_status = 0.  
+0000d500: 2020 2020 2020 7768 696c 6520 7265 7472        while retr
+0000d510: 795f 7374 6174 7573 203c 2033 3a0a 2020  y_status < 3:.  
+0000d520: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+0000d530: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
+0000d540: 616e 6473 285b 636d 645d 2c20 656e 763d  ands([cmd], env=
+0000d550: 656e 7629 0a20 2020 2020 2020 2020 2020  env).           
+0000d560: 206c 6f67 6765 722e 696e 666f 2872 6573   logger.info(res
+0000d570: 756c 7429 0a20 2020 2020 2020 2020 2020  ult).           
+0000d580: 2069 6620 7265 7375 6c74 2e6f 6b3a 0a20   if result.ok:. 
+0000d590: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d5a0: 6620 6e6f 7420 7265 7375 6c74 2e73 7464  f not result.std
+0000d5b0: 6f75 743a 0a20 2020 2020 2020 2020 2020  out:.           
+0000d5c0: 2020 2020 2020 2020 2023 2077 6169 7420           # wait 
+0000d5d0: 666f 7220 3320 7365 636f 6e64 7320 6265  for 3 seconds be
+0000d5e0: 666f 7265 2063 6865 636b 696e 6720 6167  fore checking ag
+0000d5f0: 6169 6e0a 2020 2020 2020 2020 2020 2020  ain.            
+0000d600: 2020 2020 2020 2020 7469 6d65 736c 6565          timeslee
+0000d610: 702e 736c 6565 7028 3329 0a20 2020 2020  p.sleep(3).     
+0000d620: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000d630: 2072 6574 7279 0a20 2020 2020 2020 2020   retry.         
+0000d640: 2020 2020 2020 2020 2020 2072 6574 7279             retry
+0000d650: 5f73 7461 7475 7320 2b3d 2031 0a20 2020  _status += 1.   
+0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d670: 206c 6f67 6765 722e 6465 6275 6728 0a20   logger.debug(. 
+0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d690: 2020 2020 2020 2066 2252 6574 7279 207b         f"Retry {
+0000d6a0: 7265 7472 795f 7374 6174 7573 7d20 6765  retry_status} ge
+0000d6b0: 7474 696e 6720 7374 6174 7573 205c 0a20  tting status \. 
+0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6d0: 2020 2020 2020 2020 2020 206f 6620 7b73             of {s
+0000d6e0: 6c75 726d 5f6a 6f62 5f69 6473 7d21 2229  lurm_job_ids}!")
+0000d6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d700: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000d710: 2020 2020 2020 2020 2020 2023 0a20 2020             #.   
+0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d730: 206a 6f62 5f73 7461 7475 735f 6469 6374   job_status_dict
+0000d740: 203d 207b 696e 7428 6c69 6e65 2e73 706c   = {int(line.spl
+0000d750: 6974 2829 5b30 5d2e 7370 6c69 7428 275f  it()[0].split('_
+0000d760: 2729 5b30 5d29 3a20 6c69 6e65 2e73 706c  ')[0]): line.spl
+0000d770: 6974 280a 2020 2020 2020 2020 2020 2020  it(.            
+0000d780: 2020 2020 2020 2020 295b 315d 2066 6f72          )[1] for
+0000d790: 206c 696e 6520 696e 2072 6573 756c 742e   line in result.
+0000d7a0: 7374 646f 7574 2e73 706c 6974 2822 5c6e  stdout.split("\n
+0000d7b0: 2229 2069 6620 6c69 6e65 7d0a 2020 2020  ") if line}.    
+0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7d0: 6c6f 6767 6572 2e64 6562 7567 2866 224a  logger.debug(f"J
+0000d7e0: 6f62 2073 7461 7475 7365 733a 207b 6a6f  ob statuses: {jo
+0000d7f0: 625f 7374 6174 7573 5f64 6963 747d 2229  b_status_dict}")
+0000d800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d810: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+0000d820: 2020 2020 2020 2020 2020 2320 4f4b 2c20            # OK, 
+0000d830: 7765 2068 6176 6520 746f 2066 6978 2061  we have to fix a
+0000d840: 2073 7475 7069 6420 7361 6363 7420 6675   stupid sacct fu
+0000d850: 6e63 7469 6f6e 616c 6974 793a 0a20 2020  nctionality:.   
+0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d870: 2023 2050 726f 626c 656d 3a0a 2020 2020   # Problem:.    
+0000d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d890: 2320 5768 656e 2079 6f75 2071 7565 7279  # When you query
+0000d8a0: 2066 6f72 2061 206a 6f62 2d69 642c 2074   for a job-id, t
+0000d8b0: 7572 6e73 206f 7574 2074 6861 7420 6974  urns out that it
+0000d8c0: 2071 7565 7269 6573 0a20 2020 2020 2020   queries.       
+0000d8d0: 2020 2020 2020 2020 2020 2020 2023 2066               # f
+0000d8e0: 6f72 2074 6869 7320 274a 6f62 4964 5261  or this 'JobIdRa
+0000d8f0: 7727 2e20 416e 6420 4a6f 6249 6452 6177  w'. And JobIdRaw
+0000d900: 2066 6f72 2061 7272 6179 7320 6973 2061   for arrays is a
+0000d910: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000d920: 2020 2020 2020 2320 7269 6469 6375 6c6f        # ridiculo
+0000d930: 7573 2073 756d 2c20 652e 672e 2027 4a6f  us sum, e.g. 'Jo
+0000d940: 6249 6427 2031 315f 3220 6765 7473 2061  bId' 11_2 gets a
+0000d950: 7373 6967 6e65 6420 0a20 2020 2020 2020  ssigned .       
+0000d960: 2020 2020 2020 2020 2020 2020 2023 2027               # '
+0000d970: 4a6f 6249 6452 6177 2720 3133 2028 3d20  JobIdRaw' 13 (= 
+0000d980: 3131 2b32 2921 0a20 2020 2020 2020 2020  11+2)!.         
+0000d990: 2020 2020 2020 2020 2020 2023 2055 6e74             # Unt
+0000d9a0: 696c 2079 6f75 2073 7562 6d69 7420 3220  il you submit 2 
+0000d9b0: 6d6f 7265 206a 6f62 7320 616e 6420 6163  more jobs and ac
+0000d9c0: 7475 616c 2027 4a6f 6249 6427 2031 3320  tual 'JobId' 13 
+0000d9d0: 636f 6d65 730a 2020 2020 2020 2020 2020  comes.          
+0000d9e0: 2020 2020 2020 2020 2020 2320 616c 6f6e            # alon
+0000d9f0: 672c 2066 726f 6d20 7468 656e 206f 6e20  g, from then on 
+0000da00: 796f 7520 6765 7420 7468 6174 2073 7461  you get that sta
+0000da10: 7475 7320 7265 7475 726e 6564 2e2e 2e0a  tus returned....
+0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da30: 2020 2020 2320 466f 7220 7573 2c20 7468      # For us, th
+0000da40: 6973 2063 7265 6174 6573 2061 2072 6163  is creates a rac
+0000da50: 6520 636f 6e64 6974 696f 6e2c 2077 6865  e condition, whe
+0000da60: 7265 2077 6520 6765 7420 7468 0a20 2020  re we get th.   
+0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da80: 2023 2065 2077 726f 6e67 2064 6174 6120   # e wrong data 
+0000da90: 6261 636b 2e20 5765 2065 7870 6563 7420  back. We expect 
+0000daa0: 274a 6f62 4964 2720 3133 2c20 6275 7420  'JobId' 13, but 
+0000dab0: 6974 7320 6e6f 7420 0a20 2020 2020 2020  its not .       
+0000dac0: 2020 2020 2020 2020 2020 2020 2023 2074               # t
+0000dad0: 6865 7265 2079 6574 2066 6f72 2073 6f6d  here yet for som
+0000dae0: 6520 7265 6173 6f6e 2c20 736f 2077 6520  e reason, so we 
+0000daf0: 6765 7420 736f 6d65 2072 6573 756c 7420  get some result 
+0000db00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000db10: 2020 2020 2023 2066 726f 6d20 2731 315f       # from '11_
+0000db20: 3227 2062 6163 6b20 696e 7374 6561 642e  2' back instead.
+0000db30: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+0000db40: 2020 2020 2020 2320 416e 6420 7468 6973        # And this
+0000db50: 2063 6175 7365 7320 6120 6b65 795f 6572   causes a key_er
+0000db60: 726f 7220 6c61 7465 7220 6f6e 2c20 6361  ror later on, ca
+0000db70: 7573 6520 7765 2065 7870 6563 740a 2020  use we expect.  
+0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000db90: 2020 2320 2731 3327 2073 696e 6365 2077    # '13' since w
+0000dba0: 6520 7175 6572 6965 6420 666f 7220 7468  e queried for th
+0000dbb0: 6174 206f 6e65 2e0a 2020 2020 2020 2020  at one..        
+0000dbc0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbe0: 2023 2043 7572 7265 6e74 2077 6f72 6b61   # Current worka
+0000dbf0: 726f 756e 643a 2061 7274 6966 6963 6961  round: artificia
+0000dc00: 6c6c 7920 6164 6420 2731 3327 2074 6f20  lly add '13' to 
+0000dc10: 6f75 7220 7265 7375 6c74 732e 0a20 2020  our results..   
+0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc30: 2023 2041 6e64 2072 656d 6f76 6520 7468   # And remove th
+0000dc40: 6520 6661 6b65 206f 6e65 2873 292e 0a20  e fake one(s).. 
+0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dc60: 2020 2072 6573 756c 745f 6469 6374 203d     result_dict =
+0000dc70: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
+0000dc80: 2020 2020 2020 2020 666f 7220 6a6f 625f          for job_
+0000dc90: 6964 2069 6e20 736c 7572 6d5f 6a6f 625f  id in slurm_job_
+0000dca0: 6964 733a 0a20 2020 2020 2020 2020 2020  ids:.           
+0000dcb0: 2020 2020 2020 2020 2020 2020 2023 2043               # C
+0000dcc0: 6865 636b 2069 6620 7468 6520 6a6f 6220  heck if the job 
+0000dcd0: 4944 2069 7320 6e6f 7420 616c 7265 6164  ID is not alread
+0000dce0: 7920 696e 2074 6865 206a 6f62 5f73 7461  y in the job_sta
+0000dcf0: 7475 735f 6469 6374 0a20 2020 2020 2020  tus_dict.       
+0000dd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd10: 2069 6620 6a6f 625f 6964 206e 6f74 2069   if job_id not i
+0000dd20: 6e20 6a6f 625f 7374 6174 7573 5f64 6963  n job_status_dic
+0000dd30: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+0000dd40: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+0000dd50: 6f67 6765 722e 6465 6275 6728 6622 4d69  ogger.debug(f"Mi
+0000dd60: 7373 696e 6720 6a6f 6220 7b6a 6f62 5f69  ssing job {job_i
+0000dd70: 647d 2069 6e20 6f75 7220 5c0a 2020 2020  d} in our \.    
+0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd90: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000dda0: 6c74 7321 2041 6464 696e 6720 6974 2061  lts! Adding it a
+0000ddb0: 7274 6966 6963 6961 6c6c 792e 2229 0a20  rtificially."). 
+0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ddd0: 2020 2020 2020 2020 2020 2023 2041 6464             # Add
+0000dde0: 2074 6865 206a 6f62 2049 4420 7769 7468   the job ID with
+0000ddf0: 2061 2064 6566 6175 6c74 2073 7461 7475   a default statu
+0000de00: 7320 6f66 2027 5045 4e44 494e 4727 0a20  s of 'PENDING'. 
+0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de20: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+0000de30: 745f 6469 6374 5b6a 6f62 5f69 645d 203d  t_dict[job_id] =
+0000de40: 2027 5045 4e44 494e 4727 0a20 2020 2020   'PENDING'.     
+0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000de80: 2020 2020 2023 2043 6f70 7920 7468 6f73       # Copy thos
+0000de90: 6520 7661 6c75 6573 2074 6861 7420 7765  e values that we
+0000dea0: 2077 616e 7420 7468 6520 6b65 7973 2066   want the keys f
+0000deb0: 726f 6d0a 2020 2020 2020 2020 2020 2020  rom.            
+0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ded0: 7265 7375 6c74 5f64 6963 745b 6a6f 625f  result_dict[job_
+0000dee0: 6964 5d20 3d20 6a6f 625f 7374 6174 7573  id] = job_status
+0000def0: 5f64 6963 745b 6a6f 625f 6964 5d0a 2020  _dict[job_id].  
+0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000df10: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
+0000df20: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+0000df30: 7375 6c74 5f64 6963 742c 2072 6573 756c  sult_dict, resul
+0000df40: 740a 2020 2020 2020 2020 2020 2020 656c  t.            el
+0000df50: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000df60: 2020 2020 6572 726f 7220 3d20 6622 5265      error = f"Re
+0000df70: 7375 6c74 2069 7320 6e6f 7420 6f6b 3a20  sult is not ok: 
+0000df80: 7b72 6573 756c 747d 220a 2020 2020 2020  {result}".      
+0000df90: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000dfa0: 2e65 7272 6f72 2865 7272 6f72 290a 2020  .error(error).  
+0000dfb0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000dfc0: 6973 6520 5353 4845 7863 6570 7469 6f6e  ise SSHException
+0000dfd0: 2865 7272 6f72 290a 2020 2020 2020 2020  (error).        
+0000dfe0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000dff0: 2020 6572 726f 7220 3d20 6622 4572 726f    error = f"Erro
+0000e000: 723a 2052 6574 7269 6564 207b 7265 7472  r: Retried {retr
+0000e010: 795f 7374 6174 7573 7d20 7469 6d65 7320  y_status} times 
+0000e020: 746f 2067 6574 205c 0a20 2020 2020 2020  to get \.       
+0000e030: 2020 2020 2020 2020 2073 7461 7475 7320           status 
+0000e040: 6f66 207b 736c 7572 6d5f 6a6f 625f 6964  of {slurm_job_id
+0000e050: 737d 2c20 6275 7420 6e6f 2072 6573 706f  s}, but no respo
+0000e060: 6e73 652e 220a 2020 2020 2020 2020 2020  nse.".          
+0000e070: 2020 6c6f 6767 6572 2e65 7272 6f72 2865    logger.error(e
+0000e080: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
+0000e090: 2020 7261 6973 6520 5353 4845 7863 6570    raise SSHExcep
+0000e0a0: 7469 6f6e 2865 7272 6f72 290a 0a20 2020  tion(error)..   
+0000e0b0: 2064 6566 2067 6574 5f6a 6f62 5f73 7461   def get_job_sta
+0000e0c0: 7475 735f 636f 6d6d 616e 6428 7365 6c66  tus_command(self
+0000e0d0: 2c20 736c 7572 6d5f 6a6f 625f 6964 733a  , slurm_job_ids:
+0000e0e0: 204c 6973 745b 696e 745d 2920 2d3e 2073   List[int]) -> s
+0000e0f0: 7472 3a0a 2020 2020 2020 2020 2222 220a  tr:.        """.
+0000e100: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
+0000e110: 6865 2053 6c75 726d 2063 6f6d 6d61 6e64  he Slurm command
+0000e120: 2074 6f20 6765 7420 7468 6520 7374 6174   to get the stat
+0000e130: 7573 206f 6620 6a6f 6273 2077 6974 6820  us of jobs with 
+0000e140: 7468 6520 6769 7665 6e0a 2020 2020 2020  the given.      
+0000e150: 2020 6a6f 6220 4944 732e 0a0a 2020 2020    job IDs...    
+0000e160: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000e170: 2020 2020 2020 736c 7572 6d5f 6a6f 625f        slurm_job_
+0000e180: 6964 7320 284c 6973 745b 696e 745d 293a  ids (List[int]):
+0000e190: 2054 6865 206a 6f62 2049 4473 206f 6620   The job IDs of 
+0000e1a0: 7468 6520 6a6f 6273 2074 6f20 6368 6563  the jobs to chec
+0000e1b0: 6b2e 0a0a 2020 2020 2020 2020 5265 7475  k...        Retu
+0000e1c0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000e1d0: 2073 7472 3a20 0a20 2020 2020 2020 2020   str: .         
+0000e1e0: 2020 2020 2020 2054 6865 2053 6c75 726d         The Slurm
+0000e1f0: 2063 6f6d 6d61 6e64 2074 6f20 6765 7420   command to get 
+0000e200: 7468 6520 7374 6174 7573 206f 6620 7468  the status of th
+0000e210: 6520 6a6f 6273 2e0a 2020 2020 2020 2020  e jobs..        
+0000e220: 2222 220a 2020 2020 2020 2020 2320 636f  """.        # co
+0000e230: 6e63 6174 206d 756c 7469 706c 6520 6a6f  ncat multiple jo
+0000e240: 6273 2069 6620 6e65 6564 6564 0a20 2020  bs if needed.   
+0000e250: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
+0000e260: 6420 3d20 2220 2d6a 2022 2e6a 6f69 6e28  d = " -j ".join(
+0000e270: 5b73 7472 2869 6429 2066 6f72 2069 6420  [str(id) for id 
+0000e280: 696e 2073 6c75 726d 5f6a 6f62 5f69 6473  in slurm_job_ids
+0000e290: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
+0000e2a0: 6e20 7365 6c66 2e5f 4a4f 425f 5354 4154  n self._JOB_STAT
+0000e2b0: 5553 5f43 4d44 2e66 6f72 6d61 7428 736c  US_CMD.format(sl
+0000e2c0: 7572 6d5f 6a6f 625f 6964 3d73 6c75 726d  urm_job_id=slurm
+0000e2d0: 5f6a 6f62 5f69 6429 0a0a 2020 2020 6465  _job_id)..    de
+0000e2e0: 6620 6578 7472 6163 745f 6461 7461 5f6c  f extract_data_l
+0000e2f0: 6f63 6174 696f 6e5f 6672 6f6d 5f6c 6f67  ocation_from_log
+0000e300: 2873 656c 662c 2073 6c75 726d 5f6a 6f62  (self, slurm_job
+0000e310: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
+0000e320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e340: 2020 2020 2020 2020 6c6f 6766 696c 653a          logfile:
+0000e350: 2073 7472 203d 204e 6f6e 6529 202d 3e20   str = None) -> 
+0000e360: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
+0000e370: 5265 6164 2053 4c55 524d 206a 6f62 206c  Read SLURM job l
+0000e380: 6f67 6669 6c65 2074 6f20 6669 6e64 206c  ogfile to find l
+0000e390: 6f63 6174 696f 6e20 6f66 2074 6865 2064  ocation of the d
+0000e3a0: 6174 612e 0a0a 2020 2020 2020 2020 4f6e  ata...        On
+0000e3b0: 6520 6f66 2074 6865 2070 6172 616d 6574  e of the paramet
+0000e3c0: 6572 7320 6973 2072 6571 7569 7265 642c  ers is required,
+0000e3d0: 2065 6974 6865 7220 6964 206f 7220 6669   either id or fi
+0000e3e0: 6c65 2e0a 0a20 2020 2020 2020 2041 7267  le...        Arg
+0000e3f0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
+0000e400: 6c75 726d 5f6a 6f62 5f69 6420 2873 7472  lurm_job_id (str
+0000e410: 293a 2049 6420 6f66 2074 6865 2073 6c75  ): Id of the slu
+0000e420: 726d 206a 6f62 0a20 2020 2020 2020 2020  rm job.         
+0000e430: 2020 206c 6f67 6669 6c65 2028 7374 7229     logfile (str)
+0000e440: 3a20 5061 7468 2074 6f20 7468 6520 6c6f  : Path to the lo
+0000e450: 6766 696c 650a 0a20 2020 2020 2020 2052  gfile..        R
+0000e460: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000e470: 2020 2020 7374 723a 2044 6174 6120 6c6f      str: Data lo
+0000e480: 6361 7469 6f6e 2061 6363 6f72 6469 6e67  cation according
+0000e490: 2074 6f20 7468 6520 6c6f 670a 0a20 2020   to the log..   
+0000e4a0: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+0000e4b0: 2020 2020 2020 2020 2053 5348 4578 6365           SSHExce
+0000e4c0: 7074 696f 6e3a 2049 6620 7468 6572 6520  ption: If there 
+0000e4d0: 6973 2061 6e20 6973 7375 6520 7769 7468  is an issue with
+0000e4e0: 2074 6865 2063 6f6d 6d61 6e64 2065 7865   the command exe
+0000e4f0: 6375 7469 6f6e 2e0a 2020 2020 2020 2020  cution..        
+0000e500: 2222 220a 2020 2020 2020 2020 6966 206c  """.        if l
+0000e510: 6f67 6669 6c65 2069 7320 4e6f 6e65 2061  ogfile is None a
+0000e520: 6e64 2073 6c75 726d 5f6a 6f62 5f69 6420  nd slurm_job_id 
+0000e530: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000e540: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
+0000e550: 203d 2073 656c 662e 5f4c 4f47 4649 4c45   = self._LOGFILE
+0000e560: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+0000e570: 6669 6c65 203d 206c 6f67 6669 6c65 2e66  file = logfile.f
+0000e580: 6f72 6d61 7428 736c 7572 6d5f 6a6f 625f  ormat(slurm_job_
+0000e590: 6964 3d73 6c75 726d 5f6a 6f62 5f69 6429  id=slurm_job_id)
+0000e5a0: 0a20 2020 2020 2020 2063 6d64 203d 2073  .        cmd = s
+0000e5b0: 656c 662e 5f4c 4f47 4649 4c45 5f44 4154  elf._LOGFILE_DAT
+0000e5c0: 415f 434d 442e 666f 726d 6174 286c 6f67  A_CMD.format(log
+0000e5d0: 5f66 696c 653d 6c6f 6766 696c 6529 0a20  _file=logfile). 
+0000e5e0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+0000e5f0: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
+0000e600: 7328 5b63 6d64 5d29 0a20 2020 2020 2020  s([cmd]).       
+0000e610: 2069 6620 7265 7375 6c74 2e6f 6b3a 0a20   if result.ok:. 
+0000e620: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000e630: 6e20 7265 7375 6c74 2e73 7464 6f75 740a  n result.stdout.
+0000e640: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000e650: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+0000e660: 5353 4845 7863 6570 7469 6f6e 2872 6573  SSHException(res
+0000e670: 756c 7429 0a0a 2020 2020 6465 6620 6765  ult)..    def ge
+0000e680: 745f 776f 726b 666c 6f77 5f70 6172 616d  t_workflow_param
+0000e690: 6574 6572 7328 7365 6c66 2c0a 2020 2020  eters(self,.    
+0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6b0: 2020 2020 2020 2020 2020 2020 776f 726b              work
+0000e6c0: 666c 6f77 3a20 7374 7229 202d 3e20 4469  flow: str) -> Di
+0000e6d0: 6374 5b73 7472 2c20 4469 6374 5b73 7472  ct[str, Dict[str
+0000e6e0: 2c20 416e 795d 5d3a 0a20 2020 2020 2020  , Any]]:.       
+0000e6f0: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
+0000e700: 7269 6576 6520 7468 6520 7061 7261 6d65  rieve the parame
+0000e710: 7465 7273 206f 6620 6120 776f 726b 666c  ters of a workfl
+0000e720: 6f77 2e0a 0a20 2020 2020 2020 2041 7267  ow...        Arg
+0000e730: 733a 0a20 2020 2020 2020 2020 2020 2077  s:.            w
+0000e740: 6f72 6b66 6c6f 7720 2873 7472 293a 2054  orkflow (str): T
+0000e750: 6865 2077 6f72 6b66 6c6f 7720 666f 7220  he workflow for 
+0000e760: 7768 6963 6820 746f 2072 6574 7269 6576  which to retriev
+0000e770: 6520 7468 6520 7061 7261 6d65 7465 7273  e the parameters
+0000e780: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000e790: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000e7a0: 4469 6374 5b73 7472 2c20 4469 6374 5b73  Dict[str, Dict[s
+0000e7b0: 7472 2c20 416e 795d 5d3a 0a20 2020 2020  tr, Any]]:.     
+0000e7c0: 2020 2020 2020 2020 2020 2041 2064 6963             A dic
+0000e7d0: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
+0000e7e0: 6e67 2074 6865 2077 6f72 6b66 6c6f 7720  ng the workflow 
+0000e7f0: 7061 7261 6d65 7465 7273 2e0a 0a20 2020  parameters...   
+0000e800: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
+0000e810: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
+0000e820: 726f 723a 2049 6620 616e 2065 7272 6f72  ror: If an error
+0000e830: 206f 6363 7572 7320 7768 696c 6520 7265   occurs while re
+0000e840: 7472 6965 7669 6e67 2074 6865 2077 6f72  trieving the wor
+0000e850: 6b66 6c6f 770a 2020 2020 2020 2020 2020  kflow.          
+0000e860: 2020 2020 2020 7061 7261 6d65 7465 7273        parameters
+0000e870: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000e880: 2020 2020 2020 6a73 6f6e 5f64 6573 6372        json_descr
+0000e890: 6970 746f 7220 3d20 7365 6c66 2e70 756c  iptor = self.pul
+0000e8a0: 6c5f 6465 7363 7269 7074 6f72 5f66 726f  l_descriptor_fro
+0000e8b0: 6d5f 6769 7468 7562 2877 6f72 6b66 6c6f  m_github(workflo
+0000e8c0: 7729 0a20 2020 2020 2020 2023 2063 6f6e  w).        # con
+0000e8d0: 7665 7274 2074 6f20 6f6d 6572 6f20 7479  vert to omero ty
+0000e8e0: 7065 730a 2020 2020 2020 2020 6c6f 6767  pes.        logg
+0000e8f0: 6572 2e64 6562 7567 286a 736f 6e5f 6465  er.debug(json_de
+0000e900: 7363 7269 7074 6f72 290a 2020 2020 2020  scriptor).      
+0000e910: 2020 776f 726b 666c 6f77 5f64 6963 7420    workflow_dict 
+0000e920: 3d20 7b7d 0a20 2020 2020 2020 2066 6f72  = {}.        for
+0000e930: 2069 6e70 7574 2069 6e20 6a73 6f6e 5f64   input in json_d
+0000e940: 6573 6372 6970 746f 725b 2769 6e70 7574  escriptor['input
+0000e950: 7327 5d3a 0a20 2020 2020 2020 2020 2020  s']:.           
+0000e960: 2023 2066 696c 7465 7220 6379 746f 6d69   # filter cytomi
+0000e970: 6e65 2070 6172 616d 6574 6572 730a 2020  ne parameters.  
+0000e980: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000e990: 2069 6e70 7574 5b27 6964 275d 2e73 7461   input['id'].sta
+0000e9a0: 7274 7377 6974 6828 2763 7974 6f6d 696e  rtswith('cytomin
+0000e9b0: 6527 293a 0a20 2020 2020 2020 2020 2020  e'):.           
+0000e9c0: 2020 2020 2077 6f72 6b66 6c6f 775f 7061       workflow_pa
+0000e9d0: 7261 6d73 203d 207b 7d0a 2020 2020 2020  rams = {}.      
+0000e9e0: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+0000e9f0: 6f77 5f70 6172 616d 735b 276e 616d 6527  ow_params['name'
+0000ea00: 5d20 3d20 696e 7075 745b 2769 6427 5d0a  ] = input['id'].
+0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ea20: 776f 726b 666c 6f77 5f70 6172 616d 735b  workflow_params[
+0000ea30: 2764 6566 6175 6c74 275d 203d 2069 6e70  'default'] = inp
+0000ea40: 7574 5b27 6465 6661 756c 742d 7661 6c75  ut['default-valu
+0000ea50: 6527 5d0a 2020 2020 2020 2020 2020 2020  e'].            
+0000ea60: 2020 2020 776f 726b 666c 6f77 5f70 6172      workflow_par
+0000ea70: 616d 735b 2763 7974 7970 6527 5d20 3d20  ams['cytype'] = 
+0000ea80: 696e 7075 745b 2774 7970 6527 5d0a 2020  input['type'].  
+0000ea90: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+0000eaa0: 726b 666c 6f77 5f70 6172 616d 735b 276f  rkflow_params['o
+0000eab0: 7074 696f 6e61 6c27 5d20 3d20 696e 7075  ptional'] = inpu
+0000eac0: 745b 276f 7074 696f 6e61 6c27 5d0a 2020  t['optional'].  
+0000ead0: 2020 2020 2020 2020 2020 2020 2020 636d                cm
+0000eae0: 645f 666c 6167 203d 2069 6e70 7574 5b27  d_flag = input['
+0000eaf0: 636f 6d6d 616e 642d 6c69 6e65 2d66 6c61  command-line-fla
+0000eb00: 6727 5d0a 2020 2020 2020 2020 2020 2020  g'].            
+0000eb10: 2020 2020 636d 645f 666c 6167 203d 2063      cmd_flag = c
+0000eb20: 6d64 5f66 6c61 672e 7265 706c 6163 6528  md_flag.replace(
+0000eb30: 2240 6964 222c 2069 6e70 7574 5b27 6964  "@id", input['id
+0000eb40: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
+0000eb50: 2020 2020 776f 726b 666c 6f77 5f70 6172      workflow_par
+0000eb60: 616d 735b 2763 6d64 5f66 6c61 6727 5d20  ams['cmd_flag'] 
+0000eb70: 3d20 636d 645f 666c 6167 0a20 2020 2020  = cmd_flag.     
+0000eb80: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
+0000eb90: 6c6f 775f 7061 7261 6d73 5b27 6465 7363  low_params['desc
+0000eba0: 7269 7074 696f 6e27 5d20 3d20 696e 7075  ription'] = inpu
+0000ebb0: 745b 2764 6573 6372 6970 7469 6f6e 275d  t['description']
+0000ebc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ebd0: 2077 6f72 6b66 6c6f 775f 6469 6374 5b69   workflow_dict[i
+0000ebe0: 6e70 7574 5b27 6964 275d 5d20 3d20 776f  nput['id']] = wo
+0000ebf0: 726b 666c 6f77 5f70 6172 616d 730a 2020  rkflow_params.  
+0000ec00: 2020 2020 2020 7265 7475 726e 2077 6f72        return wor
+0000ec10: 6b66 6c6f 775f 6469 6374 0a0a 2020 2020  kflow_dict..    
+0000ec20: 6465 6620 636f 6e76 6572 745f 6379 7479  def convert_cyty
+0000ec30: 7065 5f74 6f5f 6f6d 7479 7065 2873 656c  pe_to_omtype(sel
+0000ec40: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+0000ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec60: 2020 2020 6379 7479 7065 3a20 7374 722c      cytype: str,
+0000ec70: 205f 6465 6661 756c 742c 202a 6172 6773   _default, *args
+0000ec80: 2c20 2a2a 6b77 6172 6773 0a20 2020 2020  , **kwargs.     
+0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eca0: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
+0000ecb0: 2041 6e79 3a0a 2020 2020 2020 2020 2222   Any:.        ""
+0000ecc0: 220a 2020 2020 2020 2020 436f 6e76 6572  ".        Conver
+0000ecd0: 7420 6120 4379 746f 6d69 6e65 2074 7970  t a Cytomine typ
+0000ece0: 6520 746f 2061 6e20 4f4d 4552 4f20 7479  e to an OMERO ty
+0000ecf0: 7065 2061 6e64 2069 6e73 7461 6e74 6961  pe and instantia
+0000ed00: 7465 7320 6974 0a20 2020 2020 2020 2077  tes it.        w
+0000ed10: 6974 6820 6172 6773 2f6b 7761 7267 732e  ith args/kwargs.
+0000ed20: 0a0a 2020 2020 2020 2020 4e6f 7465 2074  ..        Note t
+0000ed30: 6861 7420 4379 746f 6d69 6e65 2068 6173  hat Cytomine has
+0000ed40: 2061 2050 7974 686f 6e20 436c 6965 6e74   a Python Client
+0000ed50: 2c20 616e 6420 736f 6d65 2063 6f6e 7665  , and some conve
+0000ed60: 7273 696f 6e20 6d65 7468 6f64 730a 2020  rsion methods.  
+0000ed70: 2020 2020 2020 746f 2070 7974 686f 6e20        to python 
+0000ed80: 7479 7065 732c 2062 7574 206e 6f74 6869  types, but nothi
+0000ed90: 6e67 2070 6172 7469 6375 6c61 726c 7920  ng particularly 
+0000eda0: 776f 7274 6820 6465 7065 6e64 696e 6720  worth depending 
+0000edb0: 6f6e 2074 6861 740a 2020 2020 2020 2020  on that.        
+0000edc0: 6c69 6272 6172 7920 666f 7220 7965 742e  library for yet.
+0000edd0: 204d 6967 6874 2062 6520 7573 6566 756c   Might be useful
+0000ede0: 2069 6e20 7468 6520 6675 7475 7265 2070   in the future p
+0000edf0: 6572 6861 7073 2e0a 2020 2020 2020 2020  erhaps..        
+0000ee00: 2865 2e67 2e20 6874 7470 733a 2f2f 6769  (e.g. https://gi
+0000ee10: 7468 7562 2e63 6f6d 2f43 7974 6f6d 696e  thub.com/Cytomin
+0000ee20: 652d 554c 6965 6765 2f43 7974 6f6d 696e  e-ULiege/Cytomin
+0000ee30: 652d 7079 7468 6f6e 2d63 6c69 656e 742f  e-python-client/
+0000ee40: 0a20 2020 2020 2020 2062 6c6f 622f 6d61  .        blob/ma
+0000ee50: 7374 6572 2f63 7974 6f6d 696e 652f 6379  ster/cytomine/cy
+0000ee60: 746f 6d69 6e65 5f6a 6f62 2e70 7929 0a0a  tomine_job.py)..
+0000ee70: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000ee80: 2020 2020 2020 2020 2020 6379 7479 7065            cytype
+0000ee90: 2028 7374 7229 3a20 5468 6520 4379 746f   (str): The Cyto
+0000eea0: 6d69 6e65 2074 7970 6520 746f 2063 6f6e  mine type to con
+0000eeb0: 7665 7274 2e0a 2020 2020 2020 2020 2020  vert..          
+0000eec0: 2020 5f64 6566 6175 6c74 3a20 5468 6520    _default: The 
+0000eed0: 6465 6661 756c 7420 7661 6c75 652e 2052  default value. R
+0000eee0: 6571 7569 7265 6420 746f 2064 6973 7469  equired to disti
+0000eef0: 6e67 7569 7368 2062 6574 7765 656e 2066  nguish between f
+0000ef00: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
+0000ef10: 2020 2020 2061 6e64 2069 6e74 2e0a 2020       and int..  
+0000ef20: 2020 2020 2020 2020 2020 2a61 7267 733a            *args:
+0000ef30: 2041 6464 6974 696f 6e61 6c20 706f 7369   Additional posi
+0000ef40: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
+0000ef50: 2e0a 2020 2020 2020 2020 2020 2020 2a2a  ..            **
+0000ef60: 6b77 6172 6773 3a20 4164 6469 7469 6f6e  kwargs: Addition
+0000ef70: 616c 206b 6579 776f 7264 2061 7267 756d  al keyword argum
+0000ef80: 656e 7473 2e0a 0a20 2020 2020 2020 2052  ents...        R
+0000ef90: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000efa0: 2020 2020 416e 793a 0a20 2020 2020 2020      Any:.       
+0000efb0: 2020 2020 2020 2020 2054 6865 2063 6f6e           The con
+0000efc0: 7665 7274 6564 204f 4d45 524f 2074 7970  verted OMERO typ
+0000efd0: 6520 636c 6173 7320 696e 7374 616e 6365  e class instance
+0000efe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eff0: 206f 7220 4e6f 6e65 2069 6620 6572 726f   or None if erro
+0000f000: 7273 206f 6363 7572 6564 2e0a 0a20 2020  rs occured...   
+0000f010: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f020: 2023 2054 4f44 4f20 6d61 6b65 2045 6e75   # TODO make Enu
+0000f030: 6d20 3f0a 2020 2020 2020 2020 6966 2063  m ?.        if c
+0000f040: 7974 7970 6520 3d3d 2027 4e75 6d62 6572  ytype == 'Number
+0000f050: 273a 0a20 2020 2020 2020 2020 2020 2069  ':.            i
+0000f060: 6620 6973 696e 7374 616e 6365 285f 6465  f isinstance(_de
+0000f070: 6661 756c 742c 2066 6c6f 6174 293a 0a20  fault, float):. 
+0000f080: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000f090: 2066 6c6f 6174 2069 6e73 7465 6164 0a20   float instead. 
+0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000f0b0: 6574 7572 6e20 7365 6c66 2e73 7472 5f74  eturn self.str_t
+0000f0c0: 6f5f 636c 6173 7328 226f 6d65 726f 2e73  o_class("omero.s
+0000f0d0: 6372 6970 7473 222c 2022 466c 6f61 7422  cripts", "Float"
+0000f0e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f100: 2020 2020 2020 2020 2020 202a 6172 6773             *args
+0000f110: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
+0000f120: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000f130: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000f140: 7475 726e 2073 656c 662e 7374 725f 746f  turn self.str_to
+0000f150: 5f63 6c61 7373 2822 6f6d 6572 6f2e 7363  _class("omero.sc
+0000f160: 7269 7074 7322 2c20 2249 6e74 222c 0a20  ripts", "Int",. 
+0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f190: 2020 2020 2020 2020 2a61 7267 732c 202a          *args, *
+0000f1a0: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
+0000f1b0: 2065 6c69 6620 6379 7479 7065 203d 3d20   elif cytype == 
+0000f1c0: 2742 6f6f 6c65 616e 273a 0a20 2020 2020  'Boolean':.     
+0000f1d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000f1e0: 6c66 2e73 7472 5f74 6f5f 636c 6173 7328  lf.str_to_class(
+0000f1f0: 226f 6d65 726f 2e73 6372 6970 7473 222c  "omero.scripts",
+0000f200: 2022 426f 6f6c 222c 0a20 2020 2020 2020   "Bool",.       
+0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f220: 2020 2020 2020 2020 2020 2020 2020 2a61                *a
+0000f230: 7267 732c 202a 2a6b 7761 7267 7329 0a20  rgs, **kwargs). 
+0000f240: 2020 2020 2020 2065 6c69 6620 6379 7479         elif cyty
+0000f250: 7065 203d 3d20 2753 7472 696e 6727 3a0a  pe == 'String':.
+0000f260: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000f270: 726e 2073 656c 662e 7374 725f 746f 5f63  rn self.str_to_c
+0000f280: 6c61 7373 2822 6f6d 6572 6f2e 7363 7269  lass("omero.scri
+0000f290: 7074 7322 2c20 2253 7472 696e 6722 2c0a  pts", "String",.
+0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f2c0: 2020 2020 202a 6172 6773 2c20 2a2a 6b77       *args, **kw
+0000f2d0: 6172 6773 290a 0a20 2020 2064 6566 2065  args)..    def e
+0000f2e0: 7874 7261 6374 5f70 6172 7473 5f66 726f  xtract_parts_fro
+0000f2f0: 6d5f 7572 6c28 7365 6c66 2c20 696e 7075  m_url(self, inpu
+0000f300: 745f 7572 6c3a 2073 7472 2920 2d3e 2054  t_url: str) -> T
+0000f310: 7570 6c65 5b4c 6973 745b 7374 725d 2c20  uple[List[str], 
+0000f320: 7374 725d 3a0a 2020 2020 2020 2020 2222  str]:.        ""
+0000f330: 220a 2020 2020 2020 2020 4578 7472 6163  ".        Extrac
+0000f340: 7420 7468 6520 7265 706f 7369 746f 7279  t the repository
+0000f350: 2061 6e64 2062 7261 6e63 6820 696e 666f   and branch info
+0000f360: 726d 6174 696f 6e20 6672 6f6d 2074 6865  rmation from the
+0000f370: 2069 6e70 7574 2055 524c 2e0a 0a20 2020   input URL...   
+0000f380: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+0000f390: 2020 2020 2020 2069 6e70 7574 5f75 726c         input_url
+0000f3a0: 2028 7374 7229 3a20 5468 6520 696e 7075   (str): The inpu
+0000f3b0: 7420 4769 7448 7562 2055 524c 2e0a 0a20  t GitHub URL... 
+0000f3c0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0000f3d0: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
+0000f3e0: 655b 4c69 7374 5b73 7472 5d2c 2073 7472  e[List[str], str
+0000f3f0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
+0000f400: 2020 2054 6865 206c 6973 7420 6f66 2075     The list of u
+0000f410: 726c 2070 6172 7473 2061 6e64 2074 6865  rl parts and the
+0000f420: 2062 7261 6e63 682f 7665 7273 696f 6e2e   branch/version.
+0000f430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f440: 2049 6620 6e6f 2062 7261 6e63 6820 6973   If no branch is
+0000f450: 2066 6f75 6e64 2c20 6974 2077 696c 6c20   found, it will 
+0000f460: 7265 7475 726e 2022 6d61 7374 6572 220a  return "master".
+0000f470: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+0000f480: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
+0000f490: 7565 4572 726f 723a 2049 6620 7468 6520  ueError: If the 
+0000f4a0: 696e 7075 7420 5552 4c20 6973 206e 6f74  input URL is not
+0000f4b0: 2061 2076 616c 6964 2047 6974 4875 6220   a valid GitHub 
+0000f4c0: 5552 4c2e 0a20 2020 2020 2020 2022 2222  URL..        """
+0000f4d0: 0a20 2020 2020 2020 2075 726c 5f70 6172  .        url_par
+0000f4e0: 7473 203d 2069 6e70 7574 5f75 726c 2e73  ts = input_url.s
+0000f4f0: 706c 6974 2822 2f22 290a 2020 2020 2020  plit("/").      
+0000f500: 2020 6966 206c 656e 2875 726c 5f70 6172    if len(url_par
+0000f510: 7473 2920 3c20 3520 6f72 2075 726c 5f70  ts) < 5 or url_p
+0000f520: 6172 7473 5b32 5d20 213d 2022 6769 7468  arts[2] != "gith
+0000f530: 7562 2e63 6f6d 223a 0a20 2020 2020 2020  ub.com":.       
+0000f540: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+0000f550: 4572 726f 7228 2249 6e76 616c 6964 2047  Error("Invalid G
+0000f560: 6974 4875 6220 5552 4c22 290a 0a20 2020  itHub URL")..   
+0000f570: 2020 2020 2069 6620 2274 7265 6522 2069       if "tree" i
+0000f580: 6e20 7572 6c5f 7061 7274 733a 0a20 2020  n url_parts:.   
+0000f590: 2020 2020 2020 2020 2023 2043 6173 653a           # Case:
+0000f5a0: 2055 524c 2063 6f6e 7461 696e 7320 6120   URL contains a 
+0000f5b0: 6272 616e 6368 0a20 2020 2020 2020 2020  branch.         
+0000f5c0: 2020 2062 7261 6e63 685f 696e 6465 7820     branch_index 
+0000f5d0: 3d20 7572 6c5f 7061 7274 732e 696e 6465  = url_parts.inde
+0000f5e0: 7828 2274 7265 6522 2920 2b20 310a 2020  x("tree") + 1.  
+0000f5f0: 2020 2020 2020 2020 2020 6272 616e 6368            branch
+0000f600: 203d 2075 726c 5f70 6172 7473 5b62 7261   = url_parts[bra
+0000f610: 6e63 685f 696e 6465 785d 0a20 2020 2020  nch_index].     
+0000f620: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000f630: 2020 2020 2023 2043 6173 653a 2055 524c       # Case: URL
+0000f640: 2064 6f65 7320 6e6f 7420 7370 6563 6966   does not specif
+0000f650: 7920 6120 6272 616e 6368 0a20 2020 2020  y a branch.     
+0000f660: 2020 2020 2020 2062 7261 6e63 6820 3d20         branch = 
+0000f670: 226d 6173 7465 7222 0a0a 2020 2020 2020  "master"..      
+0000f680: 2020 7265 7475 726e 2075 726c 5f70 6172    return url_par
+0000f690: 7473 2c20 6272 616e 6368 0a0a 2020 2020  ts, branch..    
+0000f6a0: 6465 6620 636f 6e76 6572 745f 7572 6c28  def convert_url(
+0000f6b0: 7365 6c66 2c20 696e 7075 745f 7572 6c3a  self, input_url:
+0000f6c0: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
+0000f6d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000f6e0: 2020 436f 6e76 6572 7420 7468 6520 696e    Convert the in
+0000f6f0: 7075 7420 4769 7448 7562 2055 524c 2074  put GitHub URL t
+0000f700: 6f20 616e 206f 7574 7075 7420 5552 4c20  o an output URL 
+0000f710: 7468 6174 2072 6574 7269 6576 6573 0a20  that retrieves. 
+0000f720: 2020 2020 2020 2074 6865 2027 6465 7363         the 'desc
+0000f730: 7269 7074 6f72 2e6a 736f 6e27 2066 696c  riptor.json' fil
+0000f740: 6520 696e 2072 6177 2066 6f72 6d61 742e  e in raw format.
+0000f750: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0000f760: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+0000f770: 745f 7572 6c20 2873 7472 293a 2054 6865  t_url (str): The
+0000f780: 2069 6e70 7574 2047 6974 4875 6220 5552   input GitHub UR
+0000f790: 4c2e 0a0a 2020 2020 2020 2020 5265 7475  L...        Retu
+0000f7a0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+0000f7b0: 2073 7472 3a20 5468 6520 6f75 7470 7574   str: The output
+0000f7c0: 2055 524c 2074 6f20 7468 6520 2764 6573   URL to the 'des
+0000f7d0: 6372 6970 746f 722e 6a73 6f6e 2720 6669  criptor.json' fi
+0000f7e0: 6c65 2e0a 0a20 2020 2020 2020 2052 6169  le...        Rai
+0000f7f0: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+0000f800: 2056 616c 7565 4572 726f 723a 2049 6620   ValueError: If 
+0000f810: 7468 6520 696e 7075 7420 5552 4c20 6973  the input URL is
+0000f820: 206e 6f74 2061 2076 616c 6964 2047 6974   not a valid Git
+0000f830: 4875 6220 5552 4c2e 0a20 2020 2020 2020  Hub URL..       
+0000f840: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
+0000f850: 5f70 6172 7473 2c20 6272 616e 6368 203d  _parts, branch =
+0000f860: 2073 656c 662e 6578 7472 6163 745f 7061   self.extract_pa
+0000f870: 7274 735f 6672 6f6d 5f75 726c 2869 6e70  rts_from_url(inp
+0000f880: 7574 5f75 726c 290a 0a20 2020 2020 2020  ut_url)..       
+0000f890: 2023 2043 6f6e 7374 7275 6374 2074 6865   # Construct the
+0000f8a0: 206f 7574 7075 7420 5552 4c20 6279 2063   output URL by c
+0000f8b0: 6f6d 6269 6e69 6e67 2074 6865 2065 7874  ombining the ext
+0000f8c0: 7261 6374 6564 2069 6e66 6f72 6d61 7469  racted informati
+0000f8d0: 6f6e 0a20 2020 2020 2020 2023 2077 6974  on.        # wit
+0000f8e0: 6820 7468 6520 6465 7369 7265 6420 6669  h the desired fi
+0000f8f0: 6c65 2070 6174 680a 2020 2020 2020 2020  le path.        
+0000f900: 6f75 7470 7574 5f75 726c 203d 2066 2268  output_url = f"h
+0000f910: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+0000f920: 6d2f 7b75 726c 5f70 6172 7473 5b33 5d7d  m/{url_parts[3]}
+0000f930: 2f7b 7572 6c5f 7061 7274 735b 345d 7d2f  /{url_parts[4]}/
+0000f940: 7261 772f 7b62 7261 6e63 687d 2f64 6573  raw/{branch}/des
+0000f950: 6372 6970 746f 722e 6a73 6f6e 220a 0a20  criptor.json".. 
+0000f960: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
+0000f970: 7470 7574 5f75 726c 0a0a 2020 2020 6465  tput_url..    de
+0000f980: 6620 7075 6c6c 5f64 6573 6372 6970 746f  f pull_descripto
+0000f990: 725f 6672 6f6d 5f67 6974 6875 6228 7365  r_from_github(se
+0000f9a0: 6c66 2c20 776f 726b 666c 6f77 3a20 7374  lf, workflow: st
+0000f9b0: 7229 202d 3e20 4469 6374 3a0a 2020 2020  r) -> Dict:.    
+0000f9c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000f9d0: 5075 6c6c 2074 6865 2077 6f72 6b66 6c6f  Pull the workflo
+0000f9e0: 7720 6465 7363 7269 7074 6f72 2066 726f  w descriptor fro
+0000f9f0: 6d20 4769 7448 7562 2e0a 0a20 2020 2020  m GitHub...     
+0000fa00: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000fa10: 2020 2020 2077 6f72 6b66 6c6f 7720 2873       workflow (s
+0000fa20: 7472 293a 2054 6865 2077 6f72 6b66 6c6f  tr): The workflo
+0000fa30: 7720 666f 7220 7768 6963 6820 746f 2070  w for which to p
+0000fa40: 756c 6c20 7468 6520 6465 7363 7269 7074  ull the descript
+0000fa50: 6f72 2e0a 0a20 2020 2020 2020 2052 6574  or...        Ret
+0000fa60: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+0000fa70: 2020 4469 6374 3a20 5468 6520 4a53 4f4e    Dict: The JSON
+0000fa80: 2064 6573 6372 6970 746f 722e 0a0a 2020   descriptor...  
+0000fa90: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
+0000faa0: 2020 2020 2020 2020 2020 5661 6c75 6545            ValueE
+0000fab0: 7272 6f72 3a20 4966 2061 6e20 6572 726f  rror: If an erro
+0000fac0: 7220 6f63 6375 7273 2077 6869 6c65 2070  r occurs while p
+0000fad0: 756c 6c69 6e67 2074 6865 2064 6573 6372  ulling the descr
+0000fae0: 6970 746f 7220 6669 6c65 2e0a 2020 2020  iptor file..    
+0000faf0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000fb00: 6769 745f 7265 706f 203d 2073 656c 662e  git_repo = self.
+0000fb10: 736c 7572 6d5f 6d6f 6465 6c5f 7265 706f  slurm_model_repo
+0000fb20: 735b 776f 726b 666c 6f77 5d0a 2020 2020  s[workflow].    
+0000fb30: 2020 2020 2320 636f 6e76 6572 7420 6769      # convert gi
+0000fb40: 7420 7265 706f 2074 6f20 6a73 6f6e 2066  t repo to json f
+0000fb50: 696c 650a 2020 2020 2020 2020 7261 775f  ile.        raw_
+0000fb60: 7572 6c20 3d20 7365 6c66 2e63 6f6e 7665  url = self.conve
+0000fb70: 7274 5f75 726c 2867 6974 5f72 6570 6f29  rt_url(git_repo)
+0000fb80: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+0000fb90: 6465 6275 6728 6622 5075 6c6c 2077 6f72  debug(f"Pull wor
+0000fba0: 6b66 6c6f 773a 207b 776f 726b 666c 6f77  kflow: {workflow
+0000fbb0: 7d3a 207b 6769 745f 7265 706f 7d20 3e3e  }: {git_repo} >>
+0000fbc0: 207b 7261 775f 7572 6c7d 2229 0a20 2020   {raw_url}").   
+0000fbd0: 2020 2020 2023 2070 756c 6c20 776f 726b       # pull work
+0000fbe0: 666c 6f77 2070 6172 616d 730a 2020 2020  flow params.    
+0000fbf0: 2020 2020 6769 7468 7562 5f73 6573 7369      github_sessi
+0000fc00: 6f6e 203d 2073 656c 662e 6765 745f 6f72  on = self.get_or
+0000fc10: 5f63 7265 6174 655f 6769 7468 7562 5f73  _create_github_s
+0000fc20: 6573 7369 6f6e 2829 0a20 2020 2020 2020  ession().       
+0000fc30: 2067 6866 696c 6520 3d20 6769 7468 7562   ghfile = github
+0000fc40: 5f73 6573 7369 6f6e 2e67 6574 2872 6177  _session.get(raw
+0000fc50: 5f75 726c 290a 2020 2020 2020 2020 6966  _url).        if
+0000fc60: 2067 6866 696c 652e 6f6b 3a0a 2020 2020   ghfile.ok:.    
+0000fc70: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000fc80: 6562 7567 2866 2243 6163 6865 643f 207b  ebug(f"Cached? {
+0000fc90: 6768 6669 6c65 2e66 726f 6d5f 6361 6368  ghfile.from_cach
+0000fca0: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
+0000fcb0: 206a 736f 6e5f 6465 7363 7269 7074 6f72   json_descriptor
+0000fcc0: 203d 2067 6866 696c 652e 6a73 6f6e 2829   = ghfile.json()
+0000fcd0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+0000fce0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000fcf0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+0000fd00: 2020 2020 2020 2020 2020 2020 2066 2745               f'E
+0000fd10: 7272 6f72 2077 6869 6c65 2070 756c 6c69  rror while pulli
+0000fd20: 6e67 2064 6573 6372 6970 746f 7220 6669  ng descriptor fi
+0000fd30: 6c65 2066 6f72 2077 6f72 6b66 6c6f 7720  le for workflow 
+0000fd40: 7b77 6f72 6b66 6c6f 777d 2c5c 0a20 2020  {workflow},\.   
+0000fd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd60: 2066 726f 6d20 7b72 6177 5f75 726c 7d3a   from {raw_url}:
+0000fd70: 207b 6768 6669 6c65 2e5f 5f64 6963 745f   {ghfile.__dict_
+0000fd80: 5f7d 2729 0a20 2020 2020 2020 2072 6574  _}').        ret
+0000fd90: 7572 6e20 6a73 6f6e 5f64 6573 6372 6970  urn json_descrip
+0000fda0: 746f 720a 0a20 2020 2064 6566 2067 6574  tor..    def get
+0000fdb0: 5f6f 725f 6372 6561 7465 5f67 6974 6875  _or_create_githu
+0000fdc0: 625f 7365 7373 696f 6e28 7365 6c66 293a  b_session(self):
+0000fdd0: 0a20 2020 2020 2020 2023 204e 6f74 652c  .        # Note,
+0000fde0: 2075 7369 6e67 2072 6571 7565 7374 735f   using requests_
+0000fdf0: 6361 6368 6520 312e 312e 312c 2063 6f6e  cache 1.1.1, con
+0000fe00: 6469 7469 6f6e 616c 2071 7565 7269 6573  ditional queries
+0000fe10: 2061 7265 2064 6566 6175 6c74 3a0a 2020   are default:.  
+0000fe20: 2020 2020 2020 2320 5468 6520 6361 6368        # The cach
+0000fe30: 6564 2072 6573 706f 6e73 6520 7769 6c6c  ed response will
+0000fe40: 2073 7469 6c6c 2062 6520 7573 6564 2075   still be used u
+0000fe50: 6e74 696c 2074 6865 2072 656d 6f74 6520  ntil the remote 
+0000fe60: 636f 6e74 656e 7420 6163 7475 616c 6c79  content actually
+0000fe70: 2063 6861 6e67 6573 0a20 2020 2020 2020   changes.       
+0000fe80: 2023 2045 7665 6e20 6966 2074 6865 2027   # Even if the '
+0000fe90: 6578 7069 7265 5f61 6674 6572 2720 6973  expire_after' is
+0000fea0: 2074 7269 6767 6572 6564 2e20 5468 6973   triggered. This
+0000feb0: 2069 7320 6275 696c 7420 696e 746f 2047   is built into G
+0000fec0: 6974 4875 622c 2077 6869 6368 2072 6574  itHub, which ret
+0000fed0: 7572 6e73 0a20 2020 2020 2020 2023 2061  urns.        # a
+0000fee0: 2045 7461 6720 696e 2074 6865 2068 6561   Etag in the hea
+0000fef0: 6465 7220 7468 6174 206f 6e6c 7920 6368  der that only ch
+0000ff00: 616e 6765 7320 7768 656e 2074 6865 2063  anges when the c
+0000ff10: 6f6e 7465 6e74 2028 652e 672e 2074 6865  ontent (e.g. the
+0000ff20: 2064 6573 6372 6970 746f 7229 2063 6861   descriptor) cha
+0000ff30: 6e67 6573 2e0a 2020 2020 2020 2020 2320  nges..        # 
+0000ff40: 4966 2079 6f75 2070 726f 7669 6465 2074  If you provide t
+0000ff50: 6869 7320 4574 6167 2077 6865 6e20 7175  his Etag when qu
+0000ff60: 6572 7969 6e67 2c20 796f 7520 7769 6c6c  erying, you will
+0000ff70: 2067 6574 2061 2033 3034 2028 276e 6f20   get a 304 ('no 
+0000ff80: 6368 616e 6765 2729 2061 6e64 2069 7420  change') and it 
+0000ff90: 7769 6c6c 0a20 2020 2020 2020 2023 204e  will.        # N
+0000ffa0: 4f54 2063 6f75 6e74 2074 6f77 6172 6473  OT count towards
+0000ffb0: 2079 6f75 7220 4769 7468 7562 206c 696d   your Github lim
+0000ffc0: 6974 732e 2041 6e64 2072 6571 7565 7374  its. And request
+0000ffd0: 735f 6361 6368 6520 646f 6573 2074 6861  s_cache does tha
+0000ffe0: 7420 666f 7220 7573 206e 6f77 2e0a 2020  t for us now..  
+0000fff0: 2020 2020 2020 2320 4e6f 7420 6176 6169        # Not avai
+00010000: 6c61 626c 6520 696e 2050 7974 686f 6e33  lable in Python3
+00010010: 2e36 2074 686f 7567 682e 0a20 2020 2020  .6 though..     
+00010020: 2020 2073 203d 2072 6571 7565 7374 735f     s = requests_
+00010030: 6361 6368 652e 4361 6368 6564 5365 7373  cache.CachedSess
+00010040: 696f 6e28 2767 6974 6875 625f 6361 6368  ion('github_cach
+00010050: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010070: 2020 2020 2020 2020 2020 2020 2062 6163               bac
+00010080: 6b65 6e64 3d73 656c 662e 6361 6368 652c  kend=self.cache,
+00010090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100b0: 2020 2020 2020 2020 2020 6578 7069 7265            expire
+000100c0: 5f61 6674 6572 3d31 2c0a 2020 2020 2020  _after=1,.      
+000100d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000100f0: 2020 2063 6163 6865 5f63 6f6e 7472 6f6c     cache_control
+00010100: 3d54 7275 650a 2020 2020 2020 2020 2020  =True.          
+00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010120: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010130: 0a20 2020 2020 2020 2023 204d 6967 6874  .        # Might
+00010140: 2068 6176 6520 6269 6767 6572 2069 7373   have bigger iss
+00010150: 7565 732c 2074 6869 7320 6973 2072 656c  ues, this is rel
+00010160: 6174 6564 2074 6f20 7261 7465 206c 696d  ated to rate lim
+00010170: 6974 7320 6f6e 2047 6974 4875 620a 2020  its on GitHub.  
+00010180: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
+00010190: 646f 6373 2e67 6974 6875 622e 636f 6d2f  docs.github.com/
+000101a0: 656e 2f72 6573 742f 7573 696e 672d 7468  en/rest/using-th
+000101b0: 652d 7265 7374 2d61 7069 2f72 6174 652d  e-rest-api/rate-
+000101c0: 6c69 6d69 7473 2d66 6f72 2d74 6865 2d72  limits-for-the-r
+000101d0: 6573 742d 6170 690a 2020 2020 2020 2020  est-api.        
+000101e0: 2320 4966 2069 7420 7374 6179 7320 6120  # If it stays a 
+000101f0: 7072 6f62 6c65 6d2c 2077 6520 6861 7665  problem, we have
+00010200: 2074 6f20 6164 6420 616e 206f 7074 696f   to add an optio
+00010210: 6e20 746f 2061 6464 2061 2047 4820 6b65  n to add a GH ke
+00010220: 7920 746f 2074 6865 2063 6f6e 6669 670a  y to the config.
+00010230: 2020 2020 2020 2020 2320 452e 672e 2073          # E.g. s
+00010240: 6565 2068 7474 7073 3a2f 2f67 6974 6875  ee https://githu
+00010250: 622e 636f 6d2f 7265 7175 6573 7473 2d63  b.com/requests-c
+00010260: 6163 6865 2f72 6571 7565 7374 732d 6361  ache/requests-ca
+00010270: 6368 652f 626c 6f62 2f35 3331 3334 6566  che/blob/53134ef
+00010280: 3065 3939 6437 3133 6665 6436 3235 3135  0e99d713fed62515
+00010290: 6466 6237 6263 6661 6163 3566 3633 6639  dfb7bcfaac5f63f9
+000102a0: 642f 6578 616d 706c 6573 2f70 7967 6974  d/examples/pygit
+000102b0: 6875 622e 7079 0a20 2020 2020 2020 2023  hub.py.        #
+000102c0: 2048 6572 6520 796f 7520 636f 756c 6420   Here you could 
+000102d0: 6861 7665 2061 6e20 4143 4345 5353 5f54  have an ACCESS_T
+000102e0: 4f4b 454e 2e0a 2020 2020 2020 2020 2320  OKEN..        # 
+000102f0: 416e 2041 4343 4553 535f 544f 4b45 4e20  An ACCESS_TOKEN 
+00010300: 636f 756c 6420 696d 7072 6f76 6520 6170  could improve ap
+00010310: 6920 6c69 6d69 7473 2074 6f20 3530 3030  i limits to 5000
+00010320: 2f68 2028 6672 6f6d 2036 302f 6829 2e0a  /h (from 60/h)..
+00010330: 2020 2020 2020 2020 7265 7472 795f 7374          retry_st
+00010340: 7261 7465 6779 203d 2052 6574 7279 280a  rategy = Retry(.
+00010350: 2020 2020 2020 2020 2020 2020 746f 7461              tota
+00010360: 6c3d 352c 2020 2020 2020 2020 2020 2020  l=5,            
+00010370: 2020 2023 204d 6178 696d 756d 206e 756d     # Maximum num
+00010380: 6265 7220 6f66 2072 6574 7269 6573 0a20  ber of retries. 
+00010390: 2020 2020 2020 2020 2020 2023 2045 7870             # Exp
+000103a0: 6f6e 656e 7469 616c 2062 6163 6b6f 6666  onential backoff
+000103b0: 2066 6163 746f 7220 2864 656c 6179 2062   factor (delay b
+000103c0: 6574 7765 656e 2072 6574 7269 6573 290a  etween retries).
+000103d0: 2020 2020 2020 2020 2020 2020 6261 636b              back
+000103e0: 6f66 665f 6661 6374 6f72 3d35 2c0a 2020  off_factor=5,.  
+000103f0: 2020 2020 2020 2020 2020 2320 5265 7472            # Retr
+00010400: 7920 6f6e 2074 6865 7365 2048 5454 5020  y on these HTTP 
+00010410: 7374 6174 7573 2063 6f64 6573 0a20 2020  status codes.   
+00010420: 2020 2020 2020 2020 2073 7461 7475 735f           status_
+00010430: 666f 7263 656c 6973 743d 5b35 3030 2c20  forcelist=[500, 
+00010440: 3530 322c 2035 3033 2c20 3530 342c 2034  502, 503, 504, 4
+00010450: 3033 2c20 3432 395d 2c0a 2020 2020 2020  03, 429],.      
+00010460: 2020 2020 2020 616c 6c6f 7765 645f 6d65        allowed_me
+00010470: 7468 6f64 733d 6672 6f7a 656e 7365 7428  thods=frozenset(
+00010480: 5b27 4745 5427 5d29 2020 2320 4f6e 6c79  ['GET'])  # Only
+00010490: 2072 6574 7279 2066 6f72 2047 4554 2072   retry for GET r
+000104a0: 6571 7565 7374 730a 2020 2020 2020 2020  equests.        
+000104b0: 290a 2020 2020 2020 2020 732e 6d6f 756e  ).        s.moun
+000104c0: 7428 2768 7474 7073 3a2f 2f67 6974 6875  t('https://githu
+000104d0: 622e 636f 6d2f 272c 2048 5454 5041 6461  b.com/', HTTPAda
+000104e0: 7074 6572 286d 6178 5f72 6574 7269 6573  pter(max_retries
+000104f0: 3d72 6574 7279 5f73 7472 6174 6567 7929  =retry_strategy)
+00010500: 290a 2020 2020 2020 2020 732e 6d6f 756e  ).        s.moun
+00010510: 7428 2768 7474 703a 2f2f 6769 7468 7562  t('http://github
+00010520: 2e63 6f6d 2f27 2c20 4854 5450 4164 6170  .com/', HTTPAdap
+00010530: 7465 7228 6d61 785f 7265 7472 6965 733d  ter(max_retries=
+00010540: 7265 7472 795f 7374 7261 7465 6779 2929  retry_strategy))
+00010550: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010560: 730a 0a20 2020 2064 6566 2067 6574 5f77  s..    def get_w
+00010570: 6f72 6b66 6c6f 775f 636f 6d6d 616e 6428  orkflow_command(
+00010580: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105a0: 2020 2077 6f72 6b66 6c6f 773a 2073 7472     workflow: str
+000105b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000105c0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+000105d0: 6f72 6b66 6c6f 775f 7665 7273 696f 6e3a  orkflow_version:
+000105e0: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010600: 2020 2069 6e70 7574 5f64 6174 613a 2073     input_data: s
+00010610: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010630: 2065 6d61 696c 3a20 4f70 7469 6f6e 616c   email: Optional
+00010640: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
+00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010660: 2020 2020 2020 2020 2020 2074 696d 653a             time:
+00010670: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
+00010680: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000106a0: 2020 2020 2a2a 6b77 6172 6773 2920 2d3e      **kwargs) ->
+000106b0: 2054 7570 6c65 5b73 7472 2c20 4469 6374   Tuple[str, Dict
+000106c0: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+000106d0: 2020 2020 2020 2047 656e 6572 6174 6520         Generate 
+000106e0: 7468 6520 536c 7572 6d20 776f 726b 666c  the Slurm workfl
+000106f0: 6f77 2063 6f6d 6d61 6e64 2061 6e64 2065  ow command and e
+00010700: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00010710: 626c 6573 2e0a 0a20 2020 2020 2020 2041  bles...        A
+00010720: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00010730: 2077 6f72 6b66 6c6f 7720 2873 7472 293a   workflow (str):
+00010740: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+00010750: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
+00010760: 2020 2020 2020 2077 6f72 6b66 6c6f 775f         workflow_
+00010770: 7665 7273 696f 6e20 2873 7472 293a 2054  version (str): T
+00010780: 6865 2076 6572 7369 6f6e 206f 6620 7468  he version of th
+00010790: 6520 776f 726b 666c 6f77 2e0a 2020 2020  e workflow..    
+000107a0: 2020 2020 2020 2020 696e 7075 745f 6461          input_da
+000107b0: 7461 2028 7374 7229 3a20 5468 6520 6e61  ta (str): The na
+000107c0: 6d65 206f 6620 7468 6520 696e 7075 7420  me of the input 
+000107d0: 6461 7461 2066 6f6c 6465 7220 636f 6e74  data folder cont
+000107e0: 6169 6e69 6e67 0a20 2020 2020 2020 2020  aining.         
+000107f0: 2020 2020 2020 2074 6865 2069 6e70 7574         the input
+00010800: 2069 6d61 6765 2066 696c 6573 2e0a 2020   image files..  
+00010810: 2020 2020 2020 2020 2020 656d 6169 6c20            email 
+00010820: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00010830: 2054 6865 2065 6d61 696c 2061 6464 7265   The email addre
+00010840: 7373 2066 6f72 206a 6f62 206e 6f74 6966  ss for job notif
+00010850: 6963 6174 696f 6e73 2e0a 2020 2020 2020  ications..      
+00010860: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00010870: 7473 2074 6f20 4e6f 6e65 2c20 7768 6963  ts to None, whic
+00010880: 6820 6465 6661 756c 7473 2074 6f20 7768  h defaults to wh
+00010890: 6174 2069 7320 696e 2074 6865 206a 6f62  at is in the job
+000108a0: 2073 6372 6970 742e 0a20 2020 2020 2020   script..       
+000108b0: 2020 2020 2074 696d 6520 2873 7472 2c20       time (str, 
+000108c0: 6f70 7469 6f6e 616c 293a 2054 6865 2074  optional): The t
+000108d0: 696d 6520 6c69 6d69 7420 666f 7220 7468  ime limit for th
+000108e0: 6520 6a6f 6220 696e 2074 6865 200a 2020  e job in the .  
+000108f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00010900: 726d 6174 2048 483a 4d4d 3a53 532e 2044  rmat HH:MM:SS. D
+00010910: 6566 6175 6c74 7320 746f 204e 6f6e 652c  efaults to None,
+00010920: 2077 6869 6368 2064 6566 6175 6c74 7320   which defaults 
+00010930: 746f 2077 6861 7420 0a20 2020 2020 2020  to what .       
+00010940: 2020 2020 2020 2020 2069 7320 696e 2074           is in t
+00010950: 6865 206a 6f62 2073 6372 6970 742e 0a20  he job script.. 
+00010960: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
+00010970: 7267 733a 2041 6464 6974 696f 6e61 6c20  rgs: Additional 
+00010980: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
+00010990: 7320 666f 7220 7468 6520 776f 726b 666c  s for the workfl
+000109a0: 6f77 2e0a 0a20 2020 2020 2020 2052 6574  ow...        Ret
+000109b0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+000109c0: 2020 5475 706c 655b 7374 722c 2044 6963    Tuple[str, Dic
+000109d0: 745d 3a0a 2020 2020 2020 2020 2020 2020  t]:.            
+000109e0: 2020 2020 4120 7475 706c 6520 636f 6e74      A tuple cont
+000109f0: 6169 6e69 6e67 2074 6865 2053 6c75 726d  aining the Slurm
+00010a00: 2077 6f72 6b66 6c6f 7720 636f 6d6d 616e   workflow comman
+00010a10: 6420 616e 640a 2020 2020 2020 2020 2020  d and.          
+00010a20: 2020 2020 2020 7468 6520 656e 7669 726f        the enviro
+00010a30: 6e6d 656e 7420 7661 7269 6162 6c65 732e  nment variables.
+00010a40: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00010a50: 2020 2020 2020 6d6f 6465 6c5f 7061 7468        model_path
+00010a60: 203d 2073 656c 662e 736c 7572 6d5f 6d6f   = self.slurm_mo
+00010a70: 6465 6c5f 7061 7468 735b 776f 726b 666c  del_paths[workfl
+00010a80: 6f77 2e6c 6f77 6572 2829 5d0a 2020 2020  ow.lower()].    
+00010a90: 2020 2020 6a6f 625f 7363 7269 7074 203d      job_script =
+00010aa0: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
+00010ab0: 6c5f 6a6f 6273 5b77 6f72 6b66 6c6f 772e  l_jobs[workflow.
+00010ac0: 6c6f 7765 7228 295d 0a20 2020 2020 2020  lower()].       
+00010ad0: 206a 6f62 5f70 6172 616d 7320 3d20 7365   job_params = se
+00010ae0: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f6a  lf.slurm_model_j
+00010af0: 6f62 735f 7061 7261 6d73 5b77 6f72 6b66  obs_params[workf
+00010b00: 6c6f 772e 6c6f 7765 7228 295d 0a20 2020  low.lower()].   
+00010b10: 2020 2020 2023 2067 7261 6220 6f6e 6c79       # grab only
+00010b20: 2074 6865 2069 6d61 6765 206e 616d 652c   the image name,
+00010b30: 206e 6f74 2074 6865 2067 726f 7570 2f63   not the group/c
+00010b40: 7265 6174 6f72 0a20 2020 2020 2020 2069  reator.        i
+00010b50: 6d61 6765 203d 2073 656c 662e 736c 7572  mage = self.slur
+00010b60: 6d5f 6d6f 6465 6c5f 696d 6167 6573 5b77  m_model_images[w
+00010b70: 6f72 6b66 6c6f 772e 6c6f 7765 7228 295d  orkflow.lower()]
+00010b80: 2e73 706c 6974 2822 2f22 295b 315d 0a0a  .split("/")[1]..
+00010b90: 2020 2020 2020 2020 7362 6174 6368 5f65          sbatch_e
+00010ba0: 6e76 203d 207b 0a20 2020 2020 2020 2020  nv = {.         
+00010bb0: 2020 2022 4441 5441 5f50 4154 4822 3a20     "DATA_PATH": 
+00010bc0: 6622 5c22 7b73 656c 662e 736c 7572 6d5f  f"\"{self.slurm_
+00010bd0: 6461 7461 5f70 6174 687d 2f7b 696e 7075  data_path}/{inpu
+00010be0: 745f 6461 7461 7d5c 2222 2c0a 2020 2020  t_data}\"",.    
+00010bf0: 2020 2020 2020 2020 2249 4d41 4745 5f50          "IMAGE_P
+00010c00: 4154 4822 3a20 6622 5c22 7b73 656c 662e  ATH": f"\"{self.
+00010c10: 736c 7572 6d5f 696d 6167 6573 5f70 6174  slurm_images_pat
+00010c20: 687d 2f7b 6d6f 6465 6c5f 7061 7468 7d5c  h}/{model_path}\
+00010c30: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+00010c40: 2249 4d41 4745 5f56 4552 5349 4f4e 223a  "IMAGE_VERSION":
+00010c50: 2066 227b 776f 726b 666c 6f77 5f76 6572   f"{workflow_ver
+00010c60: 7369 6f6e 7d22 2c0a 2020 2020 2020 2020  sion}",.        
+00010c70: 2020 2020 2253 494e 4755 4c41 5249 5459      "SINGULARITY
+00010c80: 5f49 4d41 4745 223a 2066 225c 227b 696d  _IMAGE": f"\"{im
+00010c90: 6167 657d 5f7b 776f 726b 666c 6f77 5f76  age}_{workflow_v
+00010ca0: 6572 7369 6f6e 7d2e 7369 665c 2222 2c0a  ersion}.sif\"",.
+00010cb0: 2020 2020 2020 2020 2020 2020 2253 4352              "SCR
+00010cc0: 4950 545f 5041 5448 223a 2066 225c 227b  IPT_PATH": f"\"{
+00010cd0: 7365 6c66 2e73 6c75 726d 5f73 6372 6970  self.slurm_scrip
+00010ce0: 745f 7061 7468 7d5c 2222 0a20 2020 2020  t_path}\"".     
+00010cf0: 2020 207d 0a20 2020 2020 2020 2077 6f72     }.        wor
+00010d00: 6b66 6c6f 775f 656e 7620 3d20 7365 6c66  kflow_env = self
+00010d10: 2e77 6f72 6b66 6c6f 775f 7061 7261 6d73  .workflow_params
+00010d20: 5f74 6f5f 656e 7676 6172 7328 2a2a 6b77  _to_envvars(**kw
+00010d30: 6172 6773 290a 2020 2020 2020 2020 656e  args).        en
+00010d40: 7620 3d20 7b2a 2a73 6261 7463 685f 656e  v = {**sbatch_en
+00010d50: 762c 202a 2a77 6f72 6b66 6c6f 775f 656e  v, **workflow_en
+00010d60: 767d 0a0a 2020 2020 2020 2020 656d 6169  v}..        emai
+00010d70: 6c5f 7061 7261 6d20 3d20 2222 2069 6620  l_param = "" if 
+00010d80: 656d 6169 6c20 6973 204e 6f6e 6520 656c  email is None el
+00010d90: 7365 2066 2220 2d2d 6d61 696c 2d75 7365  se f" --mail-use
+00010da0: 723d 7b65 6d61 696c 7d22 0a20 2020 2020  r={email}".     
+00010db0: 2020 2074 696d 655f 7061 7261 6d20 3d20     time_param = 
+00010dc0: 2222 2069 6620 7469 6d65 2069 7320 4e6f  "" if time is No
+00010dd0: 6e65 2065 6c73 6520 6622 202d 2d74 696d  ne else f" --tim
+00010de0: 653d 7b74 696d 657d 220a 2020 2020 2020  e={time}".      
+00010df0: 2020 6a6f 625f 7061 7261 6d73 2e61 7070    job_params.app
+00010e00: 656e 6428 7469 6d65 5f70 6172 616d 290a  end(time_param).
+00010e10: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
+00010e20: 6d73 2e61 7070 656e 6428 656d 6169 6c5f  ms.append(email_
+00010e30: 7061 7261 6d29 0a20 2020 2020 2020 206a  param).        j
+00010e40: 6f62 5f70 6172 616d 203d 2022 222e 6a6f  ob_param = "".jo
+00010e50: 696e 286a 6f62 5f70 6172 616d 7329 0a20  in(job_params). 
+00010e60: 2020 2020 2020 2073 6261 7463 685f 636d         sbatch_cm
+00010e70: 6420 3d20 6622 7362 6174 6368 7b6a 6f62  d = f"sbatch{job
+00010e80: 5f70 6172 616d 7d20 2d2d 6f75 7470 7574  _param} --output
+00010e90: 3d6f 6d65 726f 2d25 6a2e 6c6f 6720 5c0a  =omero-%j.log \.
+00010ea0: 2020 2020 2020 2020 2020 2020 5c22 7b73              \"{s
+00010eb0: 656c 662e 736c 7572 6d5f 7363 7269 7074  elf.slurm_script
+00010ec0: 5f70 6174 687d 2f7b 6a6f 625f 7363 7269  _path}/{job_scri
+00010ed0: 7074 7d5c 2222 0a0a 2020 2020 2020 2020  pt}\""..        
+00010ee0: 7265 7475 726e 2073 6261 7463 685f 636d  return sbatch_cm
+00010ef0: 642c 2065 6e76 0a0a 2020 2020 6465 6620  d, env..    def 
+00010f00: 6765 745f 636f 6e76 6572 7369 6f6e 5f63  get_conversion_c
+00010f10: 6f6d 6d61 6e64 2873 656c 662c 2064 6174  ommand(self, dat
+00010f20: 615f 7061 7468 3a20 7374 722c 0a20 2020  a_path: str,.   
+00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f40: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+00010f50: 6967 5f66 696c 653a 2073 7472 2c0a 2020  ig_file: str,.  
+00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f70: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
+00010f80: 7263 655f 666f 726d 6174 3a20 7374 7220  rce_format: str 
+00010f90: 3d20 277a 6172 7227 2c0a 2020 2020 2020  = 'zarr',.      
+00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010fb0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00010fc0: 666f 726d 6174 3a20 7374 7220 3d20 2774  format: str = 't
+00010fd0: 6966 6627 2920 2d3e 2054 7570 6c65 5b73  iff') -> Tuple[s
+00010fe0: 7472 2c20 4469 6374 5d3a 0a20 2020 2020  tr, Dict]:.     
+00010ff0: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+00011000: 656e 6572 6174 6520 536c 7572 6d20 636f  enerate Slurm co
+00011010: 6e76 6572 7369 6f6e 2063 6f6d 6d61 6e64  nversion command
+00011020: 2061 6e64 2065 6e76 6972 6f6e 6d65 6e74   and environment
+00011030: 2076 6172 6961 626c 6573 2066 6f72 2064   variables for d
+00011040: 6174 6120 636f 6e76 6572 7369 6f6e 2e0a  ata conversion..
+00011050: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00011060: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+00011070: 7061 7468 2028 7374 7229 3a20 5061 7468  path (str): Path
+00011080: 2074 6f20 7468 6520 6461 7461 2066 6f6c   to the data fol
+00011090: 6465 722e 0a20 2020 2020 2020 2020 2020  der..           
+000110a0: 2063 6f6e 6669 675f 6669 6c65 2028 7374   config_file (st
+000110b0: 7229 3a20 5061 7468 2074 6f20 7468 6520  r): Path to the 
+000110c0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+000110d0: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
+000110e0: 736f 7572 6365 5f66 6f72 6d61 7420 2873  source_format (s
+000110f0: 7472 293a 2053 6f75 7263 6520 6461 7461  tr): Source data
+00011100: 2066 6f72 6d61 7420 2864 6566 6175 6c74   format (default
+00011110: 2069 7320 277a 6172 7227 292e 0a20 2020   is 'zarr')..   
+00011120: 2020 2020 2020 2020 2074 6172 6765 745f           target_
+00011130: 666f 726d 6174 2028 7374 7229 3a20 5461  format (str): Ta
+00011140: 7267 6574 2064 6174 6120 666f 726d 6174  rget data format
+00011150: 2028 6465 6661 756c 7420 6973 2027 7469   (default is 'ti
+00011160: 6666 2729 2e0a 0a20 2020 2020 2020 2052  ff')...        R
+00011170: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00011180: 2020 2020 5475 706c 655b 7374 722c 2044      Tuple[str, D
+00011190: 6963 745d 3a0a 2020 2020 2020 2020 2020  ict]:.          
+000111a0: 2020 2020 2020 4120 7475 706c 6520 636f        A tuple co
+000111b0: 6e74 6169 6e69 6e67 2074 6865 2053 6c75  ntaining the Slu
+000111c0: 726d 2063 6f6e 7665 7273 696f 6e20 636f  rm conversion co
+000111d0: 6d6d 616e 6420 616e 640a 2020 2020 2020  mmand and.      
+000111e0: 2020 2020 2020 2020 2020 7468 6520 656e            the en
+000111f0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00011200: 6c65 732e 0a0a 2020 2020 2020 2020 5761  les...        Wa
+00011210: 726e 696e 673a 0a20 2020 2020 2020 2020  rning:.         
+00011220: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
+00011230: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f6e  mplementation on
+00011240: 6c79 2073 7570 706f 7274 7320 636f 6e76  ly supports conv
+00011250: 6572 7369 6f6e 2066 726f 6d20 277a 6172  ersion from 'zar
+00011260: 7227 2074 6f20 2774 6966 6627 2e0a 2020  r' to 'tiff'..  
+00011270: 2020 2020 2020 2020 2020 4966 2075 7369            If usi
+00011280: 6e67 206f 7468 6572 2073 6f75 7263 6520  ng other source 
+00011290: 6f72 2074 6172 6765 7420 666f 726d 6174  or target format
+000112a0: 732c 2075 7365 7273 206d 7573 7420 696d  s, users must im
+000112b0: 706c 656d 656e 7420 616e 6420 636f 6e66  plement and conf
+000112c0: 6967 7572 650a 2020 2020 2020 2020 2020  igure.          
+000112d0: 2020 6164 6469 7469 6f6e 616c 2063 6f6e    additional con
+000112e0: 7665 7274 6572 7320 7468 656d 7365 6c76  verters themselv
+000112f0: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
+00011300: 2020 2020 2020 2020 6966 2073 6f75 7263          if sourc
+00011310: 655f 666f 726d 6174 2021 3d20 227a 6172  e_format != "zar
+00011320: 7222 206f 7220 7461 7267 6574 5f66 6f72  r" or target_for
+00011330: 6d61 7420 213d 2022 7469 6666 223a 0a20  mat != "tiff":. 
+00011340: 2020 2020 2020 2020 2020 2023 2057 6172             # War
+00011350: 6e20 6162 6f75 7420 756e 7375 7070 6f72  n about unsuppor
+00011360: 7465 6420 636f 6e76 6572 7369 6f6e 3b20  ted conversion; 
+00011370: 6164 6469 7469 6f6e 616c 2063 6f6e 7665  additional conve
+00011380: 7274 6572 7320 6361 6e20 6265 0a20 2020  rters can be.   
+00011390: 2020 2020 2020 2020 2023 2061 6464 6564           # added
+000113a0: 206f 7574 7369 6465 206f 7572 206b 6e6f   outside our kno
+000113b0: 776c 6564 6765 2e0a 2020 2020 2020 2020  wledge..        
+000113c0: 2020 2020 2320 4368 6563 6b69 6e67 2053      # Checking S
+000113d0: 6c75 726d 2773 2060 736c 7572 6d5f 636f  lurm's `slurm_co
+000113e0: 6e76 6572 7465 7273 5f70 6174 6860 2069  nverters_path` i
+000113f0: 7320 736b 6970 7065 6420 666f 720a 2020  s skipped for.  
+00011400: 2020 2020 2020 2020 2020 2320 7065 7266            # perf
+00011410: 6f72 6d61 6e63 6520 7265 6173 6f6e 732e  ormance reasons.
+00011420: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00011430: 6765 722e 7761 726e 696e 6728 0a20 2020  ger.warning(.   
+00011440: 2020 2020 2020 2020 2020 2020 2066 2243               f"C
+00011450: 6f6e 7665 7273 696f 6e20 6672 6f6d 207b  onversion from {
+00011460: 736f 7572 6365 5f66 6f72 6d61 747d 2074  source_format} t
+00011470: 6f20 7b74 6172 6765 745f 666f 726d 6174  o {target_format
+00011480: 7d20 6973 206e 6f74 2073 7570 706f 7274  } is not support
+00011490: 6564 2062 7920 6465 6661 756c 7421 2229  ed by default!")
+000114a0: 0a0a 2020 2020 2020 2020 6368 6f73 656e  ..        chosen
+000114b0: 5f63 6f6e 7665 7274 6572 203d 2066 2263  _converter = f"c
+000114c0: 6f6e 7665 7274 5f7b 736f 7572 6365 5f66  onvert_{source_f
+000114d0: 6f72 6d61 747d 5f74 6f5f 7b74 6172 6765  ormat}_to_{targe
+000114e0: 745f 666f 726d 6174 7d2e 7369 6622 0a20  t_format}.sif". 
+000114f0: 2020 2020 2020 2073 6261 7463 685f 656e         sbatch_en
+00011500: 7620 3d20 7b0a 2020 2020 2020 2020 2020  v = {.          
+00011510: 2020 2244 4154 415f 5041 5448 223a 2066    "DATA_PATH": f
+00011520: 225c 227b 6461 7461 5f70 6174 687d 5c22  "\"{data_path}\"
+00011530: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+00011540: 434f 4e56 4552 5349 4f4e 5f50 4154 4822  CONVERSION_PATH"
+00011550: 3a20 6622 5c22 7b73 656c 662e 736c 7572  : f"\"{self.slur
+00011560: 6d5f 636f 6e76 6572 7465 7273 5f70 6174  m_converters_pat
+00011570: 687d 5c22 222c 0a20 2020 2020 2020 2020  h}\"",.         
+00011580: 2020 2022 434f 4e56 4552 5445 525f 494d     "CONVERTER_IM
+00011590: 4147 4522 3a20 6368 6f73 656e 5f63 6f6e  AGE": chosen_con
+000115a0: 7665 7274 6572 2c0a 2020 2020 2020 2020  verter,.        
+000115b0: 2020 2020 2253 4352 4950 545f 5041 5448      "SCRIPT_PATH
+000115c0: 223a 2066 225c 227b 7365 6c66 2e73 6c75  ": f"\"{self.slu
+000115d0: 726d 5f73 6372 6970 745f 7061 7468 7d5c  rm_script_path}\
+000115e0: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+000115f0: 2243 4f4e 4649 475f 4649 4c45 223a 2066  "CONFIG_FILE": f
+00011600: 225c 227b 636f 6e66 6967 5f66 696c 657d  "\"{config_file}
+00011610: 5c22 220a 2020 2020 2020 2020 7d0a 0a20  \"".        }.. 
+00011620: 2020 2020 2020 2063 6f6e 7665 7273 696f         conversio
+00011630: 6e5f 636d 6420 3d20 2273 6261 7463 6820  n_cmd = "sbatch 
+00011640: 2d2d 6a6f 622d 6e61 6d65 3d63 6f6e 7665  --job-name=conve
+00011650: 7273 696f 6e20 2d2d 6578 706f 7274 3d41  rsion --export=A
+00011660: 4c4c 2c43 4f4e 4649 475f 5041 5448 3d5c  LL,CONFIG_PATH=\
+00011670: 2224 5057 442f 2443 4f4e 4649 475f 4649  "$PWD/$CONFIG_FI
+00011680: 4c45 5c22 202d 2d61 7272 6179 3d31 2d24  LE\" --array=1-$
+00011690: 4e20 5c22 2453 4352 4950 545f 5041 5448  N \"$SCRIPT_PATH
+000116a0: 2f63 6f6e 7665 7274 5f6a 6f62 5f61 7272  /convert_job_arr
+000116b0: 6179 2e73 685c 2222 0a20 2020 2020 2020  ay.sh\"".       
+000116c0: 2023 2063 6f6e 7665 7273 696f 6e5f 636d   # conversion_cm
+000116d0: 645f 7761 6974 696e 6720 3d20 2273 6261  d_waiting = "sba
+000116e0: 7463 6820 2d2d 6a6f 622d 6e61 6d65 3d63  tch --job-name=c
+000116f0: 6f6e 7665 7273 696f 6e20 2d2d 6578 706f  onversion --expo
+00011700: 7274 3d41 4c4c 2c43 4f4e 4649 475f 5041  rt=ALL,CONFIG_PA
+00011710: 5448 3d5c 2224 5057 442f 2443 4f4e 4649  TH=\"$PWD/$CONFI
+00011720: 475f 4649 4c45 5c22 202d 2d61 7272 6179  G_FILE\" --array
+00011730: 3d31 2d24 4e20 2d2d 7761 6974 2024 5343  =1-$N --wait $SC
+00011740: 5249 5054 5f50 4154 482f 636f 6e76 6572  RIPT_PATH/conver
+00011750: 745f 6a6f 625f 6172 7261 792e 7368 220a  t_job_array.sh".
+00011760: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011770: 636f 6e76 6572 7369 6f6e 5f63 6d64 2c20  conversion_cmd, 
+00011780: 7362 6174 6368 5f65 6e76 0a0a 2020 2020  sbatch_env..    
+00011790: 6465 6620 776f 726b 666c 6f77 5f70 6172  def workflow_par
+000117a0: 616d 735f 746f 5f65 6e76 7661 7273 2873  ams_to_envvars(s
+000117b0: 656c 662c 202a 2a6b 7761 7267 7329 202d  elf, **kwargs) -
+000117c0: 3e20 4469 6374 3a0a 2020 2020 2020 2020  > Dict:.        
+000117d0: 2222 220a 2020 2020 2020 2020 436f 6e76  """.        Conv
+000117e0: 6572 7420 776f 726b 666c 6f77 2070 6172  ert workflow par
+000117f0: 616d 6574 6572 7320 746f 2065 6e76 6972  ameters to envir
+00011800: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
+00011810: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00011820: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+00011830: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
+00011840: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
+00011850: 6e74 7320 666f 7220 7468 6520 776f 726b  nts for the work
+00011860: 666c 6f77 2e0a 0a20 2020 2020 2020 2052  flow...        R
+00011870: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00011880: 2020 2020 4469 6374 3a20 4120 6469 6374      Dict: A dict
+00011890: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
+000118a0: 6720 7468 6520 656e 7669 726f 6e6d 656e  g the environmen
+000118b0: 7420 7661 7269 6162 6c65 732e 0a20 2020  t variables..   
+000118c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000118d0: 2077 6f72 6b66 6c6f 775f 656e 7620 3d20   workflow_env = 
+000118e0: 7b6b 6579 2e75 7070 6572 2829 3a20 6622  {key.upper(): f"
+000118f0: 7b76 616c 7565 7d22 2066 6f72 206b 6579  {value}" for key
+00011900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011910: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
+00011920: 696e 206b 7761 7267 732e 6974 656d 7328  in kwargs.items(
+00011930: 297d 0a20 2020 2020 2020 206c 6f67 6765  )}.        logge
+00011940: 722e 6465 6275 6728 776f 726b 666c 6f77  r.debug(workflow
+00011950: 5f65 6e76 290a 2020 2020 2020 2020 7265  _env).        re
+00011960: 7475 726e 2077 6f72 6b66 6c6f 775f 656e  turn workflow_en
+00011970: 760a 0a20 2020 2064 6566 2067 6574 5f63  v..    def get_c
+00011980: 656c 6c70 6f73 655f 636f 6d6d 616e 6428  ellpose_command(
+00011990: 7365 6c66 2c20 696d 6167 655f 7665 7273  self, image_vers
+000119a0: 696f 6e3a 2073 7472 2c0a 2020 2020 2020  ion: str,.      
+000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119c0: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
+000119d0: 613a 2073 7472 2c0a 2020 2020 2020 2020  a: str,.        
+000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000119f0: 2020 2020 2063 705f 6d6f 6465 6c3a 2073       cp_model: s
+00011a00: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a20: 206e 7563 5f63 6861 6e6e 656c 3a20 696e   nuc_channel: in
+00011a30: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
 00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a50: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00011a60: 202d 3e20 5265 7375 6c74 3a0a 2020 2020   -> Result:.    
-00011a70: 2020 2020 2222 225a 6970 2074 6865 206f      """Zip the o
-00011a80: 7574 7075 7420 666f 6c64 6572 206f 6620  utput folder of 
-00011a90: 6120 6a6f 6220 6f6e 2053 6c75 726d 0a0a  a job on Slurm..
-00011aa0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00011ab0: 2020 2020 2020 2020 2020 6461 7461 5f6c            data_l
-00011ac0: 6f63 6174 696f 6e20 2853 7472 696e 6729  ocation (String)
-00011ad0: 3a20 466f 6c64 6572 206f 6e20 534c 5552  : Folder on SLUR
-00011ae0: 4d20 7769 7468 2074 6865 2022 6461 7461  M with the "data
-00011af0: 2f6f 7574 220a 2020 2020 2020 2020 2020  /out".          
-00011b00: 2020 2020 2020 7375 6266 6f6c 6465 722e        subfolder.
-00011b10: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
-00011b20: 656e 616d 6520 2853 7472 696e 6729 3a20  ename (String): 
-00011b30: 4e61 6d65 2074 6f20 6769 7665 2074 6f20  Name to give to 
-00011b40: 7468 6520 7a69 7066 696c 652e 0a20 2020  the zipfile..   
-00011b50: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
-00011b60: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
-00011b70: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
-00011b80: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
-00011b90: 7269 6162 6c65 7320 746f 200a 2020 2020  riables to .    
-00011ba0: 2020 2020 2020 2020 2020 2020 7365 7420              set 
-00011bb0: 7768 656e 2072 756e 6e69 6e67 2074 6865  when running the
-00011bc0: 2063 6f6d 6d61 6e64 2e20 4465 6661 756c   command. Defaul
-00011bd0: 7473 2074 6f20 4e6f 6e65 2e0a 0a20 2020  ts to None...   
-00011be0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
-00011bf0: 2020 2020 2020 2020 2020 5265 7375 6c74            Result
-00011c00: 3a20 5468 6520 7265 7375 6c74 206f 6620  : The result of 
-00011c10: 7468 6520 7a69 7020 6174 7465 6d70 742e  the zip attempt.
-00011c20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011c30: 2020 2020 2023 207a 6970 0a20 2020 2020       # zip.     
-00011c40: 2020 207a 6970 5f63 6d64 203d 2073 656c     zip_cmd = sel
-00011c50: 662e 6765 745f 7a69 705f 636f 6d6d 616e  f.get_zip_comman
-00011c60: 6428 6461 7461 5f6c 6f63 6174 696f 6e2c  d(data_location,
-00011c70: 2066 696c 656e 616d 6529 0a20 2020 2020   filename).     
-00011c80: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
-00011c90: 225a 6970 7069 6e67 207b 6461 7461 5f6c  "Zipping {data_l
-00011ca0: 6f63 6174 696f 6e7d 2061 7320 7b66 696c  ocation} as {fil
-00011cb0: 656e 616d 657d 206f 6e20 536c 7572 6d22  ename} on Slurm"
-00011cc0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00011cd0: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
-00011ce0: 6473 285b 7a69 705f 636d 645d 2c20 656e  ds([zip_cmd], en
-00011cf0: 763d 656e 7629 0a0a 2020 2020 6465 6620  v=env)..    def 
-00011d00: 6765 745f 7a69 705f 636f 6d6d 616e 6428  get_zip_command(
-00011d10: 7365 6c66 2c20 6461 7461 5f6c 6f63 6174  self, data_locat
-00011d20: 696f 6e3a 2073 7472 2c20 6669 6c65 6e61  ion: str, filena
-00011d30: 6d65 3a20 7374 7229 202d 3e20 7374 723a  me: str) -> str:
-00011d40: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00011d50: 2020 2020 2047 656e 6572 6174 6520 6120       Generate a 
-00011d60: 636f 6d6d 616e 6420 7374 7269 6e67 2066  command string f
-00011d70: 6f72 207a 6970 7069 6e67 2074 6865 2064  or zipping the d
-00011d80: 6174 6120 6f6e 2053 6c75 726d 2e0a 0a20  ata on Slurm... 
-00011d90: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00011da0: 2020 2020 2020 2020 2064 6174 615f 6c6f           data_lo
-00011db0: 6361 7469 6f6e 2028 7374 7229 3a20 5468  cation (str): Th
-00011dc0: 6520 666f 6c64 6572 2074 6f20 6265 207a  e folder to be z
-00011dd0: 6970 7065 642e 0a20 2020 2020 2020 2020  ipped..         
-00011de0: 2020 2066 696c 656e 616d 6520 2873 7472     filename (str
-00011df0: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
-00011e00: 6865 207a 6970 2061 7263 6869 7665 2066  he zip archive f
-00011e10: 696c 6520 746f 2065 7874 7261 6374 2e0a  ile to extract..
-00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e30: 5769 7468 6f75 7420 6578 7465 6e73 696f  Without extensio
-00011e40: 6e2e 0a0a 2020 2020 2020 2020 5265 7475  n...        Retu
-00011e50: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00011e60: 2073 7472 3a20 5468 6520 636f 6d6d 616e   str: The comman
-00011e70: 6420 746f 2063 7265 6174 6520 7468 6520  d to create the 
-00011e80: 7a69 7020 6669 6c65 2e0a 2020 2020 2020  zip file..      
-00011e90: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00011ea0: 7475 726e 2073 656c 662e 5f5a 4950 5f43  turn self._ZIP_C
-00011eb0: 4d44 2e66 6f72 6d61 7428 6669 6c65 6e61  MD.format(filena
-00011ec0: 6d65 3d66 696c 656e 616d 652c 0a20 2020  me=filename,.   
-00011ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ef0: 2064 6174 615f 6c6f 6361 7469 6f6e 3d64   data_location=d
-00011f00: 6174 615f 6c6f 6361 7469 6f6e 290a 0a20  ata_location).. 
-00011f10: 2020 2064 6566 2067 6574 5f6c 6f67 6669     def get_logfi
-00011f20: 6c65 5f66 726f 6d5f 736c 7572 6d28 7365  le_from_slurm(se
-00011f30: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00011f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f50: 2020 2073 6c75 726d 5f6a 6f62 5f69 643a     slurm_job_id:
-00011f60: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-00011f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011f80: 2020 2020 206c 6f63 616c 5f74 6d70 5f73       local_tmp_s
-00011f90: 746f 7261 6765 3a20 7374 7220 3d20 222f  torage: str = "/
-00011fa0: 746d 702f 222c 0a20 2020 2020 2020 2020  tmp/",.         
-00011fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fc0: 2020 2020 2020 6c6f 6766 696c 653a 2073        logfile: s
-00011fd0: 7472 203d 204e 6f6e 650a 2020 2020 2020  tr = None.      
-00011fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ff0: 2020 2020 2020 2020 2029 202d 3e20 5475           ) -> Tu
-00012000: 706c 655b 7374 722c 2073 7472 2c20 5472  ple[str, str, Tr
-00012010: 616e 7366 6572 5265 7375 6c74 5d3a 0a20  ansferResult]:. 
-00012020: 2020 2020 2020 2022 2222 436f 7079 2074         """Copy t
-00012030: 6865 206c 6f67 6669 6c65 206f 6620 7468  he logfile of th
-00012040: 6520 6769 7665 6e20 534c 5552 4d20 6a6f  e given SLURM jo
-00012050: 6220 746f 2074 6865 206c 6f63 616c 2073  b to the local s
-00012060: 6572 7665 722e 0a0a 2020 2020 2020 2020  erver...        
-00012070: 4e6f 7465 2061 626f 7574 2028 5472 616e  Note about (Tran
-00012080: 7366 6572 2952 6573 756c 743a 0a0a 2020  sfer)Result:..  
-00012090: 2020 2020 2020 556e 6c69 6b65 2073 696d        Unlike sim
-000120a0: 696c 6172 2063 6c61 7373 6573 2073 7563  ilar classes suc
-000120b0: 6820 6173 2069 6e76 6f6b 652e 7275 6e6e  h as invoke.runn
-000120c0: 6572 732e 5265 7375 6c74 0a20 2020 2020  ers.Result.     
-000120d0: 2020 206f 7220 6661 6272 6963 2e72 756e     or fabric.run
-000120e0: 6e65 7273 2e52 6573 756c 740a 2020 2020  ners.Result.    
-000120f0: 2020 2020 2877 6869 6368 2068 6176 6520      (which have 
-00012100: 6120 636f 6e63 6570 7420 6f66 20e2 809c  a concept of ...
-00012110: 7761 726e 2061 6e64 2072 6574 7572 6e20  warn and return 
-00012120: 616e 7977 6179 7320 6f6e 2066 6169 6c75  anyways on failu
-00012130: 7265 e280 9d29 0a20 2020 2020 2020 2074  re...).        t
-00012140: 6869 7320 636c 6173 7320 6861 7320 6e6f  his class has no
-00012150: 2075 7365 6675 6c20 7472 7574 6869 6e65   useful truthine
-00012160: 7373 2062 6568 6176 696f 722e 0a20 2020  ss behavior..   
-00012170: 2020 2020 2049 6620 6120 6669 6c65 2074       If a file t
-00012180: 7261 6e73 6665 7220 6661 696c 732c 2073  ransfer fails, s
-00012190: 6f6d 6520 6578 6365 7074 696f 6e20 7769  ome exception wi
-000121a0: 6c6c 2062 6520 7261 6973 6564 2c0a 2020  ll be raised,.  
-000121b0: 2020 2020 2020 6569 7468 6572 2061 6e20        either an 
-000121c0: 4f53 4572 726f 7220 6f72 2061 6e20 6572  OSError or an er
-000121d0: 726f 7220 6672 6f6d 2077 6974 6869 6e20  ror from within 
-000121e0: 5061 7261 6d69 6b6f 2e0a 0a20 2020 2020  Paramiko...     
-000121f0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00012200: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
-00012210: 6420 2873 7472 293a 2054 6865 2049 4420  d (str): The ID 
-00012220: 6f66 2074 6865 2053 4c55 524d 206a 6f62  of the SLURM job
-00012230: 2e0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
-00012240: 6361 6c5f 746d 705f 7374 6f72 6167 6520  cal_tmp_storage 
-00012250: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-00012260: 2050 6174 6820 746f 2073 746f 7265 2074   Path to store t
-00012270: 6865 206c 6f67 6669 6c65 200a 2020 2020  he logfile .    
-00012280: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
-00012290: 6c6c 792e 2044 6566 6175 6c74 7320 746f  lly. Defaults to
-000122a0: 2022 2f74 6d70 2f22 2e0a 2020 2020 2020   "/tmp/"..      
-000122b0: 2020 2020 2020 6c6f 6766 696c 6520 2873        logfile (s
-000122c0: 7472 2c20 6f70 7469 6f6e 616c 293a 2050  tr, optional): P
-000122d0: 6174 6820 746f 2074 6865 206c 6f67 6669  ath to the logfi
-000122e0: 6c65 206f 6e20 7468 6520 534c 5552 4d20  le on the SLURM 
-000122f0: 7365 7276 6572 2e0a 2020 2020 2020 2020  server..        
-00012300: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00012310: 2074 6f20 4e6f 6e65 2e0a 0a20 2020 2020   to None...     
-00012320: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00012330: 2020 2020 2020 2020 5475 706c 653a 2064          Tuple: d
-00012340: 6972 6563 746f 7279 2c20 6675 6c6c 2070  irectory, full p
-00012350: 6174 6820 6f66 2074 6865 206c 6f67 6669  ath of the logfi
-00012360: 6c65 2c20 616e 6420 5472 616e 7366 6572  le, and Transfer
-00012370: 5265 7375 6c74 0a20 2020 2020 2020 2022  Result.        "
-00012380: 2222 0a20 2020 2020 2020 2069 6620 6c6f  "".        if lo
-00012390: 6766 696c 6520 6973 204e 6f6e 653a 0a20  gfile is None:. 
-000123a0: 2020 2020 2020 2020 2020 206c 6f67 6669             logfi
-000123b0: 6c65 203d 2073 656c 662e 5f4c 4f47 4649  le = self._LOGFI
-000123c0: 4c45 0a20 2020 2020 2020 206c 6f67 6669  LE.        logfi
-000123d0: 6c65 203d 206c 6f67 6669 6c65 2e66 6f72  le = logfile.for
-000123e0: 6d61 7428 736c 7572 6d5f 6a6f 625f 6964  mat(slurm_job_id
-000123f0: 3d73 6c75 726d 5f6a 6f62 5f69 6429 0a20  =slurm_job_id). 
-00012400: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00012410: 666f 2866 2243 6f70 7969 6e67 206c 6f67  fo(f"Copying log
-00012420: 6669 6c65 207b 6c6f 6766 696c 657d 2066  file {logfile} f
-00012430: 726f 6d20 536c 7572 6d5c 0a20 2020 2020  rom Slurm\.     
-00012440: 2020 2020 2020 2074 6f20 7b6c 6f63 616c         to {local
-00012450: 5f74 6d70 5f73 746f 7261 6765 7d22 290a  _tmp_storage}").
-00012460: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
-00012470: 2073 656c 662e 6765 7428 0a20 2020 2020   self.get(.     
-00012480: 2020 2020 2020 2072 656d 6f74 653d 6c6f         remote=lo
-00012490: 6766 696c 652c 0a20 2020 2020 2020 2020  gfile,.         
-000124a0: 2020 206c 6f63 616c 3d6c 6f63 616c 5f74     local=local_t
-000124b0: 6d70 5f73 746f 7261 6765 290a 2020 2020  mp_storage).    
-000124c0: 2020 2020 6578 706f 7274 5f66 696c 6520      export_file 
-000124d0: 3d20 6c6f 6361 6c5f 746d 705f 7374 6f72  = local_tmp_stor
-000124e0: 6167 652b 6c6f 6766 696c 650a 2020 2020  age+logfile.    
-000124f0: 2020 2020 7265 7475 726e 206c 6f63 616c      return local
-00012500: 5f74 6d70 5f73 746f 7261 6765 2c20 6578  _tmp_storage, ex
-00012510: 706f 7274 5f66 696c 652c 2072 6573 756c  port_file, resul
-00012520: 740a 0a20 2020 2064 6566 2067 6574 5f75  t..    def get_u
-00012530: 6e7a 6970 5f63 6f6d 6d61 6e64 2873 656c  nzip_command(sel
-00012540: 662c 207a 6970 6669 6c65 3a20 7374 722c  f, zipfile: str,
-00012550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012560: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-00012570: 725f 6669 6c65 7479 7065 733a 2073 7472  r_filetypes: str
-00012580: 203d 2022 2a2e 7a61 7272 202a 2e74 6966   = "*.zarr *.tif
-00012590: 6620 2a2e 7469 6622 0a20 2020 2020 2020  f *.tif".       
-000125a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125b0: 2020 2029 202d 3e20 7374 723a 0a20 2020     ) -> str:.   
-000125c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000125d0: 2047 656e 6572 6174 6520 6120 636f 6d6d   Generate a comm
-000125e0: 616e 6420 7374 7269 6e67 2066 6f72 2075  and string for u
-000125f0: 6e7a 6970 7069 6e67 2061 2064 6174 6120  nzipping a data 
-00012600: 6172 6368 6976 6520 616e 6420 6372 6561  archive and crea
-00012610: 7469 6e67 0a20 2020 2020 2020 2072 6571  ting.        req
-00012620: 7569 7265 6420 6469 7265 6374 6f72 6965  uired directorie
-00012630: 7320 666f 7220 536c 7572 6d20 6a6f 6273  s for Slurm jobs
-00012640: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00012650: 0a20 2020 2020 2020 2020 2020 207a 6970  .            zip
-00012660: 6669 6c65 2028 7374 7229 3a20 5468 6520  file (str): The 
-00012670: 6e61 6d65 206f 6620 7468 6520 7a69 7020  name of the zip 
-00012680: 6172 6368 6976 6520 6669 6c65 2074 6f20  archive file to 
-00012690: 6578 7472 6163 742e 0a20 2020 2020 2020  extract..       
-000126a0: 2020 2020 2020 2020 2057 6974 686f 7574           Without
-000126b0: 2065 7874 656e 7369 6f6e 2e0a 2020 2020   extension..    
-000126c0: 2020 2020 2020 2020 6669 6c74 6572 5f66          filter_f
-000126d0: 696c 6574 7970 6573 2028 7374 722c 206f  iletypes (str, o
-000126e0: 7074 696f 6e61 6c29 3a20 4120 7370 6163  ptional): A spac
-000126f0: 652d 7365 7061 7261 7465 6420 7374 7269  e-separated stri
-00012700: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-00012710: 2020 2063 6f6e 7461 696e 696e 6720 7468     containing th
-00012720: 6520 6669 6c65 2065 7874 656e 7369 6f6e  e file extension
-00012730: 7320 746f 2065 7874 7261 6374 2066 726f  s to extract fro
-00012740: 6d20 7468 6520 7a69 7020 6669 6c65 2e0a  m the zip file..
+00011a50: 7072 6f62 5f74 6872 6573 686f 6c64 3a20  prob_threshold: 
+00011a60: 666c 6f61 742c 0a20 2020 2020 2020 2020  float,.         
+00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a80: 2020 2020 6365 6c6c 5f64 6961 6d65 7465      cell_diamete
+00011a90: 723a 2066 6c6f 6174 2c0a 2020 2020 2020  r: float,.      
+00011aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ab0: 2020 2020 2020 2065 6d61 696c 3a20 4f70         email: Op
+00011ac0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
+00011ad0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011af0: 2074 696d 653a 204f 7074 696f 6e61 6c5b   time: Optional[
+00011b00: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
+00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b20: 2020 2020 2020 2020 2020 7573 655f 6770            use_gp
+00011b30: 753a 2062 6f6f 6c20 3d20 5472 7565 2c0a  u: bool = True,.
+00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b50: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+00011b60: 656c 3a20 7374 7220 3d20 2263 656c 6c70  el: str = "cellp
+00011b70: 6f73 6522 2920 2d3e 2054 7570 6c65 5b73  ose") -> Tuple[s
+00011b80: 7472 2c20 4469 6374 5d3a 0a20 2020 2020  tr, Dict]:.     
+00011b90: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
+00011ba0: 6574 7572 6e20 7468 6520 636f 6d6d 616e  eturn the comman
+00011bb0: 6420 616e 6420 656e 7669 726f 6e6d 656e  d and environmen
+00011bc0: 7420 6469 6374 696f 6e61 7279 2074 6f20  t dictionary to 
+00011bd0: 7275 6e20 6120 4365 6c6c 506f 7365 206a  run a CellPose j
+00011be0: 6f62 0a20 2020 2020 2020 206f 6e20 7468  ob.        on th
+00011bf0: 6520 536c 7572 6d20 776f 726b 6c6f 6164  e Slurm workload
+00011c00: 206d 616e 6167 6572 2e0a 2020 2020 2020   manager..      
+00011c10: 2020 4120 7370 6563 6966 6963 2065 7861    A specific exa
+00011c20: 6d70 6c65 206f 6620 7573 696e 6720 7468  mple of using th
+00011c30: 6520 6765 6e65 7269 6320 2767 6574 5f77  e generic 'get_w
+00011c40: 6f72 6b66 6c6f 775f 636f 6d6d 616e 6427  orkflow_command'
+00011c50: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00011c60: 0a20 2020 2020 2020 2020 2020 2069 6d61  .            ima
+00011c70: 6765 5f76 6572 7369 6f6e 2028 7374 7229  ge_version (str)
+00011c80: 3a20 5468 6520 7665 7273 696f 6e20 6f66  : The version of
+00011c90: 2074 6865 2053 696e 6775 6c61 7269 7479   the Singularity
+00011ca0: 2069 6d61 6765 2074 6f20 7573 652e 0a20   image to use.. 
+00011cb0: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00011cc0: 5f64 6174 6120 2873 7472 293a 2054 6865  _data (str): The
+00011cd0: 206e 616d 6520 6f66 2074 6865 2069 6e70   name of the inp
+00011ce0: 7574 2064 6174 6120 666f 6c64 6572 206f  ut data folder o
+00011cf0: 6e20 7468 6520 7368 6172 6564 0a20 2020  n the shared.   
+00011d00: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+00011d10: 6520 7379 7374 656d 2e0a 2020 2020 2020  e system..      
+00011d20: 2020 2020 2020 6370 5f6d 6f64 656c 2028        cp_model (
+00011d30: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
+00011d40: 6620 7468 6520 4365 6c6c 506f 7365 206d  f the CellPose m
+00011d50: 6f64 656c 2074 6f20 7573 652e 0a20 2020  odel to use..   
+00011d60: 2020 2020 2020 2020 206e 7563 5f63 6861           nuc_cha
+00011d70: 6e6e 656c 2028 696e 7429 3a20 5468 6520  nnel (int): The 
+00011d80: 696e 6465 7820 6f66 2074 6865 206e 7563  index of the nuc
+00011d90: 6c65 6172 2063 6861 6e6e 656c 2e0a 2020  lear channel..  
+00011da0: 2020 2020 2020 2020 2020 7072 6f62 5f74            prob_t
+00011db0: 6872 6573 686f 6c64 2028 666c 6f61 7429  hreshold (float)
+00011dc0: 3a20 5468 6520 7072 6f62 6162 696c 6974  : The probabilit
+00011dd0: 7920 7468 7265 7368 6f6c 6420 666f 720a  y threshold for.
+00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011df0: 6e75 636c 6569 2064 6574 6563 7469 6f6e  nuclei detection
+00011e00: 2e0a 2020 2020 2020 2020 2020 2020 6365  ..            ce
+00011e10: 6c6c 5f64 6961 6d65 7465 7220 2866 6c6f  ll_diameter (flo
+00011e20: 6174 293a 2054 6865 2065 7870 6563 7465  at): The expecte
+00011e30: 6420 6365 6c6c 2064 6961 6d65 7465 7220  d cell diameter 
+00011e40: 696e 2070 6978 656c 732e 0a20 2020 2020  in pixels..     
+00011e50: 2020 2020 2020 2065 6d61 696c 2028 4f70         email (Op
+00011e60: 7469 6f6e 616c 5b73 7472 5d29 3a20 5468  tional[str]): Th
+00011e70: 6520 656d 6169 6c20 6164 6472 6573 7320  e email address 
+00011e80: 746f 2073 656e 6420 6e6f 7469 6669 6361  to send notifica
+00011e90: 7469 6f6e 7320 746f 2e0a 2020 2020 2020  tions to..      
+00011ea0: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00011eb0: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
+00011ec0: 2020 2020 2020 2020 7469 6d65 2028 4f70          time (Op
+00011ed0: 7469 6f6e 616c 5b73 7472 5d29 3a20 5468  tional[str]): Th
+00011ee0: 6520 6d61 7869 6d75 6d20 7469 6d65 2066  e maximum time f
+00011ef0: 6f72 2074 6865 206a 6f62 2074 6f20 7275  or the job to ru
+00011f00: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
+00011f10: 2020 2044 6566 6175 6c74 7320 746f 204e     Defaults to N
+00011f20: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
+00011f30: 2075 7365 5f67 7075 2028 626f 6f6c 293a   use_gpu (bool):
+00011f40: 2057 6865 7468 6572 2074 6f20 7573 6520   Whether to use 
+00011f50: 4750 5520 666f 7220 7468 6520 4365 6c6c  GPU for the Cell
+00011f60: 506f 7365 206a 6f62 2e0a 2020 2020 2020  Pose job..      
+00011f70: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00011f80: 7473 2074 6f20 5472 7565 2e0a 2020 2020  ts to True..    
+00011f90: 2020 2020 2020 2020 6d6f 6465 6c20 2873          model (s
+00011fa0: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
+00011fb0: 2074 6865 2066 6f6c 6465 7220 6f66 2074   the folder of t
+00011fc0: 6865 2044 6f63 6b65 7220 696d 6167 6520  he Docker image 
+00011fd0: 746f 2075 7365 2e0a 2020 2020 2020 2020  to use..        
+00011fe0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+00011ff0: 2074 6f20 2263 656c 6c70 6f73 6522 2e0a   to "cellpose"..
+00012000: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00012010: 3a0a 2020 2020 2020 2020 2020 2020 5475  :.            Tu
+00012020: 706c 655b 7374 722c 2064 6963 745d 3a0a  ple[str, dict]:.
+00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012040: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
+00012050: 6e67 2074 6865 2053 6c75 726d 2073 6261  ng the Slurm sba
+00012060: 7463 6820 636f 6d6d 616e 640a 2020 2020  tch command.    
+00012070: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00012080: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
+00012090: 6469 6374 696f 6e61 7279 2e0a 2020 2020  dictionary..    
+000120a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000120b0: 7265 7475 726e 2073 656c 662e 6765 745f  return self.get_
+000120c0: 776f 726b 666c 6f77 5f63 6f6d 6d61 6e64  workflow_command
+000120d0: 2877 6f72 6b66 6c6f 773d 6d6f 6465 6c2c  (workflow=model,
+000120e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012100: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+00012110: 6f77 5f76 6572 7369 6f6e 3d69 6d61 6765  ow_version=image
+00012120: 5f76 6572 7369 6f6e 2c0a 2020 2020 2020  _version,.      
+00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012150: 2020 2069 6e70 7574 5f64 6174 613d 696e     input_data=in
+00012160: 7075 745f 6461 7461 2c0a 2020 2020 2020  put_data,.      
+00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012190: 2020 2065 6d61 696c 3d65 6d61 696c 2c0a     email=email,.
+000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121c0: 2020 2020 2020 2020 2074 696d 653d 7469           time=ti
+000121d0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121f0: 2020 2020 2020 2020 2020 2020 2063 705f               cp_
+00012200: 6d6f 6465 6c3d 6370 5f6d 6f64 656c 2c0a  model=cp_model,.
+00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012230: 2020 2020 2020 2020 206e 7563 5f63 6861           nuc_cha
+00012240: 6e6e 656c 3d6e 7563 5f63 6861 6e6e 656c  nnel=nuc_channel
+00012250: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012270: 2020 2020 2020 2020 2020 2070 726f 625f             prob_
+00012280: 7468 7265 7368 6f6c 643d 7072 6f62 5f74  threshold=prob_t
+00012290: 6872 6573 686f 6c64 2c0a 2020 2020 2020  hreshold,.      
+000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122c0: 2020 2063 656c 6c5f 6469 616d 6574 6572     cell_diameter
+000122d0: 3d63 656c 6c5f 6469 616d 6574 6572 2c0a  =cell_diameter,.
+000122e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012300: 2020 2020 2020 2020 2075 7365 5f67 7075           use_gpu
+00012310: 3d75 7365 5f67 7075 290a 0a20 2020 2064  =use_gpu)..    d
+00012320: 6566 2063 6f70 795f 7a69 705f 6c6f 6361  ef copy_zip_loca
+00012330: 6c6c 7928 7365 6c66 2c20 6c6f 6361 6c5f  lly(self, local_
+00012340: 746d 705f 7374 6f72 6167 653a 2073 7472  tmp_storage: str
+00012350: 2c20 6669 6c65 6e61 6d65 3a20 7374 720a  , filename: str.
+00012360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012370: 2020 2020 2020 2020 2029 202d 3e20 5472           ) -> Tr
+00012380: 616e 7366 6572 5265 7375 6c74 3a0a 2020  ansferResult:.  
+00012390: 2020 2020 2020 2222 2220 436f 7079 2061        """ Copy a
+000123a0: 207a 6970 2066 696c 6520 6672 6f6d 2053   zip file from S
+000123b0: 6c75 726d 2074 6f20 7468 6520 6c6f 6361  lurm to the loca
+000123c0: 6c20 7365 7276 6572 2e0a 0a20 2020 2020  l server...     
+000123d0: 2020 204e 6f74 6520 6162 6f75 7420 2854     Note about (T
+000123e0: 7261 6e73 6665 7229 5265 7375 6c74 3a0a  ransfer)Result:.
+000123f0: 0a20 2020 2020 2020 2055 6e6c 696b 6520  .        Unlike 
+00012400: 7369 6d69 6c61 7220 636c 6173 7365 7320  similar classes 
+00012410: 7375 6368 2061 7320 696e 766f 6b65 2e72  such as invoke.r
+00012420: 756e 6e65 7273 2e52 6573 756c 7420 6f72  unners.Result or
+00012430: 0a20 2020 2020 2020 2066 6162 7269 632e  .        fabric.
+00012440: 7275 6e6e 6572 732e 5265 7375 6c74 0a20  runners.Result. 
+00012450: 2020 2020 2020 2028 7768 6963 6820 6861         (which ha
+00012460: 7665 2061 2063 6f6e 6365 7074 206f 6620  ve a concept of 
+00012470: e280 9c77 6172 6e20 616e 6420 7265 7475  ...warn and retu
+00012480: 726e 2061 6e79 7761 7973 206f 6e20 6661  rn anyways on fa
+00012490: 696c 7572 65e2 809d 290a 2020 2020 2020  ilure...).      
+000124a0: 2020 7468 6973 2063 6c61 7373 2068 6173    this class has
+000124b0: 206e 6f20 7573 6566 756c 2074 7275 7468   no useful truth
+000124c0: 696e 6573 7320 6265 6861 7669 6f72 2e0a  iness behavior..
+000124d0: 2020 2020 2020 2020 4966 2061 2066 696c          If a fil
+000124e0: 6520 7472 616e 7366 6572 2066 6169 6c73  e transfer fails
+000124f0: 2c20 736f 6d65 2065 7863 6570 7469 6f6e  , some exception
+00012500: 2077 696c 6c20 6265 2072 6169 7365 642c   will be raised,
+00012510: 0a20 2020 2020 2020 2065 6974 6865 7220  .        either 
+00012520: 616e 204f 5345 7272 6f72 206f 7220 616e  an OSError or an
+00012530: 2065 7272 6f72 2066 726f 6d20 7769 7468   error from with
+00012540: 696e 2050 6172 616d 696b 6f2e 0a0a 2020  in Paramiko...  
+00012550: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00012560: 2020 2020 2020 2020 6c6f 6361 6c5f 746d          local_tm
+00012570: 705f 7374 6f72 6167 6520 2853 7472 696e  p_storage (Strin
+00012580: 6729 3a20 5061 7468 2074 6f20 7374 6f72  g): Path to stor
+00012590: 6520 7468 6520 7a69 7020 6669 6c65 206c  e the zip file l
+000125a0: 6f63 616c 6c79 2e0a 2020 2020 2020 2020  ocally..        
+000125b0: 2020 2020 6669 6c65 6e61 6d65 2028 5374      filename (St
+000125c0: 7269 6e67 293a 205a 6970 2066 696c 656e  ring): Zip filen
+000125d0: 616d 6520 6f6e 2053 6c75 726d 2e0a 0a20  ame on Slurm... 
+000125e0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+000125f0: 2020 2020 2020 2020 2020 2020 5472 616e              Tran
+00012600: 7366 6572 5265 7375 6c74 3a20 5468 6520  sferResult: The 
+00012610: 7265 7375 6c74 206f 6620 7468 6520 7363  result of the sc
+00012620: 7020 6174 7465 6d70 742e 0a20 2020 2020  p attempt..     
+00012630: 2020 2022 2222 0a20 2020 2020 2020 206c     """.        l
+00012640: 6f67 6765 722e 696e 666f 2866 2243 6f70  ogger.info(f"Cop
+00012650: 7969 6e67 207a 6970 207b 6669 6c65 6e61  ying zip {filena
+00012660: 6d65 7d20 6672 6f6d 5c0a 2020 2020 2020  me} from\.      
+00012670: 2020 2020 2020 536c 7572 6d20 746f 207b        Slurm to {
+00012680: 6c6f 6361 6c5f 746d 705f 7374 6f72 6167  local_tmp_storag
+00012690: 657d 2229 0a20 2020 2020 2020 2072 6574  e}").        ret
+000126a0: 7572 6e20 7365 6c66 2e67 6574 280a 2020  urn self.get(.  
+000126b0: 2020 2020 2020 2020 2020 7265 6d6f 7465            remote
+000126c0: 3d66 227b 6669 6c65 6e61 6d65 7d2e 7a69  =f"{filename}.zi
+000126d0: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
+000126e0: 6c6f 6361 6c3d 6c6f 6361 6c5f 746d 705f  local=local_tmp_
+000126f0: 7374 6f72 6167 6529 0a0a 2020 2020 6465  storage)..    de
+00012700: 6620 7a69 705f 6461 7461 5f6f 6e5f 736c  f zip_data_on_sl
+00012710: 7572 6d5f 7365 7276 6572 2873 656c 662c  urm_server(self,
+00012720: 2064 6174 615f 6c6f 6361 7469 6f6e 3a20   data_location: 
+00012730: 7374 722c 2066 696c 656e 616d 653a 2073  str, filename: s
+00012740: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
 00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012760: 452e 672e 2064 6566 6175 6c74 7320 746f  E.g. defaults to
-00012770: 2022 2a2e 7a61 7272 202a 2e74 6966 6620   "*.zarr *.tiff 
-00012780: 2a2e 7469 6622 2e0a 2020 2020 2020 2020  *.tif"..        
-00012790: 2020 2020 2020 2020 5365 7474 696e 6720          Setting 
-000127a0: 7468 6973 2061 7267 756d 656e 7420 746f  this argument to
-000127b0: 2060 4e6f 6e65 6020 7769 6c6c 206f 6d69   `None` will omi
-000127c0: 7420 7468 6520 6669 6c65 0a20 2020 2020  t the file.     
-000127d0: 2020 2020 2020 2020 2020 2066 696c 7465             filte
-000127e0: 7220 616e 6420 6578 7472 6163 7420 616c  r and extract al
-000127f0: 6c20 6669 6c65 732e 0a0a 2020 2020 2020  l files...      
-00012800: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00012810: 2020 2020 2020 2073 7472 3a0a 2020 2020         str:.    
-00012820: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-00012830: 636f 6d6d 616e 6420 746f 2065 7874 7261  command to extra
-00012840: 6374 2074 6865 2073 7065 6369 6669 6564  ct the specified
-00012850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012860: 2066 696c 6574 7970 6573 2066 726f 6d20   filetypes from 
-00012870: 7468 6520 7a69 7020 6669 6c65 2e0a 2020  the zip file..  
-00012880: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012890: 2020 756e 7a69 705f 636d 6420 3d20 6622    unzip_cmd = f"
-000128a0: 6d6b 6469 7220 7b73 656c 662e 736c 7572  mkdir {self.slur
-000128b0: 6d5f 6461 7461 5f70 6174 687d 2f7b 7a69  m_data_path}/{zi
-000128c0: 7066 696c 657d 205c 0a20 2020 2020 2020  pfile} \.       
-000128d0: 2020 2020 2020 2020 2020 2020 207b 7365               {se
-000128e0: 6c66 2e73 6c75 726d 5f64 6174 615f 7061  lf.slurm_data_pa
-000128f0: 7468 7d2f 7b7a 6970 6669 6c65 7d2f 6461  th}/{zipfile}/da
-00012900: 7461 205c 0a20 2020 2020 2020 2020 2020  ta \.           
-00012910: 2020 2020 2020 2020 207b 7365 6c66 2e73           {self.s
-00012920: 6c75 726d 5f64 6174 615f 7061 7468 7d2f  lurm_data_path}/
-00012930: 7b7a 6970 6669 6c65 7d2f 6461 7461 2f69  {zipfile}/data/i
-00012940: 6e20 5c0a 2020 2020 2020 2020 2020 2020  n \.            
-00012950: 2020 2020 2020 2020 7b73 656c 662e 736c          {self.sl
-00012960: 7572 6d5f 6461 7461 5f70 6174 687d 2f7b  urm_data_path}/{
-00012970: 7a69 7066 696c 657d 2f64 6174 612f 6f75  zipfile}/data/ou
-00012980: 7420 5c0a 2020 2020 2020 2020 2020 2020  t \.            
-00012990: 2020 2020 2020 2020 7b73 656c 662e 736c          {self.sl
-000129a0: 7572 6d5f 6461 7461 5f70 6174 687d 2f7b  urm_data_path}/{
-000129b0: 7a69 7066 696c 657d 2f64 6174 612f 6774  zipfile}/data/gt
-000129c0: 3b20 5c0a 2020 2020 2020 2020 2020 2020  ; \.            
-000129d0: 2020 2020 2020 2020 377a 2078 202d 7920          7z x -y 
-000129e0: 2d6f 7b73 656c 662e 736c 7572 6d5f 6461  -o{self.slurm_da
-000129f0: 7461 5f70 6174 687d 2f7b 7a69 7066 696c  ta_path}/{zipfil
-00012a00: 657d 2f64 6174 612f 696e 205c 0a20 2020  e}/data/in \.   
-00012a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012a20: 207b 7365 6c66 2e73 6c75 726d 5f64 6174   {self.slurm_dat
-00012a30: 615f 7061 7468 7d2f 7b7a 6970 6669 6c65  a_path}/{zipfile
-00012a40: 7d2e 7a69 7020 7b66 696c 7465 725f 6669  }.zip {filter_fi
-00012a50: 6c65 7479 7065 737d 220a 0a20 2020 2020  letypes}"..     
-00012a60: 2020 2072 6574 7572 6e20 756e 7a69 705f     return unzip_
-00012a70: 636d 640a 0a20 2020 2064 6566 2067 6574  cmd..    def get
-00012a80: 5f69 6d61 6765 5f76 6572 7369 6f6e 735f  _image_versions_
-00012a90: 616e 645f 6461 7461 5f66 696c 6573 2873  and_data_files(s
-00012aa0: 656c 662c 206d 6f64 656c 3a20 7374 720a  elf, model: str.
-00012ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ad0: 2020 2020 2020 2020 2020 2920 2d3e 2054            ) -> T
-00012ae0: 7570 6c65 5b4c 6973 745b 7374 725d 2c20  uple[List[str], 
-00012af0: 4c69 7374 5b73 7472 5d5d 3a0a 2020 2020  List[str]]:.    
-00012b00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00012b10: 5265 7472 6965 7665 2074 6865 2061 7661  Retrieve the ava
-00012b20: 696c 6162 6c65 2069 6d61 6765 2076 6572  ilable image ver
-00012b30: 7369 6f6e 7320 616e 6420 696e 7075 7420  sions and input 
-00012b40: 6461 7461 2066 696c 6573 2066 6f72 2061  data files for a
-00012b50: 0a20 2020 2020 2020 2067 6976 656e 206d  .        given m
-00012b60: 6f64 656c 2e0a 0a20 2020 2020 2020 2041  odel...        A
-00012b70: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00012b80: 206d 6f64 656c 2028 7374 7229 3a20 5468   model (str): Th
-00012b90: 6520 6e61 6d65 206f 6620 7468 6520 6d6f  e name of the mo
-00012ba0: 6465 6c20 746f 2071 7565 7279 2066 6f72  del to query for
-00012bb0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00012bc0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00012bd0: 5475 706c 655b 4c69 7374 5b73 7472 5d2c  Tuple[List[str],
-00012be0: 204c 6973 745b 7374 725d 5d3a 0a20 2020   List[str]]:.   
-00012bf0: 2020 2020 2020 2020 2020 2020 2041 2074               A t
-00012c00: 7570 6c65 2063 6f6e 7461 696e 696e 6720  uple containing 
-00012c10: 7477 6f20 6c69 7374 733a 0a20 2020 2020  two lists:.     
-00012c20: 2020 2020 2020 2020 2020 202d 2054 6865             - The
-00012c30: 2066 6972 7374 206c 6973 7420 696e 636c   first list incl
-00012c40: 7564 6573 2074 6865 2061 7661 696c 6162  udes the availab
-00012c50: 6c65 2069 6d61 6765 2076 6572 7369 6f6e  le image version
-00012c60: 732c 200a 2020 2020 2020 2020 2020 2020  s, .            
-00012c70: 2020 2020 2020 2020 736f 7274 6564 2069          sorted i
-00012c80: 6e20 6465 7363 656e 6469 6e67 206f 7264  n descending ord
-00012c90: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
-00012ca0: 2020 2020 2d20 5468 6520 7365 636f 6e64      - The second
-00012cb0: 206c 6973 7420 696e 636c 7564 6573 2074   list includes t
-00012cc0: 6865 2061 7661 696c 6162 6c65 2064 6174  he available dat
-00012cd0: 6120 6669 6c65 732e 0a0a 2020 2020 2020  a files...      
-00012ce0: 2020 5261 6973 6573 3a0a 2020 2020 2020    Raises:.      
-00012cf0: 2020 2020 2020 5661 6c75 6545 7272 6f72        ValueError
-00012d00: 3a20 4966 2074 6865 2070 726f 7669 6465  : If the provide
-00012d10: 6420 6d6f 6465 6c20 6973 206e 6f74 2066  d model is not f
-00012d20: 6f75 6e64 2069 6e20 7468 650a 2020 2020  ound in the.    
-00012d30: 2020 2020 2020 2020 2020 2020 536c 7572              Slur
-00012d40: 6d43 6c69 656e 7427 7320 6b6e 6f77 6e20  mClient's known 
-00012d50: 6d6f 6465 6c20 7061 7468 732e 0a20 2020  model paths..   
-00012d60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012d70: 2069 6d61 6765 5f70 6174 6820 3d20 7365   image_path = se
-00012d80: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f70  lf.slurm_model_p
-00012d90: 6174 6873 2e67 6574 286d 6f64 656c 290a  aths.get(model).
-00012da0: 2020 2020 2020 2020 6966 206e 6f74 2069          if not i
-00012db0: 6d61 6765 5f70 6174 683a 0a20 2020 2020  mage_path:.     
-00012dc0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00012dd0: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-00012de0: 2020 2020 2020 2020 2066 224e 6f20 7061           f"No pa
-00012df0: 7468 206b 6e6f 776e 2066 6f72 2070 726f  th known for pro
-00012e00: 7669 6465 6420 6d6f 6465 6c20 7b6d 6f64  vided model {mod
-00012e10: 656c 7d2c 205c 0a20 2020 2020 2020 2020  el}, \.         
-00012e20: 2020 2020 2020 2020 2020 2069 6e20 7b73             in {s
-00012e30: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
-00012e40: 7061 7468 737d 2229 0a20 2020 2020 2020  paths}").       
-00012e50: 2063 6d64 6c69 7374 203d 205b 0a20 2020   cmdlist = [.   
-00012e60: 2020 2020 2020 2020 2073 656c 662e 5f56           self._V
-00012e70: 4552 5349 4f4e 5f43 4d44 2e66 6f72 6d61  ERSION_CMD.forma
-00012e80: 7428 736c 7572 6d5f 696d 6167 6573 5f70  t(slurm_images_p
-00012e90: 6174 683d 7365 6c66 2e73 6c75 726d 5f69  ath=self.slurm_i
-00012ea0: 6d61 6765 735f 7061 7468 2c0a 2020 2020  mages_path,.    
-00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ed0: 2069 6d61 6765 5f70 6174 683d 696d 6167   image_path=imag
-00012ee0: 655f 7061 7468 292c 0a20 2020 2020 2020  e_path),.       
-00012ef0: 2020 2020 2073 656c 662e 5f44 4154 415f       self._DATA_
-00012f00: 434d 442e 666f 726d 6174 2873 6c75 726d  CMD.format(slurm
-00012f10: 5f64 6174 615f 7061 7468 3d73 656c 662e  _data_path=self.
-00012f20: 736c 7572 6d5f 6461 7461 5f70 6174 6829  slurm_data_path)
-00012f30: 5d0a 2020 2020 2020 2020 2320 7370 6c69  ].        # spli
-00012f40: 7420 7265 7370 6f6e 7365 7320 7065 7220  t responses per 
-00012f50: 636f 6d6d 616e 640a 2020 2020 2020 2020  command.        
-00012f60: 7265 7370 6f6e 7365 5f6c 6973 7420 3d20  response_list = 
-00012f70: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-00012f80: 735f 7370 6c69 745f 6f75 7428 636d 646c  s_split_out(cmdl
-00012f90: 6973 7429 0a20 2020 2020 2020 2023 2073  ist).        # s
-00012fa0: 706c 6974 206c 696e 6573 2066 7572 7468  plit lines furth
-00012fb0: 6572 2069 6e74 6f20 7375 626c 6973 7473  er into sublists
-00012fc0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
-00012fd0: 655f 6c69 7374 203d 205b 7265 7370 6f6e  e_list = [respon
-00012fe0: 7365 2e73 7472 6970 2829 2e73 706c 6974  se.strip().split
-00012ff0: 2827 5c6e 2729 0a20 2020 2020 2020 2020  ('\n').         
-00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013010: 666f 7220 7265 7370 6f6e 7365 2069 6e20  for response in 
-00013020: 7265 7370 6f6e 7365 5f6c 6973 745d 0a20  response_list]. 
-00013030: 2020 2020 2020 2072 6573 706f 6e73 655f         response_
-00013040: 6c69 7374 5b30 5d20 3d20 736f 7274 6564  list[0] = sorted
-00013050: 2872 6573 706f 6e73 655f 6c69 7374 5b30  (response_list[0
-00013060: 5d2c 2072 6576 6572 7365 3d54 7275 6529  ], reverse=True)
-00013070: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013080: 7265 7370 6f6e 7365 5f6c 6973 745b 305d  response_list[0]
-00013090: 2c20 7265 7370 6f6e 7365 5f6c 6973 745b  , response_list[
-000130a0: 315d 0a0a 2020 2020 6465 6620 6765 745f  1]..    def get_
-000130b0: 616c 6c5f 696d 6167 655f 7665 7273 696f  all_image_versio
-000130c0: 6e73 5f61 6e64 5f64 6174 615f 6669 6c65  ns_and_data_file
-000130d0: 7328 7365 6c66 0a20 2020 2020 2020 2020  s(self.         
-000130e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000130f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013100: 2020 2020 2029 202d 3e20 5475 706c 655b       ) -> Tuple[
-00013110: 4469 6374 5b73 7472 2c20 4c69 7374 5b73  Dict[str, List[s
-00013120: 7472 5d5d 2c0a 2020 2020 2020 2020 2020  tr]],.          
-00013130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013150: 2020 2020 2020 2020 2020 2020 2020 204c                 L
-00013160: 6973 745b 7374 725d 5d3a 0a20 2020 2020  ist[str]]:.     
-00013170: 2020 2022 2222 5265 7472 6965 7665 2061     """Retrieve a
-00013180: 6c6c 2061 7661 696c 6162 6c65 2069 6d61  ll available ima
-00013190: 6765 2076 6572 7369 6f6e 7320 616e 6420  ge versions and 
-000131a0: 6461 7461 2066 696c 6573 2066 726f 6d0a  data files from.
-000131b0: 2020 2020 2020 2020 7468 6520 536c 7572          the Slur
-000131c0: 6d20 636c 7573 7465 722e 0a0a 2020 2020  m cluster...    
-000131d0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-000131e0: 2020 2020 2020 2020 5475 706c 655b 4469          Tuple[Di
-000131f0: 6374 5b73 7472 2c20 4c69 7374 5b73 7472  ct[str, List[str
-00013200: 5d5d 2c20 4c69 7374 5b73 7472 5d5d 3a0a  ]], List[str]]:.
-00013210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013220: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
-00013230: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
-00013240: 2020 2020 2d20 4120 6469 6374 696f 6e61      - A dictiona
-00013250: 7279 206d 6170 7069 6e67 206d 6f64 656c  ry mapping model
-00013260: 7320 746f 2061 7661 696c 6162 6c65 2076  s to available v
-00013270: 6572 7369 6f6e 732e 0a20 2020 2020 2020  ersions..       
-00013280: 2020 2020 2020 2020 202d 2041 206c 6973           - A lis
-00013290: 7420 6f66 2061 7661 696c 6162 6c65 2069  t of available i
-000132a0: 6e70 7574 2064 6174 6120 666f 6c64 6572  nput data folder
-000132b0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-000132c0: 2020 2020 2020 2072 6573 756c 7464 6963         resultdic
-000132d0: 7420 3d20 7b7d 0a20 2020 2020 2020 2063  t = {}.        c
-000132e0: 6d64 6c69 7374 203d 205b 5d0a 0a20 2020  mdlist = []..   
-000132f0: 2020 2020 2066 6f72 2070 6174 6820 696e       for path in
-00013300: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
-00013310: 6c5f 7061 7468 732e 7661 6c75 6573 2829  l_paths.values()
-00013320: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
-00013330: 7468 636d 6420 3d20 7365 6c66 2e5f 5645  thcmd = self._VE
-00013340: 5253 494f 4e5f 434d 442e 666f 726d 6174  RSION_CMD.format
-00013350: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00013360: 2020 736c 7572 6d5f 696d 6167 6573 5f70    slurm_images_p
-00013370: 6174 683d 7365 6c66 2e73 6c75 726d 5f69  ath=self.slurm_i
-00013380: 6d61 6765 735f 7061 7468 2c0a 2020 2020  mages_path,.    
-00013390: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-000133a0: 655f 7061 7468 3d70 6174 6829 0a20 2020  e_path=path).   
-000133b0: 2020 2020 2020 2020 2063 6d64 6c69 7374           cmdlist
-000133c0: 2e61 7070 656e 6428 7061 7468 636d 6429  .append(pathcmd)
-000133d0: 0a0a 2020 2020 2020 2020 2320 4164 6420  ..        # Add 
-000133e0: 6461 7461 2070 6174 6820 746f 6f0a 2020  data path too.  
-000133f0: 2020 2020 2020 636d 646c 6973 742e 6170        cmdlist.ap
-00013400: 7065 6e64 2873 656c 662e 5f44 4154 415f  pend(self._DATA_
-00013410: 434d 442e 666f 726d 6174 280a 2020 2020  CMD.format(.    
-00013420: 2020 2020 2020 2020 736c 7572 6d5f 6461          slurm_da
-00013430: 7461 5f70 6174 683d 7365 6c66 2e73 6c75  ta_path=self.slu
-00013440: 726d 5f64 6174 615f 7061 7468 2929 0a0a  rm_data_path))..
-00013450: 2020 2020 2020 2020 2320 5370 6c69 7420          # Split 
-00013460: 7265 7370 6f6e 7365 7320 7065 7220 636f  responses per co
-00013470: 6d6d 616e 640a 2020 2020 2020 2020 7265  mmand.        re
-00013480: 7370 6f6e 7365 5f6c 6973 7420 3d20 7365  sponse_list = se
-00013490: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 735f  lf.run_commands_
-000134a0: 7370 6c69 745f 6f75 7428 636d 646c 6973  split_out(cmdlis
-000134b0: 7429 0a0a 2020 2020 2020 2020 2320 5370  t)..        # Sp
-000134c0: 6c69 7420 6c69 6e65 7320 6675 7274 6865  lit lines furthe
-000134d0: 7220 696e 746f 2073 7562 6c69 7374 730a  r into sublists.
-000134e0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-000134f0: 5f6c 6973 7420 3d20 5b72 6573 706f 6e73  _list = [respons
-00013500: 652e 7374 7269 7028 292e 7370 6c69 7428  e.strip().split(
-00013510: 275c 6e27 290a 2020 2020 2020 2020 2020  '\n').          
-00013520: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-00013530: 6f72 2072 6573 706f 6e73 6520 696e 2072  or response in r
-00013540: 6573 706f 6e73 655f 6c69 7374 5d0a 0a20  esponse_list].. 
-00013550: 2020 2020 2020 2066 6f72 2069 2c20 6b20         for i, k 
-00013560: 696e 2065 6e75 6d65 7261 7465 2873 656c  in enumerate(sel
-00013570: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7061  f.slurm_model_pa
-00013580: 7468 7329 3a0a 2020 2020 2020 2020 2020  ths):.          
-00013590: 2020 2320 5265 7475 726e 2068 6967 6865    # Return highe
-000135a0: 7374 2076 6572 7369 6f6e 2066 6972 7374  st version first
-000135b0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-000135c0: 756c 7464 6963 745b 6b5d 203d 2073 6f72  ultdict[k] = sor
-000135d0: 7465 6428 7265 7370 6f6e 7365 5f6c 6973  ted(response_lis
-000135e0: 745b 695d 2c20 7265 7665 7273 653d 5472  t[i], reverse=Tr
-000135f0: 7565 290a 0a20 2020 2020 2020 2072 6574  ue)..        ret
-00013600: 7572 6e20 7265 7375 6c74 6469 6374 2c20  urn resultdict, 
-00013610: 7265 7370 6f6e 7365 5f6c 6973 745b 2d31  response_list[-1
-00013620: 5d0a                                     ].
+00012760: 2020 2020 2065 6e76 3a20 4f70 7469 6f6e       env: Option
+00012770: 616c 5b44 6963 745b 7374 722c 2073 7472  al[Dict[str, str
+00012780: 5d5d 203d 204e 6f6e 650a 2020 2020 2020  ]] = None.      
+00012790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000127a0: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
+000127b0: 5265 7375 6c74 3a0a 2020 2020 2020 2020  Result:.        
+000127c0: 2222 225a 6970 2074 6865 206f 7574 7075  """Zip the outpu
+000127d0: 7420 666f 6c64 6572 206f 6620 6120 6a6f  t folder of a jo
+000127e0: 6220 6f6e 2053 6c75 726d 0a0a 2020 2020  b on Slurm..    
+000127f0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00012800: 2020 2020 2020 6461 7461 5f6c 6f63 6174        data_locat
+00012810: 696f 6e20 2853 7472 696e 6729 3a20 466f  ion (String): Fo
+00012820: 6c64 6572 206f 6e20 534c 5552 4d20 7769  lder on SLURM wi
+00012830: 7468 2074 6865 2022 6461 7461 2f6f 7574  th the "data/out
+00012840: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00012850: 2020 7375 6266 6f6c 6465 722e 0a20 2020    subfolder..   
+00012860: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
+00012870: 6520 2853 7472 696e 6729 3a20 4e61 6d65  e (String): Name
+00012880: 2074 6f20 6769 7665 2074 6f20 7468 6520   to give to the 
+00012890: 7a69 7066 696c 652e 0a20 2020 2020 2020  zipfile..       
+000128a0: 2020 2020 2065 6e76 2028 4469 6374 5b73       env (Dict[s
+000128b0: 7472 2c20 7374 725d 2c20 6f70 7469 6f6e  tr, str], option
+000128c0: 616c 293a 204f 7074 696f 6e61 6c20 656e  al): Optional en
+000128d0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+000128e0: 6c65 7320 746f 200a 2020 2020 2020 2020  les to .        
+000128f0: 2020 2020 2020 2020 7365 7420 7768 656e          set when
+00012900: 2072 756e 6e69 6e67 2074 6865 2063 6f6d   running the com
+00012910: 6d61 6e64 2e20 4465 6661 756c 7473 2074  mand. Defaults t
+00012920: 6f20 4e6f 6e65 2e0a 0a20 2020 2020 2020  o None...       
+00012930: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00012940: 2020 2020 2020 5265 7375 6c74 3a20 5468        Result: Th
+00012950: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
+00012960: 7a69 7020 6174 7465 6d70 742e 0a20 2020  zip attempt..   
+00012970: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012980: 2023 207a 6970 0a20 2020 2020 2020 207a   # zip.        z
+00012990: 6970 5f63 6d64 203d 2073 656c 662e 6765  ip_cmd = self.ge
+000129a0: 745f 7a69 705f 636f 6d6d 616e 6428 6461  t_zip_command(da
+000129b0: 7461 5f6c 6f63 6174 696f 6e2c 2066 696c  ta_location, fil
+000129c0: 656e 616d 6529 0a20 2020 2020 2020 206c  ename).        l
+000129d0: 6f67 6765 722e 696e 666f 2866 225a 6970  ogger.info(f"Zip
+000129e0: 7069 6e67 207b 6461 7461 5f6c 6f63 6174  ping {data_locat
+000129f0: 696f 6e7d 2061 7320 7b66 696c 656e 616d  ion} as {filenam
+00012a00: 657d 206f 6e20 536c 7572 6d22 290a 2020  e} on Slurm").  
+00012a10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+00012a20: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
+00012a30: 7a69 705f 636d 645d 2c20 656e 763d 656e  zip_cmd], env=en
+00012a40: 7629 0a0a 2020 2020 6465 6620 6765 745f  v)..    def get_
+00012a50: 7a69 705f 636f 6d6d 616e 6428 7365 6c66  zip_command(self
+00012a60: 2c20 6461 7461 5f6c 6f63 6174 696f 6e3a  , data_location:
+00012a70: 2073 7472 2c20 6669 6c65 6e61 6d65 3a20   str, filename: 
+00012a80: 7374 7229 202d 3e20 7374 723a 0a20 2020  str) -> str:.   
+00012a90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012aa0: 2047 656e 6572 6174 6520 6120 636f 6d6d   Generate a comm
+00012ab0: 616e 6420 7374 7269 6e67 2066 6f72 207a  and string for z
+00012ac0: 6970 7069 6e67 2074 6865 2064 6174 6120  ipping the data 
+00012ad0: 6f6e 2053 6c75 726d 2e0a 0a20 2020 2020  on Slurm...     
+00012ae0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00012af0: 2020 2020 2064 6174 615f 6c6f 6361 7469       data_locati
+00012b00: 6f6e 2028 7374 7229 3a20 5468 6520 666f  on (str): The fo
+00012b10: 6c64 6572 2074 6f20 6265 207a 6970 7065  lder to be zippe
+00012b20: 642e 0a20 2020 2020 2020 2020 2020 2066  d..            f
+00012b30: 696c 656e 616d 6520 2873 7472 293a 2054  ilename (str): T
+00012b40: 6865 206e 616d 6520 6f66 2074 6865 207a  he name of the z
+00012b50: 6970 2061 7263 6869 7665 2066 696c 6520  ip archive file 
+00012b60: 746f 2065 7874 7261 6374 2e0a 2020 2020  to extract..    
+00012b70: 2020 2020 2020 2020 2020 2020 5769 7468              With
+00012b80: 6f75 7420 6578 7465 6e73 696f 6e2e 0a0a  out extension...
+00012b90: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00012ba0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+00012bb0: 3a20 5468 6520 636f 6d6d 616e 6420 746f  : The command to
+00012bc0: 2063 7265 6174 6520 7468 6520 7a69 7020   create the zip 
+00012bd0: 6669 6c65 2e0a 2020 2020 2020 2020 2222  file..        ""
+00012be0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+00012bf0: 2073 656c 662e 5f5a 4950 5f43 4d44 2e66   self._ZIP_CMD.f
+00012c00: 6f72 6d61 7428 6669 6c65 6e61 6d65 3d66  ormat(filename=f
+00012c10: 696c 656e 616d 652c 0a20 2020 2020 2020  ilename,.       
+00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c30: 2020 2020 2020 2020 2020 2020 2064 6174               dat
+00012c40: 615f 6c6f 6361 7469 6f6e 3d64 6174 615f  a_location=data_
+00012c50: 6c6f 6361 7469 6f6e 290a 0a20 2020 2064  location)..    d
+00012c60: 6566 2067 6574 5f6c 6f67 6669 6c65 5f66  ef get_logfile_f
+00012c70: 726f 6d5f 736c 7572 6d28 7365 6c66 2c0a  rom_slurm(self,.
+00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00012ca0: 6c75 726d 5f6a 6f62 5f69 643a 2073 7472  lurm_job_id: str
+00012cb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cd0: 206c 6f63 616c 5f74 6d70 5f73 746f 7261   local_tmp_stora
+00012ce0: 6765 3a20 7374 7220 3d20 222f 746d 702f  ge: str = "/tmp/
+00012cf0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d10: 2020 6c6f 6766 696c 653a 2073 7472 203d    logfile: str =
+00012d20: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d40: 2020 2020 2029 202d 3e20 5475 706c 655b       ) -> Tuple[
+00012d50: 7374 722c 2073 7472 2c20 5472 616e 7366  str, str, Transf
+00012d60: 6572 5265 7375 6c74 5d3a 0a20 2020 2020  erResult]:.     
+00012d70: 2020 2022 2222 436f 7079 2074 6865 206c     """Copy the l
+00012d80: 6f67 6669 6c65 206f 6620 7468 6520 6769  ogfile of the gi
+00012d90: 7665 6e20 534c 5552 4d20 6a6f 6220 746f  ven SLURM job to
+00012da0: 2074 6865 206c 6f63 616c 2073 6572 7665   the local serve
+00012db0: 722e 0a0a 2020 2020 2020 2020 4e6f 7465  r...        Note
+00012dc0: 2061 626f 7574 2028 5472 616e 7366 6572   about (Transfer
+00012dd0: 2952 6573 756c 743a 0a0a 2020 2020 2020  )Result:..      
+00012de0: 2020 556e 6c69 6b65 2073 696d 696c 6172    Unlike similar
+00012df0: 2063 6c61 7373 6573 2073 7563 6820 6173   classes such as
+00012e00: 2069 6e76 6f6b 652e 7275 6e6e 6572 732e   invoke.runners.
+00012e10: 5265 7375 6c74 0a20 2020 2020 2020 206f  Result.        o
+00012e20: 7220 6661 6272 6963 2e72 756e 6e65 7273  r fabric.runners
+00012e30: 2e52 6573 756c 740a 2020 2020 2020 2020  .Result.        
+00012e40: 2877 6869 6368 2068 6176 6520 6120 636f  (which have a co
+00012e50: 6e63 6570 7420 6f66 20e2 809c 7761 726e  ncept of ...warn
+00012e60: 2061 6e64 2072 6574 7572 6e20 616e 7977   and return anyw
+00012e70: 6179 7320 6f6e 2066 6169 6c75 7265 e280  ays on failure..
+00012e80: 9d29 0a20 2020 2020 2020 2074 6869 7320  .).        this 
+00012e90: 636c 6173 7320 6861 7320 6e6f 2075 7365  class has no use
+00012ea0: 6675 6c20 7472 7574 6869 6e65 7373 2062  ful truthiness b
+00012eb0: 6568 6176 696f 722e 0a20 2020 2020 2020  ehavior..       
+00012ec0: 2049 6620 6120 6669 6c65 2074 7261 6e73   If a file trans
+00012ed0: 6665 7220 6661 696c 732c 2073 6f6d 6520  fer fails, some 
+00012ee0: 6578 6365 7074 696f 6e20 7769 6c6c 2062  exception will b
+00012ef0: 6520 7261 6973 6564 2c0a 2020 2020 2020  e raised,.      
+00012f00: 2020 6569 7468 6572 2061 6e20 4f53 4572    either an OSEr
+00012f10: 726f 7220 6f72 2061 6e20 6572 726f 7220  ror or an error 
+00012f20: 6672 6f6d 2077 6974 6869 6e20 5061 7261  from within Para
+00012f30: 6d69 6b6f 2e0a 0a20 2020 2020 2020 2041  miko...        A
+00012f40: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00012f50: 2073 6c75 726d 5f6a 6f62 5f69 6420 2873   slurm_job_id (s
+00012f60: 7472 293a 2054 6865 2049 4420 6f66 2074  tr): The ID of t
+00012f70: 6865 2053 4c55 524d 206a 6f62 2e0a 2020  he SLURM job..  
+00012f80: 2020 2020 2020 2020 2020 6c6f 6361 6c5f            local_
+00012f90: 746d 705f 7374 6f72 6167 6520 2873 7472  tmp_storage (str
+00012fa0: 2c20 6f70 7469 6f6e 616c 293a 2050 6174  , optional): Pat
+00012fb0: 6820 746f 2073 746f 7265 2074 6865 206c  h to store the l
+00012fc0: 6f67 6669 6c65 200a 2020 2020 2020 2020  ogfile .        
+00012fd0: 2020 2020 2020 2020 6c6f 6361 6c6c 792e          locally.
+00012fe0: 2044 6566 6175 6c74 7320 746f 2022 2f74   Defaults to "/t
+00012ff0: 6d70 2f22 2e0a 2020 2020 2020 2020 2020  mp/"..          
+00013000: 2020 6c6f 6766 696c 6520 2873 7472 2c20    logfile (str, 
+00013010: 6f70 7469 6f6e 616c 293a 2050 6174 6820  optional): Path 
+00013020: 746f 2074 6865 206c 6f67 6669 6c65 206f  to the logfile o
+00013030: 6e20 7468 6520 534c 5552 4d20 7365 7276  n the SLURM serv
+00013040: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
+00013050: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
+00013060: 4e6f 6e65 2e0a 0a20 2020 2020 2020 2052  None...        R
+00013070: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00013080: 2020 2020 5475 706c 653a 2064 6972 6563      Tuple: direc
+00013090: 746f 7279 2c20 6675 6c6c 2070 6174 6820  tory, full path 
+000130a0: 6f66 2074 6865 206c 6f67 6669 6c65 2c20  of the logfile, 
+000130b0: 616e 6420 5472 616e 7366 6572 5265 7375  and TransferResu
+000130c0: 6c74 0a20 2020 2020 2020 2022 2222 0a20  lt.        """. 
+000130d0: 2020 2020 2020 2069 6620 6c6f 6766 696c         if logfil
+000130e0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+000130f0: 2020 2020 2020 206c 6f67 6669 6c65 203d         logfile =
+00013100: 2073 656c 662e 5f4c 4f47 4649 4c45 0a20   self._LOGFILE. 
+00013110: 2020 2020 2020 206c 6f67 6669 6c65 203d         logfile =
+00013120: 206c 6f67 6669 6c65 2e66 6f72 6d61 7428   logfile.format(
+00013130: 736c 7572 6d5f 6a6f 625f 6964 3d73 6c75  slurm_job_id=slu
+00013140: 726d 5f6a 6f62 5f69 6429 0a20 2020 2020  rm_job_id).     
+00013150: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+00013160: 2243 6f70 7969 6e67 206c 6f67 6669 6c65  "Copying logfile
+00013170: 207b 6c6f 6766 696c 657d 2066 726f 6d20   {logfile} from 
+00013180: 536c 7572 6d5c 0a20 2020 2020 2020 2020  Slurm\.         
+00013190: 2020 2074 6f20 7b6c 6f63 616c 5f74 6d70     to {local_tmp
+000131a0: 5f73 746f 7261 6765 7d22 290a 2020 2020  _storage}").    
+000131b0: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
+000131c0: 662e 6765 7428 0a20 2020 2020 2020 2020  f.get(.         
+000131d0: 2020 2072 656d 6f74 653d 6c6f 6766 696c     remote=logfil
+000131e0: 652c 0a20 2020 2020 2020 2020 2020 206c  e,.            l
+000131f0: 6f63 616c 3d6c 6f63 616c 5f74 6d70 5f73  ocal=local_tmp_s
+00013200: 746f 7261 6765 290a 2020 2020 2020 2020  torage).        
+00013210: 6578 706f 7274 5f66 696c 6520 3d20 6c6f  export_file = lo
+00013220: 6361 6c5f 746d 705f 7374 6f72 6167 652b  cal_tmp_storage+
+00013230: 6c6f 6766 696c 650a 2020 2020 2020 2020  logfile.        
+00013240: 7265 7475 726e 206c 6f63 616c 5f74 6d70  return local_tmp
+00013250: 5f73 746f 7261 6765 2c20 6578 706f 7274  _storage, export
+00013260: 5f66 696c 652c 2072 6573 756c 740a 0a20  _file, result.. 
+00013270: 2020 2064 6566 2067 6574 5f75 6e7a 6970     def get_unzip
+00013280: 5f63 6f6d 6d61 6e64 2873 656c 662c 207a  _command(self, z
+00013290: 6970 6669 6c65 3a20 7374 722c 0a20 2020  ipfile: str,.   
+000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132b0: 2020 2020 2020 2066 696c 7465 725f 6669         filter_fi
+000132c0: 6c65 7479 7065 733a 2073 7472 203d 2022  letypes: str = "
+000132d0: 2a2e 7a61 7272 202a 2e74 6966 6620 2a2e  *.zarr *.tiff *.
+000132e0: 7469 6622 0a20 2020 2020 2020 2020 2020  tif".           
+000132f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00013300: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+00013310: 2022 2222 0a20 2020 2020 2020 2047 656e   """.        Gen
+00013320: 6572 6174 6520 6120 636f 6d6d 616e 6420  erate a command 
+00013330: 7374 7269 6e67 2066 6f72 2075 6e7a 6970  string for unzip
+00013340: 7069 6e67 2061 2064 6174 6120 6172 6368  ping a data arch
+00013350: 6976 6520 616e 6420 6372 6561 7469 6e67  ive and creating
+00013360: 0a20 2020 2020 2020 2072 6571 7569 7265  .        require
+00013370: 6420 6469 7265 6374 6f72 6965 7320 666f  d directories fo
+00013380: 7220 536c 7572 6d20 6a6f 6273 2e0a 0a20  r Slurm jobs... 
+00013390: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000133a0: 2020 2020 2020 2020 207a 6970 6669 6c65           zipfile
+000133b0: 2028 7374 7229 3a20 5468 6520 6e61 6d65   (str): The name
+000133c0: 206f 6620 7468 6520 7a69 7020 6172 6368   of the zip arch
+000133d0: 6976 6520 6669 6c65 2074 6f20 6578 7472  ive file to extr
+000133e0: 6163 742e 0a20 2020 2020 2020 2020 2020  act..           
+000133f0: 2020 2020 2057 6974 686f 7574 2065 7874       Without ext
+00013400: 656e 7369 6f6e 2e0a 2020 2020 2020 2020  ension..        
+00013410: 2020 2020 6669 6c74 6572 5f66 696c 6574      filter_filet
+00013420: 7970 6573 2028 7374 722c 206f 7074 696f  ypes (str, optio
+00013430: 6e61 6c29 3a20 4120 7370 6163 652d 7365  nal): A space-se
+00013440: 7061 7261 7465 6420 7374 7269 6e67 0a20  parated string. 
+00013450: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00013460: 6f6e 7461 696e 696e 6720 7468 6520 6669  ontaining the fi
+00013470: 6c65 2065 7874 656e 7369 6f6e 7320 746f  le extensions to
+00013480: 2065 7874 7261 6374 2066 726f 6d20 7468   extract from th
+00013490: 6520 7a69 7020 6669 6c65 2e0a 2020 2020  e zip file..    
+000134a0: 2020 2020 2020 2020 2020 2020 452e 672e              E.g.
+000134b0: 2064 6566 6175 6c74 7320 746f 2022 2a2e   defaults to "*.
+000134c0: 7a61 7272 202a 2e74 6966 6620 2a2e 7469  zarr *.tiff *.ti
+000134d0: 6622 2e0a 2020 2020 2020 2020 2020 2020  f"..            
+000134e0: 2020 2020 5365 7474 696e 6720 7468 6973      Setting this
+000134f0: 2061 7267 756d 656e 7420 746f 2060 4e6f   argument to `No
+00013500: 6e65 6020 7769 6c6c 206f 6d69 7420 7468  ne` will omit th
+00013510: 6520 6669 6c65 0a20 2020 2020 2020 2020  e file.         
+00013520: 2020 2020 2020 2066 696c 7465 7220 616e         filter an
+00013530: 6420 6578 7472 6163 7420 616c 6c20 6669  d extract all fi
+00013540: 6c65 732e 0a0a 2020 2020 2020 2020 5265  les...        Re
+00013550: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00013560: 2020 2073 7472 3a0a 2020 2020 2020 2020     str:.        
+00013570: 2020 2020 2020 2020 5468 6520 636f 6d6d          The comm
+00013580: 616e 6420 746f 2065 7874 7261 6374 2074  and to extract t
+00013590: 6865 2073 7065 6369 6669 6564 0a20 2020  he specified.   
+000135a0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
+000135b0: 6574 7970 6573 2066 726f 6d20 7468 6520  etypes from the 
+000135c0: 7a69 7020 6669 6c65 2e0a 2020 2020 2020  zip file..      
+000135d0: 2020 2222 220a 2020 2020 2020 2020 756e    """.        un
+000135e0: 7a69 705f 636d 6420 3d20 6622 6d6b 6469  zip_cmd = f"mkdi
+000135f0: 7220 5c22 7b73 656c 662e 736c 7572 6d5f  r \"{self.slurm_
+00013600: 6461 7461 5f70 6174 687d 2f7b 7a69 7066  data_path}/{zipf
+00013610: 696c 657d 5c22 205c 0a20 2020 2020 2020  ile}\" \.       
+00013620: 2020 2020 2020 2020 2020 2020 205c 227b               \"{
+00013630: 7365 6c66 2e73 6c75 726d 5f64 6174 615f  self.slurm_data_
+00013640: 7061 7468 7d2f 7b7a 6970 6669 6c65 7d2f  path}/{zipfile}/
+00013650: 6461 7461 5c22 205c 0a20 2020 2020 2020  data\" \.       
+00013660: 2020 2020 2020 2020 2020 2020 205c 227b               \"{
+00013670: 7365 6c66 2e73 6c75 726d 5f64 6174 615f  self.slurm_data_
+00013680: 7061 7468 7d2f 7b7a 6970 6669 6c65 7d2f  path}/{zipfile}/
+00013690: 6461 7461 2f69 6e5c 2220 5c0a 2020 2020  data/in\" \.    
+000136a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136b0: 5c22 7b73 656c 662e 736c 7572 6d5f 6461  \"{self.slurm_da
+000136c0: 7461 5f70 6174 687d 2f7b 7a69 7066 696c  ta_path}/{zipfil
+000136d0: 657d 2f64 6174 612f 6f75 745c 2220 5c0a  e}/data/out\" \.
+000136e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136f0: 2020 2020 5c22 7b73 656c 662e 736c 7572      \"{self.slur
+00013700: 6d5f 6461 7461 5f70 6174 687d 2f7b 7a69  m_data_path}/{zi
+00013710: 7066 696c 657d 2f64 6174 612f 6774 5c22  pfile}/data/gt\"
+00013720: 3b20 5c0a 2020 2020 2020 2020 2020 2020  ; \.            
+00013730: 2020 2020 2020 2020 377a 2078 202d 7920          7z x -y 
+00013740: 2d6f 5c22 7b73 656c 662e 736c 7572 6d5f  -o\"{self.slurm_
+00013750: 6461 7461 5f70 6174 687d 2f7b 7a69 7066  data_path}/{zipf
+00013760: 696c 657d 2f64 6174 612f 696e 5c22 205c  ile}/data/in\" \
+00013770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013780: 2020 2020 205c 227b 7365 6c66 2e73 6c75       \"{self.slu
+00013790: 726d 5f64 6174 615f 7061 7468 7d2f 7b7a  rm_data_path}/{z
+000137a0: 6970 6669 6c65 7d2e 7a69 705c 2220 7b66  ipfile}.zip\" {f
+000137b0: 696c 7465 725f 6669 6c65 7479 7065 737d  ilter_filetypes}
+000137c0: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+000137d0: 6e20 756e 7a69 705f 636d 640a 0a20 2020  n unzip_cmd..   
+000137e0: 2064 6566 2067 6574 5f69 6d61 6765 5f76   def get_image_v
+000137f0: 6572 7369 6f6e 735f 616e 645f 6461 7461  ersions_and_data
+00013800: 5f66 696c 6573 2873 656c 662c 206d 6f64  _files(self, mod
+00013810: 656c 3a20 7374 720a 2020 2020 2020 2020  el: str.        
+00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013840: 2020 2920 2d3e 2054 7570 6c65 5b4c 6973    ) -> Tuple[Lis
+00013850: 745b 7374 725d 2c20 4c69 7374 5b73 7472  t[str], List[str
+00013860: 5d5d 3a0a 2020 2020 2020 2020 2222 220a  ]]:.        """.
+00013870: 2020 2020 2020 2020 5265 7472 6965 7665          Retrieve
+00013880: 2074 6865 2061 7661 696c 6162 6c65 2069   the available i
+00013890: 6d61 6765 2076 6572 7369 6f6e 7320 616e  mage versions an
+000138a0: 6420 696e 7075 7420 6461 7461 2066 696c  d input data fil
+000138b0: 6573 2066 6f72 2061 0a20 2020 2020 2020  es for a.       
+000138c0: 2067 6976 656e 206d 6f64 656c 2e0a 0a20   given model... 
+000138d0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000138e0: 2020 2020 2020 2020 206d 6f64 656c 2028           model (
+000138f0: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
+00013900: 6620 7468 6520 6d6f 6465 6c20 746f 2071  f the model to q
+00013910: 7565 7279 2066 6f72 2e0a 0a20 2020 2020  uery for...     
+00013920: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00013930: 2020 2020 2020 2020 5475 706c 655b 4c69          Tuple[Li
+00013940: 7374 5b73 7472 5d2c 204c 6973 745b 7374  st[str], List[st
+00013950: 725d 5d3a 0a20 2020 2020 2020 2020 2020  r]]:.           
+00013960: 2020 2020 2041 2074 7570 6c65 2063 6f6e       A tuple con
+00013970: 7461 696e 696e 6720 7477 6f20 6c69 7374  taining two list
+00013980: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00013990: 2020 202d 2054 6865 2066 6972 7374 206c     - The first l
+000139a0: 6973 7420 696e 636c 7564 6573 2074 6865  ist includes the
+000139b0: 2061 7661 696c 6162 6c65 2069 6d61 6765   available image
+000139c0: 2076 6572 7369 6f6e 732c 200a 2020 2020   versions, .    
+000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000139e0: 736f 7274 6564 2069 6e20 6465 7363 656e  sorted in descen
+000139f0: 6469 6e67 206f 7264 6572 2e0a 2020 2020  ding order..    
+00013a00: 2020 2020 2020 2020 2020 2020 2d20 5468              - Th
+00013a10: 6520 7365 636f 6e64 206c 6973 7420 696e  e second list in
+00013a20: 636c 7564 6573 2074 6865 2061 7661 696c  cludes the avail
+00013a30: 6162 6c65 2064 6174 6120 6669 6c65 732e  able data files.
+00013a40: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
+00013a50: 3a0a 2020 2020 2020 2020 2020 2020 5661  :.            Va
+00013a60: 6c75 6545 7272 6f72 3a20 4966 2074 6865  lueError: If the
+00013a70: 2070 726f 7669 6465 6420 6d6f 6465 6c20   provided model 
+00013a80: 6973 206e 6f74 2066 6f75 6e64 2069 6e20  is not found in 
+00013a90: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00013aa0: 2020 2020 536c 7572 6d43 6c69 656e 7427      SlurmClient'
+00013ab0: 7320 6b6e 6f77 6e20 6d6f 6465 6c20 7061  s known model pa
+00013ac0: 7468 732e 0a20 2020 2020 2020 2022 2222  ths..        """
+00013ad0: 0a20 2020 2020 2020 2069 6d61 6765 5f70  .        image_p
+00013ae0: 6174 6820 3d20 7365 6c66 2e73 6c75 726d  ath = self.slurm
+00013af0: 5f6d 6f64 656c 5f70 6174 6873 2e67 6574  _model_paths.get
+00013b00: 286d 6f64 656c 290a 2020 2020 2020 2020  (model).        
+00013b10: 6966 206e 6f74 2069 6d61 6765 5f70 6174  if not image_pat
+00013b20: 683a 0a20 2020 2020 2020 2020 2020 2072  h:.            r
+00013b30: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00013b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013b50: 2066 224e 6f20 7061 7468 206b 6e6f 776e   f"No path known
+00013b60: 2066 6f72 2070 726f 7669 6465 6420 6d6f   for provided mo
+00013b70: 6465 6c20 7b6d 6f64 656c 7d2c 205c 0a20  del {model}, \. 
+00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013b90: 2020 2069 6e20 7b73 656c 662e 736c 7572     in {self.slur
+00013ba0: 6d5f 6d6f 6465 6c5f 7061 7468 737d 2229  m_model_paths}")
+00013bb0: 0a20 2020 2020 2020 2063 6d64 6c69 7374  .        cmdlist
+00013bc0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
+00013bd0: 2073 656c 662e 5f56 4552 5349 4f4e 5f43   self._VERSION_C
+00013be0: 4d44 2e66 6f72 6d61 7428 736c 7572 6d5f  MD.format(slurm_
+00013bf0: 696d 6167 6573 5f70 6174 683d 7365 6c66  images_path=self
+00013c00: 2e73 6c75 726d 5f69 6d61 6765 735f 7061  .slurm_images_pa
+00013c10: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c30: 2020 2020 2020 2020 2069 6d61 6765 5f70           image_p
+00013c40: 6174 683d 696d 6167 655f 7061 7468 292c  ath=image_path),
+00013c50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00013c60: 662e 5f44 4154 415f 434d 442e 666f 726d  f._DATA_CMD.form
+00013c70: 6174 2873 6c75 726d 5f64 6174 615f 7061  at(slurm_data_pa
+00013c80: 7468 3d73 656c 662e 736c 7572 6d5f 6461  th=self.slurm_da
+00013c90: 7461 5f70 6174 6829 5d0a 2020 2020 2020  ta_path)].      
+00013ca0: 2020 2320 7370 6c69 7420 7265 7370 6f6e    # split respon
+00013cb0: 7365 7320 7065 7220 636f 6d6d 616e 640a  ses per command.
+00013cc0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
+00013cd0: 5f6c 6973 7420 3d20 7365 6c66 2e72 756e  _list = self.run
+00013ce0: 5f63 6f6d 6d61 6e64 735f 7370 6c69 745f  _commands_split_
+00013cf0: 6f75 7428 636d 646c 6973 7429 0a20 2020  out(cmdlist).   
+00013d00: 2020 2020 2023 2073 706c 6974 206c 696e       # split lin
+00013d10: 6573 2066 7572 7468 6572 2069 6e74 6f20  es further into 
+00013d20: 7375 626c 6973 7473 0a20 2020 2020 2020  sublists.       
+00013d30: 2072 6573 706f 6e73 655f 6c69 7374 203d   response_list =
+00013d40: 205b 7265 7370 6f6e 7365 2e73 7472 6970   [response.strip
+00013d50: 2829 2e73 706c 6974 2827 5c6e 2729 0a20  ().split('\n'). 
+00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013d70: 2020 2020 2020 2020 666f 7220 7265 7370          for resp
+00013d80: 6f6e 7365 2069 6e20 7265 7370 6f6e 7365  onse in response
+00013d90: 5f6c 6973 745d 0a20 2020 2020 2020 2072  _list].        r
+00013da0: 6573 706f 6e73 655f 6c69 7374 5b30 5d20  esponse_list[0] 
+00013db0: 3d20 736f 7274 6564 2872 6573 706f 6e73  = sorted(respons
+00013dc0: 655f 6c69 7374 5b30 5d2c 2072 6576 6572  e_list[0], rever
+00013dd0: 7365 3d54 7275 6529 0a20 2020 2020 2020  se=True).       
+00013de0: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
+00013df0: 5f6c 6973 745b 305d 2c20 7265 7370 6f6e  _list[0], respon
+00013e00: 7365 5f6c 6973 745b 315d 0a0a 2020 2020  se_list[1]..    
+00013e10: 6465 6620 6765 745f 616c 6c5f 696d 6167  def get_all_imag
+00013e20: 655f 7665 7273 696f 6e73 5f61 6e64 5f64  e_versions_and_d
+00013e30: 6174 615f 6669 6c65 7328 7365 6c66 0a20  ata_files(self. 
+00013e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e60: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+00013e70: 3e20 5475 706c 655b 4469 6374 5b73 7472  > Tuple[Dict[str
+00013e80: 2c20 4c69 7374 5b73 7472 5d5d 2c0a 2020  , List[str]],.  
+00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ec0: 2020 2020 2020 204c 6973 745b 7374 725d         List[str]
+00013ed0: 5d3a 0a20 2020 2020 2020 2022 2222 5265  ]:.        """Re
+00013ee0: 7472 6965 7665 2061 6c6c 2061 7661 696c  trieve all avail
+00013ef0: 6162 6c65 2069 6d61 6765 2076 6572 7369  able image versi
+00013f00: 6f6e 7320 616e 6420 6461 7461 2066 696c  ons and data fil
+00013f10: 6573 2066 726f 6d0a 2020 2020 2020 2020  es from.        
+00013f20: 7468 6520 536c 7572 6d20 636c 7573 7465  the Slurm cluste
+00013f30: 722e 0a0a 2020 2020 2020 2020 5265 7475  r...        Retu
+00013f40: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00013f50: 5475 706c 655b 4469 6374 5b73 7472 2c20  Tuple[Dict[str, 
+00013f60: 4c69 7374 5b73 7472 5d5d 2c20 4c69 7374  List[str]], List
+00013f70: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
+00013f80: 2020 2020 2020 2020 4120 7475 706c 6520          A tuple 
+00013f90: 636f 6e74 6169 6e69 6e67 3a0a 2020 2020  containing:.    
+00013fa0: 2020 2020 2020 2020 2020 2020 2d20 4120              - A 
+00013fb0: 6469 6374 696f 6e61 7279 206d 6170 7069  dictionary mappi
+00013fc0: 6e67 206d 6f64 656c 7320 746f 2061 7661  ng models to ava
+00013fd0: 696c 6162 6c65 2076 6572 7369 6f6e 732e  ilable versions.
+00013fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ff0: 202d 2041 206c 6973 7420 6f66 2061 7661   - A list of ava
+00014000: 696c 6162 6c65 2069 6e70 7574 2064 6174  ilable input dat
+00014010: 6120 666f 6c64 6572 732e 0a20 2020 2020  a folders..     
+00014020: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+00014030: 6573 756c 7464 6963 7420 3d20 7b7d 0a20  esultdict = {}. 
+00014040: 2020 2020 2020 2063 6d64 6c69 7374 203d         cmdlist =
+00014050: 205b 5d0a 0a20 2020 2020 2020 2066 6f72   []..        for
+00014060: 2070 6174 6820 696e 2073 656c 662e 736c   path in self.sl
+00014070: 7572 6d5f 6d6f 6465 6c5f 7061 7468 732e  urm_model_paths.
+00014080: 7661 6c75 6573 2829 3a0a 2020 2020 2020  values():.      
+00014090: 2020 2020 2020 7061 7468 636d 6420 3d20        pathcmd = 
+000140a0: 7365 6c66 2e5f 5645 5253 494f 4e5f 434d  self._VERSION_CM
+000140b0: 442e 666f 726d 6174 280a 2020 2020 2020  D.format(.      
+000140c0: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
+000140d0: 696d 6167 6573 5f70 6174 683d 7365 6c66  images_path=self
+000140e0: 2e73 6c75 726d 5f69 6d61 6765 735f 7061  .slurm_images_pa
+000140f0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00014100: 2020 2020 696d 6167 655f 7061 7468 3d70      image_path=p
+00014110: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
+00014120: 2063 6d64 6c69 7374 2e61 7070 656e 6428   cmdlist.append(
+00014130: 7061 7468 636d 6429 0a0a 2020 2020 2020  pathcmd)..      
+00014140: 2020 2320 4164 6420 6461 7461 2070 6174    # Add data pat
+00014150: 6820 746f 6f0a 2020 2020 2020 2020 636d  h too.        cm
+00014160: 646c 6973 742e 6170 7065 6e64 2873 656c  dlist.append(sel
+00014170: 662e 5f44 4154 415f 434d 442e 666f 726d  f._DATA_CMD.form
+00014180: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
+00014190: 736c 7572 6d5f 6461 7461 5f70 6174 683d  slurm_data_path=
+000141a0: 7365 6c66 2e73 6c75 726d 5f64 6174 615f  self.slurm_data_
+000141b0: 7061 7468 2929 0a0a 2020 2020 2020 2020  path))..        
+000141c0: 2320 5370 6c69 7420 7265 7370 6f6e 7365  # Split response
+000141d0: 7320 7065 7220 636f 6d6d 616e 640a 2020  s per command.  
+000141e0: 2020 2020 2020 7265 7370 6f6e 7365 5f6c        response_l
+000141f0: 6973 7420 3d20 7365 6c66 2e72 756e 5f63  ist = self.run_c
+00014200: 6f6d 6d61 6e64 735f 7370 6c69 745f 6f75  ommands_split_ou
+00014210: 7428 636d 646c 6973 7429 0a0a 2020 2020  t(cmdlist)..    
+00014220: 2020 2020 2320 5370 6c69 7420 6c69 6e65      # Split line
+00014230: 7320 6675 7274 6865 7220 696e 746f 2073  s further into s
+00014240: 7562 6c69 7374 730a 2020 2020 2020 2020  ublists.        
+00014250: 7265 7370 6f6e 7365 5f6c 6973 7420 3d20  response_list = 
+00014260: 5b72 6573 706f 6e73 652e 7374 7269 7028  [response.strip(
+00014270: 292e 7370 6c69 7428 275c 6e27 290a 2020  ).split('\n').  
+00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014290: 2020 2020 2020 2066 6f72 2072 6573 706f         for respo
+000142a0: 6e73 6520 696e 2072 6573 706f 6e73 655f  nse in response_
+000142b0: 6c69 7374 5d0a 0a20 2020 2020 2020 2066  list]..        f
+000142c0: 6f72 2069 2c20 6b20 696e 2065 6e75 6d65  or i, k in enume
+000142d0: 7261 7465 2873 656c 662e 736c 7572 6d5f  rate(self.slurm_
+000142e0: 6d6f 6465 6c5f 7061 7468 7329 3a0a 2020  model_paths):.  
+000142f0: 2020 2020 2020 2020 2020 2320 5265 7475            # Retu
+00014300: 726e 2068 6967 6865 7374 2076 6572 7369  rn highest versi
+00014310: 6f6e 2066 6972 7374 0a20 2020 2020 2020  on first.       
+00014320: 2020 2020 2072 6573 756c 7464 6963 745b       resultdict[
+00014330: 6b5d 203d 2073 6f72 7465 6428 7265 7370  k] = sorted(resp
+00014340: 6f6e 7365 5f6c 6973 745b 695d 2c20 7265  onse_list[i], re
+00014350: 7665 7273 653d 5472 7565 290a 0a20 2020  verse=True)..   
+00014360: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00014370: 6c74 6469 6374 2c20 7265 7370 6f6e 7365  ltdict, response
+00014380: 5f6c 6973 745b 2d31 5d0a                 _list[-1].
```

### Comparing `biomero-1.8.0/biomero.egg-info/PKG-INFO` & `biomero-1.9.0/biomero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomero
-Version: 1.8.0
+Version: 1.9.0
 Summary: A python library for easy connecting between OMERO (jobs) and a Slurm cluster
 Author: Core Facility - Cellular Imaging
 Author-email: Torec Luik <t.t.luik@amsterdamumc.nl>, cellularimaging@amsterdamumc.nl
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -320,16 +320,18 @@
 
     - Congratulations! Now the servers are connected. Next, we make sure to setup the connection between OMERO and Slurm.
 
 3. At this point, ensure that the `slurm-config.ini` file is correctly configured with the necessary SSH and Slurm settings, including the host, data path, images path, and model details. Customize the configuration according to the specific Slurm cluster setup. We provide an example in the [resources](./resources/slurm-config.ini) section. To read it automatically, place this `ini` file in one of the following locations (on the OMERO `processor` server):
     - `/etc/slurm-config.ini`
     - `~/slurm-config.ini`
 
+    *Note*: Make sure to place the `slurm-config.ini` in the target folder at build time of your docker container instead of mounting it at runtime. This is because the library reads the config file at import time, and if it is not found, it will not work.
+
 4. Install OMERO scripts from [OMERO Slurm Scripts](https://github.com/NL-BioImaging/biomero-scripts), e.g. 
-    - `cd OMERO_DIST/lib/scripts`
+    - `cd /opt/omero/server/OMERO.server/lib/scripts`
     - `git clone https://github.com/NL-BioImaging/biomero-scripts.git slurm`
 
 !!*NOTE*: Do not install [Example Minimal Slurm Script](https://github.com/NL-BioImaging/biomero-scripts/blob/master/Example_Minimal_Slurm_Script.py) if you do not trust your users with your Slurm cluster. It has literal Command Injection for the SSH user as a **FEATURE**. 
 
 5. Install [BIOMERO Scripts](https://github.com/NL-BioImaging/biomero-scripts/) requirements, e.g.
     - `python3 -m pip install ezomero==1.1.1 tifffile==2020.9.3` 
     - the [OMERO CLI Zarr plugin](https://github.com/ome/omero-cli-zarr), e.g.
```

### Comparing `biomero-1.8.0/biomero.egg-info/SOURCES.txt` & `biomero-1.9.0/biomero.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/docs/Makefile` & `biomero-1.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/docs/conf.py` & `biomero-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/docs/index.rst` & `biomero-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/docs/make.bat` & `biomero-1.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/pyproject.toml` & `biomero-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/convert_job_array.sh` & `biomero-1.9.0/resources/convert_job_array.sh`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/convert_zarr_to_tiff.py` & `biomero-1.9.0/resources/convert_zarr_to_tiff.py`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/job_template.sh` & `biomero-1.9.0/resources/job_template.sh`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/slurm-config.ini` & `biomero-1.9.0/resources/slurm-config.ini`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/images/Cells.tif` & `biomero-1.9.0/resources/tutorials/images/Cells.tif`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/images/cellexpansion.png` & `biomero-1.9.0/resources/tutorials/images/cellexpansion.png`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/images/gc_allow_ssh.PNG` & `biomero-1.9.0/resources/tutorials/images/gc_allow_ssh.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/images/nuclei_labels.png` & `biomero-1.9.0/resources/tutorials/images/nuclei_labels.png`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/images/webclient_init_env.PNG` & `biomero-1.9.0/resources/tutorials/images/webclient_init_env.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/images/webclient_init_env_done.PNG` & `biomero-1.9.0/resources/tutorials/images/webclient_init_env_done.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/images/webclient_run_cellpose.PNG` & `biomero-1.9.0/resources/tutorials/images/webclient_run_cellpose.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/images/webclient_run_workflow.PNG` & `biomero-1.9.0/resources/tutorials/images/webclient_run_workflow.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/tutorial_Azure_slurm.md` & `biomero-1.9.0/resources/tutorials/tutorial_Azure_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/tutorial_GoogleCloud_slurm.md` & `biomero-1.9.0/resources/tutorials/tutorial_GoogleCloud_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/tutorial_cellexpansion.md` & `biomero-1.9.0/resources/tutorials/tutorial_cellexpansion.md`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/tutorial_cellprofiler.md` & `biomero-1.9.0/resources/tutorials/tutorial_cellprofiler.md`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/resources/tutorials/tutorial_local_slurm.md` & `biomero-1.9.0/resources/tutorials/tutorial_local_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.8.0/tests/unit/test_slurm_client.py` & `biomero-1.9.0/tests/unit/test_slurm_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,21 +87,21 @@
 def test_get_unzip_command(slurm_client):
     # GIVEN
     slurm_data_path = "/path/to/slurm/data"
     slurm_client.slurm_data_path = slurm_data_path
     zipfile = "example"
     filter_filetypes = "*.zarr *.tiff *.tif"
     expected_command = (
-        f"mkdir {slurm_data_path}/{zipfile} \
-                    {slurm_data_path}/{zipfile}/data \
-                    {slurm_data_path}/{zipfile}/data/in \
-                    {slurm_data_path}/{zipfile}/data/out \
-                    {slurm_data_path}/{zipfile}/data/gt; \
-                    7z x -y -o{slurm_data_path}/{zipfile}/data/in \
-                    {slurm_data_path}/{zipfile}.zip {filter_filetypes}"
+        f"mkdir \"{slurm_data_path}/{zipfile}\" \
+                    \"{slurm_data_path}/{zipfile}/data\" \
+                    \"{slurm_data_path}/{zipfile}/data/in\" \
+                    \"{slurm_data_path}/{zipfile}/data/out\" \
+                    \"{slurm_data_path}/{zipfile}/data/gt\"; \
+                    7z x -y -o\"{slurm_data_path}/{zipfile}/data/in\" \
+                    \"{slurm_data_path}/{zipfile}.zip\" {filter_filetypes}"
     )
 
     # WHEN
     unzip_command = slurm_client.get_unzip_command(
         zipfile, filter_filetypes)
 
     # THEN
@@ -145,15 +145,15 @@
     filename = "example_zip"
 
     # WHEN
     result = slurm_client.zip_data_on_slurm_server(data_location, filename)
 
     # THEN
     mock_run_commands.assert_called_once_with(
-        [f"7z a -y {filename} -tzip {data_location}/data/out"], env=None)
+        [f"7z a -y \"{filename}\" -tzip \"{data_location}/data/out\""], env=None)
     assert result.ok is True
     assert result.stdout == ""
     mock_logger.info.assert_called_with(
         f"Zipping {data_location} as {filename} on Slurm")
 
 
 @patch('biomero.slurm_client.logger')
@@ -191,21 +191,21 @@
     slurm_client.slurm_model_images = {"example_workflow": "user/image"}
     slurm_client.slurm_data_path = "/path/to/slurm_data"
     slurm_client.slurm_converters_path = "/path/to/slurm_converters"
     slurm_client.slurm_images_path = "/path/to/slurm_images"
     slurm_client.slurm_script_path = "/path/to/slurm_script"
 
     expected_sbatch_cmd = f"sbatch --param3=value3 --param4=value4 --time={time_limit} --mail-user={email} --output=omero-%j.log \
-            {slurm_client.slurm_script_path}/job_script.sh"
+            \"{slurm_client.slurm_script_path}/job_script.sh\""
     expected_env = {
-        "DATA_PATH": "/path/to/slurm_data/input_data_folder",
-        "IMAGE_PATH": "/path/to/slurm_images/workflow_path",
+        "DATA_PATH": '"/path/to/slurm_data/input_data_folder"',
+        "IMAGE_PATH": '"/path/to/slurm_images/workflow_path"',
         "IMAGE_VERSION": "1.0",
-        "SINGULARITY_IMAGE": "image_1.0.sif",
-        "SCRIPT_PATH": "/path/to/slurm_script",
+        "SINGULARITY_IMAGE": '"image_1.0.sif"',
+        "SCRIPT_PATH": '"/path/to/slurm_script"',
         "PARAM1": "value1",
         "PARAM2": "value2"
     }
 
     # WHEN
     sbatch_cmd, env = slurm_client.get_workflow_command(
         workflow, workflow_version, input_data, email, time_limit, param1="value1", param2="value2")
@@ -225,25 +225,25 @@
     slurm_client.slurm_data_path = "/path/to/slurm_data"
     slurm_client.slurm_converters_path = "/path/to/slurm_converters"
     slurm_client.slurm_script_path = "/path/to/slurm_script"
 
     expected_config_file = f"config_{folder_name}.txt"
     expected_data_path = f"{slurm_client.slurm_data_path}/{folder_name}"
     expected_conversion_cmd, expected_sbatch_env = (
-        "sbatch --job-name=conversion --export=ALL,CONFIG_PATH=\"$PWD/$CONFIG_FILE\" --array=1-$N $SCRIPT_PATH/convert_job_array.sh",
+        "sbatch --job-name=conversion --export=ALL,CONFIG_PATH=\"$PWD/$CONFIG_FILE\" --array=1-$N \"$SCRIPT_PATH/convert_job_array.sh\"",
         {
-            "DATA_PATH": f"{expected_data_path}",
-            "CONVERSION_PATH": f"{slurm_client.slurm_converters_path}",
+            "DATA_PATH": f"\"{expected_data_path}\"",
+            "CONVERSION_PATH": f"\"{slurm_client.slurm_converters_path}\"",
             "CONVERTER_IMAGE": f"convert_{source_format}_to_{target_format}.sif",
-            "SCRIPT_PATH": f"{slurm_client.slurm_script_path}",
-            "CONFIG_FILE": f"{expected_config_file}"
+            "SCRIPT_PATH": f"\"{slurm_client.slurm_script_path}\"",
+            "CONFIG_FILE": f"\"{expected_config_file}\""
         }
     )
     expected_commands = [
-        f"find {expected_data_path}/data/in -name '*.{source_format}' | awk '{{print NR, $0}}' > {expected_config_file}",
+        f"find \"{expected_data_path}/data/in\" -name \"*.{source_format}\" | awk '{{print NR, $0}}' > \"{expected_config_file}\"",
         f"N=$(wc -l < \"{expected_config_file}\")",
         f"echo \"Number of .{source_format} files: $N\"",
         expected_conversion_cmd
     ]
 
     # Mocking the run_commands method to avoid actual execution
     mock_run_commands.return_value = mock_result
@@ -462,15 +462,15 @@
     # WHEN
     with pytest.raises(SSHException):
         _ = slurm_client.extract_data_location_from_log(
             slurm_job_id=slurm_job_id, logfile=logfile)
 
     # THEN
     mock_run_commands.assert_called_with(
-        [f"cat {logfile} | perl -wne '/Running [\\w-]+? Job w\\/ .+? \\| .+? \\| (.+?) \\|.*/i and print$1'"])
+        [f"cat \"{logfile}\" | perl -wne '/Running [\\w-]+? Job w\\/ .+? \\| .+? \\| (.+?) \\|.*/i and print$1'"])
 
 
 @patch('biomero.slurm_client.SlurmClient.run_commands')
 def test_extract_data_location_from_log_2(mock_run_commands,
                                           slurm_client):
     # GIVEN
     slurm_job_id = "123"
@@ -481,15 +481,15 @@
     # WHEN
     data_location = slurm_client.extract_data_location_from_log(
         slurm_job_id=slurm_job_id, logfile=None)
 
     # THEN
     assert data_location == expected_data_location
     mock_run_commands.assert_called_with(
-        [f"cat omero-{slurm_job_id}.log | perl -wne '/Running [\\w-]+? Job w\\/ .+? \\| .+? \\| (.+?) \\|.*/i and print$1'"])
+        [f"cat \"omero-{slurm_job_id}.log\" | perl -wne '/Running [\\w-]+? Job w\\/ .+? \\| .+? \\| (.+?) \\|.*/i and print$1'"])
 
 
 @patch('biomero.slurm_client.SlurmClient.run_commands')
 def test_extract_data_location_from_log(mock_run_commands,
                                         slurm_client):
     # GIVEN
     slurm_job_id = "123"
@@ -501,15 +501,15 @@
     # WHEN
     data_location = slurm_client.extract_data_location_from_log(
         slurm_job_id=slurm_job_id, logfile=logfile)
 
     # THEN
     assert data_location == expected_data_location
     mock_run_commands.assert_called_with(
-        [f"cat {logfile} | perl -wne '/Running [\\w-]+? Job w\\/ .+? \\| .+? \\| (.+?) \\|.*/i and print$1'"])
+        [f"cat \"{logfile}\" | perl -wne '/Running [\\w-]+? Job w\\/ .+? \\| .+? \\| (.+?) \\|.*/i and print$1'"])
 
 
 def test_get_job_status_command(slurm_client):
     # GIVEN
     slurm_job_ids = [123, 456, 789]
 
     # WHEN
@@ -690,15 +690,15 @@
         {'param1': {'cmd_flag': '--param1', 'name': 'param1_name'}})
 
     # Assert that the job script is generated
     mock_generate_job.assert_called_once_with(
         "workflow_name", {'PARAMS': '--param1 $PARAM1_NAME'})
 
     # Assert that the remote directories are created
-    mock_run.assert_called_with("mkdir -p scriptpath")
+    mock_run.assert_called_with("mkdir -p \"scriptpath\"")
 
     # Assert that the job script is copied to the remote location
     mock_put.assert_called_once_with(
         local=mock_stringio("GeneratedJobScript"), remote="scriptpath/job_path")
 
     # Assert the overall behavior
     assert mock_run.call_count == 2  # Two calls, one for mkdir and one for put
@@ -849,19 +849,19 @@
     # WHEN
     result = slurm_client.cleanup_tmp_files(
         slurm_job_id, filename, data_location, logfile)
 
     # THEN
     mock_extract_data_location.assert_not_called()
     mock_run_commands.assert_called_once_with([
-        f"rm {filename}.*",
-        f"rm {logfile}",
-        f"rm slurm-{slurm_job_id}_*.out",
-        f"rm -rf {data_location} {data_location}.*",
-        f"rm config_path.txt"
+        f"rm \"{filename}\".*",
+        f"rm \"{logfile}\"",
+        f"rm \"slurm-{slurm_job_id}\"_*.out",
+        f"rm -rf \"{data_location}\" \"{data_location}\".*",
+        f"rm \"config_path.txt\""
     ], sep=' ; ')
 
     assert result.ok is True
 
 
 @patch('biomero.slurm_client.SlurmClient.run_commands')
 @patch('biomero.slurm_client.SlurmClient.extract_data_location_from_log')
@@ -883,19 +883,19 @@
     # WHEN
     result = slurm_client.cleanup_tmp_files(
         slurm_job_id, filename, data_location, logfile)
 
     # THEN
     mock_extract_data_location.assert_called_once_with(logfile)
     mock_run_commands.assert_called_once_with([
-        f"rm {filename}.*",
-        f"rm {logfile}",
-        f"rm slurm-{slurm_job_id}_*.out",
-        f"rm -rf {found_location} {found_location}.*",
-        f"rm config_path.txt"
+        f"rm \"{filename}\".*",
+        f"rm \"{logfile}\"",
+        f"rm \"slurm-{slurm_job_id}\"_*.out",
+        f"rm -rf \"{found_location}\" \"{found_location}\".*",
+        f"rm \"config_path.txt\""
     ], sep=' ; ')
 
     assert result.ok is True
 
 
 @patch('biomero.slurm_client.Connection.create_session')
 @patch('biomero.slurm_client.Connection.open')
@@ -999,15 +999,15 @@
     with pytest.raises(SSHException):
         slurm_client.setup_slurm()
 
     # THEN
     # 1 create dirs
     mock_run.assert_called()
     mock_run.assert_any_call(
-        f'mkdir -p {dpath} && mkdir -p {spath} && mkdir -p {ipath}', env={})
+        f"mkdir -p \"{dpath}\" && mkdir -p \"{spath}\" && mkdir -p \"{ipath}\"", env={})
 
 
 @patch('biomero.slurm_client.io.StringIO')
 @patch('biomero.slurm_client.SlurmClient.validate')
 @patch('biomero.slurm_client.SlurmClient.run_commands')
 @patch('biomero.slurm_client.Connection.open')
 @patch('biomero.slurm_client.Connection.put')
@@ -1049,28 +1049,28 @@
     # WHEN
     slurm_client.setup_slurm()
 
     # THEN
     mock_run.assert_called()
     # 1 create dirs
     mock_run.assert_any_call(
-        [f'mkdir -p {dpath}', f'mkdir -p {spath}', f'mkdir -p {ipath}'])
-    # 2 git
+        [f"mkdir -p \"{dpath}\"", f"mkdir -p \"{spath}\"", f"mkdir -p \"{ipath}\""])
+    # 2 git 
     mock_run.assert_any_call(
-        ['git clone "$REPOSRC" "$LOCALREPO" 2> /dev/null || git -C "$LOCALREPO" pull'],
-        {"REPOSRC": srepo, "LOCALREPO": spath})
+        ['rm -rf "$LOCALREPO"', 'git clone "$REPOSRC" "$LOCALREPO" 2> /dev/null'],
+        {"REPOSRC": f"\"{srepo}\"", "LOCALREPO": f"\"{spath}\""})
 
     # 3 converters
     _mock_Connection_put.assert_called()
     # mock_run.assert_any_call(f"mkdir -p {cpath}")
     mock_run.assert_any_call(
-        [f"singularity build -F {convert_name}.sif {convert_def} >> sing.log 2>&1 ; echo 'finished {convert_name}.sif' &"])
+        [f"singularity build -F \"{convert_name}.sif\" {convert_def} >> sing.log 2>&1 ; echo 'finished {convert_name}.sif' &"])
 
     # 4 images
-    mock_run.assert_any_call([f"mkdir -p {modelpaths}"])
+    mock_run.assert_any_call([f"mkdir -p \"{modelpaths}\""])
     _mock_Connection_put.assert_called_with(
         local=mock_stringio(), remote=f'{ipath}/{script_name}')
     mock_run.assert_any_call([f"time sh {script_name}"])
 
 
 @patch('biomero.slurm_client.SlurmClient.run')
 @patch('biomero.slurm_client.SlurmClient.setup_slurm')
```

