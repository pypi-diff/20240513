# Comparing `tmp/spcm-1.1.1.tar.gz` & `tmp/spcm-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spcm-1.1.1.tar", last modified: Fri Apr 12 11:35:26 2024, max compression
+gzip compressed data, was "spcm-1.1.2.tar", last modified: Mon May 13 09:00:40 2024, max compression
```

## Comparing `spcm-1.1.1.tar` & `spcm-1.1.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:35:26.040840 spcm-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-12 11:35:20.000000 spcm-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-12 11:35:20.000000 spcm-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21586 2024-04-12 11:35:26.040840 spcm-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-04-12 11:35:20.000000 spcm-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-12 11:35:20.000000 spcm-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:35:26.040840 spcm-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-12 11:35:20.000000 spcm-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:35:26.032840 spcm-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:35:26.036840 spcm-1.1.1/src/spcm/
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-12 11:35:26.040840 spcm-1.1.1/src/spcm/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_block_average.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_boxcar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_card_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    28176 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_channels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)    28626 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (127)    43006 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_dds.py
--rw-r--r--   0 runner    (1001) docker     (127)    18266 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_error_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_functionality.py
--rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_multi_purpose_ios.py
--rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_netbox.py
--rw-r--r--   0 runner    (1001) docker     (127)    25635 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_pulse_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_sequence.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_time_stamp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/classes_unit_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    13302 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/pyspcm.py
--rw-r--r--   0 runner    (1001) docker     (127)    89313 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/regs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-04-12 11:35:20.000000 spcm-1.1.1/src/spcm/spcerr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 11:35:26.040840 spcm-1.1.1/src/spcm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21586 2024-04-12 11:35:26.000000 spcm-1.1.1/src/spcm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-12 11:35:26.000000 spcm-1.1.1/src/spcm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 11:35:26.000000 spcm-1.1.1/src/spcm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 11:35:26.000000 spcm-1.1.1/src/spcm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-12 11:35:26.000000 spcm-1.1.1/src/spcm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-12 11:35:20.000000 spcm-1.1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:00:40.476438 spcm-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-13 09:00:34.000000 spcm-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 09:00:34.000000 spcm-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-05-13 09:00:40.476438 spcm-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20296 2024-05-13 09:00:34.000000 spcm-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-13 09:00:34.000000 spcm-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:00:40.476438 spcm-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 09:00:34.000000 spcm-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:00:40.468438 spcm-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:00:40.476438 spcm-1.1.2/src/spcm/
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-13 09:00:40.476438 spcm-1.1.2/src/spcm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_block_average.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_boxcar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9985 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7966 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_card_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28176 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_channels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28626 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43006 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_dds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18266 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_error_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6354 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_multi_purpose_ios.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_netbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25635 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_pulse_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_time_stamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15868 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/classes_unit_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13302 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/pyspcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89313 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/regs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-13 09:00:34.000000 spcm-1.1.2/src/spcm/spcerr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 09:00:40.476438 spcm-1.1.2/src/spcm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21691 2024-05-13 09:00:40.000000 spcm-1.1.2/src/spcm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-13 09:00:40.000000 spcm-1.1.2/src/spcm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 09:00:40.000000 spcm-1.1.2/src/spcm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 09:00:40.000000 spcm-1.1.2/src/spcm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-13 09:00:40.000000 spcm-1.1.2/src/spcm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-05-13 09:00:34.000000 spcm-1.1.2/versioneer.py
```

### Comparing `spcm-1.1.1/LICENSE` & `spcm-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/PKG-INFO` & `spcm-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spcm
-Version: 1.1.1
+Version: 1.1.2
 Summary: Package for Spectrum Instrumentation GmbH cards
 Author-email: Spectrum Instrumentation GmbH <info@spec.de>
 Project-URL: Homepage, https://spectrum-instrumentation.com/
 Project-URL: API, https://spectruminstrumentation.github.io/spcm/spcm.html
 Project-URL: Repository, https://github.com/SpectrumInstrumentation/spcm
 Project-URL: Examples, https://github.com/SpectrumInstrumentation/spcm/tree/master/src/examples
 Project-URL: Knowledge Base, https://spectrum-instrumentation.com/support/knowledgebase/index.php
