# Comparing `tmp/create-app-fastapi-0.0.8.tar.gz` & `tmp/create-app-fastapi-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-app-fastapi-0.0.8.tar", last modified: Sat May 11 09:16:31 2024, max compression
+gzip compressed data, was "create-app-fastapi-0.0.9.tar", last modified: Mon May 13 05:42:18 2024, max compression
```

## Comparing `create-app-fastapi-0.0.8.tar` & `create-app-fastapi-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-11 09:16:31.299889 create-app-fastapi-0.0.8/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     1118 2024-05-11 09:16:31.299889 create-app-fastapi-0.0.8/PKG-INFO
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-11 09:16:31.299889 create-app-fastapi-0.0.8/create_app_fastapi.egg-info/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     1118 2024-05-11 09:16:31.000000 create-app-fastapi-0.0.8/create_app_fastapi.egg-info/PKG-INFO
--rw-rw-r--   0 bosco     (1000) bosco     (1000)      296 2024-05-11 09:16:31.000000 create-app-fastapi-0.0.8/create_app_fastapi.egg-info/SOURCES.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)        1 2024-05-11 09:16:31.000000 create-app-fastapi-0.0.8/create_app_fastapi.egg-info/dependency_links.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       65 2024-05-11 09:16:31.000000 create-app-fastapi-0.0.8/create_app_fastapi.egg-info/entry_points.txt
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       15 2024-05-11 09:16:31.000000 create-app-fastapi-0.0.8/create_app_fastapi.egg-info/top_level.txt
-drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-11 09:16:31.299889 create-app-fastapi-0.0.8/projectfastapi/
--rw-rw-r--   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:16:31.000000 create-app-fastapi-0.0.8/projectfastapi/__init__.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     5660 2024-05-11 09:15:07.000000 create-app-fastapi-0.0.8/projectfastapi/main.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     2647 2024-05-11 08:44:02.000000 create-app-fastapi-0.0.8/projectfastapi/source.py
--rw-rw-r--   0 bosco     (1000) bosco     (1000)       38 2024-05-11 09:16:31.299889 create-app-fastapi-0.0.8/setup.cfg
--rw-rw-r--   0 bosco     (1000) bosco     (1000)     1400 2024-05-11 09:15:47.000000 create-app-fastapi-0.0.8/setup.py
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-13 05:42:18.367463 create-app-fastapi-0.0.9/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     1303 2024-05-13 05:42:18.367463 create-app-fastapi-0.0.9/PKG-INFO
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-13 05:42:18.367463 create-app-fastapi-0.0.9/create_app_fastapi.egg-info/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     1303 2024-05-13 05:42:18.000000 create-app-fastapi-0.0.9/create_app_fastapi.egg-info/PKG-INFO
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)      296 2024-05-13 05:42:18.000000 create-app-fastapi-0.0.9/create_app_fastapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)        1 2024-05-13 05:42:18.000000 create-app-fastapi-0.0.9/create_app_fastapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       65 2024-05-13 05:42:18.000000 create-app-fastapi-0.0.9/create_app_fastapi.egg-info/entry_points.txt
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       15 2024-05-13 05:42:18.000000 create-app-fastapi-0.0.9/create_app_fastapi.egg-info/top_level.txt
+drwxrwxr-x   0 bosco     (1000) bosco     (1000)        0 2024-05-13 05:42:18.367463 create-app-fastapi-0.0.9/projectfastapi/
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)        0 2024-04-27 10:16:31.000000 create-app-fastapi-0.0.9/projectfastapi/__init__.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     6424 2024-05-13 05:41:39.000000 create-app-fastapi-0.0.9/projectfastapi/main.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     3750 2024-05-13 05:35:57.000000 create-app-fastapi-0.0.9/projectfastapi/source.py
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)       38 2024-05-13 05:42:18.367463 create-app-fastapi-0.0.9/setup.cfg
+-rw-rw-r--   0 bosco     (1000) bosco     (1000)     1571 2024-05-13 05:42:05.000000 create-app-fastapi-0.0.9/setup.py
```

### Comparing `create-app-fastapi-0.0.8/PKG-INFO` & `create-app-fastapi-0.0.9/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: create-app-fastapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for initializing FastAPI projects - create-app-fastapi
 Home-page: https://github.com/ravishnu60/create-app-fastapi.git
 Author: Ravishnu
 Author-email: ravishnu60@gmail.com
 License: UNKNOWN
 Keywords: fastapi,fastapi project,project structure,api structure,python fastapi project structure
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 A package used to create fastAPI project structure with virtual environment and dependencies.
+    Can setup database connection while createing a project.
     Once you install this package use below command to create fastapi project,
     
     create-app-fastapi project-name
