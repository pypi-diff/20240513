# Comparing `tmp/vis_analysis_torch-0.4.3.tar.gz` & `tmp/vis_analysis_torch-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vis_analysis_torch-0.4.3.tar", last modified: Wed May  8 08:20:07 2024, max compression
+gzip compressed data, was "vis_analysis_torch-0.4.4.tar", last modified: Mon May 13 11:50:15 2024, max compression
```

## Comparing `vis_analysis_torch-0.4.3.tar` & `vis_analysis_torch-0.4.4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:20:07.770544 vis_analysis_torch-0.4.3/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 08:20:07.766544 vis_analysis_torch-0.4.3/PKG-INFO
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       38 2024-05-08 08:20:07.770544 vis_analysis_torch-0.4.3/setup.cfg
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      498 2024-05-08 08:20:01.000000 vis_analysis_torch-0.4.3/setup.py
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:20:07.766544 vis_analysis_torch-0.4.3/vis_analysis_torch/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 03:28:25.000000 vis_analysis_torch-0.4.3/vis_analysis_torch/__init__.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     3340 2024-05-08 08:19:44.000000 vis_analysis_torch-0.4.3/vis_analysis_torch/bbox_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     1569 2024-05-08 08:15:40.000000 vis_analysis_torch-0.4.3/vis_analysis_torch/common_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     7371 2024-05-08 08:19:55.000000 vis_analysis_torch-0.4.3/vis_analysis_torch/pose_visualization.py
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     2776 2024-05-08 07:55:53.000000 vis_analysis_torch-0.4.3/vis_analysis_torch/utils.py
-drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 08:20:07.766544 vis_analysis_torch-0.4.3/vis_analysis_torch.egg-info/
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-08 08:20:07.000000 vis_analysis_torch-0.4.3/vis_analysis_torch.egg-info/PKG-INFO
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      401 2024-05-08 08:20:07.000000 vis_analysis_torch-0.4.3/vis_analysis_torch.egg-info/SOURCES.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        1 2024-05-08 08:20:07.000000 vis_analysis_torch-0.4.3/vis_analysis_torch.egg-info/dependency_links.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       26 2024-05-08 08:20:07.000000 vis_analysis_torch-0.4.3/vis_analysis_torch.egg-info/requires.txt
--rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       19 2024-05-08 08:20:07.000000 vis_analysis_torch-0.4.3/vis_analysis_torch.egg-info/top_level.txt
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-13 11:50:15.127332 vis_analysis_torch-0.4.4/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-13 11:50:15.127332 vis_analysis_torch-0.4.4/PKG-INFO
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       38 2024-05-13 11:50:15.127332 vis_analysis_torch-0.4.4/setup.cfg
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      498 2024-05-13 11:49:45.000000 vis_analysis_torch-0.4.4/setup.py
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-13 11:50:15.127332 vis_analysis_torch-0.4.4/vis_analysis_torch/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        0 2024-05-08 03:28:25.000000 vis_analysis_torch-0.4.4/vis_analysis_torch/__init__.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     3340 2024-05-08 08:19:44.000000 vis_analysis_torch-0.4.4/vis_analysis_torch/bbox_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     1569 2024-05-08 08:15:40.000000 vis_analysis_torch-0.4.4/vis_analysis_torch/common_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     7371 2024-05-08 08:19:55.000000 vis_analysis_torch-0.4.4/vis_analysis_torch/pose_visualization.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     2438 2024-05-13 11:49:34.000000 vis_analysis_torch-0.4.4/vis_analysis_torch/results_analysis.py
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)     2776 2024-05-08 07:55:53.000000 vis_analysis_torch-0.4.4/vis_analysis_torch/utils.py
+drwxrwxr-x   0 chenyang  (1006) chenyang  (1006)        0 2024-05-13 11:50:15.127332 vis_analysis_torch-0.4.4/vis_analysis_torch.egg-info/
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      332 2024-05-13 11:50:15.000000 vis_analysis_torch-0.4.4/vis_analysis_torch.egg-info/PKG-INFO
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)      440 2024-05-13 11:50:15.000000 vis_analysis_torch-0.4.4/vis_analysis_torch.egg-info/SOURCES.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)        1 2024-05-13 11:50:15.000000 vis_analysis_torch-0.4.4/vis_analysis_torch.egg-info/dependency_links.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       26 2024-05-13 11:50:15.000000 vis_analysis_torch-0.4.4/vis_analysis_torch.egg-info/requires.txt
+-rw-rw-r--   0 chenyang  (1006) chenyang  (1006)       19 2024-05-13 11:50:15.000000 vis_analysis_torch-0.4.4/vis_analysis_torch.egg-info/top_level.txt
```

### Comparing `vis_analysis_torch-0.4.3/vis_analysis_torch/bbox_visualization.py` & `vis_analysis_torch-0.4.4/vis_analysis_torch/bbox_visualization.py`

 * *Files identical despite different names*

### Comparing `vis_analysis_torch-0.4.3/vis_analysis_torch/common_visualization.py` & `vis_analysis_torch-0.4.4/vis_analysis_torch/common_visualization.py`

 * *Files identical despite different names*

### Comparing `vis_analysis_torch-0.4.3/vis_analysis_torch/pose_visualization.py` & `vis_analysis_torch-0.4.4/vis_analysis_torch/pose_visualization.py`

 * *Files identical despite different names*

### Comparing `vis_analysis_torch-0.4.3/vis_analysis_torch/utils.py` & `vis_analysis_torch-0.4.4/vis_analysis_torch/utils.py`

 * *Files identical despite different names*

