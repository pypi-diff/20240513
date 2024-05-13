# Comparing `tmp/data-quality-validation-pydeequ-1.0.tar.gz` & `tmp/data-quality-validation-pydeequ-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-quality-validation-pydeequ-1.0.tar", last modified: Wed May  8 02:41:53 2024, max compression
+gzip compressed data, was "data-quality-validation-pydeequ-1.1.tar", last modified: Mon May 13 10:16:35 2024, max compression
```

## Comparing `data-quality-validation-pydeequ-1.0.tar` & `data-quality-validation-pydeequ-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-08 02:41:53.968831 data-quality-validation-pydeequ-1.0/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     7223 2024-05-08 02:41:53.968424 data-quality-validation-pydeequ-1.0/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6711 2024-05-08 02:41:43.000000 data-quality-validation-pydeequ-1.0/README.md
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-08 02:41:53.967971 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     7223 2024-05-08 02:41:53.000000 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/PKG-INFO
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-08 02:41:53.000000 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/SOURCES.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-08 02:41:53.000000 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/dependency_links.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-08 02:41:53.000000 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/requires.txt
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-08 02:41:53.000000 data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/top_level.txt
-drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-08 02:41:53.966956 data-quality-validation-pydeequ-1.0/dqv/
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-1.0/dqv/__init__.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-1.0/dqv/data_quality_validation_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5358 2024-05-07 16:43:25.000000 data-quality-validation-pydeequ-1.0/dqv/dqv_pydeequ.py
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-08 02:41:53.968906 data-quality-validation-pydeequ-1.0/setup.cfg
--rw-r--r--   0 ajayrahulraja   (502) staff       (20)      857 2024-05-08 02:41:51.000000 data-quality-validation-pydeequ-1.0/setup.py
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-13 10:16:35.909888 data-quality-validation-pydeequ-1.1/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6305 2024-05-13 10:16:35.909519 data-quality-validation-pydeequ-1.1/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     5793 2024-05-13 10:16:24.000000 data-quality-validation-pydeequ-1.1/README.md
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-13 10:16:35.908969 data-quality-validation-pydeequ-1.1/data_quality_validation_pydeequ.egg-info/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)     6305 2024-05-13 10:16:35.000000 data-quality-validation-pydeequ-1.1/data_quality_validation_pydeequ.egg-info/PKG-INFO
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      366 2024-05-13 10:16:35.000000 data-quality-validation-pydeequ-1.1/data_quality_validation_pydeequ.egg-info/SOURCES.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        1 2024-05-13 10:16:35.000000 data-quality-validation-pydeequ-1.1/data_quality_validation_pydeequ.egg-info/dependency_links.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       28 2024-05-13 10:16:35.000000 data-quality-validation-pydeequ-1.1/data_quality_validation_pydeequ.egg-info/requires.txt
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        4 2024-05-13 10:16:35.000000 data-quality-validation-pydeequ-1.1/data_quality_validation_pydeequ.egg-info/top_level.txt
+drwxr-xr-x   0 ajayrahulraja   (502) staff       (20)        0 2024-05-13 10:16:35.907426 data-quality-validation-pydeequ-1.1/dqv/
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)        0 2024-05-06 06:16:20.000000 data-quality-validation-pydeequ-1.1/dqv/__init__.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    11706 2024-05-06 09:17:04.000000 data-quality-validation-pydeequ-1.1/dqv/data_quality_validation_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)    16427 2024-05-13 10:15:06.000000 data-quality-validation-pydeequ-1.1/dqv/dqv_pydeequ.py
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)       38 2024-05-13 10:16:35.909956 data-quality-validation-pydeequ-1.1/setup.cfg
+-rw-r--r--   0 ajayrahulraja   (502) staff       (20)      857 2024-05-13 10:16:31.000000 data-quality-validation-pydeequ-1.1/setup.py
```

### Comparing `data-quality-validation-pydeequ-1.0/PKG-INFO` & `data-quality-validation-pydeequ-1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-quality-validation-pydeequ
-Version: 1.0
+Version: 1.1
 Summary: A library for data quality validation using PyDeequ and to send email notification.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -18,15 +18,15 @@
 
 This package is designed for performing data quality validation using PyDeequ.  
 It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  
 Also, to send email notification about the validation result.
 
 **Author**: Ketan Kirange
 
