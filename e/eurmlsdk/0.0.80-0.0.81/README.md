# Comparing `tmp/eurmlsdk-0.0.80.tar.gz` & `tmp/eurmlsdk-0.0.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eurmlsdk-0.0.80.tar", last modified: Mon May 13 10:13:36 2024, max compression
+gzip compressed data, was "dist/eurmlsdk-0.0.81.tar", last modified: Mon May 13 13:04:10 2024, max compression
```

## Comparing `eurmlsdk-0.0.80.tar` & `eurmlsdk-0.0.81.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.80/README.md
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.80/MANIFEST.in
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       79 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      790 2024-05-13 10:13:31.000000 eurmlsdk-0.0.80/setup.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.80/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/PKG-INFO
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3430 2024-05-13 10:08:36.000000 eurmlsdk-0.0.80/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6031 2024-05-13 10:08:24.000000 eurmlsdk-0.0.80/eurmlsdk/eur_sdk.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-09 09:42:44.000000 eurmlsdk-0.0.80/eurmlsdk/base_class.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-09 09:42:44.000000 eurmlsdk-0.0.80/eurmlsdk/__init__.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.81/README.md
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.81/MANIFEST.in
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       79 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      790 2024-05-13 13:03:59.000000 eurmlsdk-0.0.81/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.81/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 13:04:10.000000 eurmlsdk-0.0.81/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3430 2024-05-13 11:38:36.000000 eurmlsdk-0.0.81/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6614 2024-05-13 12:12:20.000000 eurmlsdk-0.0.81/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-09 09:42:44.000000 eurmlsdk-0.0.81/eurmlsdk/base_class.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-09 09:42:44.000000 eurmlsdk-0.0.81/eurmlsdk/__init__.py
```

### Comparing `eurmlsdk-0.0.80/setup.py` & `eurmlsdk-0.0.81/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.80',
+    version='0.0.81',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

### Comparing `eurmlsdk-0.0.80/eurmlsdk/__main__.py` & `eurmlsdk-0.0.81/eurmlsdk/__main__.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.80/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.81/eurmlsdk/eur_sdk.py`

 * *Files 10% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def uploadToRemote(self, ssh_client, local_path, remote_path):
         print("Uploading model {} to {}".format(local_path, remote_path))
         sftp_progress_bar = SFTPWithProgressBar.from_transport(ssh_client.get_transport())
         sftp_progress_bar.put(local_path, remote_path)
         print("Model upload successful")
 
-    def uploadModel(self, ssh_client, local_path, remote_path, home_path):
+    def uploadFile(self, ssh_client, local_path, remote_path, home_path):
         try:
             sftp = ssh_client.open_sftp()
             print("Checking for model file in {}".format(home_path))
             sftp.stat(remote_path)
             print('Model File already exists')
             upload = input('Do you want to upload it again (y/n)? ')
             while upload.lower() != 'y' and upload.lower() != 'n':
@@ -93,25 +93,38 @@
             print("Error Executing the script: ", err)
             exit(1)
               
     def deployModel(self, local_path, hostname, username, password, modelFile):
         # Establish SSH connection
         ssh_client = self.connect_ssh_client(hostname, username, password)
         home_path = self.execute_ssh_script(ssh_client, 'pwd')
-        if home_path != "":
-            remote_path = (f"{home_path}/{modelFile}").replace('\n', "").strip()
-            script_path = (f'{home_path}/hello.py').replace('\n', "").strip()
-            self.uploadModel(ssh_client, local_path, remote_path, home_path)
-            script_command = f'python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {script_path} {modelFile}'
-            # self.execute_script(ssh_client, script_path , modelFile)
-            execute_script = self.execute_ssh_script(ssh_client, script_command)
-            if execute_script != "":
-                print(execute_script)
-            # Close SSH connection
-            ssh_client.close()
+        if home_path == "":
+            exit(1)
+        remote_model_path = (f"{home_path}/{modelFile}").replace('\n', "").strip()
+        script_path = (f'{home_path}/hello.py').replace('\n', "").strip()
+        self.uploadFile(ssh_client, local_path, remote_model_path, home_path)
+        print("Choose between static dataset or live feed for prediction.")
+        static = input("Static dataset (y/n)? ")
+        static_path = ''
+        if static:
+            dataset_path = input("Enter img/video path: ")
+            remote_dataset_path = (f"{home_path}/{dataset_path.split("/")[-1]}").replace('\n', "").strip()
+            self.uploadFile(ssh_client, dataset_path, remote_dataset_path, home_path)
+            feedType = 'static'
+            static_path = remote_dataset_path
+        else:
+            feedType = 'live_feed'
+            exit(1)
+        script_command = f'python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {script_path} {modelFile} {feedType} {static_path}'
+        # self.execute_script(ssh_client, script_path , modelFile)
+        execute_script = self.execute_ssh_script(ssh_client, script_command)
+        if execute_script != "":
+            print(execute_script)
+        # Close SSH connection
+        ssh_client.close()
         exit(1)
 
 class ModelYolo(EurBaseSDK):
     def loadModel(self, modelPath) -> YOLO:
         modelFile = self.getModel(modelPath)
         if modelFile != "":
             model = YOLO(modelPath)
```

### Comparing `eurmlsdk-0.0.80/eurmlsdk/base_class.py` & `eurmlsdk-0.0.81/eurmlsdk/base_class.py`

 * *Files identical despite different names*

