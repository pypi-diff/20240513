# Comparing `tmp/eurmlsdk-0.0.79.tar.gz` & `tmp/eurmlsdk-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.79.tar", last modified: Mon May 13 07:29:28 2024, max compression
+gzip compressed data, was "dist/eurmlsdk-0.0.80.tar", last modified: Mon May 13 10:13:36 2024, max compression
```

## Comparing `eurmlsdk-0.0.79.tar` & `eurmlsdk-0.0.80.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 07:29:28.973101 eurmlsdk-0.0.79/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.79/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.79/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 07:29:28.973101 eurmlsdk-0.0.79/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.79/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 07:29:28.973101 eurmlsdk-0.0.79/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-09 09:42:44.000000 eurmlsdk-0.0.79/eurmlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3103 2024-05-13 06:43:21.000000 eurmlsdk-0.0.79/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-09 09:42:44.000000 eurmlsdk-0.0.79/eurmlsdk/base_class.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5868 2024-05-13 07:11:09.000000 eurmlsdk-0.0.79/eurmlsdk/eur_sdk.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 07:29:28.973101 eurmlsdk-0.0.79/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       79 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-13 07:29:28.973101 eurmlsdk-0.0.79/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      790 2024-05-13 07:28:58.000000 eurmlsdk-0.0.79/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.80/README.md
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.80/MANIFEST.in
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       79 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      790 2024-05-13 10:13:31.000000 eurmlsdk-0.0.80/setup.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.80/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/PKG-INFO
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 10:13:36.000000 eurmlsdk-0.0.80/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3430 2024-05-13 10:08:36.000000 eurmlsdk-0.0.80/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     6031 2024-05-13 10:08:24.000000 eurmlsdk-0.0.80/eurmlsdk/eur_sdk.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-09 09:42:44.000000 eurmlsdk-0.0.80/eurmlsdk/base_class.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-09 09:42:44.000000 eurmlsdk-0.0.80/eurmlsdk/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `eurmlsdk-0.0.79/eurmlsdk/__main__.py` & `eurmlsdk-0.0.80/eurmlsdk/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     print("     <hostname>   : hostname to connect to Raspberry pi")
     print("     <username>   : username to connect to Raspberry pi")
     print("     <password>   : password to connect to Raspberry pi")
     print("  help | --h                : Lists all commands available in mlsdk package")
     print("  predict <model path> <dataset> : Predicts the labels and saves the predicted image")
     print("     <model path> : path to the model file")
     print("     <dataset>    : sample dataset image")
-    print("  validate <model path>     : Validates the model and returns the metrics using default dataset")
+    print("  validate <dataType> <model path>     : Validates the model and returns the metrics using default dataset")
+    print("     <dataType>    : dataType can be of the string 'seg'  'pose' 'detect' 'classify' ")
 
 def main(): 
     if len(argv) == 1:
         print("Model Zoo SDK")
         print("Package name: eurmlsdk")
         print("Version: 0.0.76")
         print("Run 'eurmlsdk help' or eurmlsdk --h to find the list of commands.")
@@ -30,20 +31,26 @@
 
     command = argv[1]
     if command == "help" or command == "--h":
         list_commands()
         exit(1)
         
     elif command == "validate":
-        if len(argv) <3:
-            print("Give the model file name or file path")
+        taskList = ["seg", "pose", "classify", "detect"]
+        if len(argv) <4:
+            print("Please provide task type and model path")
+            exit(1)
+        elif argv[2] not in taskList:
+            print("Please provide valid task")
+            exit(1)
         else:
-            modelPath = argv[2]
+            modelPath = argv[3]
+            task = argv[2]
             yoloSDK = ModelYolo()
-            yoloSDK.validateModel(modelPath)
+            yoloSDK.validateModel(modelPath, task)
         exit(1)
         
     elif command == "predict":
         if len(argv) <3:
             print("Give the model file name or file file path")
             exit(1)
         elif len(argv) <4:
```

### Comparing `eurmlsdk-0.0.79/eurmlsdk/base_class.py` & `eurmlsdk-0.0.80/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.79/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.80/eurmlsdk/eur_sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,35 +55,36 @@
         sftp_progress_bar = SFTPWithProgressBar.from_transport(ssh_client.get_transport())
         sftp_progress_bar.put(local_path, remote_path)
         print("Model upload successful")
 
     def uploadModel(self, ssh_client, local_path, remote_path, home_path):
         try:
             sftp = ssh_client.open_sftp()
-            sftp.chdir(home_path)
+            print("Checking for model file in {}".format(home_path))
             sftp.stat(remote_path)
-            print('Model File {} already exists'.format(remote_path.split("/")[-1]))
+            print('Model File already exists')
             upload = input('Do you want to upload it again (y/n)? ')
             while upload.lower() != 'y' and upload.lower() != 'n':
                 print("Your response ('{}') was not one of the expected responses: y, n".format(upload))
                 upload = input('Do you want to upload it again (y/n)? ')
             if upload == 'y':
                 self.uploadToRemote(ssh_client, local_path, remote_path)
             sftp.close()
         except IOError:
+            print("Model File does not exist")
             self.uploadToRemote(ssh_client, local_path, remote_path)
             sftp.close()
-            exit(1)
         except Exception as err:
             print("Error uploading the model file: ", err)
             exit(1)
 
     def execute_ssh_script(self, ssh_client, command):
         try:
-            print("Executing script")
+            if command != "pwd":
+                print("Executing script")
             stdin, stdout, stderr = ssh_client.exec_command(f'{command}')
             op = stdout.read().decode('utf-8')
             err = stdout.read().decode('utf-8')
             if op:
                 return op
             if err:
                 print(err)
@@ -115,29 +116,31 @@
         if modelFile != "":
             model = YOLO(modelPath)
             return model 
         else:
             raise ModelNotFound()
         
     def predictModel(self, pathArg, dataSet):
-        data = []
-        data.append(dataSet)
         try:
             model = self.loadModel(pathArg)
             print("Prediction started.....")
             model.predict(dataSet, save=True)
         except ModelNotFound as err:
             print("Error :", err)
             exit(1)
         except Exception as err:
             print("Error in Prediction :", err)
             exit(1)
 
-    def validateModel(self, pathArg):
+    def validateModel(self, pathArg, task):
         try: 
             model = self.loadModel(pathArg)
             print("Validation started........")
-            metrics = model.val(data='coco8.yaml')
+            dataset = {
+                "seg" : "coco8-seg.yaml",
+                "pose" : "coco8-pose.yaml",
+            }
+            metrics = model.val(data=dataset.get(task, "coco8.yaml"))
             print("Validated Metrics", metrics)
         except ModelNotFound as err:
             print("Error :", err)
             exit(1)
```

### Comparing `eurmlsdk-0.0.79/setup.py` & `eurmlsdk-0.0.80/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.79',
+    version='0.0.80',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
         'numpy==1.24.3',
         'python-dotenv',
```

