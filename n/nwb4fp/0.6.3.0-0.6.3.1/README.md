# Comparing `tmp/nwb4fp-0.6.3.0.tar.gz` & `tmp/nwb4fp-0.6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.3.0.tar", last modified: Mon May 13 14:51:03 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.3.1.tar", last modified: Mon May 13 15:01:37 2024, max compression
```

## Comparing `nwb4fp-0.6.3.0.tar` & `nwb4fp-0.6.3.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:51:03.148862 nwb4fp-0.6.3.0/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.6.3.0/LICENSE
--rw-rw-rw-   0        0        0     5732 2024-05-13 14:51:03.140868 nwb4fp-0.6.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.6.3.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 14:51:03.164887 nwb4fp-0.6.3.0/setup.cfg
--rw-rw-rw-   0        0        0      886 2024-05-13 14:50:56.000000 nwb4fp-0.6.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:51:02.325862 nwb4fp-0.6.3.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 14:51:02.360870 nwb4fp-0.6.3.0/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.6.3.0/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:51:02.350864 nwb4fp-0.6.3.0/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.6.3.0/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-04-29 14:40:24.000000 nwb4fp-0.6.3.0/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:51:02.355868 nwb4fp-0.6.3.0/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.6.3.0/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.6.3.0/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1850 2024-05-06 11:49:17.000000 nwb4fp-0.6.3.0/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.6.3.0/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.6.3.0/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-04-23 15:19:46.000000 nwb4fp-0.6.3.0/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0        0 2024-05-13 10:27:15.000000 nwb4fp-0.6.3.0/src/nwb4fp/postprocess/lfp_channel.py
--rw-rw-rw-   0        0        0    17084 2024-04-29 14:39:46.000000 nwb4fp-0.6.3.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    14469 2024-05-13 10:52:36.000000 nwb4fp-0.6.3.0/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:51:02.360870 nwb4fp-0.6.3.0/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.6.3.0/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.6.3.0/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.6.3.0/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     8249 2024-05-13 14:50:49.000000 nwb4fp-0.6.3.0/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.6.3.0/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.6.3.0/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.6.3.0/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.6.3.0/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:51:02.368861 nwb4fp-0.6.3.0/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-05-13 14:51:02.368861 nwb4fp-0.6.3.0/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1525 2024-05-08 11:40:42.000000 nwb4fp-0.6.3.0/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1054 2024-05-08 19:32:57.000000 nwb4fp-0.6.3.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0     1448 2024-05-07 08:56:13.000000 nwb4fp-0.6.3.0/src/nwb4fp/test/run_scripts/readnwb_09PD.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.6.3.0/src/nwb4fp/test/run_scripts/test.py
--rw-rw-rw-   0        0        0     5828 2024-04-29 13:35:22.000000 nwb4fp-0.6.3.0/src/nwb4fp/test/run_scripts/test_lfp.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:51:02.551863 nwb4fp-0.6.3.0/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5732 2024-05-13 14:51:02.000000 nwb4fp-0.6.3.0/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2024-05-13 14:51:02.000000 nwb4fp-0.6.3.0/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:51:02.000000 nwb4fp-0.6.3.0/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2885 2024-05-13 14:51:02.000000 nwb4fp-0.6.3.0/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 14:51:02.000000 nwb4fp-0.6.3.0/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:37.407803 nwb4fp-0.6.3.1/
+-rw-rw-rw-   0        0        0     1089 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/LICENSE
+-rw-rw-rw-   0        0        0     5732 2024-05-13 15:01:37.378800 nwb4fp-0.6.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 15:01:37.409801 nwb4fp-0.6.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      886 2024-05-13 14:58:50.000000 nwb4fp-0.6.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.712802 nwb4fp-0.6.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.728802 nwb4fp-0.6.3.1/src/nwb4fp/
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.870807 nwb4fp-0.6.3.1/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:37.033805 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1850 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/lfp_channel.py
+-rw-rw-rw-   0        0        0    17084 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    14469 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.723804 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8249 2024-05-13 14:58:38.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.730803 nwb4fp-0.6.3.1/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:37.328801 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1525 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1028 2024-05-13 13:05:19.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_0283.py
+-rw-rw-rw-   0        0        0     1054 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0     1448 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_09PD.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.841806 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5732 2024-05-13 15:01:36.000000 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1143 2024-05-13 15:01:36.000000 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 15:01:36.000000 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2885 2024-05-13 15:01:36.000000 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-13 15:01:36.000000 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.3.0/LICENSE` & `nwb4fp-0.6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/PKG-INFO` & `nwb4fp-0.6.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.3.0
+Version: 0.6.3.1
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.3.0/README.md` & `nwb4fp-0.6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/setup.py` & `nwb4fp-0.6.3.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.3.0',
+    version='0.6.3.1',
     url='https://github.com/sachuriga/QuattrocoloLab-nwb4fp',
     author='sachuriga',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.3.1/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.3.1/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.3.1/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.3.1/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.3.1/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/test/run_scripts/readnwb_09PD.py` & `nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_09PD.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp/test/run_scripts/test_lfp.py` & `nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/test_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.3.1/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.3.0
+Version: 0.6.3.1
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.3.1/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 README.md
 setup.py
-src/nwb4fp/__init__.py
 src/nwb4fp.egg-info/PKG-INFO
 src/nwb4fp.egg-info/SOURCES.txt
 src/nwb4fp.egg-info/dependency_links.txt
 src/nwb4fp.egg-info/requires.txt
 src/nwb4fp.egg-info/top_level.txt
 src/nwb4fp/main/__init__.py
 src/nwb4fp/main/main_create_nwb.py
@@ -23,11 +22,12 @@
 src/nwb4fp/preprocess/down_sample.py
 src/nwb4fp/preprocess/down_sample_lfp.py
 src/nwb4fp/preprocess/extract_lfp.py
 src/nwb4fp/preprocess/get_path.py
 src/nwb4fp/preprocess/load_data.py
 src/nwb4fp/preprocess/run_phy.py
 src/nwb4fp/test/run_scripts/readnwb.py
+src/nwb4fp/test/run_scripts/readnwb_0283.py
 src/nwb4fp/test/run_scripts/readnwb_09PC.py
 src/nwb4fp/test/run_scripts/readnwb_09PD.py
 src/nwb4fp/test/run_scripts/test.py
 src/nwb4fp/test/run_scripts/test_lfp.py
```

### Comparing `nwb4fp-0.6.3.0/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.3.1/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

