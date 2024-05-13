# Comparing `tmp/anjana-0.0.2.tar.gz` & `tmp/anjana-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anjana-0.0.2.tar", max compression
+gzip compressed data, was "anjana-0.2.1.tar", max compression
```

## Comparing `anjana-0.0.2.tar` & `anjana-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11353 2024-03-19 16:17:26.810719 anjana-0.0.2/LICENSE
--rw-r--r--   0        0        0     8178 2024-04-17 15:18:31.376020 anjana-0.0.2/README.md
--rw-r--r--   0        0        0      743 2024-04-18 11:34:03.385593 anjana-0.0.2/anjana/__init__.py
--rw-r--r--   0        0        0     1277 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/__init__.py
--rw-r--r--   0        0        0     6416 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/_beta_likeness.py
--rw-r--r--   0        0        0     3629 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/_delta_disclosure.py
--rw-r--r--   0        0        0    10095 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/_k_anonymity.py
--rw-r--r--   0        0        0    13419 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/_l_diversity.py
--rw-r--r--   0        0        0     3501 2024-04-10 10:21:10.035760 anjana-0.0.2/anjana/anonymity/_t_closeness.py
--rw-r--r--   0        0        0      940 2024-04-18 11:15:39.469543 anjana-0.0.2/anjana/anonymity/utils/__init__.py
--rw-r--r--   0        0        0     4806 2024-04-18 11:34:03.385593 anjana-0.0.2/anjana/anonymity/utils/utils.py
--rw-r--r--   0        0        0     2048 2024-04-18 11:34:03.385593 anjana-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     9667 1970-01-01 00:00:00.000000 anjana-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11353 2024-05-13 14:49:49.797227 anjana-0.2.1/LICENSE
+-rw-r--r--   0        0        0     9993 2024-05-13 14:49:49.797227 anjana-0.2.1/README.md
+-rw-r--r--   0        0        0      743 2024-05-13 14:49:49.797227 anjana-0.2.1/anjana/__init__.py
+-rw-r--r--   0        0        0     1277 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/__init__.py
+-rw-r--r--   0        0        0     6416 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/_beta_likeness.py
+-rw-r--r--   0        0        0     3633 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/_delta_disclosure.py
+-rw-r--r--   0        0        0    10183 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/_k_anonymity.py
+-rw-r--r--   0        0        0    13604 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/_l_diversity.py
+-rw-r--r--   0        0        0     3501 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/_t_closeness.py
+-rw-r--r--   0        0        0      990 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/utils/__init__.py
+-rw-r--r--   0        0        0     6032 2024-05-13 14:49:49.801227 anjana-0.2.1/anjana/anonymity/utils/utils.py
+-rw-r--r--   0        0        0     2048 2024-05-13 14:49:49.829227 anjana-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    11482 1970-01-01 00:00:00.000000 anjana-0.2.1/PKG-INFO
```

### Comparing `anjana-0.0.2/LICENSE` & `anjana-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anjana-0.0.2/README.md` & `anjana-0.2.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 # ANJANA
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://gitlab.ifca.es/privacy-security/anjana/-/blob/main/LICENSE)
 [![codecov](https://codecov.io/gh/IFCA-Advanced-Computing/anjana/graph/badge.svg?token=AVI53GZ7YD)](https://codecov.io/gh/IFCA-Advanced-Computing/anjana)
-
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11184468.svg)](https://doi.org/10.5281/zenodo.11184468)
+![PyPI](https://img.shields.io/pypi/v/anjana)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/anjana)
+[![Documentation Status](https://readthedocs.org/projects/anjana/badge/?version=latest)](https://anjana.readthedocs.io/en/latest/?badge=latest)
+[![release-please](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/release-please.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/release-please.yml)
+[![Publish Package in PyPI](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/pypi.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/pypi.yml)
+[![CI/CD Pipeline](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/cicd.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/cicd.yml)
+[![Code Coverage](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/.codecov.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/.codecov.yml)
 ![Python version](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue)
 
-
 **Anonymity as major assurance of personal data privacy:**
 
 ANJANA is a Python library for anonymizing sensitive data.
 
 The following anonymity techniques are implemented, based on the Python library _[pyCANON](https://github.com/IFCA-Advanced-Computing/pycanon)_:
 * _k-anonymity_.
 * _(α,k)-anonymity_.
@@ -16,15 +22,15 @@
 * _Entropy ℓ-diversity_.
 * _Recursive (c,ℓ)-diversity_.
 * _t-closeness_.
 * _Basic β-likeness_.
 * _Enhanced β-likeness_.
 * _δ-disclosure privacy_.
 
-## :bulb: Installation
+## Installation
 First, we strongly recommend the use of a virtual environment. In linux: 
 ```bash
 virtualenv .venv -p python3
 source .venv/bin/activate
 ```
 
 **Using [pip](https://pypi.org/project/anjana/)**:
@@ -38,23 +44,23 @@
 
 Install the most updated version of anjana (linux and windows):
 
 ```bash
 pip install git+https://github.com/IFCA-Advanced-Computing/anjana.git
 ```
 
-## :rocket: Getting started
+## Getting started
 
 For anonymizing your data you need to introduce:
-* The **pandas dataframe** with the data to be anonymized. Each column can contain: indentifiers, quasi-indentifiers or sensitive attributes.
+* The **pandas dataframe** with the data to be anonymized. Each column can contain: identifiers, quasi-indentifiers or sensitive attributes.
 * The **list with the names of the identifiers** in the dataframe, in order to suppress them.
 * The **list with the names of the quasi-identifiers** in the dataframe.
 * The **sentive attribute** (only one) in case of applying other techniques than _k-anonymity_.
 * The **level of anonymity to be applied**, e.g. _k_ (for _k-anonymity_), _ℓ_ (for _ℓ-diversity_), _t_ (for _t-closeness_), _β_ (for _basic or enhanced β-likeness_), etc.
-* Maximum **level of record suppression** allowed (from 0 to 100).
+* Maximum **level of record suppression** allowed (from 0 to 100, acting as the percentage of suppressed records).
 * Dictionary containing one dictionary for each quasi-identifier with the **hierarchies** and the levels.
 
 ### Example: apply _k-anonymity_, _ℓ-diversity_ and _t-closeness_ to the [adult dataset](https://archive.ics.uci.edu/dataset/2/adult) with some predefined hierarchies:
 ```python
 import pandas as pd
 import anjana
 from anjana.anonymity import k_anonymity, l_diversity, t_closeness
@@ -133,14 +139,16 @@
 | Kishor    | 29  | Male   | Karnataka  | Heart-related  |
 | Johnson   | 17  | Male   | Kerala     | Heart-related  |
 | John      | 19  | Male   | Kerala     | Viralinfection |
 
 Then, in order to create the hierarquies we can define the following dictionary:
 
 ```python
+import numpy as np
+
 age = data['age'].values
 # Values: [29 24 28 27 24 23 19 29 17 19] (note that the following can be automatized)
 age_5years = ['[25, 30)', '[20, 25)', '[25, 30)',
               '[25, 30)', '[20, 25)', '[20, 25)',
               '[15, 20)', '[25, 30)', '[15, 20)', '[15, 20)']
 
 age_10years = ['[20, 30)', '[20, 30)', '[20, 30)',
@@ -156,18 +164,42 @@
         1: np.array(["*"] * len(data["gender"].values)) # Suppression
     },
     "city": {0: data["city"].values,
              1: np.array(["*"] * len(data["city"].values))} # Suppression
 }
 ```
 
-## :scroll: License
-This project is licensed under the [Apache 2.0 license](https://gitlab.ifca.es/privacy-security/anjana/-/blob/main/LICENSE?ref_type=heads).
+You can also use the function _generate_intervals()_ from _utils_ for creating the interval-based hierarchy as follows:
+
+```python
+import numpy as np
+from anjana.anonymity import utils
+
+age = data['age'].values
+
+hierarchies = {
+    "age": {
+        0: data["age"].values,
+        1: utils.generate_intervals(data["age"].values, 0, 100, 5),
+        2: utils.generate_intervals(data["age"].values, 0, 100, 10),
+    },
+    "gender": {
+        0: data["gender"].values,
+        1: np.array(["*"] * len(data["gender"].values)) # Suppression
+    },
+    "city": {0: data["city"].values,
+             1: np.array(["*"] * len(data["city"].values))} # Suppression
+}
+```
+
+
+## License
+This project is licensed under the [Apache 2.0 license](https://github.com/IFCA-Advanced-Computing/anjana/blob/main/LICENSE).
 
-## :warning: Project status
+## Project status
 This project is under active development.
 
 ## Funding and acknowledgments
 This work is funded by European Union through the SIESTA project (Horizon Europe) under Grant number 101131957.
 <p>
 <img align="center" width="250" src="https://ec.europa.eu/regional_policy/images/information-sources/logo-download-center/eu_funded_en.jpg">
 <img align="center" width="250" src="https://eosc.eu/wp-content/uploads/2024/01/SIESTA-Logo-1.png">
```

### Comparing `anjana-0.0.2/anjana/__init__.py` & `anjana-0.2.1/anjana/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
 """ANJANA is an open source framework for anonymizing data with different techniques."""
 
-__version__ = "0.0.2"
+__version__ = "0.2.1"
```

### Comparing `anjana-0.0.2/anjana/anonymity/__init__.py` & `anjana-0.2.1/anjana/anonymity/__init__.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.2/anjana/anonymity/_beta_likeness.py` & `anjana-0.2.1/anjana/anonymity/_beta_likeness.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.2/anjana/anonymity/_delta_disclosure.py` & `anjana-0.2.1/anjana/anonymity/_delta_disclosure.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         data, ident, quasi_ident, k, supp_level, hierarchies
     )
 
     delta_real = pycanon.anonymity.delta_disclosure(data_kanon, quasi_ident, [sens_att])
     quasi_ident_gen = copy(quasi_ident)
 
     if delta_real <= delta:
-        print(f"The data verifies delta-disclosure with t={delta_real}")
+        print(f"The data verifies delta-disclosure with delta={delta_real}")
         return data_kanon
 
     while delta_real > delta:
         if len(quasi_ident_gen) == 0:
             print(f"Delta-disclosure privacy cannot be achieved for delta={delta}")
             return pd.DataFrame()
```

### Comparing `anjana-0.0.2/anjana/anonymity/_k_anonymity.py` & `anjana-0.2.1/anjana/anonymity/_k_anonymity.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,33 +149,37 @@
         if alpha_real <= alpha:
             return data_kanon
 
         equiv_class = pycanon.anonymity.utils.aux_anonymity.get_equiv_class(
             data_kanon, quasi_ident
         )
 
+        k_ec = []
         alpha_ec = []
         for ec in equiv_class:
             data_temp = data_kanon.iloc[
                 pycanon.anonymity.utils.aux_functions.convert(ec)
             ]
             values = np.unique(data_temp[sens_att].values)
             alpha_s = [
                 len(data_temp[data_temp[sens_att] == s]) / len(data_temp)
                 for s in values
             ]
             alpha_ec.append(max(alpha_s))
+            k_ec.append(len(ec))
 
         if alpha > min(alpha_ec):
             if max(alpha_ec) <= alpha:
                 return data_kanon
 
-            data_ec = pd.DataFrame({"equiv_class": equiv_class, "alpha": alpha_ec})
+            data_ec = pd.DataFrame(
+                {"equiv_class": equiv_class, "alpha": alpha_ec, "k": k_ec}
+            )
             data_ec_alpha = data_ec[data_ec.alpha > alpha]
-            records_sup = sum(data_ec_alpha.alpha.values)
+            records_sup = sum(data_ec_alpha.k.values)
             if (records_sup + supp_records) * 100 / len(data) <= supp_level:
                 ec_elim = np.concatenate(
                     [
                         pycanon.anonymity.utils.aux_functions.convert(ec)
                         for ec in data_ec_alpha.equiv_class.values
                     ]
                 )
```

### Comparing `anjana-0.0.2/anjana/anonymity/_l_diversity.py` & `anjana-0.2.1/anjana/anonymity/_l_diversity.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,28 +250,32 @@
         c_real, l_real = pycanon.anonymity.recursive_c_l_diversity(
             data_kanon, quasi_ident, [sens_att]
         )
 
         equiv_class = pycanon.anonymity.utils.aux_anonymity.get_equiv_class(
             data_kanon, quasi_ident
         )
+        k_ec = []
         c_ec = []
         for ec in equiv_class:
             data_temp = data_kanon.iloc[
                 pycanon.anonymity.utils.aux_functions.convert(ec)
             ]
             values = np.unique(data_temp[sens_att].values)
             r_ec = np.sort([len(data_temp[data_temp[sens_att] == s]) for s in values])
             c_ec.append(np.floor(r_ec[0] / sum(r_ec[(l_div - 1) :]) + 1))
+            k_ec.append(len(ec))
             if max(c_ec) < c:
                 f"Recursive (c,l)-diversity cannot be achieved for l={l_div} and c={c}"
             else:
-                data_ec = pd.DataFrame({"equiv_class": equiv_class, "c_ec": c_ec})
+                data_ec = pd.DataFrame(
+                    {"equiv_class": equiv_class, "c_ec": c_ec, "k": k_ec}
+                )
                 data_ec_c = data_ec[data_ec.c_ec < c]
-                records_sup = sum(data_ec_c.c_ec.values)
+                records_sup = sum(data_ec_c.k.values)
                 if (records_sup + supp_records) * 100 / len(data) <= supp_level:
                     ec_elim = np.concatenate(
                         [
                             pycanon.anonymity.utils.aux_functions.convert(ec)
                             for ec in data_ec_c.equiv_class.values
                         ]
                     )
@@ -354,19 +358,22 @@
     while l_real < l_div:
         equiv_class = pycanon.anonymity.utils.aux_anonymity.get_equiv_class(
             data_kanon, quasi_ident
         )
         ec_sensitivity = [
             len(np.unique(data_kanon.iloc[ec][sens_att])) for ec in equiv_class
         ]
+        k_ec = [len(ec) for ec in equiv_class]
 
         if l_div > max(ec_sensitivity):
-            data_ec = pd.DataFrame({"equiv_class": equiv_class, "l": ec_sensitivity})
+            data_ec = pd.DataFrame(
+                {"equiv_class": equiv_class, "l": ec_sensitivity, "k": k_ec}
+            )
             data_ec_l = data_ec[data_ec.l < l_div]
-            records_sup = sum(data_ec_l.l.values)
+            records_sup = sum(data_ec_l.k.values)
             if (records_sup + supp_records_k) * 100 / len(data) <= supp_level:
                 ec_elim = np.concatenate(
                     [
                         pycanon.anonymity.utils.aux_functions.convert(ec)
                         for ec in data_ec_l.equiv_class.values
                     ]
                 )
```

### Comparing `anjana-0.0.2/anjana/anonymity/_t_closeness.py` & `anjana-0.2.1/anjana/anonymity/_t_closeness.py`

 * *Files identical despite different names*

### Comparing `anjana-0.0.2/anjana/anonymity/utils/__init__.py` & `anjana-0.2.1/anjana/anonymity/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 
 """Package containing auxiliary functions for performing the anonymization."""
 from .utils import (
     suppress_identifiers,
     apply_hierarchy,
     check_gen_level,
     get_transformation,
+    generate_intervals,
 )
 
 __all__ = [
     "suppress_identifiers",
     "apply_hierarchy",
     "check_gen_level",
     "get_transformation",
+    "generate_intervals",
 ]
```

### Comparing `anjana-0.0.2/anjana/anonymity/utils/utils.py` & `anjana-0.2.1/anjana/anonymity/utils/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -145,7 +145,48 @@
     for qi in quasi_ident:
         if qi in gen_level.keys():
             transformation.append(gen_level[qi])
         else:
             transformation.append(0)
 
     return transformation
+
+
+@beartype()
+def generate_intervals(
+    quasi_ident: typing.Union[typing.List, np.ndarray],
+    inf: typing.Union[int, float],
+    sup: typing.Union[int, float],
+    step: int,
+) -> list:
+    """
+    Generate intervals as hierarchies.
+
+    Given a quasi-identifier of numeric type, creates a list containing an
+    interval-based generalization (hierarchy) of the values of the quasi-identifier.
+    The intervals will have the length entered in step.
+
+    :param quasi_ident: values of the quasi-identifier on which the interval-based
+        generalization is to be obtained
+    :type quasi_ident: list or numpy array
+
+    :param inf: lower value of the set of intervals
+    :type inf: int or float
+
+    :param sup: bigger value of the set of intervals
+    :type sup: int or float
+
+    :param step: spacing between values of the intervals
+    :type step: int
+
+    :return: list with the intervals associated with the given values
+    :rtype: list
+    """
+    values = np.arange(inf, sup + 1, step)
+    interval = []
+    for num in quasi_ident:
+        lower = np.searchsorted(values, num)
+        if lower == 0:
+            lower = 1
+        interval.append(f"[{values[lower - 1]}, {values[lower]})")
+
+    return interval
```

### Comparing `anjana-0.0.2/pyproject.toml` & `anjana-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anjana"
-version = "0.0.2"
+version = "0.2.1"
 description = "ANJANA is an open source framework for applying different anonymity techniques."
 authors = [
     "Judith Sáinz-Pardo Díaz <sainzpardo@ifca.unican.es>",
     "Álvaro López García <aloga@ifca.unican.es>"
 ]
 maintainers = ["Judith Sáinz-Pardo Díaz <sainzpardo@ifca.unican.es>"]
 license = "Apache License 2.0"
```

### Comparing `anjana-0.0.2/PKG-INFO` & `anjana-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anjana
-Version: 0.0.2
+Version: 0.2.1
 Summary: ANJANA is an open source framework for applying different anonymity techniques.
 Home-page: https://gitlab.ifca.es/privacy-security/anjana
 License: Apache-2.0
 Keywords: anonymity,privacy
 Author: Judith Sáinz-Pardo Díaz
 Author-email: sainzpardo@ifca.unican.es
 Maintainer: Judith Sáinz-Pardo Díaz
@@ -33,18 +33,24 @@
 Requires-Dist: typing_extensions (==4.9.0)
 Project-URL: Repository, https://gitlab.ifca.es/privacy-security/anjana
 Description-Content-Type: text/markdown
 
 # ANJANA
 [![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-green.svg)](https://gitlab.ifca.es/privacy-security/anjana/-/blob/main/LICENSE)
 [![codecov](https://codecov.io/gh/IFCA-Advanced-Computing/anjana/graph/badge.svg?token=AVI53GZ7YD)](https://codecov.io/gh/IFCA-Advanced-Computing/anjana)
-
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.11184468.svg)](https://doi.org/10.5281/zenodo.11184468)
+![PyPI](https://img.shields.io/pypi/v/anjana)
+![PyPI - Downloads](https://img.shields.io/pypi/dm/anjana)
+[![Documentation Status](https://readthedocs.org/projects/anjana/badge/?version=latest)](https://anjana.readthedocs.io/en/latest/?badge=latest)
+[![release-please](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/release-please.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/release-please.yml)
+[![Publish Package in PyPI](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/pypi.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/pypi.yml)
+[![CI/CD Pipeline](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/cicd.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/cicd.yml)
+[![Code Coverage](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/.codecov.yml/badge.svg)](https://github.com/IFCA-Advanced-Computing/anjana/actions/workflows/.codecov.yml)
 ![Python version](https://img.shields.io/badge/python-3.9|3.10|3.11|3.12-blue)
 
-
 **Anonymity as major assurance of personal data privacy:**
 
 ANJANA is a Python library for anonymizing sensitive data.
 
 The following anonymity techniques are implemented, based on the Python library _[pyCANON](https://github.com/IFCA-Advanced-Computing/pycanon)_:
 * _k-anonymity_.
 * _(α,k)-anonymity_.
@@ -52,15 +58,15 @@
 * _Entropy ℓ-diversity_.
 * _Recursive (c,ℓ)-diversity_.
 * _t-closeness_.
 * _Basic β-likeness_.
 * _Enhanced β-likeness_.
 * _δ-disclosure privacy_.
 
-## :bulb: Installation
+## Installation
 First, we strongly recommend the use of a virtual environment. In linux: 
 ```bash
 virtualenv .venv -p python3
 source .venv/bin/activate
 ```
 
 **Using [pip](https://pypi.org/project/anjana/)**:
@@ -74,23 +80,23 @@
 
 Install the most updated version of anjana (linux and windows):
 
 ```bash
 pip install git+https://github.com/IFCA-Advanced-Computing/anjana.git
 ```
 
-## :rocket: Getting started
+## Getting started
 
 For anonymizing your data you need to introduce:
-* The **pandas dataframe** with the data to be anonymized. Each column can contain: indentifiers, quasi-indentifiers or sensitive attributes.
+* The **pandas dataframe** with the data to be anonymized. Each column can contain: identifiers, quasi-indentifiers or sensitive attributes.
 * The **list with the names of the identifiers** in the dataframe, in order to suppress them.
 * The **list with the names of the quasi-identifiers** in the dataframe.
 * The **sentive attribute** (only one) in case of applying other techniques than _k-anonymity_.
 * The **level of anonymity to be applied**, e.g. _k_ (for _k-anonymity_), _ℓ_ (for _ℓ-diversity_), _t_ (for _t-closeness_), _β_ (for _basic or enhanced β-likeness_), etc.
-* Maximum **level of record suppression** allowed (from 0 to 100).
+* Maximum **level of record suppression** allowed (from 0 to 100, acting as the percentage of suppressed records).
 * Dictionary containing one dictionary for each quasi-identifier with the **hierarchies** and the levels.
 
 ### Example: apply _k-anonymity_, _ℓ-diversity_ and _t-closeness_ to the [adult dataset](https://archive.ics.uci.edu/dataset/2/adult) with some predefined hierarchies:
 ```python
 import pandas as pd
 import anjana
 from anjana.anonymity import k_anonymity, l_diversity, t_closeness
@@ -169,14 +175,16 @@
 | Kishor    | 29  | Male   | Karnataka  | Heart-related  |
 | Johnson   | 17  | Male   | Kerala     | Heart-related  |
 | John      | 19  | Male   | Kerala     | Viralinfection |
 
 Then, in order to create the hierarquies we can define the following dictionary:
 
 ```python
+import numpy as np
+
 age = data['age'].values
 # Values: [29 24 28 27 24 23 19 29 17 19] (note that the following can be automatized)
 age_5years = ['[25, 30)', '[20, 25)', '[25, 30)',
               '[25, 30)', '[20, 25)', '[20, 25)',
               '[15, 20)', '[25, 30)', '[15, 20)', '[15, 20)']
 
 age_10years = ['[20, 30)', '[20, 30)', '[20, 30)',
@@ -192,18 +200,42 @@
         1: np.array(["*"] * len(data["gender"].values)) # Suppression
     },
     "city": {0: data["city"].values,
              1: np.array(["*"] * len(data["city"].values))} # Suppression
 }
 ```
 
-## :scroll: License
-This project is licensed under the [Apache 2.0 license](https://gitlab.ifca.es/privacy-security/anjana/-/blob/main/LICENSE?ref_type=heads).
+You can also use the function _generate_intervals()_ from _utils_ for creating the interval-based hierarchy as follows:
+
+```python
+import numpy as np
+from anjana.anonymity import utils
+
+age = data['age'].values
+
+hierarchies = {
+    "age": {
+        0: data["age"].values,
+        1: utils.generate_intervals(data["age"].values, 0, 100, 5),
+        2: utils.generate_intervals(data["age"].values, 0, 100, 10),
+    },
+    "gender": {
+        0: data["gender"].values,
+        1: np.array(["*"] * len(data["gender"].values)) # Suppression
+    },
+    "city": {0: data["city"].values,
+             1: np.array(["*"] * len(data["city"].values))} # Suppression
+}
+```
+
+
+## License
+This project is licensed under the [Apache 2.0 license](https://github.com/IFCA-Advanced-Computing/anjana/blob/main/LICENSE).
 
-## :warning: Project status
+## Project status
 This project is under active development.
 
 ## Funding and acknowledgments
 This work is funded by European Union through the SIESTA project (Horizon Europe) under Grant number 101131957.
 <p>
 <img align="center" width="250" src="https://ec.europa.eu/regional_policy/images/information-sources/logo-download-center/eu_funded_en.jpg">
 <img align="center" width="250" src="https://eosc.eu/wp-content/uploads/2024/01/SIESTA-Logo-1.png">
```

