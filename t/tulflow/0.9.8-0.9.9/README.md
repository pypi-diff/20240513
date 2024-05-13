# Comparing `tmp/tulflow-0.9.8.tar.gz` & `tmp/tulflow-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulflow-0.9.8.tar", last modified: Tue Feb 20 19:17:36 2024, max compression
+gzip compressed data, was "tulflow-0.9.9.tar", last modified: Tue Mar 12 17:23:04 2024, max compression
```

## Comparing `tulflow-0.9.8.tar` & `tulflow-0.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-20 19:17:36.343816 tulflow-0.9.8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-02-20 19:17:27.000000 tulflow-0.9.8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2030 2024-02-20 19:17:36.343816 tulflow-0.9.8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1562 2024-02-20 19:17:27.000000 tulflow-0.9.8/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-02-20 19:17:36.343816 tulflow-0.9.8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1376 2024-02-20 19:17:27.000000 tulflow-0.9.8/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-20 19:17:36.339815 tulflow-0.9.8/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-02-20 19:17:27.000000 tulflow-0.9.8/tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1013 2024-02-20 19:17:27.000000 tulflow-0.9.8/tests/test_devo-256_lxml_bug.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27324 2024-02-20 19:17:27.000000 tulflow-0.9.8/tests/test_harvest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10884 2024-02-20 19:17:27.000000 tulflow-0.9.8/tests/test_process.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6929 2024-02-20 19:17:27.000000 tulflow-0.9.8/tests/test_solr_api_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5361 2024-02-20 19:17:27.000000 tulflow-0.9.8/tests/test_tasks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6539 2024-02-20 19:17:27.000000 tulflow-0.9.8/tests/test_transform.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    39634 2024-02-20 19:17:27.000000 tulflow-0.9.8/tests/test_validate.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-20 19:17:36.339815 tulflow-0.9.8/tulflow/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-02-20 19:17:27.000000 tulflow-0.9.8/tulflow/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10241 2024-02-20 19:17:27.000000 tulflow-0.9.8/tulflow/harvest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4926 2024-02-20 19:17:27.000000 tulflow-0.9.8/tulflow/process.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8536 2024-02-20 19:17:27.000000 tulflow-0.9.8/tulflow/solr_api_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3446 2024-02-20 19:17:27.000000 tulflow-0.9.8/tulflow/tasks.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3102 2024-02-20 19:17:27.000000 tulflow-0.9.8/tulflow/transform.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6372 2024-02-20 19:17:27.000000 tulflow-0.9.8/tulflow/validate.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-02-20 19:17:36.343816 tulflow-0.9.8/tulflow.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2030 2024-02-20 19:17:36.000000 tulflow-0.9.8/tulflow.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2024-02-20 19:17:36.000000 tulflow-0.9.8/tulflow.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-02-20 19:17:36.000000 tulflow-0.9.8/tulflow.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-02-20 19:17:36.000000 tulflow-0.9.8/tulflow.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-12 17:23:04.915201 tulflow-0.9.9/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-03-12 17:22:57.000000 tulflow-0.9.9/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2030 2024-03-12 17:23:04.915201 tulflow-0.9.9/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1562 2024-03-12 17:22:57.000000 tulflow-0.9.9/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-03-12 17:23:04.915201 tulflow-0.9.9/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1376 2024-03-12 17:22:57.000000 tulflow-0.9.9/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-12 17:23:04.915201 tulflow-0.9.9/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-03-12 17:22:57.000000 tulflow-0.9.9/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1013 2024-03-12 17:22:57.000000 tulflow-0.9.9/tests/test_devo-256_lxml_bug.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27324 2024-03-12 17:22:57.000000 tulflow-0.9.9/tests/test_harvest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10884 2024-03-12 17:22:57.000000 tulflow-0.9.9/tests/test_process.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6929 2024-03-12 17:22:57.000000 tulflow-0.9.9/tests/test_solr_api_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5361 2024-03-12 17:22:57.000000 tulflow-0.9.9/tests/test_tasks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6539 2024-03-12 17:22:57.000000 tulflow-0.9.9/tests/test_transform.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    39657 2024-03-12 17:22:57.000000 tulflow-0.9.9/tests/test_validate.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-12 17:23:04.915201 tulflow-0.9.9/tulflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       60 2024-03-12 17:22:57.000000 tulflow-0.9.9/tulflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10241 2024-03-12 17:22:57.000000 tulflow-0.9.9/tulflow/harvest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4926 2024-03-12 17:22:57.000000 tulflow-0.9.9/tulflow/process.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8536 2024-03-12 17:22:57.000000 tulflow-0.9.9/tulflow/solr_api_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3446 2024-03-12 17:22:57.000000 tulflow-0.9.9/tulflow/tasks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3102 2024-03-12 17:22:57.000000 tulflow-0.9.9/tulflow/transform.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6409 2024-03-12 17:22:57.000000 tulflow-0.9.9/tulflow/validate.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-03-12 17:23:04.915201 tulflow-0.9.9/tulflow.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2030 2024-03-12 17:23:04.000000 tulflow-0.9.9/tulflow.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      482 2024-03-12 17:23:04.000000 tulflow-0.9.9/tulflow.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-03-12 17:23:04.000000 tulflow-0.9.9/tulflow.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2024-03-12 17:23:04.000000 tulflow-0.9.9/tulflow.egg-info/top_level.txt
```

### Comparing `tulflow-0.9.8/LICENSE` & `tulflow-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/PKG-INFO` & `tulflow-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulflow
-Version: 0.9.8
+Version: 0.9.9
 Summary: Package of Temple University Library Indexing & ETL functions used by Airflow.
 Home-page: https://github.com/tulibraries/tulflow
 Author: Temple University Libraries
 Author-email: tul08567@temple.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tulflow-0.9.8/README.md` & `tulflow-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/setup.py` & `tulflow-0.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """tulflow Python package setup."""
 
 import os
 import sys
 import setuptools
 from setuptools.command.install import install
 
