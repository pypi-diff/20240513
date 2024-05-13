# Comparing `tmp/deling-0.2.0.tar.gz` & `tmp/deling-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deling-0.2.0.tar", last modified: Fri Feb  2 20:53:39 2024, max compression
+gzip compressed data, was "deling-0.2.2.tar", last modified: Fri Feb 23 09:57:03 2024, max compression
```

## Comparing `deling-0.2.0.tar` & `deling-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 20:53:39.742301 deling-0.2.0/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2484 2024-02-02 20:53:39.742301 deling-0.2.0/PKG-INFO
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1383 2024-02-01 15:24:47.000000 deling-0.2.0/README.rst
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 20:53:39.738301 deling-0.2.0/deling/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-17 15:51:20.000000 deling-0.2.0/deling/__init__.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 20:53:39.738301 deling-0.2.0/deling/authenticators/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-18 18:35:25.000000 deling-0.2.0/deling/authenticators/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    16635 2024-02-02 17:54:06.000000 deling-0.2.0/deling/authenticators/ssh.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 20:53:39.738301 deling-0.2.0/deling/clients/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 17:54:06.000000 deling-0.2.0/deling/clients/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4390 2024-02-02 18:43:49.000000 deling-0.2.0/deling/clients/ssh.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 20:53:39.738301 deling-0.2.0/deling/io/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-17 15:51:20.000000 deling-0.2.0/deling/io/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1591 2024-01-17 15:51:20.000000 deling-0.2.0/deling/io/async.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 20:53:39.738301 deling-0.2.0/deling/io/datastores/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-17 15:51:20.000000 deling-0.2.0/deling/io/datastores/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    16484 2024-02-02 17:54:06.000000 deling-0.2.0/deling/io/datastores/core.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1420 2024-02-01 15:24:47.000000 deling-0.2.0/deling/io/datastores/erda.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     3323 2024-01-17 15:51:20.000000 deling-0.2.0/deling/io/datastores/file.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 20:53:39.738301 deling-0.2.0/deling/utils/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-18 18:36:35.000000 deling-0.2.0/deling/utils/__init__.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4524 2024-01-30 09:08:04.000000 deling-0.2.0/deling/utils/io.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1623 2024-01-30 09:08:04.000000 deling-0.2.0/deling/utils/run.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 20:53:39.742301 deling-0.2.0/deling.egg-info/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2484 2024-02-02 20:53:39.000000 deling-0.2.0/deling.egg-info/PKG-INFO
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      616 2024-02-02 20:53:39.000000 deling-0.2.0/deling.egg-info/SOURCES.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2024-02-02 20:53:39.000000 deling-0.2.0/deling.egg-info/dependency_links.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      151 2024-02-02 20:53:39.000000 deling-0.2.0/deling.egg-info/requires.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        7 2024-02-02 20:53:39.000000 deling-0.2.0/deling.egg-info/top_level.txt
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       63 2024-02-02 20:53:39.742301 deling-0.2.0/setup.cfg
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1492 2024-02-02 20:53:18.000000 deling-0.2.0/setup.py
-drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 20:53:39.742301 deling-0.2.0/tests/
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-15 07:33:13.000000 deling-0.2.0/tests/test_async.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4668 2024-02-01 15:24:47.000000 deling-0.2.0/tests/test_auth.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4683 2024-02-02 18:00:20.000000 deling-0.2.0/tests/test_client.py
--rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    25420 2024-02-01 15:24:47.000000 deling-0.2.0/tests/test_core_io.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-23 09:57:03.963829 deling-0.2.2/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2584 2024-02-23 09:57:03.963829 deling-0.2.2/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1383 2024-02-01 15:24:47.000000 deling-0.2.2/README.rst
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-23 09:57:03.959829 deling-0.2.2/deling/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-17 15:51:20.000000 deling-0.2.2/deling/__init__.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-23 09:57:03.959829 deling-0.2.2/deling/authenticators/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-18 18:35:25.000000 deling-0.2.2/deling/authenticators/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    16635 2024-02-02 17:54:06.000000 deling-0.2.2/deling/authenticators/ssh.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-23 09:57:03.963829 deling-0.2.2/deling/clients/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-02 17:54:06.000000 deling-0.2.2/deling/clients/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4433 2024-02-23 09:28:39.000000 deling-0.2.2/deling/clients/ssh.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-23 09:57:03.963829 deling-0.2.2/deling/io/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-17 15:51:20.000000 deling-0.2.2/deling/io/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1591 2024-01-17 15:51:20.000000 deling-0.2.2/deling/io/async.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-23 09:57:03.963829 deling-0.2.2/deling/io/datastores/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-17 15:51:20.000000 deling-0.2.2/deling/io/datastores/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    16484 2024-02-02 17:54:06.000000 deling-0.2.2/deling/io/datastores/core.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1420 2024-02-01 15:24:47.000000 deling-0.2.2/deling/io/datastores/erda.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     3323 2024-01-17 15:51:20.000000 deling-0.2.2/deling/io/datastores/file.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-23 09:57:03.963829 deling-0.2.2/deling/utils/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-18 18:36:35.000000 deling-0.2.2/deling/utils/__init__.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4524 2024-01-30 09:08:04.000000 deling-0.2.2/deling/utils/io.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1623 2024-01-30 09:08:04.000000 deling-0.2.2/deling/utils/run.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-23 09:57:03.963829 deling-0.2.2/deling.egg-info/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     2584 2024-02-23 09:57:03.000000 deling-0.2.2/deling.egg-info/PKG-INFO
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      616 2024-02-23 09:57:03.000000 deling-0.2.2/deling.egg-info/SOURCES.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        1 2024-02-23 09:57:03.000000 deling-0.2.2/deling.egg-info/dependency_links.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)      151 2024-02-23 09:57:03.000000 deling-0.2.2/deling.egg-info/requires.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        7 2024-02-23 09:57:03.000000 deling-0.2.2/deling.egg-info/top_level.txt
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)       63 2024-02-23 09:57:03.963829 deling-0.2.2/setup.cfg
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     1590 2024-02-23 09:46:59.000000 deling-0.2.2/setup.py
+drwxr-xr-x   0 rasmunk   (1000) rasmunk   (1000)        0 2024-02-23 09:57:03.963829 deling-0.2.2/tests/
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)        0 2024-01-15 07:33:13.000000 deling-0.2.2/tests/test_async.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     4668 2024-02-01 15:24:47.000000 deling-0.2.2/tests/test_auth.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)     3758 2024-02-23 09:28:39.000000 deling-0.2.2/tests/test_client.py
+-rw-r--r--   0 rasmunk   (1000) rasmunk   (1000)    25420 2024-02-01 15:24:47.000000 deling-0.2.2/tests/test_core_io.py
```

### Comparing `deling-0.2.0/PKG-INFO` & `deling-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: deling
-Version: 0.2.0
+Version: 0.2.2
 Summary: A library for accessing and storing data in remote storage systems
 Home-page: https://github.com/rasmunk/deling
 Author: Rasmus Munk
 Author-email: munk1@live.dk
 License: MIT
 Project-URL: Source Code, https://github.com/rasmunk/deling
 Keywords: Data IO,Staging data,Data transfer,Data storage,Data management
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fs.sshfs>=1.0.2
 Requires-Dist: fs>=2.4.16
 Requires-Dist: ssh2-python>=1.0.0
 Requires-Dist: PyYAML>=6.0.1
