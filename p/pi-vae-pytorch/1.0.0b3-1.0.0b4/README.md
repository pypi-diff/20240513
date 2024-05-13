# Comparing `tmp/pi-vae-pytorch-1.0.0b3.tar.gz` & `tmp/pi_vae_pytorch-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pi-vae-pytorch-1.0.0b3.tar", last modified: Wed Apr  3 02:42:45 2024, max compression
+gzip compressed data, was "pi_vae_pytorch-1.0.0b4.tar", last modified: Mon May 13 20:55:09 2024, max compression
```

## Comparing `pi-vae-pytorch-1.0.0b3.tar` & `pi_vae_pytorch-1.0.0b4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:42:45.926142 pi-vae-pytorch-1.0.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-03 02:42:45.926142 pi-vae-pytorch-1.0.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8183 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:42:45.922142 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/decoders.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/encoders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10690 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/pivae.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5270 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:42:45.926142 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9491 2024-04-03 02:42:45.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-03 02:42:45.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:42:45.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 02:42:45.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 02:42:45.000000 pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-03 02:42:41.000000 pi-vae-pytorch-1.0.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:42:45.926142 pi-vae-pytorch-1.0.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:55:09.750943 pi_vae_pytorch-1.0.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-05-13 20:55:09.750943 pi_vae_pytorch-1.0.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10183 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:55:09.750943 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/decoders.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1296 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/pivae.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3712 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 20:55:09.750943 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-05-13 20:55:09.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-13 20:55:09.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 20:55:09.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-13 20:55:09.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 20:55:09.000000 pi_vae_pytorch-1.0.0b4/pi_vae_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-05-13 20:55:05.000000 pi_vae_pytorch-1.0.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 20:55:09.750943 pi_vae_pytorch-1.0.0b4/setup.cfg
```

### Comparing `pi-vae-pytorch-1.0.0b3/.gitignore` & `pi_vae_pytorch-1.0.0b4/.gitignore`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b3/LICENSE` & `pi_vae_pytorch-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b3/PKG-INFO` & `pi_vae_pytorch-1.0.0b4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,66 @@
-Metadata-Version: 2.1
-Name: pi-vae-pytorch
-Version: 1.0.0b3
-Summary: A Pytorch implementation of Poisson Identifiable VAE (pi-VAE), a variational auto encoder used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables.
-Author-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
-Maintainer-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
-Project-URL: Homepage, https://mmcinnestaylor.github.io/pi-vae-pytorch/
-Project-URL: Repository, https://github.com/mmcinnestaylor/pi-vae-pytorch
-Keywords: vae,pi-vae,poisson identifiable vae,poisson identifiable variational autoencoder,identifiable vae,identifiable variational autoencoder
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-
 # Poisson Identifiable VAE (pi-VAE)
 
 This is a Pytorch implementation of [Poisson Identifiable VAE (pi-VAE)](https://arxiv.org/abs/2011.04798), used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables (non-neural variables, e.g. sensory, motor, and other externally observable states).
 
-The original implementation by [Dr. Ding Zhou](https://zhd96.github.io/) and [Dr. Xue-Xin Wei](https://sites.google.com/view/xxweineuraltheory/) in Tensorflow 1.13 is available [here](https://github.com/zhd96/pi-vae).
+The original implementation by [Ding Zhou](https://zhd96.github.io/) and [Xue-Xin Wei](https://sites.google.com/view/xxweineuraltheory/) in Tensorflow 1.13 is available [here](https://github.com/zhd96/pi-vae).
+
+Another Pytorch implementation by [Lyndon Duong](http://lyndonduong.com/) is available [here](https://github.com/lyndond/lyndond.github.io/blob/0865902edb4648a8690ed8d449573d9236a72406/code/2021-11-25-pivae.ipynb).  
 
-Another Pytorch implementation by [Dr. Lyndon Duong](http://lyndonduong.com/) is available [here](https://github.com/lyndond/lyndond.github.io/blob/0865902edb4648a8690ed8d449573d9236a72406/code/2021-11-25-pivae.ipynb).
+A special thank you to [Zhongxuan Wu](https://github.com/ZhongxuanWu) who helped in the design and testing of this implementation. 
 
 ## Install
 
 ```
 pip install pi-vae-pytorch
 ```
 
+### From Source
+
+For those interested in modifying and testing the codebase, using an editable `pip` installation is recommended:
+
+```
+# pi-vae-pytorch/
+
+pip install -e .
+```
+
+## Model Architecture
+
+pi-VAE is comprised of three main components: the encoder, the label prior estimator, and the decoder. 
+
+### MLP Structure
+
+The Multi Layer Perceptron (MLP) is the primary building block of the aforementioned components. Each MLP used in this implementation is configurable by specifying the appropriate parameters when `PiVAE` is initialized:  
+- number of hidden layers  
+- hidden layer dimension  
+    - applied to all hidden layers within a given MLP
+- hidden layer activation function  
+    - applied to all non-output layer activations within a given MLP
+
+### Encoder
+
+The model's encoder is comprised of a single MLP, which learns the distribution q(z \| x). 
+
+### Label Prior Estimator
+
+The model's label prior estimator learns the distribution p(z \| u). In the discrete label regime this module is comprised of a single `nn.Embedding` layer, while in the continuous label regime the module is comprised of a MLP.
+
+### Decoder
+
+The model's decoder learns to map a latent sample `z` to the predicted firing rate of the latent sample. Inputs to the decoder are passed through the following submodules. 
+
+#### NFlowLayer
+
+This module is comprised of a MLP which maps `z` to the concatenation of `z` and `t(z)`.
+
+#### GINBlock
+
+Outputs from the `NFlowLayer` are passed to a series of `GINBlock` modules. Each `GINBlock` is comprised of a specified number of `AffineCouplingLayer` modules. Each `AffineCouplingLayer` is comprised of a MLP and performs an affine coupling transformation.
+
 ## Usage
 
 ```
 import torch
 from pi_vae_pytorch import PiVAE
 
 model = PiVAE(
@@ -48,15 +70,15 @@
     discrete_labels=False
 )
 
 x = torch.randn(1, 100) # Size([n_samples, x_dim])
 
 u = torch.randn(1, 3) # Size([n_samples, u_dim])
 
