# Comparing `tmp/st_forna_component-0.0.1.tar.gz` & `tmp/st_forna_component-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_forna_component-0.0.1.tar", last modified: Sun May 12 16:13:16 2024, max compression
+gzip compressed data, was "st_forna_component-0.0.2.tar", last modified: Sun May 12 16:33:43 2024, max compression
```

## Comparing `st_forna_component-0.0.1.tar` & `st_forna_component-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 lmonari    (503) staff       (20)        0 2024-05-12 16:13:16.552856 st_forna_component-0.0.1/
--rw-r--r--   0 lmonari    (503) staff       (20)     1068 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/LICENSE
--rw-r--r--   0 lmonari    (503) staff       (20)       38 2024-05-12 15:38:02.000000 st_forna_component-0.0.1/MANIFEST.in
--rw-r--r--   0 lmonari    (503) staff       (20)     2569 2024-05-12 16:13:16.552168 st_forna_component-0.0.1/PKG-INFO
--rw-r--r--   0 lmonari    (503) staff       (20)     1931 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/README.md
--rw-r--r--   0 lmonari    (503) staff       (20)       38 2024-05-12 16:13:16.552932 st_forna_component-0.0.1/setup.cfg
--rw-r--r--   0 lmonari    (503) staff       (20)      899 2024-05-12 16:06:06.000000 st_forna_component-0.0.1/setup.py
-drwxr-xr-x   0 lmonari    (503) staff       (20)        0 2024-05-12 16:13:16.547597 st_forna_component-0.0.1/st_forna_component/
--rw-r--r--   0 lmonari    (503) staff       (20)     6148 2024-05-12 15:31:45.000000 st_forna_component-0.0.1/st_forna_component/.DS_Store
--rw-r--r--   0 lmonari    (503) staff       (20)      394 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/st_forna_component/02188894d5236b1517df3210b79c2a7f.svg
--rw-r--r--   0 lmonari    (503) staff       (20)      205 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/st_forna_component/__init__.py
--rw-r--r--   0 lmonari    (503) staff       (20)      394 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/st_forna_component/fa9b45d63b40299e0188927ca7d381a3.svg
--rw-r--r--   0 lmonari    (503) staff       (20)     3721 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/st_forna_component/fornac.css
--rw-r--r--   0 lmonari    (503) staff       (20)     5793 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/st_forna_component/fornac.css.map
--rw-r--r--   0 lmonari    (503) staff       (20)   114968 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/st_forna_component/fornac.js
--rw-r--r--   0 lmonari    (503) staff       (20)      225 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/st_forna_component/fornac.js.LICENSE.txt
--rw-r--r--   0 lmonari    (503) staff       (20)   479303 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/st_forna_component/fornac.js.map
--rw-r--r--   0 lmonari    (503) staff       (20)     3802 2024-05-12 14:46:42.000000 st_forna_component-0.0.1/st_forna_component/index.html
-drwxr-xr-x   0 lmonari    (503) staff       (20)        0 2024-05-12 16:13:16.550367 st_forna_component-0.0.1/st_forna_component.egg-info/
--rw-r--r--   0 lmonari    (503) staff       (20)     2569 2024-05-12 16:13:16.000000 st_forna_component-0.0.1/st_forna_component.egg-info/PKG-INFO
--rw-r--r--   0 lmonari    (503) staff       (20)      616 2024-05-12 16:13:16.000000 st_forna_component-0.0.1/st_forna_component.egg-info/SOURCES.txt
--rw-r--r--   0 lmonari    (503) staff       (20)        1 2024-05-12 16:13:16.000000 st_forna_component-0.0.1/st_forna_component.egg-info/dependency_links.txt
--rw-r--r--   0 lmonari    (503) staff       (20)      140 2024-05-12 16:13:16.000000 st_forna_component-0.0.1/st_forna_component.egg-info/requires.txt
--rw-r--r--   0 lmonari    (503) staff       (20)       19 2024-05-12 16:13:16.000000 st_forna_component-0.0.1/st_forna_component.egg-info/top_level.txt
+drwxr-xr-x   0 lmonari    (503) staff       (20)        0 2024-05-12 16:33:43.734585 st_forna_component-0.0.2/
+-rw-r--r--   0 lmonari    (503) staff       (20)     1068 2024-05-12 14:46:42.000000 st_forna_component-0.0.2/LICENSE
+-rw-r--r--   0 lmonari    (503) staff       (20)       38 2024-05-12 15:38:02.000000 st_forna_component-0.0.2/MANIFEST.in
+-rw-r--r--   0 lmonari    (503) staff       (20)     2877 2024-05-12 16:33:43.734006 st_forna_component-0.0.2/PKG-INFO
+-rw-r--r--   0 lmonari    (503) staff       (20)     2239 2024-05-12 16:32:04.000000 st_forna_component-0.0.2/README.md
+-rw-r--r--   0 lmonari    (503) staff       (20)       38 2024-05-12 16:33:43.734658 st_forna_component-0.0.2/setup.cfg
+-rw-r--r--   0 lmonari    (503) staff       (20)      899 2024-05-12 16:33:21.000000 st_forna_component-0.0.2/setup.py
+drwxr-xr-x   0 lmonari    (503) staff       (20)        0 2024-05-12 16:33:43.730268 st_forna_component-0.0.2/st_forna_component/
+-rw-r--r--   0 lmonari    (503) staff       (20)     6148 2024-05-12 15:31:45.000000 st_forna_component-0.0.2/st_forna_component/.DS_Store
+-rw-r--r--   0 lmonari    (503) staff       (20)      394 2024-05-12 14:46:42.000000 st_forna_component-0.0.2/st_forna_component/02188894d5236b1517df3210b79c2a7f.svg
+-rw-r--r--   0 lmonari    (503) staff       (20)      205 2024-05-12 14:46:42.000000 st_forna_component-0.0.2/st_forna_component/__init__.py
+-rw-r--r--   0 lmonari    (503) staff       (20)      394 2024-05-12 14:46:42.000000 st_forna_component-0.0.2/st_forna_component/fa9b45d63b40299e0188927ca7d381a3.svg
+-rw-r--r--   0 lmonari    (503) staff       (20)     3721 2024-05-12 14:46:42.000000 st_forna_component-0.0.2/st_forna_component/fornac.css
+-rw-r--r--   0 lmonari    (503) staff       (20)     5793 2024-05-12 14:46:42.000000 st_forna_component-0.0.2/st_forna_component/fornac.css.map
+-rw-r--r--   0 lmonari    (503) staff       (20)   114968 2024-05-12 14:46:42.000000 st_forna_component-0.0.2/st_forna_component/fornac.js
+-rw-r--r--   0 lmonari    (503) staff       (20)      225 2024-05-12 14:46:42.000000 st_forna_component-0.0.2/st_forna_component/fornac.js.LICENSE.txt
+-rw-r--r--   0 lmonari    (503) staff       (20)   479303 2024-05-12 14:46:42.000000 st_forna_component-0.0.2/st_forna_component/fornac.js.map
+-rw-r--r--   0 lmonari    (503) staff       (20)     3802 2024-05-12 14:46:42.000000 st_forna_component-0.0.2/st_forna_component/index.html
+drwxr-xr-x   0 lmonari    (503) staff       (20)        0 2024-05-12 16:33:43.732468 st_forna_component-0.0.2/st_forna_component.egg-info/
+-rw-r--r--   0 lmonari    (503) staff       (20)     2877 2024-05-12 16:33:43.000000 st_forna_component-0.0.2/st_forna_component.egg-info/PKG-INFO
+-rw-r--r--   0 lmonari    (503) staff       (20)      616 2024-05-12 16:33:43.000000 st_forna_component-0.0.2/st_forna_component.egg-info/SOURCES.txt
+-rw-r--r--   0 lmonari    (503) staff       (20)        1 2024-05-12 16:33:43.000000 st_forna_component-0.0.2/st_forna_component.egg-info/dependency_links.txt
+-rw-r--r--   0 lmonari    (503) staff       (20)      140 2024-05-12 16:33:43.000000 st_forna_component-0.0.2/st_forna_component.egg-info/requires.txt
+-rw-r--r--   0 lmonari    (503) staff       (20)       19 2024-05-12 16:33:43.000000 st_forna_component-0.0.2/st_forna_component.egg-info/top_level.txt
```

### Comparing `st_forna_component-0.0.1/LICENSE` & `st_forna_component-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `st_forna_component-0.0.1/PKG-INFO` & `st_forna_component-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_forna_component
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Streamlit component for the Forna RNA visualization tool
 Author: Luca Monari
 Author-email: Luca.Monari@mr.mpg.de
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: streamlit>=0.63
@@ -57,10 +57,20 @@
 st.write("Received value:", return_value) 
 # Returns None if no changes were made. 
 # When clicked on the component, it returns the current structure and sequence 
 # In case of cofold, it return a unique string without the separator '&'
 
 ```
 
