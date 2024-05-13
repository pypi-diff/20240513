# Comparing `tmp/dyspyosis-0.0.1.tar.gz` & `tmp/dyspyosis-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyspyosis-0.0.1.tar", last modified: Thu Feb  8 08:22:24 2024, max compression
+gzip compressed data, was "dyspyosis-0.0.2.tar", last modified: Mon May 13 12:51:27 2024, max compression
```

## Comparing `dyspyosis-0.0.1.tar` & `dyspyosis-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-02-08 08:22:24.096137 dyspyosis-0.0.1/
--rw-rw-rw-   0        0        0    21286 2024-02-07 16:14:54.000000 dyspyosis-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     6334 2024-02-08 08:22:24.095525 dyspyosis-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     5708 2024-02-08 08:11:15.000000 dyspyosis-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-08 08:22:24.094523 dyspyosis-0.0.1/dyspyosis.egg-info/
--rw-rw-rw-   0        0        0     6334 2024-02-08 08:22:24.000000 dyspyosis-0.0.1/dyspyosis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-02-08 08:22:24.000000 dyspyosis-0.0.1/dyspyosis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-08 08:22:24.000000 dyspyosis-0.0.1/dyspyosis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-02-08 08:22:24.000000 dyspyosis-0.0.1/dyspyosis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-02-08 08:22:24.000000 dyspyosis-0.0.1/dyspyosis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-08 08:22:24.096137 dyspyosis-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1070 2024-02-07 16:14:54.000000 dyspyosis-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 12:51:27.324611 dyspyosis-0.0.2/
+-rw-rw-rw-   0        0        0    21286 2024-02-07 10:30:24.000000 dyspyosis-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5369 2024-05-13 12:51:27.322611 dyspyosis-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4603 2024-05-13 09:06:55.000000 dyspyosis-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-13 12:51:27.324611 dyspyosis-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2024-05-13 08:57:44.000000 dyspyosis-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 12:51:26.992635 dyspyosis-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 12:51:27.222610 dyspyosis-0.0.2/src/dyspyosis/
+-rw-rw-rw-   0        0        0       26 2024-05-13 08:57:44.000000 dyspyosis-0.0.2/src/dyspyosis/__init__.py
+-rw-rw-rw-   0        0        0     1904 2024-05-13 08:57:44.000000 dyspyosis-0.0.2/src/dyspyosis/autoencoder.py
+-rw-rw-rw-   0        0        0     4042 2024-05-13 08:57:44.000000 dyspyosis-0.0.2/src/dyspyosis/dyspyosis.py
+-rw-rw-rw-   0        0        0     3071 2024-05-13 08:57:44.000000 dyspyosis-0.0.2/src/dyspyosis/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-13 12:51:27.321611 dyspyosis-0.0.2/src/dyspyosis.egg-info/
+-rw-rw-rw-   0        0        0     5369 2024-05-13 12:51:26.000000 dyspyosis-0.0.2/src/dyspyosis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2024-05-13 12:51:26.000000 dyspyosis-0.0.2/src/dyspyosis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 12:51:26.000000 dyspyosis-0.0.2/src/dyspyosis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2024-05-13 12:51:26.000000 dyspyosis-0.0.2/src/dyspyosis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-13 12:51:26.000000 dyspyosis-0.0.2/src/dyspyosis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 12:51:27.319611 dyspyosis-0.0.2/tests/
+-rw-rw-rw-   0        0        0     2050 2024-05-13 09:10:50.000000 dyspyosis-0.0.2/tests/test_autoencoder.py
+-rw-rw-rw-   0        0        0     3005 2024-05-13 09:10:05.000000 dyspyosis-0.0.2/tests/test_dyspyosis.py
+-rw-rw-rw-   0        0        0     1686 2024-05-13 09:10:34.000000 dyspyosis-0.0.2/tests/test_utils.py
```

### Comparing `dyspyosis-0.0.1/LICENSE` & `dyspyosis-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dyspyosis-0.0.1/PKG-INFO` & `dyspyosis-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,51 @@
 Metadata-Version: 2.1
 Name: dyspyosis
-Version: 0.0.1
+Version: 0.0.2
 Summary: Calculate dysbiosis scores using Python
 Home-page: https://github.com/raeslab/dyspyosis/
 Author: Sebastian Proost
 Author-email: sebastian.proost@gmail.com
 License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0. https://creativecommons.org/licenses/by-nc-sa/4.0/
 Project-URL: Bug Tracker, https://github.com/raeslab/dyspyosis/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.26.3
