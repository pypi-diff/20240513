# Comparing `tmp/pih-msg_q-0.12.tar.gz` & `tmp/pih-msg_q-0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-msg_q-0.12.tar", last modified: Wed May  8 06:45:25 2024, max compression
+gzip compressed data, was "pih-msg_q-0.13.tar", last modified: Mon May 13 01:54:43 2024, max compression
```

## Comparing `pih-msg_q-0.12.tar` & `pih-msg_q-0.13.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 06:45:25.335511 pih-msg_q-0.12/
-drwxrwxrwx   0        0        0        0 2024-05-08 06:45:24.895866 pih-msg_q-0.12/MessageQueueService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-msg_q-0.12/MessageQueueService/__init__.py
--rw-rw-rw-   0        0        0      156 2024-02-15 00:45:45.000000 pih-msg_q-0.12/MessageQueueService/__main__.py
--rw-rw-rw-   0        0        0      441 2024-05-08 06:42:36.000000 pih-msg_q-0.12/MessageQueueService/const.py
--rw-rw-rw-   0        0        0     3701 2024-05-08 06:43:07.000000 pih-msg_q-0.12/MessageQueueService/service.py
--rw-rw-rw-   0        0        0      275 2024-05-08 06:45:25.304254 pih-msg_q-0.12/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-08 06:45:25.257383 pih-msg_q-0.12/pih_msg_q.egg-info/
--rw-rw-rw-   0        0        0      275 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-08 06:45:24.000000 pih-msg_q-0.12/pih_msg_q.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 06:45:25.335511 pih-msg_q-0.12/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-13 01:54:43.248555 pih-msg_q-0.13/
+drwxrwxrwx   0        0        0        0 2024-05-13 01:54:42.478758 pih-msg_q-0.13/MessageQueueService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-msg_q-0.13/MessageQueueService/__init__.py
+-rw-rw-rw-   0        0        0      156 2024-02-15 00:45:45.000000 pih-msg_q-0.13/MessageQueueService/__main__.py
+-rw-rw-rw-   0        0        0      441 2024-05-13 01:54:20.000000 pih-msg_q-0.13/MessageQueueService/const.py
+-rw-rw-rw-   0        0        0     3701 2024-05-08 06:43:07.000000 pih-msg_q-0.13/MessageQueueService/service.py
+-rw-rw-rw-   0        0        0      275 2024-05-13 01:54:43.217303 pih-msg_q-0.13/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-13 01:54:43.170426 pih-msg_q-0.13/pih_msg_q.egg-info/
+-rw-rw-rw-   0        0        0      275 2024-05-13 01:54:41.000000 pih-msg_q-0.13/pih_msg_q.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-13 01:54:42.000000 pih-msg_q-0.13/pih_msg_q.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 01:54:42.000000 pih-msg_q-0.13/pih_msg_q.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-13 01:54:42.000000 pih-msg_q-0.13/pih_msg_q.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-13 01:54:42.000000 pih-msg_q-0.13/pih_msg_q.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-13 01:54:42.000000 pih-msg_q-0.13/pih_msg_q.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 01:54:43.264181 pih-msg_q-0.13/setup.cfg
```

### Comparing `pih-msg_q-0.12/MessageQueueService/service.py` & `pih-msg_q-0.13/MessageQueueService/service.py`

 * *Files identical despite different names*

