# Comparing `tmp/spark_expectations-1.1.1.tar.gz` & `tmp/spark_expectations-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_expectations-1.1.1.tar", max compression
+gzip compressed data, was "spark_expectations-2.0.0.tar", max compression
```

## Comparing `spark_expectations-1.1.1.tar` & `spark_expectations-2.0.0.tar`

### file list

```diff
@@ -1,51 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-03-04 19:01:52.952699 spark_expectations-1.1.1/LICENSE
--rw-r--r--   0        0        0     7126 2024-03-04 19:01:52.952699 spark_expectations-1.1.1/README.md
--rw-r--r--   0        0        0     1950 2024-03-04 19:02:55.473414 spark_expectations-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      788 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/config/__init__.py
--rw-r--r--   0        0        0     2647 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/config/user_config.py
--rw-r--r--   0        0        0     1477 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/core/__init__.py
--rw-r--r--   0        0        0    49283 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/core/context.py
--rw-r--r--   0        0        0     1629 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/core/exceptions.py
--rw-r--r--   0        0        0    29528 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/core/expectations.py
--rw-r--r--   0        0        0        0 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/__init__.py
--rw-r--r--   0        0        0     7301 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/base_setup.py
--rwxr-xr-x   0        0        0      870 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/Dockerfile
--rw-r--r--   0        0        0      966 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/create_kafka_topic.sh
--rw-r--r--   0        0        0     1034 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/delete_kafka_topic.sh
--rw-r--r--   0        0        0      919 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/docker_kafka_start_script.sh
--rw-r--r--   0        0        0      330 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/docker_kafka_stop_script.sh
--rwxr-xr-x   0        0        0      218 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/kafka_cluster_start.sh
--rwxr-xr-x   0        0        0      141 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/kafka_cluster_stop.sh
--rwxr-xr-x   0        0        0      433 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/start-kafka.sh
--rw-r--r--   0        0        0     1366 2024-03-04 19:01:53.008700 spark_expectations-1.1.1/spark_expectations/examples/read_example_dataset.py
--rw-r--r--   0        0        0   385487 2024-03-04 19:01:53.012700 spark_expectations-1.1.1/spark_expectations/examples/resources/customer.csv
--rw-r--r--   0        0        0   122408 2024-03-04 19:01:53.012700 spark_expectations-1.1.1/spark_expectations/examples/resources/employee.csv
--rw-r--r--   0        0        0   981149 2024-03-04 19:01:53.016700 spark_expectations-1.1.1/spark_expectations/examples/resources/order.csv
--rw-r--r--   0        0        0   145357 2024-03-04 19:01:53.016700 spark_expectations-1.1.1/spark_expectations/examples/resources/product.csv
--rw-r--r--   0        0        0  2288625 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/examples/resources/superstore.csv
--rw-r--r--   0        0        0     4255 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/examples/sample_dq_bigquery.py
--rw-r--r--   0        0        0     3584 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/examples/sample_dq_delta.py
--rw-r--r--   0        0        0     3607 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/examples/sample_dq_iceberg.py
--rw-r--r--   0        0        0     1473 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/notifications/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/notifications/plugins/__init__.py
--rw-r--r--   0        0        0     1001 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/notifications/plugins/base_notification.py
--rw-r--r--   0        0        0     2242 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/notifications/plugins/email.py
--rw-r--r--   0        0        0     1907 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/notifications/plugins/slack.py
--rw-r--r--   0        0        0     2252 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/notifications/plugins/teams.py
--rw-r--r--   0        0        0        0 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/notifications/push/__init__.py
--rw-r--r--   0        0        0    11818 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/notifications/push/spark_expectations_notify.py
--rw-r--r--   0        0        0     4363 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/secrets/__init__.py
--rw-r--r--   0        0        0     1000 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/sinks/__init__.py
--rw-r--r--   0        0        0        0 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/sinks/plugins/__init__.py
--rw-r--r--   0        0        0      705 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/sinks/plugins/base_writer.py
--rw-r--r--   0        0        0     1616 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/sinks/plugins/kafka_writer.py
--rw-r--r--   0        0        0        0 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/sinks/utils/__init__.py
--rw-r--r--   0        0        0     1686 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/sinks/utils/collect_statistics.py
--rw-r--r--   0        0        0    23900 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/sinks/utils/writer.py
--rw-r--r--   0        0        0        0 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/utils/__init__.py
--rw-r--r--   0        0        0    11285 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/utils/actions.py
--rw-r--r--   0        0        0    11567 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/utils/reader.py
--rw-r--r--   0        0        0     6966 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/utils/regulate_flow.py
--rw-r--r--   0        0        0     1164 2024-03-04 19:01:53.024700 spark_expectations-1.1.1/spark_expectations/utils/udf.py
--rw-r--r--   0        0        0     7790 1970-01-01 00:00:00.000000 spark_expectations-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-13 20:26:46.507852 spark_expectations-2.0.0/LICENSE
+-rw-r--r--   0        0        0     7558 2024-05-13 20:26:46.507852 spark_expectations-2.0.0/README.md
+-rw-r--r--   0        0        0     1972 2024-05-13 20:27:41.516158 spark_expectations-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      788 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/config/__init__.py
+-rw-r--r--   0        0        0     3466 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/config/user_config.py
+-rw-r--r--   0        0        0     1477 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/core/__init__.py
+-rw-r--r--   0        0        0    60501 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/core/context.py
+-rw-r--r--   0        0        0     1629 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/core/exceptions.py
+-rw-r--r--   0        0        0    32124 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/core/expectations.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/__init__.py
+-rw-r--r--   0        0        0     8635 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/base_setup.py
+-rwxr-xr-x   0        0        0      870 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/Dockerfile
+-rw-r--r--   0        0        0      966 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/create_kafka_topic.sh
+-rw-r--r--   0        0        0     1034 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/delete_kafka_topic.sh
+-rw-r--r--   0        0        0      919 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/docker_kafka_start_script.sh
+-rw-r--r--   0        0        0      330 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/docker_kafka_stop_script.sh
+-rwxr-xr-x   0        0        0      218 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/kafka_cluster_start.sh
+-rwxr-xr-x   0        0        0      141 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/kafka_cluster_stop.sh
+-rwxr-xr-x   0        0        0      433 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/start-kafka.sh
+-rw-r--r--   0        0        0     1366 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/read_example_dataset.py
+-rw-r--r--   0        0        0   385487 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/resources/customer.csv
+-rw-r--r--   0        0        0      394 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/resources/customer_source.csv
+-rw-r--r--   0        0        0      474 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/resources/customer_target.csv
+-rw-r--r--   0        0        0   122408 2024-05-13 20:26:46.567852 spark_expectations-2.0.0/spark_expectations/examples/resources/employee.csv
+-rw-r--r--   0        0        0   981149 2024-05-13 20:26:46.567852 spark_expectations-2.0.0/spark_expectations/examples/resources/order_1.csv
+-rw-r--r--   0        0        0      585 2024-05-13 20:26:46.567852 spark_expectations-2.0.0/spark_expectations/examples/resources/order_s.csv
+-rw-r--r--   0        0        0      486 2024-05-13 20:26:46.567852 spark_expectations-2.0.0/spark_expectations/examples/resources/order_t.csv
+-rw-r--r--   0        0        0   145357 2024-05-13 20:26:46.571852 spark_expectations-2.0.0/spark_expectations/examples/resources/product.csv
+-rw-r--r--   0        0        0  2288625 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/examples/resources/superstore.csv
+-rw-r--r--   0        0        0     4529 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/examples/sample_dq_bigquery.py
+-rw-r--r--   0        0        0     4799 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/examples/sample_dq_delta.py
+-rw-r--r--   0        0        0     5154 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/examples/sample_dq_iceberg.py
+-rw-r--r--   0        0        0     1473 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/plugins/__init__.py
+-rw-r--r--   0        0        0     1001 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/plugins/base_notification.py
+-rw-r--r--   0        0        0     2242 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/plugins/email.py
+-rw-r--r--   0        0        0     1907 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/plugins/slack.py
+-rw-r--r--   0        0        0     2252 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/plugins/teams.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/push/__init__.py
+-rw-r--r--   0        0        0    11818 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/push/spark_expectations_notify.py
+-rw-r--r--   0        0        0     4363 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/secrets/__init__.py
+-rw-r--r--   0        0        0     1000 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/plugins/__init__.py
+-rw-r--r--   0        0        0      705 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/plugins/base_writer.py
+-rw-r--r--   0        0        0     1616 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/plugins/kafka_writer.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/utils/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/utils/collect_statistics.py
+-rw-r--r--   0        0        0    40326 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/utils/writer.py
+-rw-r--r--   0        0        0        0 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/utils/__init__.py
+-rw-r--r--   0        0        0    28072 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/utils/actions.py
+-rw-r--r--   0        0        0    17060 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/utils/reader.py
+-rw-r--r--   0        0        0     6966 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/utils/regulate_flow.py
+-rw-r--r--   0        0        0     1164 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/utils/udf.py
+-rw-r--r--   0        0        0     8222 1970-01-01 00:00:00.000000 spark_expectations-2.0.0/PKG-INFO
```

### Comparing `spark_expectations-1.1.1/LICENSE` & `spark_expectations-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/README.md` & `spark_expectations-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -65,30 +65,35 @@
 ### Configurations
 
 In order to establish the global configuration parameter for DQ Spark Expectations, you must define and complete the 
 required fields within a variable. This involves creating a variable and ensuring that all the necessary information 
 is provided in the appropriate fields.
 
 ```python
-from spark_expectations.config.user_config import *
+from spark_expectations.config.user_config import Constants as user_config
 
 se_user_conf = {
-    se_notifications_enable_email: False,
-    se_notifications_email_smtp_host: "mailhost.nike.com",
-    se_notifications_email_smtp_port: 25,
-    se_notifications_email_from: "<sender_email_id>",
-    se_notifications_email_to_other_nike_mail_id: "<receiver_email_id's>",
-    se_notifications_email_subject: "spark expectations - data quality - notifications", 
-    se_notifications_enable_slack: True,
-    se_notifications_slack_webhook_url: "<slack-webhook-url>", 
-    se_notifications_on_start: True, 
-    se_notifications_on_completion: True,
-    se_notifications_on_fail: True,
-    se_notifications_on_error_drop_exceeds_threshold_breach: True, 
-    se_notifications_on_error_drop_threshold: 15,
+    user_config.se_notifications_enable_email: False,
+    user_config.se_notifications_email_smtp_host: "mailhost.nike.com",
+    user_config.se_notifications_email_smtp_port: 25,
+    user_config.se_notifications_email_from: "<sender_email_id>",
+    user_config.se_notifications_email_to_other_nike_mail_id: "<receiver_email_id's>",
+    user_config.se_notifications_email_subject: "spark expectations - data quality - notifications", 
+    user_config.se_notifications_enable_slack: True,
+    user_config.se_notifications_slack_webhook_url: "<slack-webhook-url>", 
+    user_config.se_notifications_on_start: True, 
+    user_config.se_notifications_on_completion: True,
+    user_config.se_notifications_on_fail: True,
+    user_config.se_notifications_on_error_drop_exceeds_threshold_breach: True, 
+    user_config.se_notifications_on_error_drop_threshold: 15,
+    #Optional
+    #Below two params are optional and need to be enabled to capture the detailed stats in the <stats_table_name>_detailed.
+    #user_config.enable_query_dq_detailed_result: True,
+    #user_config.enable_agg_dq_detailed_result: True,
+    
 }
 ```
 
 ### Spark Expectations Initialization 
 
 For all the below examples the below import and SparkExpectations class instantiation is mandatory