+## How to cite:
+
+Please include this citation if the Forna Component is used in an academic study:
+
+```
+Lucandia. Lucandia/st_forna_component; Zenodo, 2024. https://zenodo.org/doi/10.5281/zenodo.11181680.
+```
+
+[![DOI](https://zenodo.org/badge/799569235.svg)](https://zenodo.org/doi/10.5281/zenodo.11181680)
+
```

### Comparing `st_forna_component-0.0.1/README.md` & `st_forna_component-0.0.2/st_forna_component.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: st_forna_component
+Version: 0.0.2
+Summary: A Streamlit component for the Forna RNA visualization tool
+Author: Luca Monari
+Author-email: Luca.Monari@mr.mpg.de
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: streamlit>=0.63
+Provides-Extra: devel
+Requires-Dist: wheel; extra == "devel"
+Requires-Dist: pytest==7.4.0; extra == "devel"
+Requires-Dist: playwright==1.39.0; extra == "devel"
+Requires-Dist: requests==2.31.0; extra == "devel"
+Requires-Dist: pytest-playwright-snapshot==1.0; extra == "devel"
+Requires-Dist: pytest-rerunfailures==12.0; extra == "devel"
+
 # Forna Component
 
 RNA Secondary Structure Visualization Using a Force Directed Graph Layout
 
 This is a simple component that renders a [forna diagram](https://github.com/ViennaRNA/fornac.git). It is a wrapper around the [forna container](https://github.com/ViennaRNA/fornac.git).
 
 ## Installation
@@ -39,10 +57,20 @@
 st.write("Received value:", return_value) 
 # Returns None if no changes were made. 
 # When clicked on the component, it returns the current structure and sequence 
 # In case of cofold, it return a unique string without the separator '&'
 
 ```
 
+## How to cite:
+
+Please include this citation if the Forna Component is used in an academic study:
+
+```
+Lucandia. Lucandia/st_forna_component; Zenodo, 2024. https://zenodo.org/doi/10.5281/zenodo.11181680.
+```
+
+[![DOI](https://zenodo.org/badge/799569235.svg)](https://zenodo.org/doi/10.5281/zenodo.11181680)
+
```

### Comparing `st_forna_component-0.0.1/setup.py` & `st_forna_component-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='st_forna_component',
-    version='0.0.1',
+    version='0.0.2',
     author='Luca Monari',
     author_email='Luca.Monari@mr.mpg.de',
     description='A Streamlit component for the Forna RNA visualization tool',
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     include_package_data=True,
```

### Comparing `st_forna_component-0.0.1/st_forna_component/.DS_Store` & `st_forna_component-0.0.2/st_forna_component/.DS_Store`

 * *Files identical despite different names*

### Comparing `st_forna_component-0.0.1/st_forna_component/fornac.css` & `st_forna_component-0.0.2/st_forna_component/fornac.css`

 * *Files identical despite different names*

### Comparing `st_forna_component-0.0.1/st_forna_component/fornac.css.map` & `st_forna_component-0.0.2/st_forna_component/fornac.css.map`

 * *Files identical despite different names*

### Comparing `st_forna_component-0.0.1/st_forna_component/fornac.js` & `st_forna_component-0.0.2/st_forna_component/fornac.js`

 * *Files identical despite different names*

### Comparing `st_forna_component-0.0.1/st_forna_component/fornac.js.map` & `st_forna_component-0.0.2/st_forna_component/fornac.js.map`

 * *Files identical despite different names*

### Comparing `st_forna_component-0.0.1/st_forna_component/index.html` & `st_forna_component-0.0.2/st_forna_component/index.html`

 * *Files identical despite different names*

### Comparing `st_forna_component-0.0.1/st_forna_component.egg-info/PKG-INFO` & `st_forna_component-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: st_forna_component
-Version: 0.0.1
-Summary: A Streamlit component for the Forna RNA visualization tool
-Author: Luca Monari
-Author-email: Luca.Monari@mr.mpg.de
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: streamlit>=0.63
-Provides-Extra: devel
-Requires-Dist: wheel; extra == "devel"
-Requires-Dist: pytest==7.4.0; extra == "devel"
-Requires-Dist: playwright==1.39.0; extra == "devel"
-Requires-Dist: requests==2.31.0; extra == "devel"
-Requires-Dist: pytest-playwright-snapshot==1.0; extra == "devel"
-Requires-Dist: pytest-rerunfailures==12.0; extra == "devel"
-
 # Forna Component
 
 RNA Secondary Structure Visualization Using a Force Directed Graph Layout
 
 This is a simple component that renders a [forna diagram](https://github.com/ViennaRNA/fornac.git). It is a wrapper around the [forna container](https://github.com/ViennaRNA/fornac.git).
 
 ## Installation
@@ -57,10 +39,20 @@
 st.write("Received value:", return_value) 
 # Returns None if no changes were made. 
 # When clicked on the component, it returns the current structure and sequence 
 # In case of cofold, it return a unique string without the separator '&'
 
 ```
 
+## How to cite:
+
+Please include this citation if the Forna Component is used in an academic study:
+
+```
+Lucandia. Lucandia/st_forna_component; Zenodo, 2024. https://zenodo.org/doi/10.5281/zenodo.11181680.
+```
+
+[![DOI](https://zenodo.org/badge/799569235.svg)](https://zenodo.org/doi/10.5281/zenodo.11181680)
+
```

### Comparing `st_forna_component-0.0.1/st_forna_component.egg-info/SOURCES.txt` & `st_forna_component-0.0.2/st_forna_component.egg-info/SOURCES.txt`

 * *Files identical despite different names*