-VERSION = "v0.9.8"
+VERSION = "v0.9.9"
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
 class VerifyVersionCommand(install):
     """Custom command to verify that the git tag matches our version"""
     description = 'verify that the git tag matches our version'
```

### Comparing `tulflow-0.9.8/tests/test_devo-256_lxml_bug.py` & `tulflow-0.9.9/tests/test_devo-256_lxml_bug.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tests/test_harvest.py` & `tulflow-0.9.9/tests/test_harvest.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tests/test_process.py` & `tulflow-0.9.9/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tests/test_solr_api_utils.py` & `tulflow-0.9.9/tests/test_solr_api_utils.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tests/test_tasks.py` & `tulflow-0.9.9/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tests/test_transform.py` & `tulflow-0.9.9/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tests/test_validate.py` & `tulflow-0.9.9/tests/test_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import unittest
 import boto3
 from lxml import etree
 from unittest import mock
 from moto import mock_aws
 from tulflow import process, validate
 from unittest.mock import patch
-from airflow import AirflowException
+from airflow.exceptions import AirflowFailException
 
 class TestSchematronFiltering(unittest.TestCase):
     """Test Class for functions that filtering XML with Schematron."""
     maxDiff = None
     kwargs = {
         "source_prefix": "dpla_test/transformed",
         "destination_prefix": "dpla_test/transformed-filtered",
@@ -83,19 +83,19 @@
         self.assertEqual(test_object_exists["Contents"][0]["Key"], test_key)
 
         # mock schematron github retrieval response
         mocked_get_github_content.return_value = open("tests/fixtures/sch-sample.sch").read()
 
         # run tests
         with self.assertLogs() as log:
-            with self.assertRaises(AirflowException) as context:
+            with self.assertRaises(AirflowFailException) as context:
                 validate.filter_s3_schematron(**self.kwargs)
 
         errors = "All records were filtered out: 5"
-        exception = AirflowException(errors)
+        exception = AirflowFailException(errors)
         self.assertEqual(str(exception), str(context.exception))
 
         self.assertIn("INFO:root:Validating & Filtering File: dpla_test/transformed/sch-oai-invalid.xml", log.output)
         self.assertIn("ERROR:root:Invalid record found: invalid-missingtitle", log.output[1])
         self.assertIn("ERROR:root:Invalid record found: invalid-missingrights", log.output[2])
         self.assertIn('WARNING:root:All records filtered from dpla_test/transformed-filtered/sch-oai-invalid.xml. record_count: 5', log.output[6])
         self.assertEqual(len(log.output), 9)
```

### Comparing `tulflow-0.9.8/tulflow/harvest.py` & `tulflow-0.9.9/tulflow/harvest.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tulflow/process.py` & `tulflow-0.9.9/tulflow/process.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tulflow/solr_api_utils.py` & `tulflow-0.9.9/tulflow/solr_api_utils.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tulflow/tasks.py` & `tulflow-0.9.9/tulflow/tasks.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tulflow/transform.py` & `tulflow-0.9.9/tulflow/transform.py`

 * *Files identical despite different names*

### Comparing `tulflow-0.9.8/tulflow/validate.py` & `tulflow-0.9.9/tulflow/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Generic Data (primarily XML & JSON) Validation Methods."""
 import logging
 import csv
 import io
-from airflow import AirflowException
+from airflow.exceptions import AirflowFailException
 from lxml import etree, isoschematron
 from tulflow import process
 
 
 def filter_s3_schematron(**kwargs):
     """Wrapper function for using S3 Retrieval, Schematron Filtering, and S3 Writer."""
     source_prefix = kwargs.get("source_prefix")
@@ -66,15 +66,15 @@
             logging.warning(f"All records filtered from {filename}. record_count: {record_count}")
 
     invalid_filename = report_prefix + "-invalid.csv"
     logging.info("Total Filter Count: %s", total_filter_count)
     logging.info("Invalid Records report: https://%s.s3.amazonaws.com/%s", bucket, invalid_filename)
     process.generate_s3_object(csv_in_mem.getvalue(), bucket, invalid_filename, access_id, access_secret)
     if total_filter_count == total_record_count and total_record_count != 0:
-        raise AirflowException(f"All records were filtered out: {total_record_count}")
+        raise AirflowFailException(f"All records were filtered out: {total_record_count}") # pylint: disable
     return {"filtered": total_filter_count}
 
 def report_s3_schematron(**kwargs):
     """Wrapper function for using S3 Retrieval, Schematron Reporting, and S3 Writer."""
     source_prefix = kwargs.get("source_prefix")
     dest_prefix = kwargs.get("destination_prefix")
     bucket = kwargs.get("bucket")
```

### Comparing `tulflow-0.9.8/tulflow.egg-info/PKG-INFO` & `tulflow-0.9.9/tulflow.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulflow
-Version: 0.9.8
+Version: 0.9.9
 Summary: Package of Temple University Library Indexing & ETL functions used by Airflow.
 Home-page: https://github.com/tulibraries/tulflow
 Author: Temple University Libraries
 Author-email: tul08567@temple.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

