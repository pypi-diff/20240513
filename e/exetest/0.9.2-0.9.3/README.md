# Comparing `tmp/exetest-0.9.2.tar.gz` & `tmp/exetest-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exetest-0.9.2.tar", last modified: Mon May 13 09:28:32 2024, max compression
+gzip compressed data, was "exetest-0.9.3.tar", last modified: Mon May 13 10:30:54 2024, max compression
```

## Comparing `exetest-0.9.2.tar` & `exetest-0.9.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-05-13 09:28:32.266216 exetest-0.9.2/
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      699 2024-05-13 09:28:32.266216 exetest-0.9.2/PKG-INFO
-drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-05-13 09:28:32.266216 exetest-0.9.2/exetest/
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      183 2024-05-13 08:36:57.942206 exetest-0.9.2/exetest/__init__.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     6755 2024-05-13 09:19:49.446325 exetest-0.9.2/exetest/dataframe_utils.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7914 2024-05-13 08:36:57.942206 exetest-0.9.2/exetest/diff_utils.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      429 2024-05-13 08:36:57.942206 exetest-0.9.2/exetest/env_vars.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)    22270 2024-05-13 08:36:57.942206 exetest-0.9.2/exetest/exetest_decorator.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1670 2024-05-13 08:36:57.942206 exetest-0.9.2/exetest/expects_exception.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7196 2024-05-13 08:36:57.952206 exetest-0.9.2/exetest/misc_utils.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     6885 2024-05-13 08:36:57.952206 exetest-0.9.2/exetest/runmain.py
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)       62 2024-05-13 08:26:18.252304 exetest-0.9.2/setup.cfg
--rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1539 2024-05-13 09:22:06.446295 exetest-0.9.2/setup.py
+drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-05-13 10:30:54.630127 exetest-0.9.3/
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      699 2024-05-13 10:30:54.630127 exetest-0.9.3/PKG-INFO
+drwxr-xr-x   0 ggiraud   (1000) ggiraud   (1000)        0 2024-05-13 10:30:54.630127 exetest-0.9.3/exetest/
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      183 2024-05-13 08:36:57.942206 exetest-0.9.3/exetest/__init__.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     6762 2024-05-13 10:29:37.080149 exetest-0.9.3/exetest/dataframe_utils.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7914 2024-05-13 08:36:57.942206 exetest-0.9.3/exetest/diff_utils.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)      429 2024-05-13 08:36:57.942206 exetest-0.9.3/exetest/env_vars.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)    22270 2024-05-13 08:36:57.942206 exetest-0.9.3/exetest/exetest_decorator.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1670 2024-05-13 08:36:57.942206 exetest-0.9.3/exetest/expects_exception.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     7196 2024-05-13 08:36:57.952206 exetest-0.9.3/exetest/misc_utils.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     6885 2024-05-13 08:36:57.952206 exetest-0.9.3/exetest/runmain.py
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)       62 2024-05-13 08:26:18.252304 exetest-0.9.3/setup.cfg
+-rw-r--r--   0 ggiraud   (1000) ggiraud   (1000)     1539 2024-05-13 10:30:19.100144 exetest-0.9.3/setup.py
```

### Comparing `exetest-0.9.2/PKG-INFO` & `exetest-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: exetest
-Version: 0.9.2
+Version: 0.9.3
 Summary: A pytest-based test framework for black-box approach to testing executables
 Home-page: https://github.com/Guillaume227/exetest
 Author: Guillaume227
 Author-email: guillaume227@gmail.com
 License: MIT
 Download-URL: https://github.com/Guillaume227/exetest/archive/v0.1-alpha.tar.gz
 Description: UNKNOWN
```

### Comparing `exetest-0.9.2/exetest/dataframe_utils.py` & `exetest-0.9.3/exetest/dataframe_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                            np.issubdtype(df2[col].dtype, np.number):
                             numerical_diff_cols.append(col)
                         else:
                             non_numerical_diff_cols.append(col)
 
                     if numerical_diff_cols:
                         float_format = pd.options.display.float_format
-                        pd.options.display.float_format = "{:.2f}"
+                        pd.options.display.float_format = "{:.2f}".format
                         print(f'correlation of numerical cols:')
                         print(df1[numerical_diff_cols].corrwith(df2[numerical_diff_cols]).to_string())
                         print()
                         pd.options.display.float_format = float_format  # restore format
 
                     if self.num_diffs_to_display:
                         if self.num_diffs_to_display > 0:
```

### Comparing `exetest-0.9.2/exetest/diff_utils.py` & `exetest-0.9.3/exetest/diff_utils.py`

 * *Files identical despite different names*

### Comparing `exetest-0.9.2/exetest/exetest_decorator.py` & `exetest-0.9.3/exetest/exetest_decorator.py`

 * *Files identical despite different names*

### Comparing `exetest-0.9.2/exetest/expects_exception.py` & `exetest-0.9.3/exetest/expects_exception.py`

 * *Files identical despite different names*

### Comparing `exetest-0.9.2/exetest/misc_utils.py` & `exetest-0.9.3/exetest/misc_utils.py`

 * *Files identical despite different names*

### Comparing `exetest-0.9.2/exetest/runmain.py` & `exetest-0.9.3/exetest/runmain.py`

 * *Files identical despite different names*

### Comparing `exetest-0.9.2/setup.py` & `exetest-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name='exetest',         # How you named your package folder (MyLib)
   packages=['exetest'],   # Chose the same as "name"
-  version='0.9.2',      # Start with a small number and increase it with every change you make
+  version='0.9.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description='A pytest-based test framework for black-box approach to testing executables',   # Give a short description about your library
   author='Guillaume227',                   # Type in your name
   author_email='guillaume227@gmail.com',      # Type in your E-Mail
   url='https://github.com/Guillaume227/exetest',   # Provide either the link to your github or to your website
   download_url='https://github.com/Guillaume227/exetest/archive/v0.1-alpha.tar.gz',
   keywords=['test', 'pytest', 'nosetest'],  # Keywords that define your package best
```

