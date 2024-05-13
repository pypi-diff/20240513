# Comparing `tmp/tangermeme-0.2.0.tar.gz` & `tmp/tangermeme-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tangermeme-0.2.0.tar", last modified: Tue May  7 17:20:42 2024, max compression
+gzip compressed data, was "tangermeme-0.2.1.tar", last modified: Mon May 13 19:55:33 2024, max compression
```

## Comparing `tangermeme-0.2.0.tar` & `tangermeme-0.2.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-07 17:20:42.643109 tangermeme-0.2.0/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1072 2024-02-04 20:42:51.000000 tangermeme-0.2.0/LICENSE
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      591 2024-05-07 17:20:42.638109 tangermeme-0.2.0/PKG-INFO
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    16195 2024-05-07 17:13:13.000000 tangermeme-0.2.0/README.md
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)       38 2024-05-07 17:20:42.644109 tangermeme-0.2.0/setup.cfg
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      695 2024-05-07 17:13:13.000000 tangermeme-0.2.0/setup.py
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-07 17:20:42.446108 tangermeme-0.2.0/tangermeme/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      111 2024-05-07 17:13:13.000000 tangermeme-0.2.0/tangermeme/__init__.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5832 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/ablate.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    27068 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/deep_lift_shap.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6424 2024-04-19 03:17:23.000000 tangermeme-0.2.0/tangermeme/design.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22259 2024-04-12 17:47:04.000000 tangermeme-0.2.0/tangermeme/ersatz.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    14430 2024-03-28 04:48:35.000000 tangermeme-0.2.0/tangermeme/io.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6729 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/ism.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6550 2024-02-18 21:52:53.000000 tangermeme-0.2.0/tangermeme/kmers.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     4598 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/marginalize.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12384 2024-02-16 06:07:44.000000 tangermeme-0.2.0/tangermeme/match.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5027 2024-05-03 22:57:28.000000 tangermeme-0.2.0/tangermeme/plot.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3409 2024-04-01 23:34:04.000000 tangermeme-0.2.0/tangermeme/predict.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     4424 2024-04-01 23:49:41.000000 tangermeme-0.2.0/tangermeme/product.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    11906 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/seqlet.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3641 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/space.py
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-07 17:20:42.495108 tangermeme-0.2.0/tangermeme/tools/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)        0 2024-02-12 20:33:38.000000 tangermeme-0.2.0/tangermeme/tools/__init__.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13248 2024-02-19 18:37:49.000000 tangermeme-0.2.0/tangermeme/tools/fimo.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     2445 2024-02-25 18:18:37.000000 tangermeme-0.2.0/tangermeme/tools/tomtom.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9118 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tangermeme/utils.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    14343 2024-05-07 03:58:32.000000 tangermeme-0.2.0/tangermeme/variant_effect.py
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-07 17:20:42.633109 tangermeme-0.2.0/tangermeme.egg-info/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      591 2024-05-07 17:20:42.000000 tangermeme-0.2.0/tangermeme.egg-info/PKG-INFO
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      951 2024-05-07 17:20:42.000000 tangermeme-0.2.0/tangermeme.egg-info/SOURCES.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)        1 2024-05-07 17:20:42.000000 tangermeme-0.2.0/tangermeme.egg-info/dependency_links.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)      159 2024-05-07 17:20:42.000000 tangermeme-0.2.0/tangermeme.egg-info/requires.txt
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)       28 2024-05-07 17:20:42.000000 tangermeme-0.2.0/tangermeme.egg-info/top_level.txt
-drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-07 17:20:42.629109 tangermeme-0.2.0/tests/
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    28374 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_ablate.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    36846 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_deep_lift_shap.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    25611 2024-03-28 04:48:35.000000 tangermeme-0.2.0/tests/test_ersatz.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22795 2024-03-28 04:48:35.000000 tangermeme-0.2.0/tests/test_io.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12445 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_ism.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1536 2024-02-19 00:37:13.000000 tangermeme-0.2.0/tests/test_kmers.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    21450 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_marginalize.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13448 2024-02-16 07:04:10.000000 tangermeme-0.2.0/tests/test_match.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6967 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_predict.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    23116 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_product.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     8491 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_seqlet.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22448 2024-05-02 23:03:30.000000 tangermeme-0.2.0/tests/test_space.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6841 2024-02-16 07:04:33.000000 tangermeme-0.2.0/tests/test_utils.py
--rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3541 2024-05-07 04:03:24.000000 tangermeme-0.2.0/tests/test_variant_effect.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-13 19:55:33.627085 tangermeme-0.2.1/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1072 2024-02-04 20:42:51.000000 tangermeme-0.2.1/LICENSE
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      591 2024-05-13 19:55:33.625085 tangermeme-0.2.1/PKG-INFO
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    16195 2024-05-07 17:13:13.000000 tangermeme-0.2.1/README.md
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)       38 2024-05-13 19:55:33.627085 tangermeme-0.2.1/setup.cfg
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      695 2024-05-13 19:54:37.000000 tangermeme-0.2.1/setup.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-13 19:55:33.454084 tangermeme-0.2.1/tangermeme/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      111 2024-05-13 19:54:47.000000 tangermeme-0.2.1/tangermeme/__init__.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5832 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tangermeme/ablate.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    23027 2024-05-13 19:36:11.000000 tangermeme-0.2.1/tangermeme/deep_lift_shap.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6424 2024-04-19 03:17:23.000000 tangermeme-0.2.1/tangermeme/design.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22259 2024-04-12 17:47:04.000000 tangermeme-0.2.1/tangermeme/ersatz.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    14425 2024-05-09 17:55:42.000000 tangermeme-0.2.1/tangermeme/io.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6729 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tangermeme/ism.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6550 2024-02-18 21:52:53.000000 tangermeme-0.2.1/tangermeme/kmers.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     4598 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tangermeme/marginalize.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12384 2024-02-16 06:07:44.000000 tangermeme-0.2.1/tangermeme/match.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     5027 2024-05-03 22:57:28.000000 tangermeme-0.2.1/tangermeme/plot.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3409 2024-04-01 23:34:04.000000 tangermeme-0.2.1/tangermeme/predict.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     4424 2024-04-01 23:49:41.000000 tangermeme-0.2.1/tangermeme/product.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    11906 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tangermeme/seqlet.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3641 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tangermeme/space.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-13 19:55:33.485084 tangermeme-0.2.1/tangermeme/tools/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)        0 2024-02-12 20:33:38.000000 tangermeme-0.2.1/tangermeme/tools/__init__.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13248 2024-02-19 18:37:49.000000 tangermeme-0.2.1/tangermeme/tools/fimo.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     2445 2024-02-25 18:18:37.000000 tangermeme-0.2.1/tangermeme/tools/tomtom.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     9118 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tangermeme/utils.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    14343 2024-05-07 03:58:32.000000 tangermeme-0.2.1/tangermeme/variant_effect.py
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-13 19:55:33.623085 tangermeme-0.2.1/tangermeme.egg-info/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      591 2024-05-13 19:55:33.000000 tangermeme-0.2.1/tangermeme.egg-info/PKG-INFO
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      951 2024-05-13 19:55:33.000000 tangermeme-0.2.1/tangermeme.egg-info/SOURCES.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)        1 2024-05-13 19:55:33.000000 tangermeme-0.2.1/tangermeme.egg-info/dependency_links.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)      159 2024-05-13 19:55:33.000000 tangermeme-0.2.1/tangermeme.egg-info/requires.txt
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)       28 2024-05-13 19:55:33.000000 tangermeme-0.2.1/tangermeme.egg-info/top_level.txt
+drwxr-xr-x   0 jmschr    (1222) kundaje  (65541)        0 2024-05-13 19:55:33.621085 tangermeme-0.2.1/tests/
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    28374 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tests/test_ablate.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    36842 2024-05-13 19:45:34.000000 tangermeme-0.2.1/tests/test_deep_lift_shap.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    25611 2024-03-28 04:48:35.000000 tangermeme-0.2.1/tests/test_ersatz.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22795 2024-03-28 04:48:35.000000 tangermeme-0.2.1/tests/test_io.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    12445 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tests/test_ism.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     1536 2024-02-19 00:37:13.000000 tangermeme-0.2.1/tests/test_kmers.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    21450 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tests/test_marginalize.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    13448 2024-02-16 07:04:10.000000 tangermeme-0.2.1/tests/test_match.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6967 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tests/test_predict.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    23116 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tests/test_product.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     8491 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tests/test_seqlet.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)    22448 2024-05-02 23:03:30.000000 tangermeme-0.2.1/tests/test_space.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     6841 2024-02-16 07:04:33.000000 tangermeme-0.2.1/tests/test_utils.py
+-rw-r--r--   0 jmschr    (1222) kundaje  (65541)     3541 2024-05-07 04:03:24.000000 tangermeme-0.2.1/tests/test_variant_effect.py
```

### Comparing `tangermeme-0.2.0/LICENSE` & `tangermeme-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/PKG-INFO` & `tangermeme-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangermeme
-Version: 0.2.0
+Version: 0.2.1
 Summary: Biological sequence analysis for the modern age.
 Home-page: https://github.com/jmschrei/tangermeme
 Author: Jacob Schreiber
 Author-email: jmschreiber91@gmail.com
 License: LICENSE.txt
 License-File: LICENSE
 Requires-Dist: numpy>=1.14.2
