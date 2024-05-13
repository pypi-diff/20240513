# Comparing `tmp/soma_integ-0.1.3.tar.gz` & `tmp/soma_integ-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soma_integ-0.1.3.tar", last modified: Sun May 12 19:33:38 2024, max compression
+gzip compressed data, was "soma_integ-0.1.4.tar", last modified: Mon May 13 06:23:32 2024, max compression
```

## Comparing `soma_integ-0.1.3.tar` & `soma_integ-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 19:33:38.965422 soma_integ-0.1.3/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.3/LICENSE
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 19:33:38.965175 soma_integ-0.1.3/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.3/README.md
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-12 19:31:32.000000 soma_integ-0.1.3/pyproject.toml
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-12 19:33:38.965478 soma_integ-0.1.3/setup.cfg
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 19:33:38.960600 soma_integ-0.1.3/src/
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 19:33:38.963325 soma_integ-0.1.3/src/soma_integ/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      432 2024-05-12 19:26:59.000000 soma_integ-0.1.3/src/soma_integ/__init__.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 08:37:42.000000 soma_integ-0.1.3/src/soma_integ/config.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3522 2024-05-12 18:36:38.000000 soma_integ-0.1.3/src/soma_integ/data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     9100 2024-05-12 19:22:09.000000 soma_integ-0.1.3/src/soma_integ/evaluation.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-12 08:37:42.000000 soma_integ-0.1.3/src/soma_integ/methods.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 08:37:42.000000 soma_integ-0.1.3/src/soma_integ/model.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 08:37:42.000000 soma_integ-0.1.3/src/soma_integ/optimization.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.3/src/soma_integ/utils.py
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 19:33:38.964789 soma_integ-0.1.3/src/soma_integ.egg-info/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-12 19:33:38.000000 soma_integ-0.1.3/src/soma_integ.egg-info/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      474 2024-05-12 19:33:38.000000 soma_integ-0.1.3/src/soma_integ.egg-info/SOURCES.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-12 19:33:38.000000 soma_integ-0.1.3/src/soma_integ.egg-info/dependency_links.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-12 19:33:38.000000 soma_integ-0.1.3/src/soma_integ.egg-info/requires.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-12 19:33:38.000000 soma_integ-0.1.3/src/soma_integ.egg-info/top_level.txt
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-12 19:33:38.964401 soma_integ-0.1.3/tests/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      550 2024-05-12 18:49:52.000000 soma_integ-0.1.3/tests/test_data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2163 2024-05-12 19:30:36.000000 soma_integ-0.1.3/tests/test_evaluation.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 06:23:32.155311 soma_integ-0.1.4/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.4/LICENSE
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-13 06:23:32.155096 soma_integ-0.1.4/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.4/README.md
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-13 06:22:42.000000 soma_integ-0.1.4/pyproject.toml
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-13 06:23:32.155358 soma_integ-0.1.4/setup.cfg
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 06:23:32.150684 soma_integ-0.1.4/src/
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 06:23:32.153405 soma_integ-0.1.4/src/soma_integ/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      432 2024-05-12 19:26:59.000000 soma_integ-0.1.4/src/soma_integ/__init__.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 08:37:42.000000 soma_integ-0.1.4/src/soma_integ/config.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3827 2024-05-13 06:21:12.000000 soma_integ-0.1.4/src/soma_integ/data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     9100 2024-05-12 19:22:09.000000 soma_integ-0.1.4/src/soma_integ/evaluation.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-12 08:37:42.000000 soma_integ-0.1.4/src/soma_integ/methods.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 08:37:42.000000 soma_integ-0.1.4/src/soma_integ/model.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 08:37:42.000000 soma_integ-0.1.4/src/soma_integ/optimization.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.4/src/soma_integ/utils.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 06:23:32.154789 soma_integ-0.1.4/src/soma_integ.egg-info/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-13 06:23:32.000000 soma_integ-0.1.4/src/soma_integ.egg-info/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      474 2024-05-13 06:23:32.000000 soma_integ-0.1.4/src/soma_integ.egg-info/SOURCES.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-13 06:23:32.000000 soma_integ-0.1.4/src/soma_integ.egg-info/dependency_links.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-13 06:23:32.000000 soma_integ-0.1.4/src/soma_integ.egg-info/requires.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-13 06:23:32.000000 soma_integ-0.1.4/src/soma_integ.egg-info/top_level.txt
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 06:23:32.154506 soma_integ-0.1.4/tests/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      550 2024-05-12 18:49:52.000000 soma_integ-0.1.4/tests/test_data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2163 2024-05-12 19:30:36.000000 soma_integ-0.1.4/tests/test_evaluation.py
```

### Comparing `soma_integ-0.1.3/LICENSE` & `soma_integ-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.3/PKG-INFO` & `soma_integ-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.3/pyproject.toml` & `soma_integ-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "soma_integ"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = ["numpy", "scikit-learn"]
 authors = [
     { name = "Sobhan Ahmadian Moghadam", email = "sobhan.ahmadian.moghadam@gmail.com" },
     { name = "Arman Rezaei", email = "arman.x.rezaei@gmail.com" },
 ]
 description = "A package for integrating implementation and evaluation of machine learning platforms"
 readme = "README.md"
