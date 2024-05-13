# Comparing `tmp/dataprep_ml-0.0.9.tar.gz` & `tmp/dataprep_ml-24.5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataprep_ml-0.0.9.tar", max compression
+gzip compressed data, was "dataprep_ml-24.5.1.0.tar", max compression
```

## Comparing `dataprep_ml-0.0.9.tar` & `dataprep_ml-24.5.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35104 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/LICENSE
--rw-r--r--   0        0        0      130 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/README.md
--rw-r--r--   0        0        0      190 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/__init__.py
--rw-r--r--   0        0        0     1984 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/base.py
--rw-r--r--   0        0        0    13732 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/cleaners.py
--rw-r--r--   0        0        0     1191 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/helpers.py
--rw-r--r--   0        0        0     3342 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/imputers.py
--rw-r--r--   0        0        0     9213 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/insights.py
--rw-r--r--   0        0        0     6549 2023-02-22 04:59:45.199893 dataprep_ml-0.0.9/dataprep_ml/splitters.py
--rw-r--r--   0        0        0      558 2023-02-22 04:59:45.203893 dataprep_ml-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      950 1970-01-01 00:00:00.000000 dataprep_ml-0.0.9/setup.py
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 dataprep_ml-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0    35104 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/LICENSE
+-rw-r--r--   0        0        0     1762 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/README.md
+-rw-r--r--   0        0        0      193 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/__init__.py
+-rw-r--r--   0        0        0     1984 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/base.py
+-rw-r--r--   0        0        0    18873 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/cleaners.py
+-rw-r--r--   0        0        0     1197 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/helpers.py
+-rw-r--r--   0        0        0     3342 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/imputers.py
+-rw-r--r--   0        0        0     9314 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/insights.py
+-rw-r--r--   0        0        0     4615 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/recommenders.py
+-rw-r--r--   0        0        0     6633 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/dataprep_ml/splitters.py
+-rw-r--r--   0        0        0      626 2024-05-13 12:38:43.993131 dataprep_ml-24.5.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2677 1970-01-01 00:00:00.000000 dataprep_ml-24.5.1.0/PKG-INFO
```

### Comparing `dataprep_ml-0.0.9/LICENSE` & `dataprep_ml-24.5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataprep_ml-0.0.9/dataprep_ml/base.py` & `dataprep_ml-24.5.1.0/dataprep_ml/base.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-0.0.9/dataprep_ml/helpers.py` & `dataprep_ml-24.5.1.0/dataprep_ml/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
 import random
 import logging
-from typing import Iterable
-
 import colorlog
 import numpy as np
 import pandas as pd
 
 from type_infer.helpers import is_nan_numeric
 
 
@@ -27,16 +25,16 @@
 
 
 def seed(seed_nr: int) -> None:
     np.random.seed(seed_nr)
     random.seed(seed_nr)
 
 
-def filter_nan_and_none(series: Iterable) -> list:
-    return [x for x in series if not is_nan_numeric(x) and x is not None]
+def filter_nan_and_none(series: pd.Series) -> pd.Series:
+    return series.apply(lambda x: x if (not is_nan_numeric(x) and x is not None) else np.nan).dropna()
 
 
 def get_ts_groups(df: pd.DataFrame, tss) -> list:
     ##############################
     # TODO - Should refactor this
     ##############################
     group_combinations = ['__default']
```

### Comparing `dataprep_ml-0.0.9/dataprep_ml/imputers.py` & `dataprep_ml-24.5.1.0/dataprep_ml/imputers.py`

 * *Files identical despite different names*

### Comparing `dataprep_ml-0.0.9/dataprep_ml/insights.py` & `dataprep_ml-24.5.1.0/dataprep_ml/insights.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import numpy as np
 import pandas as pd
 from scipy.stats import entropy
 from dateutil.parser import parse as parse_dt
 
 from type_infer.dtype import dtype
-from type_infer.infer import infer_types
+from type_infer.api import infer_types
 
 from dataprep_ml.cleaners import cleaner
 from dataprep_ml.cleaners import _clean_float
 from dataprep_ml.helpers import get_ts_groups
 from dataprep_ml.helpers import filter_nan_and_none
 
 from dataprep_ml.helpers import log
@@ -31,15 +31,15 @@
     if target is None:
         target = df.columns[0]
     if args is None:
         args = {'target': target}
     else:
         args['target'] = target
 
-    type_information = infer_types(df, args.get('pct_invalid', 2))
+    type_information = infer_types(df)
     stats = statistical_analysis(df, type_information.dtypes, args, type_information.identifiers)
     return DataAnalysis(type_information=type_information, statistical_analysis=stats)
 
 
 def statistical_analysis(data: pd.DataFrame,
                          dtypes: Dict[str, str],
                          args,  # TODO: refactor this so that input is not ProblemDefinition but normal Dict
@@ -178,17 +178,21 @@
         ts_stats=ts_stats
     )
 
 
 def get_datetime_histogram(data: pd.Series, bins: int) -> Dict[str, list]:
     """Generates the histogram for date and datetime types
     """