-outputs = model(x, u) # dict
+outputs = model(x, u) # Dict
 ```
 
 ### Parameters
 
 - `x_dim`: int  
     Dimension of observation `x`
 - `u_dim`: int  
@@ -84,35 +106,35 @@
 
     Number of GIN blocks used within the model's decoder. 
 - `decoder_gin_block_depth`: int   
     - Default: `2`  
 
     Number of AffineCouplingLayers which comprise each GIN block.
 - `decoder_affine_input_layer_slice_dim`: int  
-    - Default None (corresponds to `x_dim / 2`)  
+    - Default None (corresponds to `x_dim // 2`)  
 
     Index at which to split an n-dimensional input x. 
 - `decoder_affine_n_hidden_layers`: int  
     - Default: `2`  
 
     Number of hidden layers in the MLP of the model's encoder. 
 - `decoder_affine_hidden_layer_dim`: int  
-    - Default: `None` (corresponds to `x_dim / 4`)  
+    - Default: `None` (corresponds to `x_dim // 4`)  
 
     Dimensionality of each hidden layer in the MLP of each AffineCouplingLayer. 
 - `decoder_affine_hidden_layer_activation`: nn.Module  
     - Default: `nn.ReLU`  
 
     Activation function applied to the outputs of each hidden layer in the MLP of each AffineCouplingLayer. 
 - `decoder_nflow_n_hidden_layers`: int  
     - Default: `2`  
 
     Number of hidden layers in the MLP of the decoder's NFlowLayer. 
 - `decoder_nflow_hidden_layer_dim`: int  
-    - Default: `None` (corresponds to `x_dim / 4`)  
+    - Default: `None` (corresponds to `x_dim // 4`)  
 
     Dimensionality of each hidden layer in the MLP of the decoder's NFlowLayer. 
 - `decoder_nflow_hidden_layer_activation`: nn.Module   
     - Default: `nn.ReLU`  
 
     Activation function applied to the outputs of each hidden layer in the MLP of the decoder's NFlowLayer. 
 - `decoder_observation_model`: str  
@@ -130,29 +152,29 @@
     - Only applied when `decoder_observation_model="poisson"`
 
     Maximum threshold used when clamping decoded firing rates.
 - `z_prior_n_hidden_layers`: int  
     - Default: `2`  
     - Only applied when `discrete_labels=False`  
 
-    Number of hidden layers in the MLP of the ZPriorContinuous module. 
+    Number of hidden layers in the MLP of the label prior estimator module. 
 - `z_prior_hidden_layer_dim`: int  
     - Default: `20`  
     - Only applied when `discrete_labels=False`
 
-    Dimensionality of each hidden layer in the MLP of the ZPriorContinuous module. 
+    Dimensionality of each hidden layer in the MLP of the label prior estimator module. 
 - `z_prior_hidden_layer_activation`: nn.Module  
     - Default: `nn.Tanh`  
     - Only applied when `discrete_labels=False`
 
-    Activation function applied to the outputs of each hidden layer in the MLP of the decoder's ZPriorContinuous module. 
+    Activation function applied to the outputs of each hidden layer in the MLP of the label prior estimator module. 
 
 ### Returns
 
-A dicitonary with the following items. 
+A `Dict` with the following items. 
 
 - `firing_rate`: Tensor   
     - Size([n_samples, x_dim])  
 
     Predicted firing rates of `z_sample`. 
 - `lambda_mean`: Tensor  
     - Size([n_samples, z_dim])  
@@ -181,14 +203,16 @@
 - `z_sample`: Tensor  
     - Size([n_samples, z_dim])  
     
     Generated latents `z`. 
 
 ## Loss Function
 
