# Comparing `tmp/pyprocessors-pseudonimizer-0.5.7.tar.gz` & `tmp/pyprocessors-pseudonimizer-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors-pseudonimizer-0.5.7.tar", last modified: Tue Feb  7 13:21:19 2023, max compression
+gzip compressed data, was "pyprocessors-pseudonimizer-0.5.9.tar", last modified: Tue Feb  7 13:23:38 2023, max compression
```

## Comparing `pyprocessors-pseudonimizer-0.5.7.tar` & `pyprocessors-pseudonimizer-0.5.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       97 2023-02-07 11:08:17.439110 pyprocessors-pseudonimizer-0.5.7/.dockerignore
--rw-r--r--   0        0        0      185 2023-02-07 13:11:52.474988 pyprocessors-pseudonimizer-0.5.7/.gitignore
--rw-r--r--   0        0        0      448 2023-02-07 11:08:17.443111 pyprocessors-pseudonimizer-0.5.7/Dockerfile
--rw-r--r--   0        0        0    10223 2023-02-07 11:23:03.170663 pyprocessors-pseudonimizer-0.5.7/Jenkinsfile
--rw-r--r--   0        0        0      380 2023-02-07 11:08:17.446111 pyprocessors-pseudonimizer-0.5.7/README.md
--rw-r--r--   0        0        0     1559 2023-02-07 11:08:17.447111 pyprocessors-pseudonimizer-0.5.7/bumpversion.py
--rw-r--r--   0        0        0       67 2023-02-07 13:21:18.633800 pyprocessors-pseudonimizer-0.5.7/pyprocessors_pseudonimizer/__init__.py
--rw-r--r--   0        0        0     2896 2023-02-07 11:08:17.448111 pyprocessors-pseudonimizer-0.5.7/pyprocessors_pseudonimizer/pseudonimizer.py
--rw-r--r--   0        0        0     2214 2023-02-07 11:23:03.170663 pyprocessors-pseudonimizer-0.5.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-07 11:08:17.449111 pyprocessors-pseudonimizer-0.5.7/tests/__init__.py
--rw-r--r--   0        0        0   119288 2023-02-07 13:21:15.650722 pyprocessors-pseudonimizer-0.5.7/tests/data/afp_ner_fr-document-test-anon.json
--rw-r--r--   0        0        0   104534 2023-02-07 11:08:17.451111 pyprocessors-pseudonimizer-0.5.7/tests/data/afp_ner_fr-document-test.json
--rw-r--r--   0        0        0      854 2023-02-07 11:08:17.451111 pyprocessors-pseudonimizer-0.5.7/tests/test_pseudonimizer.py
--rw-r--r--   0        0        0      943 2023-02-07 11:08:17.452111 pyprocessors-pseudonimizer-0.5.7/tox.ini
--rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 pyprocessors-pseudonimizer-0.5.7/setup.py
--rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 pyprocessors-pseudonimizer-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-02-07 11:08:17.439110 pyprocessors-pseudonimizer-0.5.9/.dockerignore
+-rw-r--r--   0        0        0      185 2023-02-07 13:11:52.474988 pyprocessors-pseudonimizer-0.5.9/.gitignore
+-rw-r--r--   0        0        0      448 2023-02-07 11:08:17.443111 pyprocessors-pseudonimizer-0.5.9/Dockerfile
+-rw-r--r--   0        0        0    10223 2023-02-07 11:23:03.170663 pyprocessors-pseudonimizer-0.5.9/Jenkinsfile
+-rw-r--r--   0        0        0      380 2023-02-07 11:08:17.446111 pyprocessors-pseudonimizer-0.5.9/README.md
+-rw-r--r--   0        0        0     1559 2023-02-07 11:08:17.447111 pyprocessors-pseudonimizer-0.5.9/bumpversion.py
+-rw-r--r--   0        0        0       67 2023-02-07 13:23:37.630437 pyprocessors-pseudonimizer-0.5.9/pyprocessors_pseudonimizer/__init__.py
+-rw-r--r--   0        0        0     2896 2023-02-07 11:08:17.448111 pyprocessors-pseudonimizer-0.5.9/pyprocessors_pseudonimizer/pseudonimizer.py
+-rw-r--r--   0        0        0     2214 2023-02-07 11:23:03.170663 pyprocessors-pseudonimizer-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-02-07 11:08:17.449111 pyprocessors-pseudonimizer-0.5.9/tests/__init__.py
+-rw-r--r--   0        0        0   119288 2023-02-07 13:23:34.700360 pyprocessors-pseudonimizer-0.5.9/tests/data/afp_ner_fr-document-test-anon.json
+-rw-r--r--   0        0        0   104534 2023-02-07 11:08:17.451111 pyprocessors-pseudonimizer-0.5.9/tests/data/afp_ner_fr-document-test.json
+-rw-r--r--   0        0        0      854 2023-02-07 11:08:17.451111 pyprocessors-pseudonimizer-0.5.9/tests/test_pseudonimizer.py
+-rw-r--r--   0        0        0      943 2023-02-07 11:08:17.452111 pyprocessors-pseudonimizer-0.5.9/tox.ini
+-rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 pyprocessors-pseudonimizer-0.5.9/setup.py
+-rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 pyprocessors-pseudonimizer-0.5.9/PKG-INFO
```

### Comparing `pyprocessors-pseudonimizer-0.5.7/Jenkinsfile` & `pyprocessors-pseudonimizer-0.5.9/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `pyprocessors-pseudonimizer-0.5.7/bumpversion.py` & `pyprocessors-pseudonimizer-0.5.9/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-pseudonimizer-0.5.7/pyprocessors_pseudonimizer/pseudonimizer.py` & `pyprocessors-pseudonimizer-0.5.9/pyprocessors_pseudonimizer/pseudonimizer.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-pseudonimizer-0.5.7/pyproject.toml` & `pyprocessors-pseudonimizer-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors-pseudonimizer-0.5.7/tests/data/afp_ner_fr-document-test-anon.json` & `pyprocessors-pseudonimizer-0.5.9/tests/data/afp_ner_fr-document-test-anon.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-pseudonimizer-0.5.7/tests/data/afp_ner_fr-document-test.json` & `pyprocessors-pseudonimizer-0.5.9/tests/data/afp_ner_fr-document-test.json`

 * *Files identical despite different names*

### Comparing `pyprocessors-pseudonimizer-0.5.7/tests/test_pseudonimizer.py` & `pyprocessors-pseudonimizer-0.5.9/tests/test_pseudonimizer.py`

 * *Files identical despite different names*

### Comparing `pyprocessors-pseudonimizer-0.5.7/tox.ini` & `pyprocessors-pseudonimizer-0.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors-pseudonimizer-0.5.7/setup.py` & `pyprocessors-pseudonimizer-0.5.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
           'dirty-equals']}
 
 entry_points = \
 {'pyprocessors.plugins': ['pseudonimizer = '
                           'pyprocessors_pseudonimizer.pseudonimizer:PseudonimizerProcessor']}
 
 setup(name='pyprocessors-pseudonimizer',
-      version='0.5.7',
+      version='0.5.9',
       description='Processor based on Presidio anonymizer',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyprocessors-pseudonimizer-0.5.7/PKG-INFO` & `pyprocessors-pseudonimizer-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-pseudonimizer
-Version: 0.5.7
+Version: 0.5.9
 Summary: Processor based on Presidio anonymizer
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

