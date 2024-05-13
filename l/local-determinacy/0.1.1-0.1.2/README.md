# Comparing `tmp/local_determinacy-0.1.1.tar.gz` & `tmp/local_determinacy-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_determinacy-0.1.1.tar", last modified: Mon May 13 08:01:44 2024, max compression
+gzip compressed data, was "local_determinacy-0.1.2.tar", last modified: Mon May 13 08:04:44 2024, max compression
```

## Comparing `local_determinacy-0.1.1.tar` & `local_determinacy-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:01:44.029618 local_determinacy-0.1.1/
--rw-r--r--   0 alfredlov   (502) staff       (20)     1092 2024-05-06 07:04:05.000000 local_determinacy-0.1.1/LICENSE
--rw-r--r--   0 alfredlov   (502) staff       (20)     5902 2024-05-13 08:01:44.029189 local_determinacy-0.1.1/PKG-INFO
--rw-r--r--   0 alfredlov   (502) staff       (20)     5269 2024-05-13 07:59:53.000000 local_determinacy-0.1.1/README.md
--rw-r--r--   0 alfredlov   (502) staff       (20)      856 2024-05-13 08:01:36.000000 local_determinacy-0.1.1/pyproject.toml
--rw-r--r--   0 alfredlov   (502) staff       (20)       38 2024-05-13 08:01:44.029687 local_determinacy-0.1.1/setup.cfg
-drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:01:44.024501 local_determinacy-0.1.1/src/
-drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:01:44.026271 local_determinacy-0.1.1/src/local_determinacy/
--rw-r--r--   0 alfredlov   (502) staff       (20)       24 2024-05-10 13:00:49.000000 local_determinacy-0.1.1/src/local_determinacy/__init__.py
--rw-r--r--   0 alfredlov   (502) staff       (20)     4746 2024-05-07 12:17:33.000000 local_determinacy-0.1.1/src/local_determinacy/functions.py
-drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:01:44.028884 local_determinacy-0.1.1/src/local_determinacy.egg-info/
--rw-r--r--   0 alfredlov   (502) staff       (20)     5902 2024-05-13 08:01:44.000000 local_determinacy-0.1.1/src/local_determinacy.egg-info/PKG-INFO
--rw-r--r--   0 alfredlov   (502) staff       (20)      281 2024-05-13 08:01:44.000000 local_determinacy-0.1.1/src/local_determinacy.egg-info/SOURCES.txt
--rw-r--r--   0 alfredlov   (502) staff       (20)        1 2024-05-13 08:01:44.000000 local_determinacy-0.1.1/src/local_determinacy.egg-info/dependency_links.txt
--rw-r--r--   0 alfredlov   (502) staff       (20)       18 2024-05-13 08:01:44.000000 local_determinacy-0.1.1/src/local_determinacy.egg-info/top_level.txt
+drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:04:44.516808 local_determinacy-0.1.2/
+-rw-r--r--   0 alfredlov   (502) staff       (20)     1092 2024-05-06 07:04:05.000000 local_determinacy-0.1.2/LICENSE
+-rw-r--r--   0 alfredlov   (502) staff       (20)     5902 2024-05-13 08:04:44.516428 local_determinacy-0.1.2/PKG-INFO
+-rw-r--r--   0 alfredlov   (502) staff       (20)     5269 2024-05-13 07:59:53.000000 local_determinacy-0.1.2/README.md
+-rw-r--r--   0 alfredlov   (502) staff       (20)      856 2024-05-13 08:04:30.000000 local_determinacy-0.1.2/pyproject.toml
+-rw-r--r--   0 alfredlov   (502) staff       (20)       38 2024-05-13 08:04:44.516875 local_determinacy-0.1.2/setup.cfg
+drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:04:44.511890 local_determinacy-0.1.2/src/
+drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:04:44.513530 local_determinacy-0.1.2/src/local_determinacy/
+-rw-r--r--   0 alfredlov   (502) staff       (20)       24 2024-05-10 13:00:49.000000 local_determinacy-0.1.2/src/local_determinacy/__init__.py
+-rw-r--r--   0 alfredlov   (502) staff       (20)     4747 2024-05-13 08:04:24.000000 local_determinacy-0.1.2/src/local_determinacy/functions.py
+drwxr-xr-x   0 alfredlov   (502) staff       (20)        0 2024-05-13 08:04:44.516084 local_determinacy-0.1.2/src/local_determinacy.egg-info/
+-rw-r--r--   0 alfredlov   (502) staff       (20)     5902 2024-05-13 08:04:44.000000 local_determinacy-0.1.2/src/local_determinacy.egg-info/PKG-INFO
+-rw-r--r--   0 alfredlov   (502) staff       (20)      281 2024-05-13 08:04:44.000000 local_determinacy-0.1.2/src/local_determinacy.egg-info/SOURCES.txt
+-rw-r--r--   0 alfredlov   (502) staff       (20)        1 2024-05-13 08:04:44.000000 local_determinacy-0.1.2/src/local_determinacy.egg-info/dependency_links.txt
+-rw-r--r--   0 alfredlov   (502) staff       (20)       18 2024-05-13 08:04:44.000000 local_determinacy-0.1.2/src/local_determinacy.egg-info/top_level.txt
```

### Comparing `local_determinacy-0.1.1/LICENSE` & `local_determinacy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `local_determinacy-0.1.1/PKG-INFO` & `local_determinacy-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local_determinacy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package for assessing local determinacy in incomplete markets models.
 Author-email: Alfred Løvgren <alfred.lovgren@econ.uio.no>, Marcus Hagedorn <marcus.hagedorn@econ.uio.no>
 Project-URL: Homepage, https://github.com/alfredlov/local-determinacy/
 Project-URL: Issues, https://github.com/alfredlov/local-determinacy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `local_determinacy-0.1.1/README.md` & `local_determinacy-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `local_determinacy-0.1.1/pyproject.toml` & `local_determinacy-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "matplotlib>=1.16.0"
 ]
 
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "local_determinacy"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Alfred Løvgren", email="alfred.lovgren@econ.uio.no" },
   { name="Marcus Hagedorn", email="marcus.hagedorn@econ.uio.no" },
 ]
 description = "A python package for assessing local determinacy in incomplete markets models."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `local_determinacy-0.1.1/src/local_determinacy/functions.py` & `local_determinacy-0.1.2/src/local_determinacy/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     if F == 0:
         return(winding_out + "\nThe economy is DETERMINATE")
     
     elif F > 0:
         return(winding_out + "\nThe economy is INDETERMINATE (NO SOLUTION)")    
     
     elif F < 0:
-        return(winding_out + "\nThe economy is INDETERMINATE (MULTIPLE SOLUTION)") 
+        return(winding_out + "\nThe economy is INDETERMINATE (MULTIPLE SOLUTIONS)") 
 
 def plot(F):
     plt.plot(F.real, F.imag, color='blue',linewidth=3)
 
     plt.xlabel('Real - axis', fontsize=18)
 
     plt.ylabel('Imaginary - axis', fontsize=18)
```

### Comparing `local_determinacy-0.1.1/src/local_determinacy.egg-info/PKG-INFO` & `local_determinacy-0.1.2/src/local_determinacy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: local_determinacy
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python package for assessing local determinacy in incomplete markets models.
 Author-email: Alfred Løvgren <alfred.lovgren@econ.uio.no>, Marcus Hagedorn <marcus.hagedorn@econ.uio.no>
 Project-URL: Homepage, https://github.com/alfredlov/local-determinacy/
 Project-URL: Issues, https://github.com/alfredlov/local-determinacy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

