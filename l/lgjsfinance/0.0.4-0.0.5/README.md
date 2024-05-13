# Comparing `tmp/lgjsfinance-0.0.4.tar.gz` & `tmp/lgjsfinance-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lgjsfinance-0.0.4.tar", last modified: Mon May 13 07:58:30 2024, max compression
+gzip compressed data, was "lgjsfinance-0.0.5.tar", last modified: Mon May 13 08:09:22 2024, max compression
```

## Comparing `lgjsfinance-0.0.4.tar` & `lgjsfinance-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 07:58:30.200429 lgjsfinance-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-05-13 07:32:41.000000 lgjsfinance-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      759 2024-05-13 07:58:30.196429 lgjsfinance-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-05-13 07:47:19.000000 lgjsfinance-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 07:58:30.149574 lgjsfinance-0.0.4/lgjsfinance/
--rw-rw-rw-   0        0        0      136 2024-05-13 07:58:24.000000 lgjsfinance-0.0.4/lgjsfinance/__init__.py
--rw-rw-rw-   0        0        0     1112 2024-05-13 07:47:35.000000 lgjsfinance-0.0.4/lgjsfinance/module.py
-drwxrwxrwx   0        0        0        0 2024-05-13 07:58:30.193431 lgjsfinance-0.0.4/lgjsfinance.egg-info/
--rw-rw-rw-   0        0        0      759 2024-05-13 07:58:29.000000 lgjsfinance-0.0.4/lgjsfinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-13 07:58:30.000000 lgjsfinance-0.0.4/lgjsfinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 07:58:29.000000 lgjsfinance-0.0.4/lgjsfinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-13 07:58:29.000000 lgjsfinance-0.0.4/lgjsfinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-13 07:58:29.000000 lgjsfinance-0.0.4/lgjsfinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 07:58:30.200429 lgjsfinance-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      931 2024-05-13 07:58:20.000000 lgjsfinance-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:09:22.431537 lgjsfinance-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-05-13 07:32:41.000000 lgjsfinance-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1186 2024-05-13 08:09:22.428544 lgjsfinance-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-05-13 07:47:19.000000 lgjsfinance-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 08:09:22.369275 lgjsfinance-0.0.5/lgjsfinance/
+-rw-rw-rw-   0        0        0      136 2024-05-13 08:09:02.000000 lgjsfinance-0.0.5/lgjsfinance/__init__.py
+-rw-rw-rw-   0        0        0     1112 2024-05-13 07:47:35.000000 lgjsfinance-0.0.5/lgjsfinance/module.py
+drwxrwxrwx   0        0        0        0 2024-05-13 08:09:22.425535 lgjsfinance-0.0.5/lgjsfinance.egg-info/
+-rw-rw-rw-   0        0        0     1186 2024-05-13 08:09:22.000000 lgjsfinance-0.0.5/lgjsfinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-13 08:09:22.000000 lgjsfinance-0.0.5/lgjsfinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 08:09:22.000000 lgjsfinance-0.0.5/lgjsfinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-13 08:09:22.000000 lgjsfinance-0.0.5/lgjsfinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-13 08:09:22.000000 lgjsfinance-0.0.5/lgjsfinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 08:09:22.431537 lgjsfinance-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2024-05-13 08:09:13.000000 lgjsfinance-0.0.5/setup.py
```

### Comparing `lgjsfinance-0.0.4/LICENSE` & `lgjsfinance-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lgjsfinance-0.0.4/PKG-INFO` & `lgjsfinance-0.0.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 Metadata-Version: 2.1
 Name: lgjsfinance
-Version: 0.0.4
+Version: 0.0.5
 Summary: LGJS Finance
 Home-page: https://liamgenjs.vercel.app
 Author: liamgen.js
 Author-email: liamgen.js@proton.me
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: yfinance>=0.2.38
 Requires-Dist: matplotlib
 Requires-Dist: datetime
+
+# Import des packages
+from lgjsfinance import DataRecover
+
+# Definir la classe et la currency
+data = DataRecover("EURUSD=X")
+
+# RÃ©cupÃ©rer l'historique des prix de la journÃ©e
+historique_prix = data.get_close_prices_hourly()
+
+# RÃ©cupÃ©rer les 16 derniÃ¨res donnÃ©es
+print(historique_prix.tail(16))
+
+# Tracer le graphique
+data.show_graph(historique_prix)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lgjsfinance-0.0.4/lgjsfinance/module.py` & `lgjsfinance-0.0.5/lgjsfinance/module.py`

 * *Files identical despite different names*

### Comparing `lgjsfinance-0.0.4/lgjsfinance.egg-info/PKG-INFO` & `lgjsfinance-0.0.5/lgjsfinance.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 Metadata-Version: 2.1
 Name: lgjsfinance
-Version: 0.0.4
+Version: 0.0.5
 Summary: LGJS Finance
 Home-page: https://liamgenjs.vercel.app
 Author: liamgen.js
 Author-email: liamgen.js@proton.me
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: yfinance>=0.2.38
 Requires-Dist: matplotlib
 Requires-Dist: datetime
+
+# Import des packages
+from lgjsfinance import DataRecover
+
+# Definir la classe et la currency
+data = DataRecover("EURUSD=X")
+
+# RÃ©cupÃ©rer l'historique des prix de la journÃ©e
+historique_prix = data.get_close_prices_hourly()
+
+# RÃ©cupÃ©rer les 16 derniÃ¨res donnÃ©es
+print(historique_prix.tail(16))
+
+# Tracer le graphique
+data.show_graph(historique_prix)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

