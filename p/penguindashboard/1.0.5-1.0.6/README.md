# Comparing `tmp/penguindashboard-1.0.5.tar.gz` & `tmp/penguindashboard-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penguindashboard-1.0.5.tar", last modified: Mon May 13 19:35:57 2024, max compression
+gzip compressed data, was "penguindashboard-1.0.6.tar", last modified: Mon May 13 20:05:01 2024, max compression
```

## Comparing `penguindashboard-1.0.5.tar` & `penguindashboard-1.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 19:35:57.777868 penguindashboard-1.0.5/
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1086 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/LICENSE.txt
--rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 19:35:57.773868 penguindashboard-1.0.5/PKG-INFO
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2043 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/README.md
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 19:35:57.757869 penguindashboard-1.0.5/penguindashboard/
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2508 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/penguindashboard/AntiBERTa2_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     4095 2024-05-13 19:26:55.000000 penguindashboard-1.0.5/penguindashboard/BLAST_phylo.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     3445 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/penguindashboard/ESM2_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2820 2024-05-13 19:30:38.000000 penguindashboard-1.0.5/penguindashboard/ProteinMPNN_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     3393 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/penguindashboard/SaProt_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)        0 2024-05-10 19:11:13.000000 penguindashboard-1.0.5/penguindashboard/__init__.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1556 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/penguindashboard/edit_mutcompute_output.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1137 2024-05-13 19:11:52.000000 penguindashboard-1.0.5/penguindashboard/esm_fold.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     5089 2024-05-13 19:34:51.000000 penguindashboard-1.0.5/penguindashboard/pipeline.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)    21114 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/penguindashboard/score.py
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 19:35:57.769868 penguindashboard-1.0.5/penguindashboard.egg-info/
--rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 19:35:57.000000 penguindashboard-1.0.5/penguindashboard.egg-info/PKG-INFO
--rw-rw----   0 alf3564  (600491) Wilke    (500093)      576 2024-05-13 19:35:57.000000 penguindashboard-1.0.5/penguindashboard.egg-info/SOURCES.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)        1 2024-05-13 19:35:57.000000 penguindashboard-1.0.5/penguindashboard.egg-info/dependency_links.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       59 2024-05-13 19:35:57.000000 penguindashboard-1.0.5/penguindashboard.egg-info/entry_points.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       17 2024-05-13 19:35:57.000000 penguindashboard-1.0.5/penguindashboard.egg-info/top_level.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       38 2024-05-13 19:35:57.777868 penguindashboard-1.0.5/setup.cfg
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1420 2024-05-13 19:35:31.000000 penguindashboard-1.0.5/setup.py
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 20:05:00.989675 penguindashboard-1.0.6/
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1086 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/LICENSE.txt
+-rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 20:05:00.989675 penguindashboard-1.0.6/PKG-INFO
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2043 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/README.md
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 20:05:00.973676 penguindashboard-1.0.6/penguindashboard/
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2508 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/penguindashboard/AntiBERTa2_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     4095 2024-05-13 19:26:55.000000 penguindashboard-1.0.6/penguindashboard/BLAST_phylo.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     3477 2024-05-13 20:00:50.000000 penguindashboard-1.0.6/penguindashboard/ESM2_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2820 2024-05-13 19:30:38.000000 penguindashboard-1.0.6/penguindashboard/ProteinMPNN_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     3393 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/penguindashboard/SaProt_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)        0 2024-05-10 19:11:13.000000 penguindashboard-1.0.6/penguindashboard/__init__.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1556 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/penguindashboard/edit_mutcompute_output.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1137 2024-05-13 19:11:52.000000 penguindashboard-1.0.6/penguindashboard/esm_fold.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     5060 2024-05-13 20:03:43.000000 penguindashboard-1.0.6/penguindashboard/pipeline.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)    21114 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/penguindashboard/score.py
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 20:05:00.985676 penguindashboard-1.0.6/penguindashboard.egg-info/
+-rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 20:05:00.000000 penguindashboard-1.0.6/penguindashboard.egg-info/PKG-INFO
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)      576 2024-05-13 20:05:00.000000 penguindashboard-1.0.6/penguindashboard.egg-info/SOURCES.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)        1 2024-05-13 20:05:00.000000 penguindashboard-1.0.6/penguindashboard.egg-info/dependency_links.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       59 2024-05-13 20:05:00.000000 penguindashboard-1.0.6/penguindashboard.egg-info/entry_points.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       17 2024-05-13 20:05:00.000000 penguindashboard-1.0.6/penguindashboard.egg-info/top_level.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       38 2024-05-13 20:05:00.989675 penguindashboard-1.0.6/setup.cfg
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1420 2024-05-13 20:04:50.000000 penguindashboard-1.0.6/setup.py
```

### Comparing `penguindashboard-1.0.5/LICENSE.txt` & `penguindashboard-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.5/PKG-INFO` & `penguindashboard-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penguindashboard
-Version: 1.0.5
+Version: 1.0.6
 Summary: PEngUIN: Protein Engineering Using Independent Networks
 Home-page: https://github.com/AaronFeller/PEngUIN
 Author: Aaron Feller, Phillip Woolley
 Author-email: aaronleefeller@gmail.com, prwoolley@utexas.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `penguindashboard-1.0.5/README.md` & `penguindashboard-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.5/penguindashboard/AntiBERTa2_getLogits.py` & `penguindashboard-1.0.6/penguindashboard/AntiBERTa2_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.5/penguindashboard/BLAST_phylo.py` & `penguindashboard-1.0.6/penguindashboard/BLAST_phylo.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.5/penguindashboard/ESM2_getLogits.py` & `penguindashboard-1.0.6/penguindashboard/ESM2_getLogits.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from transformers import AutoTokenizer, AutoModelForMaskedLM
 import torch
 import numpy as np
 import argparse
 
+print("ESM started running.")
+
 def load_model(model_choice):
     print('Loading ESM2 model...')
     if model_choice == 'esm2_t48_15B_UR50D':
         tokenizer = AutoTokenizer.from_pretrained("facebook/esm2_t48_15B_UR50D")
         model = AutoModelForMaskedLM.from_pretrained("facebook/esm2_t48_15B_UR50D")
         return model, tokenizer
     elif model_choice == 'esm2_t36_3B_UR50D':
@@ -49,15 +51,15 @@
     np.save(f'{output_prefix}.logits.{model_choice}.npy', new_nplogits)
 
 def main():
     parser = argparse.ArgumentParser(description='Process sequences using ESM-2 model.')
     parser.add_argument('--sequence', type=str, help='Sequence to pass through ESM-2 model')
     parser.add_argument('--model_choice', type=str, help='Choice of ESM2 model. Options: [esm2_t48_15B_UR50D, esm2_t36_3B_UR50D, esm2_t33_650M_UR50D] Default: esm2_t33_650M_UR50D', default = 'esm2_t33_650M_UR50D')
     parser.add_argument('--output_prefix', type=str, help='Optional prefix to add to the output filename')
-    parser.add_argument('--device', type=str, help='Specify the Cuda device index',default = '0')
+    parser.add_argument('--device', type=str, help='Specify the Cuda device index', default = '0')
 
     args = parser.parse_args()
     sequence = args.sequence
     model_choice = args.model_choice
     output_prefix = args.output_prefix
     device = args.device
```

