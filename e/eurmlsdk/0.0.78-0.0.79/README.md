# Comparing `tmp/eurmlsdk-0.0.78.tar.gz` & `tmp/eurmlsdk-0.0.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurmlsdk-0.0.78.tar", last modified: Fri May 10 09:56:03 2024, max compression
+gzip compressed data, was "eurmlsdk-0.0.79.tar", last modified: Mon May 13 07:29:28 2024, max compression
```

## Comparing `eurmlsdk-0.0.78.tar` & `eurmlsdk-0.0.79.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-10 09:56:03.959207 eurmlsdk-0.0.78/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/LICENSE.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/MANIFEST.in
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-10 09:56:03.959207 eurmlsdk-0.0.78/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/README.md
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-10 09:56:03.949207 eurmlsdk-0.0.78/eurmlsdk/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/eurmlsdk/__init__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3255 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/eurmlsdk/__main__.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-09 09:42:44.000000 eurmlsdk-0.0.78/eurmlsdk/base_class.py
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5427 2024-05-10 09:55:14.000000 eurmlsdk-0.0.78/eurmlsdk/eur_sdk.py
-drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-10 09:56:03.959207 eurmlsdk-0.0.78/eurmlsdk.egg-info/
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/PKG-INFO
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/SOURCES.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/dependency_links.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/entry_points.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       65 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/requires.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-10 09:56:03.000000 eurmlsdk-0.0.78/eurmlsdk.egg-info/top_level.txt
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-10 09:56:03.959207 eurmlsdk-0.0.78/setup.cfg
--rw-r--r--   0 shanmu    (1000) shanmu    (1000)      765 2024-05-10 09:55:31.000000 eurmlsdk-0.0.78/setup.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 07:29:28.973101 eurmlsdk-0.0.79/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       16 2024-05-09 09:42:44.000000 eurmlsdk-0.0.79/LICENSE.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-09 09:42:44.000000 eurmlsdk-0.0.79/MANIFEST.in
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 07:29:28.973101 eurmlsdk-0.0.79/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       10 2024-05-09 09:42:44.000000 eurmlsdk-0.0.79/README.md
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 07:29:28.973101 eurmlsdk-0.0.79/eurmlsdk/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       31 2024-05-09 09:42:44.000000 eurmlsdk-0.0.79/eurmlsdk/__init__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     3103 2024-05-13 06:43:21.000000 eurmlsdk-0.0.79/eurmlsdk/__main__.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)    10466 2024-05-09 09:42:44.000000 eurmlsdk-0.0.79/eurmlsdk/base_class.py
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)     5868 2024-05-13 07:11:09.000000 eurmlsdk-0.0.79/eurmlsdk/eur_sdk.py
+drwxr-xr-x   0 shanmu    (1000) shanmu    (1000)        0 2024-05-13 07:29:28.973101 eurmlsdk-0.0.79/eurmlsdk.egg-info/
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      383 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/PKG-INFO
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      321 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        1 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       53 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/entry_points.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       79 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/requires.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)        9 2024-05-13 07:29:28.000000 eurmlsdk-0.0.79/eurmlsdk.egg-info/top_level.txt
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)       38 2024-05-13 07:29:28.973101 eurmlsdk-0.0.79/setup.cfg
+-rw-r--r--   0 shanmu    (1000) shanmu    (1000)      790 2024-05-13 07:28:58.000000 eurmlsdk-0.0.79/setup.py
```

### Comparing `eurmlsdk-0.0.78/eurmlsdk/__main__.py` & `eurmlsdk-0.0.79/eurmlsdk/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,22 +58,20 @@
     
     elif command == "deploy":
         if len(argv) < 6:
             print("Missing required arguments")
             print("Usage: eurmlsdk deploy <model path> <hostname> <username> <password>")
         else:
             localPath = argv[2]
-            remotePath = "/home/embeduradmin/" + localPath.split("/")[-1]
             hostname = argv[3]
             username = argv[4]
             password = argv[5]
             yoloSDK = ModelYolo()
-            scriptPath = "/home/embeduradmin/hello.py"
             modelFile = localPath.split("/")[-1]
-            yoloSDK.deployModel(localPath, remotePath, hostname, username, password , scriptPath , modelFile)
+            yoloSDK.deployModel(localPath,  hostname, username, password ,  modelFile)
         exit(1)
         
     else:
         print("Unknown command. Please find the list of commands")
         list_commands()
 
 if __name__ == "__main__":
```

### Comparing `eurmlsdk-0.0.78/eurmlsdk/base_class.py` & `eurmlsdk-0.0.79/eurmlsdk/base_class.py`

 * *Files identical despite different names*

### Comparing `eurmlsdk-0.0.78/eurmlsdk/eur_sdk.py` & `eurmlsdk-0.0.79/eurmlsdk/eur_sdk.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from paramiko.ssh_exception import AuthenticationException
 import paramiko
 from tqdm import tqdm
 
 class ModelNotFound(Exception):
     def __init__(self, error= "Cannot Load Model"):
         self.error = error
