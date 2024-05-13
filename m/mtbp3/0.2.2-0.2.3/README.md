# Comparing `tmp/mtbp3-0.2.2-py3-none-any.whl.zip` & `tmp/mtbp3-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 248648 bytes, number of entries: 52
+Zip file size: 255760 bytes, number of entries: 54
 -rw-r--r--  2.0 unx     6148 b- defN 80-Jan-01 00:00 mtbp3/.DS_Store
 -rw-r--r--  2.0 unx      351 b- defN 80-Jan-01 00:00 mtbp3/__init__.py
 -rw-r--r--  2.0 unx     6148 b- defN 80-Jan-01 00:00 mtbp3/data/.DS_Store
+-rw-r--r--  2.0 unx    19789 b- defN 80-Jan-01 00:00 mtbp3/data/supp_ectd/fda_ctoc_v2.3.3.txt
 -rw-r--r--  2.0 unx  1016108 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/FMQ/FMQ_Consolidated_List.csv
 -rw-r--r--  2.0 unx       42 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/!!readme_26_1_English.txt
 -rw-r--r--  2.0 unx     2221 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/MedAscii/hlgt.asc
 -rw-r--r--  2.0 unx     3060 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/MedAscii/hlgt_hlt.asc
 -rw-r--r--  2.0 unx     6877 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/MedAscii/hlt.asc
 -rw-r--r--  2.0 unx    10906 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/MedAscii/hlt_pt.asc
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/MedAscii/intl_ord.asc
@@ -37,18 +38,19 @@
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_emt/MedDRA/whatsnew_26_1_English.pdf
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder1/testfile10
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder1/testfile11
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder1/testfile12
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder2/testfile20
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 mtbp3/data/test_lsr/testfolder2/testfile3
 -rw-r--r--  2.0 unx       19 b- defN 80-Jan-01 00:00 mtbp3/health/__init__.py
--rw-r--r--  2.0 unx     7081 b- defN 80-Jan-01 00:00 mtbp3/health/clinical.py
+-rw-r--r--  2.0 unx     9095 b- defN 80-Jan-01 00:00 mtbp3/health/clinical.py
+-rw-r--r--  2.0 unx     2113 b- defN 80-Jan-01 00:00 mtbp3/health/ectd.py
 -rw-r--r--  2.0 unx    34117 b- defN 80-Jan-01 00:00 mtbp3/health/emt.py
 -rw-r--r--  2.0 unx       58 b- defN 80-Jan-01 00:00 mtbp3/util/__init__.py
 -rw-r--r--  2.0 unx    12727 b- defN 80-Jan-01 00:00 mtbp3/util/cdt.py
 -rw-r--r--  2.0 unx    17343 b- defN 80-Jan-01 00:00 mtbp3/util/cdtg.py
 -rw-r--r--  2.0 unx    11887 b- defN 80-Jan-01 00:00 mtbp3/util/lsr.py
--rw-r--r--  2.0 unx    35107 b- defN 80-Jan-01 00:00 mtbp3-0.2.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2429 b- defN 80-Jan-01 00:00 mtbp3-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mtbp3-0.2.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     4968 b- defN 16-Jan-01 00:00 mtbp3-0.2.2.dist-info/RECORD
-52 files, 1384158 bytes uncompressed, 240414 bytes compressed:  82.6%
+-rw-r--r--  2.0 unx    35107 b- defN 80-Jan-01 00:00 mtbp3-0.2.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2672 b- defN 80-Jan-01 00:00 mtbp3-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 mtbp3-0.2.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx     5143 b- defN 16-Jan-01 00:00 mtbp3-0.2.3.dist-info/RECORD
+54 files, 1408492 bytes uncompressed, 247254 bytes compressed:  82.4%
```

## zipnote {}

```diff
@@ -3,14 +3,17 @@
 
 Filename: mtbp3/__init__.py
 Comment: 
 
 Filename: mtbp3/data/.DS_Store
 Comment: 
 
+Filename: mtbp3/data/supp_ectd/fda_ctoc_v2.3.3.txt
+Comment: 
+
 Filename: mtbp3/data/test_emt/FMQ/FMQ_Consolidated_List.csv
 Comment: 
 
 Filename: mtbp3/data/test_emt/MedDRA/!!readme_26_1_English.txt
 Comment: 
 
 Filename: mtbp3/data/test_emt/MedDRA/MedAscii/hlgt.asc
