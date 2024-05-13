# Comparing `tmp/clipzyme-0.0.8.tar.gz` & `tmp/clipzyme-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clipzyme-0.0.8.tar", max compression
+gzip compressed data, was "clipzyme-0.0.9.tar", max compression
```

## Comparing `clipzyme-0.0.8.tar` & `clipzyme-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0    11358 2024-03-28 18:26:04.343837 clipzyme-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     8681 2024-05-13 02:35:50.325862 clipzyme-0.0.8/README.md
--rw-r--r--   0        0        0     1788 2024-03-29 19:24:34.636971 clipzyme-0.0.8/clipzyme/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.578850 clipzyme-0.0.8/clipzyme/callbacks/__init__.py
--rw-r--r--   0        0        0      948 2024-03-28 15:53:13.579321 clipzyme-0.0.8/clipzyme/callbacks/basic.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.579397 clipzyme-0.0.8/clipzyme/datasets/__init__.py
--rw-r--r--   0        0        0     8552 2024-03-28 15:53:13.579934 clipzyme-0.0.8/clipzyme/datasets/abstract.py
--rw-r--r--   0        0        0    12769 2024-03-28 15:53:13.580656 clipzyme-0.0.8/clipzyme/datasets/enzyme_screening.py
--rw-r--r--   0        0        0    43705 2024-04-08 16:54:12.470132 clipzyme-0.0.8/clipzyme/datasets/enzymemap.py
--rw-r--r--   0        0        0    11861 2024-05-13 02:35:50.326101 clipzyme-0.0.8/clipzyme/datasets/reaction.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.581466 clipzyme-0.0.8/clipzyme/learning/losses/__init__.py
--rw-r--r--   0        0        0    10857 2024-03-28 15:53:13.581946 clipzyme-0.0.8/clipzyme/learning/losses/basic.py
--rw-r--r--   0        0        0    17891 2024-03-28 18:04:43.398133 clipzyme-0.0.8/clipzyme/learning/losses/contrastive.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.582586 clipzyme-0.0.8/clipzyme/learning/metrics/__init__.py
--rw-r--r--   0        0        0    20086 2024-03-28 15:53:13.582961 clipzyme-0.0.8/clipzyme/learning/metrics/basic.py
--rw-r--r--   0        0        0     6590 2024-03-28 15:53:13.583284 clipzyme-0.0.8/clipzyme/learning/metrics/representation.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583361 clipzyme-0.0.8/clipzyme/learning/optimizers/__init__.py
--rw-r--r--   0        0        0     2406 2024-03-28 15:53:13.583673 clipzyme-0.0.8/clipzyme/learning/optimizers/basic.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583744 clipzyme-0.0.8/clipzyme/learning/schedulers/__init__.py
--rw-r--r--   0        0        0     1855 2024-03-28 15:53:13.583927 clipzyme-0.0.8/clipzyme/learning/schedulers/basic.py
--rw-r--r--   0        0        0     6835 2024-03-28 18:04:43.397866 clipzyme-0.0.8/clipzyme/learning/schedulers/warmup.py
--rw-r--r--   0        0        0      122 2024-03-28 15:53:13.584578 clipzyme-0.0.8/clipzyme/learning/utils.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.584651 clipzyme-0.0.8/clipzyme/lightning/__init__.py
--rw-r--r--   0        0        0    21181 2024-03-28 15:53:13.584896 clipzyme-0.0.8/clipzyme/lightning/base.py
--rw-r--r--   0        0        0    12789 2024-05-10 20:56:23.614929 clipzyme-0.0.8/clipzyme/lightning/clipzyme.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585018 clipzyme-0.0.8/clipzyme/loggers/__init__.py
--rw-r--r--   0        0        0      637 2024-03-28 15:53:13.585360 clipzyme-0.0.8/clipzyme/loggers/tensorboard.py
--rw-r--r--   0        0        0     2254 2024-03-28 15:53:13.585569 clipzyme-0.0.8/clipzyme/loggers/wandb.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585646 clipzyme-0.0.8/clipzyme/models/__init__.py
--rw-r--r--   0        0        0      300 2024-03-28 15:53:13.585810 clipzyme-0.0.8/clipzyme/models/abstract.py
--rw-r--r--   0        0        0     7144 2024-03-28 15:53:13.585987 clipzyme-0.0.8/clipzyme/models/chemprop.py
--rw-r--r--   0        0        0     7285 2024-03-28 15:53:13.586155 clipzyme-0.0.8/clipzyme/models/classifier.py
--rw-r--r--   0        0        0    29102 2024-03-28 15:53:13.586482 clipzyme-0.0.8/clipzyme/models/egnn.py
--rw-r--r--   0        0        0     6917 2024-03-28 15:53:13.586943 clipzyme-0.0.8/clipzyme/models/fair_esm.py
--rw-r--r--   0        0        0    10220 2024-03-28 15:53:13.587252 clipzyme-0.0.8/clipzyme/models/gat.py
--rw-r--r--   0        0        0    28859 2024-03-29 19:38:31.847201 clipzyme-0.0.8/clipzyme/models/protmol.py
--rw-r--r--   0        0        0     5331 2024-03-28 15:53:13.588426 clipzyme-0.0.8/clipzyme/models/seq2seq.py
--rw-r--r--   0        0        0    24182 2024-03-28 15:53:13.588821 clipzyme-0.0.8/clipzyme/models/wln.py
--rw-r--r--   0        0        0        0 2024-03-28 15:53:13.588932 clipzyme-0.0.8/clipzyme/utils/__init__.py
--rw-r--r--   0        0        0     1891 2024-03-28 15:53:13.589041 clipzyme-0.0.8/clipzyme/utils/amino_acids.py
--rw-r--r--   0        0        0     1679 2024-03-28 15:53:13.589238 clipzyme-0.0.8/clipzyme/utils/callbacks.py
--rw-r--r--   0        0        0     3669 2024-03-28 15:53:13.589424 clipzyme-0.0.8/clipzyme/utils/classes.py
--rw-r--r--   0        0        0     8793 2024-03-28 18:04:43.397858 clipzyme-0.0.8/clipzyme/utils/colabfold_msa.py
--rw-r--r--   0        0        0    11554 2024-03-28 15:53:13.589737 clipzyme-0.0.8/clipzyme/utils/loading.py
--rw-r--r--   0        0        0      154 2024-03-28 15:53:13.589922 clipzyme-0.0.8/clipzyme/utils/messages.py
--rw-r--r--   0        0        0    22189 2024-03-28 15:53:13.590443 clipzyme-0.0.8/clipzyme/utils/parsing.py
--rw-r--r--   0        0        0    13604 2024-04-08 17:00:53.080799 clipzyme-0.0.8/clipzyme/utils/protein_utils.py
--rw-r--r--   0        0        0    15629 2024-03-28 18:04:43.398175 clipzyme-0.0.8/clipzyme/utils/proteins.py
--rw-r--r--   0        0        0    13289 2024-03-28 15:53:13.591225 clipzyme-0.0.8/clipzyme/utils/pyg.py
--rw-r--r--   0        0        0    17957 2024-03-28 18:04:43.399109 clipzyme-0.0.8/clipzyme/utils/reactions.py
--rw-r--r--   0        0        0     1187 2024-03-28 15:53:13.591465 clipzyme-0.0.8/clipzyme/utils/registry.py
--rw-r--r--   0        0        0     4638 2024-03-28 15:53:13.591739 clipzyme-0.0.8/clipzyme/utils/sampler.py
--rw-r--r--   0        0        0     4897 2024-04-08 16:56:54.314023 clipzyme-0.0.8/clipzyme/utils/screening.py
--rw-r--r--   0        0        0    22325 2024-03-28 15:53:13.591875 clipzyme-0.0.8/clipzyme/utils/smiles.py
--rw-r--r--   0        0        0    48101 2024-03-28 18:04:43.399645 clipzyme-0.0.8/clipzyme/utils/wln_processing.py
--rw-r--r--   0        0        0      623 2024-05-13 02:37:04.085962 clipzyme-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     9206 1970-01-01 00:00:00.000000 clipzyme-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-28 18:26:04.343837 clipzyme-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     8681 2024-05-13 20:48:35.586381 clipzyme-0.0.9/README.md
+-rw-r--r--   0        0        0     1788 2024-03-29 19:24:34.636971 clipzyme-0.0.9/clipzyme/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.578850 clipzyme-0.0.9/clipzyme/callbacks/__init__.py
+-rw-r--r--   0        0        0      948 2024-03-28 15:53:13.579321 clipzyme-0.0.9/clipzyme/callbacks/basic.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.579397 clipzyme-0.0.9/clipzyme/datasets/__init__.py
+-rw-r--r--   0        0        0     8552 2024-03-28 15:53:13.579934 clipzyme-0.0.9/clipzyme/datasets/abstract.py
+-rw-r--r--   0        0        0    12769 2024-03-28 15:53:13.580656 clipzyme-0.0.9/clipzyme/datasets/enzyme_screening.py
+-rw-r--r--   0        0        0    42315 2024-05-13 18:54:25.485241 clipzyme-0.0.9/clipzyme/datasets/enzymemap.py
+-rw-r--r--   0        0        0    11861 2024-05-13 02:35:50.326101 clipzyme-0.0.9/clipzyme/datasets/reaction.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.581466 clipzyme-0.0.9/clipzyme/learning/losses/__init__.py
+-rw-r--r--   0        0        0    10857 2024-03-28 15:53:13.581946 clipzyme-0.0.9/clipzyme/learning/losses/basic.py
+-rw-r--r--   0        0        0    17891 2024-03-28 18:04:43.398133 clipzyme-0.0.9/clipzyme/learning/losses/contrastive.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.582586 clipzyme-0.0.9/clipzyme/learning/metrics/__init__.py
+-rw-r--r--   0        0        0    20086 2024-03-28 15:53:13.582961 clipzyme-0.0.9/clipzyme/learning/metrics/basic.py
+-rw-r--r--   0        0        0     6590 2024-03-28 15:53:13.583284 clipzyme-0.0.9/clipzyme/learning/metrics/representation.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583361 clipzyme-0.0.9/clipzyme/learning/optimizers/__init__.py
+-rw-r--r--   0        0        0     2406 2024-03-28 15:53:13.583673 clipzyme-0.0.9/clipzyme/learning/optimizers/basic.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.583744 clipzyme-0.0.9/clipzyme/learning/schedulers/__init__.py
+-rw-r--r--   0        0        0     1855 2024-03-28 15:53:13.583927 clipzyme-0.0.9/clipzyme/learning/schedulers/basic.py
+-rw-r--r--   0        0        0     6835 2024-03-28 18:04:43.397866 clipzyme-0.0.9/clipzyme/learning/schedulers/warmup.py
+-rw-r--r--   0        0        0      122 2024-03-28 15:53:13.584578 clipzyme-0.0.9/clipzyme/learning/utils.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.584651 clipzyme-0.0.9/clipzyme/lightning/__init__.py
+-rw-r--r--   0        0        0    21181 2024-03-28 15:53:13.584896 clipzyme-0.0.9/clipzyme/lightning/base.py
+-rw-r--r--   0        0        0    12789 2024-05-13 20:48:30.324026 clipzyme-0.0.9/clipzyme/lightning/clipzyme.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585018 clipzyme-0.0.9/clipzyme/loggers/__init__.py
+-rw-r--r--   0        0        0      637 2024-03-28 15:53:13.585360 clipzyme-0.0.9/clipzyme/loggers/tensorboard.py
+-rw-r--r--   0        0        0     2254 2024-03-28 15:53:13.585569 clipzyme-0.0.9/clipzyme/loggers/wandb.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.585646 clipzyme-0.0.9/clipzyme/models/__init__.py
+-rw-r--r--   0        0        0      300 2024-03-28 15:53:13.585810 clipzyme-0.0.9/clipzyme/models/abstract.py
+-rw-r--r--   0        0        0     7144 2024-03-28 15:53:13.585987 clipzyme-0.0.9/clipzyme/models/chemprop.py
+-rw-r--r--   0        0        0     7285 2024-03-28 15:53:13.586155 clipzyme-0.0.9/clipzyme/models/classifier.py
+-rw-r--r--   0        0        0    29102 2024-03-28 15:53:13.586482 clipzyme-0.0.9/clipzyme/models/egnn.py
+-rw-r--r--   0        0        0     6917 2024-03-28 15:53:13.586943 clipzyme-0.0.9/clipzyme/models/fair_esm.py
+-rw-r--r--   0        0        0    10220 2024-03-28 15:53:13.587252 clipzyme-0.0.9/clipzyme/models/gat.py
+-rw-r--r--   0        0        0    28859 2024-03-29 19:38:31.847201 clipzyme-0.0.9/clipzyme/models/protmol.py
+-rw-r--r--   0        0        0     5331 2024-03-28 15:53:13.588426 clipzyme-0.0.9/clipzyme/models/seq2seq.py
+-rw-r--r--   0        0        0    24182 2024-03-28 15:53:13.588821 clipzyme-0.0.9/clipzyme/models/wln.py
+-rw-r--r--   0        0        0        0 2024-03-28 15:53:13.588932 clipzyme-0.0.9/clipzyme/utils/__init__.py
+-rw-r--r--   0        0        0     1891 2024-03-28 15:53:13.589041 clipzyme-0.0.9/clipzyme/utils/amino_acids.py
+-rw-r--r--   0        0        0     1679 2024-03-28 15:53:13.589238 clipzyme-0.0.9/clipzyme/utils/callbacks.py
+-rw-r--r--   0        0        0     3669 2024-03-28 15:53:13.589424 clipzyme-0.0.9/clipzyme/utils/classes.py
+-rw-r--r--   0        0        0     8793 2024-03-28 18:04:43.397858 clipzyme-0.0.9/clipzyme/utils/colabfold_msa.py
+-rw-r--r--   0        0        0    11554 2024-03-28 15:53:13.589737 clipzyme-0.0.9/clipzyme/utils/loading.py
+-rw-r--r--   0        0        0      154 2024-03-28 15:53:13.589922 clipzyme-0.0.9/clipzyme/utils/messages.py
+-rw-r--r--   0        0        0    22189 2024-03-28 15:53:13.590443 clipzyme-0.0.9/clipzyme/utils/parsing.py
+-rw-r--r--   0        0        0    13604 2024-04-08 17:00:53.080799 clipzyme-0.0.9/clipzyme/utils/protein_utils.py
+-rw-r--r--   0        0        0    15629 2024-03-28 18:04:43.398175 clipzyme-0.0.9/clipzyme/utils/proteins.py
+-rw-r--r--   0        0        0    13289 2024-03-28 15:53:13.591225 clipzyme-0.0.9/clipzyme/utils/pyg.py
+-rw-r--r--   0        0        0    17957 2024-03-28 18:04:43.399109 clipzyme-0.0.9/clipzyme/utils/reactions.py
+-rw-r--r--   0        0        0     1187 2024-03-28 15:53:13.591465 clipzyme-0.0.9/clipzyme/utils/registry.py
+-rw-r--r--   0        0        0     4638 2024-03-28 15:53:13.591739 clipzyme-0.0.9/clipzyme/utils/sampler.py
+-rw-r--r--   0        0        0     4897 2024-04-08 16:56:54.314023 clipzyme-0.0.9/clipzyme/utils/screening.py
+-rw-r--r--   0        0        0    22325 2024-03-28 15:53:13.591875 clipzyme-0.0.9/clipzyme/utils/smiles.py
+-rw-r--r--   0        0        0    48101 2024-03-28 18:04:43.399645 clipzyme-0.0.9/clipzyme/utils/wln_processing.py
+-rw-r--r--   0        0        0      623 2024-05-13 19:19:23.198639 clipzyme-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     9206 1970-01-01 00:00:00.000000 clipzyme-0.0.9/PKG-INFO
```

### Comparing `clipzyme-0.0.8/LICENSE.txt` & `clipzyme-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/README.md` & `clipzyme-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -43,32 +43,32 @@
 3. Download ESM-2 checkpoint `esm2_t33_650M_UR50D`. The `esm_dir` argument should point to this directory. The following command will download the checkpoint directly:
 ```bash
 wget https://dl.fbaipublicfiles.com/fair-esm/models/esm2_t33_650M_UR50D.pt
 ```
 
 # Checkpoints and Data Files:
 
