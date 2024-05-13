# Comparing `tmp/qiskit_scaleway-0.1.8.tar.gz` & `tmp/qiskit_scaleway-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_scaleway-0.1.8.tar", last modified: Mon May  6 11:54:01 2024, max compression
+gzip compressed data, was "qiskit_scaleway-0.1.9.tar", last modified: Tue May  7 14:49:38 2024, max compression
```

## Comparing `qiskit_scaleway-0.1.8.tar` & `qiskit_scaleway-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    11357 2024-02-29 13:51:39.000000 qiskit_scaleway-0.1.8/LICENSE
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3000 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/PKG-INFO
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2805 2024-05-03 08:18:12.000000 qiskit_scaleway-0.1.8/README.md
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/qiskit_scaleway/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       39 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      178 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5150 2024-05-06 11:30:47.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/aer_backend.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3504 2024-04-10 09:37:46.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/aer_job.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3077 2024-05-06 11:30:33.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/qsim_backend.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9781 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/qsim_job.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2038 2024-05-06 11:32:05.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/scaleway_backend.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2041 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/backends/scaleway_job.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     5244 2024-05-06 11:30:00.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/provider.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/qiskit_scaleway/utils/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       31 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/utils/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4019 2024-05-06 11:30:00.000000 qiskit_scaleway-0.1.8/qiskit_scaleway/utils/client.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3000 2024-05-06 11:54:01.000000 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/PKG-INFO
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      619 2024-05-06 11:54:01.000000 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/SOURCES.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)        1 2024-05-06 11:54:01.000000 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/dependency_links.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      148 2024-05-06 11:54:01.000000 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/requires.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       16 2024-05-06 11:54:01.000000 qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/top_level.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       38 2024-05-06 11:54:01.664412 qiskit_scaleway-0.1.8/setup.cfg
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      546 2024-05-06 11:53:18.000000 qiskit_scaleway-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:38.699156 qiskit_scaleway-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-07 14:49:38.699156 qiskit_scaleway-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:38.695156 qiskit_scaleway-0.1.9/qiskit_scaleway/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:38.695156 qiskit_scaleway-0.1.9/qiskit_scaleway/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/backends/aer_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/backends/aer_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/backends/qsim_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/backends/qsim_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/backends/scaleway_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/backends/scaleway_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:38.695156 qiskit_scaleway-0.1.9/qiskit_scaleway/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/qiskit_scaleway/utils/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 14:49:38.695156 qiskit_scaleway-0.1.9/qiskit_scaleway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-07 14:49:38.000000 qiskit_scaleway-0.1.9/qiskit_scaleway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-07 14:49:38.000000 qiskit_scaleway-0.1.9/qiskit_scaleway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 14:49:38.000000 qiskit_scaleway-0.1.9/qiskit_scaleway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-07 14:49:38.000000 qiskit_scaleway-0.1.9/qiskit_scaleway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-07 14:49:38.000000 qiskit_scaleway-0.1.9/qiskit_scaleway.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 14:49:38.699156 qiskit_scaleway-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-07 14:49:30.000000 qiskit_scaleway-0.1.9/setup.py
```

### Comparing `qiskit_scaleway-0.1.8/LICENSE` & `qiskit_scaleway-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.8/PKG-INFO` & `qiskit_scaleway-0.1.9/qiskit_scaleway.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Metadata-Version: 2.1
-Name: qiskit_scaleway
-Version: 0.1.8
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Name: qiskit-scaleway
+Version: 0.1.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Scaleway provider for Qiskit
 
 **Qiskit Scaleway** is a Python package to run quantum circuits on [Scaleway](https://www.scaleway.com/en/) infrastructure, providing access to [Aer](https://github.com/Qiskit/qiskit-aer) and [Qsim](https://github.com/quantumlib/qsim) simulators on powerful hardware (CPU and GPU).
 
@@ -95,9 +91,7 @@
 This repository is at its early stage and is still in active development. If you are looking for a way to contribute please read [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Reach us
 We love feedback. Feel free to reach us on [Scaleway Slack community](https://slack.scaleway.com/), we are waiting for you on [#opensource](https://scaleway-community.slack.com/app_redirect?channel=opensource)..
 
 ## Licence
 [License Apache 2.0](LICENCE)
-
-
```

### Comparing `qiskit_scaleway-0.1.8/README.md` & `qiskit_scaleway-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/aer_backend.py` & `qiskit_scaleway-0.1.9/qiskit_scaleway/backends/aer_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,30 +64,30 @@
         return self._target.num_qubits
 
     @property
     def max_circuits(self):
         return 1024
 
     def run(
-        self, circuits: Union[QuantumCircuit, List[QuantumCircuit]], **kwargs
+        self, circuits: Union[QuantumCircuit, List[QuantumCircuit]], **run_options
     ) -> AerJob:
         if not isinstance(circuits, list):
             circuits = [circuits]
 
         job_config = {key: value for key, value in self._options.items()}
 
-        for kwarg in kwargs:
+        for kwarg in run_options:
             if not hasattr(self.options, kwarg):
                 warnings.warn(
                     f"Option {kwarg} is not used by this backend",
                     UserWarning,
                     stacklevel=2,
                 )
             else:
-                job_config[kwarg] = kwargs[kwarg]
+                job_config[kwarg] = run_options[kwarg]
 
         job_name = f"qj-aer-{randomname.get_name()}"
 
         session_id = job_config.get("session_id", None)
 
         job_config.pop("session_id")
         job_config.pop("session_name")
```

### Comparing `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/aer_job.py` & `qiskit_scaleway-0.1.9/qiskit_scaleway/backends/aer_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/qsim_backend.py` & `qiskit_scaleway-0.1.9/qiskit_scaleway/backends/qsim_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/qsim_job.py` & `qiskit_scaleway-0.1.9/qiskit_scaleway/backends/qsim_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/scaleway_backend.py` & `qiskit_scaleway-0.1.9/qiskit_scaleway/backends/scaleway_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.8/qiskit_scaleway/backends/scaleway_job.py` & `qiskit_scaleway-0.1.9/qiskit_scaleway/backends/scaleway_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.8/qiskit_scaleway/provider.py` & `qiskit_scaleway-0.1.9/qiskit_scaleway/provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.8/qiskit_scaleway/utils/client.py` & `qiskit_scaleway-0.1.9/qiskit_scaleway/utils/client.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/PKG-INFO` & `qiskit_scaleway-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 Metadata-Version: 2.1
-Name: qiskit-scaleway
-Version: 0.1.8
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+Name: qiskit_scaleway
+Version: 0.1.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Scaleway provider for Qiskit
 
 **Qiskit Scaleway** is a Python package to run quantum circuits on [Scaleway](https://www.scaleway.com/en/) infrastructure, providing access to [Aer](https://github.com/Qiskit/qiskit-aer) and [Qsim](https://github.com/quantumlib/qsim) simulators on powerful hardware (CPU and GPU).
 
@@ -95,9 +91,7 @@
 This repository is at its early stage and is still in active development. If you are looking for a way to contribute please read [CONTRIBUTING.md](CONTRIBUTING.md).
 
 ## Reach us
 We love feedback. Feel free to reach us on [Scaleway Slack community](https://slack.scaleway.com/), we are waiting for you on [#opensource](https://scaleway-community.slack.com/app_redirect?channel=opensource)..
 
 ## Licence
 [License Apache 2.0](LICENCE)
-
-
```

### Comparing `qiskit_scaleway-0.1.8/qiskit_scaleway.egg-info/SOURCES.txt` & `qiskit_scaleway-0.1.9/qiskit_scaleway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.8/setup.py` & `qiskit_scaleway-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="qiskit_scaleway",
-    version="0.1.8",
+    version="0.1.9",
     packages=find_packages(),
     install_requires=[
         "qiskit==1.0.2",
         "qiskit-aer==0.14.0.1",
         "randomname==0.2.1",
         "httpx==0.27.0",
         "dataclasses-json==0.6.4",
```

