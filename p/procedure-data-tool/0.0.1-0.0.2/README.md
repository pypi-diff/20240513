# Comparing `tmp/procedure_data_tool-0.0.1.tar.gz` & `tmp/procedure_data_tool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procedure_data_tool-0.0.1.tar", last modified: Mon May 13 16:45:41 2024, max compression
+gzip compressed data, was "procedure_data_tool-0.0.2.tar", last modified: Mon May 13 18:07:00 2024, max compression
```

## Comparing `procedure_data_tool-0.0.1.tar` & `procedure_data_tool-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 16:45:41.966766 procedure_data_tool-0.0.1/
--rw-rw-rw-   0        0        0        0 2024-05-09 22:58:17.000000 procedure_data_tool-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      310 2024-05-13 16:45:41.964609 procedure_data_tool-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-09 23:00:28.000000 procedure_data_tool-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 16:45:41.949783 procedure_data_tool-0.0.1/procedure_data_tool/
--rw-rw-rw-   0        0        0        0 2024-05-09 23:00:15.000000 procedure_data_tool-0.0.1/procedure_data_tool/__init__.py
--rw-rw-rw-   0        0        0     2650 2024-05-08 20:03:38.000000 procedure_data_tool-0.0.1/procedure_data_tool/excelData.py
--rw-rw-rw-   0        0        0     5015 2024-05-13 15:53:37.000000 procedure_data_tool-0.0.1/procedure_data_tool/main.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:45:41.963609 procedure_data_tool-0.0.1/procedure_data_tool.egg-info/
--rw-rw-rw-   0        0        0      310 2024-05-13 16:45:41.000000 procedure_data_tool-0.0.1/procedure_data_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-05-13 16:45:41.000000 procedure_data_tool-0.0.1/procedure_data_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 16:45:41.000000 procedure_data_tool-0.0.1/procedure_data_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2024-05-13 16:45:41.000000 procedure_data_tool-0.0.1/procedure_data_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-13 16:45:41.000000 procedure_data_tool-0.0.1/procedure_data_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 16:45:41.966766 procedure_data_tool-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      783 2024-05-13 16:45:34.000000 procedure_data_tool-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:07:00.409216 procedure_data_tool-0.0.2/
+-rw-rw-rw-   0        0        0        0 2024-05-09 22:58:17.000000 procedure_data_tool-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      335 2024-05-13 18:07:00.408216 procedure_data_tool-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-09 23:00:28.000000 procedure_data_tool-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 18:07:00.389107 procedure_data_tool-0.0.2/procedure_data_tool/
+-rw-rw-rw-   0        0        0        0 2024-05-09 23:00:15.000000 procedure_data_tool-0.0.2/procedure_data_tool/__init__.py
+-rw-rw-rw-   0        0        0     2650 2024-05-08 20:03:38.000000 procedure_data_tool-0.0.2/procedure_data_tool/excelData.py
+-rw-rw-rw-   0        0        0     5015 2024-05-13 15:53:37.000000 procedure_data_tool-0.0.2/procedure_data_tool/main.py
+drwxrwxrwx   0        0        0        0 2024-05-13 18:07:00.407217 procedure_data_tool-0.0.2/procedure_data_tool.egg-info/
+-rw-rw-rw-   0        0        0      335 2024-05-13 18:07:00.000000 procedure_data_tool-0.0.2/procedure_data_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2024-05-13 18:07:00.000000 procedure_data_tool-0.0.2/procedure_data_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 18:07:00.000000 procedure_data_tool-0.0.2/procedure_data_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-13 18:07:00.000000 procedure_data_tool-0.0.2/procedure_data_tool.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2024-05-13 18:07:00.000000 procedure_data_tool-0.0.2/procedure_data_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-13 18:07:00.000000 procedure_data_tool-0.0.2/procedure_data_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      131 2024-05-13 18:07:00.411217 procedure_data_tool-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      781 2024-05-13 17:59:29.000000 procedure_data_tool-0.0.2/setup.py
```

### Comparing `procedure_data_tool-0.0.1/procedure_data_tool/excelData.py` & `procedure_data_tool-0.0.2/procedure_data_tool/excelData.py`

 * *Files identical despite different names*

### Comparing `procedure_data_tool-0.0.1/procedure_data_tool/main.py` & `procedure_data_tool-0.0.2/procedure_data_tool/main.py`

 * *Files identical despite different names*

### Comparing `procedure_data_tool-0.0.1/setup.py` & `procedure_data_tool-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="procedure_data_tool",
-    version="0.0.1",
+    version="0.0.2",
     description="add description XXXX____XXXX____XX___XX_",
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author="Josue Estrada",
     author_email="jramiroem@gmail.com",
     license="MIT",
@@ -14,14 +14,14 @@
     install_requires=[
         'openpyxl',
         'python-docx',
     ],
     # extras_require={
     #     # "dev": [pytest>=7.0]
     # }
-    # python_requires=">=3.60",
+    python_requires=">=3.60",
     # classifiers=[
     #     'Programming Language :: Python :: 3',
     #     'License :: OSI Approved :: MIT License',
     #     'Operating System :: OS Independent',
     # ],
 )
```

