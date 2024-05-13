# Comparing `tmp/shared_helpers-0.0.7.tar.gz` & `tmp/shared_helpers-0.0.9.tar.gz`

## Comparing `shared_helpers-0.0.7.tar` & `shared_helpers-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/requirements.txt
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/setup.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/__init__.py
--rw-r--r--   0        0        0     3314 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/functions.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/main.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/lm/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/lm/sbbid/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/lm/sbbid/sbbid_helper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/iam/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/organization/__init__.py
--rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/organization/organization_helper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/tracker/__init__.py
--rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/src/shared_helpers/yandex/tracker/tracker_helper.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/README.md
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 shared_helpers-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/__init__.py
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/functions.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/shared_helpers.py
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/lm/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/lm/sbbid/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/lm/sbbid/sbbid_helper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/yandex/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/yandex/iam/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/yandex/organization/__init__.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/yandex/organization/organization_helper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/yandex/tracker/__init__.py
+-rw-r--r--   0        0        0     9294 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/src/yandex/tracker/tracker_helper.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/README.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 shared_helpers-0.0.9/PKG-INFO
```

### Comparing `shared_helpers-0.0.7/src/shared_helpers/functions.py` & `shared_helpers-0.0.9/src/functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import calendar
 import requests
+from datetime import date
+from datetime import datetime
 import json
 import time
 import jwt
 import os
-from datetime import date
-from datetime import datetime
+
 from urllib3.util import Retry
 from requests.adapters import HTTPAdapter
-
-import shared_helpers.variables as variables
+#import shared_helpers.variables as variables
 
 req = requests.Session()
 retries = Retry(total=5,
                 backoff_factor=2,
                 status_forcelist=[429, 500, 502, 503, 504])
 
 req.mount('http://', HTTPAdapter(max_retries=retries))
@@ -23,17 +23,24 @@
         self.json_file_path = json_file_path
         self.api_key = api_key
         self.endpoint_url = endpoint_url
         
 
     def get_iam_token_from_endpoint(self, api_key=None, endpoint_url=None):
         """Fetch IAM token from the endpoint using the API key."""
-        headers = {'Authorization': f'Api-Key {api_key}'}
-        response = req.get(endpoint_url, headers=headers)
-        return response.json().get('token').get('access_token')
+        if not self.api_key or not self.endpoint_url:
+            return None
+        headers = {'Authorization': f'Api-Key {self.api_key}'}
+        response = req.get(self.endpoint_url, headers=headers)
+        try:
+            #token = response.json().get('token').get('access_token')
+            token = response.json()
+        except (AttributeError, ValueError):
+            token = None
+        return token
     def file_exists(self,json_file_path=None):
         if json_file_path:
             return os.path.isfile(json_file_path)
     def get_iam_token_from_file(self,json_file_path=None):
         """Fetch IAM token from a JSON file."""
         if not os.path.isfile(json_file_path):
             return None
```

### Comparing `shared_helpers-0.0.7/src/shared_helpers/lm/sbbid/sbbid_helper.py` & `shared_helpers-0.0.9/src/lm/sbbid/sbbid_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __init__(self, x_api_key=None, environment=None):
         self.x_api_key = x_api_key
         self.environment = environment
         self.headers_dict = {'x-api-key': x_api_key}
         if environment == 'external':
             self.BASE_URL = 'https://api.leroymerlin.ru:443/technologies/sbbid/catalogue/v1'
         else:
-            self.BASE_URL = 'https://api.internal.leroymerlin.ru/technologies/sbbid/infoproduct/v2'
+            self.BASE_URL = 'https://api.internal.leroymerlin.ru/technolosies/sbbid/infoproduct/v2'
 
     def get_domains(self):
         url = f'{self.BASE_URL}/domains'
         response = req.get(url, headers=self.headers_dict)
         return response.json()
     
     def get_domain_by_id(self, domainId):
```

### Comparing `shared_helpers-0.0.7/src/shared_helpers/yandex/organization/organization_helper.py` & `shared_helpers-0.0.9/src/yandex/organization/organization_helper.py`

 * *Files identical despite different names*

### Comparing `shared_helpers-0.0.7/src/shared_helpers/yandex/tracker/tracker_helper.py` & `shared_helpers-0.0.9/src/yandex/tracker/tracker_helper.py`

 * *Files identical despite different names*

### Comparing `shared_helpers-0.0.7/.gitignore` & `shared_helpers-0.0.9/.gitignore`

 * *Files identical despite different names*

