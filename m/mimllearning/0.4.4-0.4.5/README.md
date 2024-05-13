# Comparing `tmp/mimllearning-0.4.4.tar.gz` & `tmp/mimllearning-0.4.5.tar.gz`

## Comparing `mimllearning-0.4.4.tar` & `mimllearning-0.4.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.4/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.4.4/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/data/__init__.py
--rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/data/bag.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/data/instance.py
--rw-r--r--   0        0        0    19564 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/dataset_utils.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/report/__init__.py
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0    16340 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/tutorial/miml_data.ipynb
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/tutorial/miml_transformations.ipynb
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/tutorial/mimltoml_classifiers.ipynb
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.4.4/.gitignore
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.4/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.5/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.4.5/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/data/__init__.py
+-rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/data/instance.py
+-rw-r--r--   0        0        0    19692 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/datasets/dataset_utils.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     8446 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0    16223 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/tutorial/miml_data.ipynb
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/tutorial/miml_transformations.ipynb
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.4.5/src/miml/tutorial/mimltoml_classifiers.ipynb
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.4.5/.gitignore
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.5/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.4.5/PKG-INFO
```

### Comparing `mimllearning-0.4.4/readme.md` & `mimllearning-0.4.5/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.4.5/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/classifier/miml_classifier.py` & `mimllearning-0.4.5/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.4.5/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,26 +24,40 @@
 
     def __init__(self) -> None:
         """
         Constructor of the class AllPositiveAPRClassifier
         """
         self.apr = []
 
-    def fit(self, x_train, y_train) -> None:
+    def fit(self, x_train: np.ndarray, y_train: np.ndarray) -> None:
         """
         Fit the classifier to the training data.
 
         Parameters
         ----------
         x_train : ndarray of shape (n_bags, n_instances, n_features)
             Features values of bags in the training set.
         y_train : ndarray (n_bags, n_instances, n_labels)
             Labels of bags in the training set.
         """
-        self.generate_apr(x_train, y_train)
+
+        positive_bag_indices = np.where(y_train == 1)[0]
+
+        # Select a random instance as starting apr
+        initial_bag_index = np.random.choice(positive_bag_indices)
+        initial_index_instance = np.random.choice(x_train[initial_bag_index].shape[0])
+        apr_min = apr_max = x_train[initial_bag_index][initial_index_instance]
+
+        # We check all positive instances and expand apr to minimum and maximum attribute values
+        for bag_index in positive_bag_indices:
+            for instance in x_train[bag_index]:
+                apr_min = np.minimum(apr_min, instance)
+                apr_max = np.maximum(apr_max, instance)
+
+        self.apr = [apr_min, apr_max]
 
     def predict(self, bag: np.array) -> int:
         """
         Predict the label of the bag
 
         Parameters
         ----------
@@ -52,14 +66,15 @@
 
         Returns
         -------
         label: int
             Predicted label of the bag
 
         """
+        # If all instances of the bag and all feature values inside of apr, it is a positive bag
         if np.all(bag >= self.apr[0]):
             if np.all(bag <= self.apr[1]):
                 return 1
         return 0
 
     def predict_proba(self, x: np.ndarray):
         """
@@ -76,31 +91,8 @@
             Predicted probabilities for given data
         """
         result = np.zeros(x.shape[0])
         for i in range(x.shape[0]):
             result[i] = self.predict(x[i])
         return result
 
-    def generate_apr(self, x_train, y_train) -> None:
-        """
-        Generate the axis-parallel rectangle
-
-        Parameters
-        ----------
-        x_train : np.ndarray of shape (n_bags, n_instances, n_features)
-            Features values of bags in the training set.
-        y_train : np.ndarray of shape    (n_bags, n_instances, n_features)
-            Labels of bags in the training set.
-        """
-
-        positive_bag_indices = np.where(y_train == 1)[0]
-
-        initial_bag_index = np.random.choice(positive_bag_indices)
-        initial_index_instance = np.random.choice(x_train[initial_bag_index].shape[0])
-        apr_min = apr_max = x_train[initial_bag_index][initial_index_instance]
-
-        for bag_index in positive_bag_indices:
-            for instance in x_train[bag_index]:
-                apr_min = np.minimum(apr_min, instance)
-                apr_max = np.maximum(apr_max, instance)
 
-        self.apr = [apr_min, apr_max]
```

### Comparing `mimllearning-0.4.4/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.4.5/src/miml/classifier/mi/apr_classifier.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,28 +29,28 @@
 
     def __init__(self) -> None:
         """
         Constructor of the class APRClassifier
         """
         self.classifier = mil.models.APR(verbose=0)
 
-    def fit(self, x_train, y_train) -> None:
+    def fit(self, x_train: np.ndarray, y_train: np.ndarray) -> None:
         """
         Fit the classifier to the training data.
 
         Parameters
         ----------
         x_train : ndarray of shape (n_bags, n_instances, n_features)
             Features values of bags in the training set.
         y_train : ndarray (n_bags, n_instances, n_labels)
             Labels of bags in the training set.
         """
         self.classifier.fit(x_train, y_train)
 
-    def predict(self, x) -> int:
+    def predict(self, x: np.ndarray) -> int:
         """
         Predict the label of the bag
 
         Parameters
         ----------
         x: np.ndarray of shape(n_instances, n_features)
             features values of a bag
```

### Comparing `mimllearning-0.4.4/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.4.5/src/miml/classifier/mi/miles_classifier.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         Constructor of the class MILESClassifier
         """
         self.classifier = mil.models.MILES()
         self.model = None
         self.mapping = None
         self.sigma2 = sigma2
 