-The model checkpoint and data are available on Zenodo [here](https://zenodo.org/records/10950376):
+The model checkpoint and data are available on Zenodo [here](https://zenodo.org/records/11187895):
 
-- [clipzyme_data.zip](https://zenodo.org/records/10950376/files/clipzyme_data.zip?download=1):
+- [clipzyme_data.zip](https://zenodo.org/records/11187895/files/clipzyme_data.zip?download=1):
   - The following commands will download the checkpoint directly: 
   ```
-  wget https://zenodo.org/records/10950376/files/clipzyme_data.zip
+  wget https://zenodo.org/records/11187895/files/clipzyme_data.zip
   unzip clipzyme_data.zip -d files
   ```
   - Note that the data files should be extracted into the `files/` directory.
       - `enzymemap.json`: contains the EnzymeMap dataset.
       - `cached_enzymemap.p`: contains the processed EnzymeMap dataset.
       - `clipzyme_screening_set.p`: contains the screening set as dict of UniProt IDs and precomputed protein embeddings.
       - `uniprot2sequence.p`: contains the mapping form sequence ID to amino acids.
 
-- [clipzyme_model.zip](https://zenodo.org/records/10950376/files/clipzyme_model.zip?download=1):
+- [clipzyme_model.zip](https://zenodo.org/records/11187895/files/clipzyme_model.zip?download=1):
   - The following command will download the checkpoint directly: 
   ```
-  wget https://zenodo.org/records/10950376/files/clipzyme_model.zip
+  wget https://zenodo.org/records/11187895/files/clipzyme_model.zip
   unzip clipzyme_model.zip -d files
   ```
     - `clipzyme_model.ckpt`: the trained model checkpoint.
 
 
 
 # Screening with CLIPZyme
@@ -191,15 +191,15 @@
 
 ## Data processing
 
 We obtain the data from the following sources:
 - [EnzymeMap:](`https://doi.org/10.5281/zenodo.7841780`) Heid et al. Enzymemap: Curation, validation and data-driven prediction of enzymatic reactions. 2023.
 - [Terpene Synthases:](`https://zenodo.org/records/10567437`) Samusevich et al. Discovery and characterization of terpene synthases powered by machine learning. 2024. 
 
-Our processed data is can be downloaded from [here](https://zenodo.org/records/10950376). 
+Our processed data is can be downloaded from [here](https://zenodo.org/records/11187895). 
 
 
 ## Training and evaluation
 1. To train the models presented in the tables below, run the following command:
     ```
     python scripts/dispatcher.py -c {config_path} -l {log_path}
     ```
```

### Comparing `clipzyme-0.0.8/clipzyme/__init__.py` & `clipzyme-0.0.9/clipzyme/__init__.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/callbacks/basic.py` & `clipzyme-0.0.9/clipzyme/callbacks/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/datasets/abstract.py` & `clipzyme-0.0.9/clipzyme/datasets/abstract.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/datasets/enzyme_screening.py` & `clipzyme-0.0.9/clipzyme/datasets/enzyme_screening.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/datasets/enzymemap.py` & `clipzyme-0.0.9/clipzyme/datasets/enzymemap.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,41 +85,14 @@
 
         self.ec2uniprot = pickle.load(open("files/ec2uniprot.p", "rb"))
         self.uniprot2sequence = pickle.load(open("files/uniprot2sequence.p", "rb"))
         self.uniprot2sequence_len = {
             k: 0 if v is None else len(v) for k, v in self.uniprot2sequence.items()
         }
 
-        # products to remove based on smiles or pattern
-        remove_patterns_path = "files/ecreact/patterns.txt"
-        remove_molecules_path = "files/ecreact/molecules.txt"
-
-        self.remove_patterns = []
-        self.remove_molecules = []
-
-        for line in open(remove_patterns_path):
-            if not line.startswith("//") and line.strip():
-                self.remove_patterns.append(line.split("//")[0].strip())
-
-        self.remove_patterns = [
-            rdk.MolFromSmarts(smart_pattern) for smart_pattern in self.remove_patterns
-        ]
-
-        for line in open(remove_molecules_path):
-            if not line.startswith("//") and line.strip():
-                smiles = line.split("//")[0].strip()
-                mol = rdk.MolFromSmiles(smiles)
-                if mol:
-                    self.remove_molecules.append(rdk.MolToSmiles(mol))
-                    self.remove_molecules.append(
-                        Chem.CanonSmiles(
-                            self.remove_molecules[-1].replace("[O-]", "[OH]")
-                        )
-                    )
-
     def create_dataset(
         self, split_group: Literal["train", "dev", "test"]
     ) -> List[dict]:
         # if removing top K
         if self.args.topk_byproducts_to_remove is not None:
             raw_byproducts = Counter(
                 [r for d in self.metadata_json for r in d["products"]]
@@ -418,23 +391,14 @@
         # set ec levels to id for use in modeling
         ecs = [d["ec"].split(".") for d in self.dataset]
         args.ec_levels = {}
         for level in range(1, 5, 1):
             unique_classes = sorted(list(set(".".join(ec[:level]) for ec in ecs)))
             args.ec_levels[str(level)] = {c: i for i, c in enumerate(unique_classes)}
 
-    def remove_from_products(self, product):
-        mol = Chem.MolFromSmiles(product)
-        for mol_pattern in self.remove_patterns:
-            if mol.HasSubstructMatch(mol_pattern):
-                return True
-        if product in self.remove_molecules:
-            return True
-        return False
-
     def create_protein_graph(self, sample):
         try:
             raw_path = os.path.join(
                 self.args.protein_structures_dir,
                 f"AF-{sample['uniprot_id']}-F1-model_v4.cif",
             )
             protein_args = {
```

### Comparing `clipzyme-0.0.8/clipzyme/datasets/reaction.py` & `clipzyme-0.0.9/clipzyme/datasets/reaction.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/learning/losses/basic.py` & `clipzyme-0.0.9/clipzyme/learning/losses/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/learning/losses/contrastive.py` & `clipzyme-0.0.9/clipzyme/learning/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/learning/metrics/basic.py` & `clipzyme-0.0.9/clipzyme/learning/metrics/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/learning/metrics/representation.py` & `clipzyme-0.0.9/clipzyme/learning/metrics/representation.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/learning/optimizers/basic.py` & `clipzyme-0.0.9/clipzyme/learning/optimizers/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/learning/schedulers/basic.py` & `clipzyme-0.0.9/clipzyme/learning/schedulers/basic.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/learning/schedulers/warmup.py` & `clipzyme-0.0.9/clipzyme/learning/schedulers/warmup.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/lightning/base.py` & `clipzyme-0.0.9/clipzyme/lightning/base.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/lightning/clipzyme.py` & `clipzyme-0.0.9/clipzyme/lightning/clipzyme.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pytorch_lightning as pl
 import argparse
 from clipzyme.models.protmol import EnzymeReactionCLIP
 from clipzyme.utils.screening import process_mapped_reaction
 from clipzyme.utils.protein_utils import create_protein_graph
 from clipzyme.utils.loading import default_collate
 
-CHECKPOINT_URL = "https://zenodo.org/records/10950376/files/clipzyme_model.zip"
+CHECKPOINT_URL = "https://zenodo.org/records/11187895/files/clipzyme_model.zip"
 
 
 def download_and_extract(remote_model_url: str, local_model_dir: str) -> str:
     """
     Download and extract model.
 
     Parameters
```

### Comparing `clipzyme-0.0.8/clipzyme/loggers/tensorboard.py` & `clipzyme-0.0.9/clipzyme/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/loggers/wandb.py` & `clipzyme-0.0.9/clipzyme/loggers/wandb.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/models/chemprop.py` & `clipzyme-0.0.9/clipzyme/models/chemprop.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/models/classifier.py` & `clipzyme-0.0.9/clipzyme/models/classifier.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/models/egnn.py` & `clipzyme-0.0.9/clipzyme/models/egnn.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/models/fair_esm.py` & `clipzyme-0.0.9/clipzyme/models/fair_esm.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/models/gat.py` & `clipzyme-0.0.9/clipzyme/models/gat.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/models/protmol.py` & `clipzyme-0.0.9/clipzyme/models/protmol.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/models/seq2seq.py` & `clipzyme-0.0.9/clipzyme/models/seq2seq.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/models/wln.py` & `clipzyme-0.0.9/clipzyme/models/wln.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/amino_acids.py` & `clipzyme-0.0.9/clipzyme/utils/amino_acids.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/callbacks.py` & `clipzyme-0.0.9/clipzyme/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/classes.py` & `clipzyme-0.0.9/clipzyme/utils/classes.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/colabfold_msa.py` & `clipzyme-0.0.9/clipzyme/utils/colabfold_msa.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/loading.py` & `clipzyme-0.0.9/clipzyme/utils/loading.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/parsing.py` & `clipzyme-0.0.9/clipzyme/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/protein_utils.py` & `clipzyme-0.0.9/clipzyme/utils/protein_utils.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/proteins.py` & `clipzyme-0.0.9/clipzyme/utils/proteins.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/pyg.py` & `clipzyme-0.0.9/clipzyme/utils/pyg.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/reactions.py` & `clipzyme-0.0.9/clipzyme/utils/reactions.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/registry.py` & `clipzyme-0.0.9/clipzyme/utils/registry.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/sampler.py` & `clipzyme-0.0.9/clipzyme/utils/sampler.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/screening.py` & `clipzyme-0.0.9/clipzyme/utils/screening.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/smiles.py` & `clipzyme-0.0.9/clipzyme/utils/smiles.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/clipzyme/utils/wln_processing.py` & `clipzyme-0.0.9/clipzyme/utils/wln_processing.py`

 * *Files identical despite different names*

### Comparing `clipzyme-0.0.8/pyproject.toml` & `clipzyme-0.0.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clipzyme"
-version = "0.0.8"
+version = "0.0.9"
 description = "Reaction-Conditioned Virtual Screening of Enzymes"
 authors = ["Peter G Mikhael <pgmikhael@csail.mit.edu>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/pgmikhael/clipzyme"
```

### Comparing `clipzyme-0.0.8/PKG-INFO` & `clipzyme-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clipzyme
-Version: 0.0.8
+Version: 0.0.9
 Summary: Reaction-Conditioned Virtual Screening of Enzymes
 Home-page: https://github.com/pgmikhael/clipzyme
 License: Apache 2.0
 Author: Peter G Mikhael
 Author-email: pgmikhael@csail.mit.edu
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
@@ -58,32 +58,32 @@
 3. Download ESM-2 checkpoint `esm2_t33_650M_UR50D`. The `esm_dir` argument should point to this directory. The following command will download the checkpoint directly:
 ```bash
 wget https://dl.fbaipublicfiles.com/fair-esm/models/esm2_t33_650M_UR50D.pt
 ```
 
 # Checkpoints and Data Files:
 
-The model checkpoint and data are available on Zenodo [here](https://zenodo.org/records/10950376):
+The model checkpoint and data are available on Zenodo [here](https://zenodo.org/records/11187895):
 
-- [clipzyme_data.zip](https://zenodo.org/records/10950376/files/clipzyme_data.zip?download=1):
+- [clipzyme_data.zip](https://zenodo.org/records/11187895/files/clipzyme_data.zip?download=1):
   - The following commands will download the checkpoint directly: 
   ```
-  wget https://zenodo.org/records/10950376/files/clipzyme_data.zip
+  wget https://zenodo.org/records/11187895/files/clipzyme_data.zip
   unzip clipzyme_data.zip -d files
   ```
   - Note that the data files should be extracted into the `files/` directory.
       - `enzymemap.json`: contains the EnzymeMap dataset.
       - `cached_enzymemap.p`: contains the processed EnzymeMap dataset.
       - `clipzyme_screening_set.p`: contains the screening set as dict of UniProt IDs and precomputed protein embeddings.
       - `uniprot2sequence.p`: contains the mapping form sequence ID to amino acids.
 
-- [clipzyme_model.zip](https://zenodo.org/records/10950376/files/clipzyme_model.zip?download=1):
+- [clipzyme_model.zip](https://zenodo.org/records/11187895/files/clipzyme_model.zip?download=1):
   - The following command will download the checkpoint directly: 
   ```
-  wget https://zenodo.org/records/10950376/files/clipzyme_model.zip
+  wget https://zenodo.org/records/11187895/files/clipzyme_model.zip
   unzip clipzyme_model.zip -d files
   ```
     - `clipzyme_model.ckpt`: the trained model checkpoint.
 
 
 
 # Screening with CLIPZyme
@@ -206,15 +206,15 @@
 
 ## Data processing
 
 We obtain the data from the following sources:
 - [EnzymeMap:](`https://doi.org/10.5281/zenodo.7841780`) Heid et al. Enzymemap: Curation, validation and data-driven prediction of enzymatic reactions. 2023.
 - [Terpene Synthases:](`https://zenodo.org/records/10567437`) Samusevich et al. Discovery and characterization of terpene synthases powered by machine learning. 2024. 
 
-Our processed data is can be downloaded from [here](https://zenodo.org/records/10950376). 
+Our processed data is can be downloaded from [here](https://zenodo.org/records/11187895). 
 
 
 ## Training and evaluation
 1. To train the models presented in the tables below, run the following command:
     ```
     python scripts/dispatcher.py -c {config_path} -l {log_path}
     ```
```

