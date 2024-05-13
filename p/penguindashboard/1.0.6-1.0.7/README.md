# Comparing `tmp/penguindashboard-1.0.6.tar.gz` & `tmp/penguindashboard-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penguindashboard-1.0.6.tar", last modified: Mon May 13 20:05:01 2024, max compression
+gzip compressed data, was "penguindashboard-1.0.7.tar", last modified: Mon May 13 20:53:33 2024, max compression
```

## Comparing `penguindashboard-1.0.6.tar` & `penguindashboard-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 20:05:00.989675 penguindashboard-1.0.6/
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1086 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/LICENSE.txt
--rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 20:05:00.989675 penguindashboard-1.0.6/PKG-INFO
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2043 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/README.md
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 20:05:00.973676 penguindashboard-1.0.6/penguindashboard/
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2508 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/penguindashboard/AntiBERTa2_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     4095 2024-05-13 19:26:55.000000 penguindashboard-1.0.6/penguindashboard/BLAST_phylo.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     3477 2024-05-13 20:00:50.000000 penguindashboard-1.0.6/penguindashboard/ESM2_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     2820 2024-05-13 19:30:38.000000 penguindashboard-1.0.6/penguindashboard/ProteinMPNN_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     3393 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/penguindashboard/SaProt_getLogits.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)        0 2024-05-10 19:11:13.000000 penguindashboard-1.0.6/penguindashboard/__init__.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1556 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/penguindashboard/edit_mutcompute_output.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1137 2024-05-13 19:11:52.000000 penguindashboard-1.0.6/penguindashboard/esm_fold.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     5060 2024-05-13 20:03:43.000000 penguindashboard-1.0.6/penguindashboard/pipeline.py
--rw-rw----   0 alf3564  (600491) Wilke    (500093)    21114 2024-05-10 18:51:23.000000 penguindashboard-1.0.6/penguindashboard/score.py
-drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 20:05:00.985676 penguindashboard-1.0.6/penguindashboard.egg-info/
--rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 20:05:00.000000 penguindashboard-1.0.6/penguindashboard.egg-info/PKG-INFO
--rw-rw----   0 alf3564  (600491) Wilke    (500093)      576 2024-05-13 20:05:00.000000 penguindashboard-1.0.6/penguindashboard.egg-info/SOURCES.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)        1 2024-05-13 20:05:00.000000 penguindashboard-1.0.6/penguindashboard.egg-info/dependency_links.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       59 2024-05-13 20:05:00.000000 penguindashboard-1.0.6/penguindashboard.egg-info/entry_points.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       17 2024-05-13 20:05:00.000000 penguindashboard-1.0.6/penguindashboard.egg-info/top_level.txt
--rw-rw----   0 alf3564  (600491) Wilke    (500093)       38 2024-05-13 20:05:00.989675 penguindashboard-1.0.6/setup.cfg
--rw-rw----   0 alf3564  (600491) Wilke    (500093)     1420 2024-05-13 20:04:50.000000 penguindashboard-1.0.6/setup.py
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 20:53:33.425878 penguindashboard-1.0.7/
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1086 2024-05-10 18:51:23.000000 penguindashboard-1.0.7/LICENSE.txt
+-rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 20:53:33.425878 penguindashboard-1.0.7/PKG-INFO
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2043 2024-05-10 18:51:23.000000 penguindashboard-1.0.7/README.md
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 20:53:33.409879 penguindashboard-1.0.7/penguindashboard/
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2512 2024-05-13 20:52:21.000000 penguindashboard-1.0.7/penguindashboard/AntiBERTa2_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     4052 2024-05-13 20:51:49.000000 penguindashboard-1.0.7/penguindashboard/BLAST_phylo.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     3486 2024-05-13 20:51:04.000000 penguindashboard-1.0.7/penguindashboard/ESM2_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     2825 2024-05-13 20:51:24.000000 penguindashboard-1.0.7/penguindashboard/ProteinMPNN_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     3398 2024-05-13 20:52:54.000000 penguindashboard-1.0.7/penguindashboard/SaProt_getLogits.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)        0 2024-05-10 19:11:13.000000 penguindashboard-1.0.7/penguindashboard/__init__.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1556 2024-05-10 18:51:23.000000 penguindashboard-1.0.7/penguindashboard/edit_mutcompute_output.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1137 2024-05-13 19:11:52.000000 penguindashboard-1.0.7/penguindashboard/esm_fold.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     4968 2024-05-13 20:20:53.000000 penguindashboard-1.0.7/penguindashboard/pipeline.py
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)    21114 2024-05-10 18:51:23.000000 penguindashboard-1.0.7/penguindashboard/score.py
+drwxrws---   0 alf3564  (600491) Wilke    (500093)        0 2024-05-13 20:53:33.421879 penguindashboard-1.0.7/penguindashboard.egg-info/
+-rw-r--r--   0 alf3564  (600491) Wilke    (500093)     2927 2024-05-13 20:53:33.000000 penguindashboard-1.0.7/penguindashboard.egg-info/PKG-INFO
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)      576 2024-05-13 20:53:33.000000 penguindashboard-1.0.7/penguindashboard.egg-info/SOURCES.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)        1 2024-05-13 20:53:33.000000 penguindashboard-1.0.7/penguindashboard.egg-info/dependency_links.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       59 2024-05-13 20:53:33.000000 penguindashboard-1.0.7/penguindashboard.egg-info/entry_points.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       17 2024-05-13 20:53:33.000000 penguindashboard-1.0.7/penguindashboard.egg-info/top_level.txt
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)       38 2024-05-13 20:53:33.425878 penguindashboard-1.0.7/setup.cfg
+-rw-rw----   0 alf3564  (600491) Wilke    (500093)     1420 2024-05-13 20:53:23.000000 penguindashboard-1.0.7/setup.py
```

### Comparing `penguindashboard-1.0.6/LICENSE.txt` & `penguindashboard-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.6/PKG-INFO` & `penguindashboard-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penguindashboard
-Version: 1.0.6
+Version: 1.0.7
 Summary: PEngUIN: Protein Engineering Using Independent Networks
 Home-page: https://github.com/AaronFeller/PEngUIN
 Author: Aaron Feller, Phillip Woolley
 Author-email: aaronleefeller@gmail.com, prwoolley@utexas.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `penguindashboard-1.0.6/README.md` & `penguindashboard-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.6/penguindashboard/AntiBERTa2_getLogits.py` & `penguindashboard-1.0.7/penguindashboard/AntiBERTa2_getLogits.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,28 +35,27 @@
             if aa in key:
                 aa_ls.append(item)
         new_nplogits.append(np.sum(nplogits[1:-1,aa_ls],axis=1))
     new_nplogits = np.array(new_nplogits).T
     np.save(f'{output_prefix}.logits.AntiBERTa2.npy', new_nplogits)
 
 def main():
-    parser = argparse.ArgumentParser(description='Process amino acid sequences using AntiBERTa2 model.')
-    parser.add_argument('--amino_acid_str', type=str, help='Amino acid sequence')
-    parser.add_argument('--output_prefix', type=str, help='Optional prefix to add to the output filename',default = '')
-    parser.add_argument('--device', type=str, help='Specify the Cuda device index',default = '0')
-
-    args = parser.parse_args()
     amino_acid_str = args.amino_acid_str
     output_prefix = args.output_prefix
     device = args.device
 
     model, tokenizer = load_model()
     device = torch.device("cuda:"+device if torch.cuda.is_available() else "cpu")
     model = model.to(device)
     batch_tokens = tokenize_sequences(amino_acid_str, tokenizer, device)
 
     nplogits = process_sequences(model, batch_tokens)
     standardize_vocab(tokenizer,nplogits,output_prefix)
 
 if __name__ == "__main__":
-    main()
-    
+    parser = argparse.ArgumentParser(description='Process amino acid sequences using AntiBERTa2 model.')
+    parser.add_argument('--amino_acid_str', type=str, help='Amino acid sequence')
+    parser.add_argument('--output_prefix', type=str, help='Optional prefix to add to the output filename',default = '')
+    parser.add_argument('--device', type=str, help='Specify the Cuda device index',default = '0')
+    args = parser.parse_args()
+    
+    main(args)
```

