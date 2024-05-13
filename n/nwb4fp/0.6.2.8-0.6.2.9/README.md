# Comparing `tmp/nwb4fp-0.6.2.8.tar.gz` & `tmp/nwb4fp-0.6.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.2.8.tar", last modified: Mon May 13 12:54:33 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.2.9.tar", last modified: Mon May 13 13:46:27 2024, max compression
```

## Comparing `nwb4fp-0.6.2.8.tar` & `nwb4fp-0.6.2.9.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 12:54:33.651337 nwb4fp-0.6.2.8/
--rw-rw-rw-   0        0        0     1089 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/LICENSE
--rw-rw-rw-   0        0        0     5755 2024-05-13 12:54:33.645334 nwb4fp-0.6.2.8/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 12:54:33.666340 nwb4fp-0.6.2.8/setup.cfg
--rw-rw-rw-   0        0        0      886 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:54:33.026336 nwb4fp-0.6.2.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 12:54:33.043335 nwb4fp-0.6.2.8/src/nwb4fp/
-drwxrwxrwx   0        0        0        0 2024-05-13 12:54:33.034336 nwb4fp-0.6.2.8/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:54:33.038340 nwb4fp-0.6.2.8/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1850 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/postprocess/lfp_channel.py
--rw-rw-rw-   0        0        0    17084 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    14469 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:54:33.043335 nwb4fp-0.6.2.8/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     8242 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:54:33.048344 nwb4fp-0.6.2.8/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-05-13 12:54:33.050344 nwb4fp-0.6.2.8/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1525 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1054 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0     1448 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/test/run_scripts/readnwb_09PD.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/test/run_scripts/test.py
--rw-rw-rw-   0        0        0     5828 2024-05-13 12:41:11.000000 nwb4fp-0.6.2.8/src/nwb4fp/test/run_scripts/test_lfp.py
-drwxrwxrwx   0        0        0        0 2024-05-13 12:54:33.026336 nwb4fp-0.6.2.8/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5755 2024-05-13 12:54:32.000000 nwb4fp-0.6.2.8/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1099 2024-05-13 12:54:32.000000 nwb4fp-0.6.2.8/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 12:54:32.000000 nwb4fp-0.6.2.8/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2892 2024-05-13 12:54:32.000000 nwb4fp-0.6.2.8/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 12:54:32.000000 nwb4fp-0.6.2.8/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 13:46:27.340115 nwb4fp-0.6.2.9/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.2.9/LICENSE
+-rw-rw-rw-   0        0        0     5732 2024-05-13 13:46:27.330112 nwb4fp-0.6.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.2.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 13:46:27.358112 nwb4fp-0.6.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      886 2024-05-13 13:43:36.000000 nwb4fp-0.6.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:46:26.809126 nwb4fp-0.6.2.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 13:46:26.866115 nwb4fp-0.6.2.9/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.2.9/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:46:26.813114 nwb4fp-0.6.2.9/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.2.9/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-04-29 14:40:24.000000 nwb4fp-0.6.2.9/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:46:27.108113 nwb4fp-0.6.2.9/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.2.9/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.2.9/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1850 2024-05-06 11:49:17.000000 nwb4fp-0.6.2.9/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.2.9/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.2.9/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.2.9/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 10:27:15.000000 nwb4fp-0.6.2.9/src/nwb4fp/postprocess/lfp_channel.py
+-rw-rw-rw-   0        0        0    17084 2024-04-29 14:39:46.000000 nwb4fp-0.6.2.9/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    14469 2024-05-13 10:52:36.000000 nwb4fp-0.6.2.9/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:46:27.223113 nwb4fp-0.6.2.9/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.9/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.9/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.9/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8242 2024-05-06 12:27:58.000000 nwb4fp-0.6.2.9/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.9/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.9/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.9/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.2.9/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:46:26.829119 nwb4fp-0.6.2.9/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-05-13 13:46:26.829119 nwb4fp-0.6.2.9/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1525 2024-05-08 11:40:42.000000 nwb4fp-0.6.2.9/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1054 2024-05-08 19:32:57.000000 nwb4fp-0.6.2.9/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0     1448 2024-05-07 08:56:13.000000 nwb4fp-0.6.2.9/src/nwb4fp/test/run_scripts/readnwb_09PD.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.2.9/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.2.9/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:46:26.942113 nwb4fp-0.6.2.9/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5732 2024-05-13 13:46:26.000000 nwb4fp-0.6.2.9/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1122 2024-05-13 13:46:26.000000 nwb4fp-0.6.2.9/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 13:46:26.000000 nwb4fp-0.6.2.9/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2885 2024-05-13 13:46:26.000000 nwb4fp-0.6.2.9/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 13:46:26.000000 nwb4fp-0.6.2.9/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.2.8/LICENSE` & `nwb4fp-0.6.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/PKG-INFO` & `nwb4fp-0.6.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.2.8
+Version: 0.6.2.9
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
@@ -165,8 +165,7 @@
 Requires-Dist: websocket-client==1.7.0
 Requires-Dist: wheel==0.41.2
 Requires-Dist: wrapt==1.16.0
 Requires-Dist: xmltodict==0.13.0
 Requires-Dist: yarl==1.9.4
 Requires-Dist: zarr==2.17.0
 Requires-Dist: zipp==3.17.0
-Requires-Dist: nwb4fp
```

### Comparing `nwb4fp-0.6.2.8/README.md` & `nwb4fp-0.6.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/setup.py` & `nwb4fp-0.6.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.2.8',
+    version='0.6.2.9',
     url='https://github.com/sachuriga/QuattrocoloLab-nwb4fp',
     author='sachuriga',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.2.9/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.2.9/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.2.9/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.2.9/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.2.9/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.2.9/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.2.9/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.2.9/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.2.9/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.2.9/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.2.9/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.2.9/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.2.9/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/test/run_scripts/readnwb_09PD.py` & `nwb4fp-0.6.2.9/src/nwb4fp/test/run_scripts/readnwb_09PD.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp/test/run_scripts/test_lfp.py` & `nwb4fp-0.6.2.9/src/nwb4fp/test/run_scripts/test_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.2.9/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.2.8
+Version: 0.6.2.9
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
@@ -165,8 +165,7 @@
 Requires-Dist: websocket-client==1.7.0
 Requires-Dist: wheel==0.41.2
 Requires-Dist: wrapt==1.16.0
 Requires-Dist: xmltodict==0.13.0
 Requires-Dist: yarl==1.9.4
 Requires-Dist: zarr==2.17.0
 Requires-Dist: zipp==3.17.0
-Requires-Dist: nwb4fp
```

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.2.9/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 setup.py
+src/nwb4fp/__init__.py
 src/nwb4fp.egg-info/PKG-INFO
 src/nwb4fp.egg-info/SOURCES.txt
 src/nwb4fp.egg-info/dependency_links.txt
 src/nwb4fp.egg-info/requires.txt
 src/nwb4fp.egg-info/top_level.txt
 src/nwb4fp/main/__init__.py
 src/nwb4fp/main/main_create_nwb.py
```

### Comparing `nwb4fp-0.6.2.8/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.2.9/src/nwb4fp.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -157,8 +157,7 @@
 websocket-client==1.7.0
 wheel==0.41.2
 wrapt==1.16.0
 xmltodict==0.13.0
 yarl==1.9.4
 zarr==2.17.0
 zipp==3.17.0
-nwb4fp
```