```

### Comparing `tangermeme-0.2.0/README.md` & `tangermeme-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/setup.py` & `tangermeme-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='tangermeme',
-    version='0.2.0',
+    version='0.2.1',
     author='Jacob Schreiber',
     author_email='jmschreiber91@gmail.com',
     packages=['tangermeme', 'tangermeme/tools'],
     scripts=[],
     url='https://github.com/jmschrei/tangermeme',
     license='LICENSE.txt',
     description='Biological sequence analysis for the modern age.',
```

### Comparing `tangermeme-0.2.0/tangermeme/ablate.py` & `tangermeme-0.2.1/tangermeme/ablate.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/deep_lift_shap.py` & `tangermeme-0.2.1/tangermeme/deep_lift_shap.py`

 * *Files 14% similar despite different names*

```diff
@@ -75,244 +75,92 @@
 		hypothetical_contribs = hypothetical_diffs * multipliers[0]
 
 		projected_contribs[:, i] = torch.sum(hypothetical_contribs, dim=1)
 
 	return (projected_contribs,)
 
 
-class DeepLiftShap():
-	"""A vectorized version of the DeepLIFT/SHAP algorithm from Captum.
+def _register_hooks(module): 
+	if len(module._backward_hooks) > 0:
+		return
+	if not isinstance(module, tuple(module._NON_LINEAR_OPS.keys())):
+		return
 
-	DeepLIFT/SHAP is an approach for assigning importance to each input
-	feature in an example using principles from game theory. At a high level,
-	Shapley values are the average marginal contribution of each feature to
-	the prediction and DeepLIFT/SHAP approximates this value for neural
-	networks.
-
-	This algorithm is implemented as a class because it is based on the Captum 
-	approach of assigning hooks to layers in a PyTorch module object, where the
-	hooks modify the gradients to implement the rescale rule. This object 
-	implementation is much simpler than the one in Captum and adds in two 
-	features: first, the implementation is vectorized so one can accept multiple 
-	references for each example and these references can be different across 
-	examples and, second, it adds in automatic checks that the theoretical 
-	properties of the algorithm hold. 
-
-	IMPORTANT: This implementation is minimal and only supports linear
-	operations, convolutions, and dense layers. It does not support any form of
-	non-linear pooling operation and may not work on custom operations. I do 
-	not know whether it works with transformers. A warning will be raised if 
-	the layers are not supported or yield attributions that do not satisfy the
-	theoretical properties. Use the _captum_deep_lift_shap function when unsure.
+	module.handles = []
+	module.handles.append(module.register_forward_hook(_f_hook))
+	module.handles.append(module.register_forward_pre_hook(_fp_hook))
+	module.handles.append(module.register_full_backward_hook(_b_hook))
 
 
-	Parameters
-	----------
-	model: torch.nn.Module
-		A PyTorch model to use for making predictions. These models can take in
-		any number of inputs and make any number of outputs. The additional
-		inputs must be specified in the `args` parameter.
+def _clear_hooks(module):
+	if hasattr(module, "handles") and len(module.handles) > 0:
+		for handle in module.handles:
+			handle.remove()
 
-	additional_nonlinear_ops: dict or None, optional
-		If additional nonlinear ops need to be added to the dictionary of
-		operations that can be handled by DeepLIFT/SHAP, pass a dictionary here
-		where the keys are class types and the values are the name of the
-		function that handle that sort of class. Make sure that the signature
-		matches those of `_nonlinear` and `_maxpool` above. This can also be
-		used to overwrite the hard-coded operations by passing in a dictionary
-		with overlapping key names. If None, do not add any additional 
-		operations. Default is None.
+		del module.handles
 
-	ignore_layers: tuple
-		A tuple of layer objects that should be ignored when assigning hooks.
-		This should be the activations used in the model. Default is
-		(torch.nn.ReLU,).
-
-	eps: float, optional
-		An epsilon with which to threshold gradients to ensure that there
-		isn't an explosion. Default is 1e-6.
 
-	warning_threshold: float, optional
-		A threshold on the convergence delta that will always raise a warning
-		if the delta is larger than it. Normal deltas are in the range of
-		1e-6 to 1e-8. Note that convergence deltas are calculated on the
-		gradients prior to the attribution_func being applied to them. Default 
-		is 0.001. 
+def _fp_hook(module, inputs): 
+	module.input = inputs[0].clone().detach()
 
-	verbose: bool, optional
-		Whether to print the convergence delta for each example that is
-		explained, regardless of whether it surpasses the warning threshold.
-		Default is False.
-	"""
-
-	def __init__(self, model, additional_nonlinear_ops=None, eps=1e-10, 
-		warning_threshold=0.0001, verbose=False):
-		self.model = model
-		self.eps = eps
-		self.warning_threshold = warning_threshold
-		self.verbose = verbose
-
-		self.handles = []
-
-		self._NON_LINEAR_OPS = {
-			torch.nn.ReLU: _nonlinear,
-			torch.nn.ELU: _nonlinear,
-			torch.nn.LeakyReLU: _nonlinear,
-			torch.nn.Sigmoid: _nonlinear,
-			torch.nn.Tanh: _nonlinear,
-			torch.nn.Softplus: _nonlinear,
-			torch.nn.MaxPool1d: _maxpool,
-			torch.nn.MaxPool2d: _maxpool,
-			torch.nn.Softmax: _softmax
-		}
-
-		if additional_nonlinear_ops is not None:
-			for key, value in additional_nonlinear_ops.items():
-				self._NON_LINEAR_OPS[key] = value
-
-
-	def attribute(self, X, references, args=None, target=0):
-		"""Run the attribution algorithm on a set of inputs and baselines.
-
-		This method actually handles calculating the attribution values and
-		checking to make sure that they follow the theoretical properties of
-		attributions.
-
-
-		Parameters
-		----------
-		X: torch.Tensor, shape=(n, len(alphabet), length)
-			A tensor of examples to calculate attribution values for.
-
-		references: torch.Tensor, shape=(n, n_baselines, len(alphabet), length)
-			A tensor of baselines/references to calculates attributions with
-			respect to. The first dimension corresponds to the sequences that
-			attributions are calculated for, the second dimension corresponds
-			to the number of baselines that are being used for that example,
-			the the last two dimensions should match that of the inputs.
-
-		args: tuple, optional
-			A tuple of additional forward arguments to pass into the model.
-			Even when there is only a single additional argument this must be
-			provided as a tuple.
-
-		target: int, optional
-			The output of the model to calculate gradients/attributions for. 
-			This will index the last dimension of the predictions. Default is 0.
-
-
-		Returns
-		-------
-		attributions: torch.Tensor, shape=(n, len(alphabet), length)
-			Attributions for each example averaged over all of the baselines
-			provided.
-		"""
-
-		assert X.shape == references.shape
-
-		try:
-			# Apply hooks and set up inputs
-			self.model.apply(self._register_hooks)
-			X_ = torch.cat([X, references])
-
-			# Calculate the gradients using the rescale rule
-			with torch.autograd.set_grad_enabled(True):
-				if args is not None:
-					args = (torch.cat([arg, arg]) for arg in args)
-					y = self.model(X_, *args)[:, target]
-				else:
-					y = self.model(X_)[:, target]
-
-				gradients = torch.autograd.grad(y.sum(), X)[0]
-
-			# Check that the prediction-difference-from-reference is equal to
-			# the sum of the attributions
-			output_diff = torch.sub(*torch.chunk(y, 2))
-			input_diff = torch.sum((X - references) * gradients, dim=(1, 2))
-			convergence_deltas = abs(output_diff - input_diff)
-
-			if torch.any(convergence_deltas > self.warning_threshold):
-				warnings.warn("Convergence deltas too high: " +   
-					str(convergence_deltas), RuntimeWarning)
-
-			if self.verbose:
-				print(convergence_deltas)
-
-		finally:
-			for handle in self.handles:
-				handle.remove()
-
-		return gradients
 
