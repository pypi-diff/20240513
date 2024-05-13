# Comparing `tmp/GSG-0.5.5.tar.gz` & `tmp/GSG-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GSG-0.5.5.tar", last modified: Wed May  1 01:59:47 2024, max compression
+gzip compressed data, was "dist/GSG-0.5.6.tar", last modified: Mon May 13 12:59:24 2024, max compression
```

## Comparing `GSG-0.5.5.tar` & `GSG-0.5.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-01 01:59:47.000000 GSG-0.5.5/
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2941 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/SOURCES.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/dependency_links.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      223 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/requires.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-05-01 01:59:47.000000 GSG-0.5.5/GSG.egg-info/top_level.txt
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    40597 2024-04-18 05:21:38.000000 GSG-0.5.5/GSG.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2941 2024-05-01 01:59:47.000000 GSG-0.5.5/PKG-INFO
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     2764 2024-05-01 01:59:10.000000 GSG-0.5.5/README.md
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-01 01:59:47.000000 GSG-0.5.5/datasets/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.5.5/datasets/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.5.5/datasets/data_util.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-01 01:59:47.000000 GSG-0.5.5/models/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.5.5/models/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.5.5/models/dot_gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.5.5/models/edcoder.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.5.5/models/gat.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.5.5/models/gcn.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.5.5/models/gin.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.5.5/models/loss_func.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-05-01 01:59:47.000000 GSG-0.5.5/setup.cfg
--rw-r--r--   0 wuzhipeng   (501) staff       (20)      809 2024-05-01 01:59:39.000000 GSG-0.5.5/setup.py
-drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-01 01:59:47.000000 GSG-0.5.5/tools/
--rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.5.5/tools/__init__.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.5.5/tools/batch_remove.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.5.5/tools/evaluation.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.5.5/tools/parameters_dict.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.5.5/tools/test.py
--rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.5.5/tools/utils.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-13 12:59:24.000000 GSG-0.5.6/
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-13 12:59:24.000000 GSG-0.5.6/GSG.egg-info/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2941 2024-05-13 12:59:24.000000 GSG-0.5.6/GSG.egg-info/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      433 2024-05-13 12:59:24.000000 GSG-0.5.6/GSG.egg-info/SOURCES.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        1 2024-05-13 12:59:24.000000 GSG-0.5.6/GSG.egg-info/dependency_links.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      223 2024-05-13 12:59:24.000000 GSG-0.5.6/GSG.egg-info/requires.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       26 2024-05-13 12:59:24.000000 GSG-0.5.6/GSG.egg-info/top_level.txt
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    40714 2024-05-13 12:37:54.000000 GSG-0.5.6/GSG.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2941 2024-05-13 12:59:24.000000 GSG-0.5.6/PKG-INFO
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     2764 2024-05-01 01:59:10.000000 GSG-0.5.6/README.md
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-13 12:59:24.000000 GSG-0.5.6/datasets/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:19.000000 GSG-0.5.6/datasets/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6259 2024-04-10 02:47:19.000000 GSG-0.5.6/datasets/data_util.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-13 12:59:24.000000 GSG-0.5.6/models/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1306 2024-04-10 02:47:17.000000 GSG-0.5.6/models/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8563 2024-04-10 08:40:14.000000 GSG-0.5.6/models/dot_gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8671 2024-04-10 08:40:14.000000 GSG-0.5.6/models/edcoder.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    11586 2024-04-10 08:40:14.000000 GSG-0.5.6/models/gat.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     6121 2024-04-10 08:40:14.000000 GSG-0.5.6/models/gcn.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7279 2024-04-10 08:40:14.000000 GSG-0.5.6/models/gin.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      514 2024-04-10 02:47:16.000000 GSG-0.5.6/models/loss_func.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)       38 2024-05-13 12:59:24.000000 GSG-0.5.6/setup.cfg
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)      809 2024-05-13 12:59:21.000000 GSG-0.5.6/setup.py
+drwxr-xr-x   0 wuzhipeng   (501) staff       (20)        0 2024-05-13 12:59:24.000000 GSG-0.5.6/tools/
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)        0 2024-04-10 02:47:15.000000 GSG-0.5.6/tools/__init__.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    13887 2024-04-11 00:48:10.000000 GSG-0.5.6/tools/batch_remove.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     7188 2024-04-10 08:40:14.000000 GSG-0.5.6/tools/evaluation.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     1210 2024-04-10 02:47:16.000000 GSG-0.5.6/tools/parameters_dict.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)     8007 2024-04-10 02:47:15.000000 GSG-0.5.6/tools/test.py
+-rw-r--r--   0 wuzhipeng   (501) staff       (20)    15345 2024-04-11 01:04:23.000000 GSG-0.5.6/tools/utils.py
```

### Comparing `GSG-0.5.5/GSG.egg-info/PKG-INFO` & `GSG-0.5.6/GSG.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GSG
-Version: 0.5.5
+Version: 0.5.6
 Home-page: https://github.com/keaml-Guan/GSG
 License: MIT Licence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # GSG: A generative self-supervised graph learning framework for spatial transcriptomics
 ![GitHub Repo stars](https://img.shields.io/github/stars/keaml-Guan/GSG?style=social) ![GitHub forks](https://img.shields.io/github/forks/keaml-Guan/GSG?style=social) ![GitHub watchers](https://img.shields.io/github/watchers/keaml-Guan/GSG?style=social)
```

### Comparing `GSG-0.5.5/GSG.py` & `GSG-0.5.6/GSG.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,34 +85,34 @@
     parser.add_argument("--sample_name", type=str, default="151673")
     parser.add_argument("--cluster_label", type=str, default= "")
     parser.add_argument("--num_classes", type=int, default=7,help = "The number of clusters")
     # read parameters
     args = parser.parse_args(args=[])
     return args
 
-def GSG_Spatial_Pic(adata,args, result_file_path):
+def GSG_Spatial_Pic(adata,args, result_file_path, is_show = False, is_save = True, spatial_figname = "/GSG_Cluster_Spatial.pdf", ground_truth_figname = "/Ground_true.pdf"):
     if(args.cluster_label != ""):
         adata.obs[args.cluster_label] = adata.obs[args.cluster_label].astype('category').cat.add_categories(['None'])
         adata.obs[args.cluster_label] = adata.obs[args.cluster_label].fillna("None")
-        drawPicture(adata.obs,col_name ="imagecol",row_name = "imagerow",colorattribute=args.cluster_label,save_file = result_file_path + "/Ground_true.pdf",is_show=False,is_save= True)
-        drawPicture(adata.obs,col_name ="imagecol",row_name = "imagerow",colorattribute="GSG_Kmeans_cluster_str",save_file = result_file_path + "/GSG_Cluster_Spatial.pdf",is_show=False,is_save= True)
+        drawPicture(adata.obs,col_name ="imagecol",row_name = "imagerow",colorattribute=args.cluster_label,save_file = result_file_path + ground_truth_figname,is_show=is_show,is_save= is_save)
+        drawPicture(adata.obs,col_name ="imagecol",row_name = "imagerow",colorattribute="GSG_Kmeans_cluster_str",save_file = result_file_path + spatial_figname,is_show=is_show,is_save= is_save)
         k_means_score_ari = adjusted_rand_score(adata.obs["GSG_Kmeans_cluster_str"].values, adata.obs[args.cluster_label].values)
         k_means_score_silhouette = silhouette_score(adata.obsm["GSG_embedding"], adata.obs["GSG_Kmeans_cluster_str"].values, metric="sqeuclidean")
         k_means_score_nmi = normalized_mutual_info_score(adata.obs["GSG_Kmeans_cluster_str"].values, adata.obs[args.cluster_label].values)
         k_means_score_fmi = fowlkes_mallows_score(adata.obs["GSG_Kmeans_cluster_str"].values, adata.obs[args.cluster_label].values)
         k_means_score_DB = davies_bouldin_score(adata.obsm["GSG_embedding"], adata.obs["GSG_Kmeans_cluster_str"].values)
         k_means_score_chs = calinski_harabasz_score(adata.obsm["GSG_embedding"], adata.obs["GSG_Kmeans_cluster_str"].values)
         print("k_means_score_ari:" + str(k_means_score_ari))
         print("k_means_score_silhouette:" + str(k_means_score_silhouette))
         print("k_means_score_nmi:" + str(k_means_score_nmi))
         print("k_means_score_fmi:" + str(k_means_score_fmi))
         print("k_means_score_DB:" + str(k_means_score_DB))
         print("k_means_score_chs:" + str(k_means_score_chs))
     else:
-        drawPicture(adata.obs,col_name ="imagecol",row_name = "imagerow",colorattribute="GSG_Kmeans_cluster_str",save_file = result_file_path + "/GSG_Cluster_Spatial.pdf",is_show=False,is_save= True)
+        drawPicture(adata.obs,col_name ="imagecol",row_name = "imagerow",colorattribute="GSG_Kmeans_cluster_str",save_file = result_file_path + spatial_figname,is_show=is_show,is_save= is_save)
         k_means_score_silhouette = silhouette_score(adata.obsm["GSG_embedding"], adata.obs["GSG_Kmeans_cluster_str"].values, metric="sqeuclidean")
         k_means_score_DB = davies_bouldin_score(adata.obsm["GSG_embedding"], adata.obs["GSG_Kmeans_cluster_str"].values)
         k_means_score_chs = calinski_harabasz_score(adata.obsm["GSG_embedding"], adata.obs["GSG_Kmeans_cluster_str"].values)
         print("k_means_score_silhouette:" + str(k_means_score_silhouette))
         print("k_means_score_DB:" + str(k_means_score_DB))
         print("k_means_score_chs:" + str(k_means_score_chs))
     return adata
```

### Comparing `GSG-0.5.5/PKG-INFO` & `GSG-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GSG
-Version: 0.5.5
+Version: 0.5.6
 Home-page: https://github.com/keaml-Guan/GSG
 License: MIT Licence
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # GSG: A generative self-supervised graph learning framework for spatial transcriptomics
 ![GitHub Repo stars](https://img.shields.io/github/stars/keaml-Guan/GSG?style=social) ![GitHub forks](https://img.shields.io/github/forks/keaml-Guan/GSG?style=social) ![GitHub watchers](https://img.shields.io/github/watchers/keaml-Guan/GSG?style=social)
```

### Comparing `GSG-0.5.5/README.md` & `GSG-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/datasets/data_util.py` & `GSG-0.5.6/datasets/data_util.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/models/__init__.py` & `GSG-0.5.6/models/__init__.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/models/dot_gat.py` & `GSG-0.5.6/models/dot_gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/models/edcoder.py` & `GSG-0.5.6/models/edcoder.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/models/gat.py` & `GSG-0.5.6/models/gat.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/models/gcn.py` & `GSG-0.5.6/models/gcn.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/models/gin.py` & `GSG-0.5.6/models/gin.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/models/loss_func.py` & `GSG-0.5.6/models/loss_func.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/setup.py` & `GSG-0.5.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import os
 
 setup(
     name = 'GSG',
-    version='0.5.5',
+    version='0.5.6',
     packages=find_packages(),
     python_requires='>=3.8',
     py_modules=['GSG'],
     long_description=open(os.path.join("./","README.md"), encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     license="MIT Licence",
     url="https://github.com/keaml-Guan/GSG",
```

### Comparing `GSG-0.5.5/tools/batch_remove.py` & `GSG-0.5.6/tools/batch_remove.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/tools/evaluation.py` & `GSG-0.5.6/tools/evaluation.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/tools/parameters_dict.py` & `GSG-0.5.6/tools/parameters_dict.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/tools/test.py` & `GSG-0.5.6/tools/test.py`

 * *Files identical despite different names*

### Comparing `GSG-0.5.5/tools/utils.py` & `GSG-0.5.6/tools/utils.py`

 * *Files identical despite different names*

