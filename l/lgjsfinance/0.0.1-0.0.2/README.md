# Comparing `tmp/lgjsfinance-0.0.1.tar.gz` & `tmp/lgjsfinance-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lgjsfinance-0.0.1.tar", last modified: Mon May 13 07:37:43 2024, max compression
+gzip compressed data, was "lgjsfinance-0.0.2.tar", last modified: Mon May 13 07:48:22 2024, max compression
```

## Comparing `lgjsfinance-0.0.1.tar` & `lgjsfinance-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:42.997036 lgjsfinance-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-05-13 07:32:41.000000 lgjsfinance-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      780 2024-05-13 07:37:42.994032 lgjsfinance-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-13 07:29:56.000000 lgjsfinance-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:42.918668 lgjsfinance-0.0.1/lgjsfinance/
--rw-rw-rw-   0        0        0      101 2024-05-13 07:36:56.000000 lgjsfinance-0.0.1/lgjsfinance/__init__.py
--rw-rw-rw-   0        0        0     1771 2024-05-13 07:35:44.000000 lgjsfinance-0.0.1/lgjsfinance/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:37:42.992033 lgjsfinance-0.0.1/lgjsfinance.egg-info/
--rw-rw-rw-   0        0        0      780 2024-05-13 07:37:42.000000 lgjsfinance-0.0.1/lgjsfinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2024-05-13 07:37:42.000000 lgjsfinance-0.0.1/lgjsfinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 07:37:42.000000 lgjsfinance-0.0.1/lgjsfinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 07:37:42.000000 lgjsfinance-0.0.1/lgjsfinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-13 07:37:42.000000 lgjsfinance-0.0.1/lgjsfinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 07:37:42.998034 lgjsfinance-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      962 2024-05-13 07:35:53.000000 lgjsfinance-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:48:22.884774 lgjsfinance-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-05-13 07:32:41.000000 lgjsfinance-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      759 2024-05-13 07:48:22.882772 lgjsfinance-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-05-13 07:47:19.000000 lgjsfinance-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 07:48:22.812351 lgjsfinance-0.0.2/lgjsfinance/
+-rw-rw-rw-   0        0        0      101 2024-05-13 07:48:09.000000 lgjsfinance-0.0.2/lgjsfinance/__init__.py
+-rw-rw-rw-   0        0        0     1112 2024-05-13 07:47:35.000000 lgjsfinance-0.0.2/lgjsfinance/main.py
+drwxrwxrwx   0        0        0        0 2024-05-13 07:48:22.881759 lgjsfinance-0.0.2/lgjsfinance.egg-info/
+-rw-rw-rw-   0        0        0      759 2024-05-13 07:48:22.000000 lgjsfinance-0.0.2/lgjsfinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2024-05-13 07:48:22.000000 lgjsfinance-0.0.2/lgjsfinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 07:48:22.000000 lgjsfinance-0.0.2/lgjsfinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-13 07:48:22.000000 lgjsfinance-0.0.2/lgjsfinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 07:48:22.000000 lgjsfinance-0.0.2/lgjsfinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 07:48:22.885774 lgjsfinance-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      931 2024-05-13 07:47:46.000000 lgjsfinance-0.0.2/setup.py
```

### Comparing `lgjsfinance-0.0.1/LICENSE` & `lgjsfinance-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lgjsfinance-0.0.1/PKG-INFO` & `lgjsfinance-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lgjsfinance
-Version: 0.0.1
+Version: 0.0.2
 Summary: LGJS Finance
 Home-page: https://liamgenjs.vercel.app
 Author: liamgen.js
 Author-email: liamgen.js@proton.me
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -15,8 +15,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 License-File: LICENSE
 Requires-Dist: yfinance>=0.2.38
 Requires-Dist: matplotlib
 Requires-Dist: datetime
-Requires-Dist: time
```

### Comparing `lgjsfinance-0.0.1/lgjsfinance/main.py` & `lgjsfinance-0.0.2/lgjsfinance/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import yfinance as yf
 import matplotlib.pyplot as plt
-import time as tps
-from datetime import datetime, time
+from datetime import datetime
 
 class Settings:
     max_cache_age = 60
 
 class DataRecover():
     def __init__(self, entreprise, settings=Settings()):
         self.corp = entreprise
@@ -25,31 +24,9 @@
         plt.xlabel('Date')
         plt.ylabel('Prix de clôture (en $)')
         plt.legend()
         plt.grid(True)
         plt.show()#2714.735107
 
     def get_close_prices_hourly(self):
-        date_a_minuit = datetime.combine(datetime.now().replace(hour=0, minute=0, second=0, microsecond=0), time.min)
         historique_prix = yf.download(self.corp, start=datetime.now().replace(hour=0, minute=0, second=0, microsecond=0), interval='1m')
-        return historique_prix
-
-
-start_time = tps.time()
-
-data = DataRecover("EURUSD=X")
-
-historique_prix = data.get_close_prices_hourly()
-print(type(historique_prix.tail(16)))
-#print(historique_prix)
-
-"""while True:
-    historique_prix = data.get_data()
-    print("Prix de cloture : ", historique_prix.iloc[-1]['Close'])
-    tps.sleep(30)"""
-
-end_time = tps.time()
-duree_requete = end_time - start_time
-print("La requête a pris {} secondes.".format(duree_requete))
-
-# Tracer le graphique
-#data.show_graph(historique_prix)
+        return historique_prix
```

### Comparing `lgjsfinance-0.0.1/lgjsfinance.egg-info/PKG-INFO` & `lgjsfinance-0.0.2/lgjsfinance.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lgjsfinance
-Version: 0.0.1
+Version: 0.0.2
 Summary: LGJS Finance
 Home-page: https://liamgenjs.vercel.app
 Author: liamgen.js
 Author-email: liamgen.js@proton.me
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -15,8 +15,7 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 License-File: LICENSE
 Requires-Dist: yfinance>=0.2.38
 Requires-Dist: matplotlib
 Requires-Dist: datetime
-Requires-Dist: time
```

### Comparing `lgjsfinance-0.0.1/setup.py` & `lgjsfinance-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup
 
 setup(
     name='lgjsfinance',
-    version='0.0.1',    
+    version='0.0.2',    
     description='LGJS Finance',
     url='https://liamgenjs.vercel.app',
     author='liamgen.js',
     author_email='liamgen.js@proton.me',
     license='BSD 2-clause',
     packages=['lgjsfinance'],
     install_requires=['yfinance>=0.2.38',
                       'matplotlib',
-                      'datetime',
-                      'time'                 
+                      'datetime',                
                       ],
 
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: BSD License',  
         'Operating System :: POSIX :: Linux',
```