-	def _fp_hook(self, module, inputs): 
-		module.input = inputs[0].clone().detach()
+def _f_hook(module, inputs, outputs):
+	module.output = outputs.clone().detach()
 
-	def _f_hook(self, module, inputs, outputs):
-		module.output = outputs.clone().detach()
 
-	def _b_hook(self, module, grad_input, grad_output):
-		return self._NON_LINEAR_OPS[type(module)](module, grad_input, 
-			grad_output, eps=self.eps)
+def _b_hook(module, grad_input, grad_output):
+	return module._NON_LINEAR_OPS[type(module)](module, grad_input, 
+		grad_output)
 
-	def _register_hooks(self, module): 
-		if len(module._backward_hooks) > 0:
-			return
-		if not isinstance(module, tuple(self._NON_LINEAR_OPS.keys())):
-			return
 
-		self.handles.append(module.register_forward_hook(self._f_hook))
-		self.handles.append(module.register_forward_pre_hook(self._fp_hook))
-		self.handles.append(module.register_full_backward_hook(self._b_hook))
-
-
-def _nonlinear(module, grad_input, grad_output, eps):
+def _nonlinear(module, grad_input, grad_output):
 	"""An internal function implementing a general-purpose nonlinear correction.
 
 	This function, copied and slightly modified from Captum, is meant to be
 	the `rescale` rule applied to general non-linear functions such as
 	activations.
 	"""
 
 	delta_in_ = torch.sub(*module.input.chunk(2))
 	delta_out_ = torch.sub(*module.output.chunk(2))
 
 	delta_in = torch.cat([delta_in_, delta_in_])
 	delta_out = torch.cat([delta_out_, delta_out_])
 
 	delta = delta_out / delta_in