### Comparing `penguindashboard-1.0.5/penguindashboard/ProteinMPNN_getLogits.py` & `penguindashboard-1.0.6/penguindashboard/ProteinMPNN_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.5/penguindashboard/SaProt_getLogits.py` & `penguindashboard-1.0.6/penguindashboard/SaProt_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.5/penguindashboard/edit_mutcompute_output.py` & `penguindashboard-1.0.6/penguindashboard/edit_mutcompute_output.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.5/penguindashboard/esm_fold.py` & `penguindashboard-1.0.6/penguindashboard/esm_fold.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.5/penguindashboard/pipeline.py` & `penguindashboard-1.0.6/penguindashboard/pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,50 +24,50 @@
     os.makedirs(args.output_dir, exist_ok=True)
 
     print(f"Running ESMFold for {name}")
     subprocess.run(f"python3 {script_dir}/esm_fold.py --sequence {seq} --name {name} --dir {args.output_dir}", shell=True)
 
     pdb_file = os.path.join(args.output_dir, f"{name}.pdb")
 
-    ############### Running Models ###############
+    ############### Running Models ##########################################################################################
     print(f"Running models for {name}")
 
     if args.saprot:
         os.makedirs(f"{args.output_dir}/foldseek", exist_ok=True)
-        subprocess.run(f"foldseek createdb \"{pdb_file}\" \"{args.output_dir}/foldseek/{name}\" -v 1", shell=True)
-        subprocess.run(f"foldseek lndb \"{args.output_dir}/foldseek/{name}_h\" \"{args.output_dir}/foldseek/{name}_ss_h\" -v 1", shell=True)
-        subprocess.run(f"foldseek convert2fasta \"{args.output_dir}/foldseek/{name}_ss\" \"{args.output_dir}/foldseek/{name}_ss.fasta\" -v 1", shell=True)
+        subprocess.run(f"foldseek createdb {pdb_file} {args.output_dir}/foldseek/{name} -v 1", shell=True)
+        subprocess.run(f"foldseek lndb {args.output_dir}/foldseek/{name}_h {args.output_dir}/foldseek/{name}_ss_h -v 1", shell=True)
+        subprocess.run(f"foldseek convert2fasta {args.output_dir}/foldseek/{name}_ss {args.output_dir}/foldseek/{name}_ss.fasta -v 1", shell=True)
         print("Running SaProt...")
