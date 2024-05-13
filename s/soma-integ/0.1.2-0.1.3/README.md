# Comparing `tmp/soma_integ-0.1.2.tar.gz` & `tmp/soma_integ-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soma_integ-0.1.2.tar", last modified: Sun May 12 18:54:28 2024, max compression
+gzip compressed data, was "soma_integ-0.1.3.tar", last modified: Sun May 12 19:33:38 2024, max compression
```

## Comparing `soma_integ-0.1.2.tar` & `soma_integ-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 18:54:28.155751 soma_integ-0.1.2/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.2/LICENSE
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 18:54:28.155536 soma_integ-0.1.2/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.2/README.md
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-12 18:52:11.000000 soma_integ-0.1.2/pyproject.toml
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-12 18:54:28.155801 soma_integ-0.1.2/setup.cfg
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 18:54:28.150476 soma_integ-0.1.2/src/
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 18:54:28.153385 soma_integ-0.1.2/src/soma_integ/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      409 2024-05-12 08:37:42.000000 soma_integ-0.1.2/src/soma_integ/__init__.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 08:37:42.000000 soma_integ-0.1.2/src/soma_integ/config.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3522 2024-05-12 18:36:38.000000 soma_integ-0.1.2/src/soma_integ/data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     9221 2024-05-12 18:29:39.000000 soma_integ-0.1.2/src/soma_integ/evaluation.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-12 08:37:42.000000 soma_integ-0.1.2/src/soma_integ/methods.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 08:37:42.000000 soma_integ-0.1.2/src/soma_integ/model.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 08:37:42.000000 soma_integ-0.1.2/src/soma_integ/optimization.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.2/src/soma_integ/utils.py
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 18:54:28.155233 soma_integ-0.1.2/src/soma_integ.egg-info/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 18:54:28.000000 soma_integ-0.1.2/src/soma_integ.egg-info/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      474 2024-05-12 18:54:28.000000 soma_integ-0.1.2/src/soma_integ.egg-info/SOURCES.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-12 18:54:28.000000 soma_integ-0.1.2/src/soma_integ.egg-info/dependency_links.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-12 18:54:28.000000 soma_integ-0.1.2/src/soma_integ.egg-info/requires.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-12 18:54:28.000000 soma_integ-0.1.2/src/soma_integ.egg-info/top_level.txt
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 18:54:28.154901 soma_integ-0.1.2/tests/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      550 2024-05-12 18:49:52.000000 soma_integ-0.1.2/tests/test_data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      576 2024-05-12 08:37:42.000000 soma_integ-0.1.2/tests/test_evaluation.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 19:33:38.965422 soma_integ-0.1.3/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.3/LICENSE
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 19:33:38.965175 soma_integ-0.1.3/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.3/README.md
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-12 19:31:32.000000 soma_integ-0.1.3/pyproject.toml
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-12 19:33:38.965478 soma_integ-0.1.3/setup.cfg
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 19:33:38.960600 soma_integ-0.1.3/src/
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 19:33:38.963325 soma_integ-0.1.3/src/soma_integ/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      432 2024-05-12 19:26:59.000000 soma_integ-0.1.3/src/soma_integ/__init__.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 08:37:42.000000 soma_integ-0.1.3/src/soma_integ/config.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3522 2024-05-12 18:36:38.000000 soma_integ-0.1.3/src/soma_integ/data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     9100 2024-05-12 19:22:09.000000 soma_integ-0.1.3/src/soma_integ/evaluation.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-12 08:37:42.000000 soma_integ-0.1.3/src/soma_integ/methods.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 08:37:42.000000 soma_integ-0.1.3/src/soma_integ/model.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 08:37:42.000000 soma_integ-0.1.3/src/soma_integ/optimization.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.3/src/soma_integ/utils.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 19:33:38.964789 soma_integ-0.1.3/src/soma_integ.egg-info/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 19:33:38.000000 soma_integ-0.1.3/src/soma_integ.egg-info/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      474 2024-05-12 19:33:38.000000 soma_integ-0.1.3/src/soma_integ.egg-info/SOURCES.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-12 19:33:38.000000 soma_integ-0.1.3/src/soma_integ.egg-info/dependency_links.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-12 19:33:38.000000 soma_integ-0.1.3/src/soma_integ.egg-info/requires.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-12 19:33:38.000000 soma_integ-0.1.3/src/soma_integ.egg-info/top_level.txt
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 19:33:38.964401 soma_integ-0.1.3/tests/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      550 2024-05-12 18:49:52.000000 soma_integ-0.1.3/tests/test_data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2163 2024-05-12 19:30:36.000000 soma_integ-0.1.3/tests/test_evaluation.py
```

### Comparing `soma_integ-0.1.2/LICENSE` & `soma_integ-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.2/PKG-INFO` & `soma_integ-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.2/pyproject.toml` & `soma_integ-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "soma_integ"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = ["numpy", "scikit-learn"]
 authors = [
     { name = "Sobhan Ahmadian Moghadam", email = "sobhan.ahmadian.moghadam@gmail.com" },
     { name = "Arman Rezaei", email = "arman.x.rezaei@gmail.com" },
 ]
 description = "A package for integrating implementation and evaluation of machine learning platforms"
 readme = "README.md"