@@ -123,14 +126,17 @@
 
 Filename: mtbp3/health/__init__.py
 Comment: 
 
 Filename: mtbp3/health/clinical.py
 Comment: 
 
+Filename: mtbp3/health/ectd.py
+Comment: 
+
 Filename: mtbp3/health/emt.py
 Comment: 
 
 Filename: mtbp3/util/__init__.py
 Comment: 
 
 Filename: mtbp3/util/cdt.py
@@ -138,20 +144,20 @@
 
 Filename: mtbp3/util/cdtg.py
 Comment: 
 
 Filename: mtbp3/util/lsr.py
 Comment: 
 
-Filename: mtbp3-0.2.2.dist-info/LICENSE
+Filename: mtbp3-0.2.3.dist-info/LICENSE
 Comment: 
 
-Filename: mtbp3-0.2.2.dist-info/METADATA
+Filename: mtbp3-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: mtbp3-0.2.2.dist-info/WHEEL
+Filename: mtbp3-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: mtbp3-0.2.2.dist-info/RECORD
+Filename: mtbp3-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mtbp3/health/clinical.py

```diff
@@ -1,8 +1,8 @@
-#  Copyright (C) 2023 Y Hsu <yh202109@gmail.com>
+#  Copyright (C) 2023-2024 Y Hsu <yh202109@gmail.com>
 #
 #  This program is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public license as published by
 #  the Free software Foundation, either version 3 of the License, or
 #  any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -11,29 +11,50 @@
 #  GNU General Public License for more details
 #
 #  You should have received a copy of the GNU General Public license
 #  along with this program. If not, see <https://www.gnu.org/license/>
 
 import numpy as np
 import pandas as pd
-import random
 
 class summary_by_group:
+    """
+    A class for generating summary statistics and performing calculations on a DataFrame.
+
+    Attributes:
+        df (pandas.DataFrame): The input DataFrame.
+
+    Methods:
+        __init__(self, df): Initializes the summary_by_group class.
+        generate_dataset(design=1): Generate an example dataset for clinical health.
+        count_by_group(columns): Count occurrences of unique combinations of values in the DataFrame.
+        count_to_cate(group_columns, target_column, bins, stats): Convert numerical data into categorical data based on specified bins and calculate statistics.
+    """
+
     def __init__(self, df):
+        """
+        Initializes the summary_by_group class.
+
+        Args:
+            df (pandas.DataFrame): The input DataFrame.
+
+        Raises:
+            ValueError: If the input is not a DataFrame.
+        """
         if df is None:
             df = self.generate_dataset()
         self.df = df
 
     @staticmethod
     def generate_dataset(design=1):
         """
         Generate an example dataset for clinical health.
 
         Args:
-            type (int, optional): The type of dataset to generate. Defaults to 1.
+            design (int, optional): The type of dataset to generate. Defaults to 1.
 
         Returns:
             df (pandas.DataFrame): The generated example dataset.
         """
         df = pd.DataFrame()
         if design==1:
             for study in range(2): 
@@ -55,25 +76,55 @@
                                                             'subject': [f"SUBJ{subject+1:02d}"] * m0[visit],
                                                             'visit': [f"VISIT{visit+1}"] * m0[visit],
                                                             'meal': range(1, m0[visit] + 1)})
             df['calorie'] = np.random.randint(300, 2001, size=len(df))
         return df
     
     def count_by_group(self, columns):
+        """
+        Count occurrences of unique combinations of values in the DataFrame.
+
+        Args:
+            columns (list): The columns to group by.
+
+        Returns:
+            grouped_df (pandas.DataFrame): The grouped DataFrame with count.
+
+        Raises:
+            ValueError: If the input is not a DataFrame or columns is not a list or a column does not exist in the DataFrame.
+        """
         if not isinstance(self.df, pd.DataFrame):
             raise ValueError("Input is not a DataFrame.")
         if not isinstance(columns, list):
             raise ValueError("columns should be a list.")
         for col in columns:
             if col not in self.df.columns:
                 raise ValueError(f"Column '{col}' does not exist in the DataFrame.")
         grouped_df = self.df.groupby(columns, observed=False).size().reset_index(name='count')
         return grouped_df
     
     def count_to_cate(self, group_columns, target_column, bins, stats):
+        """
+        Convert numerical data into categorical data based on specified bins and calculate statistics.
+
+        Args:
+            group_columns (list): The columns to group by.
+            target_column (str): The column to convert and calculate statistics on.
+            bins (int or list or numpy.ndarray): The bin edges for converting the target_column.
+            stats (list): The statistics to calculate.
+
+        Returns:
+            out1 (pandas.DataFrame): The resulting DataFrame with calculated statistics.
+
+        Raises:
+            ValueError: If the input is not a DataFrame or group_columns is not a list or contains non-string elements,
+                        target_column is not a non-empty string or does not exist in the DataFrame,
+                        target_column is not a numerical column, bins is not an integer or a sequence of bin edges,
+                        or stats is not a list of strings or contains invalid statistics.
+        """
         if not isinstance(self.df, pd.DataFrame):
             raise ValueError("Input is not a DataFrame.")
         if not isinstance(group_columns, list):
             raise ValueError("group_columns should be a list.")
         if not all(isinstance(col, str) for col in group_columns):
             raise ValueError("group_columns should contain only strings.")
         if not target_column or not isinstance(target_column, str):
@@ -98,15 +149,15 @@
             if stat == 'count':
                 out0 = self.df.groupby(group_columns, observed=False)[target_column].apply(lambda x: np.histogram(x, bins=bins)[0]).reset_index()
                 out0_columns = [f"N({bins[i]}<=X<{bins[i+1]})" for i in range(nb - 2)]+[f"N({bins[nb-2]}<=V<={bins[nb-1]})"]
                 out0[out0_columns] = pd.DataFrame(out0[target_column].tolist(), index=out0.index)
                 out0.drop(columns=[target_column], inplace=True)
             elif stat == 'sum':
                 out0 = self.df.groupby(group_columns, observed=False)[target_column].apply(lambda x: np.histogram(x, bins=bins, weights=x)[0]).reset_index()
-                out0_columns = [f"Sum({bins[i]}<=X<{bins[i+1]})" for i in range(nb - 2)]+[f"S({bins[nb-2]}<=V<={bins[nb-1]})"]
+                out0_columns = [f"Sum({bins[i]}<=X<{bins[i+1]})" for i in range(nb - 2)]+[f"Sum({bins[nb-2]}<=V<={bins[nb-1]})"]
                 out0[out0_columns] = pd.DataFrame(out0[target_column].tolist(), index=out0.index)
                 out0.drop(columns=[target_column], inplace=True)
             elif stat == 'total_max':
                 out0 = self.df.groupby(group_columns, observed=False)[target_column].max().reset_index()
                 out0.columns = group_columns + ['Max(all)']
             elif stat == 'total_min':
                 out0 = self.df.groupby(group_columns, observed=False)[target_column].min().reset_index()
@@ -124,11 +175,8 @@
                 else:
                     out1 = out0
 
         return out1
 
 if __name__ == "__main__":
     pass
-    summary = summary_by_group(df=None)
-    result = summary.count_to_cate(['study', 'treatment', 'subject', 'visit'], 'calorie', [0,500,1000,2000], stats=['count','total_count'])
-    print(result)
```