-    if isinstance(data[0], float) or isinstance(data[0], int):
-        data = [_clean_float(x) for x in data]
+    if isinstance(data.iloc[0], float) or isinstance(data.iloc[0], int):
+        data = _clean_float(data)
+    elif isinstance(data.iloc[0], pd.Timestamp):
+        # TODO: this should probably be deleted
+        data = data.apply(lambda x: x.timestamp())
     else:
+        # TODO: slow, optimize
         data = [_clean_float(parse_dt(str(x)).timestamp()) for x in data]
 
     Y, X = np.histogram(data, bins=min(bins, len(set(data))),
                         range=(min(data), max(data)), density=False)
 
     X = X[:-1].tolist()
     Y = Y.tolist()
@@ -200,21 +204,18 @@
     }
 
 
 def get_numeric_histogram(data: pd.Series, data_dtype: dtype, bins: int) -> Dict[str, list]:
     """Generate the histogram for integer and float typed data
     """
     # Handle arrays that are actual arrays and not things that become arrays later
-    if isinstance(data[0], list):
-        new_data = []
-        for arr in data:
-            new_data.extend(arr)
-        data = new_data
+    if isinstance(data.iloc[0], list):
+        data = data.applymap(lambda x: x[0]).values.reshape(-1, 1)
 
-    data = [_clean_float(x) for x in data]
+    data = _clean_float(data)
 
     Y, X = np.histogram(data, bins=min(bins, len(set(data))),
                         range=(min(data), max(data)), density=False)
     if data_dtype == dtype.integer:
         Y, X = np.histogram(data, bins=[int(round(x)) for x in X], density=False)
 
     X = X[:-1].tolist()
```

### Comparing `dataprep_ml-0.0.9/dataprep_ml/splitters.py` & `dataprep_ml-24.5.1.0/dataprep_ml/splitters.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import List, Dict, Union
-from itertools import product
 
 import numpy as np
 import pandas as pd
 from type_infer.dtype import dtype
 
 from dataprep_ml.helpers import log
 
@@ -54,14 +53,21 @@
     # Split the data
     if stratify_on:
         reshuffle = not tss.get('is_timeseries', False)
         train, dev, test = stratify(data, pct_train, pct_dev, pct_test, stratify_on, seed, reshuffle)
     else:
         train, dev, test = simple_split(data, pct_train, pct_dev, pct_test)
 
+    # Final assertions for time series
+    if min(len(train), len(dev)) < tss.get('window', 1):
+        raise Exception(f"Dataset size is too small for the specified window size ({tss.get('window', 1)})")
+
+    if min(len(train), len(dev), len(test)) < tss.get('horizon', 1):
+        raise Exception(f"Dataset size is too small for the specified horizon size ({tss.get('horizon', 1)})")
+
     return {"train": train, "test": test, "dev": dev, "stratified_on": stratify_on}
 
 
 def simple_split(data: pd.DataFrame,
                  pct_train: float,
                  pct_dev: float,
                  pct_test: float) -> List[pd.DataFrame]:
@@ -110,31 +116,29 @@
     :param seed: Random state for pandas data-frame shuffling
     :param reshuffle: specify if reshuffling should be done post-split
     :param atol: absolute tolerance for difference in stratification percentages. If violated, reverts to a non-stratified split.
 
     :returns Stratified train, dev, test dataframes
     """  # noqa
 
-    train_st = pd.DataFrame(columns=data.columns)
-    dev_st = pd.DataFrame(columns=data.columns)
-    test_st = pd.DataFrame(columns=data.columns)
-
-    all_group_combinations = list(product(*[data[col].unique() for col in stratify_on]))
-    for group in all_group_combinations:
-        df = data
-        for idx, col in enumerate(stratify_on):
-            df = df[df[col] == group[idx]]
-
-        train_cutoff = round(df.shape[0] * pct_train)
-        dev_cutoff = round(df.shape[0] * pct_dev) + train_cutoff
-        test_cutoff = round(df.shape[0] * pct_test) + dev_cutoff
-
-        train_st = pd.concat([train_st, df[:train_cutoff]])
-        dev_st = pd.concat([dev_st, df[train_cutoff:dev_cutoff]])
-        test_st = pd.concat([test_st, df[dev_cutoff:test_cutoff]])
+    train_sts = []
+    dev_sts = []
+    test_sts = []
+
+    fractions = np.array([pct_train, pct_dev, pct_test])
+    groups = data.groupby(by=stratify_on)
+    for _, df in groups:
+        train_st, dev_st, test_st = np.array_split(df, (fractions[:-1].cumsum() * len(df)).round().astype(int))
+        train_sts.append(train_st)
+        dev_sts.append(dev_st)
+        test_sts.append(test_st)
+
+    train_st = pd.concat(train_sts)
+    dev_st = pd.concat(dev_sts)
+    test_st = pd.concat(test_sts)
 
     if reshuffle:
         train_st, dev_st, test_st = [df.sample(frac=1, random_state=seed).reset_index(drop=True)
                                      for df in [train_st, dev_st, test_st]]
 
     # check that stratified lengths conform to expected percentages
     emp_tr = len(train_st) / len(data)
```

