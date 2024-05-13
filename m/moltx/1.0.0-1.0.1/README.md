# Comparing `tmp/moltx-1.0.0.tar.gz` & `tmp/moltx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moltx-1.0.0.tar", last modified: Tue May  7 15:06:08 2024, max compression
+gzip compressed data, was "moltx-1.0.1.tar", last modified: Mon May 13 09:12:47 2024, max compression
```

## Comparing `moltx-1.0.0.tar` & `moltx-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:06:08.320443 moltx-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 15:05:59.000000 moltx-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-07 15:06:08.320443 moltx-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-07 15:05:59.000000 moltx-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:06:08.320443 moltx-1.0.0/moltx/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:06:08.320443 moltx-1.0.0/moltx/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/data/spe_safe.txt
--rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/data/spe_smiles.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/data/tks_safe.json
--rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/data/tks_smiles.json
--rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/nets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-07 15:05:59.000000 moltx-1.0.0/moltx/tokenizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:06:08.320443 moltx-1.0.0/moltx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-07 15:06:08.000000 moltx-1.0.0/moltx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-07 15:06:08.000000 moltx-1.0.0/moltx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 15:06:08.000000 moltx-1.0.0/moltx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 15:06:08.000000 moltx-1.0.0/moltx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 15:06:08.000000 moltx-1.0.0/moltx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 15:05:59.000000 moltx-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-07 15:06:08.324442 moltx-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 15:05:59.000000 moltx-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 15:06:08.320443 moltx-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-07 15:05:59.000000 moltx-1.0.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-07 15:05:59.000000 moltx-1.0.0/tests/test_nets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-07 15:05:59.000000 moltx-1.0.0/tests/test_pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-07 15:05:59.000000 moltx-1.0.0/tests/test_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:12:47.942317 moltx-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 09:12:41.000000 moltx-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-13 09:12:47.942317 moltx-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-13 09:12:41.000000 moltx-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:12:47.938317 moltx-1.0.1/moltx/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:12:47.942317 moltx-1.0.1/moltx/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11088 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/data/spe_safe.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    27879 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/data/spe_smiles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/data/tks_safe.json
+-rw-r--r--   0 runner    (1001) docker     (127)    36304 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/data/tks_smiles.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5984 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6643 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4530 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10328 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8411 2024-05-13 09:12:41.000000 moltx-1.0.1/moltx/tokenizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:12:47.942317 moltx-1.0.1/moltx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-05-13 09:12:47.000000 moltx-1.0.1/moltx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-13 09:12:47.000000 moltx-1.0.1/moltx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:12:47.000000 moltx-1.0.1/moltx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 09:12:47.000000 moltx-1.0.1/moltx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 09:12:47.000000 moltx-1.0.1/moltx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 09:12:41.000000 moltx-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-13 09:12:47.942317 moltx-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:12:41.000000 moltx-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:12:47.942317 moltx-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-05-13 09:12:41.000000 moltx-1.0.1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-13 09:12:41.000000 moltx-1.0.1/tests/test_nets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-13 09:12:41.000000 moltx-1.0.1/tests/test_pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-13 09:12:41.000000 moltx-1.0.1/tests/test_tokenizer.py
```

### Comparing `moltx-1.0.0/LICENSE` & `moltx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/PKG-INFO` & `moltx-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
```

### Comparing `moltx-1.0.0/README.md` & `moltx-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/moltx/data/spe_safe.txt` & `moltx-1.0.1/moltx/data/spe_safe.txt`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/moltx/data/spe_smiles.txt` & `moltx-1.0.1/moltx/data/spe_smiles.txt`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/moltx/data/tks_safe.json` & `moltx-1.0.1/moltx/data/tks_safe.json`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/moltx/data/tks_smiles.json` & `moltx-1.0.1/moltx/data/tks_smiles.json`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/moltx/datasets.py` & `moltx-1.0.1/moltx/datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/moltx/models.py` & `moltx-1.0.1/moltx/models.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/moltx/nets.py` & `moltx-1.0.1/moltx/nets.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/moltx/pipelines.py` & `moltx-1.0.1/moltx/pipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,25 +85,25 @@
             meet_end = (next_tokens.squeeze(1).eq(eos).nonzero()).squeeze(1)
             if meet_end.numel() > 0:
                 beam_width -= meet_end.size(0)
                 probs.extend(log_probs.index_select(0, meet_end).squeeze(1).exp().tolist())
                 end_tgt = tgt.index_select(0, tgt_idx.index_select(0, meet_end).squeeze(1))
                 smiles.extend(map(self.tokenizer.decode, end_tgt[:, prefixlen:].tolist()))
                 if beam_width == 0:
