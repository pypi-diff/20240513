# Comparing `tmp/payopt-1.0.1.tar.gz` & `tmp/payopt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "payopt-1.0.1.tar", last modified: Sun May 12 21:23:58 2024, max compression
+gzip compressed data, was "payopt-1.0.2.tar", last modified: Sun May 12 22:03:46 2024, max compression
```

## Comparing `payopt-1.0.1.tar` & `payopt-1.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 21:23:58.431706 payopt-1.0.1/
--rw-r--r--   0 areg       (502) staff       (20)     1083 2024-04-09 20:32:48.000000 payopt-1.0.1/LICENSE
--rw-r--r--   0 areg       (502) staff       (20)    11780 2024-05-12 21:23:58.429368 payopt-1.0.1/PKG-INFO
-drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 21:23:58.364518 payopt-1.0.1/PayOpt.egg-info/
--rw-r--r--   0 areg       (502) staff       (20)    11780 2024-05-12 21:23:58.000000 payopt-1.0.1/PayOpt.egg-info/PKG-INFO
--rw-r--r--   0 areg       (502) staff       (20)      801 2024-05-12 21:23:58.000000 payopt-1.0.1/PayOpt.egg-info/SOURCES.txt
--rw-r--r--   0 areg       (502) staff       (20)        1 2024-05-12 21:23:58.000000 payopt-1.0.1/PayOpt.egg-info/dependency_links.txt
--rw-r--r--   0 areg       (502) staff       (20)     2522 2024-05-12 21:23:58.000000 payopt-1.0.1/PayOpt.egg-info/requires.txt
--rw-r--r--   0 areg       (502) staff       (20)       18 2024-05-12 21:23:58.000000 payopt-1.0.1/PayOpt.egg-info/top_level.txt
--rw-r--r--   0 areg       (502) staff       (20)     6841 2024-05-12 21:06:01.000000 payopt-1.0.1/README.md
-drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 21:23:58.341634 payopt-1.0.1/payment_optimizer/
--rw-r--r--   0 areg       (502) staff       (20)       48 2024-05-09 17:02:35.000000 payopt-1.0.1/payment_optimizer/__init__.py
-drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 21:23:58.347161 payopt-1.0.1/payment_optimizer/api/
--rw-r--r--   0 areg       (502) staff       (20)        0 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/api/__init__.py
--rw-r--r--   0 areg       (502) staff       (20)     9338 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/api/auth_required.py
--rw-r--r--   0 areg       (502) staff       (20)     4918 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/api/endpoints.py
--rw-r--r--   0 areg       (502) staff       (20)     3653 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/api/granted_user_required.py
--rw-r--r--   0 areg       (502) staff       (20)     3106 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/api/schemas.py
--rw-r--r--   0 areg       (502) staff       (20)     4210 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/api/utils.py
-drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 21:23:58.355453 payopt-1.0.1/payment_optimizer/db/
--rw-r--r--   0 areg       (502) staff       (20)      404 2024-05-09 17:02:35.000000 payopt-1.0.1/payment_optimizer/db/__init__.py
--rw-r--r--   0 areg       (502) staff       (20)     1277 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/db/basic_etl.py
--rw-r--r--   0 areg       (502) staff       (20)     2913 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/db/csv_files_creator.py
--rw-r--r--   0 areg       (502) staff       (20)     4607 2024-05-11 08:03:41.000000 payopt-1.0.1/payment_optimizer/db/data_generator.py
--rw-r--r--   0 areg       (502) staff       (20)     2382 2024-05-11 07:40:32.000000 payopt-1.0.1/payment_optimizer/db/logger.py
--rw-r--r--   0 areg       (502) staff       (20)     6201 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/db/schema.py
--rw-r--r--   0 areg       (502) staff       (20)    18760 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/db/sql_interactions.py
-drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 21:23:58.358120 payopt-1.0.1/payment_optimizer/modeling/
--rw-r--r--   0 areg       (502) staff       (20)       45 2024-04-09 20:15:34.000000 payopt-1.0.1/payment_optimizer/modeling/__init__.py
--rw-r--r--   0 areg       (502) staff       (20)     8792 2024-05-12 21:06:01.000000 payopt-1.0.1/payment_optimizer/modeling/models.py
--rw-r--r--   0 areg       (502) staff       (20)       38 2024-05-12 21:23:58.433792 payopt-1.0.1/setup.cfg
--rw-r--r--   0 areg       (502) staff       (20)      936 2024-05-12 21:23:40.000000 payopt-1.0.1/setup.py
-drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 21:23:58.361618 payopt-1.0.1/tests/
--rw-r--r--   0 areg       (502) staff       (20)     1652 2024-05-12 21:06:01.000000 payopt-1.0.1/tests/test_modeling.py
--rw-r--r--   0 areg       (502) staff       (20)     4344 2024-05-12 21:06:01.000000 payopt-1.0.1/tests/test_transactions.py
+drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 22:03:46.891970 payopt-1.0.2/
+-rw-r--r--   0 areg       (502) staff       (20)     1083 2024-04-09 20:32:48.000000 payopt-1.0.2/LICENSE
+-rw-r--r--   0 areg       (502) staff       (20)    11760 2024-05-12 22:03:46.890509 payopt-1.0.2/PKG-INFO
+drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 22:03:46.823581 payopt-1.0.2/PayOpt.egg-info/
+-rw-r--r--   0 areg       (502) staff       (20)    11760 2024-05-12 22:03:46.000000 payopt-1.0.2/PayOpt.egg-info/PKG-INFO
+-rw-r--r--   0 areg       (502) staff       (20)      801 2024-05-12 22:03:46.000000 payopt-1.0.2/PayOpt.egg-info/SOURCES.txt
+-rw-r--r--   0 areg       (502) staff       (20)        1 2024-05-12 22:03:46.000000 payopt-1.0.2/PayOpt.egg-info/dependency_links.txt
+-rw-r--r--   0 areg       (502) staff       (20)     2522 2024-05-12 22:03:46.000000 payopt-1.0.2/PayOpt.egg-info/requires.txt
+-rw-r--r--   0 areg       (502) staff       (20)       18 2024-05-12 22:03:46.000000 payopt-1.0.2/PayOpt.egg-info/top_level.txt
+-rw-r--r--   0 areg       (502) staff       (20)     6821 2024-05-12 21:58:19.000000 payopt-1.0.2/README.md
+drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 22:03:46.799824 payopt-1.0.2/payment_optimizer/
+-rw-r--r--   0 areg       (502) staff       (20)       48 2024-05-09 17:02:35.000000 payopt-1.0.2/payment_optimizer/__init__.py
+drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 22:03:46.807513 payopt-1.0.2/payment_optimizer/api/
+-rw-r--r--   0 areg       (502) staff       (20)        0 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/api/__init__.py
+-rw-r--r--   0 areg       (502) staff       (20)     9338 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/api/auth_required.py
+-rw-r--r--   0 areg       (502) staff       (20)     4918 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/api/endpoints.py
+-rw-r--r--   0 areg       (502) staff       (20)     3653 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/api/granted_user_required.py
+-rw-r--r--   0 areg       (502) staff       (20)     3106 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/api/schemas.py
+-rw-r--r--   0 areg       (502) staff       (20)     4210 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/api/utils.py
+drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 22:03:46.815338 payopt-1.0.2/payment_optimizer/db/
+-rw-r--r--   0 areg       (502) staff       (20)      404 2024-05-09 17:02:35.000000 payopt-1.0.2/payment_optimizer/db/__init__.py
+-rw-r--r--   0 areg       (502) staff       (20)     1277 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/db/basic_etl.py
+-rw-r--r--   0 areg       (502) staff       (20)     2913 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/db/csv_files_creator.py
+-rw-r--r--   0 areg       (502) staff       (20)     4607 2024-05-11 08:03:41.000000 payopt-1.0.2/payment_optimizer/db/data_generator.py
+-rw-r--r--   0 areg       (502) staff       (20)     2382 2024-05-11 07:40:32.000000 payopt-1.0.2/payment_optimizer/db/logger.py
+-rw-r--r--   0 areg       (502) staff       (20)     6201 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/db/schema.py
+-rw-r--r--   0 areg       (502) staff       (20)    18760 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/db/sql_interactions.py
+drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 22:03:46.819160 payopt-1.0.2/payment_optimizer/modeling/
+-rw-r--r--   0 areg       (502) staff       (20)       45 2024-04-09 20:15:34.000000 payopt-1.0.2/payment_optimizer/modeling/__init__.py
+-rw-r--r--   0 areg       (502) staff       (20)     8792 2024-05-12 21:06:01.000000 payopt-1.0.2/payment_optimizer/modeling/models.py
+-rw-r--r--   0 areg       (502) staff       (20)       38 2024-05-12 22:03:46.892246 payopt-1.0.2/setup.cfg
+-rw-r--r--   0 areg       (502) staff       (20)      936 2024-05-12 22:03:37.000000 payopt-1.0.2/setup.py
+drwxr-xr-x   0 areg       (502) staff       (20)        0 2024-05-12 22:03:46.821666 payopt-1.0.2/tests/
+-rw-r--r--   0 areg       (502) staff       (20)     1652 2024-05-12 21:06:01.000000 payopt-1.0.2/tests/test_modeling.py
+-rw-r--r--   0 areg       (502) staff       (20)     4344 2024-05-12 21:06:01.000000 payopt-1.0.2/tests/test_transactions.py
```

### Comparing `payopt-1.0.1/LICENSE` & `payopt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/PKG-INFO` & `payopt-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PayOpt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Optimizing the payment process of e-commerce
 Author: Nane Mambreyan, Areg Amirjanyan, Gayane Ohanjanyan, Hasmik Sahakyan
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8.2, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -173,23 +173,23 @@
 ![Alt Text](Documents/ERD.png)
 
 ## Installation
 
 You can install Payment Optimizer using pip:
 
 ```bash
-pip install payment_optimizer
+pip install pay_opt
 ```
 
 ## Usage
 
 Below is a basic example demonstrating how to utilize certain functions from the package:
 
 ```python
-from payment_optimizer.models import ABTesting
+from pay_opt.models import ABTesting
 
 ab_test = ABTesting(data_connect)
 ab_test.preprocess_data()
 model_result = ab_test.perform_ab_test(start_date, end_date)
 ```
 
 ## API Calls