```

### Comparing `deling-0.2.0/README.rst` & `deling-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `deling-0.2.0/deling/authenticators/ssh.py` & `deling-0.2.2/deling/authenticators/ssh.py`

 * *Files identical despite different names*

### Comparing `deling-0.2.0/deling/clients/ssh.py` & `deling-0.2.2/deling/clients/ssh.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,21 +9,23 @@
 
 class SSHClient(object):
     def __init__(self, host, authenticator, port=22, proxy=None):
         self.host = host
         self.authenticator = authenticator
         if isinstance(port, str):
             self.port = int(port)
+        else:
+            self.port = port
         self.proxy = proxy
+
         self.socket = None
         self.session = None
         self.channel = None
         self.sftp_channel = None
 
-
     def __del__(self):
         self.disconnect()
 
     def is_socket_connected(self):
         if not self.socket:
             return False
         error_code = self.socket.getsockopt(socket.SOL_SOCKET, socket.SO_ERROR)
```

### Comparing `deling-0.2.0/deling/io/async.py` & `deling-0.2.2/deling/io/async.py`

 * *Files identical despite different names*

### Comparing `deling-0.2.0/deling/io/datastores/core.py` & `deling-0.2.2/deling/io/datastores/core.py`

 * *Files identical despite different names*

### Comparing `deling-0.2.0/deling/io/datastores/erda.py` & `deling-0.2.2/deling/io/datastores/erda.py`

 * *Files identical despite different names*

### Comparing `deling-0.2.0/deling/io/datastores/file.py` & `deling-0.2.2/deling/io/datastores/file.py`

 * *Files identical despite different names*

### Comparing `deling-0.2.0/deling/utils/io.py` & `deling-0.2.2/deling/utils/io.py`

 * *Files identical despite different names*

### Comparing `deling-0.2.0/deling/utils/run.py` & `deling-0.2.2/deling/utils/run.py`

 * *Files identical despite different names*

### Comparing `deling-0.2.0/deling.egg-info/PKG-INFO` & `deling-0.2.2/deling.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: deling
-Version: 0.2.0
+Version: 0.2.2
 Summary: A library for accessing and storing data in remote storage systems
 Home-page: https://github.com/rasmunk/deling
 Author: Rasmus Munk
 Author-email: munk1@live.dk
 License: MIT
 Project-URL: Source Code, https://github.com/rasmunk/deling
 Keywords: Data IO,Staging data,Data transfer,Data storage,Data management
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fs.sshfs>=1.0.2
 Requires-Dist: fs>=2.4.16
 Requires-Dist: ssh2-python>=1.0.0
 Requires-Dist: PyYAML>=6.0.1
