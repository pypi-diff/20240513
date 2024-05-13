# Comparing `tmp/nbtof-0.0.7.tar.gz` & `tmp/nbtof-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbtof-0.0.7.tar", last modified: Sat May  4 13:52:18 2024, max compression
+gzip compressed data, was "nbtof-0.0.8.tar", last modified: Mon May 13 13:55:43 2024, max compression
```

## Comparing `nbtof-0.0.7.tar` & `nbtof-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 13:52:18.168233 nbtof-0.0.7/
--rw-rw-rw-   0        0        0     1084 2023-11-20 14:37:06.000000 nbtof-0.0.7/LICENSE
--rw-rw-rw-   0        0        0        0 2023-12-12 14:56:20.000000 nbtof-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     4462 2024-05-04 13:52:18.166229 nbtof-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3788 2024-05-04 09:38:02.000000 nbtof-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 13:52:18.154507 nbtof-0.0.7/nbtof/
--rw-rw-rw-   0        0        0       54 2024-05-03 07:16:39.000000 nbtof-0.0.7/nbtof/__init__.py
--rw-rw-rw-   0        0        0    12387 2024-05-04 13:46:23.000000 nbtof-0.0.7/nbtof/nbtof_base.py
--rw-rw-rw-   0        0        0     9289 2024-05-02 07:02:04.000000 nbtof-0.0.7/nbtof/nbtof_concat.py
--rw-rw-rw-   0        0        0     2777 2024-05-03 06:05:36.000000 nbtof-0.0.7/nbtof/nbtof_generate.py
-drwxrwxrwx   0        0        0        0 2024-05-04 13:52:18.162432 nbtof-0.0.7/nbtof.egg-info/
--rw-rw-rw-   0        0        0     4462 2024-05-04 13:52:17.000000 nbtof-0.0.7/nbtof.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-04 13:52:18.000000 nbtof-0.0.7/nbtof.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 13:52:17.000000 nbtof-0.0.7/nbtof.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-04 13:52:17.000000 nbtof-0.0.7/nbtof.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-04 13:52:18.169228 nbtof-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1337 2024-05-04 13:48:19.000000 nbtof-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:55:43.632219 nbtof-0.0.8/
+-rw-rw-rw-   0        0        0     1084 2023-11-20 14:37:06.000000 nbtof-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-12-12 14:56:20.000000 nbtof-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5939 2024-05-13 13:55:43.629220 nbtof-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     5265 2024-05-07 13:43:47.000000 nbtof-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-13 13:55:43.574895 nbtof-0.0.8/nbtof/
+-rw-rw-rw-   0        0        0       54 2024-05-13 13:45:55.000000 nbtof-0.0.8/nbtof/__init__.py
+-rw-rw-rw-   0        0        0    12374 2024-05-13 13:51:46.000000 nbtof-0.0.8/nbtof/nbtof_base.py
+-rw-rw-rw-   0        0        0     9289 2024-05-02 07:02:04.000000 nbtof-0.0.8/nbtof/nbtof_concat.py
+-rw-rw-rw-   0        0        0     2777 2024-05-03 06:05:36.000000 nbtof-0.0.8/nbtof/nbtof_generate.py
+drwxrwxrwx   0        0        0        0 2024-05-13 13:55:43.625206 nbtof-0.0.8/nbtof.egg-info/
+-rw-rw-rw-   0        0        0     5939 2024-05-13 13:55:43.000000 nbtof-0.0.8/nbtof.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-13 13:55:43.000000 nbtof-0.0.8/nbtof.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 13:55:43.000000 nbtof-0.0.8/nbtof.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-13 13:55:43.000000 nbtof-0.0.8/nbtof.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-13 13:55:43.633225 nbtof-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1337 2024-05-13 13:52:51.000000 nbtof-0.0.8/setup.py
```

### Comparing `nbtof-0.0.7/LICENSE` & `nbtof-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nbtof-0.0.7/PKG-INFO` & `nbtof-0.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbtof
-Version: 0.0.7
+Version: 0.0.8
 Summary: nbtof: transfering notebook to function
 Home-page: https://github.com/Nodaka/nbtof
 Download-URL: https://github.com/Nodaka/nbtof
 Author: Haruka Nodaka
 Author-email: haruka.nodaka@gmail.com
 Maintainer: Haruka Nodaka
 Maintainer-email: haruka.nodaka@gmail.com