```

### Comparing `payopt-1.0.1/PayOpt.egg-info/PKG-INFO` & `payopt-1.0.2/PayOpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PayOpt
-Version: 1.0.1
+Version: 1.0.2
 Summary: Optimizing the payment process of e-commerce
 Author: Nane Mambreyan, Areg Amirjanyan, Gayane Ohanjanyan, Hasmik Sahakyan
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.8.2, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -173,23 +173,23 @@
 ![Alt Text](Documents/ERD.png)
 
 ## Installation
 
 You can install Payment Optimizer using pip:
 
 ```bash
-pip install payment_optimizer
+pip install pay_opt
 ```
 
 ## Usage
 
 Below is a basic example demonstrating how to utilize certain functions from the package:
 
 ```python
-from payment_optimizer.models import ABTesting
+from pay_opt.models import ABTesting
 
 ab_test = ABTesting(data_connect)
 ab_test.preprocess_data()
 model_result = ab_test.perform_ab_test(start_date, end_date)
 ```
 
 ## API Calls
```

### Comparing `payopt-1.0.1/PayOpt.egg-info/SOURCES.txt` & `payopt-1.0.2/PayOpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/PayOpt.egg-info/requires.txt` & `payopt-1.0.2/PayOpt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/README.md` & `payopt-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,23 +23,23 @@
 ![Alt Text](Documents/ERD.png)
 
 ## Installation
 
 You can install Payment Optimizer using pip:
 
 ```bash
-pip install payment_optimizer
+pip install pay_opt
 ```
 
 ## Usage
 
 Below is a basic example demonstrating how to utilize certain functions from the package:
 
 ```python
-from payment_optimizer.models import ABTesting
+from pay_opt.models import ABTesting
 
 ab_test = ABTesting(data_connect)
 ab_test.preprocess_data()
 model_result = ab_test.perform_ab_test(start_date, end_date)
 ```
 
 ## API Calls