-	idxs = torch.abs(delta_in) < eps
+	idxs = torch.abs(delta_in) < 1e-6
 
 	return (torch.where(idxs, grad_input[0], grad_output[0] * delta),)
 
 
-def _softmax(module, grad_input, grad_output, eps):
+def _softmax(module, grad_input, grad_output):
 	"""An internal function implementing a correction for softmax activations.
 
 	This function, copied and slightly modified from Captum, is meant to be
 	the `rescale` rule applied specifically to softmax activations without
 	needing to remove them and operate on the underlying logits.
 	"""
 
 	delta_in_ = torch.sub(*module.input.chunk(2))
 	delta_out_ = torch.sub(*module.output.chunk(2))
 
 	delta_in = torch.cat([delta_in_, delta_in_])
 	delta_out = torch.cat([delta_out_, delta_out_])
 
 	delta = delta_out / delta_in
-	idxs = torch.abs(delta_in) < eps
+	idxs = torch.abs(delta_in) < 1e-6
 
 	grad_input_unnorm = torch.where(idxs, grad_input[0], grad_output[0] * delta)
 
 	n = grad_input[0].numel()
 	new_grad_inp = grad_input_unnorm - grad_input_unnorm.sum() * 1 / n
 	return (new_grad_inp,)
 
 