-    def fit(self, x_train, y_train) -> None:
+    def fit(self, x_train: np.array, y_train: np.array) -> None:
         """
         Fit the classifier to the training data.
 
         Parameters
         ----------
         x_train : ndarray of shape (n_bags, n_instances, n_features)
             Features values of bags in the training set.
```

### Comparing `mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.4.5/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ...transformation import BinaryRelevanceTransformation
 from ...data import Bag
 from ...data import MIMLDataset
 
 
 class MIMLtoMIBRClassifier(MIMLtoMIClassifier):
     """
-    Class to represent a multi-instance classifier
+    Class to represent a multi-instance classifier using a binary relevance transformation
     """
 
     def __init__(self, classifier) -> None:
         """
         Constructor of the class MIMLtoMIBRClassifier
 
         Parameters
@@ -30,18 +30,21 @@
         Training the classifier
 
         Parameters
         ----------
         dataset_train: MIMLDataset
             Dataset to train the classifier
         """
+
+        # Create as many classifier as labels
         for x in range(dataset_train.get_number_labels()):
             classifier = deepcopy(self.classifier)
             self.classifiers.append(classifier)
 
+        # Obtain converted datasets and train each classifier
         datasets = self.transformation.transform_dataset(dataset_train)
         for i, dataset in enumerate(datasets):
             self.classifiers[i].fit(dataset.get_features_by_bag(), dataset.get_labels_by_bag())
 
         self.trained = True
 
     def predict(self, x: np.ndarray) -> np.ndarray:
```

### Comparing `mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.4.5/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py` & `mimllearning-0.4.5/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ...transformation import LabelPowersetTransformation
 from ...data import Bag
 from ...data import MIMLDataset
 
 
 class MIMLtoMILPClassifier(MIMLtoMIClassifier):
     """
-    Class to represent a multi-instance classifier
+    Class to represent a multi-instance classifier using a label powerset transformation
     """
 
     def __init__(self, classifier) -> None:
         """
         Constructor of the class MIMLtoMILPClassifier
 
         Parameters
```

### Comparing `mimllearning-0.4.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.4.5/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/data/bag.py` & `mimllearning-0.4.5/src/miml/data/bag.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/data/instance.py` & `mimllearning-0.4.5/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/data/miml_dataset.py` & `mimllearning-0.4.5/src/miml/data/miml_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         name : str
             Name of the dataset
         """
         self.name = name
 
     def get_name(self) -> str:
         """
-         Get function for dataset name
+        Get function for dataset name
 
         Returns
         ----------
         name : str
             Name of the dataset
         """
         return self.name
@@ -112,22 +112,29 @@
         Returns
         -------
         features: ndarray of shape (n_instances, n_features)
             Values of the features of the dataset
         """
         features = np.zeros((self.get_number_instances(), self.get_number_features()))
         count = 0
-        for key in self.data.keys():
+        for key in range(self.get_number_bags()):
             for instance in self.get_bag(key).get_features():
                 features[count] = instance
                 count += 1
         return features
 
     def get_features_by_bag(self) -> np.ndarray:
-        # TODO: Doc
+        """
+        Get features values of the dataset by bag
+
+        Returns
+        -------
+        features: ndarray of shape (n_bags, n_instances, n_features)
+            Values of the features of the dataset
+        """
         features = []
         for key in self.data.keys():
             features.append(self.get_bag(key).get_features())
         return np.array(features, dtype=object)
 
     def get_number_features(self) -> int:
         """
@@ -431,15 +438,14 @@
 
             mode : str
                 Mode to show the dataset. Modes available are "table" and "compact" (csv format)
 
             info: Boolean
                 Show more info
         """
-        # TODO: implement head and tail functionality from pandas, optional attributes list too
         if info:
             print("Name: ", self.get_name())
             print("Features: ", self.get_features_name())
             print("Labels: ", self.get_labels_name())
             print("Bags:")
 
         if end is None:
```

### Comparing `mimllearning-0.4.4/src/miml/datasets/dataset_utils.py` & `mimllearning-0.4.5/src/miml/datasets/dataset_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return load_dataset_csv(file)
     elif file[-5:] == ".arff":
         return load_dataset_arff(file)
     else:
         raise Exception("Filetype is not admitted. You should use an .arff or .csv file")
 
 
-def load_dataset_csv(file: str, header=0):
+def load_dataset_csv(file: str):
     """
     Function to load a dataset in csv format
 
     Parameters
     ----------
     file : str
         Path of the dataset file
@@ -149,30 +149,58 @@
                 else:
                     dataset.add_instance(key, instance)
 
     return dataset
 
 
 def load_toy():
-    # TODO: Doc
+    """
+    Load toy dataset from package
+
+    Returns
+    ----------
+    dataset : MIMLDataset
+        Dataset loaded
+    """
     return load_dataset(pkg_resources.resource_filename('miml', 'datasets/toy.arff'))
 
 
 def load_birds():
-    # TODO: Doc
+    """
+    Load birds dataset from package
+
+    Returns
+    ----------
+    dataset : MIMLDataset
+        Dataset loaded
+    """
     return load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds.arff'))
 
 
 def load_birds_train():
-    # TODO: Doc
+    """
+    Load a train partition of birds dataset from package
+
+    Returns
+    ----------
+    dataset : MIMLDataset
+        Dataset loaded
+    """
     return load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds_random_80train.arff'))
 
 
 def load_birds_test():
-    # TODO: Doc
+    """
+    Load a test partition of birds dataset from package
+
+    Returns
+    ----------
+    dataset : MIMLDataset
+        Dataset loaded
+    """
     return load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds_random_20test.arff'))
 
 
 def arff_to_csv(file: str) -> None:
     """
     Convert MIML Arff to CSV.
 
@@ -220,9 +248,7 @@
             labels = line[line.find(delimiter) + 2:]
 
             for v in values:
                 csv.write(key + "," + v + "," + labels + "\n")
 
     arff.close()
     csv.close()