+	
     
     The Project structure will be created in current working directory.
     The structure will be,
     
 		root-folder
 		|-APIs
 		|  |-__init__.py
@@ -38,9 +40,11 @@
 		|  |-__init__.py
 		|  |-test_main.py
 		|-venv
 		|-.gitignore
 		|-main.py
 		|-requirements.txt
     
+        
+        ____________________________________________ Happy coding !!! __________________________________________
```

### Comparing `create-app-fastapi-0.0.8/create_app_fastapi.egg-info/PKG-INFO` & `create-app-fastapi-0.0.9/create_app_fastapi.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: create-app-fastapi
-Version: 0.0.8
+Version: 0.0.9
 Summary: Library for initializing FastAPI projects - create-app-fastapi
 Home-page: https://github.com/ravishnu60/create-app-fastapi.git
 Author: Ravishnu
 Author-email: ravishnu60@gmail.com
 License: UNKNOWN
 Keywords: fastapi,fastapi project,project structure,api structure,python fastapi project structure
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 A package used to create fastAPI project structure with virtual environment and dependencies.
+    Can setup database connection while createing a project.
     Once you install this package use below command to create fastapi project,
     
     create-app-fastapi project-name
+	
     
     The Project structure will be created in current working directory.
     The structure will be,
     
 		root-folder
 		|-APIs
 		|  |-__init__.py
@@ -38,9 +40,11 @@
 		|  |-__init__.py
 		|  |-test_main.py
 		|-venv
 		|-.gitignore
 		|-main.py
 		|-requirements.txt
     
+        
+        ____________________________________________ Happy coding !!! __________________________________________
```

### Comparing `create-app-fastapi-0.0.8/projectfastapi/main.py` & `create-app-fastapi-0.0.9/projectfastapi/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-import os, platform, sys, subprocess, threading, time, argparse
+import os, platform, sys, subprocess, threading, time, argparse, urllib, json
+import urllib.request
 from .source import getFileData
 
-version= '0.0.8'
+version= '0.0.9'
 
 def main():
     try:
         parser = argparse.ArgumentParser(prog ='create-app-fastapi', description="Create fastapi project") 
         parser.add_argument('name', metavar ='NAME', type = str, help ='create a project in this name')
         parser.add_argument('-v','--version',action='version',
                         version='%(prog)s '+version, help ="show program's version number and exit")
@@ -17,32 +18,39 @@
 
         # terminal color code
         RED = "\033[31m"
         GREEN = "\033[32m"
         RESET = "\033[0m"
 
         # validate latest version
-        out= subprocess.run("create-app-fastapi -v", shell=True, capture_output=True)
-
-        if not out.stdout.decode('utf-8').split(" ")[1][:-1] == version:
+        library_name= 'create-app-fastapi'
+        pypi_url = f'https://pypi.org/pypi/{library_name}/json'
+        response = urllib.request.urlopen(pypi_url).read().decode()
+        if version != max(json.loads(response)['releases'].keys()):
             print(RED + "Please update the latest version to access new features" + RESET)
             print("To upgrade use "+GREEN + "pip install create-app-fastapi --upgrade" + RESET)
             if (input("Do you want to continue with older ? (y/n): ").lower() != 'y'):
                 exit()
 
