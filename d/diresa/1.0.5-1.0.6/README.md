# Comparing `tmp/diresa-1.0.5.tar.gz` & `tmp/diresa-1.0.6.tar.gz`

## Comparing `diresa-1.0.5.tar` & `diresa-1.0.6.tar`

### file list

```diff
@@ -1,19 +1,27 @@
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 diresa-1.0.5/pyproject.toml.bak
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/__init__.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/callback.py
--rw-r--r--   0        0        0     2825 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/layers.py
--rw-r--r--   0        0        0     7529 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/loss.py
--rw-r--r--   0        0        0    25668 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/models.py
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/toolbox.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/.idea/.gitignore
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/.idea/diresa.iml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/.idea/misc.xml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/.idea/modules.xml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/.idea/vcs.xml
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/.idea/workspace.xml
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 diresa-1.0.5/src/diresa/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 diresa-1.0.5/LICENSE
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 diresa-1.0.5/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 diresa-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 diresa-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 diresa-1.0.6/.readthedocs.yaml
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/build.rst
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/conf.py
+-rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/custom.rst
+-rw-r--r--   0        0        0   451592 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/diresa.ipynb
+-rw-r--r--   0        0        0    32517 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/diresa.png
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/eval.rst
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/index.rst
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/install.rst
+-rw-r--r--   0        0        0   203392 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/latent.png
+-rw-r--r--   0        0        0  3039998 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/lorenz.csv
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/loss.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/models.rst
+-rw-r--r--   0        0        0   112518 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/reconstruction.png
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/requirements.txt
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 diresa-1.0.6/docs/start.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 diresa-1.0.6/src/diresa/__init__.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 diresa-1.0.6/src/diresa/callback.py
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 diresa-1.0.6/src/diresa/layers.py
+-rw-r--r--   0        0        0     7530 2020-02-02 00:00:00.000000 diresa-1.0.6/src/diresa/loss.py
+-rw-r--r--   0        0        0    25669 2020-02-02 00:00:00.000000 diresa-1.0.6/src/diresa/models.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 diresa-1.0.6/src/diresa/toolbox.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 diresa-1.0.6/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 diresa-1.0.6/LICENSE
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 diresa-1.0.6/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 diresa-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 diresa-1.0.6/PKG-INFO
```

### Comparing `diresa-1.0.5/src/diresa/callback.py` & `diresa-1.0.6/src/diresa/callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 """
 DIRESA callback classes/functions
 :Author:  Geert De Paepe
 :Email:   geert.de.paepe@vub.be
-:License: Apache 2.0
+:License: MIT License
 """
 
 import tensorflow as tf
 from keras.callbacks import Callback
 
 
 class LossWeightAnnealing(Callback):
```

### Comparing `diresa-1.0.5/src/diresa/layers.py` & `diresa-1.0.6/src/diresa/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 """
 DIRESA custom layer classes
 :Author:  Geert De Paepe
 :Email:   geert.de.paepe@vub.be
-:License: Apache 2.0
+:License: MIT License
 """
 
 import keras
 import tensorflow as tf
 from keras import layers
 
 class Sampling(layers.Layer):
```

### Comparing `diresa-1.0.5/src/diresa/loss.py` & `diresa-1.0.6/src/diresa/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 """
 DIRESA loss classes/functions
 :Author:  Geert De Paepe
 :Email:   geert.de.paepe@vub.be
-:License: Apache 2.0
+:License: MIT License
 """
 
 import tensorflow as tf
 import tensorflow_probability as tfp
 from keras.losses import Loss
```

### Comparing `diresa-1.0.5/src/diresa/models.py` & `diresa-1.0.6/src/diresa/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """
 Creates DIRESA and (V)AE models out of an encoder and decoder model
 Creates DIRESA and AE models from hyperparameters
 :Author:  Geert De Paepe
 :Email:   geert.de.paepe@vub.be
-:License: Apache 2.0
+:License: MIT License
 
 1. Creating (V)AE and Diresa models out of an encoder and decoder model:
  - autoencoder_model(x, encoder, decoder, mask_layer=False)
  - vae_model(x, encoder, decoder)
  - cov_reg_ae_model(x, encoder, decoder)
  - siamese_twin_model(x, x_twin, encoder, decoder)
  - diresa_model(x, x_twin, encoder, decoder)
```

### Comparing `diresa-1.0.5/src/diresa/toolbox.py` & `diresa-1.0.6/src/diresa/toolbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 """
 DIRESA helper functions
 :Author:  Geert De Paepe
 :Email:   geert.de.paepe@vub.be
-:License: Apache 2.0
+:License: MIT License
 """
 
 from keras.models import Model
 from diresa.layers import MaskLayer, DistLayer, Sampling
 from diresa.loss import (mae_dist_loss, male_dist_loss, mape_dist_loss, mse_dist_loss, msle_dist_loss,
                   corr_dist_loss, corr_log_dist_loss, loc_corr_dist_loss,
                   spear_dist_loss, canberra_dist_loss, LatentCovLoss, KLLoss)
```

### Comparing `diresa-1.0.5/LICENSE` & `diresa-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `diresa-1.0.5/pyproject.toml` & `diresa-1.0.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "diresa"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Geert De Paepe", email="geert.de.paepe@vub.be" },
 ]
 description = "Diresa - distance-regularized siamese twin autoencoder"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
@@ -16,14 +16,14 @@
   "tensorflow_probability>=0.15",
 ]
 keywords = ["weather", "climate", "tensorflow", "machine", "learning"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: Apache Software License",
+    "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 	"Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 [project.urls]
-Homepage = "https://gitlab.com/etrovub/ai4wcm/geert/diresa"
-Issues = "https://gitlab.com/etrovub/ai4wcm/geert/diresa/-/issues"
+Homepage = "https://gitlab.com/etrovub/ai4wcm/public/diresa"
+Issues = "https://gitlab.com/etrovub/ai4wcm/public/diresa/-/issues"
```