### Comparing `penguindashboard-1.0.6/penguindashboard/BLAST_phylo.py` & `penguindashboard-1.0.7/penguindashboard/BLAST_phylo.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,17 @@
     # softmax across columns
     percentage_df = percentage_df.div(percentage_df.sum(axis=1), axis=0)
 
     return percentage_df
 
 
 def main(args):
+    os.makedirs(args.outdir, exist_ok=True)
+    os.makedirs(args.outdir + '/BLAST', exist_ok=True)
+
     xml_blast = perform_blast_search(args.sequence)
     blast_record = parse_blast_xml(xml_blast)
     df = create_df(blast_record, args.sequence)
     write_sequences(df)
     perform_msa()
     df = calculate_percentages()
     
@@ -88,13 +91,10 @@
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description='BLAST search and analysis')
     parser.add_argument('--sequence', type=str, required=True, help='Amino acid sequence for BLAST search')
     parser.add_argument('--outdir', type=str, required=True, help='Output directory for results')
     parser.add_argument('--name', type=str, required=True, help='Name of the sequence')
     args = parser.parse_args()
-    # create directory if it does not exist
-    os.makedirs(args.outdir, exist_ok=True)
-    os.makedirs(args.outdir + '/BLAST', exist_ok=True)
 
     main(args)