-        # Inputs
-        name= args.name
-        virENV= input("Virtual environment name (default 'venv'): ")
-        virENV= virENV if virENV else 'venv'
-        dependencies= ['fastapi[all]','sqlalchemy','pytest']
-
-        # get file data
-        fileData= getFileData(name, virENV)
+                # display loading
+        def loading():
+            load= 0
+            symbol=['*   ',' *  ','  * ','   *']
+            while True:
+                print("\r", end="")
+                print("Setup virtual environment and installing dependencies", end="")
+                print(GREEN,symbol[load],RESET, end="")
+                load +=1
+                time.sleep(0.5)
+                if load >= 3:   load= 0
+                if threadStop:    
+                    print()
+                    break
 
-        # create folders and files
+                # create folders and files
         def create_dir(folderName, base= False):
             fullFolderName= folderName if base else os.path.join(name, folderName)
             files= {'settings':['auth.py','config.py','db.py'], 'models':['model.py'],'schemas':['schema.py'],'APIs':['api.py'],'testcase':['test_main.py']}
             try:
                 if os.path.exists(fullFolderName):
                     exit(RED + f"Folder {fullFolderName} already exists" + RESET)
                 os.mkdir(fullFolderName)
@@ -54,43 +62,49 @@
                             f.writelines(fileData[file])
                 if not base:
                     with open(fullFolderName+'/__init__.py','w') as f:
                         pass
             except Exception as err:
                 exit(err)
 
-        # display loading
-        def loading():
-            load= 0
-            symbol=['*   ',' *  ','  * ','   *']
-            while True:
-                print("\r", end="")
-                print("Setup virtual environment and installing dependencies", end="")
-                print(GREEN,symbol[load],RESET, end="")
-                load +=1
-                time.sleep(0.5)
-                if load >= 3:   load= 0
-                if threadStop:    
-                    print()
-                    break
-
         # execute system cmd using subprocess
         def run(cmd):
             status= subprocess.run(cmd, shell=True,cwd=os.path.join(curdir, name),capture_output=True)
             if status.returncode != 0:
                 raise Exception(status.stderr.decode('utf-8'))
         
         # function to delete project if error
         def errorExit(error):
             run(f"rm -rf {os.path.join(curdir, name)}")
             exit(F"{error}\n")
 
         # thread for display loading same time of execute cmd
         thread= threading.Thread(target=loading)
 
+        # Inputs
+        name= args.name
+        virENV= input("Virtual environment name (default 'venv'): ")
+        db_data={}
+        if input("Continue with database setup ? (y/n): ").lower() == 'y':
+            db_data.update( {
+                'db':input("Database (mysql or postgresql): "),
+                'database':input("Database name: "),
+                'dbuser':input("Database user : "),
+                'password':input("Database password: "),
+                'host':input("Database host (default 'localhost'): "),
+                'port':input("Database port: "),
+            })
+        virENV= virENV if virENV else 'venv'
+        dependencies= ['fastapi[all]','sqlalchemy','pytest']
+        dependencies.append('psycopg2') if db_data.get('db').lower()=='postgresql' else dependencies.append('mysql-connector-python')
+
+        # get file data
+        fileData= getFileData(name, virENV, db_data)
+
+
         # create project directory
         create_dir(name, base= True)
 
         # Start loading thread for show loading while install dependencies
         thread.start()
         err= False
```

### Comparing `create-app-fastapi-0.0.8/projectfastapi/source.py` & `create-app-fastapi-0.0.9/projectfastapi/source.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 # include api routes with main app
 app.include_router(api.app)
 
 """
 # gitignore file data
 def gitignore(venv):
     return f"""__pycache__
-{venv}
+    .pytest_cache
+{venv}/
 .env
 """
 
 # auth file
 def auth():
     return """from fastapi.security import OAuth2PasswordBearer
 
@@ -40,21 +41,27 @@
     pass
 
 def verify_pwd():
     pass
 """
 
 # env file
-def env():
+def env(data:dict):
     return """# environment varibales here
 DATABASE=<dbname>
 DBUSER=<dbusername>
 PASSWORD=<db password>
 HOST=<db host>
 PORT=<db port>
+""" if not data.keys() else f"""# environment varibales here
+DATABASE={data['database']}
+DBUSER={data['dbuser']}
+PASSWORD={data['password']}
+HOST={'localhost' if data['host']=='' else data['host']}
+PORT={data['port']}
 """
 
 # config file
 def config():
     return """from pydantic_settings import BaseSettings, SettingsConfigDict
     
 # env variable access code here