-def _maxpool(module, grad_input, grad_output, eps):
+def _maxpool(module, grad_input, grad_output):
 	"""An internal function implementing a 1D max-pooling correction.
 
 	This function, copied and slightly modified from Captum, is meant to be
 	the `rescale` rule applied to max pooling layers given their nature of
 	aggregating values across multiple positions.
 	"""
 
@@ -339,23 +187,23 @@
 		unpool_ = unpool_func(grad_output[0] * delta_out, indices, 
 			module.kernel_size, module.stride, module.padding, 
 			list(module.input.shape))
 		unpool_delta, unpool_ref_delta = torch.chunk(unpool_, 2)
 
 	unpool_delta_ = unpool_delta + unpool_ref_delta
 	unpool_delta = torch.cat([unpool_delta_, unpool_delta_])
-	idxs = torch.abs(delta_in) < eps
+	idxs = torch.abs(delta_in) < 1e-7
 
 	new_grad_inp = torch.where(idxs, grad_input[0], unpool_delta / delta_in)
 	return (new_grad_inp,)
 
 
 def deep_lift_shap(model, X, args=None, target=0,  batch_size=32,
 	references=dinucleotide_shuffle, n_shuffles=20, return_references=False, 
-	hypothetical=False, warning_threshold=0.0001, additional_nonlinear_ops=None,
+	hypothetical=False, warning_threshold=0.001, additional_nonlinear_ops=None,
 	print_convergence_deltas=False, raw_outputs=False, device='cuda', 
 	random_state=None, verbose=False):
 	"""Calculate attributions for a set of sequences using DeepLIFT/SHAP.
 
 	This function will calculate the DeepLIFT/SHAP attributions on a set of
 	sequences given a model. These attributions have the additive property that
 	the sum of the attributions is ~equal to the difference in prediction
@@ -488,23 +336,55 @@
 
 	references: torch.tensor, optional
 		The references used for each input sequence, with the shape
 		(n_input_sequences, n_shuffles, 4, length). Only returned if
 		`return_references = True`. 
 	"""
 