-
-
```

### Comparing `mimllearning-0.4.4/src/miml/datasets/miml_birds.arff` & `mimllearning-0.4.5/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/datasets/miml_birds.csv` & `mimllearning-0.4.5/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.4.5/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.4.5/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/report/report.py` & `mimllearning-0.4.5/src/miml/report/report.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,17 @@
     """
     Class to generate a report
     """
 
     def __init__(self, classifier: MIMLClassifier, dataset_test: MIMLDataset, metrics: list[str] = None,
                  header: bool = True, per_label: bool = True):
 
+        """
+        Constructor of the class report
+        """
         self.dataset = dataset_test
         self.y_true = dataset_test.get_labels_by_bag()
         self.y_pred = classifier.evaluate(dataset_test)
         self.probs = classifier.predict_proba(dataset_test)
 
         all_metrics = ["precision-score-macro", "precision-score-micro", "average-precision-score-macro",
                        "average-precision-score-micro", "recall-score-macro", "recall-score-micro", "f1-score-macro",
@@ -37,14 +40,17 @@
                     raise Exception("Metric ", metric, "is not valid\n", "Metrics available: ", all_metrics)
         self.header = header
         self.metrics_name = metrics
         self.per_label = per_label
         self.metrics_value = dict()
 
     def calculate_metrics(self):
+        """
+        Calculate metrics of the predicted data
+        """
         self.metrics_value["precision-score-macro"] = precision_score(self.y_true, self.y_pred, average="macro",
                                                                       zero_division=0)
         self.metrics_value["precision-score-micro"] = precision_score(self.y_true, self.y_pred, average="micro",
                                                                       zero_division=0)
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=UserWarning)
             # When average_precision_score called raise this warming:
@@ -90,33 +96,56 @@
                 self.metrics_value["precision-score-" + label] = precision_score_per_label[i]
                 self.metrics_value["recall-score-" + label] = recall_score_per_label[i]
                 self.metrics_value["f1-score-" + label] = f1_score_per_label[i]
                 self.metrics_value["fbeta-score-" + label] = fbeta_score_per_label[i]
                 # self.metrics_value["roc-auc-score-"+label] = roc_auc_score_per_label[i]
                 self.metrics_value["jaccard-score-" + label] = jaccard_score_per_label[i]
 
-    def to_csv(self, path=None):
+    def to_csv(self, path: str = None):
+        """
+        Print/save data as csv format
+
+        Parameters
+        ----------
+        path : str, default=None
+            Path to csv where the data would be stored
+
+        """
         self.calculate_metrics()
         header = ""
         if self.header:
             header = ",".join(str(metric) for metric in self.metrics_name)
         values = ",".join(str(self.metrics_value[metric]) for metric in self.metrics_name)
         if path is None:
             print(header)
             print(values)
         else:
             with open(path, mode="a") as f:
                 f.write(header)
                 f.write(values)
 
     def to_string(self):
+        """
+        Print data as string format
+        """
         self.calculate_metrics()
         for metric in self.metrics_name:
             print(metric, ": ", self.metrics_value[metric])
 
 
 def hamming_score(y_true: np.ndarray, y_pred: np.ndarray):
+    """
+    Calculate hamming score of given data
+
+    Parameters
+    ----------
+    y_true : np.ndarray of shape (n_bags, n_labels)
+       Labels from the test dataset
+
+    y_pred : np.ndarray of shape (n_bags, n_labels)
+       Predicted labels from the test dataset
+    """
     numerator = (y_true & y_pred).sum(axis=1)
     denominator = (y_true | y_pred).sum(axis=1)
 
     return np.divide(numerator, denominator, out=np.ones_like(numerator, dtype=np.float_),
                      where=denominator != 0).mean()