```

### Comparing `penguindashboard-1.0.6/penguindashboard/ESM2_getLogits.py` & `penguindashboard-1.0.7/penguindashboard/ESM2_getLogits.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,30 +46,31 @@
 
     new_nplogits = []
     for aa in amino_acids:
         new_nplogits.append(nplogits[1:-1,filtered_vocab[aa]])
     new_nplogits = np.array(new_nplogits).T
     np.save(f'{output_prefix}.logits.{model_choice}.npy', new_nplogits)
 
-def main():
-    parser = argparse.ArgumentParser(description='Process sequences using ESM-2 model.')
-    parser.add_argument('--sequence', type=str, help='Sequence to pass through ESM-2 model')
-    parser.add_argument('--model_choice', type=str, help='Choice of ESM2 model. Options: [esm2_t48_15B_UR50D, esm2_t36_3B_UR50D, esm2_t33_650M_UR50D] Default: esm2_t33_650M_UR50D', default = 'esm2_t33_650M_UR50D')
-    parser.add_argument('--output_prefix', type=str, help='Optional prefix to add to the output filename')
-    parser.add_argument('--device', type=str, help='Specify the Cuda device index', default = '0')
+def main(args):
 
-    args = parser.parse_args()
     sequence = args.sequence
     model_choice = args.model_choice
     output_prefix = args.output_prefix
     device = args.device
 
     model, tokenizer = load_model(model_choice)
     device = torch.device(f"cuda:{device}" if torch.cuda.is_available() else "cpu")
     model = model.to(device)
     tokens = tokenize_sequences(sequence, tokenizer, device)
 
     nplogits = process_sequences(model, tokens)
     standardize_vocab(tokenizer,nplogits,model_choice,output_prefix)
 
 if __name__ == "__main__":
-    main()
+    parser = argparse.ArgumentParser(description='Process sequences using ESM-2 model.')
+    parser.add_argument('--sequence', type=str, help='Sequence to pass through ESM-2 model')
+    parser.add_argument('--model_choice', type=str, help='Choice of ESM2 model. Options: [esm2_t48_15B_UR50D, esm2_t36_3B_UR50D, esm2_t33_650M_UR50D] Default: esm2_t33_650M_UR50D', default = 'esm2_t33_650M_UR50D')
+    parser.add_argument('--output_prefix', type=str, help='Optional prefix to add to the output filename')
+    parser.add_argument('--device', type=str, help='Specify the Cuda device index', default = '0')
+
+    args = parser.parse_args()
+    main(args)
```

### Comparing `penguindashboard-1.0.6/penguindashboard/ProteinMPNN_getLogits.py` & `penguindashboard-1.0.7/penguindashboard/ProteinMPNN_getLogits.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,29 +40,30 @@
     new_nplogits = []
     for aa in amino_acids:
         new_nplogits.append(nplogits[:,mpnn_alphabet[aa]])
     new_nplogits = np.array(new_nplogits).T
     np.save(f'{output_prefix}/{pdb_file.split("/")[-1].split(".")[0]}.logits.ProteinMPNN_v_48_020.npy', new_nplogits)
 
 def main():