+pi-VAE learns the deep generative model and the approximate posterior q(z \| x, u) of the true posterior p(z \| x, u) by maximizing the evidence lower bound (ELBO) of p(x \| u).
+
 ### Poisson observation model
 
 ```
 from pi_vae_pytorch.utils import compute_loss
 
 outputs = model(x, u) # Initialized with decoder_observation_model="poisson" 
 
@@ -257,15 +281,15 @@
     - Should use the same value passed to `decoder_observation_model` when initializing `PiVAE`.  
 
     The observation model used by pi-VAE's decoder.
 - `observation_noise_model`: nn.Module 
     - Default: None  
     - Only applied when `observation model="gaussian"`  
     
-    The noise model used when pi-VAE's decoder utilizes a Gaussian observation model. When `PiVAE` is initialized with `decoder_observation_model="gaussian"`, the model's `observation_noise_model` attribute can be used.
+    The noise model used when pi-VAE's decoder utilizes a Gaussian observation model. When `PiVAE` is initialized with `decoder_observation_model="gaussian"`, the model's `observation_noise_model` attribute should be used.
 
 ## Citation
 
 ```
 @misc{zhou2020learning,
     title={Learning identifiable and interpretable latent models of high-dimensional neural activity using pi-VAE}, 
     author={Ding Zhou and Xue-Xin Wei},
```

### Comparing `pi-vae-pytorch-1.0.0b3/README.md` & `pi_vae_pytorch-1.0.0b4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,89 @@
+Metadata-Version: 2.1
+Name: pi-vae-pytorch
+Version: 1.0.0b4
+Summary: A Pytorch implementation of Poisson Identifiable VAE (pi-VAE), a variational auto encoder used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables.
+Author-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
+Maintainer-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
+Project-URL: Homepage, https://mmcinnestaylor.github.io/pi-vae-pytorch/
+Project-URL: Repository, https://github.com/mmcinnestaylor/pi-vae-pytorch
+Keywords: vae,pi-vae,poisson identifiable vae,poisson identifiable variational autoencoder,identifiable vae,identifiable variational autoencoder
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: torch
+
 # Poisson Identifiable VAE (pi-VAE)
 
 This is a Pytorch implementation of [Poisson Identifiable VAE (pi-VAE)](https://arxiv.org/abs/2011.04798), used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables (non-neural variables, e.g. sensory, motor, and other externally observable states).
 
-The original implementation by [Dr. Ding Zhou](https://zhd96.github.io/) and [Dr. Xue-Xin Wei](https://sites.google.com/view/xxweineuraltheory/) in Tensorflow 1.13 is available [here](https://github.com/zhd96/pi-vae).
+The original implementation by [Ding Zhou](https://zhd96.github.io/) and [Xue-Xin Wei](https://sites.google.com/view/xxweineuraltheory/) in Tensorflow 1.13 is available [here](https://github.com/zhd96/pi-vae).
+
+Another Pytorch implementation by [Lyndon Duong](http://lyndonduong.com/) is available [here](https://github.com/lyndond/lyndond.github.io/blob/0865902edb4648a8690ed8d449573d9236a72406/code/2021-11-25-pivae.ipynb).  
 
-Another Pytorch implementation by [Dr. Lyndon Duong](http://lyndonduong.com/) is available [here](https://github.com/lyndond/lyndond.github.io/blob/0865902edb4648a8690ed8d449573d9236a72406/code/2021-11-25-pivae.ipynb).
+A special thank you to [Zhongxuan Wu](https://github.com/ZhongxuanWu) who helped in the design and testing of this implementation. 
 
 ## Install
 
 ```
 pip install pi-vae-pytorch
 ```
 
+### From Source
+
+For those interested in modifying and testing the codebase, using an editable `pip` installation is recommended:
+
+```
+# pi-vae-pytorch/
+
+pip install -e .
+```
+
+## Model Architecture
+
+pi-VAE is comprised of three main components: the encoder, the label prior estimator, and the decoder. 
+
+### MLP Structure
+
+The Multi Layer Perceptron (MLP) is the primary building block of the aforementioned components. Each MLP used in this implementation is configurable by specifying the appropriate parameters when `PiVAE` is initialized:  
+- number of hidden layers  
+- hidden layer dimension  
+    - applied to all hidden layers within a given MLP
+- hidden layer activation function  
+    - applied to all non-output layer activations within a given MLP
+
+### Encoder
+
+The model's encoder is comprised of a single MLP, which learns the distribution q(z \| x). 
+
+### Label Prior Estimator
+
+The model's label prior estimator learns the distribution p(z \| u). In the discrete label regime this module is comprised of a single `nn.Embedding` layer, while in the continuous label regime the module is comprised of a MLP.
+
+### Decoder
+
+The model's decoder learns to map a latent sample `z` to the predicted firing rate of the latent sample. Inputs to the decoder are passed through the following submodules. 
+
+#### NFlowLayer
+
+This module is comprised of a MLP which maps `z` to the concatenation of `z` and `t(z)`.
+
+#### GINBlock
+
+Outputs from the `NFlowLayer` are passed to a series of `GINBlock` modules. Each `GINBlock` is comprised of a specified number of `AffineCouplingLayer` modules. Each `AffineCouplingLayer` is comprised of a MLP and performs an affine coupling transformation.
+
 ## Usage
 
 ```
 import torch
 from pi_vae_pytorch import PiVAE
 
 model = PiVAE(
@@ -25,15 +93,15 @@
     discrete_labels=False
 )
 
 x = torch.randn(1, 100) # Size([n_samples, x_dim])
 
 u = torch.randn(1, 3) # Size([n_samples, u_dim])
 
-outputs = model(x, u) # dict
+outputs = model(x, u) # Dict
 ```
 
 ### Parameters
 
 - `x_dim`: int  
     Dimension of observation `x`
 - `u_dim`: int  
@@ -61,35 +129,35 @@
 
     Number of GIN blocks used within the model's decoder. 
 - `decoder_gin_block_depth`: int   
     - Default: `2`  
 
     Number of AffineCouplingLayers which comprise each GIN block.
 - `decoder_affine_input_layer_slice_dim`: int  
-    - Default None (corresponds to `x_dim / 2`)  
+    - Default None (corresponds to `x_dim // 2`)  
 
     Index at which to split an n-dimensional input x. 
 - `decoder_affine_n_hidden_layers`: int  
     - Default: `2`  
 
     Number of hidden layers in the MLP of the model's encoder. 
 - `decoder_affine_hidden_layer_dim`: int  
-    - Default: `None` (corresponds to `x_dim / 4`)  
+    - Default: `None` (corresponds to `x_dim // 4`)  
 
     Dimensionality of each hidden layer in the MLP of each AffineCouplingLayer. 
 - `decoder_affine_hidden_layer_activation`: nn.Module  
     - Default: `nn.ReLU`  
 
     Activation function applied to the outputs of each hidden layer in the MLP of each AffineCouplingLayer. 
 - `decoder_nflow_n_hidden_layers`: int  
     - Default: `2`  
 
     Number of hidden layers in the MLP of the decoder's NFlowLayer. 
 - `decoder_nflow_hidden_layer_dim`: int  
-    - Default: `None` (corresponds to `x_dim / 4`)  
+    - Default: `None` (corresponds to `x_dim // 4`)  
 
     Dimensionality of each hidden layer in the MLP of the decoder's NFlowLayer. 
 - `decoder_nflow_hidden_layer_activation`: nn.Module   
     - Default: `nn.ReLU`  
 
     Activation function applied to the outputs of each hidden layer in the MLP of the decoder's NFlowLayer. 
 - `decoder_observation_model`: str  
@@ -107,29 +175,29 @@
     - Only applied when `decoder_observation_model="poisson"`
 
     Maximum threshold used when clamping decoded firing rates.
 - `z_prior_n_hidden_layers`: int  
     - Default: `2`  
     - Only applied when `discrete_labels=False`  
 
-    Number of hidden layers in the MLP of the ZPriorContinuous module. 
+    Number of hidden layers in the MLP of the label prior estimator module. 
 - `z_prior_hidden_layer_dim`: int  
     - Default: `20`  
     - Only applied when `discrete_labels=False`
 
-    Dimensionality of each hidden layer in the MLP of the ZPriorContinuous module. 
+    Dimensionality of each hidden layer in the MLP of the label prior estimator module. 
 - `z_prior_hidden_layer_activation`: nn.Module  
     - Default: `nn.Tanh`  
     - Only applied when `discrete_labels=False`
 
-    Activation function applied to the outputs of each hidden layer in the MLP of the decoder's ZPriorContinuous module. 
+    Activation function applied to the outputs of each hidden layer in the MLP of the label prior estimator module. 
 
 ### Returns
 
-A dicitonary with the following items. 
+A `Dict` with the following items. 
 
 - `firing_rate`: Tensor   
     - Size([n_samples, x_dim])  
 
     Predicted firing rates of `z_sample`. 
 - `lambda_mean`: Tensor  
     - Size([n_samples, z_dim])  
@@ -158,14 +226,16 @@
 - `z_sample`: Tensor  
     - Size([n_samples, z_dim])  
     
     Generated latents `z`. 
 
 ## Loss Function
 
+pi-VAE learns the deep generative model and the approximate posterior q(z \| x, u) of the true posterior p(z \| x, u) by maximizing the evidence lower bound (ELBO) of p(x \| u).
+
 ### Poisson observation model
 
 ```
 from pi_vae_pytorch.utils import compute_loss
 
 outputs = model(x, u) # Initialized with decoder_observation_model="poisson" 
 
@@ -234,15 +304,15 @@
     - Should use the same value passed to `decoder_observation_model` when initializing `PiVAE`.  
 
     The observation model used by pi-VAE's decoder.
 - `observation_noise_model`: nn.Module 
     - Default: None  
     - Only applied when `observation model="gaussian"`  
     
-    The noise model used when pi-VAE's decoder utilizes a Gaussian observation model. When `PiVAE` is initialized with `decoder_observation_model="gaussian"`, the model's `observation_noise_model` attribute can be used.
+    The noise model used when pi-VAE's decoder utilizes a Gaussian observation model. When `PiVAE` is initialized with `decoder_observation_model="gaussian"`, the model's `observation_noise_model` attribute should be used.
 
 ## Citation
 
 ```
 @misc{zhou2020learning,
     title={Learning identifiable and interpretable latent models of high-dimensional neural activity using pi-VAE}, 
     author={Ding Zhou and Xue-Xin Wei},
```

### Comparing `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/decoders.py` & `pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/decoders.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,20 +56,20 @@
         )
 
         layers = []
         for _ in range(n_gin_blocks):
             layers.append(PermutationLayer(x_dim))
             layers.append(
                 GINBlock(
-                        x_dim=x_dim,
-                        n_affine_layers=gin_block_depth,
-                        affine_input_layer_slice_dim=affine_input_layer_slice_dim,
-                        affine_n_hidden_layers=affine_n_hidden_layers,
-                        affine_hidden_layer_dim=affine_hidden_layer_dim,
-                        affine_hidden_layer_activation=affine_hidden_layer_activation
+                    x_dim=x_dim,
+                    n_affine_layers=gin_block_depth,
+                    affine_input_layer_slice_dim=affine_input_layer_slice_dim,
+                    affine_n_hidden_layers=affine_n_hidden_layers,
+                    affine_hidden_layer_dim=affine_hidden_layer_dim,
+                    affine_hidden_layer_activation=affine_hidden_layer_activation
                 )
             )
 
         self.gin_blocks = nn.Sequential(*layers)
     
     def forward(
         self,
```

### Comparing `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/encoders.py` & `pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/encoders.py`

 * *Files identical despite different names*

### Comparing `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/layers.py` & `pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/layers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from typing import Tuple
 
 import torch
 from torch import nn, Tensor
 
-from pi_vae_pytorch.utils import build_mlp_layers
-
 
 class MLP(nn.Module):
     """
     A basic Multilayer Perceptron (MLP) module.
 
     Parameters
     ----------
@@ -25,28 +23,33 @@
         out_features: int,
         n_hidden_layers: int,
         hidden_layer_features: int,
         activation: nn.Module
         ) -> None:
         super().__init__()
 
-        self.net = nn.ModuleList([])
-
         # Construct layer dims
         dims = [in_features]
         for _ in range(n_hidden_layers * 2):
             dims.append(hidden_layer_features)
         dims.append(out_features)
 
-        # Construct MLP
-        self.net = build_mlp_layers(
-            n_hidden_layers=n_hidden_layers,
-            hidden_layer_dims=dims,
-            activation=activation
-        )
+        # Build layers
+        layers = []
+        act = activation
+
+        for i in range(n_hidden_layers+1):
+            # Output layer
+            if i == n_hidden_layers:
+                act = nn.Identity
+            
+            layers.append(nn.Linear(dims[2*i], dims[2*i+1]))
+            layers.append(act())
+
+        self.net = nn.Sequential(*layers)
 
     def forward(
         self,
         input: Tensor
         ) -> Tensor:
 
         return self.net(input)
@@ -170,15 +173,15 @@
         ) -> None:
         super().__init__()
 
         self.x_dim = x_dim
 
         # Compute slice dimension
         if x_slice_dim is None:
-            self.slice_dim = self.x_dim // 2
+            self.slice_dim = x_dim // 2
         else:
             if x_slice_dim >= x_dim:
                 raise ValueError(f"x_slice_dim must be less than x_dim.")
             self.slice_dim = x_slice_dim
 
         # Compute hidden layer dimension
         if hidden_layer_dim is not None:
@@ -202,15 +205,15 @@
         Perform affine coupling transform while preserving volume.
         """
 
         # Split input
         x_1 = torch.narrow(x, 1, 0, self.slice_dim)
         x_2 = torch.narrow(x, 1, self.slice_dim, self.x_dim - self.slice_dim)
 
-        # Compute scale and transla
+        # Compute scale and translation
         s_t = self.net(x_1)
         s_out = torch.narrow(s_t, 1, 0, self.x_dim - self.slice_dim - 1)
         t_out = torch.narrow(s_t, 1, self.x_dim - self.slice_dim - 1, self.x_dim - self.slice_dim)
 
         # clamp to ensure output of s is small
         s_out = 0.1 * torch.tanh(s_out)
         # preserve volume by ensuring the last layer has sum 0
@@ -302,15 +305,15 @@
             n_hidden_layers=n_hidden_layers,
             hidden_layer_features=hidden_layer_dim,
             activation=hidden_layer_activation
         )
     
     def forward(
         self,
-        u: torch.Tensor
+        u: Tensor
         ) -> Tuple[Tensor, Tensor]:
         """
         Maps u to mean and log of variance of p(z|u).
         """
         
         z_prior = self.net(u)
         # lambda_mean, lambda_log_variance
@@ -342,15 +345,15 @@
         self.embedded_log_variance = nn.Embedding(
             num_embeddings=u_dim,
             embedding_dim=z_dim
         )
 
     def forward(
         self,
-        u: torch.Tensor
+        u: Tensor
         ) -> Tuple[Tensor, Tensor]:
         """
         Maps u to mean and log of variance of p(z|u).
         """
 
         # lambda_mean, lambda_log_variance
         return self.embedded_mean(u), self.embedded_log_variance(u)
```

### Comparing `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/pivae.py` & `pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/pivae.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Dict
 
-from torch import clamp, nn, Tensor
+import torch
+from torch import nn, Tensor
 
 from pi_vae_pytorch.decoders import GINFlowDecoder
 from pi_vae_pytorch.encoders import MLPEncoder
 from pi_vae_pytorch.layers import ZPriorContinuous, ZPriorDiscrete
-from pi_vae_pytorch.utils import compute_posterior, generate_latent_z
+from pi_vae_pytorch.utils import compute_posterior
 
 
 class PiVAE(nn.Module):
     """
     The pi-VAE model which constructs a latent variable model of neural activity while 
     simultaneously modeling the relation between the latent and task variables.
 
@@ -37,17 +38,18 @@
     z_prior_n_hidden_layers (int) - number of the ZPriorContinuous's MLP hidden layers. Default: 2
     z_prior_hidden_layer_dim (int) - dimension of the ZPriorContinuous's MLP hidden layers. Default: 20
     z_prior_hidden_layer_activation (nn.Module) - activation function applied to the ZPriorContinuous's MLP hidden layers. Default: nn.Tanh
 
     Notes
     -----
     decoder_affine_input_layer_slice_dim (int) - when None, x_dim // 2 is assigned. Otherwise assigns the specified value, assuming 0 < decoder_affine_input_layer_slice_dim < x_dim.
-    decoder_affine_hidden_layer_dim (int) - when None, x_dim // 4 is assigned. Otherwise max(affine_hidden_layer_dim, x_dim // 4).
-    decoder_nflow_hidden_layer_dim (int) - when None, x_dim // 4 is assigned. Otherwise max(nflow_hidden_layer_dim, x_dim // 4).
+    decoder_affine_hidden_layer_dim (int) - when None, x_dim // 4 is assigned. Otherwise max(decoder_affine_hidden_layer_dim, x_dim // 4).
+    decoder_nflow_hidden_layer_dim (int) - when None, x_dim // 4 is assigned. Otherwise max(decoder_nflow_hidden_layer_dim, x_dim // 4).
     """
+    
     def __init__(
         self,
         x_dim: int,
         u_dim: int,
         z_dim: int,
         discrete_labels: bool = True,
         encoder_n_hidden_layers: int = 2,
@@ -78,14 +80,16 @@
                 bias=False
             )
         elif decoder_observation_model == "poisson":
             self.observation_noise_model = None
         else:
             raise ValueError(f"Invalid observation model: {decoder_observation_model}")
         
+        self.decoder_observation_model = decoder_observation_model
+        
         self.decoder = GINFlowDecoder(
             x_dim=x_dim,
             z_dim=z_dim,
             n_gin_blocks=decoder_n_gin_blocks,
             gin_block_depth=decoder_gin_block_depth,
             affine_input_layer_slice_dim=decoder_affine_input_layer_slice_dim,
             affine_n_hidden_layers=decoder_affine_n_hidden_layers,
@@ -93,17 +97,20 @@
             affine_hidden_layer_activation=decoder_affine_hidden_layer_activation,
             nflow_n_hidden_layers=decoder_nflow_n_hidden_layers,
             nflow_hidden_layer_dim=decoder_nflow_hidden_layer_dim,
             nflow_hidden_layer_activation=decoder_nflow_hidden_layer_activation,
             observation_model=decoder_observation_model
         )
 
-        self.decoder_fr_clamp_min = decoder_fr_clamp_min
-        self.decoder_fr_clamp_max = decoder_fr_clamp_max
-        self.decoder_observation_model = decoder_observation_model
+        if decoder_fr_clamp_min < decoder_fr_clamp_max:
+            self.decoder_fr_clamp_min = decoder_fr_clamp_min
+            self.decoder_fr_clamp_max = decoder_fr_clamp_max
+        else:
+            raise ValueError(f"decoder_fr_clamp_min: {decoder_fr_clamp_min} must be less than decoder_fr_clamp_max: {decoder_fr_clamp_max}")
+        
         
         self.encoder = MLPEncoder(
             x_dim=x_dim,
             z_dim=z_dim,
             n_hidden_layers=encoder_n_hidden_layers,
             hidden_layer_dim=encoder_hidden_layer_dim,
             activation=encoder_hidden_layer_activation
@@ -135,23 +142,20 @@
         # Map each sample observation x to latent z approximating q(z|x)
         z_mean, z_log_variance = self.encoder(x)  
 
         # Compute the full posterior of q(z|x,u)~q(z|x)p(z|u) as a product of Gaussians
         posterior_mean, posterior_log_variance = compute_posterior(z_mean, z_log_variance, lambda_mean, lambda_log_variance)  
 
         # Sample latent z using reparameterization trick
-        z_sample = generate_latent_z(
-            mean=posterior_mean,
-            log_variance=posterior_log_variance
-        )  
+        z_sample = posterior_mean + torch.exp(0.5 * posterior_log_variance) * torch.randn_like(posterior_mean)
 
         # Generate firing rate using sampled latent z
         firing_rate = self.decoder(z_sample)
         if self.decoder_observation_model == "poisson":
-            firing_rate = clamp(firing_rate, min=self.decoder_fr_clamp_min, max=self.decoder_fr_clamp_max)
+            firing_rate = torch.clamp(firing_rate, min=self.decoder_fr_clamp_min, max=self.decoder_fr_clamp_max)
 
         return {
             "firing_rate": firing_rate,
             "lambda_mean": lambda_mean,
             "lambda_log_variance": lambda_log_variance,
             "posterior_mean": posterior_mean,
             "posterior_log_variance": posterior_log_variance,
```

### Comparing `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch/utils.py` & `pi_vae_pytorch-1.0.0b4/pi_vae_pytorch/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,11 @@
-from typing import List
-
 import torch
 from torch import nn, Tensor
 
 
-def build_mlp_layers(
-    n_hidden_layers: int,
-    hidden_layer_dims: List[int],
-    activation: nn.Module
-    ) -> nn.Sequential:
-    """
-    Helper method to construct a Multilayer Perceptron (MLP). 
-
-    Parameters
-    ----------
-    n_hidden_layers (int) - the number of hidden in the model
-    hidden_layer_dim (List[int]) - a list of integers specifying the input/output dimensions of each layer
-    activation (nn.Module) - the activation function to apply after each hidden layer
-
-    Returns
-    -------
-    nn.Sequential(*layers) - a Sequential container of the specified layers
-
-    Notes
-    -----
-    A nn.Identity activation is applied after the final layer.
-    """
-
-    layers = []
-    act = activation
-
-    # Build layers
-    for i in range(n_hidden_layers+1):
-        # Output layer
-        if i == n_hidden_layers:
-            act = nn.Identity
-        
-        layers.append(nn.Linear(hidden_layer_dims[2*i], hidden_layer_dims[2*i+1]))
-        layers.append(act())
-
-    return nn.Sequential(*layers)
-
 def compute_loss(
     x: Tensor,
     firing_rate: Tensor,
     lambda_mean: Tensor, 
     lambda_log_variance: Tensor,
     posterior_mean: Tensor, 
     posterior_log_variance: Tensor,
@@ -117,26 +78,7 @@
     """
 
     variance_difference = z_log_variance - lambda_log_variance
     posterior_mean = (z_mean / (1 + torch.exp(variance_difference))) + (lambda_mean / (1 + torch.exp(torch.neg(variance_difference))))
     posterior_log_variance = z_log_variance + lambda_log_variance - torch.log(torch.exp(z_log_variance) + torch.exp(lambda_log_variance))
 
     return posterior_mean, posterior_log_variance
-
-def generate_latent_z(
-    mean: Tensor,
-    log_variance: Tensor
-    ) -> Tensor:
-    """
-    Reparameterization trick by sampling from an isotropic unit Gaussian.
-
-    Parameters
-    -----------
-    mean (Tensor) - means of each z sample. Size([n_samples, z_dim])
-    log_variance (Tensor) - log of variances of each z sample. Size([n_samples, z_dim])
-
-    Returns
-    ------
-    Samples of latent z. Size([n_samples, z_dim])
-    """
-
-    return mean + torch.exp(0.5 * log_variance) * torch.randn_like(mean)
```

### Comparing `pi-vae-pytorch-1.0.0b3/pi_vae_pytorch.egg-info/PKG-INFO` & `pi_vae_pytorch-1.0.0b4/pi_vae_pytorch.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pi-vae-pytorch
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: A Pytorch implementation of Poisson Identifiable VAE (pi-VAE), a variational auto encoder used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables.
 Author-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
 Maintainer-email: Marlan McInnes-Taylor <mmcinnestaylor@gmail.com>
 Project-URL: Homepage, https://mmcinnestaylor.github.io/pi-vae-pytorch/
 Project-URL: Repository, https://github.com/mmcinnestaylor/pi-vae-pytorch
 Keywords: vae,pi-vae,poisson identifiable vae,poisson identifiable variational autoencoder,identifiable vae,identifiable variational autoencoder
 Classifier: Development Status :: 5 - Production/Stable
@@ -21,24 +21,69 @@
 License-File: LICENSE
 Requires-Dist: torch
 
 # Poisson Identifiable VAE (pi-VAE)
 
 This is a Pytorch implementation of [Poisson Identifiable VAE (pi-VAE)](https://arxiv.org/abs/2011.04798), used to construct latent variable models of neural activity while simultaneously modeling the relation between the latent and task variables (non-neural variables, e.g. sensory, motor, and other externally observable states).
 
-The original implementation by [Dr. Ding Zhou](https://zhd96.github.io/) and [Dr. Xue-Xin Wei](https://sites.google.com/view/xxweineuraltheory/) in Tensorflow 1.13 is available [here](https://github.com/zhd96/pi-vae).
+The original implementation by [Ding Zhou](https://zhd96.github.io/) and [Xue-Xin Wei](https://sites.google.com/view/xxweineuraltheory/) in Tensorflow 1.13 is available [here](https://github.com/zhd96/pi-vae).
 
-Another Pytorch implementation by [Dr. Lyndon Duong](http://lyndonduong.com/) is available [here](https://github.com/lyndond/lyndond.github.io/blob/0865902edb4648a8690ed8d449573d9236a72406/code/2021-11-25-pivae.ipynb).
+Another Pytorch implementation by [Lyndon Duong](http://lyndonduong.com/) is available [here](https://github.com/lyndond/lyndond.github.io/blob/0865902edb4648a8690ed8d449573d9236a72406/code/2021-11-25-pivae.ipynb).  
+
+A special thank you to [Zhongxuan Wu](https://github.com/ZhongxuanWu) who helped in the design and testing of this implementation. 
 
 ## Install
 
 ```
 pip install pi-vae-pytorch
 ```
 
+### From Source
+
+For those interested in modifying and testing the codebase, using an editable `pip` installation is recommended:
+
+```
+# pi-vae-pytorch/
+
+pip install -e .
+```
+
+## Model Architecture
+
+pi-VAE is comprised of three main components: the encoder, the label prior estimator, and the decoder. 
+
+### MLP Structure
+
+The Multi Layer Perceptron (MLP) is the primary building block of the aforementioned components. Each MLP used in this implementation is configurable by specifying the appropriate parameters when `PiVAE` is initialized:  
+- number of hidden layers  
+- hidden layer dimension  
+    - applied to all hidden layers within a given MLP
+- hidden layer activation function  
+    - applied to all non-output layer activations within a given MLP
+
+### Encoder
+
+The model's encoder is comprised of a single MLP, which learns the distribution q(z \| x). 
+
+### Label Prior Estimator
+
+The model's label prior estimator learns the distribution p(z \| u). In the discrete label regime this module is comprised of a single `nn.Embedding` layer, while in the continuous label regime the module is comprised of a MLP.
+
+### Decoder
+
+The model's decoder learns to map a latent sample `z` to the predicted firing rate of the latent sample. Inputs to the decoder are passed through the following submodules. 
+
+#### NFlowLayer
+
+This module is comprised of a MLP which maps `z` to the concatenation of `z` and `t(z)`.
+
+#### GINBlock
+
+Outputs from the `NFlowLayer` are passed to a series of `GINBlock` modules. Each `GINBlock` is comprised of a specified number of `AffineCouplingLayer` modules. Each `AffineCouplingLayer` is comprised of a MLP and performs an affine coupling transformation.
+
 ## Usage
 
 ```
 import torch
 from pi_vae_pytorch import PiVAE
 
 model = PiVAE(
@@ -48,15 +93,15 @@
     discrete_labels=False
 )
 
 x = torch.randn(1, 100) # Size([n_samples, x_dim])
 
 u = torch.randn(1, 3) # Size([n_samples, u_dim])
 
-outputs = model(x, u) # dict
+outputs = model(x, u) # Dict
 ```
 
 ### Parameters
 
 - `x_dim`: int  
     Dimension of observation `x`
 - `u_dim`: int  
@@ -84,35 +129,35 @@
 
     Number of GIN blocks used within the model's decoder. 
 - `decoder_gin_block_depth`: int   
     - Default: `2`  
 
     Number of AffineCouplingLayers which comprise each GIN block.
 - `decoder_affine_input_layer_slice_dim`: int  
-    - Default None (corresponds to `x_dim / 2`)  
+    - Default None (corresponds to `x_dim // 2`)  
 
     Index at which to split an n-dimensional input x. 
 - `decoder_affine_n_hidden_layers`: int  
     - Default: `2`  
 
     Number of hidden layers in the MLP of the model's encoder. 
 - `decoder_affine_hidden_layer_dim`: int  
-    - Default: `None` (corresponds to `x_dim / 4`)  
+    - Default: `None` (corresponds to `x_dim // 4`)  
 
     Dimensionality of each hidden layer in the MLP of each AffineCouplingLayer. 
 - `decoder_affine_hidden_layer_activation`: nn.Module  
     - Default: `nn.ReLU`  
 
     Activation function applied to the outputs of each hidden layer in the MLP of each AffineCouplingLayer. 
 - `decoder_nflow_n_hidden_layers`: int  
     - Default: `2`  
 
     Number of hidden layers in the MLP of the decoder's NFlowLayer. 
 - `decoder_nflow_hidden_layer_dim`: int  
-    - Default: `None` (corresponds to `x_dim / 4`)  
+    - Default: `None` (corresponds to `x_dim // 4`)  
 
     Dimensionality of each hidden layer in the MLP of the decoder's NFlowLayer. 
 - `decoder_nflow_hidden_layer_activation`: nn.Module   
     - Default: `nn.ReLU`  
 
     Activation function applied to the outputs of each hidden layer in the MLP of the decoder's NFlowLayer. 
 - `decoder_observation_model`: str  
@@ -130,29 +175,29 @@
     - Only applied when `decoder_observation_model="poisson"`
 
     Maximum threshold used when clamping decoded firing rates.
 - `z_prior_n_hidden_layers`: int  
     - Default: `2`  
     - Only applied when `discrete_labels=False`  
 
-    Number of hidden layers in the MLP of the ZPriorContinuous module. 
+    Number of hidden layers in the MLP of the label prior estimator module. 
 - `z_prior_hidden_layer_dim`: int  
     - Default: `20`  
     - Only applied when `discrete_labels=False`
 
-    Dimensionality of each hidden layer in the MLP of the ZPriorContinuous module. 
+    Dimensionality of each hidden layer in the MLP of the label prior estimator module. 
 - `z_prior_hidden_layer_activation`: nn.Module  
     - Default: `nn.Tanh`  
     - Only applied when `discrete_labels=False`
 
-    Activation function applied to the outputs of each hidden layer in the MLP of the decoder's ZPriorContinuous module. 
+    Activation function applied to the outputs of each hidden layer in the MLP of the label prior estimator module. 
 
 ### Returns
 
-A dicitonary with the following items. 
+A `Dict` with the following items. 
 
 - `firing_rate`: Tensor   
     - Size([n_samples, x_dim])  
 
     Predicted firing rates of `z_sample`. 
 - `lambda_mean`: Tensor  
     - Size([n_samples, z_dim])  
@@ -181,14 +226,16 @@
 - `z_sample`: Tensor  
     - Size([n_samples, z_dim])  
     
     Generated latents `z`. 
 
 ## Loss Function
 
+pi-VAE learns the deep generative model and the approximate posterior q(z \| x, u) of the true posterior p(z \| x, u) by maximizing the evidence lower bound (ELBO) of p(x \| u).
+
 ### Poisson observation model
 
 ```
 from pi_vae_pytorch.utils import compute_loss
 
 outputs = model(x, u) # Initialized with decoder_observation_model="poisson" 
 
@@ -257,15 +304,15 @@
     - Should use the same value passed to `decoder_observation_model` when initializing `PiVAE`.  
 
     The observation model used by pi-VAE's decoder.
 - `observation_noise_model`: nn.Module 
     - Default: None  
     - Only applied when `observation model="gaussian"`  
     
-    The noise model used when pi-VAE's decoder utilizes a Gaussian observation model. When `PiVAE` is initialized with `decoder_observation_model="gaussian"`, the model's `observation_noise_model` attribute can be used.
+    The noise model used when pi-VAE's decoder utilizes a Gaussian observation model. When `PiVAE` is initialized with `decoder_observation_model="gaussian"`, the model's `observation_noise_model` attribute should be used.
 
 ## Citation
 
 ```
 @misc{zhou2020learning,
     title={Learning identifiable and interpretable latent models of high-dimensional neural activity using pi-VAE}, 
     author={Ding Zhou and Xue-Xin Wei},
```

### Comparing `pi-vae-pytorch-1.0.0b3/pyproject.toml` & `pi_vae_pytorch-1.0.0b4/pyproject.toml`

 * *Files identical despite different names*

