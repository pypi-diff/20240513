# Comparing `tmp/soma_integ-0.1.4.tar.gz` & `tmp/soma_integ-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soma_integ-0.1.4.tar", last modified: Mon May 13 06:23:32 2024, max compression
+gzip compressed data, was "soma_integ-0.1.5.tar", last modified: Mon May 13 08:34:23 2024, max compression
```

## Comparing `soma_integ-0.1.4.tar` & `soma_integ-0.1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 06:23:32.155311 soma_integ-0.1.4/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.4/LICENSE
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-13 06:23:32.155096 soma_integ-0.1.4/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.4/README.md
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-13 06:22:42.000000 soma_integ-0.1.4/pyproject.toml
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-13 06:23:32.155358 soma_integ-0.1.4/setup.cfg
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 06:23:32.150684 soma_integ-0.1.4/src/
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 06:23:32.153405 soma_integ-0.1.4/src/soma_integ/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      432 2024-05-12 19:26:59.000000 soma_integ-0.1.4/src/soma_integ/__init__.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 08:37:42.000000 soma_integ-0.1.4/src/soma_integ/config.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3827 2024-05-13 06:21:12.000000 soma_integ-0.1.4/src/soma_integ/data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     9100 2024-05-12 19:22:09.000000 soma_integ-0.1.4/src/soma_integ/evaluation.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-12 08:37:42.000000 soma_integ-0.1.4/src/soma_integ/methods.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 08:37:42.000000 soma_integ-0.1.4/src/soma_integ/model.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 08:37:42.000000 soma_integ-0.1.4/src/soma_integ/optimization.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.4/src/soma_integ/utils.py
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 06:23:32.154789 soma_integ-0.1.4/src/soma_integ.egg-info/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-13 06:23:32.000000 soma_integ-0.1.4/src/soma_integ.egg-info/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      474 2024-05-13 06:23:32.000000 soma_integ-0.1.4/src/soma_integ.egg-info/SOURCES.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-13 06:23:32.000000 soma_integ-0.1.4/src/soma_integ.egg-info/dependency_links.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-13 06:23:32.000000 soma_integ-0.1.4/src/soma_integ.egg-info/requires.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-13 06:23:32.000000 soma_integ-0.1.4/src/soma_integ.egg-info/top_level.txt
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 06:23:32.154506 soma_integ-0.1.4/tests/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      550 2024-05-12 18:49:52.000000 soma_integ-0.1.4/tests/test_data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2163 2024-05-12 19:30:36.000000 soma_integ-0.1.4/tests/test_evaluation.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 08:34:23.812941 soma_integ-0.1.5/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.5/LICENSE
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-13 08:34:23.812707 soma_integ-0.1.5/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.5/README.md
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-13 08:33:52.000000 soma_integ-0.1.5/pyproject.toml
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-13 08:34:23.812990 soma_integ-0.1.5/setup.cfg
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 08:34:23.807594 soma_integ-0.1.5/src/
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 08:34:23.810660 soma_integ-0.1.5/src/soma_integ/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      432 2024-05-12 19:26:59.000000 soma_integ-0.1.5/src/soma_integ/__init__.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 08:37:42.000000 soma_integ-0.1.5/src/soma_integ/config.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3893 2024-05-13 08:22:30.000000 soma_integ-0.1.5/src/soma_integ/data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8483 2024-05-13 08:26:14.000000 soma_integ-0.1.5/src/soma_integ/evaluation.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-12 08:37:42.000000 soma_integ-0.1.5/src/soma_integ/methods.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 08:37:42.000000 soma_integ-0.1.5/src/soma_integ/model.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 08:37:42.000000 soma_integ-0.1.5/src/soma_integ/optimization.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.5/src/soma_integ/utils.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 08:34:23.812230 soma_integ-0.1.5/src/soma_integ.egg-info/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-13 08:34:23.000000 soma_integ-0.1.5/src/soma_integ.egg-info/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      474 2024-05-13 08:34:23.000000 soma_integ-0.1.5/src/soma_integ.egg-info/SOURCES.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-13 08:34:23.000000 soma_integ-0.1.5/src/soma_integ.egg-info/dependency_links.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-13 08:34:23.000000 soma_integ-0.1.5/src/soma_integ.egg-info/requires.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-13 08:34:23.000000 soma_integ-0.1.5/src/soma_integ.egg-info/top_level.txt
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 08:34:23.811938 soma_integ-0.1.5/tests/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      550 2024-05-12 18:49:52.000000 soma_integ-0.1.5/tests/test_data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2169 2024-05-13 08:24:55.000000 soma_integ-0.1.5/tests/test_evaluation.py
```

### Comparing `soma_integ-0.1.4/LICENSE` & `soma_integ-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.4/PKG-INFO` & `soma_integ-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.4/pyproject.toml` & `soma_integ-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "soma_integ"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = ["numpy", "scikit-learn"]
 authors = [
     { name = "Sobhan Ahmadian Moghadam", email = "sobhan.ahmadian.moghadam@gmail.com" },
     { name = "Arman Rezaei", email = "arman.x.rezaei@gmail.com" },
 ]
 description = "A package for integrating implementation and evaluation of machine learning platforms"
 readme = "README.md"
