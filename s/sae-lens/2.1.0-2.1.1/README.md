# Comparing `tmp/sae_lens-2.1.0.tar.gz` & `tmp/sae_lens-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-2.1.0.tar", max compression
+gzip compressed data, was "sae_lens-2.1.1.tar", max compression
```

## Comparing `sae_lens-2.1.0.tar` & `sae_lens-2.1.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1069 2024-05-11 12:33:26.177972 sae_lens-2.1.0/LICENSE
--rw-r--r--   0        0        0     3381 2024-05-11 12:33:26.177972 sae_lens-2.1.0/README.md
--rw-r--r--   0        0        0     1917 2024-05-11 12:33:27.521975 sae_lens-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      939 2024-05-11 12:33:27.521975 sae_lens-2.1.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15645 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    17062 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    20134 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     1164 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/pretrained_saes.yaml
--rw-r--r--   0        0        0        0 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/toolkit/__init__.py
--rw-r--r--   0        0        0     2674 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/toolkit/pretrained_sae_loaders.py
--rw-r--r--   0        0        0     6651 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0     1143 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/toolkit/pretrained_saes_directory.py
--rw-r--r--   0        0        0        0 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0      471 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/activation_functions.py
--rw-r--r--   0        0        0    20594 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     6065 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0    15345 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     6785 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     4377 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     1280 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/load_model.py
--rw-r--r--   0        0        0     5065 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     8403 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2424 2024-05-11 12:33:26.189972 sae_lens-2.1.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    20000 2024-05-11 12:33:26.193972 sae_lens-2.1.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     1932 2024-05-11 12:33:26.193972 sae_lens-2.1.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    18456 2024-05-11 12:33:26.193972 sae_lens-2.1.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    30701 2024-05-11 12:33:26.193972 sae_lens-2.1.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     5002 2024-05-11 12:33:26.193972 sae_lens-2.1.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0      423 2024-05-11 12:33:26.193972 sae_lens-2.1.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 sae_lens-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-13 05:14:13.133482 sae_lens-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3381 2024-05-13 05:14:13.133482 sae_lens-2.1.1/README.md
+-rw-r--r--   0        0        0     2041 2024-05-13 05:14:14.605508 sae_lens-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      939 2024-05-13 05:14:14.605508 sae_lens-2.1.1/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15645 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0    17062 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    20134 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     1164 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/pretrained_saes.yaml
+-rw-r--r--   0        0        0        0 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/toolkit/__init__.py
+-rw-r--r--   0        0        0     2674 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/toolkit/pretrained_sae_loaders.py
+-rw-r--r--   0        0        0     6844 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0     1143 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/toolkit/pretrained_saes_directory.py
+-rw-r--r--   0        0        0        0 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0      471 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/activation_functions.py
+-rw-r--r--   0        0        0    20594 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     6065 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0    15345 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/config.py
+-rw-r--r--   0        0        0     6711 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     4377 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     1280 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/load_model.py
+-rw-r--r--   0        0        0     5065 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     8403 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2424 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    20000 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     1932 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    18456 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    30701 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     5002 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0      423 2024-05-13 05:14:13.145482 sae_lens-2.1.1/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     5024 1970-01-01 00:00:00.000000 sae_lens-2.1.1/PKG-INFO
```

### Comparing `sae_lens-2.1.0/LICENSE` & `sae_lens-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/README.md` & `sae_lens-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/pyproject.toml` & `sae_lens-2.1.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "2.1.0"
+version = "2.1.1"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 include = ["pretrained_saes.yaml"]
 
 [tool.poetry.dependencies]
@@ -43,14 +43,17 @@
 pytest = "^8.0.2"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.2"
 flake8 = "7.0.0"
 isort = "5.13.2"
 pyright = "^1.1.351"
 mamba-lens = "^0.0.4"
+ansible-lint = { version = "^24.2.3", markers = "platform_system != 'Windows'" }
+botocore = "^1.34.101"
+boto3 = "^1.34.101"
 
 [tool.poetry.extras]
 mamba = ["mamba-lens"]
 
 
 [tool.isort]
 profile = "black"