```

### Comparing `soma_integ-0.1.3/src/soma_integ/config.py` & `soma_integ-0.1.4/src/soma_integ/config.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.3/src/soma_integ/data.py` & `soma_integ-0.1.4/src/soma_integ/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         k (int): number of folds.
         data (Data): data object.
     """
 
     def __init__(self, k: int, data: Data):
         self.k = k
         self.data = data
+        self.data_size = self.get_data_size()
         self.subsets = self.get_subsets()
 
     @abc.abstractmethod
     def split(self, i):
         """
         Split the data into train and test sets for the i-th fold.
 
@@ -44,25 +45,35 @@
 
         Returns:
             tuple: A tuple containing the train and test data. <train_data, test_data>
         """
         logger.info("{:#^50}".format(f"  Splitting Fold {i + 1}   "))
         raise NotImplementedError
 
+    @abc.abstractmethod
+    def get_data_size(self):
+        """
+        Get the size of the data. This will be used to calculate the size of the subsets.
+
+        Returns:
+            int: The size of the data.
+        """
+        raise NotImplementedError
+
     def get_subsets(self):
         """
         Generate subsets of data.
 
         Returns:
             dict: A dictionary containing subsets of data, where the keys represent the subset index and the values
                     represent the indices of the elements in the subset.
         """
         subsets = dict()
-        subset_size = int(len(self.data) / self.k)
-        remain = list(range(0, len(self.data)))
+        subset_size = int(self.data_size / self.k)
+        remain = list(range(0, self.data_size))
         for i in range(self.k - 1):
             subsets[i] = random.sample(remain, subset_size)
             remain = list(set(remain).difference(subsets[i]))
         subsets[self.k - 1] = remain
         return subsets
```

### Comparing `soma_integ-0.1.3/src/soma_integ/evaluation.py` & `soma_integ-0.1.4/src/soma_integ/evaluation.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.3/src/soma_integ/methods.py` & `soma_integ-0.1.4/src/soma_integ/methods.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.3/src/soma_integ/model.py` & `soma_integ-0.1.4/src/soma_integ/model.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.3/src/soma_integ/optimization.py` & `soma_integ-0.1.4/src/soma_integ/optimization.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.3/src/soma_integ.egg-info/PKG-INFO` & `soma_integ-0.1.4/src/soma_integ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.3/tests/test_data.py` & `soma_integ-0.1.4/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.3/tests/test_evaluation.py` & `soma_integ-0.1.4/tests/test_evaluation.py`

 * *Files identical despite different names*