-	attributions, references_ = [], []
+	_NON_LINEAR_OPS = {
+		torch.nn.ReLU: _nonlinear,
+		torch.nn.ReLU6: _nonlinear,
+		torch.nn.RReLU: _nonlinear,
+		torch.nn.SELU: _nonlinear,
+		torch.nn.CELU: _nonlinear,
+		torch.nn.GELU: _nonlinear,
+		torch.nn.SiLU: _nonlinear,
+		torch.nn.Mish: _nonlinear,
+		torch.nn.GLU: _nonlinear,
+		torch.nn.ELU: _nonlinear,
+		torch.nn.LeakyReLU: _nonlinear,
+		torch.nn.Sigmoid: _nonlinear,
+		torch.nn.Tanh: _nonlinear,
+		torch.nn.Softplus: _nonlinear,
+		torch.nn.Softshrink: _nonlinear,
+		torch.nn.LogSigmoid: _nonlinear,
+		torch.nn.PReLU: _nonlinear,
+		torch.nn.MaxPool1d: _maxpool,
+		torch.nn.MaxPool2d: _maxpool,
+		torch.nn.Softmax: _softmax
+	}
+
+	if additional_nonlinear_ops is not None:
+		for key, value in additional_nonlinear_ops.items():
+			_NON_LINEAR_OPS[key] = value
+
 	model = model.to(device).eval()
+	for module in model.modules():
+		module._NON_LINEAR_OPS = _NON_LINEAR_OPS
 
+	attributions, references_, Xi, rj, attr_ = [], [], [], [], []
 	if isinstance(references, torch.Tensor):
 		n_shuffles = references.shape[1]
+	n, z = X.shape[0] * n_shuffles, 0
 