```

### Comparing `sae_lens-2.1.0/sae_lens/__init__.py` & `sae_lens-2.1.1/sae_lens/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import CacheActivationsRunner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-2.1.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-2.1.1/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-2.1.1/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-2.1.1/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-2.1.1/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/analysis/tsea.py` & `sae_lens-2.1.1/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/pretrained_saes.yaml` & `sae_lens-2.1.1/sae_lens/pretrained_saes.yaml`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/toolkit/pretrained_sae_loaders.py` & `sae_lens-2.1.1/sae_lens/toolkit/pretrained_sae_loaders.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-2.1.1/sae_lens/toolkit/pretrained_saes.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,26 +169,34 @@
 
     REPO_ID = "ckkissane/attn-saes-gpt2-small-all-layers"
 
     # list all files in repo
     saes_weights = {}
     sae_configs = {}
     repo_files = list_repo_tree(REPO_ID)
+
+    device = "cpu"
+    if torch.cuda.is_available():
+        device = "cuda"
+    elif torch.backends.mps.is_available():
+        device = "mps"
+
     for i in tqdm(repo_files):
         file_name = i.path
         if file_name.endswith(".pt"):
             # print(f"Downloading {file_name}")
             path = hf_hub_download(REPO_ID, file_name)
             name = path.split("/")[-1].split(".pt")[0]
-            saes_weights[name] = torch.load(path, map_location="mps")
+            saes_weights[name] = torch.load(path, map_location=device)
         elif file_name.endswith(".json"):
             # print(f"Downloading {file_name}")
             config_path = hf_hub_download(REPO_ID, file_name)
             name = config_path.split("/")[-1].split("_cfg.json")[0]
             sae_configs[name] = json.load(open(config_path, "r"))
+            sae_configs[name].device = device
 
     saes = {}
     for name, config in sae_configs.items():
         print(f"Loading {name}")
         saes[name] = convert_connor_rob_sae_to_our_saelens_format(
             saes_weights[name], config
         )
```

### Comparing `sae_lens-2.1.0/sae_lens/toolkit/pretrained_saes_directory.py` & `sae_lens-2.1.1/sae_lens/toolkit/pretrained_saes_directory.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/activations_store.py` & `sae_lens-2.1.1/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-2.1.1/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/config.py` & `sae_lens-2.1.1/sae_lens/training/config.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/evals.py` & `sae_lens-2.1.1/sae_lens/training/evals.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,17 +58,14 @@
         original_act = cache[hook_point].flatten(-2, -1)
     else:
         original_act = cache[hook_point]
 
     sae_out, _, _, _, _, _ = sparse_autoencoder(original_act)
     del cache
 
-    if "cuda" in str(model.cfg.device):
-        torch.cuda.empty_cache()
-
     l2_norm_in = torch.norm(original_act, dim=-1)
     l2_norm_out = torch.norm(sae_out, dim=-1)
     l2_norm_in_for_div = l2_norm_in.clone()
     l2_norm_in_for_div[torch.abs(l2_norm_in_for_div) < 0.0001] = 1
     l2_norm_ratio = l2_norm_out / l2_norm_in_for_div
 
     W_dec_norm_dist = sparse_autoencoder.W_dec.norm(dim=1).detach().cpu().numpy()
```

### Comparing `sae_lens-2.1.0/sae_lens/training/geometric_median.py` & `sae_lens-2.1.1/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/lm_runner.py` & `sae_lens-2.1.1/sae_lens/training/lm_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/load_model.py` & `sae_lens-2.1.1/sae_lens/training/load_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/optim.py` & `sae_lens-2.1.1/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/sae_group.py` & `sae_lens-2.1.1/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/session_loader.py` & `sae_lens-2.1.1/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-2.1.1/sae_lens/training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/toy_model_runner.py` & `sae_lens-2.1.1/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/toy_models.py` & `sae_lens-2.1.1/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-2.1.1/sae_lens/training/train_sae_on_language_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-2.1.1/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-2.1.0/PKG-INFO` & `sae_lens-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 2.1.0
+Version: 2.1.1
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