@@ -68,21 +75,56 @@
     model_config= SettingsConfigDict(env_file=".env")
     
 secret= Secret()
 
 """
 
 #db file
-def db():
-    return"""from sqlalchemy import create_engine, URL
-from sqlalchemy.orm import sessionmaker
-from sqlalchemy.ext.declarative import declarative_base
-from config import secret
+def db(data:dict):
+    db= False
+    if data.keys():
+        if data['db'].lower()=='mysql':
+            driver= 'mysql+mysqlconnector'
+        else:
+            driver= 'postgresql'
+        db=f"""
+db_url= URL.create(
+    drivername= '{driver}',
+    username= secret.dbuser,
+    password= secret.password,
+    host= secret.host,
+    port= secret.port
+)
+
+engine= create_engine(db_url, pool_pre_ping= True)
+session_local= sessionmaker(autocommit= False, autoflush= False, bind= engine)
+Base= declarative_base()
+
+def get_db():
+    db= session_local()
+    try:
+        yield db
+    finally:
+        db.close()
+
+try:
+    db= session_local()
+    db.execute(text('SELECT 1'))
+    print('\\n----- Connected to db! -----')
+except Exception as e:
+    print('\\n----- Connection failed! ERROR : ', e)
+
+"""
+
+    return f"""from sqlalchemy import create_engine, URL, {'text' if db else ''}
+from sqlalchemy.orm import sessionmaker, declarative_base
+from settings.config import secret
 
 # database connection code here
+{db if db else ''}
 """
 #model file
 def model():
     return"""from sqlalchemy import Column, Integer, String, Float
 from settings.db import Base
 
 # model code here
@@ -94,14 +136,15 @@
 # schema code here
 class Sample(BaseModel):
     pass
 """
 #api file
 def api():
     return """from fastapi import APIRouter
+from settings.db import get_db
 
 # api code here
 app= APIRouter(
     prefix="/api/v1",
     tags=["api"]
 )
 @app.get('/')
@@ -123,21 +166,21 @@
 
 # the api test case
 def test_api():
     response= client.get('/api/v1')
     assert response.status_code == 200
 """ 
 
-def getFileData(name, venv):
+def getFileData(name, venv, db_data):
     return {
             'auth.py': auth(),
             'config.py': config(),
-            'db.py': db(),
+            'db.py': db(db_data),
             'model.py': model(),
             'schema.py': schema(),
             'api.py': api(),
             'main.py': main(name),
             'test_main.py': test_main(),
             '.gitignore':gitignore(venv),
-            '.env':env(),
+            '.env':env(db_data),
             }
```

### Comparing `create-app-fastapi-0.0.8/setup.py` & `create-app-fastapi-0.0.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from setuptools import setup, find_packages
 from projectfastapi.main import version
-print(version)
+
 setup( 
 	name="create-app-fastapi", 
 	version= version, 
 	author="Ravishnu", 
 	author_email="ravishnu60@gmail.com", 
 	packages=find_packages(), 
     url="https://github.com/ravishnu60/create-app-fastapi.git",
 	description="Library for initializing FastAPI projects - create-app-fastapi", 
 	long_description="""A package used to create fastAPI project structure with virtual environment and dependencies.
+    Can setup database connection while createing a project.
     Once you install this package use below command to create fastapi project,
     
     create-app-fastapi project-name
+	
     
     The Project structure will be created in current working directory.
     The structure will be,
     
 		root-folder
 		|-APIs
 		|  |-__init__.py
@@ -36,14 +38,16 @@
 		|  |-__init__.py
 		|  |-test_main.py
 		|-venv
 		|-.gitignore
 		|-main.py
 		|-requirements.txt
     
+        
+        ____________________________________________ Happy coding !!! __________________________________________
     """, 
 	long_description_content_type="text/markdown", 
 	python_requires='>=3.9', 
 	install_requires=[],
 	entry_points ={ 
 		'console_scripts': [ 
 			'create-app-fastapi=projectfastapi.main:main'
```

