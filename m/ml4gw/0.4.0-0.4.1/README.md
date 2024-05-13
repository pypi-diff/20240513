# Comparing `tmp/ml4gw-0.4.0.tar.gz` & `tmp/ml4gw-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml4gw-0.4.0.tar", max compression
+gzip compressed data, was "ml4gw-0.4.1.tar", max compression
```

## Comparing `ml4gw-0.4.0.tar` & `ml4gw-0.4.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     5102 2024-02-20 16:03:02.673994 ml4gw-0.4.0/README.md
--rw-r--r--   0        0        0        0 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/__init__.py
--rw-r--r--   0        0        0     1027 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/augmentations.py
--rw-r--r--   0        0        0      149 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/dataloading/__init__.py
--rw-r--r--   0        0        0     5195 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/dataloading/chunked_dataset.py
--rw-r--r--   0        0        0     6643 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/dataloading/hdf5_dataset.py
--rw-r--r--   0        0        0     9801 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/dataloading/in_memory_dataset.py
--rw-r--r--   0        0        0     3428 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/distributions.py
--rw-r--r--   0        0        0    17914 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/gw.py
--rw-r--r--   0        0        0        0 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/__init__.py
--rw-r--r--   0        0        0      161 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/autoencoder/__init__.py
--rw-r--r--   0        0        0     3098 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/autoencoder/base.py
--rw-r--r--   0        0        0     5316 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/autoencoder/convolutional.py
--rw-r--r--   0        0        0     1304 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/autoencoder/skip_connection.py
--rw-r--r--   0        0        0      326 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/autoencoder/utils.py
--rw-r--r--   0        0        0     3250 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/norm.py
--rw-r--r--   0        0        0       64 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/resnet/__init__.py
--rw-r--r--   0        0        0    13218 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/resnet/resnet_1d.py
--rw-r--r--   0        0        0    13301 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/resnet/resnet_2d.py
--rw-r--r--   0        0        0       80 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/streaming/__init__.py
--rw-r--r--   0        0        0     4561 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/streaming/online_average.py
--rw-r--r--   0        0        0     4432 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/nn/streaming/snapshotter.py
--rw-r--r--   0        0        0    19021 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/spectral.py
--rw-r--r--   0        0        0      314 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/transforms/__init__.py
--rw-r--r--   0        0        0     3133 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/transforms/pearson.py
--rw-r--r--   0        0        0     2327 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/transforms/scaler.py
--rw-r--r--   0        0        0     2275 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/transforms/snr_rescaler.py
--rw-r--r--   0        0        0     3771 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/transforms/spectral.py
--rw-r--r--   0        0        0     6024 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/transforms/spectrogram.py
--rw-r--r--   0        0        0     2408 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/transforms/transform.py
--rw-r--r--   0        0        0     3060 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/transforms/waveforms.py
--rw-r--r--   0        0        0     9428 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/transforms/whitening.py
--rw-r--r--   0        0        0      429 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/types.py
--rw-r--r--   0        0        0     1519 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/utils/interferometer.py
--rw-r--r--   0        0        0    13535 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/utils/slicing.py
--rw-r--r--   0        0        0      104 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/waveforms/__init__.py
--rw-r--r--   0        0        0     1057 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/waveforms/generator.py
--rw-r--r--   0        0        0    38419 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/waveforms/phenom_d.py
--rw-r--r--   0        0        0    53447 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/waveforms/phenom_d_data.py
--rw-r--r--   0        0        0     3577 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/waveforms/sine_gaussian.py
--rw-r--r--   0        0        0     8482 2024-02-20 16:03:02.673994 ml4gw-0.4.0/ml4gw/waveforms/taylorf2.py
--rw-r--r--   0        0        0     1490 2024-02-20 16:03:02.677994 ml4gw-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5944 1970-01-01 00:00:00.000000 ml4gw-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     5102 2024-05-13 16:57:04.502735 ml4gw-0.4.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/__init__.py
+-rw-r--r--   0        0        0     1027 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/augmentations.py
+-rw-r--r--   0        0        0      149 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/dataloading/__init__.py
+-rw-r--r--   0        0        0     5195 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/dataloading/chunked_dataset.py
+-rw-r--r--   0        0        0     6643 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/dataloading/hdf5_dataset.py
+-rw-r--r--   0        0        0     9801 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/dataloading/in_memory_dataset.py
+-rw-r--r--   0        0        0     3428 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/distributions.py
+-rw-r--r--   0        0        0    17914 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/gw.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/__init__.py
+-rw-r--r--   0        0        0      161 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3098 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/autoencoder/base.py
+-rw-r--r--   0        0        0     5316 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/autoencoder/convolutional.py
+-rw-r--r--   0        0        0     1304 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/autoencoder/skip_connection.py
+-rw-r--r--   0        0        0      326 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/autoencoder/utils.py
+-rw-r--r--   0        0        0     3250 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/norm.py
+-rw-r--r--   0        0        0       64 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/resnet/__init__.py
+-rw-r--r--   0        0        0    13218 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/resnet/resnet_1d.py
+-rw-r--r--   0        0        0    13301 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/resnet/resnet_2d.py
+-rw-r--r--   0        0        0       80 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/streaming/__init__.py
+-rw-r--r--   0        0        0     4561 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/streaming/online_average.py
+-rw-r--r--   0        0        0     4432 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/nn/streaming/snapshotter.py
+-rw-r--r--   0        0        0    19021 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/spectral.py
+-rw-r--r--   0        0        0      314 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/transforms/__init__.py
+-rw-r--r--   0        0        0     3133 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/transforms/pearson.py
+-rw-r--r--   0        0        0     2327 2024-05-13 16:57:04.502735 ml4gw-0.4.1/ml4gw/transforms/scaler.py
+-rw-r--r--   0        0        0     2275 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/transforms/snr_rescaler.py
+-rw-r--r--   0        0        0     3771 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/transforms/spectral.py
+-rw-r--r--   0        0        0     6024 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/transforms/spectrogram.py
+-rw-r--r--   0        0        0     2408 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/transforms/transform.py
+-rw-r--r--   0        0        0     3060 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/transforms/waveforms.py
+-rw-r--r--   0        0        0     9428 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/transforms/whitening.py
+-rw-r--r--   0        0        0      429 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/types.py
+-rw-r--r--   0        0        0     1519 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/utils/interferometer.py
+-rw-r--r--   0        0        0    13535 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/utils/slicing.py
+-rw-r--r--   0        0        0      104 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/waveforms/__init__.py
+-rw-r--r--   0        0        0     1057 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/waveforms/generator.py
+-rw-r--r--   0        0        0    38419 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/waveforms/phenom_d.py
+-rw-r--r--   0        0        0    53447 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/waveforms/phenom_d_data.py
+-rw-r--r--   0        0        0     3577 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/waveforms/sine_gaussian.py
+-rw-r--r--   0        0        0     8482 2024-05-13 16:57:04.506735 ml4gw-0.4.1/ml4gw/waveforms/taylorf2.py
+-rw-r--r--   0        0        0     1314 2024-05-13 16:57:04.506735 ml4gw-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5706 1970-01-01 00:00:00.000000 ml4gw-0.4.1/PKG-INFO
```

### Comparing `ml4gw-0.4.0/README.md` & `ml4gw-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/augmentations.py` & `ml4gw-0.4.1/ml4gw/augmentations.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/dataloading/chunked_dataset.py` & `ml4gw-0.4.1/ml4gw/dataloading/chunked_dataset.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/dataloading/hdf5_dataset.py` & `ml4gw-0.4.1/ml4gw/dataloading/hdf5_dataset.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/dataloading/in_memory_dataset.py` & `ml4gw-0.4.1/ml4gw/dataloading/in_memory_dataset.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/distributions.py` & `ml4gw-0.4.1/ml4gw/distributions.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/gw.py` & `ml4gw-0.4.1/ml4gw/gw.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/nn/autoencoder/base.py` & `ml4gw-0.4.1/ml4gw/nn/autoencoder/base.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/nn/autoencoder/convolutional.py` & `ml4gw-0.4.1/ml4gw/nn/autoencoder/convolutional.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/nn/autoencoder/skip_connection.py` & `ml4gw-0.4.1/ml4gw/nn/autoencoder/skip_connection.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/nn/norm.py` & `ml4gw-0.4.1/ml4gw/nn/norm.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/nn/resnet/resnet_1d.py` & `ml4gw-0.4.1/ml4gw/nn/resnet/resnet_1d.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/nn/resnet/resnet_2d.py` & `ml4gw-0.4.1/ml4gw/nn/resnet/resnet_2d.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/nn/streaming/online_average.py` & `ml4gw-0.4.1/ml4gw/nn/streaming/online_average.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/nn/streaming/snapshotter.py` & `ml4gw-0.4.1/ml4gw/nn/streaming/snapshotter.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/spectral.py` & `ml4gw-0.4.1/ml4gw/spectral.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/transforms/pearson.py` & `ml4gw-0.4.1/ml4gw/transforms/pearson.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/transforms/scaler.py` & `ml4gw-0.4.1/ml4gw/transforms/scaler.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/transforms/snr_rescaler.py` & `ml4gw-0.4.1/ml4gw/transforms/snr_rescaler.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/transforms/spectral.py` & `ml4gw-0.4.1/ml4gw/transforms/spectral.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/transforms/spectrogram.py` & `ml4gw-0.4.1/ml4gw/transforms/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/transforms/transform.py` & `ml4gw-0.4.1/ml4gw/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/transforms/waveforms.py` & `ml4gw-0.4.1/ml4gw/transforms/waveforms.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/transforms/whitening.py` & `ml4gw-0.4.1/ml4gw/transforms/whitening.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/utils/interferometer.py` & `ml4gw-0.4.1/ml4gw/utils/interferometer.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/utils/slicing.py` & `ml4gw-0.4.1/ml4gw/utils/slicing.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/waveforms/generator.py` & `ml4gw-0.4.1/ml4gw/waveforms/generator.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/waveforms/phenom_d.py` & `ml4gw-0.4.1/ml4gw/waveforms/phenom_d.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/waveforms/phenom_d_data.py` & `ml4gw-0.4.1/ml4gw/waveforms/phenom_d_data.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/waveforms/sine_gaussian.py` & `ml4gw-0.4.1/ml4gw/waveforms/sine_gaussian.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/ml4gw/waveforms/taylorf2.py` & `ml4gw-0.4.1/ml4gw/waveforms/taylorf2.py`

 * *Files identical despite different names*

### Comparing `ml4gw-0.4.0/pyproject.toml` & `ml4gw-0.4.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,22 @@
 [tool.poetry]
 name = "ml4gw"
