# Comparing `tmp/annonition-0.0.2.tar.gz` & `tmp/annonition-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annonition-0.0.2.tar", last modified: Wed May  8 00:00:20 2024, max compression
+gzip compressed data, was "annonition-0.0.3.tar", last modified: Sun May 12 22:41:56 2024, max compression
```

## Comparing `annonition-0.0.2.tar` & `annonition-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 00:00:20.370000 annonition-0.0.2/
--rw-rw-rw-   0        0        0      396 2024-05-08 00:00:22.000000 annonition-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       32 2024-05-07 21:46:06.000000 annonition-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-08 00:00:20.380000 annonition-0.0.2/annonition/
--rw-rw-rw-   0        0        0       27 2024-05-07 23:59:42.000000 annonition-0.0.2/annonition/__init__.py
--rw-rw-rw-   0        0        0       88 2024-05-07 21:23:14.000000 annonition-0.0.2/annonition/main.py
-drwxrwxrwx   0        0        0        0 2024-05-08 00:00:20.400000 annonition-0.0.2/annonition.egg-info/
--rw-rw-rw-   0        0        0      396 2024-05-08 00:00:22.000000 annonition-0.0.2/annonition.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-05-08 00:00:22.000000 annonition-0.0.2/annonition.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 00:00:22.000000 annonition-0.0.2/annonition.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-08 00:00:22.000000 annonition-0.0.2/annonition.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-08 00:00:22.000000 annonition-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      790 2024-05-08 00:00:10.000000 annonition-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:41:54.410000 annonition-0.0.3/
+-rw-rw-rw-   0        0        0      452 2024-05-12 22:41:58.000000 annonition-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       32 2024-05-07 21:46:06.000000 annonition-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 22:41:54.820000 annonition-0.0.3/annonition/
+-rw-rw-rw-   0        0        0       77 2024-05-12 22:40:06.000000 annonition-0.0.3/annonition/__init__.py
+-rw-rw-rw-   0        0        0     2524 2024-05-12 22:39:52.000000 annonition-0.0.3/annonition/logger.py
+-rw-rw-rw-   0        0        0       88 2024-05-07 21:23:14.000000 annonition-0.0.3/annonition/main.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:41:55.270000 annonition-0.0.3/annonition.egg-info/
+-rw-rw-rw-   0        0        0      452 2024-05-12 22:41:54.000000 annonition-0.0.3/annonition.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      250 2024-05-12 22:41:56.000000 annonition-0.0.3/annonition.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 22:41:56.000000 annonition-0.0.3/annonition.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-12 22:41:56.000000 annonition-0.0.3/annonition.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-12 22:41:56.000000 annonition-0.0.3/annonition.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 22:41:58.000000 annonition-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      843 2024-05-12 22:41:44.000000 annonition-0.0.3/setup.py
```

### Comparing `annonition-0.0.2/setup.py` & `annonition-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 
 with open(path.join(working_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="annonition",
-    version="0.0.2",
+    version="0.0.3",
     author="Abtin Turing",
     author_email="abtinturing@gmail.com",
     description="Beginning of a new era in annotation tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     # url="https://github.com/abtinturing/anno",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    install_requires=[]
+    install_requires=[
+        "coloredlogs",
+        "verboselogs"
+    ]
 )
```

