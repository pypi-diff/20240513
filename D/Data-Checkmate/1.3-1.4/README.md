# Comparing `tmp/Data-Checkmate-1.3.tar.gz` & `tmp/Data-Checkmate-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Data-Checkmate-1.3.tar", last modified: Mon May 13 11:03:28 2024, max compression
+gzip compressed data, was "Data-Checkmate-1.4.tar", last modified: Mon May 13 11:15:08 2024, max compression
```

## Comparing `Data-Checkmate-1.3.tar` & `Data-Checkmate-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-13 11:03:28.750975 Data-Checkmate-1.3/
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-13 11:03:28.749945 Data-Checkmate-1.3/Data_Checkmate.egg-info/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6865 2024-05-13 11:03:28.000000 Data-Checkmate-1.3/Data_Checkmate.egg-info/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      283 2024-05-13 11:03:28.000000 Data-Checkmate-1.3/Data_Checkmate.egg-info/SOURCES.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-13 11:03:28.000000 Data-Checkmate-1.3/Data_Checkmate.egg-info/dependency_links.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-13 11:03:28.000000 Data-Checkmate-1.3/Data_Checkmate.egg-info/requires.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-13 11:03:28.000000 Data-Checkmate-1.3/Data_Checkmate.egg-info/top_level.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6865 2024-05-13 11:03:28.750532 Data-Checkmate-1.3/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6355 2024-05-13 10:53:48.000000 Data-Checkmate-1.3/README.md
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-13 11:03:28.749176 Data-Checkmate-1.3/dqv/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 Data-Checkmate-1.3/dqv/__init__.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 Data-Checkmate-1.3/dqv/data_quality_validation_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    16890 2024-05-13 11:02:24.000000 Data-Checkmate-1.3/dqv/datacheckmate.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-13 11:03:28.751251 Data-Checkmate-1.3/setup.cfg
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      855 2024-05-13 11:00:02.000000 Data-Checkmate-1.3/setup.py
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-13 11:15:08.903118 Data-Checkmate-1.4/
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-13 11:15:08.896968 Data-Checkmate-1.4/Data_Checkmate.egg-info/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     7398 2024-05-13 11:15:08.000000 Data-Checkmate-1.4/Data_Checkmate.egg-info/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      283 2024-05-13 11:15:08.000000 Data-Checkmate-1.4/Data_Checkmate.egg-info/SOURCES.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-13 11:15:08.000000 Data-Checkmate-1.4/Data_Checkmate.egg-info/dependency_links.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-13 11:15:08.000000 Data-Checkmate-1.4/Data_Checkmate.egg-info/requires.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-13 11:15:08.000000 Data-Checkmate-1.4/Data_Checkmate.egg-info/top_level.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     7398 2024-05-13 11:15:08.899286 Data-Checkmate-1.4/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6888 2024-05-13 11:14:55.000000 Data-Checkmate-1.4/README.md
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-13 11:15:08.894222 Data-Checkmate-1.4/dqv/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 Data-Checkmate-1.4/dqv/__init__.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 Data-Checkmate-1.4/dqv/data_quality_validation_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    16890 2024-05-13 11:02:24.000000 Data-Checkmate-1.4/dqv/datacheckmate.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-13 11:15:08.903243 Data-Checkmate-1.4/setup.cfg
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      855 2024-05-13 11:15:00.000000 Data-Checkmate-1.4/setup.py
```

### Comparing `Data-Checkmate-1.3/Data_Checkmate.egg-info/PKG-INFO` & `Data-Checkmate-1.4/Data_Checkmate.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Data-Checkmate
-Version: 1.3
+Version: 1.4
 Summary: A library for data quality validation using PyDeequ and to send email notification.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ data-checkmate
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -13,16 +13,15 @@
 Requires-Dist: pydeequ
 Requires-Dist: boto3
 Requires-Dist: pyyaml
 
 <span style='color: Pink; font-size:25px'>  **Data-Checkmate, a Data Quality Validation** </span>
 
 This package is designed for performing data quality validation using PyDeequ.  
-It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  
-Also, to send email notification about the validation result.
+It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  Also, to send email notification about the validation result.
 
 **Author**: Ketan Kirange
 
 **Contributors**: Ketan Kirange, Ajay Rahul Raja
 
 This package contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