-version = "0.4.0"
+version = "0.4.1"
 description = "Tools for training torch models on gravitational wave data"
 readme = "README.md"
 authors = [
     "Alec Gunny <alec.gunny@ligo.org>", "Ethan Marx <emarx@mit.edu>", "Will Benoit <benoi090@umn.edu>", "Deep Chatterjee <deep1018@mit.edu"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 
 # torch deps
-torch = [
-    {version = "^1.10", python = ">=3.8,<3.11"},
-    {version = "^2.0", python = ">=3.11"}
-]
-torchaudio = [
-    {version = "^0.13", python = ">=3.8,<3.11"},
-    {version = "^2.0", python = ">=3.11"}
-]
+torch = "^2.0"
+torchaudio = "^2.0"
 torchtyping = "^0.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.16"
 pytest = "^7.0"
 
 # need lalsuite to compute gmst in injection testing
```

### Comparing `ml4gw-0.4.0/PKG-INFO` & `ml4gw-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: ml4gw
-Version: 0.4.0
+Version: 0.4.1
 Summary: Tools for training torch models on gravitational wave data
 Author: Alec Gunny
 Author-email: alec.gunny@ligo.org
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: torch (>=1.10,<2.0) ; python_version >= "3.8" and python_version < "3.11"
-Requires-Dist: torch (>=2.0,<3.0) ; python_version >= "3.11"
-Requires-Dist: torchaudio (>=0.13,<0.14) ; python_version >= "3.8" and python_version < "3.11"
-Requires-Dist: torchaudio (>=2.0,<3.0) ; python_version >= "3.11"
+Requires-Dist: torch (>=2.0,<3.0)
+Requires-Dist: torchaudio (>=2.0,<3.0)
 Requires-Dist: torchtyping (>=0.1,<0.2)
 Description-Content-Type: text/markdown
 
 # ML4GW
 
 Torch utilities for training neural networks in gravitational wave physics applications.
```

