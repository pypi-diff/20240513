# Comparing `tmp/airflow_providers_wherobots-0.1.1.tar.gz` & `tmp/airflow_providers_wherobots-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airflow_providers_wherobots-0.1.1.tar", max compression
+gzip compressed data, was "airflow_providers_wherobots-0.1.2.tar", max compression
```

## Comparing `airflow_providers_wherobots-0.1.1.tar` & `airflow_providers_wherobots-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/LICENSE
--rw-r--r--   0        0        0     2441 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/hooks/__init__.py
--rw-r--r--   0        0        0     1873 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/hooks/sql.py
--rw-r--r--   0        0        0       57 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/hooks/wherobots.py
--rw-r--r--   0        0        0        0 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/operators/__init__.py
--rw-r--r--   0        0        0     2000 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/operators/sql.py
--rw-r--r--   0        0        0      492 2024-04-29 08:37:11.797088 airflow_providers_wherobots-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 airflow_providers_wherobots-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2436 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/hooks/__init__.py
+-rw-r--r--   0        0        0     1873 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/hooks/sql.py
+-rw-r--r--   0        0        0       57 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/hooks/wherobots.py
+-rw-r--r--   0        0        0        0 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/operators/__init__.py
+-rw-r--r--   0        0        0     2000 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/operators/sql.py
+-rw-r--r--   0        0        0      492 2024-05-13 03:06:51.851714 airflow_providers_wherobots-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3006 1970-01-01 00:00:00.000000 airflow_providers_wherobots-0.1.2/PKG-INFO
```

### Comparing `airflow_providers_wherobots-0.1.1/LICENSE` & `airflow_providers_wherobots-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow_providers_wherobots-0.1.1/README.md` & `airflow_providers_wherobots-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 The `WherobotsSqlOperator` allows you to run SQL queries on the
 Wherobots cloud, from which you can build your ETLs and data
 transformation workflows by querying, manipulating, and producing
 datasets with WherobotsDB.
 
 Refer to the [Wherobots Documentation](https://docs.wherobots.com) and
-this [guidance](https://docs.wherobots.services/1.2.2/tutorials/sedonadb/vector-data/vector-load/)
+this [guidance](https://docs.wherobots.com/1.2.2/tutorials/sedonadb/vector-data/vector-load/)
 to learn how to read data, transform data, and write results in Spatial
 SQL with WherobotsDB.
 
 ## Example
 
 Below is an example Airflow DAG that executes a SQL query on Wherobots
 Cloud:
```

### Comparing `airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/hooks/sql.py` & `airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/hooks/sql.py`

 * *Files identical despite different names*

### Comparing `airflow_providers_wherobots-0.1.1/airflow_providers_wherobots/operators/sql.py` & `airflow_providers_wherobots-0.1.2/airflow_providers_wherobots/operators/sql.py`

 * *Files identical despite different names*

### Comparing `airflow_providers_wherobots-0.1.1/PKG-INFO` & `airflow_providers_wherobots-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: airflow-providers-wherobots
-Version: 0.1.1
+Version: 0.1.2
 Summary: Airflow extension for communicating with Wherobots Cloud
 Author: zongsi.zhang
 Author-email: zongsi@wherobots.com
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: wherobots-python-dbapi (>=0.4.0,<0.5.0)
+Requires-Dist: wherobots-python-dbapi (>=0.5.0,<0.6.0)
 Description-Content-Type: text/markdown
 
 # Airflow Providers for Wherobots
 
 Airflow providers to bring [Wherobots Cloud](https://www.wherobots.com)'s
 spatial compute to your data workflows and ETLs.
 
@@ -58,15 +58,15 @@
 
 The `WherobotsSqlOperator` allows you to run SQL queries on the
 Wherobots cloud, from which you can build your ETLs and data
 transformation workflows by querying, manipulating, and producing
 datasets with WherobotsDB.
 
 Refer to the [Wherobots Documentation](https://docs.wherobots.com) and
-this [guidance](https://docs.wherobots.services/1.2.2/tutorials/sedonadb/vector-data/vector-load/)
+this [guidance](https://docs.wherobots.com/1.2.2/tutorials/sedonadb/vector-data/vector-load/)
 to learn how to read data, transform data, and write results in Spatial
 SQL with WherobotsDB.
 
 ## Example
 
 Below is an example Airflow DAG that executes a SQL query on Wherobots
 Cloud:
```

