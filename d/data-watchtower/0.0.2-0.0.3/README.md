# Comparing `tmp/data_watchtower-0.0.2.tar.gz` & `tmp/data_watchtower-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_watchtower-0.0.2.tar", last modified: Sun May  5 07:24:00 2024, max compression
+gzip compressed data, was "data_watchtower-0.0.3.tar", last modified: Mon May  6 08:22:17 2024, max compression
```

## Comparing `data_watchtower-0.0.2.tar` & `data_watchtower-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.348128 data_watchtower-0.0.2/
--rw-rw-rw-   0        0        0     1090 2024-05-01 02:10:55.000000 data_watchtower-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      511 2024-05-05 07:24:00.348128 data_watchtower-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2435 2024-05-03 13:56:51.000000 data_watchtower-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.271070 data_watchtower-0.0.2/data_watchtower/
--rw-rw-rw-   0        0        0      270 2024-05-05 07:21:20.000000 data_watchtower-0.0.2/data_watchtower/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.288437 data_watchtower-0.0.2/data_watchtower/api/
--rw-rw-rw-   0        0        0       48 2024-05-03 02:34:32.000000 data_watchtower-0.0.2/data_watchtower/api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.301283 data_watchtower-0.0.2/data_watchtower/api/handlers/
--rw-rw-rw-   0        0        0       48 2024-05-03 03:21:05.000000 data_watchtower-0.0.2/data_watchtower/api/handlers/__init__.py
--rw-rw-rw-   0        0        0      845 2024-05-05 04:43:17.000000 data_watchtower-0.0.2/data_watchtower/api/handlers/base.py
--rw-rw-rw-   0        0        0      553 2024-05-03 12:39:06.000000 data_watchtower-0.0.2/data_watchtower/api/handlers/watchtower.py
--rw-rw-rw-   0        0        0      835 2024-05-05 04:40:00.000000 data_watchtower-0.0.2/data_watchtower/api/server.py
--rw-rw-rw-   0        0        0      291 2024-05-05 06:57:58.000000 data_watchtower-0.0.2/data_watchtower/api/url.py
-drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.320817 data_watchtower-0.0.2/data_watchtower/core/
--rw-rw-rw-   0        0        0       48 2024-04-26 07:27:27.000000 data_watchtower-0.0.2/data_watchtower/core/__init__.py
--rw-rw-rw-   0        0        0     2809 2024-05-05 04:36:42.000000 data_watchtower-0.0.2/data_watchtower/core/base.py
--rw-rw-rw-   0        0        0     1138 2024-05-03 09:14:39.000000 data_watchtower-0.0.2/data_watchtower/core/data_loaders.py
--rw-rw-rw-   0        0        0     1546 2024-05-03 04:45:13.000000 data_watchtower-0.0.2/data_watchtower/core/macro.py
--rw-rw-rw-   0        0        0    10439 2024-04-28 03:18:50.000000 data_watchtower-0.0.2/data_watchtower/core/validators.py
--rw-rw-rw-   0        0        0     5861 2024-05-03 12:39:06.000000 data_watchtower-0.0.2/data_watchtower/core/watchtower.py
-drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.334605 data_watchtower-0.0.2/data_watchtower/model/
--rw-rw-rw-   0        0        0       48 2024-04-26 07:38:23.000000 data_watchtower-0.0.2/data_watchtower/model/__init__.py
--rw-rw-rw-   0        0        0     2528 2024-05-03 15:15:42.000000 data_watchtower-0.0.2/data_watchtower/model/models.py
--rw-rw-rw-   0        0        0     8448 2024-05-03 15:15:42.000000 data_watchtower-0.0.2/data_watchtower/model/services.py
--rw-rw-rw-   0        0        0     5473 2024-05-03 12:33:46.000000 data_watchtower-0.0.2/data_watchtower/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.346089 data_watchtower-0.0.2/data_watchtower.egg-info/
--rw-rw-rw-   0        0        0      511 2024-05-05 07:23:59.000000 data_watchtower-0.0.2/data_watchtower.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      806 2024-05-05 07:24:00.000000 data_watchtower-0.0.2/data_watchtower.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-05 07:24:00.000000 data_watchtower-0.0.2/data_watchtower.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-05-05 07:24:00.000000 data_watchtower-0.0.2/data_watchtower.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-05 07:24:00.000000 data_watchtower-0.0.2/data_watchtower.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-05 07:24:00.349167 data_watchtower-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      802 2024-05-05 07:22:28.000000 data_watchtower-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-05 07:24:00.342425 data_watchtower-0.0.2/tests/
--rw-rw-rw-   0        0        0     7055 2024-05-05 04:20:24.000000 data_watchtower-0.0.2/tests/test_validator.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.255872 data_watchtower-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2024-05-01 02:10:55.000000 data_watchtower-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      504 2024-05-06 08:22:17.254844 data_watchtower-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2435 2024-05-03 13:56:51.000000 data_watchtower-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.232454 data_watchtower-0.0.3/data_watchtower/
+-rw-rw-rw-   0        0        0      270 2024-05-05 08:41:55.000000 data_watchtower-0.0.3/data_watchtower/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.240245 data_watchtower-0.0.3/data_watchtower/api/
+-rw-rw-rw-   0        0        0       48 2024-05-03 02:34:32.000000 data_watchtower-0.0.3/data_watchtower/api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.243364 data_watchtower-0.0.3/data_watchtower/api/handlers/
+-rw-rw-rw-   0        0        0       48 2024-05-03 03:21:05.000000 data_watchtower-0.0.3/data_watchtower/api/handlers/__init__.py
+-rw-rw-rw-   0        0        0      845 2024-05-05 04:43:17.000000 data_watchtower-0.0.3/data_watchtower/api/handlers/base.py
+-rw-rw-rw-   0        0        0      553 2024-05-03 12:39:06.000000 data_watchtower-0.0.3/data_watchtower/api/handlers/watchtower.py
+-rw-rw-rw-   0        0        0      835 2024-05-05 04:40:00.000000 data_watchtower-0.0.3/data_watchtower/api/server.py
+-rw-rw-rw-   0        0        0      291 2024-05-05 06:57:58.000000 data_watchtower-0.0.3/data_watchtower/api/url.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.248064 data_watchtower-0.0.3/data_watchtower/core/
+-rw-rw-rw-   0        0        0       48 2024-04-26 07:27:27.000000 data_watchtower-0.0.3/data_watchtower/core/__init__.py
+-rw-rw-rw-   0        0        0     2809 2024-05-05 04:36:42.000000 data_watchtower-0.0.3/data_watchtower/core/base.py
+-rw-rw-rw-   0        0        0     1138 2024-05-03 09:14:39.000000 data_watchtower-0.0.3/data_watchtower/core/data_loaders.py
+-rw-rw-rw-   0        0        0     1546 2024-05-03 04:45:13.000000 data_watchtower-0.0.3/data_watchtower/core/macro.py
+-rw-rw-rw-   0        0        0    10439 2024-04-28 03:18:50.000000 data_watchtower-0.0.3/data_watchtower/core/validators.py
+-rw-rw-rw-   0        0        0     5861 2024-05-03 12:39:06.000000 data_watchtower-0.0.3/data_watchtower/core/watchtower.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.251181 data_watchtower-0.0.3/data_watchtower/model/
+-rw-rw-rw-   0        0        0       48 2024-04-26 07:38:23.000000 data_watchtower-0.0.3/data_watchtower/model/__init__.py
+-rw-rw-rw-   0        0        0     2528 2024-05-03 15:15:42.000000 data_watchtower-0.0.3/data_watchtower/model/models.py
+-rw-rw-rw-   0        0        0     8448 2024-05-03 15:15:42.000000 data_watchtower-0.0.3/data_watchtower/model/services.py
+-rw-rw-rw-   0        0        0     5473 2024-05-03 12:33:46.000000 data_watchtower-0.0.3/data_watchtower/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.253258 data_watchtower-0.0.3/data_watchtower.egg-info/
+-rw-rw-rw-   0        0        0      504 2024-05-06 08:22:17.000000 data_watchtower-0.0.3/data_watchtower.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2024-05-06 08:22:17.000000 data_watchtower-0.0.3/data_watchtower.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-06 08:22:17.000000 data_watchtower-0.0.3/data_watchtower.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2024-05-06 08:22:17.000000 data_watchtower-0.0.3/data_watchtower.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-06 08:22:17.000000 data_watchtower-0.0.3/data_watchtower.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-06 08:22:17.255872 data_watchtower-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      795 2024-05-06 08:21:51.000000 data_watchtower-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-06 08:22:17.252218 data_watchtower-0.0.3/tests/
+-rw-rw-rw-   0        0        0     7055 2024-05-05 04:20:24.000000 data_watchtower-0.0.3/tests/test_validator.py
```

### Comparing `data_watchtower-0.0.2/LICENSE` & `data_watchtower-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/README.md` & `data_watchtower-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/api/handlers/base.py` & `data_watchtower-0.0.3/data_watchtower/api/handlers/base.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/api/handlers/watchtower.py` & `data_watchtower-0.0.3/data_watchtower/api/handlers/watchtower.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/api/server.py` & `data_watchtower-0.0.3/data_watchtower/api/server.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/core/base.py` & `data_watchtower-0.0.3/data_watchtower/core/base.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/core/data_loaders.py` & `data_watchtower-0.0.3/data_watchtower/core/data_loaders.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/core/macro.py` & `data_watchtower-0.0.3/data_watchtower/core/macro.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/core/validators.py` & `data_watchtower-0.0.3/data_watchtower/core/validators.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/core/watchtower.py` & `data_watchtower-0.0.3/data_watchtower/core/watchtower.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/model/models.py` & `data_watchtower-0.0.3/data_watchtower/model/models.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/model/services.py` & `data_watchtower-0.0.3/data_watchtower/model/services.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower/utils.py` & `data_watchtower-0.0.3/data_watchtower/utils.py`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/data_watchtower.egg-info/SOURCES.txt` & `data_watchtower-0.0.3/data_watchtower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_watchtower-0.0.2/setup.py` & `data_watchtower-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     #     "pytest==8.2.0",
     #     "faker",
     #     "PyMySQL==1.1.0",
     #     "psycopg2==2.9.9",
     # ],
     install_requires=[
         "attrs==23.2.0",
-        "peewee==3.17.0",
+        "peewee==3.17.3",
         "shortuuid==1.0.13",
         "tornado==6.4",
         "pandas==2.2.2",
         "polars==0.20.23",
-        "connectorx==0.3.2",
+        "connectorx",
     ],
 )
```

### Comparing `data_watchtower-0.0.2/tests/test_validator.py` & `data_watchtower-0.0.3/tests/test_validator.py`

 * *Files identical despite different names*