```

### Comparing `soma_integ-0.1.4/src/soma_integ/config.py` & `soma_integ-0.1.5/src/soma_integ/config.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.4/src/soma_integ/data.py` & `soma_integ-0.1.5/src/soma_integ/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,17 @@
         Args:
             i (int): The index of the subset to use for the test set.
 
         Returns:
             tuple: A tuple containing the train and test data objects.
 
         """
-        indices = set(range(0, len(self.data)))
+        indices = set(range(0, self.data_size))
         test_indices = list(self.subsets[i])
         train_indices = list(indices.difference(self.subsets[i]))
 
         train_data = PytorchData(self.data.X[train_indices], self.data.y[train_indices])
         test_data = PytorchData(self.data.X[test_indices], self.data.y[test_indices])
         return train_data, test_data
+
+    def get_data_size(self):
+        return self.data.X.shape[0]
```

### Comparing `soma_integ-0.1.4/src/soma_integ/evaluation.py` & `soma_integ-0.1.5/src/soma_integ/evaluation.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,17 +23,16 @@
         f1 (float): The F1 score value.
         aupr (float): The Area Under the Precision-Recall Curve (AUPR) value.
         loss (float): The loss value.
         recall (float): The recall value.
         precision (float): The precision value.
         mcc (float): The Matthews Correlation Coefficient (MCC) value.
         max_f1 (float): The maximum F1 score value for different thresholds.
-        fpr_list (list): The list of False Positive Rate values for different thresholds.
-        tpr_list (list): The list of True Positive Rate values for different thresholds.
-        auc_list (list): The list of AUC values for different thresholds.
+        fpr (np.ndarray): The false positive rate values.
+        tpr (np.ndarray): The true positive rate values.
 
     Methods:
         get_result(): Returns the evaluation result as a dictionary.
         add(result): Adds the values of another Result object to this Result object.
         divide(k): Divides the values of this Result object by a given number.
     """
 
@@ -43,17 +42,16 @@
         self.f1 = 0
         self.aupr = 0
         self.loss = 0
         self.recall = 0
         self.precision = 0
         self.mcc = 0
         self.max_f1 = 0
-        self.fpr_list = []
-        self.tpr_list = []
-        self.auc_list = []
+        self.fpr = None
+        self.tpr = None
 
     def get_result(self):
         """
         Returns the evaluation result as a dictionary.
 
         Returns:
             dict: A dictionary containing the evaluation metrics and their corresponding values.
@@ -123,17 +121,16 @@
         self.result.auc = self.result.auc / k
         self.result.aupr = self.result.aupr / k
         self.result.loss = self.result.loss / k
         self.result.recall = self.result.recall / k
         self.result.precision = self.result.precision / k
         self.result.mcc = self.result.mcc / k
         self.result.max_f1 = self.result.max_f1 / k
-        self.result.fpr_list = (np.array(self.result.fpr_list) / k).tolist()
-        self.result.tpr_list = (np.array(self.result.tpr_list) / k).tolist()
-        self.result.auc_list = (np.array(self.result.auc_list) / k).tolist()
+        self.result.fpr = self.result.fpr / k if self.result.fpr is not None else None
+        self.result.tpr = self.result.tpr / k if self.result.tpr is not None else None
 
     def _accumulate(self, test_result):
         """
         Accumulates the result of a fold to the aggregated result.
 
         Args:
             test_result (Result): The result of a fold.
@@ -144,43 +141,45 @@
         self.result.aupr += test_result.aupr
         self.result.loss += test_result.loss
         self.result.recall += test_result.recall
         self.result.precision += test_result.precision
         self.result.mcc += test_result.mcc
         self.result.max_f1 += test_result.max_f1
 
