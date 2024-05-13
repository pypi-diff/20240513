# Comparing `tmp/penguindashboard-1.0.4.tar.gz` & `tmp/penguindashboard-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penguindashboard-1.0.4.tar", last modified: Mon May 13 19:07:55 2024, max compression
+gzip compressed data, was "penguindashboard-1.0.5.tar", last modified: Mon May 13 19:35:57 2024, max compression
```

## Comparing `penguindashboard-1.0.4.tar` & `penguindashboard-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 19:07:55.134819 penguindashboard-1.0.4/
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1086 2024-05-10 18:51:23.000000 penguindashboard-1.0.4/LICENSE.txt
--rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 19:07:55.134819 penguindashboard-1.0.4/PKG-INFO
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2043 2024-05-10 18:51:23.000000 penguindashboard-1.0.4/README.md
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 19:07:55.118819 penguindashboard-1.0.4/penguindashboard/
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2508 2024-05-10 18:51:23.000000 penguindashboard-1.0.4/penguindashboard/AntiBERTa2_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     4095 2024-05-10 18:51:23.000000 penguindashboard-1.0.4/penguindashboard/BLAST_phylo.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     3445 2024-05-10 18:51:23.000000 penguindashboard-1.0.4/penguindashboard/ESM2_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2820 2024-05-10 18:51:23.000000 penguindashboard-1.0.4/penguindashboard/ProteinMPNN_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     3393 2024-05-10 18:51:23.000000 penguindashboard-1.0.4/penguindashboard/SaProt_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)        0 2024-05-10 19:11:13.000000 penguindashboard-1.0.4/penguindashboard/__init__.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1556 2024-05-10 18:51:23.000000 penguindashboard-1.0.4/penguindashboard/edit_mutcompute_output.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1185 2024-05-10 18:51:23.000000 penguindashboard-1.0.4/penguindashboard/esm_fold.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     4986 2024-05-13 19:07:18.000000 penguindashboard-1.0.4/penguindashboard/pipeline.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)    21114 2024-05-10 18:51:23.000000 penguindashboard-1.0.4/penguindashboard/score.py
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 19:07:55.130819 penguindashboard-1.0.4/penguindashboard.egg-info/
--rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 19:07:54.000000 penguindashboard-1.0.4/penguindashboard.egg-info/PKG-INFO
--rw-rw----   0 alf3564  (600491) Wilke    (500093)      576 2024-05-13 19:07:54.000000 penguindashboard-1.0.4/penguindashboard.egg-info/SOURCES.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)        1 2024-05-13 19:07:54.000000 penguindashboard-1.0.4/penguindashboard.egg-info/dependency_links.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       59 2024-05-13 19:07:54.000000 penguindashboard-1.0.4/penguindashboard.egg-info/entry_points.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       17 2024-05-13 19:07:54.000000 penguindashboard-1.0.4/penguindashboard.egg-info/top_level.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       38 2024-05-13 19:07:55.134819 penguindashboard-1.0.4/setup.cfg
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1420 2024-05-13 19:07:45.000000 penguindashboard-1.0.4/setup.py
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 19:35:57.777868 penguindashboard-1.0.5/
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1086 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/LICENSE.txt
+-rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 19:35:57.773868 penguindashboard-1.0.5/PKG-INFO
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2043 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/README.md
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 19:35:57.757869 penguindashboard-1.0.5/penguindashboard/
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2508 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/penguindashboard/AntiBERTa2_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     4095 2024-05-13 19:26:55.000000 penguindashboard-1.0.5/penguindashboard/BLAST_phylo.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     3445 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/penguindashboard/ESM2_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2820 2024-05-13 19:30:38.000000 penguindashboard-1.0.5/penguindashboard/ProteinMPNN_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     3393 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/penguindashboard/SaProt_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)        0 2024-05-10 19:11:13.000000 penguindashboard-1.0.5/penguindashboard/__init__.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1556 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/penguindashboard/edit_mutcompute_output.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1137 2024-05-13 19:11:52.000000 penguindashboard-1.0.5/penguindashboard/esm_fold.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     5089 2024-05-13 19:34:51.000000 penguindashboard-1.0.5/penguindashboard/pipeline.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)    21114 2024-05-10 18:51:23.000000 penguindashboard-1.0.5/penguindashboard/score.py
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 19:35:57.769868 penguindashboard-1.0.5/penguindashboard.egg-info/
+-rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 19:35:57.000000 penguindashboard-1.0.5/penguindashboard.egg-info/PKG-INFO
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)      576 2024-05-13 19:35:57.000000 penguindashboard-1.0.5/penguindashboard.egg-info/SOURCES.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)        1 2024-05-13 19:35:57.000000 penguindashboard-1.0.5/penguindashboard.egg-info/dependency_links.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       59 2024-05-13 19:35:57.000000 penguindashboard-1.0.5/penguindashboard.egg-info/entry_points.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       17 2024-05-13 19:35:57.000000 penguindashboard-1.0.5/penguindashboard.egg-info/top_level.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       38 2024-05-13 19:35:57.777868 penguindashboard-1.0.5/setup.cfg
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1420 2024-05-13 19:35:31.000000 penguindashboard-1.0.5/setup.py
```

### Comparing `penguindashboard-1.0.4/LICENSE.txt` & `penguindashboard-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.4/PKG-INFO` & `penguindashboard-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penguindashboard
-Version: 1.0.4
+Version: 1.0.5
 Summary: PEngUIN: Protein Engineering Using Independent Networks
 Home-page: https://github.com/AaronFeller/PEngUIN
 Author: Aaron Feller, Phillip Woolley
 Author-email: aaronleefeller@gmail.com, prwoolley@utexas.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `penguindashboard-1.0.4/README.md` & `penguindashboard-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.4/penguindashboard/AntiBERTa2_getLogits.py` & `penguindashboard-1.0.5/penguindashboard/AntiBERTa2_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.4/penguindashboard/BLAST_phylo.py` & `penguindashboard-1.0.5/penguindashboard/BLAST_phylo.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.4/penguindashboard/ESM2_getLogits.py` & `penguindashboard-1.0.5/penguindashboard/ESM2_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.4/penguindashboard/ProteinMPNN_getLogits.py` & `penguindashboard-1.0.5/penguindashboard/ProteinMPNN_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.4/penguindashboard/SaProt_getLogits.py` & `penguindashboard-1.0.5/penguindashboard/SaProt_getLogits.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.4/penguindashboard/edit_mutcompute_output.py` & `penguindashboard-1.0.5/penguindashboard/edit_mutcompute_output.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.4/penguindashboard/esm_fold.py` & `penguindashboard-1.0.5/penguindashboard/esm_fold.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import argparse
 import requests
 
 def main(args):
     # Input sequence
-    prefix = f'{args.dir}/{args.name}' #@param {type:"string"}
-    sequence = f'{args.sequence}' #@param {type:"string"}
+    prefix = f'{args.dir}/{args.name}'
+    sequence = f'{args.sequence}'
 
     # Making a POST request to the ESMFold API
     url = "https://api.esmatlas.com/foldSequence/v1/pdb/"
     headers = {'Content-Type': 'text/plain'}
     pdb_str = requests.post(url, headers=headers, data=sequence, verify=False)  # `verify=False` ignores SSL certificate validation
 
     # Check if the request was successful
```