@@ -48,16 +48,17 @@
 
 # Supported devices
 
 See the [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices.
 
 # Requirements
 [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)](https://badge.fury.io/py/spcm)
-[![Static Badge](https://img.shields.io/badge/NumPy-1.25-green)](https://numpy.org/)
-[![Static Badge](https://img.shields.io/badge/h5py-3.10-orange)](https://www.h5py.org/)
+[![Static Badge](https://img.shields.io/badge/NumPy-1.25+-green)](https://numpy.org/)
+[![Static Badge](https://img.shields.io/badge/h5py-3.10+-orange)](https://www.h5py.org/)
+[![Static Badge](https://img.shields.io/badge/pint-0.23+-teal)](https://pint.readthedocs.io/en/stable/)
 
 `spcm` requires the Spectrum Instrumentation [driver](https://spectrum-instrumentation.com/support/downloads.php) which is available for Windows and Linux. 
 Please have a look in the manual of your product for more information about installing the driver on the different plattforms.
 
 # Installation and dependencies
 [![Pip Package](https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
 [![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml)
@@ -172,15 +173,15 @@
 
 `spcm` uses [pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that have a physical unit. To enable the use of qunatities simply import the units module from `spcm`:
 
 ```python
 from spcm import units
 ```
 
-This import the `units` object from `spcm`. which is a `UnitRegistry` object from  `pint`. Defining a quantity is as simples as:
+This imports the `units` object from `spcm`. which is a `UnitRegistry` object from `pint`. Defining a quantity is as simple as:
 
 ```python
 from spcm import units
 
 frequency = 100 * units.MHz
 amplitude = 1 * units.V
 # etc...
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spcm Version: 1.1.1 Summary: Package for Spectrum
+Metadata-Version: 2.1 Name: spcm Version: 1.1.2 Summary: Package for Spectrum
 Instrumentation GmbH cards Author-email: Spectrum Instrumentation GmbH
 spec.de> Project-URL: Homepage, https://spectrum-instrumentation.com/ Project-
 URL: API, https://spectruminstrumentation.github.io/spcm/spcm.html Project-URL:
 Repository, https://github.com/SpectrumInstrumentation/spcm Project-URL:
 Examples, https://github.com/SpectrumInstrumentation/spcm/tree/master/src/
 examples Project-URL: Knowledge Base, https://spectrum-instrumentation.com/
 support/knowledgebase/index.php Classifier: Development Status :: 4 - Beta
@@ -30,22 +30,24 @@
 oriented Python package for interfacing with Spectrum Instrumentation GmbH
 devices. `spcm` can handle individual cards (`Card`), StarHubs (`Sync`), groups
 of cards (`CardStack`) and Netboxes (`Netbox`). # Supported devices See the
 [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/
 master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices. #
 Requirements [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)]
 (https://badge.fury.io/py/spcm) [![Static Badge](https://img.shields.io/badge/
-NumPy-1.25-green)](https://numpy.org/) [![Static Badge](https://img.shields.io/
-badge/h5py-3.10-orange)](https://www.h5py.org/) `spcm` requires the Spectrum
-Instrumentation [driver](https://spectrum-instrumentation.com/support/
-downloads.php) which is available for Windows and Linux. Please have a look in
-the manual of your product for more information about installing the driver on
-the different plattforms. # Installation and dependencies [![Pip Package]
-(https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
-[![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/
+NumPy-1.25+-green)](https://numpy.org/) [![Static Badge](https://
+img.shields.io/badge/h5py-3.10+-orange)](https://www.h5py.org/) [![Static
+Badge](https://img.shields.io/badge/pint-0.23+-teal)](https://
+pint.readthedocs.io/en/stable/) `spcm` requires the Spectrum Instrumentation
+[driver](https://spectrum-instrumentation.com/support/downloads.php) which is
+available for Windows and Linux. Please have a look in the manual of your
+product for more information about installing the driver on the different
+plattforms. # Installation and dependencies [![Pip Package](https://
+img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm) [!
+[Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/
 workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/
 SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml) Start
 by installing Python 3.9 or higher. We recommend using the latest version. You
 can download Python from [https://www.python.org/](https://www.python.org/).
 You would probably also like to install and use a virtual environment, although
 it's not strictly necessary. See the examples [README.md](https://github.com/
 SpectrumInstrumentation/spcm/blob/master/src/examples/README.md) for a more
@@ -108,46 +110,46 @@
 Center gives the user the option to create [demo devices](https://spectrum-
 instrumentation.com/support/knowledgebase/software/
 How_to_set_up_a_demo_card.php). These demo devices can be used in the same
 manner as real devices. Simply change the device identifier string to the
 string as shown in the Control Center. ## Units and quantities `spcm` uses
 [pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that
 have a physical unit. To enable the use of qunatities simply import the units
-module from `spcm`: ```python from spcm import units ``` This import the
+module from `spcm`: ```python from spcm import units ``` This imports the
 `units` object from `spcm`. which is a `UnitRegistry` object from `pint`.
-Defining a quantity is as simples as: ```python from spcm import units
-frequency = 100 * units.MHz amplitude = 1 * units.V # etc... ``` All methods
-within the `spcm` that expect a value that is related to a physical quantity
-support the quantities, for example setting a timeout: ```python card.timeout(5
-* units.s) ``` See our dedicated examples for more information about where
-units can be used. ## Card Functionality After opening a card, StarHub or group
-of card, specific functionality of the cards can be accessed through
-`CardFunctionality` classes. | Name | Description | |---------------------|----
------------------------------------------------------------------| | `Channels`
-| class for setting up the in- or output stage of the channels of a card | |
-`Clock` | class for setting up the clock engine of the card | | `Trigger` |
-class for setting up the trigger engine of the card | | `MultiPurposeIOs` |
-class for setting up the multi purpose i/o of the card | | `DataTransfer` |
-class for handling data transfer functionality | | `Multi` | class for handling
-multiple recording and replay mode functionality | | `Sequence` | class for
-handling sequence mode functionality | | `TimeStamp` | class for handling time
-stamped data | | `Boxcar` | class for handling boxcar averaging | |
-`BlockAverage` | class for handling block averaging functionality | |
-`PulseGenerators` | class for setting up the pulse generator functionality | |
-`DDS` | class for handling DDS functionality | To use a specific functionality
-simply initiate an instance of one of the classes and pass a device object:
-```python import spcm with spcm.Card('/dev/spcm0') as card: clock = spcm.Clock
-(card) # (or) trigger = spcm.Trigger(card) # (or) multi_io =
-spcm.MultiPurposeIOs(card) # (or) data_transfer = spcm.DataTransfer(card) # etc
-... ``` Each of these functionalities typically corresponds to a chapter in
-your device manual, so for further reference please have a look in the device
-manual. ## Setting up Channels The Channels functionality allows the user to
-setup individual channels on a Card or a CardStack. The channels object is also
-a Python iterator, hence if a channels object is used it a for-loop, each
-iteration provides a Channel object: ```python channels = spcm.Channels(card,
+Defining a quantity is as simple as: ```python from spcm import units frequency
+= 100 * units.MHz amplitude = 1 * units.V # etc... ``` All methods within the
+`spcm` that expect a value that is related to a physical quantity support the
+quantities, for example setting a timeout: ```python card.timeout(5 * units.s)
+``` See our dedicated examples for more information about where units can be
+used. ## Card Functionality After opening a card, StarHub or group of card,
+specific functionality of the cards can be accessed through `CardFunctionality`
+classes. | Name | Description | |---------------------|------------------------
+---------------------------------------------| | `Channels` | class for setting
+up the in- or output stage of the channels of a card | | `Clock` | class for
+setting up the clock engine of the card | | `Trigger` | class for setting up
+the trigger engine of the card | | `MultiPurposeIOs` | class for setting up the
+multi purpose i/o of the card | | `DataTransfer` | class for handling data
+transfer functionality | | `Multi` | class for handling multiple recording and
+replay mode functionality | | `Sequence` | class for handling sequence mode
+functionality | | `TimeStamp` | class for handling time stamped data | |
+`Boxcar` | class for handling boxcar averaging | | `BlockAverage` | class for
+handling block averaging functionality | | `PulseGenerators` | class for
+setting up the pulse generator functionality | | `DDS` | class for handling DDS
+functionality | To use a specific functionality simply initiate an instance of
+one of the classes and pass a device object: ```python import spcm with
+spcm.Card('/dev/spcm0') as card: clock = spcm.Clock(card) # (or) trigger =
+spcm.Trigger(card) # (or) multi_io = spcm.MultiPurposeIOs(card) # (or)
+data_transfer = spcm.DataTransfer(card) # etc ... ``` Each of these
+functionalities typically corresponds to a chapter in your device manual, so
+for further reference please have a look in the device manual. ## Setting up
+Channels The Channels functionality allows the user to setup individual
+channels on a Card or a CardStack. The channels object is also a Python
+iterator, hence if a channels object is used it a for-loop, each iteration
+provides a Channel object: ```python channels = spcm.Channels(card,
 card_enable=spcm.CHANNEL0 | CHANNEL1) for channel in channels: # do something
 with each channel ``` In addition, the user can define the output load
 connected to the channel (standard value 50 Ohm), to any resistor value or high
 impedance (`units.highZ`). With this output load, the amplitude setting can be
 done with the repect to this output load: ```python channels = Channels(card,
 card_enable=spcm.CHANNEL0 | CHANNEL1) channels[0].output_load(units.highZ)
 channels[0].amp(1 * units.V) # or for all channels channels.output_load
```

### Comparing `spcm-1.1.1/README.md` & `spcm-1.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 # Supported devices
 
 See the [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices.
 
 # Requirements
 [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)](https://badge.fury.io/py/spcm)
-[![Static Badge](https://img.shields.io/badge/NumPy-1.25-green)](https://numpy.org/)
-[![Static Badge](https://img.shields.io/badge/h5py-3.10-orange)](https://www.h5py.org/)
+[![Static Badge](https://img.shields.io/badge/NumPy-1.25+-green)](https://numpy.org/)
+[![Static Badge](https://img.shields.io/badge/h5py-3.10+-orange)](https://www.h5py.org/)
+[![Static Badge](https://img.shields.io/badge/pint-0.23+-teal)](https://pint.readthedocs.io/en/stable/)
 
 `spcm` requires the Spectrum Instrumentation [driver](https://spectrum-instrumentation.com/support/downloads.php) which is available for Windows and Linux. 
 Please have a look in the manual of your product for more information about installing the driver on the different plattforms.
 
 # Installation and dependencies
 [![Pip Package](https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
 [![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml)
@@ -141,15 +142,15 @@
 
 `spcm` uses [pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that have a physical unit. To enable the use of qunatities simply import the units module from `spcm`:
 
 ```python
 from spcm import units
 ```
 
-This import the `units` object from `spcm`. which is a `UnitRegistry` object from  `pint`. Defining a quantity is as simples as:
+This imports the `units` object from `spcm`. which is a `UnitRegistry` object from `pint`. Defining a quantity is as simple as:
 
 ```python
 from spcm import units
 
 frequency = 100 * units.MHz
 amplitude = 1 * units.V
 # etc...
```

#### html2text {}

```diff
@@ -11,22 +11,24 @@
 oriented Python package for interfacing with Spectrum Instrumentation GmbH
 devices. `spcm` can handle individual cards (`Card`), StarHubs (`Sync`), groups
 of cards (`CardStack`) and Netboxes (`Netbox`). # Supported devices See the
 [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/
 master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices. #
 Requirements [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)]
 (https://badge.fury.io/py/spcm) [![Static Badge](https://img.shields.io/badge/
-NumPy-1.25-green)](https://numpy.org/) [![Static Badge](https://img.shields.io/
-badge/h5py-3.10-orange)](https://www.h5py.org/) `spcm` requires the Spectrum
-Instrumentation [driver](https://spectrum-instrumentation.com/support/
-downloads.php) which is available for Windows and Linux. Please have a look in
-the manual of your product for more information about installing the driver on
-the different plattforms. # Installation and dependencies [![Pip Package]
-(https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
-[![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/
+NumPy-1.25+-green)](https://numpy.org/) [![Static Badge](https://
+img.shields.io/badge/h5py-3.10+-orange)](https://www.h5py.org/) [![Static
+Badge](https://img.shields.io/badge/pint-0.23+-teal)](https://
+pint.readthedocs.io/en/stable/) `spcm` requires the Spectrum Instrumentation
+[driver](https://spectrum-instrumentation.com/support/downloads.php) which is
+available for Windows and Linux. Please have a look in the manual of your
+product for more information about installing the driver on the different
+plattforms. # Installation and dependencies [![Pip Package](https://
+img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm) [!
+[Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/
 workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/
 SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml) Start
 by installing Python 3.9 or higher. We recommend using the latest version. You
 can download Python from [https://www.python.org/](https://www.python.org/).
 You would probably also like to install and use a virtual environment, although
 it's not strictly necessary. See the examples [README.md](https://github.com/
 SpectrumInstrumentation/spcm/blob/master/src/examples/README.md) for a more
@@ -89,46 +91,46 @@
 Center gives the user the option to create [demo devices](https://spectrum-
 instrumentation.com/support/knowledgebase/software/
 How_to_set_up_a_demo_card.php). These demo devices can be used in the same
 manner as real devices. Simply change the device identifier string to the
 string as shown in the Control Center. ## Units and quantities `spcm` uses
 [pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that
 have a physical unit. To enable the use of qunatities simply import the units
-module from `spcm`: ```python from spcm import units ``` This import the
+module from `spcm`: ```python from spcm import units ``` This imports the
 `units` object from `spcm`. which is a `UnitRegistry` object from `pint`.
-Defining a quantity is as simples as: ```python from spcm import units
-frequency = 100 * units.MHz amplitude = 1 * units.V # etc... ``` All methods
-within the `spcm` that expect a value that is related to a physical quantity
-support the quantities, for example setting a timeout: ```python card.timeout(5
-* units.s) ``` See our dedicated examples for more information about where
-units can be used. ## Card Functionality After opening a card, StarHub or group
-of card, specific functionality of the cards can be accessed through
-`CardFunctionality` classes. | Name | Description | |---------------------|----
------------------------------------------------------------------| | `Channels`
-| class for setting up the in- or output stage of the channels of a card | |
-`Clock` | class for setting up the clock engine of the card | | `Trigger` |
-class for setting up the trigger engine of the card | | `MultiPurposeIOs` |
-class for setting up the multi purpose i/o of the card | | `DataTransfer` |
-class for handling data transfer functionality | | `Multi` | class for handling
-multiple recording and replay mode functionality | | `Sequence` | class for
-handling sequence mode functionality | | `TimeStamp` | class for handling time
-stamped data | | `Boxcar` | class for handling boxcar averaging | |
-`BlockAverage` | class for handling block averaging functionality | |
-`PulseGenerators` | class for setting up the pulse generator functionality | |
-`DDS` | class for handling DDS functionality | To use a specific functionality
-simply initiate an instance of one of the classes and pass a device object:
-```python import spcm with spcm.Card('/dev/spcm0') as card: clock = spcm.Clock
-(card) # (or) trigger = spcm.Trigger(card) # (or) multi_io =
-spcm.MultiPurposeIOs(card) # (or) data_transfer = spcm.DataTransfer(card) # etc
-... ``` Each of these functionalities typically corresponds to a chapter in
-your device manual, so for further reference please have a look in the device
-manual. ## Setting up Channels The Channels functionality allows the user to
-setup individual channels on a Card or a CardStack. The channels object is also
-a Python iterator, hence if a channels object is used it a for-loop, each
-iteration provides a Channel object: ```python channels = spcm.Channels(card,
+Defining a quantity is as simple as: ```python from spcm import units frequency
+= 100 * units.MHz amplitude = 1 * units.V # etc... ``` All methods within the
+`spcm` that expect a value that is related to a physical quantity support the
+quantities, for example setting a timeout: ```python card.timeout(5 * units.s)
+``` See our dedicated examples for more information about where units can be
+used. ## Card Functionality After opening a card, StarHub or group of card,
+specific functionality of the cards can be accessed through `CardFunctionality`
+classes. | Name | Description | |---------------------|------------------------
+---------------------------------------------| | `Channels` | class for setting
+up the in- or output stage of the channels of a card | | `Clock` | class for
+setting up the clock engine of the card | | `Trigger` | class for setting up
+the trigger engine of the card | | `MultiPurposeIOs` | class for setting up the
+multi purpose i/o of the card | | `DataTransfer` | class for handling data
+transfer functionality | | `Multi` | class for handling multiple recording and
+replay mode functionality | | `Sequence` | class for handling sequence mode
+functionality | | `TimeStamp` | class for handling time stamped data | |
+`Boxcar` | class for handling boxcar averaging | | `BlockAverage` | class for
+handling block averaging functionality | | `PulseGenerators` | class for
+setting up the pulse generator functionality | | `DDS` | class for handling DDS
+functionality | To use a specific functionality simply initiate an instance of
+one of the classes and pass a device object: ```python import spcm with
+spcm.Card('/dev/spcm0') as card: clock = spcm.Clock(card) # (or) trigger =
+spcm.Trigger(card) # (or) multi_io = spcm.MultiPurposeIOs(card) # (or)
+data_transfer = spcm.DataTransfer(card) # etc ... ``` Each of these
+functionalities typically corresponds to a chapter in your device manual, so
+for further reference please have a look in the device manual. ## Setting up
+Channels The Channels functionality allows the user to setup individual
+channels on a Card or a CardStack. The channels object is also a Python
+iterator, hence if a channels object is used it a for-loop, each iteration
+provides a Channel object: ```python channels = spcm.Channels(card,
 card_enable=spcm.CHANNEL0 | CHANNEL1) for channel in channels: # do something
 with each channel ``` In addition, the user can define the output load
 connected to the channel (standard value 50 Ohm), to any resistor value or high
 impedance (`units.highZ`). With this output load, the amplitude setting can be
 done with the repect to this output load: ```python channels = Channels(card,
 card_enable=spcm.CHANNEL0 | CHANNEL1) channels[0].output_load(units.highZ)
 channels[0].amp(1 * units.V) # or for all channels channels.output_load
```

### Comparing `spcm-1.1.1/pyproject.toml` & `spcm-1.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/__init__.py` & `spcm-1.1.2/src/spcm/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,15 +61,22 @@
 __version__ = _version.get_versions()['version']
 
 # Writing spcm package version to log file
 try:
     from .pyspcm import spcm_dwGetParam_i64, spcm_dwSetParam_ptr, create_string_buffer, byref, int64
     driver_version = int64(0)
     spcm_dwGetParam_i64(None, SPC_GETDRVVERSION, byref(driver_version))
+    version_hex = driver_version.value
+    major = (version_hex & 0xFF000000) >> 24
+    minor = (version_hex & 0x00FF0000) >> 16
+    build = version_hex & 0x0000FFFF
     # Available starting from build 21797
-    if (driver_version.value & 0x0000FFFF) < 21797:
-        raise OSError("Driver version {} does not support writing spcm version to log".format(driver_version))
-    version_str = bytes("Python package spcm v{}".format(__version__), "utf-8")
+    if build < 21797:
+        version_str = "v{}.{}.{}".format(major, minor, build)
+        raise OSError(f"Driver version build {version_str} does not support writing spcm version to log")
+    from importlib.metadata import version
+    version_tag = version('spcm')
+    version_str = bytes("Python package spcm v{}".format(version_tag), "utf-8")
     version_ptr = create_string_buffer(version_str)
     dwErr = spcm_dwSetParam_ptr(None, SPC_WRITE_TO_LOG, version_ptr, len(version_str))
 except OSError as e:
     print(e)
```

### Comparing `spcm-1.1.1/src/spcm/classes_block_average.py` & `spcm-1.1.2/src/spcm/classes_block_average.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_boxcar.py` & `spcm-1.1.2/src/spcm/classes_boxcar.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_card.py` & `spcm-1.1.2/src/spcm/classes_card.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_card_stack.py` & `spcm-1.1.2/src/spcm/classes_card_stack.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_channels.py` & `spcm-1.1.2/src/spcm/classes_channels.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_clock.py` & `spcm-1.1.2/src/spcm/classes_clock.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_data_transfer.py` & `spcm-1.1.2/src/spcm/classes_data_transfer.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_dds.py` & `spcm-1.1.2/src/spcm/classes_dds.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_device.py` & `spcm-1.1.2/src/spcm/classes_device.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_error_exception.py` & `spcm-1.1.2/src/spcm/classes_error_exception.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_functionality.py` & `spcm-1.1.2/src/spcm/classes_functionality.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_multi.py` & `spcm-1.1.2/src/spcm/classes_multi.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_multi_purpose_ios.py` & `spcm-1.1.2/src/spcm/classes_multi_purpose_ios.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_netbox.py` & `spcm-1.1.2/src/spcm/classes_netbox.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_pulse_generators.py` & `spcm-1.1.2/src/spcm/classes_pulse_generators.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_sequence.py` & `spcm-1.1.2/src/spcm/classes_sequence.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_sync.py` & `spcm-1.1.2/src/spcm/classes_sync.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_time_stamp.py` & `spcm-1.1.2/src/spcm/classes_time_stamp.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_trigger.py` & `spcm-1.1.2/src/spcm/classes_trigger.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/classes_unit_conversion.py` & `spcm-1.1.2/src/spcm/classes_unit_conversion.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/pyspcm.py` & `spcm-1.1.2/src/spcm/pyspcm.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/regs.py` & `spcm-1.1.2/src/spcm/regs.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm/spcerr.py` & `spcm-1.1.2/src/spcm/spcerr.py`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/src/spcm.egg-info/PKG-INFO` & `spcm-1.1.2/src/spcm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spcm
-Version: 1.1.1
+Version: 1.1.2
 Summary: Package for Spectrum Instrumentation GmbH cards
 Author-email: Spectrum Instrumentation GmbH <info@spec.de>
 Project-URL: Homepage, https://spectrum-instrumentation.com/
 Project-URL: API, https://spectruminstrumentation.github.io/spcm/spcm.html
 Project-URL: Repository, https://github.com/SpectrumInstrumentation/spcm
 Project-URL: Examples, https://github.com/SpectrumInstrumentation/spcm/tree/master/src/examples
 Project-URL: Knowledge Base, https://spectrum-instrumentation.com/support/knowledgebase/index.php
@@ -48,16 +48,17 @@
 
 # Supported devices
 
 See the [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices.
 
 # Requirements
 [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)](https://badge.fury.io/py/spcm)
-[![Static Badge](https://img.shields.io/badge/NumPy-1.25-green)](https://numpy.org/)
-[![Static Badge](https://img.shields.io/badge/h5py-3.10-orange)](https://www.h5py.org/)
+[![Static Badge](https://img.shields.io/badge/NumPy-1.25+-green)](https://numpy.org/)
+[![Static Badge](https://img.shields.io/badge/h5py-3.10+-orange)](https://www.h5py.org/)
+[![Static Badge](https://img.shields.io/badge/pint-0.23+-teal)](https://pint.readthedocs.io/en/stable/)
 
 `spcm` requires the Spectrum Instrumentation [driver](https://spectrum-instrumentation.com/support/downloads.php) which is available for Windows and Linux. 
 Please have a look in the manual of your product for more information about installing the driver on the different plattforms.
 
 # Installation and dependencies
 [![Pip Package](https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
 [![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml)
@@ -172,15 +173,15 @@
 
 `spcm` uses [pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that have a physical unit. To enable the use of qunatities simply import the units module from `spcm`:
 
 ```python
 from spcm import units
 ```
 
-This import the `units` object from `spcm`. which is a `UnitRegistry` object from  `pint`. Defining a quantity is as simples as:
+This imports the `units` object from `spcm`. which is a `UnitRegistry` object from `pint`. Defining a quantity is as simple as:
 
 ```python
 from spcm import units
 
 frequency = 100 * units.MHz
 amplitude = 1 * units.V
 # etc...
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: spcm Version: 1.1.1 Summary: Package for Spectrum
+Metadata-Version: 2.1 Name: spcm Version: 1.1.2 Summary: Package for Spectrum
 Instrumentation GmbH cards Author-email: Spectrum Instrumentation GmbH
 spec.de> Project-URL: Homepage, https://spectrum-instrumentation.com/ Project-
 URL: API, https://spectruminstrumentation.github.io/spcm/spcm.html Project-URL:
 Repository, https://github.com/SpectrumInstrumentation/spcm Project-URL:
 Examples, https://github.com/SpectrumInstrumentation/spcm/tree/master/src/
 examples Project-URL: Knowledge Base, https://spectrum-instrumentation.com/
 support/knowledgebase/index.php Classifier: Development Status :: 4 - Beta
@@ -30,22 +30,24 @@
 oriented Python package for interfacing with Spectrum Instrumentation GmbH
 devices. `spcm` can handle individual cards (`Card`), StarHubs (`Sync`), groups
 of cards (`CardStack`) and Netboxes (`Netbox`). # Supported devices See the
 [SUPPORTED_DEVICES.md](https://github.com/SpectrumInstrumentation/spcm/blob/
 master/src/spcm/SUPPORTED_DEVICES.md) file for a list of supported devices. #
 Requirements [![Python](https://img.shields.io/pypi/pyversions/spcm.svg)]
 (https://badge.fury.io/py/spcm) [![Static Badge](https://img.shields.io/badge/
-NumPy-1.25-green)](https://numpy.org/) [![Static Badge](https://img.shields.io/
-badge/h5py-3.10-orange)](https://www.h5py.org/) `spcm` requires the Spectrum
-Instrumentation [driver](https://spectrum-instrumentation.com/support/
-downloads.php) which is available for Windows and Linux. Please have a look in
-the manual of your product for more information about installing the driver on
-the different plattforms. # Installation and dependencies [![Pip Package]
-(https://img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm)
-[![Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/
+NumPy-1.25+-green)](https://numpy.org/) [![Static Badge](https://
+img.shields.io/badge/h5py-3.10+-orange)](https://www.h5py.org/) [![Static
+Badge](https://img.shields.io/badge/pint-0.23+-teal)](https://
+pint.readthedocs.io/en/stable/) `spcm` requires the Spectrum Instrumentation
+[driver](https://spectrum-instrumentation.com/support/downloads.php) which is
+available for Windows and Linux. Please have a look in the manual of your
+product for more information about installing the driver on the different
+plattforms. # Installation and dependencies [![Pip Package](https://
+img.shields.io/pypi/v/spcm?logo=PyPI)](https://pypi.org/project/spcm) [!
+[Publish to PyPI](https://github.com/SpectrumInstrumentation/spcm/actions/
 workflows/spcm-publish-to-pypi.yml/badge.svg)](https://github.com/
 SpectrumInstrumentation/spcm/actions/workflows/spcm-publish-to-pypi.yml) Start
 by installing Python 3.9 or higher. We recommend using the latest version. You
 can download Python from [https://www.python.org/](https://www.python.org/).
 You would probably also like to install and use a virtual environment, although
 it's not strictly necessary. See the examples [README.md](https://github.com/
 SpectrumInstrumentation/spcm/blob/master/src/examples/README.md) for a more
@@ -108,46 +110,46 @@
 Center gives the user the option to create [demo devices](https://spectrum-
 instrumentation.com/support/knowledgebase/software/
 How_to_set_up_a_demo_card.php). These demo devices can be used in the same
 manner as real devices. Simply change the device identifier string to the
 string as shown in the Control Center. ## Units and quantities `spcm` uses
 [pint](https://pint.readthedocs.io/en/stable/) to handle all quantities that
 have a physical unit. To enable the use of qunatities simply import the units
-module from `spcm`: ```python from spcm import units ``` This import the
+module from `spcm`: ```python from spcm import units ``` This imports the
 `units` object from `spcm`. which is a `UnitRegistry` object from `pint`.
-Defining a quantity is as simples as: ```python from spcm import units
-frequency = 100 * units.MHz amplitude = 1 * units.V # etc... ``` All methods
-within the `spcm` that expect a value that is related to a physical quantity
-support the quantities, for example setting a timeout: ```python card.timeout(5
-* units.s) ``` See our dedicated examples for more information about where
-units can be used. ## Card Functionality After opening a card, StarHub or group
-of card, specific functionality of the cards can be accessed through
-`CardFunctionality` classes. | Name | Description | |---------------------|----
------------------------------------------------------------------| | `Channels`
-| class for setting up the in- or output stage of the channels of a card | |
-`Clock` | class for setting up the clock engine of the card | | `Trigger` |
-class for setting up the trigger engine of the card | | `MultiPurposeIOs` |
-class for setting up the multi purpose i/o of the card | | `DataTransfer` |
-class for handling data transfer functionality | | `Multi` | class for handling
-multiple recording and replay mode functionality | | `Sequence` | class for
-handling sequence mode functionality | | `TimeStamp` | class for handling time
-stamped data | | `Boxcar` | class for handling boxcar averaging | |
-`BlockAverage` | class for handling block averaging functionality | |
-`PulseGenerators` | class for setting up the pulse generator functionality | |
-`DDS` | class for handling DDS functionality | To use a specific functionality
-simply initiate an instance of one of the classes and pass a device object:
-```python import spcm with spcm.Card('/dev/spcm0') as card: clock = spcm.Clock
-(card) # (or) trigger = spcm.Trigger(card) # (or) multi_io =
-spcm.MultiPurposeIOs(card) # (or) data_transfer = spcm.DataTransfer(card) # etc
-... ``` Each of these functionalities typically corresponds to a chapter in
-your device manual, so for further reference please have a look in the device
-manual. ## Setting up Channels The Channels functionality allows the user to
-setup individual channels on a Card or a CardStack. The channels object is also
-a Python iterator, hence if a channels object is used it a for-loop, each
-iteration provides a Channel object: ```python channels = spcm.Channels(card,
+Defining a quantity is as simple as: ```python from spcm import units frequency
+= 100 * units.MHz amplitude = 1 * units.V # etc... ``` All methods within the
+`spcm` that expect a value that is related to a physical quantity support the
+quantities, for example setting a timeout: ```python card.timeout(5 * units.s)
+``` See our dedicated examples for more information about where units can be
+used. ## Card Functionality After opening a card, StarHub or group of card,
+specific functionality of the cards can be accessed through `CardFunctionality`
+classes. | Name | Description | |---------------------|------------------------
+---------------------------------------------| | `Channels` | class for setting
+up the in- or output stage of the channels of a card | | `Clock` | class for
+setting up the clock engine of the card | | `Trigger` | class for setting up
+the trigger engine of the card | | `MultiPurposeIOs` | class for setting up the
+multi purpose i/o of the card | | `DataTransfer` | class for handling data
+transfer functionality | | `Multi` | class for handling multiple recording and
+replay mode functionality | | `Sequence` | class for handling sequence mode
+functionality | | `TimeStamp` | class for handling time stamped data | |
+`Boxcar` | class for handling boxcar averaging | | `BlockAverage` | class for
+handling block averaging functionality | | `PulseGenerators` | class for
+setting up the pulse generator functionality | | `DDS` | class for handling DDS
+functionality | To use a specific functionality simply initiate an instance of
+one of the classes and pass a device object: ```python import spcm with
+spcm.Card('/dev/spcm0') as card: clock = spcm.Clock(card) # (or) trigger =
+spcm.Trigger(card) # (or) multi_io = spcm.MultiPurposeIOs(card) # (or)
+data_transfer = spcm.DataTransfer(card) # etc ... ``` Each of these
+functionalities typically corresponds to a chapter in your device manual, so
+for further reference please have a look in the device manual. ## Setting up
+Channels The Channels functionality allows the user to setup individual
+channels on a Card or a CardStack. The channels object is also a Python
+iterator, hence if a channels object is used it a for-loop, each iteration
+provides a Channel object: ```python channels = spcm.Channels(card,
 card_enable=spcm.CHANNEL0 | CHANNEL1) for channel in channels: # do something
 with each channel ``` In addition, the user can define the output load
 connected to the channel (standard value 50 Ohm), to any resistor value or high
 impedance (`units.highZ`). With this output load, the amplitude setting can be
 done with the repect to this output load: ```python channels = Channels(card,
 card_enable=spcm.CHANNEL0 | CHANNEL1) channels[0].output_load(units.highZ)
 channels[0].amp(1 * units.V) # or for all channels channels.output_load
```

### Comparing `spcm-1.1.1/src/spcm.egg-info/SOURCES.txt` & `spcm-1.1.2/src/spcm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spcm-1.1.1/versioneer.py` & `spcm-1.1.2/versioneer.py`

 * *Files identical despite different names*