-**Contributors**: Ketan Kirange, Ajay Rahul Raja, Ruth Mifsud
+**Contributors**: Ketan Kirange, Ajay Rahul Raja
 
 This package contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
  - Dask, and 
  - PySpark formats, leveraging libraries such as PyDeequ and SODA utilities.
 
 These checks help ensure the integrity, accuracy, and completeness of the data, essential for robust data-driven decision-making processes.
@@ -54,22 +54,15 @@
 Poor data quality can lead to misleading reports and flawed interpretations.
 
 <span style='color: Pink; font-size:25px'> 4. Regulatory Compliance </span>
 
 In many industries, compliance with regulations such as GDPR, HIPAA, or industry-specific standards is mandatory.  
 Ensuring data quality is essential for meeting these regulatory requirements and avoiding potential legal consequences.
 
-<span style='color: Pink; font-size:25px'> **Data Quality Validation Tools** </span>
 
-This repository provides a set of tools and utilities to perform comprehensive data quality validation on various data formats:
-
-- **Pandas**: Data quality checks for data stored in Pandas DataFrames, including checks for missing values, data types, and statistical summaries.
-- **Dask**: Scalable data quality checks for large-scale datasets using Dask, ensuring consistency and accuracy across distributed computing environments.
-- **PySpark with PyDeequ**: Integration with PyDeequ, enabling data quality validation on data processed using PySpark, including checks for schema validation, data distribution, and anomaly detection.
-- **SODA Utilities**: Utilities for validating data quality using SODA (Scalable Observations of Data Attributes) framework, allowing for automated quality checks and anomaly detection.
 
 <span style='color: Pink; font-size:25px'> **Getting Started** </span>
 
 To get started with data quality validation using this repository, follow the instructions in the respective documentation for each tool:
 
 - [Pandas Data Quality Validation Guide](link-to-pandas-guide)
 - [Dask Data Quality Validation Guide](link-to-dask-guide)
```

### Comparing `data-quality-validation-pydeequ-1.0/README.md` & `data-quality-validation-pydeequ-1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 This package is designed for performing data quality validation using PyDeequ.  
 It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  
 Also, to send email notification about the validation result.
 
 **Author**: Ketan Kirange
 
-**Contributors**: Ketan Kirange, Ajay Rahul Raja, Ruth Mifsud
+**Contributors**: Ketan Kirange, Ajay Rahul Raja
 
 This package contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
  - Dask, and 
  - PySpark formats, leveraging libraries such as PyDeequ and SODA utilities.
 
 These checks help ensure the integrity, accuracy, and completeness of the data, essential for robust data-driven decision-making processes.
@@ -38,22 +38,15 @@
 Poor data quality can lead to misleading reports and flawed interpretations.
 
 <span style='color: Pink; font-size:25px'> 4. Regulatory Compliance </span>
 
 In many industries, compliance with regulations such as GDPR, HIPAA, or industry-specific standards is mandatory.  
 Ensuring data quality is essential for meeting these regulatory requirements and avoiding potential legal consequences.
 
-<span style='color: Pink; font-size:25px'> **Data Quality Validation Tools** </span>
 