-	n = X.shape[0] * n_shuffles
-	Xi, rj, attr_ = [], [], []
-	z = 0
+	try:
+		model.apply(_register_hooks)
+	except Exception as e:
+		model.apply(_clear_hooks)
+		raise(e)
 
 	for i in trange(n, disable=not verbose):
 		Xi.append(i // n_shuffles)
 		rj.append(i % n_shuffles)
 
 		if len(Xi) == batch_size or i == (n-1):
 			_X = X[Xi].cpu()
@@ -520,24 +400,53 @@
 				if random_state is None:
 					_references = references(_X, n=1)[:, 0]
 				else:
 					_references = torch.cat([references(_X[j:j+1], n=1, 
 						random_state=random_state+rj[j])[:, 0] 
 							for j in range(len(_X))])
 
-			_X = _X.to(device).float().requires_grad_()
-			_references = _references.to(device).float().requires_grad_()
+			_X = _X.to(device).requires_grad_()
+			_references = _references.to(device).requires_grad_()
+
+			# This next block is actually running DeepLIFT by concatenating the
+			# batch of examples and the batch of references and running the
+			# forward and backward passes that have been modified by the above
+			# hooks. In a try-except block to make sure we remove hooks if an
+			# error is raised. 
+			try:
+				X_ = torch.cat([_X, _references])
+
+				# Calculate the gradients using the rescale rule
+				with torch.autograd.set_grad_enabled(True):
+					if _args is not None:
+						_args = (torch.cat([arg, arg]) for arg in _args)
+						y = model(X_, *_args)[:, target]
+					else:
+						y = model(X_)[:, target]
+
+					multipliers = torch.autograd.grad(y.sum(), _X)[0]
+
+				# Check that the prediction-difference-from-reference is equal to
+				# the sum of the attributions
+				output_diff = torch.sub(*torch.chunk(y, 2))
+				input_diff = torch.sum((_X - _references) * multipliers, 
+					dim=(1, 2))
+				convergence_deltas = abs(output_diff - input_diff)
+
+				if torch.any(convergence_deltas > warning_threshold):
+					warnings.warn("Convergence deltas too high: " +   
+						str(convergence_deltas), RuntimeWarning)
+
+				if print_convergence_deltas:
+					print(convergence_deltas)
+
+			except Exception as e:
+				model.apply(_clear_hooks)
+				raise(e)
 
-			# Run DeepLiftShap
-			multipliers = DeepLiftShap(model, 
-				warning_threshold=warning_threshold, 
-				additional_nonlinear_ops=additional_nonlinear_ops, 
-				verbose=print_convergence_deltas).attribute(_X, _references, 
-				args=_args, target=target)
-			
 			# If not returning the raw multipliers then apply the correction for
 			# character encodings
 			if raw_outputs == False:
 				multipliers = hypothetical_attributions((multipliers,), (_X,), 
 					(_references,))[0]
 
 			# attr_ is a list where each element is a tensor for the multipliers
@@ -562,21 +471,25 @@
 				z += 1
 
 			if return_references:
 				references_.extend(list(_references.cpu().detach()))
 
 			Xi, rj = [], []
 
+
+	model.apply(_clear_hooks)
+	for module in model.modules():
+		del(module._NON_LINEAR_OPS)
+
 	attributions = torch.stack(attributions)
-	
+
 	if return_references:
 		references_ = torch.cat(references_).reshape(X.shape[0], n_shuffles, 
 			*X.shape[1:])
 		return attributions, references_
-	
 	return attributions
 
 
 def _captum_deep_lift_shap(model, X, args=None, target=0, batch_size=32,
 	references=dinucleotide_shuffle, n_shuffles=20,  return_references=False, 
 	hypothetical=False, device='cuda', random_state=None, verbose=False):
 	"""Calculate attributions using DeepLift/Shap and a given model. 
@@ -703,8 +616,8 @@
 
 			attributions.append(attr.cpu())
 
 	attributions = torch.cat(attributions)
 
 	if return_references:
 		return attributions, torch.cat(references_)
-	return attributions
+	return attributions
```

### Comparing `tangermeme-0.2.0/tangermeme/design.py` & `tangermeme-0.2.1/tangermeme/design.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/ersatz.py` & `tangermeme-0.2.1/tangermeme/ersatz.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/io.py` & `tangermeme-0.2.1/tangermeme/io.py`

 * *Files 3% similar despite different names*

```diff
@@ -360,24 +360,23 @@
 
 		seqs.append(seq)
 
 	if not isinstance(sequences, dict):
 		sequences.close()
 
 	seqs = torch.from_numpy(numpy.stack(seqs))
+	y_return = [seqs]
+
 	if signals is not None:
-		signals_ = torch.from_numpy(numpy.stack(signals_))
-		
-		if in_signals is not None:
-			in_signals_ = torch.from_numpy(numpy.stack(in_signals_))
-			return seqs, signals_, in_signals_
-
-		return seqs, signals_
-	else:
-		return seqs			
+		y_return.append(torch.from_numpy(numpy.stack(signals_)))
+
+	if in_signals is not None:
+		y_return.append(torch.from_numpy(numpy.stack(in_signals_)))
+
+	return y_return[0] if len(y_return) == 1 else y_return
 
 
 def read_meme(filename, n_motifs=None):
 	"""Read a MEME file and return a dictionary of PWMs.
 
 	This method takes in the filename of a MEME-formatted file to read in
 	and returns a dictionary of the PWMs where the keys are the metadata
```

### Comparing `tangermeme-0.2.0/tangermeme/ism.py` & `tangermeme-0.2.1/tangermeme/ism.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/kmers.py` & `tangermeme-0.2.1/tangermeme/kmers.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/marginalize.py` & `tangermeme-0.2.1/tangermeme/marginalize.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/match.py` & `tangermeme-0.2.1/tangermeme/match.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/plot.py` & `tangermeme-0.2.1/tangermeme/plot.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/predict.py` & `tangermeme-0.2.1/tangermeme/predict.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/product.py` & `tangermeme-0.2.1/tangermeme/product.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/seqlet.py` & `tangermeme-0.2.1/tangermeme/seqlet.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/space.py` & `tangermeme-0.2.1/tangermeme/space.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/tools/fimo.py` & `tangermeme-0.2.1/tangermeme/tools/fimo.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/tools/tomtom.py` & `tangermeme-0.2.1/tangermeme/tools/tomtom.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/utils.py` & `tangermeme-0.2.1/tangermeme/utils.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme/variant_effect.py` & `tangermeme-0.2.1/tangermeme/variant_effect.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tangermeme.egg-info/PKG-INFO` & `tangermeme-0.2.1/tangermeme.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tangermeme
-Version: 0.2.0
+Version: 0.2.1
 Summary: Biological sequence analysis for the modern age.
 Home-page: https://github.com/jmschrei/tangermeme
 Author: Jacob Schreiber
 Author-email: jmschreiber91@gmail.com
 License: LICENSE.txt
 License-File: LICENSE
 Requires-Dist: numpy>=1.14.2
```

### Comparing `tangermeme-0.2.0/tangermeme.egg-info/SOURCES.txt` & `tangermeme-0.2.1/tangermeme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_ablate.py` & `tangermeme-0.2.1/tests/test_ablate.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_deep_lift_shap.py` & `tangermeme-0.2.1/tests/test_deep_lift_shap.py`

 * *Files 0% similar despite different names*

```diff
@@ -550,17 +550,17 @@
 	assert_raises(IndexError, deep_lift_shap, model, X, args=(alpha[:5], 
 		beta[:3]), device='cpu')
 	assert_raises(IndexError, deep_lift_shap, model, X, args=(alpha, beta[:3]),
 		device='cpu')
 	
 	assert_raises(IndexError, deep_lift_shap, model, X, 
 		references=references[:10], device='cpu')
-	assert_raises(AssertionError, deep_lift_shap, model, X, 
+	assert_raises(RuntimeError, deep_lift_shap, model, X, 
 		references=references[:, :, :2], device='cpu')
-	assert_raises(AssertionError, deep_lift_shap, model, X, 
+	assert_raises(RuntimeError, deep_lift_shap, model, X, 
 		references=references[:, :, :, :10], device='cpu')
 
 
 ### Test a bunch of different models with different configurations/operations
 
 
 def test_deep_lift_shap_flattendense(X):
```

### Comparing `tangermeme-0.2.0/tests/test_ersatz.py` & `tangermeme-0.2.1/tests/test_ersatz.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_io.py` & `tangermeme-0.2.1/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_ism.py` & `tangermeme-0.2.1/tests/test_ism.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_kmers.py` & `tangermeme-0.2.1/tests/test_kmers.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_marginalize.py` & `tangermeme-0.2.1/tests/test_marginalize.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_match.py` & `tangermeme-0.2.1/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_predict.py` & `tangermeme-0.2.1/tests/test_predict.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_product.py` & `tangermeme-0.2.1/tests/test_product.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_seqlet.py` & `tangermeme-0.2.1/tests/test_seqlet.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_space.py` & `tangermeme-0.2.1/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_utils.py` & `tangermeme-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tangermeme-0.2.0/tests/test_variant_effect.py` & `tangermeme-0.2.1/tests/test_variant_effect.py`

 * *Files identical despite different names*

