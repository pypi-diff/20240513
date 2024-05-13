# Comparing `tmp/dane-0.4.1.tar.gz` & `tmp/dane-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dane-0.4.1.tar", max compression
+gzip compressed data, was "dane-0.4.2.tar", max compression
```

## Comparing `dane-0.4.1.tar` & `dane-0.4.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2022-12-20 11:50:37.871142 dane-0.4.1/LICENSE
--rw-r--r--   0        0        0     2362 2022-12-20 11:50:37.871142 dane-0.4.1/README.md
--rw-r--r--   0        0        0      245 2023-06-19 12:18:27.536564 dane-0.4.1/dane/__init__.py
--rw-r--r--   0        0        0    14589 2023-06-23 07:10:50.684841 dane-0.4.1/dane/base_classes.py
--rw-r--r--   0        0        0     4478 2023-06-19 14:20:12.773557 dane-0.4.1/dane/config.py
--rw-r--r--   0        0        0     5679 2022-12-20 11:50:37.871142 dane-0.4.1/dane/document.py
--rw-r--r--   0        0        0     2187 2022-12-20 11:50:37.871142 dane-0.4.1/dane/errors.py
--rw-r--r--   0        0        0     4858 2023-06-19 12:18:27.536564 dane-0.4.1/dane/es_queries.py
--rw-r--r--   0        0        0    39686 2023-06-19 12:18:27.536564 dane-0.4.1/dane/handlers/ESHandler.py
--rw-r--r--   0        0        0     4335 2023-06-19 12:18:27.536564 dane-0.4.1/dane/handlers/RabbitMQHandler.py
--rw-r--r--   0        0        0      213 2022-12-20 11:50:37.871142 dane-0.4.1/dane/handlers/__init__.py
--rw-r--r--   0        0        0     9821 2023-06-19 12:18:27.536564 dane-0.4.1/dane/handlers/base_handler.py
--rw-r--r--   0        0        0     4158 2023-11-08 14:35:58.733111 dane-0.4.1/dane/provenance.py
--rw-r--r--   0        0        0     3770 2022-12-20 11:50:37.871142 dane-0.4.1/dane/results.py
--rw-r--r--   0        0        0     5257 2023-10-30 14:03:56.448909 dane-0.4.1/dane/s3_util.py
--rw-r--r--   0        0        0     1384 2023-06-19 12:18:27.536564 dane-0.4.1/dane/state.py
--rw-r--r--   0        0        0     9860 2023-06-19 12:18:27.536564 dane-0.4.1/dane/tasks.py
--rw-r--r--   0        0        0     1357 2022-12-20 11:50:37.871142 dane-0.4.1/dane/utils.py
--rw-r--r--   0        0        0     1836 2023-11-08 14:36:41.895151 dane-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 dane-0.4.1/setup.py
--rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 dane-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-12-20 11:50:37.871142 dane-0.4.2/LICENSE
+-rw-r--r--   0        0        0     2362 2022-12-20 11:50:37.871142 dane-0.4.2/README.md
+-rw-r--r--   0        0        0      245 2023-06-19 12:18:27.536564 dane-0.4.2/dane/__init__.py
+-rw-r--r--   0        0        0    14589 2023-06-23 07:10:50.684841 dane-0.4.2/dane/base_classes.py
+-rw-r--r--   0        0        0     4478 2023-06-19 14:20:12.773557 dane-0.4.2/dane/config.py
+-rw-r--r--   0        0        0     5679 2022-12-20 11:50:37.871142 dane-0.4.2/dane/document.py
+-rw-r--r--   0        0        0     2187 2022-12-20 11:50:37.871142 dane-0.4.2/dane/errors.py
+-rw-r--r--   0        0        0     4858 2023-06-19 12:18:27.536564 dane-0.4.2/dane/es_queries.py
+-rw-r--r--   0        0        0    39686 2023-06-19 12:18:27.536564 dane-0.4.2/dane/handlers/ESHandler.py
+-rw-r--r--   0        0        0     4335 2023-06-19 12:18:27.536564 dane-0.4.2/dane/handlers/RabbitMQHandler.py
+-rw-r--r--   0        0        0      213 2022-12-20 11:50:37.871142 dane-0.4.2/dane/handlers/__init__.py
+-rw-r--r--   0        0        0     9821 2023-06-19 12:18:27.536564 dane-0.4.2/dane/handlers/base_handler.py
+-rw-r--r--   0        0        0     3927 2023-11-08 14:53:21.958899 dane-0.4.2/dane/provenance.py
+-rw-r--r--   0        0        0     3770 2022-12-20 11:50:37.871142 dane-0.4.2/dane/results.py
+-rw-r--r--   0        0        0     5257 2023-10-30 14:03:56.448909 dane-0.4.2/dane/s3_util.py
+-rw-r--r--   0        0        0     1384 2023-06-19 12:18:27.536564 dane-0.4.2/dane/state.py
+-rw-r--r--   0        0        0     9860 2023-06-19 12:18:27.536564 dane-0.4.2/dane/tasks.py
+-rw-r--r--   0        0        0     1357 2022-12-20 11:50:37.871142 dane-0.4.2/dane/utils.py
+-rw-r--r--   0        0        0     1836 2023-11-08 14:53:41.662001 dane-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     3292 1970-01-01 00:00:00.000000 dane-0.4.2/setup.py
+-rw-r--r--   0        0        0     3572 1970-01-01 00:00:00.000000 dane-0.4.2/PKG-INFO
```

### Comparing `dane-0.4.1/LICENSE` & `dane-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/README.md` & `dane-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/base_classes.py` & `dane-0.4.2/dane/base_classes.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/config.py` & `dane-0.4.2/dane/config.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/document.py` & `dane-0.4.2/dane/document.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/errors.py` & `dane-0.4.2/dane/errors.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/es_queries.py` & `dane-0.4.2/dane/es_queries.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/handlers/ESHandler.py` & `dane-0.4.2/dane/handlers/ESHandler.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/handlers/RabbitMQHandler.py` & `dane-0.4.2/dane/handlers/RabbitMQHandler.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/handlers/base_handler.py` & `dane-0.4.2/dane/handlers/base_handler.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/provenance.py` & `dane-0.4.2/dane/provenance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from dataclasses import dataclass, field
 import json
 import logging
 from time import time
 from typing import Any, Dict, List, Optional
