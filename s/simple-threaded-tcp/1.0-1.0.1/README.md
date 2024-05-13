# Comparing `tmp/simple_threaded_tcp-1.0.tar.gz` & `tmp/simple_threaded_tcp-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_threaded_tcp-1.0.tar", last modified: Mon May 13 14:07:15 2024, max compression
+gzip compressed data, was "simple_threaded_tcp-1.0.1.tar", last modified: Mon May 13 14:22:47 2024, max compression
```

## Comparing `simple_threaded_tcp-1.0.tar` & `simple_threaded_tcp-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 14:07:15.433582 simple_threaded_tcp-1.0/
--rw-rw-rw-   0        0        0      402 2024-05-13 14:07:15.430585 simple_threaded_tcp-1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-13 14:02:45.000000 simple_threaded_tcp-1.0/README.md
--rw-rw-rw-   0        0        0      612 2024-05-13 14:07:04.000000 simple_threaded_tcp-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 14:07:15.433582 simple_threaded_tcp-1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-13 14:07:15.347644 simple_threaded_tcp-1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 14:07:15.428586 simple_threaded_tcp-1.0/src/simple_threaded_tcp.egg-info/
--rw-rw-rw-   0        0        0      402 2024-05-13 14:07:15.000000 simple_threaded_tcp-1.0/src/simple_threaded_tcp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-13 14:07:15.000000 simple_threaded_tcp-1.0/src/simple_threaded_tcp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 14:07:15.000000 simple_threaded_tcp-1.0/src/simple_threaded_tcp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-13 14:07:15.000000 simple_threaded_tcp-1.0/src/simple_threaded_tcp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-13 14:07:15.425589 simple_threaded_tcp-1.0/src/sttcp/
--rw-rw-rw-   0        0        0        0 2024-05-13 09:33:43.000000 simple_threaded_tcp-1.0/src/sttcp/__init__.py
--rw-rw-rw-   0        0        0     1553 2024-05-13 09:56:29.000000 simple_threaded_tcp-1.0/src/sttcp/client.py
--rw-rw-rw-   0        0        0     2946 2024-05-13 09:56:28.000000 simple_threaded_tcp-1.0/src/sttcp/server.py
+drwxrwxrwx   0        0        0        0 2024-05-13 14:22:47.575780 simple_threaded_tcp-1.0.1/
+-rw-rw-rw-   0        0        0     1408 2024-05-13 14:22:47.573781 simple_threaded_tcp-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1046 2024-05-13 14:19:06.000000 simple_threaded_tcp-1.0.1/README.md
+-rw-rw-rw-   0        0        0      614 2024-05-13 14:22:12.000000 simple_threaded_tcp-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-13 14:22:47.576778 simple_threaded_tcp-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 14:22:47.530811 simple_threaded_tcp-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 14:22:47.571782 simple_threaded_tcp-1.0.1/src/simple_threaded_tcp.egg-info/
+-rw-rw-rw-   0        0        0     1408 2024-05-13 14:22:47.000000 simple_threaded_tcp-1.0.1/src/simple_threaded_tcp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-13 14:22:47.000000 simple_threaded_tcp-1.0.1/src/simple_threaded_tcp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 14:22:47.000000 simple_threaded_tcp-1.0.1/src/simple_threaded_tcp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 14:22:47.000000 simple_threaded_tcp-1.0.1/src/simple_threaded_tcp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 14:22:47.568784 simple_threaded_tcp-1.0.1/src/sttcp/
+-rw-rw-rw-   0        0        0        0 2024-05-13 09:33:43.000000 simple_threaded_tcp-1.0.1/src/sttcp/__init__.py
+-rw-rw-rw-   0        0        0     1553 2024-05-13 09:56:29.000000 simple_threaded_tcp-1.0.1/src/sttcp/client.py
+-rw-rw-rw-   0        0        0     2946 2024-05-13 09:56:28.000000 simple_threaded_tcp-1.0.1/src/sttcp/server.py
```

### Comparing `simple_threaded_tcp-1.0/pyproject.toml` & `simple_threaded_tcp-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "simple_threaded_tcp"
-version = "1.0"
+version = "1.0.1"
 authors = [
     {name = "Emil", email = "emilahmaboy@gmail.com"}
 ]
 description = "Client-Server threaded TCP connector. This project also uses socket library."
 readme = "README.md"
 requires-python = ">3.8"
 classifiers = [
```

### Comparing `simple_threaded_tcp-1.0/src/sttcp/client.py` & `simple_threaded_tcp-1.0.1/src/sttcp/client.py`

 * *Files identical despite different names*

### Comparing `simple_threaded_tcp-1.0/src/sttcp/server.py` & `simple_threaded_tcp-1.0.1/src/sttcp/server.py`

 * *Files identical despite different names*