-        subprocess.run(f"python3 {script_dir}/SaProt_getLogits.py --amino_acid_str \"{seq}\" --foldseek_tokens \"{args.output_dir}/foldseek/{name}_ss.fasta\" --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"", shell=True)
+        subprocess.run(f"python3 {script_dir}/SaProt_getLogits.py --amino_acid_str {seq} --foldseek_tokens {args.output_dir}/foldseek/{name}_ss.fasta --output_prefix {args.output_dir}/{name} --device {args.device}", shell=True)
 
     if args.antiberta:
         print("Running AntiBERTa2...")
-        subprocess.run(f"python3 {script_dir}/AntiBERTa2_getLogits.py --amino_acid_str \"{seq}\" --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"", shell=True)
+        subprocess.run(f"python3 {script_dir}/AntiBERTa2_getLogits.py --amino_acid_str {seq} --output_prefix {args.output_dir}/{name} --device {args.device}", shell=True)
 
     if args.esm:
         print("Running ESM2 (650M)...")
-        subprocess.run(f"python3 {script_dir}/ESM2_getLogits.py --sequence \"{seq}\" --model_choice esm2_t33_650M_UR50D --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"", shell=True)
+        subprocess.run(f"python3 {script_dir}/ESM2_getLogits.py --sequence {seq} --model_choice esm2_t33_650M_UR50D --output_prefix {args.output_dir}/{name} --device {args.device}", shell=True)
 
     if args.proteinmpnn:
         proteinmpnn_dir = os.path.join(args.output_dir, "../LigandMPNN")
         if not os.path.isdir(proteinmpnn_dir):
             print("Setting up ProteinMPNN...")
-            subprocess.run(f"git clone https://github.com/dauparas/LigandMPNN.git \"{proteinmpnn_dir}\"", shell=True)
+            subprocess.run(f"git clone https://github.com/dauparas/LigandMPNN.git {proteinmpnn_dir}", shell=True)
             os.makedirs(f"{proteinmpnn_dir}/model_params", exist_ok=True)
-            subprocess.run(f"wget https://github.com/dauparas/ProteinMPNN/raw/main/vanilla_model_weights/v_48_020.pt -P \"{proteinmpnn_dir}/model_params\"", shell=True)
-            subprocess.run(f"cp \"{script_dir}/score.py\" \"{proteinmpnn_dir}/score.py\"", shell=True)
+            subprocess.run(f"wget https://github.com/dauparas/ProteinMPNN/raw/main/vanilla_model_weights/v_48_020.pt -P {proteinmpnn_dir}/model_params", shell=True)
+            subprocess.run(f"cp {script_dir}/score.py {proteinmpnn_dir}/score.py", shell=True)
         else:
             print("ProteinMPNN already set up.")
 
         print("Running ProteinMPNN...")
-        subprocess.run(f"python3 {script_dir}/ProteinMPNN_getLogits.py --output_prefix \"{args.output_dir}\" --proteinmpnn_dir {proteinmpnn_dir} --pdb_file \"{pdb_file}\" --device \"{args.device}\"", shell=True)
+        subprocess.run(f"python3 {script_dir}/ProteinMPNN_getLogits.py --output_prefix {args.output_dir} --proteinmpnn_dir {proteinmpnn_dir} --pdb_file {pdb_file} --device {args.device}", shell=True)
 
     if args.blast:
         print("Running BLAST phylogeny...")
-        subprocess.run(f"python3 {script_dir}/BLAST_phylo.py --outdir \"{args.output_dir}\" --sequence \"{seq}\" --name \"{name}\"", shell=True)
+        subprocess.run(f"python3 {script_dir}/BLAST_phylo.py --outdir {args.output_dir} --sequence {seq} --name {name}", shell=True)
 
 
     ### MUTCOMPUTE SECITON ###
     if args.mutcompute:
         print("Running MutCompute...")
         docker_command = (
         f"docker run --rm -v $(pwd)/{args.output_dir}:/mutcompute/input "
```

### Comparing `penguindashboard-1.0.5/penguindashboard/score.py` & `penguindashboard-1.0.6/penguindashboard/score.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.5/penguindashboard.egg-info/PKG-INFO` & `penguindashboard-1.0.6/penguindashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penguindashboard
-Version: 1.0.5
+Version: 1.0.6
 Summary: PEngUIN: Protein Engineering Using Independent Networks
 Home-page: https://github.com/AaronFeller/PEngUIN
 Author: Aaron Feller, Phillip Woolley
 Author-email: aaronleefeller@gmail.com, prwoolley@utexas.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `penguindashboard-1.0.5/penguindashboard.egg-info/SOURCES.txt` & `penguindashboard-1.0.6/penguindashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.5/setup.py` & `penguindashboard-1.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 # Text of the README file
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='penguindashboard',
-    version='1.0.5',
+    version='1.0.6',
     author='Aaron Feller, Phillip Woolley',
     author_email='aaronleefeller@gmail.com, prwoolley@utexas.edu',
     description='PEngUIN: Protein Engineering Using Independent Networks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AaronFeller/PEngUIN',
     license='MIT',
```