-    parser = argparse.ArgumentParser(description='Process amino acid and 3Di sequences using SaProt model.')
-    parser.add_argument('--proteinmpnn_dir', type=str, help='Path to the proteinmpnn directory')
-    parser.add_argument('--pdb_file', type=str, help='Path to the pdb file')
-    parser.add_argument('--output_prefix', type=str, help='Optional prefix to add to the output filename')
-    parser.add_argument('--device', type=str, help='Specify the Cuda device index', default = '0')
-
-    args = parser.parse_args()
     proteinmpnn_dir = args.proteinmpnn_dir
     pdb_file = args.pdb_file
     output_prefix = args.output_prefix
     device = args.device
 
     # make directory {output_prefix}/ProteinMPNN/ if it does not exist
     os.makedirs(f'{output_prefix}/ProteinMPNN/', exist_ok=True)
 
     nplogits = run_mpnn(proteinmpnn_dir, pdb_file, device, output_prefix).astype(np.float128)
     
     standardize_vocab(nplogits, output_prefix, pdb_file)
 
 
 if __name__ == "__main__":
-    main()
+    parser = argparse.ArgumentParser(description='Process amino acid and 3Di sequences using SaProt model.')
+    parser.add_argument('--proteinmpnn_dir', type=str, help='Path to the proteinmpnn directory')
+    parser.add_argument('--pdb_file', type=str, help='Path to the pdb file')
+    parser.add_argument('--output_prefix', type=str, help='Optional prefix to add to the output filename')
+    parser.add_argument('--device', type=str, help='Specify the Cuda device index', default = '0')
+
+    args = parser.parse_args()
+
+    main(args)
```

### Comparing `penguindashboard-1.0.6/penguindashboard/SaProt_getLogits.py` & `penguindashboard-1.0.7/penguindashboard/SaProt_getLogits.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,21 +60,14 @@
         new_nplogits.append(np.sum(nplogits[1:-1,aa_ls],axis=1))
     new_nplogits = np.array(new_nplogits).T
     
     np.save(f'{output_prefix}.logits.SaProt_650M_PDB.npy', new_nplogits)
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Process amino acid and 3Di sequences using SaProt model.')
-    parser.add_argument('--amino_acid_str', type=str, help='Amino acid sequence')
-    parser.add_argument('--foldseek_tokens', type=str, help='Path to the amino acid fasta file')
-    parser.add_argument('--output_prefix', type=str, help='Optional prefix to add to the output filename',default = '')
-    parser.add_argument('--device', type=str, help='Specify the Cuda device index',default = '0')
-
-    args = parser.parse_args()
     amino_acid_str = args.amino_acid_str
     foldseek_tokens_input = args.foldseek_tokens
     output_prefix = args.output_prefix
     device = args.device
 
     model, tokenizer = load_model()
     device = torch.device("cuda:"+device if torch.cuda.is_available() else "cpu")
@@ -83,9 +76,17 @@
     data = combine_data(amino_acid_str, foldseek_str)
     batch_tokens = tokenize_sequences(data, tokenizer,device)
 
     nplogits = process_sequences(model, batch_tokens)
     standardize_vocab(tokenizer,nplogits,output_prefix)
 
 if __name__ == "__main__":
-    main()
+    parser = argparse.ArgumentParser(description='Process amino acid and 3Di sequences using SaProt model.')
+    parser.add_argument('--amino_acid_str', type=str, help='Amino acid sequence')
+    parser.add_argument('--foldseek_tokens', type=str, help='Path to the amino acid fasta file')
+    parser.add_argument('--output_prefix', type=str, help='Optional prefix to add to the output filename',default = '')
+    parser.add_argument('--device', type=str, help='Specify the Cuda device index',default = '0')
+
+    args = parser.parse_args()
+
+    main(args)
```

### Comparing `penguindashboard-1.0.6/penguindashboard/edit_mutcompute_output.py` & `penguindashboard-1.0.7/penguindashboard/edit_mutcompute_output.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.6/penguindashboard/esm_fold.py` & `penguindashboard-1.0.7/penguindashboard/esm_fold.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.6/penguindashboard/pipeline.py` & `penguindashboard-1.0.7/penguindashboard/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,37 +33,37 @@
 
     if args.saprot:
         os.makedirs(f"{args.output_dir}/foldseek", exist_ok=True)
         subprocess.run(f"foldseek createdb {pdb_file} {args.output_dir}/foldseek/{name} -v 1", shell=True)
         subprocess.run(f"foldseek lndb {args.output_dir}/foldseek/{name}_h {args.output_dir}/foldseek/{name}_ss_h -v 1", shell=True)
         subprocess.run(f"foldseek convert2fasta {args.output_dir}/foldseek/{name}_ss {args.output_dir}/foldseek/{name}_ss.fasta -v 1", shell=True)
         print("Running SaProt...")