-        super().___init__(self.error)
+        super().__init__(self.error)
 
 class SFTPWithProgressBar(paramiko.SFTPClient):
     def put(self, localpath, remotepath, callback=None, confirm=True):
         total_size = os.stat(localpath).st_size
         with tqdm(total=total_size, unit='B', unit_scale=True, desc=remotepath) as pbar:
             def _callback(bytes_transferred, bytes_remaining):
                 pbar.update(bytes_transferred - pbar.n)
@@ -52,18 +52,18 @@
 
     def uploadToRemote(self, ssh_client, local_path, remote_path):
         print("Uploading model {} to {}".format(local_path, remote_path))
         sftp_progress_bar = SFTPWithProgressBar.from_transport(ssh_client.get_transport())
         sftp_progress_bar.put(local_path, remote_path)
         print("Model upload successful")
 
-    def uploadModel(self, ssh_client, local_path, remote_path):
+    def uploadModel(self, ssh_client, local_path, remote_path, home_path):
         try:
             sftp = ssh_client.open_sftp()
-            sftp.chdir("/home/embeduradmin/")
+            sftp.chdir(home_path)
             sftp.stat(remote_path)
             print('Model File {} already exists'.format(remote_path.split("/")[-1]))
             upload = input('Do you want to upload it again (y/n)? ')
             while upload.lower() != 'y' and upload.lower() != 'n':
                 print("Your response ('{}') was not one of the expected responses: y, n".format(upload))
                 upload = input('Do you want to upload it again (y/n)? ')
             if upload == 'y':
@@ -73,37 +73,44 @@
             self.uploadToRemote(ssh_client, local_path, remote_path)
             sftp.close()
             exit(1)
         except Exception as err:
             print("Error uploading the model file: ", err)
             exit(1)
 
-    def execute_script(self, ssh_client, script_path, modelFile):
+    def execute_ssh_script(self, ssh_client, command):
         try:
-            print("Starting script execution...")
-            stdin, stdout, stderr = ssh_client.exec_command('python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {} {}'.format(script_path , modelFile))
-            #python3 {}'.format(script_path)
+            print("Executing script")
+            stdin, stdout, stderr = ssh_client.exec_command(f'{command}')
             op = stdout.read().decode('utf-8')
-            err = stderr.read().decode('utf-8')
+            err = stdout.read().decode('utf-8')
             if op:
-                print(op)
+                return op
             if err:
-                print("Error:")
                 print(err)
+                return ""
         except Exception as err:
-            print("Error executing the script: ", err)
+            print("Error Executing the script: ", err)
             exit(1)
-        
-    def deployModel(self, local_path, remote_path, hostname, username, password, script_path, modelFile):
+              
+    def deployModel(self, local_path, hostname, username, password, modelFile):
         # Establish SSH connection
         ssh_client = self.connect_ssh_client(hostname, username, password)
-        self.uploadModel(ssh_client, local_path, remote_path)
-        self.execute_script(ssh_client, script_path , modelFile)
-        # Close SSH connection
-        ssh_client.close()
+        home_path = self.execute_ssh_script(ssh_client, 'pwd')
+        if home_path != "":
+            remote_path = (f"{home_path}/{modelFile}").replace('\n', "").strip()
+            script_path = (f'{home_path}/hello.py').replace('\n', "").strip()
+            self.uploadModel(ssh_client, local_path, remote_path, home_path)
+            script_command = f'python3 -m venv mlsdk-venv && source ./mlsdk-venv/bin/activate && pip install eurmlsdk --upgrade && python3 {script_path} {modelFile}'
+            # self.execute_script(ssh_client, script_path , modelFile)
+            execute_script = self.execute_ssh_script(ssh_client, script_command)
+            if execute_script != "":
+                print(execute_script)
+            # Close SSH connection
+            ssh_client.close()
         exit(1)
 
 class ModelYolo(EurBaseSDK):
     def loadModel(self, modelPath) -> YOLO:
         modelFile = self.getModel(modelPath)
         if modelFile != "":
             model = YOLO(modelPath)
@@ -113,21 +120,24 @@
         
     def predictModel(self, pathArg, dataSet):
         data = []
         data.append(dataSet)
         try:
             model = self.loadModel(pathArg)
             print("Prediction started.....")
-            model(data, save=True)
+            model.predict(dataSet, save=True)
         except ModelNotFound as err:
             print("Error :", err)
+            exit(1)
         except Exception as err:
             print("Error in Prediction :", err)
+            exit(1)
 
     def validateModel(self, pathArg):
         try: 
             model = self.loadModel(pathArg)
             print("Validation started........")
             metrics = model.val(data='coco8.yaml')
             print("Validated Metrics", metrics)
         except ModelNotFound as err:
-            print("Error :", err)
+            print("Error :", err)
+            exit(1)
```

### Comparing `eurmlsdk-0.0.78/setup.py` & `eurmlsdk-0.0.79/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='eurmlsdk',
-    version='0.0.78',
+    version='0.0.79',
     packages=find_packages(),
     description='eUR ML SDK',
     long_description=open('README.md').read(),
     install_requires=[
         'boto3',
+        'numpy==1.24.3',
         'python-dotenv',
         'paramiko',
         'tensorflow==2.13.1',
         'tqdm',
         'ultralytics'
     ],
     author='eUR',
```