## Comparing `mtbp3-0.2.2.dist-info/LICENSE` & `mtbp3-0.2.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mtbp3-0.2.2.dist-info/METADATA` & `mtbp3-0.2.3.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mtbp3
-Version: 0.2.2
+Version: 0.2.3
 Summary: my tool box
 License: GNU General Public License v3.0
 Author: Y. Hsu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -16,21 +16,25 @@
 Description-Content-Type: text/markdown
 
 # mtbp3
 
 ![PyPI](https://img.shields.io/pypi/v/mtbp3?label=pypi%20package)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mtbp3)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/yh202109/mtbp3supp/main?filepath=binder/example_emt3_appendix.ipynb)
 
 My tool box in Python.
 
 Functions are grouped into:
-- MedDRA (drug labeling, safety reporting, pharmacovigilance, etc.)
-- Clinical trial data
+- Clinical data standards (CDISC, etc.)
+- Clinical study data summary
+- eCTD (including FDA CTOC, etc.)
 - Graphs
+- MedDRA (for drug labeling, safety reporting, pharmacovigilance, etc.)
+- Sampling 
 - System
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Usage](#usage)
 - [Contributing](#contributing)
```

## Comparing `mtbp3-0.2.2.dist-info/RECORD` & `mtbp3-0.2.3.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 mtbp3/.DS_Store,sha256=QzT-vQLbfKBTCne-BfEgM-Wl9Y13mU3n2WgdSkUKIBE,6148
 mtbp3/__init__.py,sha256=QB3CP0nW5h-qIPPjAABV0RPW0Oru4AZec5b7obo3se0,351
 mtbp3/data/.DS_Store,sha256=6nQgUIvYQeZiI_zuWycQpr6AFWMVk0MKrwm6Ek62nM0,6148
+mtbp3/data/supp_ectd/fda_ctoc_v2.3.3.txt,sha256=Vmzs3iMwqmOMM6VxC-B59mrO6WiOM4FPvIaKnewaQuA,19789
 mtbp3/data/test_emt/FMQ/FMQ_Consolidated_List.csv,sha256=kfXNT7SdZlXC71yYxfjQ0PNzzg1A9-QAHueAHR5IxbE,1016108
 mtbp3/data/test_emt/MedDRA/!!readme_26_1_English.txt,sha256=vGFFAJEm0yQIO8iWEgyYLssajjqZzs3mTuUbYxRkF7w,42
 mtbp3/data/test_emt/MedDRA/MedAscii/hlgt.asc,sha256=en5F63b8e9WHHryRUCbOAFE2KFIF3JJCdS9W9a02NCs,2221
 mtbp3/data/test_emt/MedDRA/MedAscii/hlgt_hlt.asc,sha256=taSowlfByEL3RIc_VXfMu_HpIjg8yivHUYgmPUXMSQ0,3060
 mtbp3/data/test_emt/MedDRA/MedAscii/hlt.asc,sha256=xCesMnCxxJf6Seig8IHaiN9NRU9c01Cv4itbO5btEcc,6877
 mtbp3/data/test_emt/MedDRA/MedAscii/hlt_pt.asc,sha256=fC0DtweOJBusW9AqUTkEFQUmzovo2LIfgL3y0p0PlNU,10906
 mtbp3/data/test_emt/MedDRA/MedAscii/intl_ord.asc,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -36,17 +37,18 @@
 mtbp3/data/test_emt/MedDRA/whatsnew_26_1_English.pdf,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/data/test_lsr/testfolder1/testfile10,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/data/test_lsr/testfolder1/testfile11,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/data/test_lsr/testfolder1/testfile12,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/data/test_lsr/testfolder2/testfile20,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/data/test_lsr/testfolder2/testfile3,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mtbp3/health/__init__.py,sha256=BqJVi0OMHyBp0zcg0IYDcPK1c9q8Fdil-Kcb2AHwNGY,19
-mtbp3/health/clinical.py,sha256=pS-Xr3BkMYhhpoWG62_NNWg_g0M3Iqgi1WH2VWpUG58,7081
+mtbp3/health/clinical.py,sha256=EiDRv70YPkc7sWtAs20a2X6c23uE3SWE9vucZQI1wYs,9095
+mtbp3/health/ectd.py,sha256=r-cifGeHTXbxwgFdkZX7nGfjR2fvEyXjifTAoovguic,2113
 mtbp3/health/emt.py,sha256=FwQUI70DL-O1Y_pGKjDiLziNcgWAYxlYXG6L-Egn0sk,34117
 mtbp3/util/__init__.py,sha256=dbXCXornfglTSgUXCslcrqXyt1lMaUjf5TCn0RdHApc,58
 mtbp3/util/cdt.py,sha256=H7Zsvr39VgIwktVl8kuifHdku2Pc2sPKCTOKAi0r0kw,12727
 mtbp3/util/cdtg.py,sha256=GC71CPeUhQIpsezfGlZsqASLm-kTQCBM7hl0hbda3Eo,17343
 mtbp3/util/lsr.py,sha256=zwoEKj2slqYa17joB1Zit55G9QEd52MVuW3teV4bUJk,11887
-mtbp3-0.2.2.dist-info/LICENSE,sha256=W6tWaP6lQAHSSUjl4SjXv1Ge3HPPc0CsPwJzih6lkWU,35107
-mtbp3-0.2.2.dist-info/METADATA,sha256=zSddRdSoPHmZX6Mj6BTq8k2o1IzazLmZ4XrmVFxRpSQ,2429
-mtbp3-0.2.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-mtbp3-0.2.2.dist-info/RECORD,,
+mtbp3-0.2.3.dist-info/LICENSE,sha256=W6tWaP6lQAHSSUjl4SjXv1Ge3HPPc0CsPwJzih6lkWU,35107
+mtbp3-0.2.3.dist-info/METADATA,sha256=l5Y7Ydq_VAhCZw6SbRxDkC27rkNjxAk5K_jSRHUq2zA,2672
+mtbp3-0.2.3.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+mtbp3-0.2.3.dist-info/RECORD,,
```