@@ -16,35 +16,41 @@
 Classifier: Framework :: Jupyter
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nbtof <!-- omit in toc -->
 
-This module is used to convert .ipynb file to .py function.  
+---
 
-- [Intoroduction](#intoroduction)
+| English | [日本語](https://github.com/Nodaka/nbtof/blob/main/i18n/README-JA.md) |
+
+---
+
+This module is used to convert Jupyter Notebook to the python function with the same process.  
+
+
+- [Introduction](#introduction)
 - [Installation](#installation)
-- [Documantation](#documantation)
+- [Documentation](#documentation)
   - [Marks list](#marks-list)
   - [Details about marks](#details-about-marks)
     - [#@param](#param)
     - [#@default](#default)
-    - [#@default](#default-1)
     - [#@args](#args)
     - [#@kwargs](#kwargs)
     - [#@return](#return)
     - [#@ignore](#ignore)
     - [#@help](#help)
     - [#@advance](#advance)
     - [#@r\_advance](#r_advance)
 
 
 
-## Intoroduction
+## Introduction
 
 Only by writing the `#@~` marks in Jupyter Notebook file, you can easily convert Jupyter Notebook file to the python source file with the function which perform the same process as the Jupyter Notebook file. For example, in the case that you want to convert `sample.ipynb` to function,
 
   
 **sample.ipynb**
 
 ```python
@@ -56,57 +62,57 @@
 c = a + b
 ```
 ```python
 #@return
 c
 ```
   
-you can get `output.py` by executing the next code.
+you can get `sample.py` by executing the next code.
 
 ```python
 import nbtof
 
 nbtof.nbtof_generate(
     notebook_name='sample.ipynb',
-    func_py_name='sample_output.py',
+    func_py_name='sample.py',
     )
 ```
 
-**sample_output.py**
+**sample.py**
 
 ```python
 def sample(a, b):
     c = a + b
     return c
 ```
 
 
 ## Installation
 The latest nbtof can be installed from PyPI:  
 
 ```
-pip install nbtof
+$ pip install nbtof
 ```
 
 
-## Documantation
+## Documentation
 
 ### Marks list
 
 | Mark | Description |
 | ---- | ---- |
 | `#@param` | Variable names in the cell become function's argument names. The values assigned at the Jupyter Notebook is ignored. |
 | `#@default` | Variable names in the cell become function's argument names. The values assigned at the Jupyter Notebook get default values. |
 | `#@args` | Variable names in the cell become function's variable length argument *args names. The values assigned at the notebook is ignored. |
 | `#@kwargs` | Variable names in the cell become function's variable length argument **kwargs names. The values assigned at the notebook is ignored. |
 | `#@return` | The line after this mark become function's return value |
 | `#@ignore` | Anything in the cell is ignored. |
 | `#@help` | What you write in the cell becomes function's docstring. Please write it in quotation marks. |
 | `#@advance` | What you write in the cell is written before the function declaration as it is. (e.g., imports) |
-| `#@r_advance` | The comment line with `#` in the cell is written with the `#` removed before the function declaration. (e.g., relative imports) | 
+| `#@r_advance` | The comment line with `#` in the cell is written with the `#` removed before the function declaration. Please use to avoid the error in Jupyter Notebook (e.g., relative imports) | 
 
 ### Details about marks
 
 #### #@param
 
 The Jupyter Notebook
 
@@ -148,82 +154,192 @@
 ```python
 
 def sample_default(a=0):
     print('Hello world !')
 
 ```
 
-#### #@default
-
-The Jupyter Notebook
+#### #@args
 
-**sample_default.ipynb**
+**sample_args.ipynb**
 ```python
-#@default
+#@args
 a = 0
 ```
 ```python
 print("Hello World !")
 ```
 
 is converted into
 
 
 ```python
 
-def sample_default(a=0):
+def sample_args(*a):
     print('Hello world !')
 
 ```
 
-#### #@args
 
-**sample_args.ipynb**
+#### #@kwargs
+
+**sample_kwargs.ipynb**
 ```python
-#@args
+#@kwargs
 a = 0
 ```
 ```python
 print("Hello World !")
 ```
 
 is converted into
 
 
 ```python
-
-def sample_args(*a):
+def sample_kwargs(**a):
     print('Hello world !')
-
 ```
 
 
-#### #@kwargs
+#### #@return
 
-**sample_kwargs.ipynb**
+**sample_return.ipynb**
 ```python
-#@kwargs
+#@return
 a = 0
 ```
 ```python
-print("Hello World !")
+if a == 0:
+#@return
+    True
+else:
+#@return
+    False
 ```
 
 is converted into
 
 
 ```python
 
-def sample_kwargs(**a):
-    print('Hello world !')
-
+def sample_return(a):
+    if a == 0:
+        return True
+    else:
+        return False
 ```
 
 
-#### #@return
 
+#### #@ignore
+
+**sample_ignore.ipynb**
+```python
+#@ignore
+1 + 1
+```
+```python
+print('Hello world !')
+```
+
+is converted into
 
 
-#### #@ignore
+```python
+def sample_ignore():
+    print('Hello world !')
+```
+
 #### #@help
+**sample_help.ipynb**
+```python
+#@help
+"""
+This function outputs "Hello world !" sentence.
+
+Parameters
+----------
+
+Returns
+-------
+
+"""
+```
+```python
+print('Hello world !')
+```
+
+is converted into
+
+
+```python
+def sample_help():
+    """
+    This function outputs "Hello world !" sentence.
+    
+    Parameters
+    ----------
+    
+    Returns
+    -------
+    
+    """
+    print('Hello world !')
+```
+
 #### #@advance
+
+**sample_advance.ipynb**
+```python
+#@advance
+import os
+import sys
+```
+```python
+#@advance
+def func():
+    print(os.getcwd())
+    print(sys.prefix)
+    print("Hello world !")
+```
+```python
+func()
+```
+
+is converted into
+
+
+```python
+import os
+import sys
+
+def func():
+    print(os.getcwd())
+    print(sys.prefix)
+    print('Hello world !')
+
+def sample_advance():
+    func()
+```
+
 #### #@r_advance
+
+**sample_r_advance.ipynb**
+```python
+#@r_advance
+#from . import foo
+#from . import bar
+```
+```python
+print("Hello world !")
+```
+
+is converted into
+
+
+```python
+from . import foo
+from . import bar
+
+def sample_r_advance():
+    print('Hello world !')
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nbtof-0.0.7/nbtof/nbtof_base.py` & `nbtof-0.0.8/nbtof/nbtof_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 import subprocess
 import sys
 import copy
 
 def nbtof_base(
     notebook_name,
-    func_name=None,
-    func_file_name=None,
+    func_name = None,
+    func_file_name = None,
     ):
     """
     This function converts noetbook into a function that performs the same processing as the notebook according to nbtof tags.
     
     Parameters
     ----------
     notebook_name : str
@@ -228,15 +228,15 @@
             instant_list[1] = '    ' + instant_list[1]
         
         elif (instant_list[0]==code_dict['#@param'])*('=' in (instant_list[1])):
             instant_list[1] = '    ' + instant_list[1].split('=')[0].replace(' ', '') + ',\n'
         elif (instant_list[0]==code_dict['#@args'])*('=' in (instant_list[1])):
             instant_list[1] = '    *' + instant_list[1].split('=')[0].replace(' ', '') + ',\n'
         elif (instant_list[0]==code_dict['#@default'])*('=' in (instant_list[1])):
-            instant_list[1] = '    ' + instant_list[1].replace('\n','').replace(' ', '') + ',\n'
+            instant_list[1] = '    ' + instant_list[1].replace('\n','') + ',\n'
         elif (instant_list[0]==code_dict['#@kwargs'])*('=' in (instant_list[1])):
             instant_list[1] = '    **' + instant_list[1].split('=')[0].replace(' ', '') + ',\n'
         
         elif (instant_list[0]==code_dict['#@param'])*('=' not in (instant_list[1])):
             continue
         elif (instant_list[0]==code_dict['#@args'])*('=' not in (instant_list[1])):
             continue
```

### Comparing `nbtof-0.0.7/nbtof/nbtof_concat.py` & `nbtof-0.0.8/nbtof/nbtof_concat.py`

 * *Files identical despite different names*

### Comparing `nbtof-0.0.7/nbtof/nbtof_generate.py` & `nbtof-0.0.8/nbtof/nbtof_generate.py`

 * *Files identical despite different names*

### Comparing `nbtof-0.0.7/nbtof.egg-info/PKG-INFO` & `nbtof-0.0.8/nbtof.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbtof
-Version: 0.0.7
+Version: 0.0.8
 Summary: nbtof: transfering notebook to function
 Home-page: https://github.com/Nodaka/nbtof
 Download-URL: https://github.com/Nodaka/nbtof
 Author: Haruka Nodaka
 Author-email: haruka.nodaka@gmail.com
 Maintainer: Haruka Nodaka
 Maintainer-email: haruka.nodaka@gmail.com
@@ -16,35 +16,41 @@
 Classifier: Framework :: Jupyter
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nbtof <!-- omit in toc -->
 
-This module is used to convert .ipynb file to .py function.  
+---
 
-- [Intoroduction](#intoroduction)
+| English | [日本語](https://github.com/Nodaka/nbtof/blob/main/i18n/README-JA.md) |
+
+---
+
+This module is used to convert Jupyter Notebook to the python function with the same process.  
+
+
+- [Introduction](#introduction)
 - [Installation](#installation)
-- [Documantation](#documantation)
+- [Documentation](#documentation)
   - [Marks list](#marks-list)
   - [Details about marks](#details-about-marks)
     - [#@param](#param)
     - [#@default](#default)
-    - [#@default](#default-1)
     - [#@args](#args)
     - [#@kwargs](#kwargs)
     - [#@return](#return)
     - [#@ignore](#ignore)
     - [#@help](#help)
     - [#@advance](#advance)
     - [#@r\_advance](#r_advance)
 
 
 
-## Intoroduction
+## Introduction
 
 Only by writing the `#@~` marks in Jupyter Notebook file, you can easily convert Jupyter Notebook file to the python source file with the function which perform the same process as the Jupyter Notebook file. For example, in the case that you want to convert `sample.ipynb` to function,
 
   
 **sample.ipynb**
 
 ```python
@@ -56,57 +62,57 @@
 c = a + b
 ```
 ```python
 #@return
 c
 ```
   
-you can get `output.py` by executing the next code.
+you can get `sample.py` by executing the next code.
 
 ```python
 import nbtof
 
 nbtof.nbtof_generate(
     notebook_name='sample.ipynb',
-    func_py_name='sample_output.py',
+    func_py_name='sample.py',
     )
 ```
 
-**sample_output.py**
+**sample.py**
 
 ```python
 def sample(a, b):
     c = a + b
     return c
 ```
 
 
 ## Installation
 The latest nbtof can be installed from PyPI:  
 
 ```
-pip install nbtof
+$ pip install nbtof
 ```
 
 
-## Documantation
+## Documentation
 
 ### Marks list
 
 | Mark | Description |
 | ---- | ---- |
 | `#@param` | Variable names in the cell become function's argument names. The values assigned at the Jupyter Notebook is ignored. |
 | `#@default` | Variable names in the cell become function's argument names. The values assigned at the Jupyter Notebook get default values. |
 | `#@args` | Variable names in the cell become function's variable length argument *args names. The values assigned at the notebook is ignored. |
 | `#@kwargs` | Variable names in the cell become function's variable length argument **kwargs names. The values assigned at the notebook is ignored. |
 | `#@return` | The line after this mark become function's return value |
 | `#@ignore` | Anything in the cell is ignored. |
 | `#@help` | What you write in the cell becomes function's docstring. Please write it in quotation marks. |
 | `#@advance` | What you write in the cell is written before the function declaration as it is. (e.g., imports) |
-| `#@r_advance` | The comment line with `#` in the cell is written with the `#` removed before the function declaration. (e.g., relative imports) | 
+| `#@r_advance` | The comment line with `#` in the cell is written with the `#` removed before the function declaration. Please use to avoid the error in Jupyter Notebook (e.g., relative imports) | 
 
 ### Details about marks
 
 #### #@param
 
 The Jupyter Notebook
 
@@ -148,82 +154,192 @@
 ```python
 
 def sample_default(a=0):
     print('Hello world !')
 
 ```
 
-#### #@default
-
-The Jupyter Notebook
+#### #@args
 
-**sample_default.ipynb**
+**sample_args.ipynb**
 ```python
-#@default
+#@args
 a = 0
 ```
 ```python
 print("Hello World !")
 ```
 
 is converted into
 
 
 ```python
 
-def sample_default(a=0):
+def sample_args(*a):
     print('Hello world !')
 
 ```
 
-#### #@args
 
-**sample_args.ipynb**
+#### #@kwargs
+
+**sample_kwargs.ipynb**
 ```python
-#@args
+#@kwargs
 a = 0
 ```
 ```python
 print("Hello World !")
 ```
 
 is converted into
 
 
 ```python
-
-def sample_args(*a):
+def sample_kwargs(**a):
     print('Hello world !')
-
 ```
 
 
-#### #@kwargs
+#### #@return
 
-**sample_kwargs.ipynb**
+**sample_return.ipynb**
 ```python
-#@kwargs
+#@return
 a = 0
 ```
 ```python
-print("Hello World !")
+if a == 0:
+#@return
+    True
+else:
+#@return
+    False
 ```
 
 is converted into
 
 
 ```python
 
-def sample_kwargs(**a):
-    print('Hello world !')
-
+def sample_return(a):
+    if a == 0:
+        return True
+    else:
+        return False
 ```
 
 
-#### #@return
 
+#### #@ignore
+
+**sample_ignore.ipynb**
+```python
+#@ignore
+1 + 1
+```
+```python
+print('Hello world !')
+```
+
+is converted into
 
 
-#### #@ignore
+```python
+def sample_ignore():
+    print('Hello world !')
+```
+
 #### #@help
+**sample_help.ipynb**
+```python
+#@help
+"""
+This function outputs "Hello world !" sentence.
+
+Parameters
+----------
+
+Returns
+-------
+
+"""
+```
+```python
+print('Hello world !')
+```
+
+is converted into
+
+
+```python
+def sample_help():
+    """
+    This function outputs "Hello world !" sentence.
+    
+    Parameters
+    ----------
+    
+    Returns
+    -------
+    
+    """
+    print('Hello world !')
+```
+
 #### #@advance
+
+**sample_advance.ipynb**
+```python
+#@advance
+import os
+import sys
+```
+```python
+#@advance
+def func():
+    print(os.getcwd())
+    print(sys.prefix)
+    print("Hello world !")
+```
+```python
+func()
+```
+
+is converted into
+
+
+```python
+import os
+import sys
+
+def func():
+    print(os.getcwd())
+    print(sys.prefix)
+    print('Hello world !')
+
+def sample_advance():
+    func()
+```
+
 #### #@r_advance
+
+**sample_r_advance.ipynb**
+```python
+#@r_advance
+#from . import foo
+#from . import bar
+```
+```python
+print("Hello world !")
+```
+
+is converted into
+
+
+```python
+from . import foo
+from . import bar
+
+def sample_r_advance():
+    print('Hello world !')
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nbtof-0.0.7/setup.py` & `nbtof-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DESCRIPTION = "nbtof: transfering notebook to function"
 NAME = 'nbtof'
 AUTHOR = 'Haruka Nodaka'
 AUTHOR_EMAIL = 'haruka.nodaka@gmail.com'
 URL = 'https://github.com/Nodaka/nbtof'
 LICENSE = 'MIT'
 DOWNLOAD_URL = 'https://github.com/Nodaka/nbtof'
-VERSION = "0.0.7"
+VERSION = "0.0.8"
 PYTHON_REQUIRES = ">=3.9"
 
 INSTALL_REQUIRES = [
 #    'pandas',
 #    'nbconvert',
 #    'jupyter',
 ]
```

