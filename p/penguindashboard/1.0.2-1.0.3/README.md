# Comparing `tmp/penguindashboard-1.0.2.tar.gz` & `tmp/penguindashboard-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penguindashboard-1.0.2.tar", last modified: Mon May 13 17:22:07 2024, max compression
+gzip compressed data, was "penguindashboard-1.0.3.tar", last modified: Mon May 13 18:58:35 2024, max compression
```

## Comparing `penguindashboard-1.0.2.tar` & `penguindashboard-1.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 17:22:07.277235 penguindashboard-1.0.2/
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1086 2024-05-10 18:51:23.000000 penguindashboard-1.0.2/LICENSE.txt
--rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 17:22:07.277235 penguindashboard-1.0.2/PKG-INFO
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2043 2024-05-10 18:51:23.000000 penguindashboard-1.0.2/README.md
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 17:22:07.265236 penguindashboard-1.0.2/penguindashboard/
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2508 2024-05-10 18:51:23.000000 penguindashboard-1.0.2/penguindashboard/AntiBERTa2_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     4095 2024-05-10 18:51:23.000000 penguindashboard-1.0.2/penguindashboard/BLAST_phylo.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     3445 2024-05-10 18:51:23.000000 penguindashboard-1.0.2/penguindashboard/ESM2_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2820 2024-05-10 18:51:23.000000 penguindashboard-1.0.2/penguindashboard/ProteinMPNN_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     3393 2024-05-10 18:51:23.000000 penguindashboard-1.0.2/penguindashboard/SaProt_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)        0 2024-05-10 19:11:13.000000 penguindashboard-1.0.2/penguindashboard/__init__.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1556 2024-05-10 18:51:23.000000 penguindashboard-1.0.2/penguindashboard/edit_mutcompute_output.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1185 2024-05-10 18:51:23.000000 penguindashboard-1.0.2/penguindashboard/esm_fold.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     5007 2024-05-13 17:13:19.000000 penguindashboard-1.0.2/penguindashboard/pipeline.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)    21114 2024-05-10 18:51:23.000000 penguindashboard-1.0.2/penguindashboard/score.py
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 17:22:07.273236 penguindashboard-1.0.2/penguindashboard.egg-info/
--rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 17:22:06.000000 penguindashboard-1.0.2/penguindashboard.egg-info/PKG-INFO
--rw-rw----   0 alf3564  (600491) Wilke    (500093)      576 2024-05-13 17:22:06.000000 penguindashboard-1.0.2/penguindashboard.egg-info/SOURCES.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)        1 2024-05-13 17:22:06.000000 penguindashboard-1.0.2/penguindashboard.egg-info/dependency_links.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       59 2024-05-13 17:22:06.000000 penguindashboard-1.0.2/penguindashboard.egg-info/entry_points.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       17 2024-05-13 17:22:06.000000 penguindashboard-1.0.2/penguindashboard.egg-info/top_level.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       38 2024-05-13 17:22:07.277235 penguindashboard-1.0.2/setup.cfg
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1420 2024-05-13 17:17:53.000000 penguindashboard-1.0.2/setup.py
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 18:58:35.319230 penguindashboard-1.0.3/
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1086 2024-05-10 18:51:23.000000 penguindashboard-1.0.3/LICENSE.txt
+-rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 18:58:35.315230 penguindashboard-1.0.3/PKG-INFO
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2043 2024-05-10 18:51:23.000000 penguindashboard-1.0.3/README.md
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 18:58:35.299231 penguindashboard-1.0.3/penguindashboard/
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2508 2024-05-10 18:51:23.000000 penguindashboard-1.0.3/penguindashboard/AntiBERTa2_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     4095 2024-05-10 18:51:23.000000 penguindashboard-1.0.3/penguindashboard/BLAST_phylo.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     3445 2024-05-10 18:51:23.000000 penguindashboard-1.0.3/penguindashboard/ESM2_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2820 2024-05-10 18:51:23.000000 penguindashboard-1.0.3/penguindashboard/ProteinMPNN_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     3393 2024-05-10 18:51:23.000000 penguindashboard-1.0.3/penguindashboard/SaProt_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)        0 2024-05-10 19:11:13.000000 penguindashboard-1.0.3/penguindashboard/__init__.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1556 2024-05-10 18:51:23.000000 penguindashboard-1.0.3/penguindashboard/edit_mutcompute_output.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1185 2024-05-10 18:51:23.000000 penguindashboard-1.0.3/penguindashboard/esm_fold.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     5006 2024-05-13 18:57:15.000000 penguindashboard-1.0.3/penguindashboard/pipeline.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)    21114 2024-05-10 18:51:23.000000 penguindashboard-1.0.3/penguindashboard/score.py
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 18:58:35.311230 penguindashboard-1.0.3/penguindashboard.egg-info/
+-rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 18:58:35.000000 penguindashboard-1.0.3/penguindashboard.egg-info/PKG-INFO
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)      576 2024-05-13 18:58:35.000000 penguindashboard-1.0.3/penguindashboard.egg-info/SOURCES.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)        1 2024-05-13 18:58:35.000000 penguindashboard-1.0.3/penguindashboard.egg-info/dependency_links.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       59 2024-05-13 18:58:35.000000 penguindashboard-1.0.3/penguindashboard.egg-info/entry_points.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       17 2024-05-13 18:58:35.000000 penguindashboard-1.0.3/penguindashboard.egg-info/top_level.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       38 2024-05-13 18:58:35.319230 penguindashboard-1.0.3/setup.cfg
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1420 2024-05-13 18:43:48.000000 penguindashboard-1.0.3/setup.py
```

### Comparing `penguindashboard-1.0.2/LICENSE.txt` & `penguindashboard-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/PKG-INFO` & `penguindashboard-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penguindashboard
-Version: 1.0.2
+Version: 1.0.3
 Summary: PEngUIN: Protein Engineering Using Independent Networks
 Home-page: https://github.com/AaronFeller/PEngUIN
 Author: Aaron Feller, Phillip Woolley
 Author-email: aaronleefeller@gmail.com, prwoolley@utexas.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `penguindashboard-1.0.2/README.md` & `penguindashboard-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/penguindashboard/AntiBERTa2_getLogits.py` & `penguindashboard-1.0.3/penguindashboard/AntiBERTa2_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/penguindashboard/BLAST_phylo.py` & `penguindashboard-1.0.3/penguindashboard/BLAST_phylo.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/penguindashboard/ESM2_getLogits.py` & `penguindashboard-1.0.3/penguindashboard/ESM2_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/penguindashboard/ProteinMPNN_getLogits.py` & `penguindashboard-1.0.3/penguindashboard/ProteinMPNN_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/penguindashboard/SaProt_getLogits.py` & `penguindashboard-1.0.3/penguindashboard/SaProt_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/penguindashboard/edit_mutcompute_output.py` & `penguindashboard-1.0.3/penguindashboard/edit_mutcompute_output.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/penguindashboard/esm_fold.py` & `penguindashboard-1.0.3/penguindashboard/esm_fold.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/penguindashboard/pipeline.py` & `penguindashboard-1.0.3/penguindashboard/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 def main(args):
     import os
     import sys
     import subprocess
 
     def check_call(command):
         try:
-            subprocess.check_call(command, shell=True)
+            subprocess.call(command, shell=True)
         except subprocess.CalledProcessError:
             sys.exit(1)
 
 
     script_dir = os.path.dirname(os.path.realpath(__file__))
 
     if not os.path.isfile(args.fasta_file):
@@ -49,15 +49,15 @@
         check_call(f"python3 {script_dir}/AntiBERTa2_getLogits.py --amino_acid_str \"{seq}\" --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"")
 
     if args.esm:
         print("Running ESM2 (650M)...")
         check_call(f"python3 {script_dir}/ESM2_getLogits.py --sequence \"{seq}\" --model_choice esm2_t33_650M_UR50D --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"")
 
     if args.proteinmpnn:
-        proteinmpnn_dir = os.path.join(script_dir, "../LigandMPNN")
+        proteinmpnn_dir = os.path.join(args.output_dir, "../LigandMPNN")
         if not os.path.isdir(proteinmpnn_dir):
             print("Setting up ProteinMPNN...")
             check_call(f"git clone https://github.com/dauparas/LigandMPNN.git \"{proteinmpnn_dir}\"")
             os.makedirs(f"{proteinmpnn_dir}/model_params", exist_ok=True)
             check_call(f"wget https://github.com/dauparas/ProteinMPNN/raw/main/vanilla_model_weights/v_48_020.pt -P \"{proteinmpnn_dir}/model_params\"")
             check_call(f"cp \"{script_dir}/score.py\" \"{proteinmpnn_dir}/score.py\"")
         else:
```

### Comparing `penguindashboard-1.0.2/penguindashboard/score.py` & `penguindashboard-1.0.3/penguindashboard/score.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/penguindashboard.egg-info/PKG-INFO` & `penguindashboard-1.0.3/penguindashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penguindashboard
-Version: 1.0.2
+Version: 1.0.3
 Summary: PEngUIN: Protein Engineering Using Independent Networks
 Home-page: https://github.com/AaronFeller/PEngUIN
 Author: Aaron Feller, Phillip Woolley
 Author-email: aaronleefeller@gmail.com, prwoolley@utexas.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `penguindashboard-1.0.2/penguindashboard.egg-info/SOURCES.txt` & `penguindashboard-1.0.3/penguindashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.2/setup.py` & `penguindashboard-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 # Text of the README file
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='penguindashboard',
-    version='1.0.2',
+    version='1.0.3',
     author='Aaron Feller, Phillip Woolley',
     author_email='aaronleefeller@gmail.com, prwoolley@utexas.edu',
     description='PEngUIN: Protein Engineering Using Independent Networks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AaronFeller/PEngUIN',
     license='MIT',
```