+Requires-Dist: pandas>=2.1.4
+Requires-Dist: scikit-learn>=1.3.2
+Requires-Dist: tensorflow==2.10.1
+Requires-Dist: keras==2.10.0
 
 [![Run Pytest](https://github.com/raeslab/dyspyosis/actions/workflows/autopytest.yml/badge.svg)](https://github.com/raeslab/dyspyosis/actions/workflows/autopytest.yml) [![Coverage](https://raw.githubusercontent.com/raeslab/dyspyosis/main/docs/coverage-badge.svg)](https://raw.githubusercontent.com/raeslab/dyspyosis/main/docs/coverage-badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
 
 # Dyspyosis
 
 Python package that can be used to compute dysbiosis scores. The package leverages autoencoders based
 anomaly detection. Further details on this method are available [here](./docs/method.md).
 
-![A gumpy black snake, minimalist illustration](https://raw.githubusercontent.com/raeslab/dyspyosis/main/docs/img/dyspyosis_logo_small.jpg)
+![A gumpy black snake, minimalist illustration](./docs/img/dyspyosis_logo_small.jpg)
 
 ## Installation
 
-Before installing dyspyosis, ensure you have the CUDA toolkit v11.x and matching cuDNN installed, these are required for Tensorflow. Which version you need 
-depends on your hardware, e.g. for a GTX 10XX you'll need [CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)], for
-more recent cards you can get more recent versions.
-
-
-Next, install dyspyosis using the command below.
+Make sure you have [CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)] installed on your system (required for Tensorflow).
 
 ```commandline
 pip install dyspyosis
 ```
 
 ## Usage
 
 Below you can find an example how to use the dyspyosis package. Note that this is for testing purposes and parameters 
 have been set to complete the script quickly. For real data you'll want to increase the ```rarefication_count``` (the 
 number of times samples will be rarefied) to a large number (the number of samples x rarefication_count should be > 10k) 
 and increase the number of ```epochs``` to 4000.
 
-**Note**: Depending on your system, you might need to set an environmental variable ```CUDA_VISIBLE_DEVICES``` to "0" before
-loading dyspyosis to use the GPU. Try this in case CUDA is installed, but you get an error that no CUDA device was found.
-
-**Note**: The neural network dyspyosis is based on is relatively small, depending on the complexity of your dataset and 
-size of the latent space, running dyspyosis on CPU might outperform the GPU (see benchmarks)! To do so, set 
-```CUDA_VISIBLE_DEVICES``` to "-1" and ```CUDA_DEVICE_ORDER``` to "PCI_BUS_ID" in your environment before launching 
-dyspyosis.
-
 ```python
 import pandas as pd
 from dyspyosis import Dyspyosis
 
 if __name__ == "__main__":
     df = pd.read_table("./data/test.tsv", index_col=0)
 
@@ -73,29 +64,28 @@
 
 ## Benchmarks
 
 There are two benchmark scripts included in the repository: ```benchmark_cpu.py``` and ```benchmark_gpu.py```. When
 running the CPU benchmark it is important to set two environmental variables before running the code, ```CUDA_VISIBLE_DEVICES``` needs to be "-1"
 and ```CUDA_DEVICE_ORDER``` needs to be "PCI_BUS_ID". This ensures that the CPU benchmark actually runs on the CPU in case a GPU is available.
 
-Here are some results running dyspyosis on hardware we have access to.
+Here are some results running dyspyosis on hardware we have access too.
 
-| Type |                     Hardware | Epochs |       Time (s) |
-|-----:|-----------------------------:|-------:|---------------:|
-|  CPU |       Intel i5-7500 @ 3.4Ghz |    100 |       185.0017 |
-|  CPU |            AMD Ryzen 7 3700X |    100 |       115.1882 |
-|  GPU |  NVIDIA GeForce GTX 1060 6GB |    100 |       691.4091 |
-|  GPU | NVIDIA GeForce RTX 4080 16GB |    100 |       340.6128 |
+| Type |                    Hardware | Epochs | Time (s) |
+|-----:|----------------------------:|-------:|---------:|
+|  CPU |      Intel i5-7500 @ 3.4Ghz |    100 | 185.0017 |
+|  GPU | NVIDIA GeForce GTX 1060 6GB |    100 | 691.4091 |
 
 ## For developers
 
+To create the same environment the main devs are using, use [requirements.txt](./docs/dev/requirements.txt) to install
+the exact versions off all packages.
+
 Clone the repository, create a virtual environment and install all requirements first. Additionally, ensure you have
-the CUDA toolkit v11.x and matching cuDNN installed, these are required for Tensorflow. Which version you need 
-depends on your hardware, e.g. for a GTX 10XX you'll need [CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)], for
-more recent cards you can get more recent versions.
+[CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)] installed on your system (required for Tensorflow).
 
 ```commandline
 git clone https://github.com/raeslab/dyspyosis
 cd dyspyosis
 python -m venv venv
 source venv/activate
 pip install -r requirements.txt
@@ -104,23 +94,22 @@
 To run tests, use the command below. There are a number of Deprecation Warnings (due to tensorflow) that can be
 suppressed by ```--disable-warnings```.
 
 ```commandline
 pytest tests/ --disable-warnings --cov=dyspyosis --cov-report=term-missing --cov-report=xml
 ```
 
+[CUDA Toolkit 11.2]: https://developer.nvidia.com/cuda-11.2.0-download-archive
+[cuDNN (8.1.1)]: https://developer.nvidia.com/rdp/cudnn-archive
+
 ## Contributing
 
 Any contributions you make are **greatly appreciated**.
 
   * Found a bug or have some suggestions? Open an [issue](https://github.com/raeslab/dyspyosis/issues).
   * Pull requests are welcome! Though open an [issue](https://github.com/raeslab/dyspyosis/issues) first to discuss which features/changes you wish to implement.
 
 ## Contact and License
 
 dyspyosis was developed by [Sebastian Proost](https://sebastian.proost.science/) at the [RaesLab](https://raeslab.sites.vib.be/en) (part of [VIB](https://vib.be/en#/) and [KULeuven](https://www.kuleuven.be/english/kuleuven/index.html)). dyspyosis is available under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.
 
 For commercial access inquiries, please contact [Jeroen Raes](mailto:jeroen.raes@kuleuven.vib.be).
-
-[CUDA Toolkit 11.2]: https://developer.nvidia.com/cuda-11.2.0-download-archive
-[cuDNN (8.1.1)]: https://developer.nvidia.com/rdp/cudnn-archive
-
```

### Comparing `dyspyosis-0.0.1/README.md` & `dyspyosis-0.0.2/src/dyspyosis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,51 @@
+Metadata-Version: 2.1
+Name: dyspyosis
+Version: 0.0.2
+Summary: Calculate dysbiosis scores using Python
+Home-page: https://github.com/raeslab/dyspyosis/
+Author: Sebastian Proost
+Author-email: sebastian.proost@gmail.com
+License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0. https://creativecommons.org/licenses/by-nc-sa/4.0/
+Project-URL: Bug Tracker, https://github.com/raeslab/dyspyosis/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.26.3
+Requires-Dist: pandas>=2.1.4
+Requires-Dist: scikit-learn>=1.3.2
+Requires-Dist: tensorflow==2.10.1
+Requires-Dist: keras==2.10.0
+
 [![Run Pytest](https://github.com/raeslab/dyspyosis/actions/workflows/autopytest.yml/badge.svg)](https://github.com/raeslab/dyspyosis/actions/workflows/autopytest.yml) [![Coverage](https://raw.githubusercontent.com/raeslab/dyspyosis/main/docs/coverage-badge.svg)](https://raw.githubusercontent.com/raeslab/dyspyosis/main/docs/coverage-badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
 
 # Dyspyosis
 
 Python package that can be used to compute dysbiosis scores. The package leverages autoencoders based
 anomaly detection. Further details on this method are available [here](./docs/method.md).
 
-![A gumpy black snake, minimalist illustration](https://raw.githubusercontent.com/raeslab/dyspyosis/main/docs/img/dyspyosis_logo_small.jpg)
+![A gumpy black snake, minimalist illustration](./docs/img/dyspyosis_logo_small.jpg)
 
 ## Installation
 
-Before installing dyspyosis, ensure you have the CUDA toolkit v11.x and matching cuDNN installed, these are required for Tensorflow. Which version you need 
-depends on your hardware, e.g. for a GTX 10XX you'll need [CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)], for
-more recent cards you can get more recent versions.
-
-
-Next, install dyspyosis using the command below.
+Make sure you have [CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)] installed on your system (required for Tensorflow).
 
 ```commandline
 pip install dyspyosis
 ```
 
 ## Usage
 
 Below you can find an example how to use the dyspyosis package. Note that this is for testing purposes and parameters 
 have been set to complete the script quickly. For real data you'll want to increase the ```rarefication_count``` (the 
 number of times samples will be rarefied) to a large number (the number of samples x rarefication_count should be > 10k) 
 and increase the number of ```epochs``` to 4000.
 
-**Note**: Depending on your system, you might need to set an environmental variable ```CUDA_VISIBLE_DEVICES``` to "0" before
-loading dyspyosis to use the GPU. Try this in case CUDA is installed, but you get an error that no CUDA device was found.
-
-**Note**: The neural network dyspyosis is based on is relatively small, depending on the complexity of your dataset and 
-size of the latent space, running dyspyosis on CPU might outperform the GPU (see benchmarks)! To do so, set 
-```CUDA_VISIBLE_DEVICES``` to "-1" and ```CUDA_DEVICE_ORDER``` to "PCI_BUS_ID" in your environment before launching 
-dyspyosis.
-
 ```python
 import pandas as pd
 from dyspyosis import Dyspyosis
 
 if __name__ == "__main__":
     df = pd.read_table("./data/test.tsv", index_col=0)
 
@@ -57,29 +64,28 @@
 
 ## Benchmarks
 
 There are two benchmark scripts included in the repository: ```benchmark_cpu.py``` and ```benchmark_gpu.py```. When
 running the CPU benchmark it is important to set two environmental variables before running the code, ```CUDA_VISIBLE_DEVICES``` needs to be "-1"
 and ```CUDA_DEVICE_ORDER``` needs to be "PCI_BUS_ID". This ensures that the CPU benchmark actually runs on the CPU in case a GPU is available.
 
-Here are some results running dyspyosis on hardware we have access to.
+Here are some results running dyspyosis on hardware we have access too.
 
-| Type |                     Hardware | Epochs |       Time (s) |
-|-----:|-----------------------------:|-------:|---------------:|
-|  CPU |       Intel i5-7500 @ 3.4Ghz |    100 |       185.0017 |
-|  CPU |            AMD Ryzen 7 3700X |    100 |       115.1882 |
-|  GPU |  NVIDIA GeForce GTX 1060 6GB |    100 |       691.4091 |
-|  GPU | NVIDIA GeForce RTX 4080 16GB |    100 |       340.6128 |
+| Type |                    Hardware | Epochs | Time (s) |
+|-----:|----------------------------:|-------:|---------:|
+|  CPU |      Intel i5-7500 @ 3.4Ghz |    100 | 185.0017 |
+|  GPU | NVIDIA GeForce GTX 1060 6GB |    100 | 691.4091 |
 
 ## For developers
 
+To create the same environment the main devs are using, use [requirements.txt](./docs/dev/requirements.txt) to install
+the exact versions off all packages.
+
 Clone the repository, create a virtual environment and install all requirements first. Additionally, ensure you have
-the CUDA toolkit v11.x and matching cuDNN installed, these are required for Tensorflow. Which version you need 
-depends on your hardware, e.g. for a GTX 10XX you'll need [CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)], for
-more recent cards you can get more recent versions.
+[CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)] installed on your system (required for Tensorflow).
 
 ```commandline
 git clone https://github.com/raeslab/dyspyosis
 cd dyspyosis
 python -m venv venv
 source venv/activate
 pip install -r requirements.txt
@@ -88,22 +94,22 @@
 To run tests, use the command below. There are a number of Deprecation Warnings (due to tensorflow) that can be
 suppressed by ```--disable-warnings```.
 
 ```commandline
 pytest tests/ --disable-warnings --cov=dyspyosis --cov-report=term-missing --cov-report=xml
 ```
 
+[CUDA Toolkit 11.2]: https://developer.nvidia.com/cuda-11.2.0-download-archive
+[cuDNN (8.1.1)]: https://developer.nvidia.com/rdp/cudnn-archive
+
 ## Contributing
 
 Any contributions you make are **greatly appreciated**.
 
   * Found a bug or have some suggestions? Open an [issue](https://github.com/raeslab/dyspyosis/issues).
   * Pull requests are welcome! Though open an [issue](https://github.com/raeslab/dyspyosis/issues) first to discuss which features/changes you wish to implement.
 
 ## Contact and License
 
 dyspyosis was developed by [Sebastian Proost](https://sebastian.proost.science/) at the [RaesLab](https://raeslab.sites.vib.be/en) (part of [VIB](https://vib.be/en#/) and [KULeuven](https://www.kuleuven.be/english/kuleuven/index.html)). dyspyosis is available under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.
 
 For commercial access inquiries, please contact [Jeroen Raes](mailto:jeroen.raes@kuleuven.vib.be).
-
-[CUDA Toolkit 11.2]: https://developer.nvidia.com/cuda-11.2.0-download-archive
-[cuDNN (8.1.1)]: https://developer.nvidia.com/rdp/cudnn-archive
```

### Comparing `dyspyosis-0.0.1/dyspyosis.egg-info/PKG-INFO` & `dyspyosis-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,31 @@
-Metadata-Version: 2.1
-Name: dyspyosis
-Version: 0.0.1
-Summary: Calculate dysbiosis scores using Python
-Home-page: https://github.com/raeslab/dyspyosis/
-Author: Sebastian Proost
-Author-email: sebastian.proost@gmail.com
-License: Creative Commons Attribution-NonCommercial-ShareAlike 4.0. https://creativecommons.org/licenses/by-nc-sa/4.0/
-Project-URL: Bug Tracker, https://github.com/raeslab/dyspyosis/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Run Pytest](https://github.com/raeslab/dyspyosis/actions/workflows/autopytest.yml/badge.svg)](https://github.com/raeslab/dyspyosis/actions/workflows/autopytest.yml) [![Coverage](https://raw.githubusercontent.com/raeslab/dyspyosis/main/docs/coverage-badge.svg)](https://raw.githubusercontent.com/raeslab/dyspyosis/main/docs/coverage-badge.svg) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by-nc-sa/4.0/)
 
 # Dyspyosis
 
 Python package that can be used to compute dysbiosis scores. The package leverages autoencoders based
 anomaly detection. Further details on this method are available [here](./docs/method.md).
 
-![A gumpy black snake, minimalist illustration](https://raw.githubusercontent.com/raeslab/dyspyosis/main/docs/img/dyspyosis_logo_small.jpg)
+![A gumpy black snake, minimalist illustration](./docs/img/dyspyosis_logo_small.jpg)
 
 ## Installation
 
-Before installing dyspyosis, ensure you have the CUDA toolkit v11.x and matching cuDNN installed, these are required for Tensorflow. Which version you need 
-depends on your hardware, e.g. for a GTX 10XX you'll need [CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)], for
-more recent cards you can get more recent versions.
-
-
-Next, install dyspyosis using the command below.
+Make sure you have [CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)] installed on your system (required for Tensorflow).
 
 ```commandline
 pip install dyspyosis
 ```
 
 ## Usage
 
 Below you can find an example how to use the dyspyosis package. Note that this is for testing purposes and parameters 
 have been set to complete the script quickly. For real data you'll want to increase the ```rarefication_count``` (the 
 number of times samples will be rarefied) to a large number (the number of samples x rarefication_count should be > 10k) 
 and increase the number of ```epochs``` to 4000.
 
-**Note**: Depending on your system, you might need to set an environmental variable ```CUDA_VISIBLE_DEVICES``` to "0" before
-loading dyspyosis to use the GPU. Try this in case CUDA is installed, but you get an error that no CUDA device was found.
-
-**Note**: The neural network dyspyosis is based on is relatively small, depending on the complexity of your dataset and 
-size of the latent space, running dyspyosis on CPU might outperform the GPU (see benchmarks)! To do so, set 
-```CUDA_VISIBLE_DEVICES``` to "-1" and ```CUDA_DEVICE_ORDER``` to "PCI_BUS_ID" in your environment before launching 
-dyspyosis.
-
 ```python
 import pandas as pd
 from dyspyosis import Dyspyosis
 
 if __name__ == "__main__":
     df = pd.read_table("./data/test.tsv", index_col=0)
 
@@ -73,29 +44,28 @@
 
 ## Benchmarks
 
 There are two benchmark scripts included in the repository: ```benchmark_cpu.py``` and ```benchmark_gpu.py```. When
 running the CPU benchmark it is important to set two environmental variables before running the code, ```CUDA_VISIBLE_DEVICES``` needs to be "-1"
 and ```CUDA_DEVICE_ORDER``` needs to be "PCI_BUS_ID". This ensures that the CPU benchmark actually runs on the CPU in case a GPU is available.
 
-Here are some results running dyspyosis on hardware we have access to.
+Here are some results running dyspyosis on hardware we have access too.
 
-| Type |                     Hardware | Epochs |       Time (s) |
-|-----:|-----------------------------:|-------:|---------------:|
-|  CPU |       Intel i5-7500 @ 3.4Ghz |    100 |       185.0017 |
-|  CPU |            AMD Ryzen 7 3700X |    100 |       115.1882 |
-|  GPU |  NVIDIA GeForce GTX 1060 6GB |    100 |       691.4091 |
-|  GPU | NVIDIA GeForce RTX 4080 16GB |    100 |       340.6128 |
+| Type |                    Hardware | Epochs | Time (s) |
+|-----:|----------------------------:|-------:|---------:|
+|  CPU |      Intel i5-7500 @ 3.4Ghz |    100 | 185.0017 |
+|  GPU | NVIDIA GeForce GTX 1060 6GB |    100 | 691.4091 |
 
 ## For developers
 
+To create the same environment the main devs are using, use [requirements.txt](./docs/dev/requirements.txt) to install
+the exact versions off all packages.
+
 Clone the repository, create a virtual environment and install all requirements first. Additionally, ensure you have
-the CUDA toolkit v11.x and matching cuDNN installed, these are required for Tensorflow. Which version you need 
-depends on your hardware, e.g. for a GTX 10XX you'll need [CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)], for
-more recent cards you can get more recent versions.
+[CUDA Toolkit 11.2] and the matching [cuDNN (8.1.1)] installed on your system (required for Tensorflow).
 
 ```commandline
 git clone https://github.com/raeslab/dyspyosis
 cd dyspyosis
 python -m venv venv
 source venv/activate
 pip install -r requirements.txt
@@ -104,23 +74,22 @@
 To run tests, use the command below. There are a number of Deprecation Warnings (due to tensorflow) that can be
 suppressed by ```--disable-warnings```.
 
 ```commandline
 pytest tests/ --disable-warnings --cov=dyspyosis --cov-report=term-missing --cov-report=xml
 ```
 
+[CUDA Toolkit 11.2]: https://developer.nvidia.com/cuda-11.2.0-download-archive
+[cuDNN (8.1.1)]: https://developer.nvidia.com/rdp/cudnn-archive
+
 ## Contributing
 
 Any contributions you make are **greatly appreciated**.
 
   * Found a bug or have some suggestions? Open an [issue](https://github.com/raeslab/dyspyosis/issues).
   * Pull requests are welcome! Though open an [issue](https://github.com/raeslab/dyspyosis/issues) first to discuss which features/changes you wish to implement.
 
 ## Contact and License
 
 dyspyosis was developed by [Sebastian Proost](https://sebastian.proost.science/) at the [RaesLab](https://raeslab.sites.vib.be/en) (part of [VIB](https://vib.be/en#/) and [KULeuven](https://www.kuleuven.be/english/kuleuven/index.html)). dyspyosis is available under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International](https://creativecommons.org/licenses/by-nc-sa/4.0/) license.
 
-For commercial access inquiries, please contact [Jeroen Raes](mailto:jeroen.raes@kuleuven.vib.be).
-
-[CUDA Toolkit 11.2]: https://developer.nvidia.com/cuda-11.2.0-download-archive
-[cuDNN (8.1.1)]: https://developer.nvidia.com/rdp/cudnn-archive
-
+For commercial access inquiries, please contact [Jeroen Raes](mailto:jeroen.raes@kuleuven.vib.be).
```

### Comparing `dyspyosis-0.0.1/setup.py` & `dyspyosis-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import setuptools
+from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
-setuptools.setup(
+setup(
     name="dyspyosis",
-    version="0.0.1",
+    version="0.0.2",
     author="Sebastian Proost",
     author_email="sebastian.proost@gmail.com",
     description="Calculate dysbiosis scores using Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raeslab/dyspyosis/",
     project_urls={
@@ -23,10 +23,11 @@
         "keras==2.10.0",
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     license="Creative Commons Attribution-NonCommercial-ShareAlike 4.0. https://creativecommons.org/licenses/by-nc-sa/4.0/",
-    packages=setuptools.find_packages(where="dyspyosis"),
+    packages=find_packages("src"),
+    package_dir={"": "src"},
     python_requires=">=3.10",
 )
```

