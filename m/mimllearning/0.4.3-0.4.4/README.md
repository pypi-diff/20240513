# Comparing `tmp/mimllearning-0.4.3.tar.gz` & `tmp/mimllearning-0.4.4.tar.gz`

## Comparing `mimllearning-0.4.3.tar` & `mimllearning-0.4.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.3/readme.md
--rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.4.3/documentation/AnteproyectoDamianTFG.pdf
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/__init__.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/miml_classifier.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/mi/__init__.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/mi/all_positive_apr_classifier.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/mi/apr_classifier.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/mi/miles_classifier.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/mimlTOml/__init__.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/data/__init__.py
--rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/data/bag.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/data/instance.py
--rw-r--r--   0        0        0    19553 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/data/miml_dataset.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/datasets/__init__.py
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/datasets/dataset_utils.py
--rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/datasets/miml_birds.arff
--rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/datasets/miml_birds.csv
--rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/datasets/miml_birds_random_20test.arff
--rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/datasets/miml_birds_random_80train.arff
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/datasets/toy.arff
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/report/__init__.py
--rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/report/report.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/test/data_test.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/transformation/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/transformation/mimlTOmi/__init__.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/transformation/mimlTOml/__init__.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/transformation/mimlTOml/arithmetic.py
--rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/transformation/mimlTOml/geometric.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
--rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/transformation/mimlTOml/minmax.py
--rw-r--r--   0        0        0    16340 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/tutorial/demo.ipynb
--rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/tutorial/miml_data.ipynb
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/tutorial/miml_transformations.ipynb
--rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.4.3/src/miml/tutorial/mimltoml_classifiers.ipynb
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.4.3/.gitignore
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.3/README.md
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.4/readme.md
+-rw-r--r--   0        0        0   258069 2020-02-02 00:00:00.000000 mimllearning-0.4.4/documentation/AnteproyectoDamianTFG.pdf
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/__init__.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/miml_classifier.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mi/__init__.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mi/all_positive_apr_classifier.py
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mi/apr_classifier.py
+-rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mi/miles_classifier.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2949 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/data/__init__.py
+-rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/data/bag.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/data/instance.py
+-rw-r--r--   0        0        0    19564 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/data/miml_dataset.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/__init__.py
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/dataset_utils.py
+-rw-r--r--   0        0        0   735908 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/miml_birds.arff
+-rw-r--r--   0        0        0   842801 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/miml_birds.csv
+-rw-r--r--   0        0        0   134841 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/miml_birds_random_20test.arff
+-rw-r--r--   0        0        0   498562 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/miml_birds_random_80train.arff
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/datasets/toy.arff
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/report/__init__.py
+-rw-r--r--   0        0        0     7748 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/report/report.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/test/data_test.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOmi/__init__.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOmi/label_powerset_transformation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOml/__init__.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOml/arithmetic.py
+-rw-r--r--   0        0        0     2574 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOml/geometric.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOml/miml_to_ml_transformation.py
+-rw-r--r--   0        0        0     3035 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/transformation/mimlTOml/minmax.py
+-rw-r--r--   0        0        0    16340 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/tutorial/demo.ipynb
+-rw-r--r--   0        0        0     6394 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/tutorial/miml_data.ipynb
+-rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/tutorial/miml_transformations.ipynb
+-rw-r--r--   0        0        0    11077 2020-02-02 00:00:00.000000 mimllearning-0.4.4/src/miml/tutorial/mimltoml_classifiers.ipynb
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 mimllearning-0.4.4/.gitignore
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 mimllearning-0.4.4/README.md
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mimllearning-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 mimllearning-0.4.4/PKG-INFO
```

### Comparing `mimllearning-0.4.3/readme.md` & `mimllearning-0.4.4/readme.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/documentation/AnteproyectoDamianTFG.pdf` & `mimllearning-0.4.4/documentation/AnteproyectoDamianTFG.pdf`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/classifier/miml_classifier.py` & `mimllearning-0.4.4/src/miml/classifier/miml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/classifier/mi/all_positive_apr_classifier.py` & `mimllearning-0.4.4/src/miml/classifier/mi/all_positive_apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/classifier/mi/apr_classifier.py` & `mimllearning-0.4.4/src/miml/classifier/mi/apr_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/classifier/mi/miles_classifier.py` & `mimllearning-0.4.4/src/miml/classifier/mi/miles_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py` & `mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_br_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py` & `mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py` & `mimllearning-0.4.4/src/miml/classifier/mimlTOmi/miml_to_mi_lp_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py` & `mimllearning-0.4.4/src/miml/classifier/mimlTOml/miml_to_ml_classifier.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/data/bag.py` & `mimllearning-0.4.4/src/miml/data/bag.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,19 +303,17 @@
 
         mode : str
             Mode to show the bag. Modes available are "table" and "compact" (csv format)
         attributes : list[str]
             List of attributes to display. If empty, all attributes will be displayed.
         """
         header = [self.key]
-        print("end: ", end)
+
         if end is None:
-            print("entro")
             end = self.get_number_instances()
-            print("end: ", end)
 
         if not attributes:
             header += [""] * self.get_number_attributes()
             if self.dataset is not None:
                 header = [self.key] + self.get_features_name() + self.get_labels_name()
         else:
             header = [self.key] + attributes
```