-                    return smiles, probs
+                    return sorted(zip(smiles, probs), key=lambda x: x[1], reverse=True)
             not_end = (next_tokens.squeeze(1).ne(eos).nonzero()).squeeze(1)
             log_probs = log_probs.index_select(0, not_end)
             next_tokens = next_tokens.index_select(0, not_end)
             tgt = tgt.index_select(0, tgt_idx.index_select(0, not_end).squeeze(1))
             tgt = torch.concat((tgt, next_tokens), dim=-1)
             if 'src' in kwds:
                 kwds['src'] = kwds['src'].index_select(0, tgt_idx.index_select(0, not_end).squeeze(1))
         probs.extend(log_probs.squeeze(1).exp().tolist())
         smiles.extend(map(self.tokenizer.decode, tgt[:, prefixlen:].tolist()))
-        return smiles, probs
+        return sorted(zip(smiles, probs), key=lambda x: x[1], reverse=True)
 
 
 class AdaMR(Base):
 
     def _model_args(self, smiles: str) -> typing.Tuple[torch.Tensor]:
         src = self._tokenize(smiles)
         tgt = self._tokenize(self.tokenizer.BOS)
@@ -122,16 +122,16 @@
             'probability': prob
         }
 
     def _do_generate(self, src: torch.Tensor, tgt: torch.Tensor) -> typing.Mapping:
         return self._random_sample(src=src, tgt=tgt)
 
     def _do_canonicalize(self, src: torch.Tensor, tgt: torch.Tensor) -> typing.Mapping:
-        smiles, probs = self._beam_search(src=src, tgt=tgt, beam_width=3)
-        return smiles[0], probs[0]
+        out = self._beam_search(src=src, tgt=tgt, beam_width=3)
+        return out[0]
 
 
 class AdaMRClassifier(AdaMR):
     def _model_args(self, smiles: str) -> typing.Tuple[torch.Tensor]:
         src = self._tokenize(smiles)
         tgt = self._tokenize(f"{self.tokenizer.BOS}{smiles}{self.tokenizer.EOS}")
         return src, tgt
@@ -213,16 +213,16 @@
             'probability': prob
         }
 
     def _do_generate(self, tgt: torch.Tensor) -> typing.Mapping:
         return self._random_sample(tgt=tgt)
 
     def _do_canonicalize(self, tgt: torch.Tensor) -> typing.Mapping:
-        smiles, probs = self._beam_search(tgt=tgt)
-        return smiles[0], probs[0]
+        out = self._beam_search(tgt=tgt)
+        return out[0]
 
 
 class AdaMR2Classifier(AdaMR):
 
     def __call__(self, smiles: str) -> typing.Mapping:
         tgt = self._tokenize(f"{self.tokenizer.BOS}{smiles}{self.tokenizer.EOS}")
         out = self.model(tgt)
```

### Comparing `moltx-1.0.0/moltx/tokenizers.py` & `moltx-1.0.1/moltx/tokenizers.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/moltx.egg-info/PKG-INFO` & `moltx-1.0.1/moltx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moltx
-Version: 1.0.0
+Version: 1.0.1
 Summary: Molcule Transformer X Model
 Author: Michael Ding
 Author-email: yandy.ding@gmail.com
 Keywords: molcule,AI,deep learning,transformer
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: POSIX
```

### Comparing `moltx-1.0.0/moltx.egg-info/SOURCES.txt` & `moltx-1.0.1/moltx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/setup.cfg` & `moltx-1.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/tests/test_datasets.py` & `moltx-1.0.1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/tests/test_nets.py` & `moltx-1.0.1/tests/test_nets.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/tests/test_pipelines.py` & `moltx-1.0.1/tests/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `moltx-1.0.0/tests/test_tokenizer.py` & `moltx-1.0.1/tests/test_tokenizer.py`

 * *Files identical despite different names*