```

### Comparing `deling-0.2.0/deling.egg-info/SOURCES.txt` & `deling-0.2.2/deling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deling-0.2.0/setup.py` & `deling-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,12 +38,14 @@
     },
     project_urls={"Source Code": "https://github.com/rasmunk/deling"},
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `deling-0.2.0/tests/test_auth.py` & `deling-0.2.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `deling-0.2.0/tests/test_client.py` & `deling-0.2.2/tests/test_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -87,31 +87,7 @@
         self.assertTrue(self.client.open_channel(channel_type=CHANNEL_TYPE_SFTP))
         sftp_channel = self.client.get_channel(channel_type=CHANNEL_TYPE_SFTP)
         self.assertIsInstance(sftp_channel, SFTP)
         self.assertEqual(sftp_channel, self.client.sftp_channel)
         self.client.close_channel(channel_type=CHANNEL_TYPE_SFTP)
         self.assertIsNone(self.client.sftp_channel)
         self.client.disconnect()
-
-
-class SSHClientProxyTest(CommonClientTestCases, unittest.TestCase):
-    def setUp(self):
-        self.seed = str(random())[2:10]
-        tmp_test_dir = os.path.join(os.getcwd(), "tests", "tmp")
-        self.test_ssh_dir = os.path.join(tmp_test_dir, "ssh-{}".format(self.seed))
-        if not exists(self.test_ssh_dir):
-            self.assertTrue(makedirs(self.test_ssh_dir))
-
-        host = "127.0.0.1"
-        port = "2222"
-        username = "mountuser"
-        password = "Passw0rd!"
-
-        authenticator = SSHAuthenticator(username=username, password=password)
-        self.proxy = SSHClient(host, authenticator, port=port)
-        self.client = SSHClient(host, authenticator, port=port, proxy=self.proxy)
-
-    def tearDown(self):
-        # Remove every file from test_ssh_dir
-        if exists(self.test_ssh_dir):
-            self.assertTrue(removedirs(self.test_ssh_dir, recursive=True))
-        self.share = None
```

### Comparing `deling-0.2.0/tests/test_core_io.py` & `deling-0.2.2/tests/test_core_io.py`

 * *Files identical despite different names*

