# Comparing `tmp/idf-analysis-0.2.4.tar.gz` & `tmp/idf_analysis-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf-analysis-0.2.4.tar", last modified: Wed Jan 24 09:56:30 2024, max compression
+gzip compressed data, was "idf_analysis-0.2.5.tar", last modified: Mon May 13 09:27:49 2024, max compression
```

## Comparing `idf-analysis-0.2.4.tar` & `idf_analysis-0.2.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:56:30.080724 idf-analysis-0.2.4/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       98 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    14907 2024-01-24 09:56:30.080724 idf-analysis-0.2.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13279 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:56:30.076723 idf-analysis-0.2.4/idf_analysis/
--rw-r--r--   0 root         (0) root         (0)      624 2024-01-24 09:56:24.000000 idf-analysis-0.2.4/idf_analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)      245 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/__main__.py
--rw-r--r--   0 root         (0) root         (0)      254 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/_console_script.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:56:30.080724 idf-analysis-0.2.4/idf_analysis/approaches/
--rw-r--r--   0 root         (0) root         (0)      283 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/approaches/ATV-A_121.yaml
--rw-r--r--   0 root         (0) root         (0)      239 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/approaches/KOSTRA.yaml
--rw-r--r--   0 root         (0) root         (0)      241 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/approaches/convective_vs_advective.yaml
--rw-r--r--   0 root         (0) root         (0)     4309 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/arg_parser.py
--rw-r--r--   0 root         (0) root         (0)     1941 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/definitions.py
--rw-r--r--   0 root         (0) root         (0)     8024 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/event_series_analysis.py
--rw-r--r--   0 root         (0) root         (0)    24196 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/heavy_rainfall_index.py
--rw-r--r--   0 root         (0) root         (0)    12585 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/idf_backend.py
--rw-r--r--   0 root         (0) root         (0)    35308 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/idf_class.py
--rw-r--r--   0 root         (0) root         (0)     2546 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/in_out.py
--rw-r--r--   0 root         (0) root         (0)     5113 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/interim_result_plots.py
--rw-r--r--   0 root         (0) root         (0)     6906 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/little_helpers.py
--rw-r--r--   0 root         (0) root         (0)     3953 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/parameter_formulation_class.py
--rw-r--r--   0 root         (0) root         (0)     3750 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/parameter_formulations.py
--rw-r--r--   0 root         (0) root         (0)     4083 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/plot_helpers.py
--rw-r--r--   0 root         (0) root         (0)     6651 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/sww_utils.py
--rw-r--r--   0 root         (0) root         (0)     4988 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/idf_analysis/synthetic_rainseries.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-24 09:56:30.080724 idf-analysis-0.2.4/idf_analysis.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14907 2024-01-24 09:56:30.000000 idf-analysis-0.2.4/idf_analysis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      931 2024-01-24 09:56:30.000000 idf-analysis-0.2.4/idf_analysis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-24 09:56:30.000000 idf-analysis-0.2.4/idf_analysis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       80 2024-01-24 09:56:30.000000 idf-analysis-0.2.4/idf_analysis.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      147 2024-01-24 09:56:30.000000 idf-analysis-0.2.4/idf_analysis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-01-24 09:56:30.000000 idf-analysis-0.2.4/idf_analysis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2440 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-24 09:56:30.080724 idf-analysis-0.2.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-24 09:56:23.000000 idf-analysis-0.2.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       98 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    16171 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14543 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/idf_analysis/
+-rw-r--r--   0 root         (0) root         (0)      624 2024-05-13 09:27:46.000000 idf_analysis-0.2.5/idf_analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      245 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      254 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/_console_script.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/idf_analysis/approaches/
+-rw-r--r--   0 root         (0) root         (0)      283 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/approaches/ATV-A_121.yaml
+-rw-r--r--   0 root         (0) root         (0)      239 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/approaches/KOSTRA.yaml
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/approaches/convective_vs_advective.yaml
+-rw-r--r--   0 root         (0) root         (0)     4309 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/arg_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1941 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/definitions.py
+-rw-r--r--   0 root         (0) root         (0)     8024 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/event_series_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    24196 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/heavy_rainfall_index.py
+-rw-r--r--   0 root         (0) root         (0)    12585 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/idf_backend.py
+-rw-r--r--   0 root         (0) root         (0)    36166 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/idf_class.py
+-rw-r--r--   0 root         (0) root         (0)     2546 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/in_out.py
+-rw-r--r--   0 root         (0) root         (0)     5113 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/interim_result_plots.py
+-rw-r--r--   0 root         (0) root         (0)     6920 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/little_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     3953 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/parameter_formulation_class.py
+-rw-r--r--   0 root         (0) root         (0)     3750 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/parameter_formulations.py
+-rw-r--r--   0 root         (0) root         (0)     4083 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/plot_helpers.py
+-rw-r--r--   0 root         (0) root         (0)     6661 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/sww_utils.py
+-rw-r--r--   0 root         (0) root         (0)     4988 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/idf_analysis/synthetic_rainseries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/idf_analysis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16171 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      931 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      147 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-13 09:27:49.000000 idf_analysis-0.2.5/idf_analysis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2440 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 09:27:49.554271 idf_analysis-0.2.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 09:27:45.000000 idf_analysis-0.2.5/setup.py
```

### Comparing `idf-analysis-0.2.4/LICENSE` & `idf_analysis-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/PKG-INFO` & `idf_analysis-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-analysis
-Version: 0.2.4
+Version: 0.2.5
 Summary: heavy rain as a function of the duration and the return period acc. to DWA-A 531 (2012)
 Author-email: Markus Pichler <markus.pichler@tugraz.at>
 License: MIT
 Project-URL: Documentation, https://markuspic.github.io/intensity_duration_frequency_analysis/
 Project-URL: Changelog, https://github.com/MarkusPic/intensity_duration_frequency_analysis/-/blob/master/CHANGELOG.md
 Project-URL: homepage, https://github.com/MarkusPic/intensity_duration_frequency_analysis
 Keywords: duration,analysis,rainfall,dwd,idf,measurement-data,precipitation,kostra,dwa,heavy-rain,intensity-duration-frequency,design-rainfall,duration-steps,return-period,dwa-a-531