-This repository provides a set of tools and utilities to perform comprehensive data quality validation on various data formats:
-
-- **Pandas**: Data quality checks for data stored in Pandas DataFrames, including checks for missing values, data types, and statistical summaries.
-- **Dask**: Scalable data quality checks for large-scale datasets using Dask, ensuring consistency and accuracy across distributed computing environments.
-- **PySpark with PyDeequ**: Integration with PyDeequ, enabling data quality validation on data processed using PySpark, including checks for schema validation, data distribution, and anomaly detection.
-- **SODA Utilities**: Utilities for validating data quality using SODA (Scalable Observations of Data Attributes) framework, allowing for automated quality checks and anomaly detection.
 
 <span style='color: Pink; font-size:25px'> **Getting Started** </span>
 
 To get started with data quality validation using this repository, follow the instructions in the respective documentation for each tool:
 
 - [Pandas Data Quality Validation Guide](link-to-pandas-guide)
 - [Dask Data Quality Validation Guide](link-to-dask-guide)
```

### Comparing `data-quality-validation-pydeequ-1.0/data_quality_validation_pydeequ.egg-info/PKG-INFO` & `data-quality-validation-pydeequ-1.1/data_quality_validation_pydeequ.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-quality-validation-pydeequ
-Version: 1.0
+Version: 1.1
 Summary: A library for data quality validation using PyDeequ and to send email notification.
 Author: Ketan Kirange
 Author-email: k.kirange@reply.com
 Keywords: data quality validation pydeequ
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -18,15 +18,15 @@
 
 This package is designed for performing data quality validation using PyDeequ.  
 It enables users to validate the quality of their data, identifying any potential issues that may affect its suitability for processing or analysis.  
 Also, to send email notification about the validation result.
 
 **Author**: Ketan Kirange
 
-**Contributors**: Ketan Kirange, Ajay Rahul Raja, Ruth Mifsud
+**Contributors**: Ketan Kirange, Ajay Rahul Raja
 
 This package contains tools and utilities for performing data quality checks on data files in 
  - Pandas, 
  - Dask, and 
  - PySpark formats, leveraging libraries such as PyDeequ and SODA utilities.
 
 These checks help ensure the integrity, accuracy, and completeness of the data, essential for robust data-driven decision-making processes.
@@ -54,22 +54,15 @@
 Poor data quality can lead to misleading reports and flawed interpretations.
 
 <span style='color: Pink; font-size:25px'> 4. Regulatory Compliance </span>
 
 In many industries, compliance with regulations such as GDPR, HIPAA, or industry-specific standards is mandatory.  
 Ensuring data quality is essential for meeting these regulatory requirements and avoiding potential legal consequences.
 
-<span style='color: Pink; font-size:25px'> **Data Quality Validation Tools** </span>
 
-This repository provides a set of tools and utilities to perform comprehensive data quality validation on various data formats:
-
-- **Pandas**: Data quality checks for data stored in Pandas DataFrames, including checks for missing values, data types, and statistical summaries.
-- **Dask**: Scalable data quality checks for large-scale datasets using Dask, ensuring consistency and accuracy across distributed computing environments.
-- **PySpark with PyDeequ**: Integration with PyDeequ, enabling data quality validation on data processed using PySpark, including checks for schema validation, data distribution, and anomaly detection.
-- **SODA Utilities**: Utilities for validating data quality using SODA (Scalable Observations of Data Attributes) framework, allowing for automated quality checks and anomaly detection.
 
 <span style='color: Pink; font-size:25px'> **Getting Started** </span>
 
 To get started with data quality validation using this repository, follow the instructions in the respective documentation for each tool:
 
 - [Pandas Data Quality Validation Guide](link-to-pandas-guide)
 - [Dask Data Quality Validation Guide](link-to-dask-guide)
```

### Comparing `data-quality-validation-pydeequ-1.0/dqv/data_quality_validation_pydeequ.py` & `data-quality-validation-pydeequ-1.1/dqv/data_quality_validation_pydeequ.py`

 * *Files identical despite different names*

### Comparing `data-quality-validation-pydeequ-1.0/setup.py` & `data-quality-validation-pydeequ-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Reading the README.md file for long description in PyPI site
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='data-quality-validation-pydeequ',
-    version='1.0',
+    version='1.1',
     author='Ketan Kirange',
     author_email='k.kirange@reply.com',
     description='A library for data quality validation using PyDeequ and to send email notification.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

