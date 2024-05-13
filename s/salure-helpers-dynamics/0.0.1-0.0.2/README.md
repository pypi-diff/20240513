# Comparing `tmp/salure_helpers_dynamics-0.0.1.tar.gz` & `tmp/salure_helpers_dynamics-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_dynamics-0.0.1.tar", last modified: Wed Dec 20 14:46:35 2023, max compression
+gzip compressed data, was "dist/salure_helpers_dynamics-0.0.2.tar", last modified: Mon May 13 15:45:05 2024, max compression
```

## Comparing `salure_helpers_dynamics-0.0.1.tar` & `salure_helpers_dynamics-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/
--rw-r--r--   0 root         (0) root         (0)      273 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/salure_helpers/dynamics/
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-12-20 14:46:22.000000 salure_helpers_dynamics-0.0.1/salure_helpers/dynamics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1276 2023-12-20 14:46:22.000000 salure_helpers_dynamics-0.0.1/salure_helpers/dynamics/dynamics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/salure_helpers_dynamics.egg-info/
--rw-r--r--   0 root         (0) root         (0)      273 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/salure_helpers_dynamics.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      360 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/salure_helpers_dynamics.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/salure_helpers_dynamics.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/salure_helpers_dynamics.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       32 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/salure_helpers_dynamics.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/salure_helpers_dynamics.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-12-20 14:46:35.000000 salure_helpers_dynamics-0.0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      439 2023-12-20 14:46:22.000000 salure_helpers_dynamics-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/salure_helpers/dynamics/
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-05-13 15:44:44.000000 salure_helpers_dynamics-0.0.2/salure_helpers/dynamics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1550 2024-05-13 15:44:44.000000 salure_helpers_dynamics-0.0.2/salure_helpers/dynamics/dynamics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/salure_helpers_dynamics.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      273 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/salure_helpers_dynamics.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      360 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/salure_helpers_dynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/salure_helpers_dynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/salure_helpers_dynamics.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       32 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/salure_helpers_dynamics.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/salure_helpers_dynamics.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 15:45:05.000000 salure_helpers_dynamics-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      439 2024-05-13 15:44:44.000000 salure_helpers_dynamics-0.0.2/setup.py
```

### Comparing `salure_helpers_dynamics-0.0.1/salure_helpers/dynamics/dynamics.py` & `salure_helpers_dynamics-0.0.2/salure_helpers/dynamics/dynamics.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,12 +18,24 @@
         payload = {'grant_type': 'client_credentials',
                    'client_id': self.client_id,
                    'client_secret': self.client_secret,
                    'resource': self.resource}
         response = requests.request("POST", url, data=payload)
         return response.json()['access_token']
 
-    def get_data(self, endpoint: str, odata_filter: str = None) -> requests.Response:
+    def get_data(self, endpoint: str, params: dict = None) -> pd.DataFrame:
         url = f'{self.resource}/data/{endpoint}'
-        if odata_filter:
-            url += f'?$filter={odata_filter}'
-        return requests.request("GET", url, headers=self.headers)
+        df = pd.DataFrame()
+
+        while True:
+            response = requests.get(url, headers=self.headers, params=params)
+            df = pd.concat([df, pd.DataFrame(response.json()['value'])], ignore_index=True)
+
+            if '@odata.nextLink' in response.json():
+                url = response.json()['@odata.nextLink']
+                params = None
+            else:
+                break
+
+        return df
+
+
```

