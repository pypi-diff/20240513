# Comparing `tmp/dalgorithms-0.0.1.tar.gz` & `tmp/dalgorithms-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalgorithms-0.0.1.tar", last modified: Mon May 13 14:36:29 2024, max compression
+gzip compressed data, was "dalgorithms-0.0.2.tar", last modified: Mon May 13 15:58:59 2024, max compression
```

## Comparing `dalgorithms-0.0.1.tar` & `dalgorithms-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 14:36:29.990479 dalgorithms-0.0.1/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      687 2024-05-13 14:36:29.990479 dalgorithms-0.0.1/PKG-INFO
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       22 2024-05-06 18:11:07.000000 dalgorithms-0.0.1/README.md
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 14:36:29.989478 dalgorithms-0.0.1/compress_algorithms/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       68 2024-05-13 14:32:58.000000 dalgorithms-0.0.1/compress_algorithms/__init__.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     6976 2024-05-13 13:56:21.000000 dalgorithms-0.0.1/compress_algorithms/algorithms.py
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)     5426 2024-05-13 11:00:25.000000 dalgorithms-0.0.1/compress_algorithms/app.py
-drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 14:36:29.990479 dalgorithms-0.0.1/dalgorithms.egg-info/
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      687 2024-05-13 14:36:29.000000 dalgorithms-0.0.1/dalgorithms.egg-info/PKG-INFO
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      285 2024-05-13 14:36:29.000000 dalgorithms-0.0.1/dalgorithms.egg-info/SOURCES.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-13 14:36:29.000000 dalgorithms-0.0.1/dalgorithms.egg-info/dependency_links.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       10 2024-05-13 14:36:29.000000 dalgorithms-0.0.1/dalgorithms.egg-info/requires.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       20 2024-05-13 14:36:29.000000 dalgorithms-0.0.1/dalgorithms.egg-info/top_level.txt
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)       38 2024-05-13 14:36:29.990479 dalgorithms-0.0.1/setup.cfg
--rw-r--r--   0 gllekk    (1000) gllekk    (1000)      993 2024-05-13 14:32:32.000000 dalgorithms-0.0.1/setup.py
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 15:58:59.294489 dalgorithms-0.0.2/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      687 2024-05-13 15:58:59.293489 dalgorithms-0.0.2/PKG-INFO
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       22 2024-05-06 18:11:07.000000 dalgorithms-0.0.2/README.md
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 15:58:59.292489 dalgorithms-0.0.2/compress_algorithms/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       58 2024-05-13 15:26:25.000000 dalgorithms-0.0.2/compress_algorithms/__init__.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     5438 2024-05-13 15:23:58.000000 dalgorithms-0.0.2/compress_algorithms/app.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     5247 2024-05-13 15:25:53.000000 dalgorithms-0.0.2/compress_algorithms/huffman.py
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)     2204 2024-05-13 15:24:26.000000 dalgorithms-0.0.2/compress_algorithms/lzw.py
+drwxr-xr-x   0 gllekk    (1000) gllekk    (1000)        0 2024-05-13 15:58:59.293489 dalgorithms-0.0.2/dalgorithms.egg-info/
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      687 2024-05-13 15:58:59.000000 dalgorithms-0.0.2/dalgorithms.egg-info/PKG-INFO
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      309 2024-05-13 15:58:59.000000 dalgorithms-0.0.2/dalgorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)        1 2024-05-13 15:58:59.000000 dalgorithms-0.0.2/dalgorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       10 2024-05-13 15:58:59.000000 dalgorithms-0.0.2/dalgorithms.egg-info/requires.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       20 2024-05-13 15:58:59.000000 dalgorithms-0.0.2/dalgorithms.egg-info/top_level.txt
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)       38 2024-05-13 15:58:59.294489 dalgorithms-0.0.2/setup.cfg
+-rw-r--r--   0 gllekk    (1000) gllekk    (1000)      969 2024-05-13 15:27:29.000000 dalgorithms-0.0.2/setup.py
```

### Comparing `dalgorithms-0.0.1/PKG-INFO` & `dalgorithms-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalgorithms
-Version: 0.0.1
+Version: 0.0.2
 Summary: Compress algorithms
 Author: UCUgllekk
 Author-email: pavlosiuk.pn@ucu.edu.ua
 Keywords: python,compress,compression,algorithm,lz78,lzw,huffman,deflate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dalgorithms-0.0.1/compress_algorithms/app.py` & `dalgorithms-0.0.2/compress_algorithms/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 '''App for compression'''
 import tkinter as tk
 from tkinter import filedialog
 from threading import Thread
-from algorithms import HuffmanCompression, LZW
+from huffman import HuffmanCompression
+from lzw import LZW
 import os
 
 class CompressionProgramGUI:
     '''Compression app'''
     def __init__(self):
         self.root = tk.Tk()
         self.root.title("Compression App")
```

### Comparing `dalgorithms-0.0.1/dalgorithms.egg-info/PKG-INFO` & `dalgorithms-0.0.2/dalgorithms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalgorithms
-Version: 0.0.1
+Version: 0.0.2
 Summary: Compress algorithms
 Author: UCUgllekk
 Author-email: pavlosiuk.pn@ucu.edu.ua
 Keywords: python,compress,compression,algorithm,lz78,lzw,huffman,deflate
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dalgorithms-0.0.1/setup.py` & `dalgorithms-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from setuptools import setup, find_packages
-import codecs
-import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Compress algorithms'
 LONG_DESCRIPTION = 'A package that allows to compress different types of data using different algorithms such as LZW, LZ78, Deflate, Huffman'
 
 setup(
     name="dalgorithms",
     version=VERSION,
     author="UCUgllekk",
```