```

### Comparing `soma_integ-0.1.2/src/soma_integ/config.py` & `soma_integ-0.1.3/src/soma_integ/config.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.2/src/soma_integ/data.py` & `soma_integ-0.1.3/src/soma_integ/data.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.2/src/soma_integ/evaluation.py` & `soma_integ-0.1.3/src/soma_integ/evaluation.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,16 +23,14 @@
         f1 (float): The F1 score value.
         aupr (float): The Area Under the Precision-Recall Curve (AUPR) value.
         loss (float): The loss value.
         recall (float): The recall value.
         precision (float): The precision value.
         mcc (float): The Matthews Correlation Coefficient (MCC) value.
         max_f1 (float): The maximum F1 score value for different thresholds.
-        tpr (float): The True Positive Rate (TPR) value.
-        fpr (float): The False Positive Rate (FPR) value.
         fpr_list (list): The list of False Positive Rate values for different thresholds.
         tpr_list (list): The list of True Positive Rate values for different thresholds.
         auc_list (list): The list of AUC values for different thresholds.
 
     Methods:
         get_result(): Returns the evaluation result as a dictionary.
         add(result): Adds the values of another Result object to this Result object.
@@ -45,16 +43,14 @@
         self.f1 = 0
         self.aupr = 0
         self.loss = 0
         self.recall = 0
         self.precision = 0
         self.mcc = 0
         self.max_f1 = 0
-        self.tpr = 0
-        self.fpr = 0
         self.fpr_list = []
         self.tpr_list = []
         self.auc_list = []
 
     def get_result(self):
         """
         Returns the evaluation result as a dictionary.
@@ -127,16 +123,14 @@
         self.result.auc = self.result.auc / k
         self.result.aupr = self.result.aupr / k
         self.result.loss = self.result.loss / k
         self.result.recall = self.result.recall / k
         self.result.precision = self.result.precision / k
         self.result.mcc = self.result.mcc / k
         self.result.max_f1 = self.result.max_f1 / k
-        self.result.tpr = self.result.tpr / k
-        self.result.fpr = self.result.fpr / k
         self.result.fpr_list = (np.array(self.result.fpr_list) / k).tolist()
         self.result.tpr_list = (np.array(self.result.tpr_list) / k).tolist()
         self.result.auc_list = (np.array(self.result.auc_list) / k).tolist()
 
     def _accumulate(self, test_result):
         """
         Accumulates the result of a fold to the aggregated result.
@@ -149,25 +143,30 @@
         self.result.auc += test_result.auc
         self.result.aupr += test_result.aupr
         self.result.loss += test_result.loss
         self.result.recall += test_result.recall
         self.result.precision += test_result.precision
         self.result.mcc += test_result.mcc
         self.result.max_f1 += test_result.max_f1
-        self.result.tpr += test_result.tpr
-        self.result.fpr += test_result.fpr
+
         self.result.fpr_list = (
-            np.array(self.result.fpr_list) + np.array(test_result.fpr_list)
-        ).tolist()
+            (np.array(self.result.fpr_list) + np.array(test_result.fpr_list)).tolist()
+            if len(self.result.fpr_list) > 0
+            else test_result.fpr_list
+        )
         self.result.tpr_list = (
-            np.array(self.result.tpr_list) + np.array(test_result.tpr_list)
-        ).tolist()
+            (np.array(self.result.tpr_list) + np.array(test_result.tpr_list)).tolist()
+            if len(self.result.tpr_list) > 0
+            else test_result.tpr_list
+        )
         self.result.auc_list = (
-            np.array(self.result.auc_list) + np.array(test_result.auc_list)
-        ).tolist()
+            (np.array(self.result.auc_list) + np.array(test_result.auc_list)).tolist()
+            if len(self.result.auc_list) > 0
+            else test_result.auc_list
+        )
 
     def get_roc_curve(self, ax):
         """
         Plots the receiver operating characteristic (ROC) curve.
 
         Args:
             ax: The matplotlib axes object to plot on.
@@ -253,16 +252,14 @@
         numerator, denominator, out=np.zeros_like(denominator), where=(denominator != 0)
     )
     result.max_f1 = np.max(f1_scores)
 
     # Calculate AUC, TPR, FPR
     fpr, tpr, _ = roc_curve(y_test, y_predict, pos_label=1)
     result.auc = auc(fpr, tpr)
-    result.tpr = tpr
-    result.fpr = fpr
 
     # Calculate FPR, TPR and AUC Lists
     viz = RocCurveDisplay(fpr=fpr, tpr=tpr, roc_auc=result.auc)
     interp_tpr = np.interp(mean_fpr_list, viz.fpr, viz.tpr)
     interp_tpr[0] = 0.0
 
     result.mean_fpr_list = [mean_fpr_list]
```

### Comparing `soma_integ-0.1.2/src/soma_integ/methods.py` & `soma_integ-0.1.3/src/soma_integ/methods.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.2/src/soma_integ/model.py` & `soma_integ-0.1.3/src/soma_integ/model.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.2/src/soma_integ/optimization.py` & `soma_integ-0.1.3/src/soma_integ/optimization.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.2/src/soma_integ.egg-info/PKG-INFO` & `soma_integ-0.1.3/src/soma_integ.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.2/tests/test_data.py` & `soma_integ-0.1.3/tests/test_data.py`

 * *Files identical despite different names*

