# Comparing `tmp/exponentation-0.0.6.tar.gz` & `tmp/exponentation-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exponentation-0.0.6.tar", last modified: Mon May 13 14:24:14 2024, max compression
+gzip compressed data, was "exponentation-0.0.7.tar", last modified: Mon May 13 14:54:15 2024, max compression
```

## Comparing `exponentation-0.0.6.tar` & `exponentation-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:24:14.786175 exponentation-0.0.6/
--rw-rw-rw-   0        0        0      617 2024-05-13 14:24:14.786175 exponentation-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-11 19:12:12.000000 exponentation-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 14:24:14.754899 exponentation-0.0.6/exponentation/
--rw-rw-rw-   0        0        0       47 2024-05-11 19:22:20.000000 exponentation-0.0.6/exponentation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:24:14.786175 exponentation-0.0.6/exponentation/data/
--rw-rw-rw-   0        0        0    33030 2024-05-10 16:20:40.000000 exponentation-0.0.6/exponentation/data/my_model.pth
--rw-rw-rw-   0        0        0     2458 2024-05-11 19:24:51.000000 exponentation-0.0.6/exponentation/methods.py
--rw-rw-rw-   0        0        0     4546 2024-05-13 14:19:18.000000 exponentation-0.0.6/exponentation/neuron.py
-drwxrwxrwx   0        0        0        0 2024-05-13 14:24:14.786175 exponentation-0.0.6/exponentation.egg-info/
--rw-rw-rw-   0        0        0      617 2024-05-13 14:24:14.000000 exponentation-0.0.6/exponentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2024-05-13 14:24:14.000000 exponentation-0.0.6/exponentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:24:14.000000 exponentation-0.0.6/exponentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-13 14:24:14.000000 exponentation-0.0.6/exponentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-13 14:24:14.000000 exponentation-0.0.6/exponentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 14:24:14.786175 exponentation-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      959 2024-05-13 14:23:37.000000 exponentation-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:15.432483 exponentation-0.0.7/
+-rw-rw-rw-   0        0        0      617 2024-05-13 14:54:15.432483 exponentation-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-11 19:12:12.000000 exponentation-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:15.401319 exponentation-0.0.7/exponentation/
+-rw-rw-rw-   0        0        0       47 2024-05-11 19:22:20.000000 exponentation-0.0.7/exponentation/__init__.py
+-rw-rw-rw-   0        0        0     2458 2024-05-11 19:24:51.000000 exponentation-0.0.7/exponentation/methods.py
+-rw-rw-rw-   0        0        0     4556 2024-05-13 14:52:44.000000 exponentation-0.0.7/exponentation/neuron.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:54:15.432483 exponentation-0.0.7/exponentation.egg-info/
+-rw-rw-rw-   0        0        0      617 2024-05-13 14:54:15.000000 exponentation-0.0.7/exponentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-13 14:54:15.000000 exponentation-0.0.7/exponentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:54:15.000000 exponentation-0.0.7/exponentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-13 14:54:15.000000 exponentation-0.0.7/exponentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 14:54:15.000000 exponentation-0.0.7/exponentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:54:15.432483 exponentation-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1002 2024-05-13 14:54:11.000000 exponentation-0.0.7/setup.py
```

### Comparing `exponentation-0.0.6/PKG-INFO` & `exponentation-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exponentation
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is the simplest module for quick work with files.
 Home-page: https://github.com/katya_r/exponentation
 Author: katya_r
 Author-email: katerina.riabova@gmail.com
 Project-URL: GitHub, https://github.com/your_username/your_project
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `exponentation-0.0.6/exponentation/methods.py` & `exponentation-0.0.7/exponentation/methods.py`

 * *Files identical despite different names*

### Comparing `exponentation-0.0.6/exponentation/neuron.py` & `exponentation-0.0.7/exponentation/neuron.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import pandas as pd
 import torch
 import torch.nn as nn
 import numpy as np
 from .methods import *
 
-file_path = 'data/Data_learning.csv'
+
+file_path = '../data/Data_learning.csv'
 train_data = pd.read_csv(file_path)
 
+
 class Exponentation(nn.Module):
     def __init__(self):
         super(Exponentation, self).__init__()
         self.fc1 = nn.Linear(4, 32)
         self.relu = nn.ReLU()
         self.fc2 = nn.Linear(32, 64)
         self.fc3 = nn.Linear(64, 64)
@@ -29,15 +31,15 @@
         memory_prediction = self.fc_memory(x)
 
         return time_prediction, memory_prediction
 
 
 model = Exponentation()
 
-model.load_state_dict(torch.load('data/my_model.pth'))
+model.load_state_dict(torch.load('../data/my_model.pth'))
 
 # Перевод модели в режим оценки
 model.eval()
 
 
 def get_key(d, value):
     for k, v in d.items():
```

### Comparing `exponentation-0.0.6/exponentation.egg-info/PKG-INFO` & `exponentation-0.0.7/exponentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exponentation
-Version: 0.0.6
+Version: 0.0.7
 Summary: This is the simplest module for quick work with files.
 Home-page: https://github.com/katya_r/exponentation
 Author: katya_r
 Author-email: katerina.riabova@gmail.com
 Project-URL: GitHub, https://github.com/your_username/your_project
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `exponentation-0.0.6/setup.py` & `exponentation-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='exponentation',
-  version='0.0.6',
+  version='0.0.7',
   author='katya_r',
   author_email='katerina.riabova@gmail.com',
   description='This is the simplest module for quick work with files.',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/katya_r/exponentation',
   packages=find_packages(),
@@ -28,9 +28,11 @@
   ],
   keywords='files speedfiles ',
   project_urls={
     'GitHub': 'https://github.com/your_username/your_project'
   },
   python_requires='>=3.6',
   include_package_data=True,
-  package_data={'': ['data/*.csv'], '': ['data/*.pth']},
+    package_data={
+        'exponentation': ['data/Data_learning.csv', 'data/my_model.pth']
+    }
 )
```