### Comparing `mimllearning-0.4.3/src/miml/data/instance.py` & `mimllearning-0.4.4/src/miml/data/instance.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/data/miml_dataset.py` & `mimllearning-0.4.4/src/miml/data/miml_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,15 +444,15 @@
 
         if end is None:
             end = self.get_number_bags()
 
         if mode == "table":
             for bag_index in range(start, end):
                 bag = self.get_bag(bag_index)
-                bag.show_bag(attributes)
+                bag.show_bag(attributes=attributes)
 
         elif mode == "compact":
             header = ["bag_id"] + self.get_features_name() + self.get_labels_name()
             if attributes:
                 header = ["bag_id"] + attributes
             print(", ".join(header))
             for bag_index in range(start, end):
```

### Comparing `mimllearning-0.4.3/src/miml/datasets/dataset_utils.py` & `mimllearning-0.4.4/src/miml/datasets/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/datasets/miml_birds.arff` & `mimllearning-0.4.4/src/miml/datasets/miml_birds.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/datasets/miml_birds.csv` & `mimllearning-0.4.4/src/miml/datasets/miml_birds.csv`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/datasets/miml_birds_random_20test.arff` & `mimllearning-0.4.4/src/miml/datasets/miml_birds_random_20test.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/datasets/miml_birds_random_80train.arff` & `mimllearning-0.4.4/src/miml/datasets/miml_birds_random_80train.arff`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/report/report.py` & `mimllearning-0.4.4/src/miml/report/report.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/test/data_test.py` & `mimllearning-0.4.4/src/miml/test/data_test.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py` & `mimllearning-0.4.4/src/miml/transformation/mimlTOmi/binary_relevance_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/transformation/mimlTOmi/label_powerset_transformation.py` & `mimllearning-0.4.4/src/miml/transformation/mimlTOmi/label_powerset_transformation.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/transformation/mimlTOml/arithmetic.py` & `mimllearning-0.4.4/src/miml/transformation/mimlTOml/arithmetic.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/transformation/mimlTOml/geometric.py` & `mimllearning-0.4.4/src/miml/transformation/mimlTOml/geometric.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/transformation/mimlTOml/minmax.py` & `mimllearning-0.4.4/src/miml/transformation/mimlTOml/minmax.py`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/tutorial/demo.ipynb` & `mimllearning-0.4.4/src/miml/tutorial/demo.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/tutorial/miml_data.ipynb` & `mimllearning-0.4.4/src/miml/tutorial/miml_data.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/tutorial/miml_transformations.ipynb` & `mimllearning-0.4.4/src/miml/tutorial/miml_transformations.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/src/miml/tutorial/mimltoml_classifiers.ipynb` & `mimllearning-0.4.4/src/miml/tutorial/mimltoml_classifiers.ipynb`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/README.md` & `mimllearning-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `mimllearning-0.4.3/PKG-INFO` & `mimllearning-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: mimllearning
-Version: 0.4.3
+Version: 0.4.4
 Summary: MIML Learning Library
 Project-URL: Homepage, https://github.com/p82maavd/miml
 Author-email: Damian Martinez <damianmartinezavila@gmail.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