-from dane.config import cfg
 
 
 logger = logging.getLogger("DANE")
 SOFTWARE_PROVENANCE_FILE = "/software_provenance.txt"
 PROVENANCE_FILE = "provenance.json"
 
 
@@ -46,21 +45,18 @@
     description: str,
     input_data: Dict[str, Any],
     parameters: Dict[str, Any] = {},
     software_version: Dict[str, Any] = {},
     start_time: float = time(),
 ):
     return Provenance(
-        activity_name="VisXP prep",
-        activity_description=(
-            "Detect shots and keyframes, "
-            "extract keyframes and corresponding audio spectograms"
-        ),
+        activity_name=name,
+        activity_description=description,
         input_data=input_data,
-        parameters=cfg.VISXP_PREP,
+        parameters=parameters,
         software_version=software_version,
         start_time_unix=start_time,
     )
 
 
 # Generates a the main Provenance object, which will embed/include the provided provenance_chain
 def stop_timer_and_persist_provenance_chain(
@@ -70,16 +66,14 @@
     provenance_file_path: str,  # where to write provenance.json
 ) -> Provenance:
     provenance.output_data = output_data
     provenance.processing_time_ms = time() - provenance.start_time_unix
     provenance.steps = provenance_chain
 
     fdata = provenance.to_json()
-    logger.info("Going to write the following to disk:")
-    logger.info(fdata)
     with open(provenance_file_path, "w", encoding="utf-8") as f:
         json.dump(fdata, f, ensure_ascii=False, indent=4)
         logger.info(f"Wrote provenance info to file: {provenance_file_path}")
     return provenance
 
 
 # NOTE: software_provenance.txt is created while building the container image (see Dockerfile)