### Comparing `penguindashboard-1.0.4/penguindashboard/pipeline.py` & `penguindashboard-1.0.5/penguindashboard/pipeline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 def main(args):
     import os
     import sys
     import subprocess
-
+    
     script_dir = os.path.dirname(os.path.realpath(__file__))
 
+    os.makedirs(args.output_dir, exist_ok=True)
+
     if not os.path.isfile(args.fasta_file):
         print(f"Error: The file {args.fasta_file} does not exist.")
         sys.exit(1)
 
     with open(args.fasta_file) as f:
         for line in f:
             if line.startswith('>'):
@@ -18,70 +20,70 @@
 
     with open(args.fasta_file) as f:
         seq = ''.join(line.strip() for line in f if not line.startswith('>'))
 
     os.makedirs(args.output_dir, exist_ok=True)
 
     print(f"Running ESMFold for {name}")
-    subprocess.check_call(f"python3 {script_dir}/esm_fold.py --sequence \"{seq}\" --name \"{name}\" --dir \"{args.output_dir}\"")
+    subprocess.run(f"python3 {script_dir}/esm_fold.py --sequence {seq} --name {name} --dir {args.output_dir}", shell=True)
 
     pdb_file = os.path.join(args.output_dir, f"{name}.pdb")
 
     ############### Running Models ###############
     print(f"Running models for {name}")
 
     if args.saprot:
         os.makedirs(f"{args.output_dir}/foldseek", exist_ok=True)