@@ -63,21 +62,24 @@
 This repository provides a set of tools and utilities to perform comprehensive data quality validation on various data formats:
 
 - **Pandas**: Data quality checks for data stored in Pandas DataFrames, including checks for missing values, data types, and statistical summaries.
 - **Dask**: Scalable data quality checks for large-scale datasets using Dask, ensuring consistency and accuracy across distributed computing environments.
 - **PySpark with PyDeequ**: Integration with PyDeequ, enabling data quality validation on data processed using PySpark, including checks for schema validation, data distribution, and anomaly detection.
 - **SODA Utilities**: Utilities for validating data quality using SODA (Scalable Observations of Data Attributes) framework, allowing for automated quality checks and anomaly detection.
 
-<span style='color: Pink; font-size:25px'> **Getting Started** </span>
+## Examples
 
-<span style='color: Pink; font-size:25px'> **Contributing** </span>
-
-We welcome contributions from the community to enhance and expand the capabilities of this data quality validation repository.  
-Please refer to the [contribution guidelines](link-to-contribution-guidelines) for more information on how to contribute.
+To get started with Data-Checkmate for validation, please refer these below notebooks:
 
+- [Pandas Data Quality Validation Guide](https://github.com/dataruk/data-quality-validation/blob/main/notebook/Test_DQ_checks_pandas.ipynb)
+- [Dask Data Quality Validation Guide](https://github.com/dataruk/data-quality-validation/blob/main/notebook/Test_DQ_checks_dask.ipynb)
+- [PySpark with PyDeequ](https://github.com/dataruk/data-quality-validation/blob/main/notebook/demo_packageInstallation_and_email.ipynb)
+- [PySpark with PyDeequ Guide using hospital data](https://github.com/dataruk/data-quality-validation/blob/main/notebook/hospital_pydeequ.ipynb)
+- [PySpark with PyDeequ Guide using AML data](https://github.com/dataruk/data-quality-validation/blob/main/notebook/aml_pydeequ.ipynb)
+- [PySpark with PyDeequ Guide using PL data](https://github.com/dataruk/data-quality-validation/blob/main/notebook/pl_pydeequ.ipynb)
 
 
 
 <br></br>
 <span style="font-size:13pt; color:orange">**Prerequisites:**</span>
 
 - Step 1: Download Java, Python, and Apache Spark.
```

### Comparing `Data-Checkmate-1.3/PKG-INFO` & `Data-Checkmate-1.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Data-Checkmate
-Version: 1.3
+Version: 1.4
 Summary: A library for data quality validation using PyDeequ and to send email notification.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ data-checkmate
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -13,16 +13,15 @@
 Requires-Dist: pydeequ
 Requires-Dist: boto3
 Requires-Dist: pyyaml
 
 <span style='color: Pink; font-size:25px'>  **Data-Checkmate, a Data Quality Validation** </span>
 
 This package is designed for performing data quality validation using PyDeequ.  
-It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  
-Also, to send email notification about the validation result.
+It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  Also, to send email notification about the validation result.
 
 **Author**: Ketan Kirange
 
 **Contributors**: Ketan Kirange, Ajay Rahul Raja
 
 This package contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
@@ -63,21 +62,24 @@
 This repository provides a set of tools and utilities to perform comprehensive data quality validation on various data formats:
 
 - **Pandas**: Data quality checks for data stored in Pandas DataFrames, including checks for missing values, data types, and statistical summaries.
 - **Dask**: Scalable data quality checks for large-scale datasets using Dask, ensuring consistency and accuracy across distributed computing environments.
 - **PySpark with PyDeequ**: Integration with PyDeequ, enabling data quality validation on data processed using PySpark, including checks for schema validation, data distribution, and anomaly detection.
 - **SODA Utilities**: Utilities for validating data quality using SODA (Scalable Observations of Data Attributes) framework, allowing for automated quality checks and anomaly detection.
 
-<span style='color: Pink; font-size:25px'> **Getting Started** </span>
+## Examples
 
-<span style='color: Pink; font-size:25px'> **Contributing** </span>
-
-We welcome contributions from the community to enhance and expand the capabilities of this data quality validation repository.  
-Please refer to the [contribution guidelines](link-to-contribution-guidelines) for more information on how to contribute.
+To get started with Data-Checkmate for validation, please refer these below notebooks:
 
+- [Pandas Data Quality Validation Guide](https://github.com/dataruk/data-quality-validation/blob/main/notebook/Test_DQ_checks_pandas.ipynb)
+- [Dask Data Quality Validation Guide](https://github.com/dataruk/data-quality-validation/blob/main/notebook/Test_DQ_checks_dask.ipynb)
+- [PySpark with PyDeequ](https://github.com/dataruk/data-quality-validation/blob/main/notebook/demo_packageInstallation_and_email.ipynb)
+- [PySpark with PyDeequ Guide using hospital data](https://github.com/dataruk/data-quality-validation/blob/main/notebook/hospital_pydeequ.ipynb)
+- [PySpark with PyDeequ Guide using AML data](https://github.com/dataruk/data-quality-validation/blob/main/notebook/aml_pydeequ.ipynb)
+- [PySpark with PyDeequ Guide using PL data](https://github.com/dataruk/data-quality-validation/blob/main/notebook/pl_pydeequ.ipynb)
 
 
 
 <br></br>
 <span style="font-size:13pt; color:orange">**Prerequisites:**</span>
 
 - Step 1: Download Java, Python, and Apache Spark.
```

### Comparing `Data-Checkmate-1.3/README.md` & `Data-Checkmate-1.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 <span style='color: Pink; font-size:25px'>  **Data-Checkmate, a Data Quality Validation** </span>
 
 This package is designed for performing data quality validation using PyDeequ.  
-It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  
-Also, to send email notification about the validation result.
+It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  Also, to send email notification about the validation result.
 
 **Author**: Ketan Kirange
 
 **Contributors**: Ketan Kirange, Ajay Rahul Raja
 
 This package contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
@@ -47,21 +46,24 @@
 This repository provides a set of tools and utilities to perform comprehensive data quality validation on various data formats:
 
 - **Pandas**: Data quality checks for data stored in Pandas DataFrames, including checks for missing values, data types, and statistical summaries.
 - **Dask**: Scalable data quality checks for large-scale datasets using Dask, ensuring consistency and accuracy across distributed computing environments.
 - **PySpark with PyDeequ**: Integration with PyDeequ, enabling data quality validation on data processed using PySpark, including checks for schema validation, data distribution, and anomaly detection.
 - **SODA Utilities**: Utilities for validating data quality using SODA (Scalable Observations of Data Attributes) framework, allowing for automated quality checks and anomaly detection.
 
-<span style='color: Pink; font-size:25px'> **Getting Started** </span>
+## Examples
 
-<span style='color: Pink; font-size:25px'> **Contributing** </span>
-
-We welcome contributions from the community to enhance and expand the capabilities of this data quality validation repository.  
-Please refer to the [contribution guidelines](link-to-contribution-guidelines) for more information on how to contribute.
+To get started with Data-Checkmate for validation, please refer these below notebooks:
 
+- [Pandas Data Quality Validation Guide](https://github.com/dataruk/data-quality-validation/blob/main/notebook/Test_DQ_checks_pandas.ipynb)
+- [Dask Data Quality Validation Guide](https://github.com/dataruk/data-quality-validation/blob/main/notebook/Test_DQ_checks_dask.ipynb)
+- [PySpark with PyDeequ](https://github.com/dataruk/data-quality-validation/blob/main/notebook/demo_packageInstallation_and_email.ipynb)
+- [PySpark with PyDeequ Guide using hospital data](https://github.com/dataruk/data-quality-validation/blob/main/notebook/hospital_pydeequ.ipynb)
+- [PySpark with PyDeequ Guide using AML data](https://github.com/dataruk/data-quality-validation/blob/main/notebook/aml_pydeequ.ipynb)
+- [PySpark with PyDeequ Guide using PL data](https://github.com/dataruk/data-quality-validation/blob/main/notebook/pl_pydeequ.ipynb)
 
 
 
 <br></br>
 <span style="font-size:13pt; color:orange">**Prerequisites:**</span>
 
 - Step 1: Download Java, Python, and Apache Spark.
```

### Comparing `Data-Checkmate-1.3/dqv/data_quality_validation_pydeequ.py` & `Data-Checkmate-1.4/dqv/data_quality_validation_pydeequ.py`

 * *Files identical despite different names*

### Comparing `Data-Checkmate-1.3/dqv/datacheckmate.py` & `Data-Checkmate-1.4/dqv/datacheckmate.py`

 * *Files identical despite different names*

### Comparing `Data-Checkmate-1.3/setup.py` & `Data-Checkmate-1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Reading the README.md file for long description in PyPI site
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='Data-Checkmate',
-    version='1.3',
+    version='1.4',
     author='Ketan Kirange',
     author_email='k.kirange@reply.com',
     description='A library for data quality validation using PyDeequ and to send email notification.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