```

### Comparing `dane-0.4.1/dane/results.py` & `dane-0.4.2/dane/results.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/s3_util.py` & `dane-0.4.2/dane/s3_util.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/state.py` & `dane-0.4.2/dane/state.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/tasks.py` & `dane-0.4.2/dane/tasks.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/dane/utils.py` & `dane-0.4.2/dane/utils.py`

 * *Files identical despite different names*

### Comparing `dane-0.4.1/pyproject.toml` & `dane-0.4.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "DANE"
-version = "0.4.1"
+version = "0.4.2"
 description = "Utils for working with the Distributed Annotation and Enrichment system"
 readme = "README.md"
 authors = [
     "Nanne van Noord <n.j.e.vannoord@uva.nl>",
     "jblom <jblom@beeldengeluid.nl>"
 ]
 license = "Apache License 2.0"
```

### Comparing `dane-0.4.1/setup.py` & `dane-0.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'pika>=1.3.1,<2.0.0',
  'requests>=2.28.1,<3.0.0',
  'urllib3>=1.26.12,<2.0.0',
  'yacs>=0.1.8,<0.2.0']
 
 setup_kwargs = {
     'name': 'dane',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': 'Utils for working with the Distributed Annotation and Enrichment system',
     'long_description': "# DANE\nThe Distributed Annotation 'n' Enrichment (DANE) system handles compute task assignment and file storage for the automatic annotation of content.\n\nThis repository contains contains the building blocks for with DANE, such as creating custom analysis workers or submitting new task.\n\n## Installation\n\nThis package can be installed through pip:\n\n    pip install dane\n\n### Configuration\n\nDANE components are configured through the dane.config module, which is described here: https://dane.readthedocs.io/en/latest/intro.html#configuration \nIt is however noteable that, because all DANE components are expected to rely on it, some of the DANE-server, ElasticSearch and RabbitMQ configuration \nare included in the default config. As such it is recommended that you create a `$HOME/.dane/config.yml` or `$DANE_HOME/config.yml` which contain machine-wide settings for how to connect to these services, which involves specifying the following settings:\n\n```\nDANE:\n    API_URL: 'http://localhost:5500/DANE/'\n    MANAGE_URL: 'http://localhost:5500/manage/'\nRABBITMQ:\n    HOST: 'localhost'\n    PORT: 5672\n    EXCHANGE: 'DANE-exchange'\n    RESPONSE_QUEUE: 'DANE-response-queue'\n    USER: 'guest'\n    PASSWORD: 'guest'\nELASTICSEARCH:\n    HOST: ['localhost']\n    PORT: 9200\n    USER: 'elastic'\n    PASSWORD: 'changeme'\n    SCHEME: 'http'\n    INDEX: 'your_dane_index'\n```\n\nThe values given here are the default values.\n\n### Usage\n\nExamples of how to use DANE can be found in the `examples/` directory.\n\n## Local Development\n\nWe moved from `setup.py` & `requirements.txt` to a single `pyproject.toml`. For local builds and publishing we use [poetry](https://python-poetry.org/).\n\nFor local installation:\n\n```bash\npoetry install\npoetry shell\n```\n\nAfter installation the following unit test should succeed:\n\n```bash\npython -m test.test_dane\n```\n\nTo build a wheel + source package (will end up in `dist` directory):\n\n```bash\npoetry build\n```\n\nThe wheel can be conveniently tested in e.g. your own DANE worker by installing it e.g. using `pip`:\n\n```bash\npip install path_to_dane_wheel_file\n```\n\nor with poetry\n\n```bash\npoetry add path_to_dane_wheel_file\n```\n\n### Breaking changes after 0.3.1 \n\nSince version 0.3.1 DANE must be imported in lowercase letters:\n\n```python\nimport dane\n```\n\nBefore version 0.3.1 you should import using uppercase letters:\n\n```python\nimport DANE\n```",
     'author': 'Nanne van Noord',
     'author_email': 'n.j.e.vannoord@uva.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/CLARIAH/DANE',
```

### Comparing `dane-0.4.1/PKG-INFO` & `dane-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dane
-Version: 0.4.1
+Version: 0.4.2
 Summary: Utils for working with the Distributed Annotation and Enrichment system
 Home-page: https://github.com/CLARIAH/DANE
 License: Apache-2.0
 Author: Nanne van Noord
 Author-email: n.j.e.vannoord@uva.nl
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

