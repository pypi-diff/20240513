# Comparing `tmp/basharmor-3.0.0.tar.gz` & `tmp/basharmor-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "basharmor-3.0.0.tar", last modified: Tue Mar 19 22:17:54 2024, max compression
+gzip compressed data, was "basharmor-3.1.0.tar", last modified: Sun May 12 18:02:47 2024, max compression
```

## Comparing `basharmor-3.0.0.tar` & `basharmor-3.1.0.tar`

### file list

```diff
@@ -1,9 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:17:54.211326 basharmor-3.0.0/
--rw-r--r--   0 root         (0) root         (0)      687 2024-03-19 22:17:54.211326 basharmor-3.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 22:17:54.211326 basharmor-3.0.0/basharmor.egg-info/
--rw-r--r--   0 root         (0) root         (0)      687 2024-03-19 22:17:54.000000 basharmor-3.0.0/basharmor.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      140 2024-03-19 22:17:54.000000 basharmor-3.0.0/basharmor.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 22:17:54.000000 basharmor-3.0.0/basharmor.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 22:17:54.000000 basharmor-3.0.0/basharmor.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-19 22:17:54.211326 basharmor-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1232 2024-03-19 22:11:27.000000 basharmor-3.0.0/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2024-05-12 18:02:47.239838 basharmor-3.1.0/
+-rw-rw----   0 root         (0) everybody  (9997)      501 2024-05-12 18:02:47.215838 basharmor-3.1.0/PKG-INFO
+drwxrwx---   0 root         (0) everybody  (9997)        0 2024-05-12 18:02:46.943838 basharmor-3.1.0/basharmor/
+-rw-rw----   0 root         (0) everybody  (9997)     1806 2024-03-19 20:33:36.000000 basharmor-3.1.0/basharmor/.load
+-rw-rw----   0 root         (0) everybody  (9997)      392 2024-03-22 19:45:44.000000 basharmor-3.1.0/basharmor/__init__.py
+-rw-rw----   0 root         (0) everybody  (9997)     2055 2024-03-22 13:00:16.000000 basharmor-3.1.0/basharmor/basharmor.py
+-rw-rw----   0 root         (0) everybody  (9997)      790 2024-03-22 12:22:10.000000 basharmor-3.1.0/basharmor/obsf.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2024-05-12 18:02:47.199838 basharmor-3.1.0/basharmor.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)      501 2024-05-12 18:02:46.000000 basharmor-3.1.0/basharmor.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      287 2024-05-12 18:02:46.000000 basharmor-3.1.0/basharmor.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2024-05-12 18:02:46.000000 basharmor-3.1.0/basharmor.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       52 2024-05-12 18:02:46.000000 basharmor-3.1.0/basharmor.egg-info/entry_points.txt
+-rw-rw----   0 root         (0) everybody  (9997)       21 2024-05-12 18:02:46.000000 basharmor-3.1.0/basharmor.egg-info/requires.txt
+-rw-rw----   0 root         (0) everybody  (9997)       10 2024-05-12 18:02:46.000000 basharmor-3.1.0/basharmor.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2024-05-12 18:02:47.239838 basharmor-3.1.0/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)      923 2024-05-12 18:00:33.000000 basharmor-3.1.0/setup.py
```