-        subprocess.check_call(f"foldseek createdb \"{pdb_file}\" \"{args.output_dir}/foldseek/{name}\" -v 1")
-        subprocess.check_call(f"foldseek lndb \"{args.output_dir}/foldseek/{name}_h\" \"{args.output_dir}/foldseek/{name}_ss_h\" -v 1")
-        subprocess.check_call(f"foldseek convert2fasta \"{args.output_dir}/foldseek/{name}_ss\" \"{args.output_dir}/foldseek/{name}_ss.fasta\" -v 1")
+        subprocess.run(f"foldseek createdb \"{pdb_file}\" \"{args.output_dir}/foldseek/{name}\" -v 1", shell=True)
+        subprocess.run(f"foldseek lndb \"{args.output_dir}/foldseek/{name}_h\" \"{args.output_dir}/foldseek/{name}_ss_h\" -v 1", shell=True)
+        subprocess.run(f"foldseek convert2fasta \"{args.output_dir}/foldseek/{name}_ss\" \"{args.output_dir}/foldseek/{name}_ss.fasta\" -v 1", shell=True)
         print("Running SaProt...")
-        subprocess.check_call(f"python3 {script_dir}/SaProt_getLogits.py --amino_acid_str \"{seq}\" --foldseek_tokens \"{args.output_dir}/foldseek/{name}_ss.fasta\" --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"")
+        subprocess.run(f"python3 {script_dir}/SaProt_getLogits.py --amino_acid_str \"{seq}\" --foldseek_tokens \"{args.output_dir}/foldseek/{name}_ss.fasta\" --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"", shell=True)
 
     if args.antiberta:
         print("Running AntiBERTa2...")
-        subprocess.check_call(f"python3 {script_dir}/AntiBERTa2_getLogits.py --amino_acid_str \"{seq}\" --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"")
+        subprocess.run(f"python3 {script_dir}/AntiBERTa2_getLogits.py --amino_acid_str \"{seq}\" --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"", shell=True)
 
     if args.esm:
         print("Running ESM2 (650M)...")
-        subprocess.check_call(f"python3 {script_dir}/ESM2_getLogits.py --sequence \"{seq}\" --model_choice esm2_t33_650M_UR50D --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"")
+        subprocess.run(f"python3 {script_dir}/ESM2_getLogits.py --sequence \"{seq}\" --model_choice esm2_t33_650M_UR50D --output_prefix \"{args.output_dir}/{name}\" --device \"{args.device}\"", shell=True)
 
     if args.proteinmpnn:
         proteinmpnn_dir = os.path.join(args.output_dir, "../LigandMPNN")
         if not os.path.isdir(proteinmpnn_dir):
             print("Setting up ProteinMPNN...")
-            subprocess.check_call(f"git clone https://github.com/dauparas/LigandMPNN.git \"{proteinmpnn_dir}\"")
+            subprocess.run(f"git clone https://github.com/dauparas/LigandMPNN.git \"{proteinmpnn_dir}\"", shell=True)
             os.makedirs(f"{proteinmpnn_dir}/model_params", exist_ok=True)
-            subprocess.check_call(f"wget https://github.com/dauparas/ProteinMPNN/raw/main/vanilla_model_weights/v_48_020.pt -P \"{proteinmpnn_dir}/model_params\"")
-            subprocess.check_call(f"cp \"{script_dir}/score.py\" \"{proteinmpnn_dir}/score.py\"")
+            subprocess.run(f"wget https://github.com/dauparas/ProteinMPNN/raw/main/vanilla_model_weights/v_48_020.pt -P \"{proteinmpnn_dir}/model_params\"", shell=True)
+            subprocess.run(f"cp \"{script_dir}/score.py\" \"{proteinmpnn_dir}/score.py\"", shell=True)
         else:
             print("ProteinMPNN already set up.")
 
         print("Running ProteinMPNN...")
-        subprocess.check_call(f"python3 {script_dir}/ProteinMPNN_getLogits.py --output_prefix \"{args.output_dir}\" --proteinmpnn_dir {proteinmpnn_dir} --pdb_file \"{pdb_file}\" --device \"{args.device}\"")
+        subprocess.run(f"python3 {script_dir}/ProteinMPNN_getLogits.py --output_prefix \"{args.output_dir}\" --proteinmpnn_dir {proteinmpnn_dir} --pdb_file \"{pdb_file}\" --device \"{args.device}\"", shell=True)
 
     if args.blast:
         print("Running BLAST phylogeny...")
-        subprocess.check_call(f"python3 {script_dir}/BLAST_phylo.py --outdir \"{args.output_dir}\" --sequence \"{seq}\" --name \"{name}\"")
+        subprocess.run(f"python3 {script_dir}/BLAST_phylo.py --outdir \"{args.output_dir}\" --sequence \"{seq}\" --name \"{name}\"", shell=True)
 
 
     ### MUTCOMPUTE SECITON ###
     if args.mutcompute:
         print("Running MutCompute...")
         docker_command = (
         f"docker run --rm -v $(pwd)/{args.output_dir}:/mutcompute/input "
         f"aaronfeller/penguin "
         f"-c 'cd scripts && python run.py -p {name}.pdb -d ../input/ > ../input/{name}.mutcompute.txt'"
         )
         
         # Execute the Docker command
-        subprocess.check_call(docker_command, shell=True)
+        subprocess.run(docker_command, shell=True)
 
         print("Editing MutCompute output...")
-        subprocess.check_call(f"python {script_dir}/edit_mutcompute_output.py --output {args.output_dir} --name {name}")
+        subprocess.run(f"python {script_dir}/edit_mutcompute_output.py --output {args.output_dir} --name {name}", shell=True)
 
     print(f"Predictions complete for {name}")
 
 if __name__ == "__main__":
     import argparse
     parser = argparse.ArgumentParser(description="Process a FASTA file and run a sequence analysis pipeline.")
     parser.add_argument("fasta_file", type=str, help="Path to the input FASTA file.")
@@ -90,8 +92,8 @@
     parser.add_argument("--saprot", type=bool, default="True", help="Run SaProt")
     parser.add_argument("--esm", type=bool, default="True", help="Run ESM2")
     parser.add_argument("--proteinmpnn", type=bool, default="True", help="Run ProteinMPNN")
     parser.add_argument("--blast", type=bool, default="True", help="Run BLAST phylogeny")
     parser.add_argument("--mutcompute", type=bool, default="True", help="Run MutCompute")
     parser.add_argument("--antiberta", type=bool, default="False", help="Run AntiBERTa2")    
     args = parser.parse_args()
-    main()
+    main(args)
```

### Comparing `penguindashboard-1.0.4/penguindashboard/score.py` & `penguindashboard-1.0.5/penguindashboard/score.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.4/penguindashboard.egg-info/PKG-INFO` & `penguindashboard-1.0.5/penguindashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penguindashboard
-Version: 1.0.4
+Version: 1.0.5
 Summary: PEngUIN: Protein Engineering Using Independent Networks
 Home-page: https://github.com/AaronFeller/PEngUIN
 Author: Aaron Feller, Phillip Woolley
 Author-email: aaronleefeller@gmail.com, prwoolley@utexas.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `penguindashboard-1.0.4/penguindashboard.egg-info/SOURCES.txt` & `penguindashboard-1.0.5/penguindashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.4/setup.py` & `penguindashboard-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 # Text of the README file
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='penguindashboard',
-    version='1.0.4',
+    version='1.0.5',
     author='Aaron Feller, Phillip Woolley',
     author_email='aaronleefeller@gmail.com, prwoolley@utexas.edu',
     description='PEngUIN: Protein Engineering Using Independent Networks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AaronFeller/PEngUIN',
     license='MIT',
```

