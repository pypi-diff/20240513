# Comparing `tmp/ludfor-utils-0.1.6.tar.gz` & `tmp/ludfor-utils-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ludfor-utils-0.1.6.tar", last modified: Thu Mar 14 17:42:52 2024, max compression
+gzip compressed data, was "ludfor-utils-0.1.7.tar", last modified: Mon May 13 10:59:30 2024, max compression
```

## Comparing `ludfor-utils-0.1.6.tar` & `ludfor-utils-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 17:42:52.906383 ludfor-utils-0.1.6/
--rw-rw-rw-   0        0        0      165 2024-03-14 17:42:52.904381 ludfor-utils-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0       66 2024-03-14 11:55:33.000000 ludfor-utils-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 17:42:52.902380 ludfor-utils-0.1.6/ludfor_utils.egg-info/
--rw-rw-rw-   0        0        0      165 2024-03-14 17:42:52.000000 ludfor-utils-0.1.6/ludfor_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-03-14 17:42:52.000000 ludfor-utils-0.1.6/ludfor_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 17:42:52.000000 ludfor-utils-0.1.6/ludfor_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-14 17:42:52.000000 ludfor-utils-0.1.6/ludfor_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-14 17:42:52.000000 ludfor-utils-0.1.6/ludfor_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-14 17:42:52.900380 ludfor-utils-0.1.6/ludforlib/
--rw-rw-rw-   0        0        0        0 2024-03-14 13:09:25.000000 ludfor-utils-0.1.6/ludforlib/__init__.py
--rw-rw-rw-   0        0        0     2743 2024-03-14 17:17:16.000000 ludfor-utils-0.1.6/ludforlib/database.py
--rw-rw-rw-   0        0        0     2022 2024-03-14 17:08:14.000000 ludfor-utils-0.1.6/ludforlib/email.py
--rw-rw-rw-   0        0        0      602 2024-03-14 17:18:03.000000 ludfor-utils-0.1.6/ludforlib/logger.py
--rw-rw-rw-   0        0        0       42 2024-03-14 17:42:52.908382 ludfor-utils-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      288 2024-03-14 17:42:30.000000 ludfor-utils-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:59:30.878310 ludfor-utils-0.1.7/
+-rw-rw-rw-   0        0        0      140 2024-05-13 10:59:30.878310 ludfor-utils-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0       66 2024-03-14 11:55:33.000000 ludfor-utils-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 10:59:30.864308 ludfor-utils-0.1.7/ludfor-lib/
+-rw-rw-rw-   0        0        0        0 2024-03-14 13:09:25.000000 ludfor-utils-0.1.7/ludfor-lib/__init__.py
+-rw-rw-rw-   0        0        0     2743 2024-03-14 17:17:16.000000 ludfor-utils-0.1.7/ludfor-lib/database.py
+-rw-rw-rw-   0        0        0     2022 2024-03-14 17:08:14.000000 ludfor-utils-0.1.7/ludfor-lib/email.py
+-rw-rw-rw-   0        0        0      622 2024-05-13 10:43:16.000000 ludfor-utils-0.1.7/ludfor-lib/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-13 10:59:30.876311 ludfor-utils-0.1.7/ludfor_utils.egg-info/
+-rw-rw-rw-   0        0        0      140 2024-05-13 10:59:30.000000 ludfor-utils-0.1.7/ludfor_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-13 10:59:30.000000 ludfor-utils-0.1.7/ludfor_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 10:59:30.000000 ludfor-utils-0.1.7/ludfor_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-13 10:59:30.000000 ludfor-utils-0.1.7/ludfor_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-13 10:59:30.000000 ludfor-utils-0.1.7/ludfor_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 10:59:30.879310 ludfor-utils-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      288 2024-05-13 10:59:22.000000 ludfor-utils-0.1.7/setup.py
```

### Comparing `ludfor-utils-0.1.6/ludforlib/database.py` & `ludfor-utils-0.1.7/ludfor-lib/database.py`

 * *Files identical despite different names*

### Comparing `ludfor-utils-0.1.6/ludforlib/email.py` & `ludfor-utils-0.1.7/ludfor-lib/email.py`

 * *Files identical despite different names*

### Comparing `ludfor-utils-0.1.6/ludforlib/logger.py` & `ludfor-utils-0.1.7/ludfor-lib/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 def logger(log_path: str, logging_level: str, log_entry: str):
     """
     Função para logar informações em um arquivo. Formatação [datetime | logging_level] logging_entry
     log_path = Caminho de arquivo .log/.txt.
     logging_level = Níveis usados geralmente INFO, DEBUG, WARNING, ERROR, FATAL/SEVERE.
     logging_entry = Mensagem a ser adicionada.
     """
-    with open(log_path, 'a') as log:
+    with open(log_path, 'a', encoding = 'utf-8') as log:
         message = f"[{datetime.now()} | {logging_level.upper()}] {log_entry}\n"
         log.write(message)
```