-        self.result.fpr_list = (
-            (np.array(self.result.fpr_list) + np.array(test_result.fpr_list)).tolist()
-            if len(self.result.fpr_list) > 0
-            else test_result.fpr_list
+        self.result.fpr = (
+            self.result.fpr + test_result.fpr if self.result.fpr is not None else test_result.fpr
         )
-        self.result.tpr_list = (
-            (np.array(self.result.tpr_list) + np.array(test_result.tpr_list)).tolist()
-            if len(self.result.tpr_list) > 0
-            else test_result.tpr_list
-        )
-        self.result.auc_list = (
-            (np.array(self.result.auc_list) + np.array(test_result.auc_list)).tolist()
-            if len(self.result.auc_list) > 0
-            else test_result.auc_list
+        self.result.tpr = (
+            self.result.tpr + test_result.tpr if self.result.tpr is not None else test_result.tpr
         )
 
-    def get_roc_curve(self, ax):
+    def get_roc_curve(self, ax, mean_fpr=np.linspace(0, 1, 100)):
         """
         Plots the receiver operating characteristic (ROC) curve.
 
         Args:
             ax: The matplotlib axes object to plot on.
+            mean_fpr (array-like, optional): List of mean false positive rates for ROC curve interpolation.
+                Defaults to np.linspace(0, 1, 100).
         """
         if not self.is_result_calculated:
             self.calculate_cv_result()
 
-        tprs = [result.tpr_list for result in self.fold_results]
-        aucs = [result.auc_list for result in self.fold_results]
-        mean_fpr = self.result.fpr_list
+        tpr_list = []
+        auc_list = []
+        for r in self.fold_results:
+            viz = RocCurveDisplay(fpr=r.fpr, tpr=r.tpr, roc_auc=r.auc)
+            interp_tpr = np.interp(mean_fpr, viz.fpr, viz.tpr)
+            interp_tpr[0] = 0.0
+            
+            tpr_list.append(interp_tpr)
+            auc_list.append(viz.roc_auc)
+        
+        tprs = np.array(tpr_list)
+        aucs = np.array(auc_list)
 
         ax.plot(
             [0, 1], [0, 1], linestyle="--", lw=2, color="r", label="Random", alpha=0.8
         )  # Plotting the random line
 
         mean_tpr = np.mean(tprs, axis=0)
         mean_tpr[-1] = 1.0
@@ -211,26 +210,22 @@
             xlim=[-0.05, 1.05],
             ylim=[-0.05, 1.05],
             title="Receiver operating characteristic",
         )
         ax.legend(loc="lower right")
 
 
-def evaluate_binary_classification(
-    y_test, y_predict, threshold, mean_fpr_list=np.linspace(0, 1, 100)
-):
+def evaluate_binary_classification(y_test, y_predict, threshold):
     """
     Calculate various evaluation metrics for binary classification predictions.
 
     Args:
         y_test (array-like): True labels of the test set.
         y_predict (array-like): Predicted labels of the test set.
         threshold (float): Threshold value for converting predicted probabilities to binary predictions.
-        mean_fpr_list (array-like, optional): List of mean false positive rates for ROC curve interpolation.
-            Defaults to np.linspace(0, 1, 100).
 
     Returns:
         Result: An object containing the calculated evaluation metrics.
 
     """
 
     result = Result()
@@ -252,18 +247,11 @@
         numerator, denominator, out=np.zeros_like(denominator), where=(denominator != 0)
     )
     result.max_f1 = np.max(f1_scores)
 
     # Calculate AUC, TPR, FPR
     fpr, tpr, _ = roc_curve(y_test, y_predict, pos_label=1)
     result.auc = auc(fpr, tpr)
-
-    # Calculate FPR, TPR and AUC Lists
-    viz = RocCurveDisplay(fpr=fpr, tpr=tpr, roc_auc=result.auc)
-    interp_tpr = np.interp(mean_fpr_list, viz.fpr, viz.tpr)
-    interp_tpr[0] = 0.0
-
-    result.mean_fpr_list = [mean_fpr_list]
-    result.tpr_list = [interp_tpr]
-    result.auc_list = [viz.roc_auc]
+    result.fpr = fpr
+    result.tpr = tpr
 
     return result
```

### Comparing `soma_integ-0.1.4/src/soma_integ/methods.py` & `soma_integ-0.1.5/src/soma_integ/methods.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.4/src/soma_integ/model.py` & `soma_integ-0.1.5/src/soma_integ/model.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.4/src/soma_integ/optimization.py` & `soma_integ-0.1.5/src/soma_integ/optimization.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.4/src/soma_integ.egg-info/PKG-INFO` & `soma_integ-0.1.5/src/soma_integ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.4
+Version: 0.1.5
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.4/tests/test_data.py` & `soma_integ-0.1.5/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.4/tests/test_evaluation.py` & `soma_integ-0.1.5/tests/test_evaluation.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,20 +52,20 @@
     assert cv_result.result.f1 == 0.7
     assert cv_result.result.auc == 0.875
 
 
 def test_cross_validation_result_get_roc_curve():
     cv_result = CrossValidationResult()
     fold_result1 = Result()
-    fold_result1.fpr_list = [0.1, 0.2, 0.3]
-    fold_result1.tpr_list = [0.4, 0.5, 0.6]
-    fold_result1.auc_list = [0.7]
+    fold_result1.fpr = np.array([0.1, 0.2, 0.3])
+    fold_result1.tpr = np.array([0.4, 0.5, 0.6])
+    fold_result1.auc = 0.7
     fold_result2 = Result()
-    fold_result2.fpr_list = [0.2, 0.3, 0.4]
-    fold_result2.tpr_list = [0.5, 0.6, 0.7]
-    fold_result2.auc_list = [0.8]
+    fold_result2.fpr = np.array([0.2, 0.3, 0.4])
+    fold_result2.tpr = np.array([0.5, 0.6, 0.7])
+    fold_result2.auc = 0.8
 
     cv_result.add_fold_result(fold_result1)
     cv_result.add_fold_result(fold_result2)
 
     ax = plt.subplot()
     cv_result.get_roc_curve(ax)
```