```

### Comparing `mimllearning-0.4.4/src/miml/test/data_test.py` & `mimllearning-0.4.5/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.4.5/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/transformation/mimlTOmi/label_powerset_transformation.py` & `mimllearning-0.4.5/src/miml/transformation/mimlTOmi/label_powerset_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.4.5/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.4.5/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.4.5/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/tutorial/demo.ipynb` & `mimllearning-0.4.5/src/miml/tutorial/demo.ipynb`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9926344931912159%*

 * *Differences: {"'cells'": "{3: {'execution_count': 2, 'source': {insert: [(1, 'from miml.datasets import "*

 * *            'load_dataset, load_birds\\n\'), (3, "# dataset = '*

 * *            "load_dataset(pkg_resources.resource_filename('miml', "*

 * *            '\'datasets/miml_birds\'))\\n"), (4, \'dataset = load_birds()\\n\'), (5, \'\\n\'), (6, '*

 * *            "'dataset_train, dataset_test = dataset.split_dataset(0.8)')], delete: [6, 5, 4, 3, "*

 * *            "1]}}, 5: {'execution_count': 3}, 7: {'execution_count': 4}, 9: {'source': { […]*

```diff
@@ -30,41 +30,41 @@
             },
             "source": [
                 "# Loading of datasets"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 2,
             "metadata": {
                 "id": "L-_qkpnOxj_V"
             },
             "outputs": [],
             "source": [
                 "import pkg_resources\n",
-                "from miml.data.load_datasets import load_dataset, load_toy\n",
+                "from miml.datasets import load_dataset, load_birds\n",
+                "\n",
+                "# dataset = load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds'))\n",
+                "dataset = load_birds()\n",
                 "\n",
-                "dataset_train = load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds_random_80train.arff'),\n",
-                "                             delimiter=\"'\")\n",
-                "dataset_test = load_dataset(pkg_resources.resource_filename('miml', 'datasets/miml_birds_random_20test.arff'),\n",
-                "                            delimiter=\"'\")"
+                "dataset_train, dataset_test = dataset.split_dataset(0.8)"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "Rf5EX0HXEtZA"
             },
             "source": [
                 "# MIMLtoML Classifier"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 3,
             "metadata": {
                 "id": "c1OvYWW9Eyhw"
             },
             "outputs": [],
             "source": [
                 "from sklearn.neighbors import KNeighborsClassifier\n",
                 "from miml.transformation import ArithmeticTransformation\n",
@@ -81,15 +81,15 @@
             },
             "source": [
                 "# MIMLtoMI Classifier\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 4,
             "metadata": {
                 "id": "J7CxjYzK9jdX"
             },
             "outputs": [],
             "source": [
                 "from miml.classifier import MIMLtoMIBRClassifier, AllPositiveAPRClassifier\n",
                 "\n",
@@ -104,97 +104,97 @@
             },
             "source": [
                 "# Prediction of a bag"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 5,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "2oUifr2vxY8L",
-                "outputId": "4991b1ee-9a64-4bf7-c055-9b3dab1050cf"
+                "outputId": "d1d857de-8fa0-491c-ca55-f5f67c3defe2"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "MIMLtoML Classifier\n",
                         "-------------------\n",
                         "\n",
-                        "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n",
-                        "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 0. 0. 0. 0. 0.]]\n",
+                        "True Labels:        [0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0.]\n",
+                        "Predicted Labels:  [[0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 0. 0. 0.]]\n",
                         "\n",
                         "MIMLtoMI Classifier\n",
                         "-------------------\n",
                         "\n",
-                        "True Labels:       [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0. 1. 0. 0. 0. 0. 0.]\n",
-                        "Predicted Labels:  [0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 1. 0. 0. 0. 0. 0. 0. 0. 0.]\n"
+                        "True Labels:       [0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 1. 0. 0. 0.]\n",
+                        "Predicted Labels:  [0. 1. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0. 0.]\n"
                     ]
                 }
             ],
             "source": [
                 "print(\"MIMLtoML Classifier\")\n",
                 "print(\"-------------------\")\n",
                 "print(\"\")\n",
-                "print(\"True Labels:       \", dataset_test.get_bag(\"366\").get_labels()[0])\n",
-                "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"366\")))\n",
+                "print(\"True Labels:       \", dataset_test.get_bag(\"254\").get_labels()[0])\n",
+                "print(\"Predicted Labels: \", classifier_ml.predict_bag(dataset_test.get_bag(\"254\")))\n",
                 "print(\"\")\n",
                 "print(\"MIMLtoMI Classifier\")\n",
                 "print(\"-------------------\")\n",
                 "print(\"\")\n",
-                "print(\"True Labels:      \", dataset_test.get_bag(\"366\").get_labels()[0])\n",
-                "print(\"Predicted Labels: \", classifier_mi.predict_bag(dataset_test.get_bag(\"366\")))"
+                "print(\"True Labels:      \", dataset_test.get_bag(\"254\").get_labels()[0])\n",
+                "print(\"Predicted Labels: \", classifier_mi.predict_bag(dataset_test.get_bag(\"254\")))"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {
                 "id": "3Ns-WjntvZEH"
             },
             "source": [
                 "#  Report ML\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 6,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "ysIgN-dkvc8r",
-                "outputId": "5d5423de-c417-451a-8be1-2e3a4cab5559"
+                "outputId": "f53bc618-971a-4bf6-9cd7-5797dfb505b1"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "precision-score-macro :  0.15994152046783625\n",
-                        "precision-score-micro :  0.2647058823529412\n",
-                        "average-precision-score-macro :  0.14935540515371115\n",
-                        "average-precision-score-micro :  0.19872173297119117\n",
-                        "recall-score-macro :  0.04923706324635117\n",
-                        "recall-score-micro :  0.09\n",
-                        "f1-score-macro :  0.06413078149920254\n",
-                        "f1-score-micro :  0.13432835820895522\n",
-                        "fbeta-score-macro :  0.06413078149920254\n",
-                        "fbeta-score-micro :  0.13432835820895522\n",
-                        "accuracy-score :  0.057692307692307696\n",
-                        "hamming-loss :  0.11740890688259109\n",
-                        "jaccard-score-macro :  0.03588039217329836\n",
-                        "jaccard-score-micro :  0.072\n",
-                        "log-loss :  24.54438872787161\n",
+                        "precision-score-macro :  0.11025641025641027\n",
+                        "precision-score-micro :  0.3548387096774194\n",
+                        "average-precision-score-macro :  0.18543572591101495\n",
+                        "average-precision-score-micro :  0.21535397464607572\n",
+                        "recall-score-macro :  0.044037232117727476\n",
+                        "recall-score-micro :  0.10185185185185185\n",
+                        "f1-score-macro :  0.054704944178628395\n",
+                        "f1-score-micro :  0.15827338129496402\n",
+                        "fbeta-score-macro :  0.06945975659091401\n",
+                        "fbeta-score-micro :  0.2370689655172414\n",
+                        "subset-accuracy-score :  0.058823529411764705\n",
+                        "hamming-loss :  0.12074303405572756\n",
+                        "jaccard-score-macro :  0.03210078625591091\n",
+                        "jaccard-score-micro :  0.0859375\n",
+                        "log-loss :  30.660915561748453\n",
                         "\n",
-                        "precision-score-macro,precision-score-micro,average-precision-score-macro,average-precision-score-micro,recall-score-macro,recall-score-micro,f1-score-macro,f1-score-micro,fbeta-score-macro,fbeta-score-micro,accuracy-score,hamming-loss,jaccard-score-macro,jaccard-score-micro,log-loss\n",
-                        "0.15994152046783625,0.2647058823529412,0.14935540515371115,0.19872173297119117,0.04923706324635117,0.09,0.06413078149920254,0.13432835820895522,0.06413078149920254,0.13432835820895522,0.057692307692307696,0.11740890688259109,0.03588039217329836,0.072,24.54438872787161\n"
+                        "precision-score-macro,precision-score-micro,average-precision-score-macro,average-precision-score-micro,recall-score-macro,recall-score-micro,f1-score-macro,f1-score-micro,fbeta-score-macro,fbeta-score-micro,subset-accuracy-score,hamming-loss,jaccard-score-macro,jaccard-score-micro,log-loss\n",
+                        "0.11025641025641027,0.3548387096774194,0.18543572591101495,0.21535397464607572,0.044037232117727476,0.10185185185185185,0.054704944178628395,0.15827338129496402,0.06945975659091401,0.2370689655172414,0.058823529411764705,0.12074303405572756,0.03210078625591091,0.0859375,30.660915561748453\n"
                     ]
                 }
             ],
             "source": [
                 "from miml.report import Report\n",
                 "\n",
                 "report = Report(classifier_ml, dataset_test, per_label=False)\n",
@@ -210,140 +210,140 @@
             },
             "source": [
                 "# Report MI"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 12,
+            "execution_count": 7,
             "metadata": {
                 "colab": {
                     "base_uri": "https://localhost:8080/"
                 },
                 "id": "_blawc4pZWuH",
-                "outputId": "1153b4a3-1c83-4dff-dbe0-88b3cdce6797"
+                "outputId": "a7b9c0e5-6fcf-473f-94da-3623266addb0"
             },
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "precision-score-macro :  0.1303731663842467\n",
-                        "precision-score-micro :  0.22485207100591717\n",
-                        "average-precision-score-macro :  0.12150756876844539\n",
-                        "average-precision-score-micro :  0.14819682341949547\n",
-                        "recall-score-macro :  0.25229986731534715\n",
-                        "recall-score-micro :  0.38\n",
-                        "f1-score-macro :  0.16567017223361705\n",
-                        "f1-score-micro :  0.2825278810408922\n",
-                        "fbeta-score-macro :  0.16567017223361705\n",
-                        "fbeta-score-micro :  0.2825278810408922\n",
-                        "accuracy-score :  0.019230769230769232\n",
-                        "hamming-loss :  0.19534412955465588\n",
-                        "jaccard-score-macro :  0.09851845957380101\n",
-                        "jaccard-score-micro :  0.1645021645021645\n",
-                        "log-loss :  24.234665595432148\n",
+                        "precision-score-macro :  0.16599026450285032\n",
+                        "precision-score-micro :  0.208955223880597\n",
+                        "average-precision-score-macro :  0.13233912181953641\n",
+                        "average-precision-score-micro :  0.13673291608692004\n",
+                        "recall-score-macro :  0.15933416428772468\n",
+                        "recall-score-micro :  0.25925925925925924\n",
+                        "f1-score-macro :  0.14296150593201268\n",
+                        "f1-score-micro :  0.23140495867768596\n",
+                        "fbeta-score-macro :  0.14634518676605035\n",
+                        "fbeta-score-micro :  0.2173913043478261\n",
+                        "subset-accuracy-score :  0.0196078431372549\n",
+                        "hamming-loss :  0.19195046439628483\n",
+                        "jaccard-score-macro :  0.08445809323477566\n",
+                        "jaccard-score-micro :  0.1308411214953271\n",
+                        "log-loss :  23.432988277126885\n",
                         "precision-score-BRCR :  0.0\n",
-                        "precision-score-PAWR :  0.4\n",
-                        "precision-score-PSFL :  0.07692307692307693\n",
+                        "precision-score-PAWR :  0.3333333333333333\n",
+                        "precision-score-PSFL :  0.23076923076923078\n",
                         "precision-score-RBNU :  0.0\n",
-                        "precision-score-DEJU :  0.14285714285714285\n",
-                        "precision-score-OSFL :  0.0\n",
-                        "precision-score-HETH :  0.13333333333333333\n",
-                        "precision-score-CBCH :  0.2222222222222222\n",
-                        "precision-score-VATH :  0.2777777777777778\n",
-                        "precision-score-HEWA :  0.21052631578947367\n",
-                        "precision-score-SWTH :  0.3\n",
+                        "precision-score-DEJU :  0.0\n",
+                        "precision-score-OSFL :  1.0\n",
+                        "precision-score-HETH :  0.2857142857142857\n",
+                        "precision-score-CBCH :  0.0\n",
+                        "precision-score-VATH :  0.07692307692307693\n",
+                        "precision-score-HEWA :  0.3\n",
+                        "precision-score-SWTH :  0.30434782608695654\n",
                         "precision-score-HAFL :  0.0\n",
-                        "precision-score-WETA :  0.2222222222222222\n",
+                        "precision-score-WETA :  0.2727272727272727\n",
                         "precision-score-BHGB :  0.0\n",
-                        "precision-score-GCKI :  0.15789473684210525\n",
+                        "precision-score-GCKI :  0.1\n",
                         "precision-score-WAVI :  0.0\n",
                         "precision-score-MGWA :  0.0\n",
                         "precision-score-STJA :  0.0\n",
-                        "precision-score-CONI :  0.3333333333333333\n",
+                        "precision-score-CONI :  0.25\n",
                         "recall-score-BRCR :  0.0\n",
                         "recall-score-PAWR :  0.5\n",
-                        "recall-score-PSFL :  0.25\n",
+                        "recall-score-PSFL :  0.42857142857142855\n",
                         "recall-score-RBNU :  0.0\n",
-                        "recall-score-DEJU :  0.5\n",
-                        "recall-score-OSFL :  0.0\n",
-                        "recall-score-HETH :  0.4\n",
-                        "recall-score-CBCH :  0.2857142857142857\n",
-                        "recall-score-VATH :  0.5\n",
-                        "recall-score-HEWA :  0.4\n",
-                        "recall-score-SWTH :  0.5294117647058824\n",
+                        "recall-score-DEJU :  0.0\n",
+                        "recall-score-OSFL :  0.2\n",
+                        "recall-score-HETH :  0.16666666666666666\n",
+                        "recall-score-CBCH :  0.0\n",
+                        "recall-score-VATH :  0.14285714285714285\n",
+                        "recall-score-HEWA :  0.2727272727272727\n",
+                        "recall-score-SWTH :  0.4117647058823529\n",
                         "recall-score-HAFL :  0.0\n",
-                        "recall-score-WETA :  0.6666666666666666\n",
+                        "recall-score-WETA :  0.42857142857142855\n",
                         "recall-score-BHGB :  0.0\n",
-                        "recall-score-GCKI :  0.42857142857142855\n",
+                        "recall-score-GCKI :  0.14285714285714285\n",
                         "recall-score-WAVI :  0.0\n",
                         "recall-score-MGWA :  0.0\n",
                         "recall-score-STJA :  0.0\n",
                         "recall-score-CONI :  0.3333333333333333\n",
                         "f1-score-BRCR :  0.0\n",
-                        "f1-score-PAWR :  0.4444444444444445\n",
-                        "f1-score-PSFL :  0.11764705882352941\n",
+                        "f1-score-PAWR :  0.4\n",
+                        "f1-score-PSFL :  0.3\n",
                         "f1-score-RBNU :  0.0\n",
-                        "f1-score-DEJU :  0.22222222222222224\n",
-                        "f1-score-OSFL :  0.0\n",
-                        "f1-score-HETH :  0.2\n",
-                        "f1-score-CBCH :  0.25\n",
-                        "f1-score-VATH :  0.35714285714285715\n",
-                        "f1-score-HEWA :  0.27586206896551724\n",
-                        "f1-score-SWTH :  0.3829787234042553\n",
+                        "f1-score-DEJU :  0.0\n",
+                        "f1-score-OSFL :  0.33333333333333337\n",
+                        "f1-score-HETH :  0.2105263157894737\n",
+                        "f1-score-CBCH :  0.0\n",
+                        "f1-score-VATH :  0.1\n",
+                        "f1-score-HEWA :  0.28571428571428564\n",
+                        "f1-score-SWTH :  0.35\n",
                         "f1-score-HAFL :  0.0\n",
-                        "f1-score-WETA :  0.3333333333333333\n",
+                        "f1-score-WETA :  0.33333333333333326\n",
                         "f1-score-BHGB :  0.0\n",
-                        "f1-score-GCKI :  0.23076923076923078\n",
+                        "f1-score-GCKI :  0.11764705882352941\n",
                         "f1-score-WAVI :  0.0\n",
                         "f1-score-MGWA :  0.0\n",
                         "f1-score-STJA :  0.0\n",
-                        "f1-score-CONI :  0.3333333333333333\n",
+                        "f1-score-CONI :  0.28571428571428575\n",
                         "fbeta-score-BRCR :  0.0\n",
-                        "fbeta-score-PAWR :  0.4444444444444445\n",
-                        "fbeta-score-PSFL :  0.11764705882352941\n",
+                        "fbeta-score-PAWR :  0.3571428571428571\n",
+                        "fbeta-score-PSFL :  0.2542372881355932\n",
                         "fbeta-score-RBNU :  0.0\n",
-                        "fbeta-score-DEJU :  0.22222222222222224\n",
-                        "fbeta-score-OSFL :  0.0\n",
-                        "fbeta-score-HETH :  0.2\n",
-                        "fbeta-score-CBCH :  0.25\n",
-                        "fbeta-score-VATH :  0.35714285714285715\n",
-                        "fbeta-score-HEWA :  0.27586206896551724\n",
-                        "fbeta-score-SWTH :  0.3829787234042553\n",
+                        "fbeta-score-DEJU :  0.0\n",
+                        "fbeta-score-OSFL :  0.5555555555555556\n",
+                        "fbeta-score-HETH :  0.24999999999999997\n",
+                        "fbeta-score-CBCH :  0.0\n",
+                        "fbeta-score-VATH :  0.08474576271186442\n",
+                        "fbeta-score-HEWA :  0.29411764705882354\n",
+                        "fbeta-score-SWTH :  0.3211009174311927\n",
                         "fbeta-score-HAFL :  0.0\n",
-                        "fbeta-score-WETA :  0.3333333333333333\n",
+                        "fbeta-score-WETA :  0.29411764705882354\n",
                         "fbeta-score-BHGB :  0.0\n",
-                        "fbeta-score-GCKI :  0.23076923076923078\n",
+                        "fbeta-score-GCKI :  0.10638297872340426\n",
                         "fbeta-score-WAVI :  0.0\n",
                         "fbeta-score-MGWA :  0.0\n",
                         "fbeta-score-STJA :  0.0\n",
-                        "fbeta-score-CONI :  0.3333333333333333\n",
+                        "fbeta-score-CONI :  0.2631578947368421\n",
                         "jaccard-score-BRCR :  0.0\n",
-                        "jaccard-score-PAWR :  0.2857142857142857\n",
-                        "jaccard-score-PSFL :  0.0625\n",
+                        "jaccard-score-PAWR :  0.25\n",
+                        "jaccard-score-PSFL :  0.17647058823529413\n",
                         "jaccard-score-RBNU :  0.0\n",
-                        "jaccard-score-DEJU :  0.125\n",
-                        "jaccard-score-OSFL :  0.0\n",
-                        "jaccard-score-HETH :  0.1111111111111111\n",
-                        "jaccard-score-CBCH :  0.14285714285714285\n",
-                        "jaccard-score-VATH :  0.21739130434782608\n",
-                        "jaccard-score-HEWA :  0.16\n",
-                        "jaccard-score-SWTH :  0.23684210526315788\n",
+                        "jaccard-score-DEJU :  0.0\n",
+                        "jaccard-score-OSFL :  0.2\n",
+                        "jaccard-score-HETH :  0.11764705882352941\n",
+                        "jaccard-score-CBCH :  0.0\n",
+                        "jaccard-score-VATH :  0.05263157894736842\n",
+                        "jaccard-score-HEWA :  0.16666666666666666\n",
+                        "jaccard-score-SWTH :  0.21212121212121213\n",
                         "jaccard-score-HAFL :  0.0\n",
                         "jaccard-score-WETA :  0.2\n",
                         "jaccard-score-BHGB :  0.0\n",
-                        "jaccard-score-GCKI :  0.13043478260869565\n",
+                        "jaccard-score-GCKI :  0.0625\n",
                         "jaccard-score-WAVI :  0.0\n",
                         "jaccard-score-MGWA :  0.0\n",
                         "jaccard-score-STJA :  0.0\n",
-                        "jaccard-score-CONI :  0.2\n",
+                        "jaccard-score-CONI :  0.16666666666666666\n",
                         "\n",
-                        "precision-score-macro,precision-score-micro,average-precision-score-macro,average-precision-score-micro,recall-score-macro,recall-score-micro,f1-score-macro,f1-score-micro,fbeta-score-macro,fbeta-score-micro,accuracy-score,hamming-loss,jaccard-score-macro,jaccard-score-micro,log-loss,precision-score-BRCR,precision-score-PAWR,precision-score-PSFL,precision-score-RBNU,precision-score-DEJU,precision-score-OSFL,precision-score-HETH,precision-score-CBCH,precision-score-VATH,precision-score-HEWA,precision-score-SWTH,precision-score-HAFL,precision-score-WETA,precision-score-BHGB,precision-score-GCKI,precision-score-WAVI,precision-score-MGWA,precision-score-STJA,precision-score-CONI,recall-score-BRCR,recall-score-PAWR,recall-score-PSFL,recall-score-RBNU,recall-score-DEJU,recall-score-OSFL,recall-score-HETH,recall-score-CBCH,recall-score-VATH,recall-score-HEWA,recall-score-SWTH,recall-score-HAFL,recall-score-WETA,recall-score-BHGB,recall-score-GCKI,recall-score-WAVI,recall-score-MGWA,recall-score-STJA,recall-score-CONI,f1-score-BRCR,f1-score-PAWR,f1-score-PSFL,f1-score-RBNU,f1-score-DEJU,f1-score-OSFL,f1-score-HETH,f1-score-CBCH,f1-score-VATH,f1-score-HEWA,f1-score-SWTH,f1-score-HAFL,f1-score-WETA,f1-score-BHGB,f1-score-GCKI,f1-score-WAVI,f1-score-MGWA,f1-score-STJA,f1-score-CONI,fbeta-score-BRCR,fbeta-score-PAWR,fbeta-score-PSFL,fbeta-score-RBNU,fbeta-score-DEJU,fbeta-score-OSFL,fbeta-score-HETH,fbeta-score-CBCH,fbeta-score-VATH,fbeta-score-HEWA,fbeta-score-SWTH,fbeta-score-HAFL,fbeta-score-WETA,fbeta-score-BHGB,fbeta-score-GCKI,fbeta-score-WAVI,fbeta-score-MGWA,fbeta-score-STJA,fbeta-score-CONI,jaccard-score-BRCR,jaccard-score-PAWR,jaccard-score-PSFL,jaccard-score-RBNU,jaccard-score-DEJU,jaccard-score-OSFL,jaccard-score-HETH,jaccard-score-CBCH,jaccard-score-VATH,jaccard-score-HEWA,jaccard-score-SWTH,jaccard-score-HAFL,jaccard-score-WETA,jaccard-score-BHGB,jaccard-score-GCKI,jaccard-score-WAVI,jaccard-score-MGWA,jaccard-score-STJA,jaccard-score-CONI\n",
-                        "0.1303731663842467,0.22485207100591717,0.12150756876844539,0.14819682341949547,0.25229986731534715,0.38,0.16567017223361705,0.2825278810408922,0.16567017223361705,0.2825278810408922,0.019230769230769232,0.19534412955465588,0.09851845957380101,0.1645021645021645,24.234665595432148,0.0,0.4,0.07692307692307693,0.0,0.14285714285714285,0.0,0.13333333333333333,0.2222222222222222,0.2777777777777778,0.21052631578947367,0.3,0.0,0.2222222222222222,0.0,0.15789473684210525,0.0,0.0,0.0,0.3333333333333333,0.0,0.5,0.25,0.0,0.5,0.0,0.4,0.2857142857142857,0.5,0.4,0.5294117647058824,0.0,0.6666666666666666,0.0,0.42857142857142855,0.0,0.0,0.0,0.3333333333333333,0.0,0.4444444444444445,0.11764705882352941,0.0,0.22222222222222224,0.0,0.2,0.25,0.35714285714285715,0.27586206896551724,0.3829787234042553,0.0,0.3333333333333333,0.0,0.23076923076923078,0.0,0.0,0.0,0.3333333333333333,0.0,0.4444444444444445,0.11764705882352941,0.0,0.22222222222222224,0.0,0.2,0.25,0.35714285714285715,0.27586206896551724,0.3829787234042553,0.0,0.3333333333333333,0.0,0.23076923076923078,0.0,0.0,0.0,0.3333333333333333,0.0,0.2857142857142857,0.0625,0.0,0.125,0.0,0.1111111111111111,0.14285714285714285,0.21739130434782608,0.16,0.23684210526315788,0.0,0.2,0.0,0.13043478260869565,0.0,0.0,0.0,0.2\n"
+                        "precision-score-macro,precision-score-micro,average-precision-score-macro,average-precision-score-micro,recall-score-macro,recall-score-micro,f1-score-macro,f1-score-micro,fbeta-score-macro,fbeta-score-micro,subset-accuracy-score,hamming-loss,jaccard-score-macro,jaccard-score-micro,log-loss,precision-score-BRCR,precision-score-PAWR,precision-score-PSFL,precision-score-RBNU,precision-score-DEJU,precision-score-OSFL,precision-score-HETH,precision-score-CBCH,precision-score-VATH,precision-score-HEWA,precision-score-SWTH,precision-score-HAFL,precision-score-WETA,precision-score-BHGB,precision-score-GCKI,precision-score-WAVI,precision-score-MGWA,precision-score-STJA,precision-score-CONI,recall-score-BRCR,recall-score-PAWR,recall-score-PSFL,recall-score-RBNU,recall-score-DEJU,recall-score-OSFL,recall-score-HETH,recall-score-CBCH,recall-score-VATH,recall-score-HEWA,recall-score-SWTH,recall-score-HAFL,recall-score-WETA,recall-score-BHGB,recall-score-GCKI,recall-score-WAVI,recall-score-MGWA,recall-score-STJA,recall-score-CONI,f1-score-BRCR,f1-score-PAWR,f1-score-PSFL,f1-score-RBNU,f1-score-DEJU,f1-score-OSFL,f1-score-HETH,f1-score-CBCH,f1-score-VATH,f1-score-HEWA,f1-score-SWTH,f1-score-HAFL,f1-score-WETA,f1-score-BHGB,f1-score-GCKI,f1-score-WAVI,f1-score-MGWA,f1-score-STJA,f1-score-CONI,fbeta-score-BRCR,fbeta-score-PAWR,fbeta-score-PSFL,fbeta-score-RBNU,fbeta-score-DEJU,fbeta-score-OSFL,fbeta-score-HETH,fbeta-score-CBCH,fbeta-score-VATH,fbeta-score-HEWA,fbeta-score-SWTH,fbeta-score-HAFL,fbeta-score-WETA,fbeta-score-BHGB,fbeta-score-GCKI,fbeta-score-WAVI,fbeta-score-MGWA,fbeta-score-STJA,fbeta-score-CONI,jaccard-score-BRCR,jaccard-score-PAWR,jaccard-score-PSFL,jaccard-score-RBNU,jaccard-score-DEJU,jaccard-score-OSFL,jaccard-score-HETH,jaccard-score-CBCH,jaccard-score-VATH,jaccard-score-HEWA,jaccard-score-SWTH,jaccard-score-HAFL,jaccard-score-WETA,jaccard-score-BHGB,jaccard-score-GCKI,jaccard-score-WAVI,jaccard-score-MGWA,jaccard-score-STJA,jaccard-score-CONI\n",
+                        "0.16599026450285032,0.208955223880597,0.13233912181953641,0.13673291608692004,0.15933416428772468,0.25925925925925924,0.14296150593201268,0.23140495867768596,0.14634518676605035,0.2173913043478261,0.0196078431372549,0.19195046439628483,0.08445809323477566,0.1308411214953271,23.432988277126885,0.0,0.3333333333333333,0.23076923076923078,0.0,0.0,1.0,0.2857142857142857,0.0,0.07692307692307693,0.3,0.30434782608695654,0.0,0.2727272727272727,0.0,0.1,0.0,0.0,0.0,0.25,0.0,0.5,0.42857142857142855,0.0,0.0,0.2,0.16666666666666666,0.0,0.14285714285714285,0.2727272727272727,0.4117647058823529,0.0,0.42857142857142855,0.0,0.14285714285714285,0.0,0.0,0.0,0.3333333333333333,0.0,0.4,0.3,0.0,0.0,0.33333333333333337,0.2105263157894737,0.0,0.1,0.28571428571428564,0.35,0.0,0.33333333333333326,0.0,0.11764705882352941,0.0,0.0,0.0,0.28571428571428575,0.0,0.3571428571428571,0.2542372881355932,0.0,0.0,0.5555555555555556,0.24999999999999997,0.0,0.08474576271186442,0.29411764705882354,0.3211009174311927,0.0,0.29411764705882354,0.0,0.10638297872340426,0.0,0.0,0.0,0.2631578947368421,0.0,0.25,0.17647058823529413,0.0,0.0,0.2,0.11764705882352941,0.0,0.05263157894736842,0.16666666666666666,0.21212121212121213,0.0,0.2,0.0,0.0625,0.0,0.0,0.0,0.16666666666666666\n"
                     ]
                 }
             ],
             "source": [
                 "report = Report(classifier_mi, dataset_test)\n",
                 "report.to_string()\n",
                 "print(\"\")\n",
```

### Comparing `mimllearning-0.4.4/src/miml/tutorial/miml_data.ipynb` & `mimllearning-0.4.5/src/miml/tutorial/miml_data.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/tutorial/miml_transformations.ipynb` & `mimllearning-0.4.5/src/miml/tutorial/miml_transformations.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/src/miml/tutorial/mimltoml_classifiers.ipynb` & `mimllearning-0.4.5/src/miml/tutorial/mimltoml_classifiers.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/README.md` & `mimllearning-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.4/pyproject.toml` & `mimllearning-0.4.5/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 requires = ["hatchling", "pkginfo >= 1.10"]
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/miml", "src/miml/*"]
 
 [metadata]
-version = "0.4.4"
+version = "0.4.5"
 name = "mimllearning"
 
 [project]
 name = "mimllearning"
-version = "0.4.4"
+version = "0.4.5"
 authors = [
   { name="Damian Martinez", email="damianmartinezavila@gmail.com" },
 ]
 description = "MIML Learning Library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `mimllearning-0.4.4/PKG-INFO` & `mimllearning-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.4.4
+Version: 0.4.5
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

