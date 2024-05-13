# Comparing `tmp/exponentation-0.0.5.tar.gz` & `tmp/exponentation-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exponentation-0.0.5.tar", last modified: Sun May 12 19:56:55 2024, max compression
+gzip compressed data, was "exponentation-0.0.6.tar", last modified: Mon May 13 14:24:14 2024, max compression
```

## Comparing `exponentation-0.0.5.tar` & `exponentation-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-12 19:56:55.044642 exponentation-0.0.5/
--rw-rw-rw-   0        0        0       75 2024-05-12 19:38:19.000000 exponentation-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      617 2024-05-12 19:56:55.044642 exponentation-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-11 19:12:12.000000 exponentation-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-12 19:56:55.029040 exponentation-0.0.5/exponentation/
--rw-rw-rw-   0        0        0 14089821 2024-05-03 15:48:36.000000 exponentation-0.0.5/exponentation/Data_learning.csv
--rw-rw-rw-   0        0        0       47 2024-05-11 19:22:20.000000 exponentation-0.0.5/exponentation/__init__.py
--rw-rw-rw-   0        0        0     2458 2024-05-11 19:24:51.000000 exponentation-0.0.5/exponentation/methods.py
--rw-rw-rw-   0        0        0    33030 2024-05-10 16:20:40.000000 exponentation-0.0.5/exponentation/my_model.pth
--rw-rw-rw-   0        0        0     4538 2024-05-12 19:52:59.000000 exponentation-0.0.5/exponentation/neuron.py
-drwxrwxrwx   0        0        0        0 2024-05-12 19:56:55.044642 exponentation-0.0.5/exponentation.egg-info/
--rw-rw-rw-   0        0        0      617 2024-05-12 19:56:54.000000 exponentation-0.0.5/exponentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2024-05-12 19:56:54.000000 exponentation-0.0.5/exponentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-12 19:56:54.000000 exponentation-0.0.5/exponentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-12 19:56:54.000000 exponentation-0.0.5/exponentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-12 19:56:54.000000 exponentation-0.0.5/exponentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-12 19:56:55.044642 exponentation-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      868 2024-05-12 19:53:53.000000 exponentation-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:24:14.786175 exponentation-0.0.6/
+-rw-rw-rw-   0        0        0      617 2024-05-13 14:24:14.786175 exponentation-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-11 19:12:12.000000 exponentation-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 14:24:14.754899 exponentation-0.0.6/exponentation/
+-rw-rw-rw-   0        0        0       47 2024-05-11 19:22:20.000000 exponentation-0.0.6/exponentation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:24:14.786175 exponentation-0.0.6/exponentation/data/
+-rw-rw-rw-   0        0        0    33030 2024-05-10 16:20:40.000000 exponentation-0.0.6/exponentation/data/my_model.pth
+-rw-rw-rw-   0        0        0     2458 2024-05-11 19:24:51.000000 exponentation-0.0.6/exponentation/methods.py
+-rw-rw-rw-   0        0        0     4546 2024-05-13 14:19:18.000000 exponentation-0.0.6/exponentation/neuron.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:24:14.786175 exponentation-0.0.6/exponentation.egg-info/
+-rw-rw-rw-   0        0        0      617 2024-05-13 14:24:14.000000 exponentation-0.0.6/exponentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      319 2024-05-13 14:24:14.000000 exponentation-0.0.6/exponentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:24:14.000000 exponentation-0.0.6/exponentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-13 14:24:14.000000 exponentation-0.0.6/exponentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-13 14:24:14.000000 exponentation-0.0.6/exponentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:24:14.786175 exponentation-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      959 2024-05-13 14:23:37.000000 exponentation-0.0.6/setup.py
```

### Comparing `exponentation-0.0.5/PKG-INFO` & `exponentation-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exponentation
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is the simplest module for quick work with files.
 Home-page: https://github.com/katya_r/exponentation
 Author: katya_r
 Author-email: katerina.riabova@gmail.com
 Project-URL: GitHub, https://github.com/your_username/your_project
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `exponentation-0.0.5/exponentation/methods.py` & `exponentation-0.0.6/exponentation/methods.py`

 * *Files identical despite different names*

### Comparing `exponentation-0.0.5/exponentation/my_model.pth` & `exponentation-0.0.6/exponentation/data/my_model.pth`

 * *Files identical despite different names*

### Comparing `exponentation-0.0.5/exponentation/neuron.py` & `exponentation-0.0.6/exponentation/neuron.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 import torch
 import torch.nn as nn
 import numpy as np
 from .methods import *
 
-file_path = './Data_learning.csv'
+file_path = 'data/Data_learning.csv'
 train_data = pd.read_csv(file_path)
 
 class Exponentation(nn.Module):
     def __init__(self):
         super(Exponentation, self).__init__()
         self.fc1 = nn.Linear(4, 32)
         self.relu = nn.ReLU()
@@ -29,15 +29,15 @@
         memory_prediction = self.fc_memory(x)
 
         return time_prediction, memory_prediction
 
 
 model = Exponentation()
 
-model.load_state_dict(torch.load('my_model.pth'))
+model.load_state_dict(torch.load('data/my_model.pth'))
 
 # Перевод модели в режим оценки
 model.eval()
 
 
 def get_key(d, value):
     for k, v in d.items():
```

### Comparing `exponentation-0.0.5/exponentation.egg-info/PKG-INFO` & `exponentation-0.0.6/exponentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exponentation
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is the simplest module for quick work with files.
 Home-page: https://github.com/katya_r/exponentation
 Author: katya_r
 Author-email: katerina.riabova@gmail.com
 Project-URL: GitHub, https://github.com/your_username/your_project
 Keywords: files speedfiles
 Classifier: Programming Language :: Python :: 3.11
```