```

### Comparing `payopt-1.0.1/payment_optimizer/api/auth_required.py` & `payopt-1.0.2/payment_optimizer/api/auth_required.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/api/endpoints.py` & `payopt-1.0.2/payment_optimizer/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/api/granted_user_required.py` & `payopt-1.0.2/payment_optimizer/api/granted_user_required.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/api/schemas.py` & `payopt-1.0.2/payment_optimizer/api/schemas.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/api/utils.py` & `payopt-1.0.2/payment_optimizer/api/utils.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/db/basic_etl.py` & `payopt-1.0.2/payment_optimizer/db/basic_etl.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/db/csv_files_creator.py` & `payopt-1.0.2/payment_optimizer/db/csv_files_creator.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/db/data_generator.py` & `payopt-1.0.2/payment_optimizer/db/data_generator.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/db/logger.py` & `payopt-1.0.2/payment_optimizer/db/logger.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/db/schema.py` & `payopt-1.0.2/payment_optimizer/db/schema.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/db/sql_interactions.py` & `payopt-1.0.2/payment_optimizer/db/sql_interactions.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/payment_optimizer/modeling/models.py` & `payopt-1.0.2/payment_optimizer/modeling/models.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/setup.py` & `payopt-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with open("docs_requirements.txt") as f: 
     docreqs = f.read().splitlines() 
 
 
 setup( 
     name="PayOpt", 
-    version='1.0.1',
+    version='1.0.2',
     description="Optimizing the payment process of e-commerce", 
     long_description=pathlib.Path("README.md").read_text(), 
     long_description_content_type="text/markdown", 
     author="Nane Mambreyan, Areg Amirjanyan, Gayane Ohanjanyan, Hasmik Sahakyan", 
     license="MIT", 
     classifiers=[ 
         "Development Status :: 3 - Alpha"
```

### Comparing `payopt-1.0.1/tests/test_modeling.py` & `payopt-1.0.2/tests/test_modeling.py`

 * *Files identical despite different names*

### Comparing `payopt-1.0.1/tests/test_transactions.py` & `payopt-1.0.2/tests/test_transactions.py`

 * *Files identical despite different names*