```

### Comparing `spark_expectations-1.1.1/pyproject.toml` & `spark_expectations-2.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spark-expectations"
-version = "1.1.1"
+version = "2.0.0"
 description = "This project helps us to run Data Quality Rules in flight while spark job is being run"
 authors = ["Ashok Singamaneni <ashok.singamaneni@nike.com>"]
 readme = "README.md"
 packages = [{ include = "spark_expectations" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.9"
@@ -29,14 +29,15 @@
 mkdocs-click = "0.8.0"
 types-requests = "2.28.11.16"
 types-setuptools = "67.7.0.2"
 cerberus-python-client= "2.5.4"
 mike = "1.1.2"
 pre-commit = "3.3.1"
 botocore = "1.29.133" # This is just for fixing the dependency resolution version on cerberus-python-client
+ipykernel = "^6.29.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 bump = true
 style = "semver"
```

### Comparing `spark_expectations-1.1.1/spark_expectations/__init__.py` & `spark_expectations-2.0.0/spark_expectations/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/core/__init__.py` & `spark_expectations-2.0.0/spark_expectations/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/core/context.py` & `spark_expectations-2.0.0/spark_expectations/core/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pylint: disable=too-many-lines
 import os
 from datetime import timezone
 from datetime import datetime
 from dataclasses import dataclass
 from uuid import uuid1
-from typing import Dict, Optional, List
+from typing import Dict, Optional, List, Tuple
 from pyspark.sql import DataFrame, SparkSession
 from spark_expectations.config.user_config import Constants as user_config
 from spark_expectations.core.exceptions import SparkExpectationsMiscException
 
 
 # TODO: Add exceptions to follow standardized naming conventions for _run_id, product_id and _dq_stats_table_name in
 #       the future
@@ -21,26 +21,29 @@
     product_id: str
     spark: SparkSession
 
     def __post_init__(self) -> None:
         self._run_id: str = f"{self.product_id}_{uuid1()}"
         self._run_date: str = self.set_run_date()
         self._dq_stats_table_name: Optional[str] = None
+        self._dq_detailed_stats_table_name: Optional[str] = None
         self._final_table_name: Optional[str] = None
         self._error_table_name: Optional[str] = None
         self._row_dq_rule_type_name: str = "row_dq"
         self._agg_dq_rule_type_name: str = "agg_dq"
         self._query_dq_rule_type_name: str = "query_dq"
         self._row_dq_status: str = "Skipped"
         self._source_agg_dq_status: str = "Skipped"
         self._final_agg_dq_status: str = "Skipped"
         self._source_query_dq_status: str = "Skipped"
         self._final_query_dq_status: str = "Skipped"
         self._dq_run_status: str = "Failed"
         self._dq_expectations: Optional[Dict[str, str]] = None
+        self._se_enable_error_table: bool = True
+        self._dq_rules_params: Dict[str, str] = {}
 
         # above configuration variable value has to be set to python
         self._dq_project_env_name = "spark_expectations"
         self._dq_config_file_name = "dq_spark_expectations_config.ini"
         self._dq_config_abs_path: Optional[str] = None
 
         self._enable_mail: bool = False
@@ -69,14 +72,20 @@
         )
 
         self._source_agg_dq_result: Optional[List[Dict[str, str]]] = None
         self._final_agg_dq_result: Optional[List[Dict[str, str]]] = None
         self._source_query_dq_result: Optional[List[Dict[str, str]]] = None
         self._final_query_dq_result: Optional[List[Dict[str, str]]] = None
 
+        self._source_agg_dq_detailed_stats: Optional[List[Tuple]] = None
+        self._source_query_dq_detailed_stats: Optional[List[Tuple]] = None
+
+        self._target_agg_dq_detailed_stats: Optional[List[Tuple]] = None
+        self._target_query_dq_detailed_stats: Optional[List[Tuple]] = None
+
         self._notification_on_start: bool = False
         self._notification_on_completion: bool = False
         self._notification_on_fail: bool = False
         self._error_drop_threshold: int = 100
 
         self._cerberus_url: str = "your_cerberus_url"
         self._cerberus_cred_path: str = "your_cerberus_sdb_path"
@@ -123,14 +132,27 @@
         self._num_dq_rules: int = 0
         self._summarized_row_dq_res: Optional[List[Dict[str, str]]] = None
         self._rules_error_per: Optional[List[dict]] = None
 
         self._target_and_error_table_writer_config: dict = {}
         self._stats_table_writer_config: dict = {}
 
+        # The below config is user config and will be enabled if detailed result is required for agg and query dq
+        self._enable_agg_dq_detailed_result: bool = False
+        self._enable_query_dq_detailed_result: bool = False
+
+        self._rules_execution_settings_config: Dict[str, str]
+        self._querydq_secondary_queries: dict
+
+        self._source_query_dq_output: Optional[List[dict]] = None
+
+        self._target_query_dq_output: Optional[List[dict]] = None
+
+        self._query_dq_output_custom_table_name: str
+
     @property
     def get_run_id(self) -> str:
         """
         Get run_id for the instance of spark-expectations class
 
         Returns:
             str: returns the run_id
@@ -1164,22 +1186,51 @@
         """
         This function sets start time row dq computation
         Returns:
             None
         """
         self._row_dq_start_time = datetime.now()
 
+    @property
+    def get_row_dq_start_time(self) -> datetime:
+        """
+        This function sets start time row dq computation
+        Returns:
+            None
+        """
+        if self._row_dq_start_time:
+            return self._row_dq_start_time
+        raise SparkExpectationsMiscException(
+            """The spark expectations context is not set completely, 
+            please assign '_row_dq_start_time'  before 
+            accessing it"""
+        )
+
     def set_row_dq_end_time(self) -> None:
         """
         This function sets end time row dq computation
         Returns:
             None
         """
         self._row_dq_end_time = datetime.now()
 
+    @property
+    def get_row_dq_end_time(self) -> datetime:
+        """
+        This function sets end time row dq computation
+        Returns:
+            None
+        """
+        if self._row_dq_end_time:
+            return self._row_dq_end_time
+        raise SparkExpectationsMiscException(
+            """The spark expectations context is not set completely, please assign '_row_dq_end_time'  before 
+            accessing it"""
+        )
+
     def set_dq_start_time(self) -> None:
         """
         This function sets start time dq computation
         Returns:
             None
         """
         self._dq_start_time = datetime.now()
@@ -1560,7 +1611,303 @@
     def get_stats_table_writer_config(self) -> dict:
         """
         This function returns stats table writer config
         Returns:
             dict: Returns stats_table_writer_config which in dict
         """
         return self._stats_table_writer_config
+
+    def set_agg_dq_detailed_stats_status(
+        self, agg_dq_detailed_result_status: bool
+    ) -> None:
+        """
+        Args:
+            _enable_agg_dq_detailed_result:
+        Returns:
+        """
+        self._enable_agg_dq_detailed_result = bool(agg_dq_detailed_result_status)
+
+    @property
+    def get_agg_dq_detailed_stats_status(self) -> bool:
+        """
+        This function returns whether to enable detailed result for Agg and Query dq is enabled or not
+        Returns: Returns _enable_agg_dq_detailed_result(bool)
+        """
+
+        return self._enable_agg_dq_detailed_result
+
+    def set_query_dq_detailed_stats_status(
+        self, query_dq_detailed_result_status: bool
+    ) -> None:
+        """
+        Args:
+            _enable_query_dq_detailed_result:
+        Returns:
+        """
+        self._enable_query_dq_detailed_result = bool(query_dq_detailed_result_status)
+
+    @property
+    def get_query_dq_detailed_stats_status(self) -> bool:
+        """
+        This function returns whether to enable detailed result for Agg and Query dq is enabled or not
+        Returns: Returns _enable_query_dq_detailed_result(bool)
+        """
+
+        return self._enable_query_dq_detailed_result
+
+    def set_source_agg_dq_detailed_stats(
+        self, source_agg_dq_detailed_stats: Optional[List[Tuple]] = None
+    ) -> None:
+        """
+        Args:
+            _source_agg_dq_detailed_stats:
+        Returns:
+        """
+        self._source_agg_dq_detailed_stats = source_agg_dq_detailed_stats
+
+    @property
+    def get_source_agg_dq_detailed_stats(self) -> Optional[List[Tuple]]:
+        """
+        This function returns the detailed result for Agg and Query dq
+        Returns: Returns _source_agg_dq_detailed_stats
+        """
+
+        return self._source_agg_dq_detailed_stats
+
+    def set_source_query_dq_detailed_stats(
+        self, source_query_dq_detailed_stats: Optional[List[Tuple]] = None
+    ) -> None:
+        """
+        Args:
+            _source_query_dq_detailed_stats:
+        Returns:
+        """
+        self._source_query_dq_detailed_stats = source_query_dq_detailed_stats
+
+    @property
+    def get_source_query_dq_detailed_stats(self) -> Optional[List[Tuple]]:
+        """
+        This function returns the detailed result for Agg and Query dq
+        Returns: Returns _source_query_dq_detailed_stats
+        """
+
+        return self._source_query_dq_detailed_stats
+
+    def set_target_agg_dq_detailed_stats(
+        self, target_agg_dq_detailed_stats: Optional[List[Tuple]] = None
+    ) -> None:
+        """
+        Args:
+            _target_agg_dq_detailed_stats:
+        Returns:
+        """
+        self._target_agg_dq_detailed_stats = target_agg_dq_detailed_stats
+
+    @property
+    def get_target_agg_dq_detailed_stats(self) -> Optional[List[Tuple]]:
+        """
+        This function returns the detailed result for Agg and Query dq
+        Returns: Returns _target_agg_dq_detailed_stats
+        """
+
+        return self._target_agg_dq_detailed_stats
+
+    def set_target_query_dq_detailed_stats(
+        self, target_query_dq_detailed_stats: Optional[List[Tuple]] = None
+    ) -> None:
+        """
+        Args:
+            _target_query_dq_detailed_stats:
+        Returns:
+        """
+        self._target_query_dq_detailed_stats = target_query_dq_detailed_stats
+
+    @property
+    def get_target_query_dq_detailed_stats(self) -> Optional[List[Tuple]]:
+        """
+        This function returns the detailed result for Agg and Query dq
+        Returns: Returns _target_query_dq_detailed_stats
+        """
+
+        return self._target_query_dq_detailed_stats
+
+    def set_dq_detailed_stats_table_name(
+        self, dq_detailed_stats_table_name: str
+    ) -> None:
+        self._dq_detailed_stats_table_name = dq_detailed_stats_table_name
+
+    @property
+    def get_dq_detailed_stats_table_name(self) -> str:
+        """
+        Get dq_stats_table_name to which the final stats of the dq job will be written into
+
+        Returns:
+            str: returns the dq_stats_table_name
+        """
+        if (
+            self.get_agg_dq_detailed_stats_status
+            or self.get_query_dq_detailed_stats_status
+        ) and self._dq_detailed_stats_table_name:
+            return self._dq_detailed_stats_table_name
+        raise SparkExpectationsMiscException(
+            """The spark expectations context is not set completely, please assign 
+            '_dq_detailed_stats_table_name' before 
+            accessing it"""
+        )
+
+    def set_query_dq_output_custom_table_name(
+        self, query_dq_output_custom_table_name: str
+    ) -> None:
+        self._query_dq_output_custom_table_name = query_dq_output_custom_table_name
+
+    @property
+    def get_query_dq_output_custom_table_name(self) -> str:
+        """
+        Get query_dq_detailed_stats_status to which the final output of the query of the querydq  will be written into
+
+        Returns:
+            str: returns the query_dq_output_custom_table_name
+        """
+        if (
+            self.get_query_dq_detailed_stats_status
+            and self._dq_detailed_stats_table_name
+        ):
+            return self._query_dq_output_custom_table_name
+        raise SparkExpectationsMiscException(
+            """The spark expectations context is not set completely, please assign 
+            '_dq_detailed_stats_table_name,query_dq_detailed_stats_status' before 
+            accessing it"""
+        )
+
+    def set_detailed_stats_table_writer_config(self, config: dict) -> None:
+        """
+        This function sets stats table writer config
+        Args:
+            config: dict
+        Returns: None
+        """
+        self._stats_table_writer_config = config
+
+    @property
+    def get_detailed_stats_table_writer_config(self) -> dict:
+        """
+        This function returns stats table writer config
+        Returns:
+            dict: Returns detailed_stats_table_writer_config which in dict
+        """
+        return self._stats_table_writer_config
+
+    def set_rules_execution_settings_config(self, config: dict) -> None:
+        """
+        This function sets stats table writer config
+        Args:
+            config: dict
+        Returns: None
+        """
+        self._rules_execution_settings_config = config
+
+    @property
+    def get_rules_execution_settings_config(self) -> dict:
+        """
+        This function returns stats table writer config
+        Returns:
+            dict: Returns detailed_stats_table_writer_config which in dict
+        """
+        return self._rules_execution_settings_config
+
+    def set_querydq_secondary_queries(self, querydq_secondary_queries: dict) -> None:
+        """
+        This function sets row dq secondary queries
+        Args:
+            querydq_secondary_queries: dict
+        Returns: None
+        """
+        self._querydq_secondary_queries = querydq_secondary_queries
+
+    @property
+    def get_querydq_secondary_queries(self) -> dict:
+        """
+        This function gets row dq secondary queries
+        Returns:
+            dict: Returns querydq_secondary_queries
+        """
+        return self._querydq_secondary_queries
+
+    def set_source_query_dq_output(
+        self, source_query_dq_output: Optional[List[dict]] = None
+    ) -> None:
+        """
+        This function sets row dq secondary queries
+        Args:
+            source_query_dq_output: List[dict]
+        Returns: None
+        """
+        self._source_query_dq_output = source_query_dq_output
+
+    @property
+    def get_source_query_dq_output(self) -> Optional[List[dict]]:
+        """
+        This function gets row dq secondary queries
+        Returns:
+            dict: Returns source_query_dq_output
+        """
+        return self._source_query_dq_output
+
+    def set_target_query_dq_output(
+        self, target_query_dq_output: Optional[List[dict]] = None
+    ) -> None:
+        """
+        This function sets row dq secondary queries
+        Args:
+            target_query_dq_output: List[dict]
+        Returns: None
+        """
+        self._target_query_dq_output = target_query_dq_output
+
+    @property
+    def get_target_query_dq_output(self) -> Optional[List[dict]]:
+        """
+        This function gets row dq secondary queries
+        Returns:
+            dict: Returns target_query_dq_output
+        """
+        return self._target_query_dq_output
+
+    def set_se_enable_error_table(self, _enable_error_table: bool) -> None:
+        """
+
+        Args:
+            _se_enable_error_table:
+
+        Returns:
+
+        """
+        self._se_enable_error_table = _enable_error_table
+
+    @property
+    def get_se_enable_error_table(self) -> bool:
+        """
+        This function returns whether to enable relational table or not
+        Returns: Returns _se_enable_error_table(bool)
+
+        """
+        return self._se_enable_error_table
+
+    def set_dq_rules_params(self, _dq_rules_params: dict) -> None:
+        """
+        This function set params for dq rules
+        Args:
+            _se_dq_rules_params:
+
+        Returns:
+
+        """
+        self._dq_rules_params = _dq_rules_params
+
+    @property
+    def get_dq_rules_params(self) -> dict:
+        """
+        This function returns params which are mapping in dq rules
+        Returns: _dq_rules_params(dict)
+
+        """
+        return self._dq_rules_params
```

### Comparing `spark_expectations-1.1.1/spark_expectations/core/exceptions.py` & `spark_expectations-2.0.0/spark_expectations/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/core/expectations.py` & `spark_expectations-2.0.0/spark_expectations/core/expectations.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,16 +67,20 @@
         )
         self.reader = SparkExpectationsReader(_context=self._context)
 
         self._context.set_target_and_error_table_writer_config(
             self.target_and_error_table_writer.build()
         )
         self._context.set_stats_table_writer_config(self.stats_table_writer.build())
+        self._context.set_detailed_stats_table_writer_config(
+            self.stats_table_writer.build()
+        )
         self._context.set_debugger_mode(self.debugger)
         self._context.set_dq_stats_table_name(self.stats_table)
+        self._context.set_dq_detailed_stats_table_name(f"{self.stats_table}_detailed")
         self.rules_df = self.rules_df.persist(StorageLevel.MEMORY_AND_DISK)
 
     # TODO Add target_error_table_writer and stats_table_writer as parameters to this function so this takes precedence
     #  if user provides it
     def with_expectations(
         self,
         target_table: str,
@@ -103,22 +107,28 @@
         Returns:
             Any: Returns a function which applied the expectations on dataset
         """
 
         def _except(func: Any) -> Any:
             # variable used for enabling notification at different level
 
-            _default_notification_dict: Dict[str, Union[str, int, bool]] = {
+            _default_notification_dict: Dict[
+                str, Union[str, int, bool, Dict[str, str]]
+            ] = {
                 user_config.se_notifications_on_start: False,
                 user_config.se_notifications_on_completion: False,
                 user_config.se_notifications_on_fail: True,
                 user_config.se_notifications_on_error_drop_exceeds_threshold_breach: False,
                 user_config.se_notifications_on_error_drop_threshold: 100,
+                user_config.se_enable_agg_dq_detailed_result: False,
+                user_config.se_enable_query_dq_detailed_result: False,
+                user_config.querydq_output_custom_table_name: f"{self.stats_table}_querydq_output",
             }
-            _notification_dict: Dict[str, Union[str, int, bool]] = (
+
+            _notification_dict: Dict[str, Union[str, int, bool, Dict[str, str]]] = (
                 {**_default_notification_dict, **user_conf}
                 if user_conf
                 else _default_notification_dict
             )
             _default_stats_streaming_dict: Dict[str, Union[bool, str]] = {
                 user_config.se_enable_streaming: True,
                 user_config.secret_type: "databricks",
@@ -132,23 +142,74 @@
             }
             _se_stats_streaming_dict: Dict[str, Any] = (
                 {**self.stats_streaming_options}
                 if self.stats_streaming_options
                 else _default_stats_streaming_dict
             )
 
+            enable_error_table = _notification_dict.get(
+                user_config.se_enable_error_table, True
+            )
+            self._context.set_se_enable_error_table(
+                enable_error_table if isinstance(enable_error_table, bool) else True
+            )
+
+            dq_rules_params = _notification_dict.get(user_config.se_dq_rules_params, {})
+            self._context.set_dq_rules_params(
+                dq_rules_params if isinstance(dq_rules_params, dict) else {}
+            )
+
             # Overwrite the writers if provided by the user in the with_expectations explicitly
             if target_and_error_table_writer:
                 self._context.set_target_and_error_table_writer_config(
                     target_and_error_table_writer.build()
                 )
 
+            _agg_dq_detailed_stats: bool = (
+                bool(_notification_dict[user_config.se_enable_agg_dq_detailed_result])
+                if isinstance(
+                    _notification_dict[user_config.se_enable_agg_dq_detailed_result],
+                    bool,
+                )
+                else False
+            )
+
+            _query_dq_detailed_stats: bool = (
+                bool(_notification_dict[user_config.se_enable_query_dq_detailed_result])
+                if isinstance(
+                    _notification_dict[user_config.se_enable_query_dq_detailed_result],
+                    bool,
+                )
+                else False
+            )
+
+            if _agg_dq_detailed_stats or _query_dq_detailed_stats:
+                if _agg_dq_detailed_stats:
+                    self._context.set_agg_dq_detailed_stats_status(
+                        _agg_dq_detailed_stats
+                    )
+
+                if _query_dq_detailed_stats:
+                    self._context.set_query_dq_detailed_stats_status(
+                        _query_dq_detailed_stats
+                    )
+
+                self._context.set_query_dq_output_custom_table_name(
+                    str(
+                        _notification_dict[user_config.querydq_output_custom_table_name]
+                    )
+                )
+
             # need to call the get_rules_frm_table function to get the rules from the table as expectations
-            expectations, rules_execution_settings = self.reader.get_rules_from_df(
-                self.rules_df, target_table
+            (
+                dq_queries_dict,
+                expectations,
+                rules_execution_settings,
+            ) = self.reader.get_rules_from_df(
+                self.rules_df, target_table, params=self._context.get_dq_rules_params
             )
 
             _row_dq: bool = rules_execution_settings.get("row_dq", False)
             _source_agg_dq: bool = rules_execution_settings.get("source_agg_dq", False)
             _target_agg_dq: bool = rules_execution_settings.get("target_agg_dq", False)
             _source_query_dq: bool = rules_execution_settings.get(
                 "source_query_dq", False
@@ -196,35 +257,33 @@
                     _notification_dict[
                         user_config.se_notifications_on_error_drop_exceeds_threshold_breach
                     ],
                     bool,
                 )
                 else False
             )
+
+            notifications_on_error_drop_threshold = _notification_dict.get(
+                user_config.se_notifications_on_error_drop_threshold, 100
+            )
             _error_drop_threshold: int = (
-                int(
-                    _notification_dict[
-                        user_config.se_notifications_on_error_drop_threshold
-                    ]
-                )
-                if isinstance(
-                    _notification_dict[
-                        user_config.se_notifications_on_error_drop_threshold
-                    ],
-                    int,
-                )
+                notifications_on_error_drop_threshold
+                if isinstance(notifications_on_error_drop_threshold, int)
                 else 100
             )
 
             self.reader.set_notification_param(user_conf)
             self._context.set_notification_on_start(_notification_on_start)
             self._context.set_notification_on_completion(_notification_on_completion)
             self._context.set_notification_on_fail(_notification_on_fail)
 
             self._context.set_se_streaming_stats_dict(_se_stats_streaming_dict)
+            self._context.set_dq_expectations(expectations)
+            self._context.set_rules_execution_settings_config(rules_execution_settings)
+            self._context.set_querydq_secondary_queries(dq_queries_dict)
 
             @self._notification.send_notification_decorator
             @self._statistics_decorator.collect_stats_decorator
             @functools.wraps(func)
             def wrapper(*args: tuple, **kwargs: dict) -> DataFrame:
                 try:
                     _log.info("The function dataframe is getting created")
@@ -412,14 +471,15 @@
                             self._context.set_final_agg_dq_start_time()
                             # In this steps final agg data quality expectations run on final dataframe
                             # returns:
                             #        _final_dq_df: applied data quality dataframe at row level on raw dataframe,
                             #        _dq_final_agg_results: final agg dq result in dictionary
                             #        _: number of error records
                             #        status: status of the execution
+
                             (
                                 _final_dq_df,
                                 _dq_final_agg_results,
                                 _,
                                 status,
                             ) = func_process(
                                 _row_dq_df,
```

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/base_setup.py` & `spark_expectations-2.0.0/spark_expectations/examples/base_setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,34 +14,40 @@
     action_if_failed STRING,
     tag STRING,
     description STRING,
     enable_for_source_dq_validation BOOLEAN, 
     enable_for_target_dq_validation BOOLEAN,
     is_active BOOLEAN,
     enable_error_drop_alert BOOLEAN,
-    error_drop_threshold INT )
+    error_drop_threshold INT ,
+    query_dq_delimiter STRING,
+    enable_querydq_custom_output BOOLEAN
+    )
 """
 
+
 RULES_DATA = """ 
-    ("your_product", "dq_spark_local.customer_order",  "row_dq", "customer_id_is_not_null", "customer_id", "customer_id is not null","drop", "validity", "customer_id ishould not be null", true, true,false, false, 0)
-    ,("your_product", "dq_spark_local.customer_order", "row_dq", "sales_greater_than_zero", "sales", "sales > 2", "drop", "accuracy", "sales value should be greater than zero", true, true, true, false, 0)
-    ,("your_product", "dq_spark_local.customer_order", "row_dq", "discount_threshold", "discount", "discount*100 < 60","drop", "validity", "discount should be less than 40", true, true, false, false, 0)
-    ,("your_product", "dq_spark_local.customer_order", "row_dq", "ship_mode_in_set", "ship_mode", "lower(trim(ship_mode)) in('second class', 'standard class', 'standard class')", "drop", "validity", "ship_mode mode belongs in the sets", true, true, false, false, 0)
-    ,("your_product", "dq_spark_local.customer_order", "row_dq", "profit_threshold", "profit", "profit>0", "drop", "validity", "profit threshold should be greater tahn 0", true, true, false, true, 0)
+
+     ("your_product", "dq_spark_dev.customer_order", "row_dq", "sales_greater_than_zero", "sales", "sales > 2", "ignore", "accuracy", "sales value should be greater than zero", false, true, true, false, 0,null, null)
+    ,("your_product", "dq_spark_{env}.customer_order", "row_dq", "discount_threshold", "discount", "discount*100 < 60","drop", "validity", "discount should be less than 40", true, true, true, false, 0,null, null)
+    ,("your_product", "dq_spark_{env}.customer_order", "row_dq", "ship_mode_in_set", "ship_mode", "lower(trim(ship_mode)) in('second class', 'standard class', 'standard class')", "drop", "validity", "ship_mode mode belongs in the sets", true, true, true, false, 0,null, null)
+    ,("your_product", "dq_spark_{env}.customer_order", "row_dq", "profit_threshold", "profit", "profit>0", "ignore", "validity", "profit threshold should be greater tahn 0", false, true, false, true, 0,null, null)
+    ,("your_product", "dq_spark_dev.customer_order", "agg_dq", "sum_of_sales_range type 1", "sales", "sum(sales)>99 and sum(sales)<99999", "ignore", "validity", "regex format validation for quantity",  true, true, true, false, 0, null, true)
+    ,("your_product", "dq_spark_dev.customer_order", "agg_dq", "sum_of_sales_range type 2", "sales", "sum(sales) between 100 and 10000 ", "ignore", "validity", "regex format validation for quantity", true, true, true, false, 0, null, true)
+    ,("your_product", "dq_spark_dev.customer_order", "agg_dq", "sum_of_sales", "sales", "sum(sales)>10000", "ignore", "validity", "regex format validation for quantity",  true, true, true, false, 0,null, null)
+    ,("your_product", "dq_spark_dev.customer_order", "agg_dq", "sum_of_quantity", "quantity", "sum(quantity)>10000", "ignore", "validity", "regex format validation for quantity", true, true, true, false, 0,null, null)
+    ,("your_product", "dq_spark_dev.customer_order", "query_dq", "product_missing_count_threshold", "*", "((select count(*) from ({source_f1}) a) - (select count(*) from ({target_f1}) b) ) < 3@source_f1@select distinct product_id,order_id from order_source@target_f1@select distinct product_id,order_id from order_target", "ignore", "validity", "row count threshold", true, true, true, false, 0,null, true)
+    ,("your_product", "dq_spark_dev.customer_order", "query_dq", "customer_missing_count_threshold","*", "((select count(*) from ({source_f1}) a join ({source_f2}) b on a.customer_id = b.customer_id) - (select count(*) from ({target_f1}) a join ({target_f2}) b on a.customer_id = b.customer_id)) > ({target_f3})@source_f1@select customer_id, count(*) from customer_source group by customer_id@source_f2@select customer_id, count(*) from order_source group by customer_id@target_f1@select customer_id, count(*) from customer_target group by customer_id@target_f2@select customer_id, count(*) from order_target group by customer_id@target_f3@select count(*) from order_source", "ignore", "validity", "customer count threshold", true, true, true, false, 0,null, true)
+    ,("your_product", "dq_spark_dev.customer_order", "query_dq", "order_count_validity", "*", "({source_f1}) > 10@source_f1@select count(*) from order_source", "ignore", "validity", "row count threshold", true, true, true, false, 0, "@", true)
+    ,("your_product", "dq_spark_dev.customer_order", "query_dq", "order_count_validity_check", "*", "(select count(*) from order_source) > 10", "ignore", "validity", "row count threshold", true, true, true, false, 0, null, true)
+    ,("your_product", "dq_spark_{env}.customer_order", "query_dq", "product_category", "*", "(select count(distinct category) from {table}) < 5", "ignore", "validity", "distinct product category", true, true, true, false, 0,null, true)
+    ,("your_product", "dq_spark_{env}.customer_order", "agg_dq", "distinct_of_ship_mode", "ship_mode", "count(distinct ship_mode) <= 3", "ignore", "validity", "regex format validation for quantity", true, true, true, false, 0,null, null)
     
-    ,("your_product", "dq_spark_local.customer_order", "agg_dq", "sum_of_sales", "sales", "sum(sales)>10000", "ignore", "validity", "regex format validation for quantity",  true, true, true, false, 0)
-    ,("your_product", "dq_spark_local.customer_order", "agg_dq", "sum_of_quantity", "quantity", "sum(sales)>10000", "ignore", "validity", "regex format validation for quantity", true, true, true, false, 0)
-    ,("your_product", "dq_spark_local.customer_order", "agg_dq", "distinct_of_ship_mode", "ship_mode", "count(distinct ship_mode)<=3", "ignore", "validity", "regex format validation for quantity", true, true, true, false, 0)
-    ,("your_product", "dq_spark_local.customer_order", "agg_dq", "row_count", "*", "count(*)>=10000", "ignore", "validity", "regex format validation for quantity", true, true, true, false, 0)
-
-    ,("your_product", "dq_spark_local.customer_order", "query_dq", "product_missing_count_threshold", "*", "((select count(distinct product_id) from product) - (select count(distinct product_id) from order))>(select count(distinct product_id) from product)*0.2", "ignore", "validity", "row count threshold", true, true, true, false, 0)
-    ,("your_product", "dq_spark_local.customer_order", "query_dq", "product_category", "*", "(select count(distinct category) from product) < 5", "ignore", "validity", "distinct product category", true, true, true, false, 0)
-    ,("your_product", "dq_spark_local.customer_order", "query_dq", "row_count_in_order", "*", "(select count(*) from order)<10000", "ignore", "accuracy", "count of the row in order dataset", true, true, true, false, 0)
     
-"""
+    """
 
 
 def set_up_kafka() -> None:
     print("create or run if exist docker container")
     os.system(f"sh {CURRENT_DIR}/docker_scripts/docker_kafka_start_script.sh")
 
 
@@ -127,21 +133,23 @@
         )
         .config("spark.sql.warehouse.dir", "/tmp/hive/warehouse")
         .config("spark.driver.extraJavaOptions", "-Dderby.system.home=/tmp/derby")
         .config("spark.jars.ivy", "/tmp/ivy2")
     )
     spark = builder.getOrCreate()
 
-    os.system("rm -rf /tmp/hive/warehouse/dq_spark_local.db")
+    os.system("rm -rf /tmp/hive/warehouse/dq_spark_dev.db")
 
-    spark.sql("create database if not exists dq_spark_local")
-    spark.sql("use dq_spark_local")
+    spark.sql("create database if not exists dq_spark_dev")
+    spark.sql("use dq_spark_dev")
 
     spark.sql("drop table if exists dq_stats")
 
     spark.sql("drop table if exists dq_rules")
 
     spark.sql(f" CREATE TABLE dq_rules {RULES_TABLE_SCHEMA} USING DELTA")
+
     spark.sql(f" INSERT INTO dq_rules  values {RULES_DATA}")
 
     spark.sql("select * from dq_rules").show(truncate=False)
+
     return spark
```

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/Dockerfile` & `spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/Dockerfile`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/create_kafka_topic.sh` & `spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/create_kafka_topic.sh`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/delete_kafka_topic.sh` & `spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/delete_kafka_topic.sh`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/docker_scripts/docker_kafka_start_script.sh` & `spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/docker_kafka_start_script.sh`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/read_example_dataset.py` & `spark_expectations-2.0.0/spark_expectations/examples/read_example_dataset.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/resources/customer.csv` & `spark_expectations-2.0.0/spark_expectations/examples/resources/customer.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/resources/employee.csv` & `spark_expectations-2.0.0/spark_expectations/examples/resources/employee.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/resources/order.csv` & `spark_expectations-2.0.0/spark_expectations/examples/resources/order_1.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/resources/product.csv` & `spark_expectations-2.0.0/spark_expectations/examples/resources/product.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/resources/superstore.csv` & `spark_expectations-2.0.0/spark_expectations/examples/resources/superstore.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/sample_dq_bigquery.py` & `spark_expectations-2.0.0/spark_expectations/examples/sample_dq_bigquery.py`

 * *Files 7% similar despite different names*

```diff
@@ -52,14 +52,21 @@
     user_config.se_notifications_enable_slack: False,
     user_config.se_notifications_slack_webhook_url: "",
     user_config.se_notifications_on_start: True,
     user_config.se_notifications_on_completion: True,
     user_config.se_notifications_on_fail: True,
     user_config.se_notifications_on_error_drop_exceeds_threshold_breach: True,
     user_config.se_notifications_on_error_drop_threshold: 15,
+    user_config.se_enable_query_dq_detailed_result: True,
+    user_config.se_enable_agg_dq_detailed_result: True,
+    user_config.se_enable_error_table: True,
+    user_config.se_dq_rules_params: {
+        "env": "local",
+        "table": "product",
+    },
 }
 
 
 @se.with_expectations(
     target_table="<project_id>.<dataset_id>.<target_table_name>",
     write_to_table=True,
     user_conf=user_conf,
@@ -99,22 +106,24 @@
     spark.sql("select * from dq_spark_local.customer_order").show(truncate=False)
     spark.sql("select count(*) from dq_spark_local.customer_order_error").show(
         truncate=False
     )
 
     _log.info("stats data in the kafka topic")
     # display posted statistics from the kafka topic
+    """
     spark.read.format("kafka").option(
         "kafka.bootstrap.servers", "localhost:9092"
     ).option("subscribe", "dq-sparkexpectations-stats").option(
         "startingOffsets", "earliest"
     ).option(
         "endingOffsets", "latest"
     ).load().selectExpr(
         "cast(value as string) as stats_records"
     ).show(
         truncate=False
     )
+    """
 
     # remove docker container
     current_dir = os.path.dirname(os.path.abspath(__file__))
-    os.system(f"sh {current_dir}/docker_scripts/docker_kafka_stop_script.sh")
+    # os.system(f"sh {current_dir}/docker_scripts/docker_kafka_stop_script.sh")
```

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/sample_dq_delta.py` & `spark_expectations-2.0.0/spark_expectations/examples/sample_dq_iceberg.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,125 @@
 # mypy: ignore-errors
 import os
 
 from pyspark.sql import DataFrame
 from spark_expectations import _log
-from spark_expectations.examples.base_setup import set_up_delta
+from spark_expectations.examples.base_setup import set_up_iceberg
 from spark_expectations.core.expectations import (
     SparkExpectations,
     WrappedDataFrameWriter,
 )
 from spark_expectations.config.user_config import Constants as user_config
 
+writer = WrappedDataFrameWriter().mode("append").format("iceberg")
 
-writer = WrappedDataFrameWriter().mode("append").format("delta")
-
-spark = set_up_delta()
+spark = set_up_iceberg()
 
+print(spark.sparkContext.getConf().getAll())
 se: SparkExpectations = SparkExpectations(
     product_id="your_product",
-    rules_df=spark.table("dq_spark_local.dq_rules"),
+    rules_df=spark.sql("select * from dq_spark_local.dq_rules"),
     stats_table="dq_spark_local.dq_stats",
     stats_table_writer=writer,
     target_and_error_table_writer=writer,
     debugger=False,
-    # stats_streaming_options={user_config.se_enable_streaming: False},
+    stats_streaming_options={user_config.se_enable_streaming: False},
 )
 
-
 user_conf = {
     user_config.se_notifications_enable_email: False,
     user_config.se_notifications_email_smtp_host: "mailhost.com",
     user_config.se_notifications_email_smtp_port: 25,
     user_config.se_notifications_email_from: "",
     user_config.se_notifications_email_to_other_mail_id: "",
     user_config.se_notifications_email_subject: "spark expectations - data quality - notifications",
     user_config.se_notifications_enable_slack: False,
     user_config.se_notifications_slack_webhook_url: "",
     user_config.se_notifications_on_start: True,
     user_config.se_notifications_on_completion: True,
     user_config.se_notifications_on_fail: True,
     user_config.se_notifications_on_error_drop_exceeds_threshold_breach: True,
     user_config.se_notifications_on_error_drop_threshold: 15,
+    user_config.se_enable_query_dq_detailed_result: True,
+    user_config.se_enable_agg_dq_detailed_result: True,
+    user_config.se_enable_error_table: True,
+    user_config.enable_query_dq_detailed_result: True,
+    user_config.enable_agg_dq_detailed_result: True,
+    user_config.se_dq_rules_params: {
+        "env": "local",
+        "table": "product",
+    },
 }
 
 
 @se.with_expectations(
     target_table="dq_spark_local.customer_order",
     write_to_table=True,
     user_conf=user_conf,
     target_table_view="order",
 )
 def build_new() -> DataFrame:
-    _df_order: DataFrame = (
+    _df_order_source: DataFrame = (
         spark.read.option("header", "true")
         .option("inferSchema", "true")
-        .csv(os.path.join(os.path.dirname(__file__), "resources/order.csv"))
+        .csv(os.path.join(os.path.dirname(__file__), "resources/order_s.csv"))
     )
-    _df_order.createOrReplaceTempView("order")
+    _df_order_source.createOrReplaceTempView("order_source")
+
+    _df_order_target: DataFrame = (
+        spark.read.option("header", "true")
+        .option("inferSchema", "true")
+        .csv(os.path.join(os.path.dirname(__file__), "resources/order_t.csv"))
+    )
+    _df_order_target.createOrReplaceTempView("order_target")
 
     _df_product: DataFrame = (
         spark.read.option("header", "true")
         .option("inferSchema", "true")
         .csv(os.path.join(os.path.dirname(__file__), "resources/product.csv"))
     )
     _df_product.createOrReplaceTempView("product")
 
-    _df_customer: DataFrame = (
+    _df_customer_source: DataFrame = (
         spark.read.option("header", "true")
         .option("inferSchema", "true")
-        .csv(os.path.join(os.path.dirname(__file__), "resources/customer.csv"))
+        .csv(os.path.join(os.path.dirname(__file__), "resources/customer_source.csv"))
     )
 
-    _df_customer.createOrReplaceTempView("customer")
+    _df_customer_source.createOrReplaceTempView("customer_source")
 
-    return _df_order
+    _df_customer_target: DataFrame = (
+        spark.read.option("header", "true")
+        .option("inferSchema", "true")
+        .csv(os.path.join(os.path.dirname(__file__), "resources/customer_source.csv"))
+    )
+    _df_customer_target.createOrReplaceTempView("customer_target")
+
+    return _df_order_source
 
 
 if __name__ == "__main__":
     build_new()
 
+    # spark.sql("select * from dq_spark_local.dq_stats").show(truncate=False)
+    # spark.sql("select * from dq_spark_local.dq_stats").printSchema()
+    # spark.sql("select * from dq_spark_local.customer_order").show(truncate=False)
+    # spark.sql("select count(*) from dq_spark_local.customer_order_error").show(
+    #     truncate=False
+    # )
+
     spark.sql("use dq_spark_local")
     spark.sql("select * from dq_spark_local.dq_stats").show(truncate=False)
+    spark.sql("select * from dq_spark_local.dq_stats_detailed").show(truncate=False)
+    spark.sql("select * from dq_spark_local.dq_stats_querydq_output").show(
+        truncate=False
+    )
     spark.sql("select * from dq_spark_local.dq_stats").printSchema()
     spark.sql("select * from dq_spark_local.customer_order").show(truncate=False)
-    spark.sql("select count(*) from dq_spark_local.customer_order_error").show(
+    spark.sql("select count(*) from dq_spark_local.customer_order_error ").show(
         truncate=False
     )
 
     _log.info("stats data in the kafka topic")
     # display posted statistics from the kafka topic
     spark.read.format("kafka").option(
         "kafka.bootstrap.servers", "localhost:9092"
```

### Comparing `spark_expectations-1.1.1/spark_expectations/examples/sample_dq_iceberg.py` & `spark_expectations-2.0.0/spark_expectations/examples/sample_dq_delta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # mypy: ignore-errors
 import os
 
 from pyspark.sql import DataFrame
 from spark_expectations import _log
-from spark_expectations.examples.base_setup import set_up_iceberg
+from spark_expectations.examples.base_setup import set_up_delta
 from spark_expectations.core.expectations import (
     SparkExpectations,
     WrappedDataFrameWriter,
 )
 from spark_expectations.config.user_config import Constants as user_config
 
-writer = WrappedDataFrameWriter().mode("append").format("iceberg")
 
-spark = set_up_iceberg()
+writer = WrappedDataFrameWriter().mode("append").format("delta")
+
+spark = set_up_delta()
 
-print(spark.sparkContext.getConf().getAll())
 se: SparkExpectations = SparkExpectations(
     product_id="your_product",
-    rules_df=spark.sql("select * from dq_spark_local.dq_rules"),
-    stats_table="dq_spark_local.dq_stats",
+    rules_df=spark.table("dq_spark_dev.dq_rules"),
+    stats_table="dq_spark_dev.dq_stats",
     stats_table_writer=writer,
     target_and_error_table_writer=writer,
     debugger=False,
-    stats_streaming_options={user_config.se_enable_streaming: False},
+    # stats_streaming_options={user_config.se_enable_streaming: False},
 )
 
 user_conf = {
     user_config.se_notifications_enable_email: False,
     user_config.se_notifications_email_smtp_host: "mailhost.com",
     user_config.se_notifications_email_smtp_port: 25,
     user_config.se_notifications_email_from: "",
@@ -35,69 +35,98 @@
     user_config.se_notifications_enable_slack: False,
     user_config.se_notifications_slack_webhook_url: "",
     user_config.se_notifications_on_start: True,
     user_config.se_notifications_on_completion: True,
     user_config.se_notifications_on_fail: True,
     user_config.se_notifications_on_error_drop_exceeds_threshold_breach: True,
     user_config.se_notifications_on_error_drop_threshold: 15,
+    user_config.se_enable_query_dq_detailed_result: True,
+    user_config.se_enable_agg_dq_detailed_result: True,
+    # user_config.querydq_output_custom_table_name: "dq_spark_local.dq_stats_detailed_outputt",
+    user_config.se_enable_error_table: True,
+    user_config.se_dq_rules_params: {
+        "env": "dev",
+        "table": "product",
+    },
 }
 
 
 @se.with_expectations(
-    target_table="dq_spark_local.customer_order",
+    target_table="dq_spark_dev.customer_order",
     write_to_table=True,
     user_conf=user_conf,
     target_table_view="order",
 )
 def build_new() -> DataFrame:
-    _df_order: DataFrame = (
+    _df_order_source: DataFrame = (
+        spark.read.option("header", "true")
+        .option("inferSchema", "true")
+        .csv(os.path.join(os.path.dirname(__file__), "resources/order_s.csv"))
+    )
+    _df_order_source.createOrReplaceTempView("order_source")
+
+    _df_order_target: DataFrame = (
         spark.read.option("header", "true")
         .option("inferSchema", "true")
-        .csv(os.path.join(os.path.dirname(__file__), "resources/order.csv"))
+        .csv(os.path.join(os.path.dirname(__file__), "resources/order_t.csv"))
     )
-    _df_order.createOrReplaceTempView("order")
+    _df_order_target.createOrReplaceTempView("order_target")
 
     _df_product: DataFrame = (
         spark.read.option("header", "true")
         .option("inferSchema", "true")
         .csv(os.path.join(os.path.dirname(__file__), "resources/product.csv"))
     )
     _df_product.createOrReplaceTempView("product")
 
-    _df_customer: DataFrame = (
+    _df_customer_source: DataFrame = (
         spark.read.option("header", "true")
         .option("inferSchema", "true")
-        .csv(os.path.join(os.path.dirname(__file__), "resources/customer.csv"))
+        .csv(os.path.join(os.path.dirname(__file__), "resources/customer_source.csv"))
     )
 
-    _df_customer.createOrReplaceTempView("customer")
+    _df_customer_source.createOrReplaceTempView("customer_source")
+
+    _df_customer_target: DataFrame = (
+        spark.read.option("header", "true")
+        .option("inferSchema", "true")
+        .csv(os.path.join(os.path.dirname(__file__), "resources/customer_source.csv"))
+    )
+    _df_customer_target.createOrReplaceTempView("customer_target")
 
-    return _df_order
+    return _df_order_source
 
 
 if __name__ == "__main__":
     build_new()
 
-    spark.sql("select * from dq_spark_local.dq_stats").show(truncate=False)
-    spark.sql("select * from dq_spark_local.dq_stats").printSchema()
-    spark.sql("select * from dq_spark_local.customer_order").show(truncate=False)
-    spark.sql("select count(*) from dq_spark_local.customer_order_error").show(
-        truncate=False
-    )
+    spark.sql("use dq_spark_dev")
+    spark.sql("select * from dq_spark_dev.dq_stats").show(truncate=False)
+    spark.sql("select * from dq_spark_dev.dq_stats_detailed").show(truncate=False)
+    spark.sql("select * from dq_spark_dev.dq_stats_querydq_output").show(truncate=False)
+    spark.sql("select * from dq_spark_dev.dq_stats").printSchema()
+    spark.sql("select * from dq_spark_dev.dq_stats_detailed").printSchema()
+    spark.sql("select * from dq_spark_dev.customer_order").show(truncate=False)
+    # spark.sql("select count(*) from dq_spark_local.customer_order_error ").show(
+    #    truncate=False
+    # )
 
     _log.info("stats data in the kafka topic")
     # display posted statistics from the kafka topic
+
+    """
     spark.read.format("kafka").option(
         "kafka.bootstrap.servers", "localhost:9092"
     ).option("subscribe", "dq-sparkexpectations-stats").option(
         "startingOffsets", "earliest"
     ).option(
         "endingOffsets", "latest"
     ).load().selectExpr(
         "cast(value as string) as stats_records"
     ).show(
         truncate=False
     )
+    """
 
     # remove docker container
     current_dir = os.path.dirname(os.path.abspath(__file__))
-    os.system(f"sh {current_dir}/docker_scripts/docker_kafka_stop_script.sh")
+    # os.system(f"sh {current_dir}/docker_scripts/docker_kafka_stop_script.sh")
```

### Comparing `spark_expectations-1.1.1/spark_expectations/notifications/__init__.py` & `spark_expectations-2.0.0/spark_expectations/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/notifications/plugins/base_notification.py` & `spark_expectations-2.0.0/spark_expectations/notifications/plugins/base_notification.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/notifications/plugins/email.py` & `spark_expectations-2.0.0/spark_expectations/notifications/plugins/email.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/notifications/plugins/slack.py` & `spark_expectations-2.0.0/spark_expectations/notifications/plugins/slack.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/notifications/plugins/teams.py` & `spark_expectations-2.0.0/spark_expectations/notifications/plugins/teams.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/notifications/push/spark_expectations_notify.py` & `spark_expectations-2.0.0/spark_expectations/notifications/push/spark_expectations_notify.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/secrets/__init__.py` & `spark_expectations-2.0.0/spark_expectations/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/sinks/__init__.py` & `spark_expectations-2.0.0/spark_expectations/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/sinks/plugins/base_writer.py` & `spark_expectations-2.0.0/spark_expectations/sinks/plugins/base_writer.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/sinks/plugins/kafka_writer.py` & `spark_expectations-2.0.0/spark_expectations/sinks/plugins/kafka_writer.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/sinks/utils/collect_statistics.py` & `spark_expectations-2.0.0/spark_expectations/sinks/utils/collect_statistics.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/sinks/utils/writer.py` & `spark_expectations-2.0.0/spark_expectations/utils/actions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,566 +1,691 @@
-from dataclasses import dataclass
-from typing import Dict, Optional, Tuple, List
-from datetime import datetime
+from typing import Dict, List, Any, Optional, Tuple
+import re
 from pyspark.sql import DataFrame
+
+
 from pyspark.sql.functions import (
-    lit,
+    create_map,
     expr,
     when,
     array,
-    to_timestamp,
-    round as sql_round,
-    create_map,
-    explode,
-    to_json,
     col,
+    lit,
+    struct,
+    map_from_entries,
+    array_contains,
 )
-from spark_expectations import _log
+from spark_expectations.utils.udf import remove_empty_maps, get_actions_list
+from spark_expectations.core.context import SparkExpectationsContext
+from spark_expectations.config.user_config import Constants as constant_config
 from spark_expectations.core.exceptions import (
-    SparkExpectationsUserInputOrConfigInvalidException,
     SparkExpectationsMiscException,
+    SparkExpectOrFailException,
 )
-from spark_expectations.secrets import SparkExpectationsSecretsBackend
-from spark_expectations.utils.udf import remove_empty_maps
-from spark_expectations.core.context import SparkExpectationsContext
-from spark_expectations.sinks import _sink_hook
-from spark_expectations.config.user_config import Constants as user_config
 
 
-@dataclass
-class SparkExpectationsWriter:
+class SparkExpectationsActions:
     """
-    This class implements/supports writing data into the sink system
+    This class implements/supports applying data quality rules on given dataframe and performing required action
     """
 
-    _context: SparkExpectationsContext
+    @staticmethod
+    def get_rule_is_active(
+        _context: SparkExpectationsContext,
+        rule: dict,
+        _rule_type_name: str,
+        _source_dq_enabled: bool = False,
+        _target_dq_enabled: bool = False,
+    ) -> bool:
+        """
+        Args:
+            _context: SparkExpectationsContext class object
+            rule: dict with rule properties
+            _rule_type_name: which determines the type of the rule
+            _source_dq_enabled: Mark it as True when dq running for source dataframe
+            _target_dq_enabled: Mark it as True when dq running for target dataframe
+
+        Returns:
+
+        """
+        _is_active: bool = False
+        if (
+            _rule_type_name
+            in [
+                _context.get_query_dq_rule_type_name,
+                _context.get_agg_dq_rule_type_name,
+            ]
+            and _source_dq_enabled is True
+        ):
+            _is_active = rule["enable_for_source_dq_validation"]
+        elif (
+            _rule_type_name
+            in [
+                _context.get_query_dq_rule_type_name,
+                _context.get_agg_dq_rule_type_name,
+            ]
+            and _target_dq_enabled is True
+        ):
+            _is_active = rule["enable_for_target_dq_validation"]
 
-    def __post_init__(self) -> None:
-        self.spark = self._context.spark
+        return _is_active
 
-    def save_df_as_table(
-        self, df: DataFrame, table_name: str, config: dict, stats_table: bool = False
-    ) -> None:
+    @staticmethod
+    def create_rules_map(_rule_map: Dict[str, str]) -> Any:
         """
-        This function takes a dataframe and writes into a table
+        This function helps to extract the selected rules properties and returns array of dict with key and value
 
         Args:
-            df: Provide the dataframe which need to be written as a table
-            table_name: Provide the table name to which the dataframe need to be written to
-            config: Provide the config to write the dataframe into the table
-            stats_table: Provide if this is for writing stats table
+            _rule_map: dict with rules properties
+        Returns: Array of tuple with expectations rule properties
+
+        """
+        return array(
+            [
+                struct(lit(elem), lit(_rule_map.get(elem)))
+                for elem in [
+                    "rule_type",
+                    "rule",
+                    "action_if_failed",
+                    "tag",
+                    "description",
+                ]
+            ]
+        )
+
+    @staticmethod
+    def match_parentheses(dq_query_string: str) -> bool:
+        """
+        Check if the parentheses in the given query string are properly matched.
+
+        Args:
+            dq_query_string (str): The query string to check.
 
         Returns:
-            None:
+            bool: True if all parentheses are properly matched, False otherwise.
+        """
+        _parentheses_branch_check: List = []
+        for _index_val, _dq_query_string_char in enumerate(dq_query_string):
+            if _dq_query_string_char == "(":
+                _parentheses_branch_check.append(_index_val)
+            elif _dq_query_string_char == ")":
+                if not _parentheses_branch_check:
+                    return False
+                _parentheses_branch_check.pop()
+        return (
+            not _parentheses_branch_check
+        )  # return True if no unmatched left parentheses remain
+
+    @staticmethod
+    def agg_query_dq_detailed_result(
+        _context: SparkExpectationsContext,
+        _dq_rule: Dict[str, str],
+        df: DataFrame,
+        querydq_output: List[Tuple[str, str, str, str, Any, str, dict, str]],
+        _source_dq_status: bool = False,
+        _target_dq_status: bool = False,
+    ) -> Any:
+        """
+        Executes detailed result aggregation for query-based data quality rules.
+
+        Args:
+            _context (SparkExpectationsContext): The context object containing Spark session and other information.
+            _dq_rule (Dict[str, str]): The dictionary containing the data quality rule details.
+            df (DataFrame): The input DataFrame to be evaluated against the data quality rule.
+            querydq_output (List[Tuple[str, str, str, str, Any, str, dict, str]]):
+            The list to store the querydq output.
+            _source_dq_status (bool, optional):
+            The flag indicating if the rule is for source data quality. Defaults to False.
+            _target_dq_status (bool, optional):
+            The flag indicating if the rule is for target data quality. Defaults to False.
 
+        Returns:
+            Any: The querydq_output and detailed result of the data quality rule.
         """
+
         try:
-            print("run date ", self._context.get_run_date)
-            if not stats_table:
-                df = df.withColumn(
-                    self._context.get_run_id_name, lit(f"{self._context.get_run_id}")
-                ).withColumn(
-                    self._context.get_run_date_time_name,
-                    to_timestamp(
-                        lit(f"{self._context.get_run_date}"), "yyyy-MM-dd HH:mm:ss"
-                    ),
-                )
-            _log.info("_save_df_as_table started")
+            if (
+                _dq_rule["rule_type"] == _context.get_agg_dq_rule_type_name
+                and _context.get_agg_dq_detailed_stats_status is True
+            ):
+                if not (
+                    ">" in _dq_rule["expectation"] and "<" in _dq_rule["expectation"]
+                ):
+                    _pattern = rf"{constant_config.se_agg_dq_expectation_regex_pattern}"
+                    _re_compile = re.compile(_pattern)
+                    _agg_dq_expectation_match = re.match(
+                        _re_compile, _dq_rule["expectation"]
+                    )
+                    _agg_dq_expectation_expr = None
+                    if _agg_dq_expectation_match:
+                        _agg_dq_expectation_aggstring = _agg_dq_expectation_match.group(
+                            1
+                        )
+                        _agg_dq_expectation_expr = _agg_dq_expectation_match.group(2)
+                        _agg_dq_expectation_cond_expr = expr(
+                            _agg_dq_expectation_aggstring
+                        )
 
-            _df_writer = df.write
+                        _agg_dq_actual_count_value = int(
+                            df.agg(_agg_dq_expectation_cond_expr).collect()[0][0]
+                        )
 
-            if config["mode"] is not None:
-                _df_writer = _df_writer.mode(config["mode"])
-            if config["format"] is not None:
-                _df_writer = _df_writer.format(config["format"])
-            if config["partitionBy"] is not None and config["partitionBy"] != []:
-                _df_writer = _df_writer.partitionBy(config["partitionBy"])
-            if config["sortBy"] is not None and config["sortBy"] != []:
-                _df_writer = _df_writer.sortBy(config["sortBy"])
-            if config["bucketBy"] is not None and config["bucketBy"] != {}:
-                bucket_by_config = config["bucketBy"]
-                _df_writer = _df_writer.bucketBy(
-                    bucket_by_config["numBuckets"], bucket_by_config["colName"]
-                )
-            if config["options"] is not None and config["options"] != {}:
-                _df_writer = _df_writer.options(**config["options"])
+                        _agg_dq_expression_str = (
+                            str(_agg_dq_actual_count_value) + _agg_dq_expectation_expr
+                        )
 
-            _log.info("Writing records to table: %s", table_name)
+                        _agg_dq_expr_condition = []
 
-            if config["format"] == "bigquery":
-                _df_writer.option("table", table_name).save()
-            else:
-                _df_writer.saveAsTable(name=table_name)
-                _log.info("finished writing records to table: %s,", table_name)
-                if not stats_table:
-                    # Fetch table properties
-                    table_properties = self.spark.sql(
-                        f"SHOW TBLPROPERTIES {table_name}"
-                    ).collect()
-                    table_properties_dict = {
-                        row["key"]: row["value"] for row in table_properties
-                    }
+                        _agg_dq_expr_condition.append(
+                            when(expr(_agg_dq_expression_str), True)
+                            .otherwise(False)
+                            .alias("agg_dq_aggregation_check")
+                        )
 
-                    # Set product_id in table properties
-                    if (
-                        table_properties_dict.get("product_id") is None
-                        or table_properties_dict.get("product_id")
-                        != self._context.product_id
-                    ):
-                        _log.info(
-                            "product_id is not set for table %s in tableproperties, setting it now",
-                            table_name,
-                        )
-                        self.spark.sql(
-                            f"ALTER TABLE {table_name} SET TBLPROPERTIES ('product_id' = "
-                            f"'{self._context.product_id}')"
+                        _df_agg_dq_expr_result = df.select(*_agg_dq_expr_condition)
+
+                        # status = "pass" if eval(_agg_dq_expression_str) else "fail"
+
+                        status = (
+                            "pass"
+                            if _df_agg_dq_expr_result.filter(
+                                _df_agg_dq_expr_result["agg_dq_aggregation_check"]
+                            ).count()
+                            > 0
+                            else "fail"
                         )
 
-        except Exception as e:
-            raise SparkExpectationsUserInputOrConfigInvalidException(
-                f"error occurred while writing data in to the table - {table_name}: {e}"
-            )
+                        if _source_dq_status:
+                            row_count = _context.get_input_count
+                        elif _target_dq_status:
+                            row_count = _context.get_output_count
+                        else:
+                            row_count = None
+
+                        actual_row_count = row_count if status == "pass" else None
+                        error_row_count = 0 if status == "pass" else row_count
+
+                        actual_outcome = (
+                            _agg_dq_actual_count_value
+                            if (_agg_dq_actual_count_value is not None)
+                            else None
+                        )
+                        expected_outcome = (
+                            str(_agg_dq_expectation_expr)
+                            if (_agg_dq_expectation_expr is not None)
+                            else None
+                        )
+                else:
+                    pattern = (
+                        rf"{constant_config.se_agg_dq_expectation_range_regex_pattern}"
+                    )
+                    matches = re.match(pattern, _dq_rule["expectation"])
+                    result = None
+                    if matches:
+                        result = matches.groups()
+                        _agg_dq_expectation_aggstring = result[0]
+                        _agg_dq_expectation_expr_lowerbound = result[1]
+                        _agg_dq_expectation_expr_upperbound = result[4]
 
-    def write_error_stats(self) -> None:
-        """
-        This functions takes the stats table and write it into error table
+                        _agg_dq_expectation_cond_expr = expr(
+                            _agg_dq_expectation_aggstring
+                        )
 
-        Args:
-            config: Provide the config to write the dataframe into the table
+                        _agg_dq_actual_count_value = int(
+                            df.agg(_agg_dq_expectation_cond_expr).collect()[0][0]
+                        )
 
-        Returns:
-            None:
+                        _agg_dq_expression_str_lower = (
+                            str(_agg_dq_actual_count_value)
+                            + _agg_dq_expectation_expr_lowerbound
+                        )
 
-        """
-        try:
-            self.spark.conf.set("spark.sql.session.timeZone", "Etc/UTC")
-            from datetime import date
+                        _agg_dq_expression_str_upper = (
+                            str(_agg_dq_actual_count_value)
+                            + _agg_dq_expectation_expr_upperbound
+                        )
 
-            table_name: str = self._context.get_table_name
-            input_count: int = self._context.get_input_count
-            error_count: int = self._context.get_error_count
-            output_count: int = self._context.get_output_count
-            source_agg_dq_result: Optional[
-                List[Dict[str, str]]
-            ] = self._context.get_source_agg_dq_result
-            final_agg_dq_result: Optional[
-                List[Dict[str, str]]
-            ] = self._context.get_final_agg_dq_result
-            source_query_dq_result: Optional[
-                List[Dict[str, str]]
-            ] = self._context.get_source_query_dq_result
-            final_query_dq_result: Optional[
-                List[Dict[str, str]]
-            ] = self._context.get_final_query_dq_result
-
-            error_stats_data = [
-                (
-                    self._context.product_id,
-                    table_name,
-                    input_count,
-                    error_count,
-                    output_count,
-                    self._context.get_output_percentage,
-                    self._context.get_success_percentage,
-                    self._context.get_error_percentage,
-                    (
-                        source_agg_dq_result
-                        if source_agg_dq_result and len(source_agg_dq_result) > 0
-                        else None
-                    ),
-                    (
-                        final_agg_dq_result
-                        if final_agg_dq_result and len(final_agg_dq_result) > 0
-                        else None
-                    ),
-                    (
-                        source_query_dq_result
-                        if source_query_dq_result and len(source_query_dq_result) > 0
-                        else None
-                    ),
-                    (
-                        final_query_dq_result
-                        if final_query_dq_result and len(final_query_dq_result) > 0
-                        else None
-                    ),
-                    self._context.get_summarized_row_dq_res,
-                    self._context.get_rules_exceeds_threshold,
-                    {
-                        "run_status": self._context.get_dq_run_status,
-                        "source_agg_dq": self._context.get_source_agg_dq_status,
-                        "source_query_dq": self._context.get_source_query_dq_status,
-                        "row_dq": self._context.get_row_dq_status,
-                        "final_agg_dq": self._context.get_final_agg_dq_status,
-                        "final_query_dq": self._context.get_final_query_dq_status,
-                    },
-                    {
-                        "run_time": self._context.get_dq_run_time,
-                        "source_agg_dq_run_time": self._context.get_source_agg_dq_run_time,
-                        "source_query_dq_run_time": self._context.get_source_query_dq_run_time,
-                        "row_dq_run_time": self._context.get_row_dq_run_time,
-                        "final_agg_dq_run_time": self._context.get_final_agg_dq_run_time,
-                        "final_query_dq_run_time": self._context.get_final_query_dq_run_time,
-                    },
-                    {
-                        "rules": {
-                            "num_row_dq_rules": self._context.get_num_row_dq_rules,
-                            "num_dq_rules": self._context.get_num_dq_rules,
-                        },
-                        "agg_dq_rules": self._context.get_num_agg_dq_rules,
-                        "query_dq_rules": self._context.get_num_query_dq_rules,
-                    },
-                    self._context.get_run_id,
-                    date.fromisoformat(self._context.get_run_date[0:10]),
-                    datetime.strptime(
-                        self._context.get_run_date,
-                        "%Y-%m-%d %H:%M:%S",
-                    ),
-                )
-            ]
+                        _agg_dq_expr_condition = []
 
-            from pyspark.sql.types import (
-                StructType,
-                StructField,
-                StringType,
-                IntegerType,
-                LongType,
-                FloatType,
-                DateType,
-                ArrayType,
-                MapType,
-                TimestampType,
-            )
+                        _agg_dq_expression_str = (
+                            f"{str(_agg_dq_expression_str_lower)}"
+                            " and "
+                            f"{str(_agg_dq_expression_str_upper)}"
+                        )
 
-            error_stats_schema = StructType(
-                [
-                    StructField("product_id", StringType(), True),
-                    StructField("table_name", StringType(), True),
-                    StructField("input_count", LongType(), True),
-                    StructField("error_count", LongType(), True),
-                    StructField("output_count", LongType(), True),
-                    StructField("output_percentage", FloatType(), True),
-                    StructField("success_percentage", FloatType(), True),
-                    StructField("error_percentage", FloatType(), True),
-                    StructField(
-                        "source_agg_dq_results",
-                        ArrayType(MapType(StringType(), StringType())),
-                        True,
-                    ),
-                    StructField(
-                        "final_agg_dq_results",
-                        ArrayType(MapType(StringType(), StringType())),
-                        True,
-                    ),
-                    StructField(
-                        "source_query_dq_results",
-                        ArrayType(MapType(StringType(), StringType())),
-                        True,
-                    ),
-                    StructField(
-                        "final_query_dq_results",
-                        ArrayType(MapType(StringType(), StringType())),
-                        True,
-                    ),
-                    StructField(
-                        "row_dq_res_summary",
-                        ArrayType(MapType(StringType(), StringType())),
-                        True,
-                    ),
-                    StructField(
-                        "row_dq_error_threshold",
-                        ArrayType(MapType(StringType(), StringType())),
-                        True,
-                    ),
-                    StructField("dq_status", MapType(StringType(), StringType()), True),
-                    StructField(
-                        "dq_run_time", MapType(StringType(), FloatType()), True
-                    ),
-                    StructField(
-                        "dq_rules",
-                        MapType(StringType(), MapType(StringType(), IntegerType())),
-                        True,
-                    ),
-                    StructField(self._context.get_run_id_name, StringType(), True),
-                    StructField(self._context.get_run_date_name, DateType(), True),
-                    StructField(
-                        self._context.get_run_date_time_name, TimestampType(), True
-                    ),
-                ]
-            )
+                        _agg_dq_expr_condition.append(
+                            when(expr(_agg_dq_expression_str), True)
+                            .otherwise(False)
+                            .alias("agg_dq_aggregation_check")
+                        )
 
-            df = self.spark.createDataFrame(error_stats_data, schema=error_stats_schema)
-            self._context.print_dataframe_with_debugger(df)
+                        _df_agg_dq_expr_result = df.select(*_agg_dq_expr_condition)
 
-            df = (
-                df.withColumn("output_percentage", sql_round(df.output_percentage, 2))
-                .withColumn("success_percentage", sql_round(df.success_percentage, 2))
-                .withColumn("error_percentage", sql_round(df.error_percentage, 2))
-            )
-            _log.info(
-                "Writing metrics to the stats table: %s, started",
-                self._context.get_dq_stats_table_name,
-            )
-            if self._context.get_stats_table_writer_config["format"] == "bigquery":
-                df = df.withColumn("dq_rules", to_json(df["dq_rules"]))
+                        status = (
+                            "pass"
+                            if _df_agg_dq_expr_result.filter(
+                                _df_agg_dq_expr_result["agg_dq_aggregation_check"]
+                            ).count()
+                            > 0
+                            else "fail"
+                        )
 
-            self.save_df_as_table(
-                df,
-                self._context.get_dq_stats_table_name,
-                config=self._context.get_stats_table_writer_config,
-                stats_table=True,
-            )
+                        if _source_dq_status:
+                            row_count = _context.get_input_count
+                        elif _target_dq_status:
+                            row_count = _context.get_output_count
+                        else:
+                            row_count = None
+                        actual_row_count = row_count if status == "pass" else None
+                        error_row_count = 0 if status == "pass" else row_count
+
+                        actual_outcome = (
+                            _agg_dq_actual_count_value
+                            if (_agg_dq_actual_count_value is not None)
+                            else None
+                        )
 
-            _log.info(
-                "Writing metrics to the stats table: %s, ended",
-                {self._context.get_dq_stats_table_name},
-            )
+                        expected_outcome = (
+                            _agg_dq_expression_str
+                            if (
+                                _agg_dq_expression_str_lower is not None
+                                and _agg_dq_expression_str_upper is not None
+                            )
+                            else None
+                        )
+            elif (
+                _dq_rule["rule_type"] == _context.get_query_dq_rule_type_name
+                and _context.get_query_dq_detailed_stats_status is True
+            ):
+                _querydq_secondary_query = _context.get_querydq_secondary_queries
+
+                if _source_dq_status is True:
+                    _query_prefix = "_source_dq"
+                elif _target_dq_status is True:
+                    _query_prefix = "_target_dq"
+                else:
+                    _query_prefix = ""
 
-            # TODO check if streaming_stats is set to off, if it's enabled only then this should run
+                if (_dq_rule["enable_querydq_custom_output"]) and (
+                    sub_key_value := _querydq_secondary_query.get(
+                        _dq_rule["product_id"]
+                        + "|"
+                        + _dq_rule["table_name"]
+                        + "|"
+                        + _dq_rule["rule"],
+                        {},
+                    )
+                ):
+                    for _key, _querydq_query in sub_key_value.items():
+                        querydq_output.append(
+                            (
+                                _context.get_run_id,
+                                _dq_rule["product_id"],
+                                _dq_rule["table_name"],
+                                _dq_rule["rule"],
+                                _key,
+                                _query_prefix,
+                                dict(
+                                    [
+                                        (
+                                            _key,
+                                            _context.spark.sql(
+                                                _dq_rule["expectation" + "_" + _key]
+                                            )
+                                            .toJSON()
+                                            .collect(),
+                                        )
+                                    ]
+                                ),
+                                _context.get_run_date,
+                            )
+                        )
 
-            _se_stats_dict = self._context.get_se_streaming_stats_dict
-            if _se_stats_dict["se.enable.streaming"]:
-                secret_handler = SparkExpectationsSecretsBackend(
-                    secret_dict=_se_stats_dict
-                )
-                kafka_write_options: dict = (
-                    {
-                        "kafka.bootstrap.servers": "localhost:9092",
-                        "topic": self._context.get_se_streaming_stats_topic_name,
-                        "failOnDataLoss": "true",
-                    }
-                    if self._context.get_env == "local"
-                    else (
-                        {
-                            "kafka.bootstrap.servers": f"{secret_handler.get_secret(self._context.get_server_url_key)}",
-                            "kafka.security.protocol": "SASL_SSL",
-                            "kafka.sasl.mechanism": "OAUTHBEARER",
-                            "kafka.sasl.jaas.config": "kafkashaded.org.apache.kafka.common.security.oauthbearer."
-                            "OAuthBearerLoginModule required oauth.client.id="
-                            f"'{secret_handler.get_secret(self._context.get_client_id)}'  "
-                            + "oauth.client.secret="
-                            f"'{secret_handler.get_secret(self._context.get_token)}' "
-                            "oauth.token.endpoint.uri="
-                            f"'{secret_handler.get_secret(self._context.get_token_endpoint_url)}'; ",
-                            "kafka.sasl.login.callback.handler.class": "io.strimzi.kafka.oauth.client"
-                            ".JaasClientOauthLoginCallbackHandler",
-                            "topic": (
-                                self._context.get_se_streaming_stats_topic_name
-                                if self._context.get_env == "local"
-                                else secret_handler.get_secret(
-                                    self._context.get_topic_name
-                                )
-                            ),
-                        }
+                if SparkExpectationsActions.match_parentheses(_dq_rule["expectation"]):
+                    pattern = r"(\(.*\))\s*([<>!=]=?)\s*((\d+)|(\(.*\)))|(\(.*\))"
+                    match = re.search(pattern, _dq_rule["expectation"])
+                    if match:
+                        # function to execute SQL and get the result
+                        def execute_sql_and_get_result(
+                            _se_context: SparkExpectationsContext, query: str
+                        ) -> int:
+                            return (
+                                _se_context.spark.sql(
+                                    f"SELECT ({query}) AS OUTPUT"
+                                ).collect()[0][0]
+                                if query
+                                else None
+                            )
+
+                        # function to get the query outputs
+                        _querydq_source_query_output = execute_sql_and_get_result(
+                            _context, match.group(1)
+                        )
+                        _querydq_target_query_output = match.group(
+                            4
+                        ) or execute_sql_and_get_result(_context, match.group(5))
+
+                        # assignment of actual_outcome and expected_outcome
+                        actual_outcome = _querydq_source_query_output
+                        expected_outcome = (
+                            str(match.group(2)) + str(_querydq_target_query_output)
+                            if _querydq_target_query_output
+                            else None
+                        )
+
+                else:
+                    raise SparkExpectationsMiscException(
+                        """Sql query is invalid. Parentheses are missing in the sql query."""
                     )
-                )
 
-                _sink_hook.writer(
-                    _write_args={
-                        "product_id": self._context.product_id,
-                        "enable_se_streaming": _se_stats_dict[
-                            user_config.se_enable_streaming
-                        ],
-                        "kafka_write_options": kafka_write_options,
-                        "stats_df": df,
-                    }
+                _querydq_status_query = (
+                    "SELECT (" + str(_dq_rule["expectation"]) + ") AS OUTPUT"
                 )
-            else:
-                _log.info(
-                    "Streaming stats to kafka is disabled, hence skipping writing to kafka"
+
+                _query_dq_result = int(
+                    _context.spark.sql(_querydq_status_query).collect()[0][0]
                 )
 
-        except Exception as e:
-            raise SparkExpectationsMiscException(
-                f"error occurred while saving the data into the stats table {e}"
-            )
+                status = "pass" if _query_dq_result else "fail"
 
-    def write_error_records_final(
-        self, df: DataFrame, error_table: str, rule_type: str
-    ) -> Tuple[int, DataFrame]:
-        try:
-            _log.info("_write_error_records_final started")
+                if _source_dq_status:
+                    row_count = _context.get_input_count
+                elif _target_dq_status:
+                    row_count = _context.get_output_count
+                else:
+                    row_count = None
 
-            failed_records = [
-                f"size({dq_column}) != 0"
-                for dq_column in df.columns
-                if dq_column.startswith(f"{rule_type}")
-            ]
+                actual_row_count = row_count if _query_dq_result else None
 
-            failed_records_rules = " or ".join(failed_records)
-            # df = df.filter(expr(failed_records_rules))
+                error_row_count = 0 if _query_dq_result else row_count
 
-            df = df.withColumn(
-                f"meta_{rule_type}_results",
-                when(
-                    expr(failed_records_rules),
-                    array(
-                        *[
-                            _col
-                            for _col in df.columns
-                            if _col.startswith(f"{rule_type}")
-                        ]
-                    ),
-                ).otherwise(array(create_map())),
-            ).drop(*[_col for _col in df.columns if _col.startswith(f"{rule_type}")])
-
-            df = (
-                df.withColumn(
-                    f"meta_{rule_type}_results",
-                    remove_empty_maps(df[f"meta_{rule_type}_results"]),
-                )
-                .withColumn(
-                    self._context.get_run_id_name, lit(self._context.get_run_id)
-                )
-                .withColumn(
-                    self._context.get_run_date_time_name,
-                    lit(self._context.get_run_date),
-                )
+            else:
+                status = None
+                actual_row_count = None
+                error_row_count = None
+                row_count = None
+                actual_outcome = None
+                expected_outcome = None
+
+            return querydq_output, (
+                _context.get_run_id,
+                _dq_rule["product_id"],
+                _dq_rule["table_name"],
+                _dq_rule["rule_type"],
+                _dq_rule["rule"],
+                _dq_rule["expectation"],
+                _dq_rule["tag"],
+                _dq_rule["description"],
+                status,
+                actual_outcome,
+                expected_outcome,
+                actual_row_count,
+                error_row_count,
+                row_count,
             )
-            error_df = df.filter(f"size(meta_{rule_type}_results) != 0")
-            self._context.print_dataframe_with_debugger(error_df)
-
-            self.save_df_as_table(
-                error_df,
-                error_table,
-                self._context.get_target_and_error_table_writer_config,
+        except Exception as e:
+            raise SparkExpectationsMiscException(
+                f"error occurred while running agg_query_dq_detailed_result {e}"
             )
 
-            _error_count = error_df.count()
-            if _error_count > 0:
-                self.generate_summarized_row_dq_res(error_df, rule_type)
+    @staticmethod
+    def create_agg_dq_results(
+        _context: SparkExpectationsContext, _df: DataFrame, _rule_type_name: str
+    ) -> Optional[List[Dict[str, str]]]:
+        """
+        This function helps to collect the aggregation results in to the list
+         Args:
+             _context: SparkContext object
+             _df: dataframe which contains agg data quality results
+             _rule_type_name: which determines the type of the rule
+
+         Returns:
+                List with dict of agg rules property name and value
 
-            _log.info("_write_error_records_final ended")
-            return _error_count, df
 
+        """
+        try:
+            first_row = _df.first()
+            if (
+                first_row is not None
+                and f"meta_{_rule_type_name}_results" in _df.columns
+            ):
+                meta_results = first_row[f"meta_{_rule_type_name}_results"]
+                if meta_results is not None and len(meta_results) > 0:
+                    return meta_results
+            return None
         except Exception as e:
             raise SparkExpectationsMiscException(
-                f"error occurred while saving data into the final error table {e}"
+                f"error occurred while running create agg dq results {e}"
             )
 
-    def generate_summarized_row_dq_res(self, df: DataFrame, rule_type: str) -> None:
+    @staticmethod
+    def run_dq_rules(
+        _context: SparkExpectationsContext,
+        df: DataFrame,
+        expectations: Dict[str, List[dict]],
+        rule_type: str,
+        _source_dq_enabled: bool = False,
+        _target_dq_enabled: bool = False,
+    ) -> DataFrame:
         """
-        This function implements/supports summarizing row dq error result
+        This function builds the expressions for the data quality rules and returns the dataframe with results
+
         Args:
-            df: error dataframe(DataFrame)
-            rule_type: type of the rule(str)
+            _context: Provide SparkExpectationsContext
+            df: Input dataframe on which data quality rules need to be applied
+            expectations: Provide the dict which has all the rules
+            rule_type: identifier for the type of rule to be applied in processing
+            _source_dq_enabled: Mark it as True when dq running for source dataframe
+            _target_dq_enabled: Mark it as True when dq running for target dataframe
 
         Returns:
-            None
+            DataFrame: Returns a dataframe with all the rules run the input dataframe
 
         """
         try:
-            df_explode = df.select(
-                explode(f"meta_{rule_type}_results").alias("row_dq_res")
-            )
-            df_res = (
-                df_explode.withColumn("rule_type", col("row_dq_res")["rule_type"])
-                .withColumn("rule", col("row_dq_res")["rule"])
-                .withColumn("description", col("row_dq_res")["description"])
-                .withColumn("tag", col("row_dq_res")["tag"])
-                .withColumn("action_if_failed", col("row_dq_res")["action_if_failed"])
-                .select("rule_type", "rule", "description", "tag", "action_if_failed")
-                .groupBy("rule_type", "rule", "description", "tag", "action_if_failed")
-                .count()
-                .withColumnRenamed("count", "failed_row_count")
-            )
-            summarized_row_dq_list = [
-                {
-                    "rule_type": row.rule_type,
-                    "rule": row.rule,
-                    "description": row.description,
-                    "tag": row.tag,
-                    "action_if_failed": row.action_if_failed,
-                    "failed_row_count": row.failed_row_count,
-                }
-                for row in df_res.select(
-                    "rule_type",
-                    "rule",
-                    "description",
-                    "tag",
-                    "action_if_failed",
-                    "failed_row_count",
-                ).collect()
-            ]
-            failed_rule_list = []
-            for failed_rule in summarized_row_dq_list:
-                failed_rule_list.append(failed_rule["rule"])
-
-            for (
-                each_rule_type,
-                all_rule_type_rules,
-            ) in self._context.get_dq_expectations.items():
-                if each_rule_type in ["row_dq_rules"]:
-                    for each_rule in all_rule_type_rules:
-                        if each_rule["rule"] not in failed_rule_list:
-                            summarized_row_dq_list.append(
-                                {
-                                    "description": each_rule["description"],
-                                    "tag": each_rule["tag"],
-                                    "rule": each_rule["rule"],
-                                    "action_if_failed": each_rule["action_if_failed"],
-                                    "rule_type": each_rule["rule_type"],
-                                    "failed_row_count": 0,
-                                }
+            condition_expressions: List = []
+            _agg_query_dq_results: List = []
+            querydq_output: List = []
+            if len(expectations) <= 0:
+                raise SparkExpectationsMiscException("no rules found to process")
+
+            if (
+                f"{rule_type}_rules" not in expectations
+                or len(expectations[f"{rule_type}_rules"]) <= 0
+            ):
+                raise SparkExpectationsMiscException(
+                    f"zero expectations to process for {rule_type}_rules from the `dq_rules` table, "
+                    f"please configure rules or avoid this error by setting {rule_type} to False"
+                )
+
+            for rule in expectations[f"{rule_type}_rules"]:
+                _rule_is_active = SparkExpectationsActions.get_rule_is_active(
+                    _context,
+                    rule,
+                    rule_type,
+                    _source_dq_enabled=_source_dq_enabled,
+                    _target_dq_enabled=_target_dq_enabled,
+                )
+
+                if _rule_is_active or rule_type == _context.get_row_dq_rule_type_name:
+                    column = f"{rule_type}_{rule['rule']}"
+                    condition_expressions.append(
+                        when(expr(rule["expectation"]), create_map())
+                        .otherwise(
+                            map_from_entries(
+                                SparkExpectationsActions.create_rules_map(rule)
                             )
+                        )
+                        .alias(column)
+                    )
+                    if (
+                        rule_type
+                        in (
+                            _context.get_agg_dq_rule_type_name,
+                            _context.get_query_dq_rule_type_name,
+                        )
+                    ) and (
+                        _context.get_agg_dq_detailed_stats_status is True
+                        or _context.get_query_dq_detailed_stats_status is True
+                    ):
+                        (
+                            _querydq_output_list,
+                            _agg_query_dq_output_tuple,
+                        ) = SparkExpectationsActions.agg_query_dq_detailed_result(
+                            _context,
+                            rule,
+                            df,
+                            querydq_output,
+                            _source_dq_status=_source_dq_enabled,
+                            _target_dq_status=_target_dq_enabled,
+                        )
 
-            self._context.set_summarized_row_dq_res(summarized_row_dq_list)
+                        _agg_query_dq_results.append(_agg_query_dq_output_tuple)
+
+            if (
+                rule_type == _context.get_agg_dq_rule_type_name
+                and _context.get_agg_dq_detailed_stats_status is True
+                and _source_dq_enabled
+            ):
+                _context.set_source_agg_dq_detailed_stats(_agg_query_dq_results)
+
+            elif (
+                rule_type == _context.get_agg_dq_rule_type_name
+                and _context.get_agg_dq_detailed_stats_status is True
+                and _target_dq_enabled
+            ):
+                _context.set_target_agg_dq_detailed_stats(_agg_query_dq_results)
+
+            elif (
+                rule_type == _context.get_query_dq_rule_type_name
+                and _context.get_query_dq_detailed_stats_status is True
+                and _source_dq_enabled
+            ):
+                _context.set_source_query_dq_detailed_stats(_agg_query_dq_results)
+
+                _context.set_source_query_dq_output(_querydq_output_list)
+
+            elif (
+                rule_type == _context.get_query_dq_rule_type_name
+                and _context.get_query_dq_detailed_stats_status is True
+                and _target_dq_enabled
+            ):
+                _context.set_target_query_dq_detailed_stats(_agg_query_dq_results)
+
+                _context.set_target_query_dq_output(_querydq_output_list)
+
+            if len(condition_expressions) > 0:
+                if rule_type in [
+                    _context.get_query_dq_rule_type_name,
+                    _context.get_agg_dq_rule_type_name,
+                ]:
+                    df = (
+                        df
+                        if rule_type == _context.get_agg_dq_rule_type_name
+                        else _context.get_supported_df_query_dq
+                    )
+
+                    df = df.select(*condition_expressions)
+
+                    df = df.withColumn(
+                        f"meta_{rule_type}_results", array(*list(df.columns))
+                    )
+
+                    df = df.withColumn(
+                        f"meta_{rule_type}_results",
+                        remove_empty_maps(df[f"meta_{rule_type}_results"]),
+                    ).drop(
+                        *[
+                            _col
+                            for _col in df.columns
+                            if _col != f"meta_{rule_type}_results"
+                        ]
+                    )
+
+                    _context.print_dataframe_with_debugger(df)
+
+                elif rule_type == _context.get_row_dq_rule_type_name:
+                    df = df.select(col("*"), *condition_expressions)
+
+            else:
+                raise SparkExpectationsMiscException(
+                    f"zero active expectations to process for {rule_type}_rules from the `dq_rules` table, "
+                    f"at {f'final_{rule_type}' if _source_dq_enabled else f'final_{rule_type}' }"
+                    f", please configure rules or avoid this error by setting final_{rule_type} to False"
+                )
+
+            return df
 
         except Exception as e:
             raise SparkExpectationsMiscException(
-                f"error occurred created summarized row dq statistics {e}"
+                f"error occurred while running expectations {e}"
             )
 
-    def generate_rules_exceeds_threshold(self, rules: dict) -> None:
+    @staticmethod
+    def action_on_rules(
+        _context: SparkExpectationsContext,
+        _df_dq: DataFrame,
+        _input_count: int,
+        _error_count: int = 0,
+        _output_count: int = 0,
+        _rule_type: Optional[str] = None,
+        _row_dq_flag: bool = False,
+        _source_agg_dq_flag: bool = False,
+        _final_agg_dq_flag: bool = False,
+        _source_query_dq_flag: bool = False,
+        _final_query_dq_flag: bool = False,
+    ) -> DataFrame:
         """
-        This function implements/supports summarizing row dq error threshold
+        This function takes necessary action set by the user on the rules and returns the dataframe with results
         Args:
-            rules: accepts rule metadata within dict
+            _context: Provide SparkExpectationsContext
+            _df_dq: Input dataframe on which data quality rules need to be applied
+            _input_count: input dataset count
+            _error_count: error count in the dataset
+            _output_count: output count in the dataset
+            _rule_type: type of rule expectations
+            _row_dq_flag: Mark it as True when dq running for row level expectations
+            _source_agg_dq_flag: Mark it as True when dq running for agg level expectations on source dataframe
+            _final_agg_dq_flag: Mark it as True when dq running for agg level expectations on final dataframe
+            _source_query_dq_flag: Mark it as True when dq running for query level expectations on source dataframe
+            _final_query_dq_flag: Mark it as True when dq running for query level expectations on final dataframe
         Returns:
-            None
+                DataFrame: Returns a dataframe after dropping the error from the dataset
+
         """
         try:
-            error_threshold_list = []
-            rules_failed_row_count: Dict[str, int] = {}
-            if self._context.get_summarized_row_dq_res is None:
-                return None
-
-            rules_failed_row_count = {
-                itr["rule"]: int(itr["failed_row_count"])
-                for itr in self._context.get_summarized_row_dq_res
-            }
-
-            for rule in rules[f"{self._context.get_row_dq_rule_type_name}_rules"]:
-                # if (
-                #         not rule["enable_error_drop_alert"]
-                #         or rule["rule"] not in rules_failed_row_count.keys()
-                # ):
-                #     continue  # pragma: no cover
-
-                rule_name = rule["rule"]
-                rule_action = rule["action_if_failed"]
-                if rule_name in rules_failed_row_count.keys():
-                    failed_row_count = int(rules_failed_row_count[rule_name])
-                else:
-                    failed_row_count = 0
-
-                if failed_row_count is not None and failed_row_count > 0:
-                    error_drop_percentage = round(
-                        (failed_row_count / self._context.get_input_count) * 100, 2
-                    )
-                    error_threshold_list.append(
-                        {
-                            "rule_name": rule_name,
-                            "action_if_failed": rule_action,
-                            "description": rule["description"],
-                            "rule_type": rule["rule_type"],
-                            "error_drop_threshold": str(rule["error_drop_threshold"]),
-                            "error_drop_percentage": str(error_drop_percentage),
-                        }
-                    )
+            _df_dq = _df_dq.withColumn(
+                "action_if_failed", get_actions_list(col(f"meta_{_rule_type}_results"))
+            ).drop(f"meta_{_rule_type}_results")
+
+            if (
+                not _df_dq.filter(
+                    array_contains(_df_dq.action_if_failed, "fail")
+                ).count()
+                > 0
+            ):
+                _df_dq = _df_dq.filter(~array_contains(_df_dq.action_if_failed, "drop"))
+            else:
+                if _row_dq_flag:
+                    _context.set_row_dq_status("Failed")
+                elif _source_agg_dq_flag:
+                    _context.set_source_agg_dq_status("Failed")
+                elif _final_agg_dq_flag:
+                    _context.set_final_agg_dq_status("Failed")
+                elif _source_query_dq_flag:
+                    _context.set_source_query_dq_status("Failed")
+                elif _final_query_dq_flag:
+                    _context.set_final_query_dq_status("Failed")
+
+                raise SparkExpectOrFailException(
+                    f"Job failed, as there is a data quality issue at {_rule_type} "
+                    f"expectations and the action_if_failed "
+                    "suggested to fail"
+                )
 
-            if len(error_threshold_list) > 0:
-                self._context.set_rules_exceeds_threshold(error_threshold_list)
+            return _df_dq.drop(_df_dq.action_if_failed)
 
         except Exception as e:
             raise SparkExpectationsMiscException(
-                f"An error occurred while creating error threshold list : {e}"
+                f"error occurred while taking action on given rules {e}"
             )
```

### Comparing `spark_expectations-1.1.1/spark_expectations/utils/regulate_flow.py` & `spark_expectations-2.0.0/spark_expectations/utils/regulate_flow.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/spark_expectations/utils/udf.py` & `spark_expectations-2.0.0/spark_expectations/utils/udf.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-1.1.1/PKG-INFO` & `spark_expectations-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-expectations
-Version: 1.1.1
+Version: 2.0.0
 Summary: This project helps us to run Data Quality Rules in flight while spark job is being run
 Author: Ashok Singamaneni
 Author-email: ashok.singamaneni@nike.com
 Requires-Python: >=3.8.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -82,30 +82,35 @@
 ### Configurations
 
 In order to establish the global configuration parameter for DQ Spark Expectations, you must define and complete the 
 required fields within a variable. This involves creating a variable and ensuring that all the necessary information 
 is provided in the appropriate fields.
 
 ```python
-from spark_expectations.config.user_config import *
+from spark_expectations.config.user_config import Constants as user_config
 
 se_user_conf = {
-    se_notifications_enable_email: False,
-    se_notifications_email_smtp_host: "mailhost.nike.com",
-    se_notifications_email_smtp_port: 25,
-    se_notifications_email_from: "<sender_email_id>",
-    se_notifications_email_to_other_nike_mail_id: "<receiver_email_id's>",
-    se_notifications_email_subject: "spark expectations - data quality - notifications", 
-    se_notifications_enable_slack: True,
-    se_notifications_slack_webhook_url: "<slack-webhook-url>", 
-    se_notifications_on_start: True, 
-    se_notifications_on_completion: True,
-    se_notifications_on_fail: True,
-    se_notifications_on_error_drop_exceeds_threshold_breach: True, 
-    se_notifications_on_error_drop_threshold: 15,
+    user_config.se_notifications_enable_email: False,
+    user_config.se_notifications_email_smtp_host: "mailhost.nike.com",
+    user_config.se_notifications_email_smtp_port: 25,
+    user_config.se_notifications_email_from: "<sender_email_id>",
+    user_config.se_notifications_email_to_other_nike_mail_id: "<receiver_email_id's>",
+    user_config.se_notifications_email_subject: "spark expectations - data quality - notifications", 
+    user_config.se_notifications_enable_slack: True,
+    user_config.se_notifications_slack_webhook_url: "<slack-webhook-url>", 
+    user_config.se_notifications_on_start: True, 
+    user_config.se_notifications_on_completion: True,
+    user_config.se_notifications_on_fail: True,
+    user_config.se_notifications_on_error_drop_exceeds_threshold_breach: True, 
+    user_config.se_notifications_on_error_drop_threshold: 15,
+    #Optional
+    #Below two params are optional and need to be enabled to capture the detailed stats in the <stats_table_name>_detailed.
+    #user_config.enable_query_dq_detailed_result: True,
+    #user_config.enable_agg_dq_detailed_result: True,
+    
 }
 ```
 
 ### Spark Expectations Initialization 
 
 For all the below examples the below import and SparkExpectations class instantiation is mandatory
```