@@ -39,14 +39,15 @@
 
 
 # Intensity duration frequency analysis (based on KOSTRA)
 
 
 [![license](https://img.shields.io/github/license/markuspic/intensity_duration_frequency_analysis.svg?style=flat)](https://github.com/MarkusPic/intensity_duration_frequency_analysis/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/idf-analysis.svg)](https://pypi.python.org/pypi/idf-analysis)
+[![DOI](https://zenodo.org/badge/142560436.svg)](https://zenodo.org/doi/10.5281/zenodo.10559991)
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dd/idf-analysis)](https://pypi.python.org/pypi/idf-analysis)
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/idf-analysis)](https://pypi.python.org/pypi/idf-analysis)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/idf-analysis)](https://pypi.python.org/pypi/idf-analysis)
 
 
 Heavy rain as a function of the duration and the return period acc. to [DWA-A 531 (2012)](http://www.dwa.de/dwa/shop/shop.nsf/Produktanzeige?openform&produktid=P-DWAA-8XMUY2).
@@ -72,14 +73,18 @@
 
 This package was developed by [Markus Pichler](mailto:markus.pichler@tugraz.at) during his bachelor thesis and finalised it in the course of his employment at the [Institute of Urban Water Management and Landscape Water Engineering](https://www.sww.tugraz.at).
 
 ## Documentation
 
 Read the docs [here 📖](https://markuspic.github.io/intensity_duration_frequency_analysis).
 
+## Please cite as
+
+Pichler, M. (2024). idf_analysis: Intensity duration frequency analysis with python based on KOSTRA (v0.2.4). Zenodo. https://doi.org/10.5281/zenodo.10559992
+
 ## Installation
 
 This package is written in Python3. (use a version > 3.5)
 
 ```
 pip install idf-analysis
 ```
@@ -109,14 +114,45 @@
 Packages required for this program will be installed with pip during the installation process and can be seen 
 in the [`requirements.txt`](https://github.com/MarkusPic/intensity_duration_frequency_analysis/blob/master/requirements.txt) file.
 
 ## Usage
 
 The documentation of the python-API can be found [here](https://markuspic.github.io/intensity_duration_frequency_analysis/api.html).
 
+One basic usage could be:
+
+```python
+import pandas as pd
+from idf_analysis import IntensityDurationFrequencyAnalyse
+from idf_analysis.definitions import *
+
+# initialize of the analysis class
+idf = IntensityDurationFrequencyAnalyse(series_kind=SERIES.PARTIAL, worksheet=METHOD.KOSTRA, extended_durations=True)
+
+series = pd.Series(index=pd.DatetimeIndex(...), data=...)
+
+# setting the series for the analysis
+idf.set_series(series)
+# auto-save the calculated parameter so save time for a later use, as the parameters doesn't have to be calculated again.
+idf.auto_save_parameters('idf_parameters.yaml')
+```
+
+If you only want to analyse an already existing IDF-table
+
+```python
+import pandas as pd
+from idf_analysis import IntensityDurationFrequencyAnalyse
+
+idf_table = pd.DataFrame(...)
+# index: Duration Steps in minutes as int or float
+# columns: Return Periods in years as int or float
+# values: rainfall height in mm
+idf = IntensityDurationFrequencyAnalyse.from_idf_table(idf_table)
+```
+
 ## Commandline tool
 
 The following commands show the usage for Linux/Unix systems.
 To use these features on Windows you have to add ```python -m``` before each command.
 
 To start the script use following commands in the terminal/Prompt
```

### Comparing `idf-analysis-0.2.4/README.md` & `idf_analysis-0.2.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 # Intensity duration frequency analysis (based on KOSTRA)
 
 
 [![license](https://img.shields.io/github/license/markuspic/intensity_duration_frequency_analysis.svg?style=flat)](https://github.com/MarkusPic/intensity_duration_frequency_analysis/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/idf-analysis.svg)](https://pypi.python.org/pypi/idf-analysis)
+[![DOI](https://zenodo.org/badge/142560436.svg)](https://zenodo.org/doi/10.5281/zenodo.10559991)
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dd/idf-analysis)](https://pypi.python.org/pypi/idf-analysis)
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/idf-analysis)](https://pypi.python.org/pypi/idf-analysis)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/idf-analysis)](https://pypi.python.org/pypi/idf-analysis)
 
 
 Heavy rain as a function of the duration and the return period acc. to [DWA-A 531 (2012)](http://www.dwa.de/dwa/shop/shop.nsf/Produktanzeige?openform&produktid=P-DWAA-8XMUY2).
@@ -35,14 +36,18 @@
 
 This package was developed by [Markus Pichler](mailto:markus.pichler@tugraz.at) during his bachelor thesis and finalised it in the course of his employment at the [Institute of Urban Water Management and Landscape Water Engineering](https://www.sww.tugraz.at).
 
 ## Documentation
 
 Read the docs [here 📖](https://markuspic.github.io/intensity_duration_frequency_analysis).
 
+## Please cite as
+
+Pichler, M. (2024). idf_analysis: Intensity duration frequency analysis with python based on KOSTRA (v0.2.4). Zenodo. https://doi.org/10.5281/zenodo.10559992
+
 ## Installation
 
 This package is written in Python3. (use a version > 3.5)
 
 ```
 pip install idf-analysis
 ```
@@ -72,14 +77,45 @@
 Packages required for this program will be installed with pip during the installation process and can be seen 
 in the [`requirements.txt`](https://github.com/MarkusPic/intensity_duration_frequency_analysis/blob/master/requirements.txt) file.
 
 ## Usage
 
 The documentation of the python-API can be found [here](https://markuspic.github.io/intensity_duration_frequency_analysis/api.html).
 
+One basic usage could be:
+
+```python
+import pandas as pd
+from idf_analysis import IntensityDurationFrequencyAnalyse
+from idf_analysis.definitions import *
+
+# initialize of the analysis class
+idf = IntensityDurationFrequencyAnalyse(series_kind=SERIES.PARTIAL, worksheet=METHOD.KOSTRA, extended_durations=True)
+
+series = pd.Series(index=pd.DatetimeIndex(...), data=...)
+
+# setting the series for the analysis
+idf.set_series(series)
+# auto-save the calculated parameter so save time for a later use, as the parameters doesn't have to be calculated again.
+idf.auto_save_parameters('idf_parameters.yaml')
+```
+
+If you only want to analyse an already existing IDF-table
+
+```python
+import pandas as pd
+from idf_analysis import IntensityDurationFrequencyAnalyse
+
+idf_table = pd.DataFrame(...)
+# index: Duration Steps in minutes as int or float
+# columns: Return Periods in years as int or float
+# values: rainfall height in mm
+idf = IntensityDurationFrequencyAnalyse.from_idf_table(idf_table)
+```
+
 ## Commandline tool
 
 The following commands show the usage for Linux/Unix systems.
 To use these features on Windows you have to add ```python -m``` before each command.
 
 To start the script use following commands in the terminal/Prompt
```

### Comparing `idf-analysis-0.2.4/idf_analysis/__init__.py` & `idf_analysis-0.2.5/idf_analysis/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __author__ = "Markus Pichler"
 __credits__ = ["Markus Pichler"]
 __maintainer__ = "Markus Pichler"
 __email__ = "markus.pichler@tugraz.at"
-__version__ = '0.2.4'
+__version__ = '0.2.5'
 __license__ = "MIT"
 
 from .idf_class import IntensityDurationFrequencyAnalyse, SERIES, METHOD
 
 """
 Heavy rain as a function of the duration and the return period acc. to DWA-A 531 (2012)
```

### Comparing `idf-analysis-0.2.4/idf_analysis/arg_parser.py` & `idf_analysis-0.2.5/idf_analysis/arg_parser.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis/definitions.py` & `idf_analysis-0.2.5/idf_analysis/definitions.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis/event_series_analysis.py` & `idf_analysis-0.2.5/idf_analysis/event_series_analysis.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis/heavy_rainfall_index.py` & `idf_analysis-0.2.5/idf_analysis/heavy_rainfall_index.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis/idf_backend.py` & `idf_analysis-0.2.5/idf_analysis/idf_backend.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis/idf_class.py` & `idf_analysis-0.2.5/idf_analysis/idf_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,22 +290,23 @@
 
         Returns:
             float: duration in minutes
         """
         return newton(lambda d: self.depth_of_rainfall(d, return_period) - height_of_rainfall, x0=1)
 
     # __________________________________________________________________________________________________________________
-    def result_table(self, durations=None, return_periods=None, add_names=False):
+    def result_table(self, durations=None, return_periods=None, add_names=False, add_unit=True):
         """
         Get an idf-table of rainfall depth with return periods as columns and durations as rows.
 
         Args:
             durations (list | numpy.ndarray): list of durations in minutes for the table
             return_periods (list): list of return periods in years for the table
-            add_names (bool): weather to use expressive names as index-&column-label
+            add_names (bool): weather to use expressive names as index- & column-label
+            add_unit (bool): weather to add units to index- & column-label
 
         Returns:
             pandas.DataFrame: idf table
         """
         if durations is None:
             durations = self.duration_steps_for_output
 
@@ -315,17 +316,18 @@
         result_table = {}
         for t in return_periods:
             result_table[t] = self.depth_of_rainfall(durations, t)
 
         result_table = pd.DataFrame(result_table, index=durations)
 
         if add_names:
-            result_table.index.name = 'duration (min)'
+            result_table.index.name = 'duration' + (' (min)' if add_unit else '')
             result_table.columns = pd.MultiIndex.from_tuples([(rp, round(1 / rp, 3)) for rp in result_table.columns])
-            result_table.columns.names = ['return period (a)', 'frequency (1/a)']
+            result_table.columns.names = ['return period' + (' (a)' if add_unit else ''),
+                                          'frequency' + (' (1/a)' if add_unit else '')]
         return result_table
 
     ####################################################################################################################
     def result_figure(self, min_duration=5.0, max_duration=720.0, logx=False, return_periods=None, color=True, ax=None,
                       linestyle=None, add_interim=False, alpha=1):
         """
         Create a plot with the idf-curves with duration on the x-axis and rainfall depth on the y-axis.
@@ -645,14 +647,29 @@
             pandas.DataFrame: events table including the columns with the maximum intensities
         """
         sum_frame = self.rainfall_sum_frame
         for duration in self.duration_steps:
             events[f'max_sum_{duration:0.0f}'] = agg_events(events, sum_frame[duration], 'max').round(2)
         return events
 
+    def add_max_return_periods_pre_duration_to_events(self, events):
+        """
+        Add the maximum return periods for all duration steps to the events table.
+
+        Args:
+            events (pandas.DataFrame): events table
+
+        Returns:
+            pandas.DataFrame: events table including the columns with the maximum return periods
+        """
+        return_periods_frame = self.return_periods_frame
+        for duration in self.duration_steps:
+            events[f'max_return_period_{duration:0.0f}'] = agg_events(events, return_periods_frame[duration], 'max').round(2)
+        return events
+
     ####################################################################################################################
     def event_report(self, filename, min_event_rain_sum=25, min_return_period=0.5, durations=None):
         """
         create pdf file with the biggest rain events
         for each event is represented by a plot of the rain series
         and a IDF analysis where the return periods are calculated
 
@@ -735,15 +752,16 @@
             idf_bar_ax = idf_bar_axes(idf_bar_ax, return_periods_frame_extended)
             rain_ax = fig.add_subplot(212, sharex=idf_bar_ax)
 
         # -------------------------------------
         ts_sum, minutes = resample_rain_series(ts)
         rain_ax = rain_bar_plot(ts_sum, rain_ax)
         rain_ax.set_ylabel('{} in {}/{}min'.format(column_name, unit, minutes if minutes != 1 else ''))
-        rain_ax.set_xlim(ts.index[0], ts.index[-1])
+        if ts.index.size > 1:
+            rain_ax.set_xlim(ts.index[0], ts.index[-1])
 
         return fig, (event_caption_ger(event) if german_caption else event_caption(event, unit))
 
     ####################################################################################################################
     def event_return_period_report(self, filename, min_return_period=1):
         import matplotlib.pyplot as plt
         from matplotlib.backends.backend_pdf import PdfPages
```

### Comparing `idf-analysis-0.2.4/idf_analysis/in_out.py` & `idf_analysis-0.2.5/idf_analysis/in_out.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis/interim_result_plots.py` & `idf_analysis-0.2.5/idf_analysis/interim_result_plots.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis/little_helpers.py` & `idf_analysis-0.2.5/idf_analysis/little_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     Args:
         time_delta (pandas.Timedelta, pandas.DateOffset):
 
     Returns:
         float: the timedelta in minutes
     """
     if isinstance(time_delta, pd.DateOffset):
-        time_delta = time_delta.delta
+        time_delta = pd.Timedelta(time_delta)
     return int(time_delta.total_seconds() / 60)
 
 
 def minutes_readable(minutes):
     """
     convert the duration in minutes to a more readable form
 
@@ -175,15 +175,15 @@
         return '$\\gg$ 100'
     elif t > 100:
         return '> 100'
     else:
         return f'{t:0.1f}'
 
 
-def timedelta_components_plus(td, min_freq='T'):
+def timedelta_components_plus(td, min_freq='min'):
     """Schaltjahre nicht miteinbezogen"""
     l = []
 
     # years, weeks
     days_year = 365
     days_week = 7
 
@@ -206,20 +206,20 @@
         ['{}{}{}'.format(v, '' if short else ' ', c[0] if short else (c if v > 1 else c[:-1])) for v, c in l if v > 0])
     if not short:
         # replace last "," with "and"
         s = ' and '.join(s.rsplit(sep, 1))
     return s
 
 
-def timedelta_readable(td, min_freq='T', short=False, sep=', '):
+def timedelta_readable(td, min_freq='min', short=False, sep=', '):
     """Schaltjahre nicht miteinbezogen"""
     return timedelta_components_readable(timedelta_components_plus(td, min_freq), short=short, sep=sep)
 
 
-def timedelta_readable2(d1, d2, min_freq='T', short=False, sep=', '):
+def timedelta_readable2(d1, d2, min_freq='min', short=False, sep=', '):
     td = d2 - d1
 
     years = None
     if td > Timedelta(days=365):
         d2_new = d2.replace(year=d1.year)
 
         if d2_new < d1:
```

### Comparing `idf-analysis-0.2.4/idf_analysis/parameter_formulation_class.py` & `idf_analysis-0.2.5/idf_analysis/parameter_formulation_class.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis/parameter_formulations.py` & `idf_analysis-0.2.5/idf_analysis/parameter_formulations.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis/plot_helpers.py` & `idf_analysis-0.2.5/idf_analysis/plot_helpers.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis/sww_utils.py` & `idf_analysis-0.2.5/idf_analysis/sww_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,12 +207,12 @@
     freq = guess_freq(series.index)
 
     minutes = 1
     for duration_limit, minutes in resample_minutes:
         if dur < duration_limit:
             break
 
-    if freq.delta > pd.Timedelta(minutes=minutes):
+    if pd.Timedelta(freq) > pd.Timedelta(minutes=minutes):
         return series, int(freq / pd.Timedelta(minutes=1))
 
     # print('resample_rain_series: ', dur, duration_limit, minutes)
-    return series.resample('{}T'.format(minutes)).sum(), minutes
+    return series.resample('{}min'.format(minutes)).sum(), minutes
```

### Comparing `idf-analysis-0.2.4/idf_analysis/synthetic_rainseries.py` & `idf_analysis-0.2.5/idf_analysis/synthetic_rainseries.py`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/idf_analysis.egg-info/PKG-INFO` & `idf_analysis-0.2.5/idf_analysis.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-analysis
-Version: 0.2.4
+Version: 0.2.5
 Summary: heavy rain as a function of the duration and the return period acc. to DWA-A 531 (2012)
 Author-email: Markus Pichler <markus.pichler@tugraz.at>
 License: MIT
 Project-URL: Documentation, https://markuspic.github.io/intensity_duration_frequency_analysis/
 Project-URL: Changelog, https://github.com/MarkusPic/intensity_duration_frequency_analysis/-/blob/master/CHANGELOG.md
 Project-URL: homepage, https://github.com/MarkusPic/intensity_duration_frequency_analysis
 Keywords: duration,analysis,rainfall,dwd,idf,measurement-data,precipitation,kostra,dwa,heavy-rain,intensity-duration-frequency,design-rainfall,duration-steps,return-period,dwa-a-531
@@ -39,14 +39,15 @@
 
 
 # Intensity duration frequency analysis (based on KOSTRA)
 
 
 [![license](https://img.shields.io/github/license/markuspic/intensity_duration_frequency_analysis.svg?style=flat)](https://github.com/MarkusPic/intensity_duration_frequency_analysis/blob/master/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/idf-analysis.svg)](https://pypi.python.org/pypi/idf-analysis)
+[![DOI](https://zenodo.org/badge/142560436.svg)](https://zenodo.org/doi/10.5281/zenodo.10559991)
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dd/idf-analysis)](https://pypi.python.org/pypi/idf-analysis)
 [![PyPI - Downloads](https://img.shields.io/pypi/dw/idf-analysis)](https://pypi.python.org/pypi/idf-analysis)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/idf-analysis)](https://pypi.python.org/pypi/idf-analysis)
 
 
 Heavy rain as a function of the duration and the return period acc. to [DWA-A 531 (2012)](http://www.dwa.de/dwa/shop/shop.nsf/Produktanzeige?openform&produktid=P-DWAA-8XMUY2).
@@ -72,14 +73,18 @@
 
 This package was developed by [Markus Pichler](mailto:markus.pichler@tugraz.at) during his bachelor thesis and finalised it in the course of his employment at the [Institute of Urban Water Management and Landscape Water Engineering](https://www.sww.tugraz.at).
 
 ## Documentation
 
 Read the docs [here 📖](https://markuspic.github.io/intensity_duration_frequency_analysis).
 
+## Please cite as
+
+Pichler, M. (2024). idf_analysis: Intensity duration frequency analysis with python based on KOSTRA (v0.2.4). Zenodo. https://doi.org/10.5281/zenodo.10559992
+
 ## Installation
 
 This package is written in Python3. (use a version > 3.5)
 
 ```
 pip install idf-analysis
 ```
@@ -109,14 +114,45 @@
 Packages required for this program will be installed with pip during the installation process and can be seen 
 in the [`requirements.txt`](https://github.com/MarkusPic/intensity_duration_frequency_analysis/blob/master/requirements.txt) file.
 
 ## Usage
 
 The documentation of the python-API can be found [here](https://markuspic.github.io/intensity_duration_frequency_analysis/api.html).
 
+One basic usage could be:
+
+```python
+import pandas as pd
+from idf_analysis import IntensityDurationFrequencyAnalyse
+from idf_analysis.definitions import *
+
+# initialize of the analysis class
+idf = IntensityDurationFrequencyAnalyse(series_kind=SERIES.PARTIAL, worksheet=METHOD.KOSTRA, extended_durations=True)
+
+series = pd.Series(index=pd.DatetimeIndex(...), data=...)
+
+# setting the series for the analysis
+idf.set_series(series)
+# auto-save the calculated parameter so save time for a later use, as the parameters doesn't have to be calculated again.
+idf.auto_save_parameters('idf_parameters.yaml')
+```
+
+If you only want to analyse an already existing IDF-table
+
+```python
+import pandas as pd
+from idf_analysis import IntensityDurationFrequencyAnalyse
+
+idf_table = pd.DataFrame(...)
+# index: Duration Steps in minutes as int or float
+# columns: Return Periods in years as int or float
+# values: rainfall height in mm
+idf = IntensityDurationFrequencyAnalyse.from_idf_table(idf_table)
+```
+
 ## Commandline tool
 
 The following commands show the usage for Linux/Unix systems.
 To use these features on Windows you have to add ```python -m``` before each command.
 
 To start the script use following commands in the terminal/Prompt
```

### Comparing `idf-analysis-0.2.4/idf_analysis.egg-info/SOURCES.txt` & `idf_analysis-0.2.5/idf_analysis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idf-analysis-0.2.4/pyproject.toml` & `idf_analysis-0.2.5/pyproject.toml`

 * *Files identical despite different names*