-        subprocess.run(f"python3 {script_dir}/SaProt_getLogits.py --amino_acid_str {seq} --foldseek_tokens {args.output_dir}/foldseek/{name}_ss.fasta --output_prefix {args.output_dir}/{name} --device {args.device}", shell=True)
+        subprocess.run(f"python3 {script_dir}/SaProt_getLogits.py --amino_acid_str {seq} --foldseek_tokens {args.output_dir}/foldseek/{name}_ss.fasta --output_prefix {args.output_dir}/{name}", shell=True)
 
     if args.antiberta:
         print("Running AntiBERTa2...")
-        subprocess.run(f"python3 {script_dir}/AntiBERTa2_getLogits.py --amino_acid_str {seq} --output_prefix {args.output_dir}/{name} --device {args.device}", shell=True)
+        subprocess.run(f"python3 {script_dir}/AntiBERTa2_getLogits.py --amino_acid_str {seq} --output_prefix {args.output_dir}/{name}", shell=True)
 
     if args.esm:
         print("Running ESM2 (650M)...")
-        subprocess.run(f"python3 {script_dir}/ESM2_getLogits.py --sequence {seq} --model_choice esm2_t33_650M_UR50D --output_prefix {args.output_dir}/{name} --device {args.device}", shell=True)
+        subprocess.run(f"python3 {script_dir}/ESM2_getLogits.py --sequence {seq} --model_choice esm2_t33_650M_UR50D --output_prefix {args.output_dir}/{name}", shell=True)
 
     if args.proteinmpnn:
         proteinmpnn_dir = os.path.join(args.output_dir, "../LigandMPNN")
         if not os.path.isdir(proteinmpnn_dir):
             print("Setting up ProteinMPNN...")
             subprocess.run(f"git clone https://github.com/dauparas/LigandMPNN.git {proteinmpnn_dir}", shell=True)
             os.makedirs(f"{proteinmpnn_dir}/model_params", exist_ok=True)
             subprocess.run(f"wget https://github.com/dauparas/ProteinMPNN/raw/main/vanilla_model_weights/v_48_020.pt -P {proteinmpnn_dir}/model_params", shell=True)
             subprocess.run(f"cp {script_dir}/score.py {proteinmpnn_dir}/score.py", shell=True)
         else:
             print("ProteinMPNN already set up.")
 
         print("Running ProteinMPNN...")
-        subprocess.run(f"python3 {script_dir}/ProteinMPNN_getLogits.py --output_prefix {args.output_dir} --proteinmpnn_dir {proteinmpnn_dir} --pdb_file {pdb_file} --device {args.device}", shell=True)
+        subprocess.run(f"python3 {script_dir}/ProteinMPNN_getLogits.py --output_prefix {args.output_dir} --proteinmpnn_dir {proteinmpnn_dir} --pdb_file {pdb_file}", shell=True)
 
     if args.blast:
         print("Running BLAST phylogeny...")
         subprocess.run(f"python3 {script_dir}/BLAST_phylo.py --outdir {args.output_dir} --sequence {seq} --name {name}", shell=True)
 
 
     ### MUTCOMPUTE SECITON ###
```

### Comparing `penguindashboard-1.0.6/penguindashboard/score.py` & `penguindashboard-1.0.7/penguindashboard/score.py`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.6/penguindashboard.egg-info/PKG-INFO` & `penguindashboard-1.0.7/penguindashboard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: penguindashboard
-Version: 1.0.6
+Version: 1.0.7
 Summary: PEngUIN: Protein Engineering Using Independent Networks
 Home-page: https://github.com/AaronFeller/PEngUIN
 Author: Aaron Feller, Phillip Woolley
 Author-email: aaronleefeller@gmail.com, prwoolley@utexas.edu
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `penguindashboard-1.0.6/penguindashboard.egg-info/SOURCES.txt` & `penguindashboard-1.0.7/penguindashboard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `penguindashboard-1.0.6/setup.py` & `penguindashboard-1.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 this_directory = os.path.abspath(os.path.dirname(__file__))
 # Text of the README file
 with open(os.path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='penguindashboard',
-    version='1.0.6',
+    version='1.0.7',
     author='Aaron Feller, Phillip Woolley',
     author_email='aaronleefeller@gmail.com, prwoolley@utexas.edu',
     description='PEngUIN: Protein Engineering Using Independent Networks',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/AaronFeller/PEngUIN',
     license='MIT',
```

