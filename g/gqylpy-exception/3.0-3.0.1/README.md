# Comparing `tmp/gqylpy_exception-3.0.tar.gz` & `tmp/gqylpy_exception-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqylpy_exception-3.0.tar", last modified: Fri Feb  9 10:02:15 2024, max compression
+gzip compressed data, was "gqylpy_exception-3.0.1.tar", last modified: Mon May 13 01:21:49 2024, max compression
```

## Comparing `gqylpy_exception-3.0.tar` & `gqylpy_exception-3.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 10:02:15.476002 gqylpy_exception-3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11389 2024-02-09 10:02:03.000000 gqylpy_exception-3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-02-09 10:02:15.476002 gqylpy_exception-3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-09 10:02:03.000000 gqylpy_exception-3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 10:02:15.472002 gqylpy_exception-3.0/gqylpy_exception/
--rw-r--r--   0 runner    (1001) docker     (127)     7684 2024-02-09 10:02:03.000000 gqylpy_exception-3.0/gqylpy_exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11192 2024-02-09 10:02:03.000000 gqylpy_exception-3.0/gqylpy_exception/g exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 10:02:15.476002 gqylpy_exception-3.0/gqylpy_exception.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-02-09 10:02:15.000000 gqylpy_exception-3.0/gqylpy_exception.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-09 10:02:15.000000 gqylpy_exception-3.0/gqylpy_exception.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 10:02:15.000000 gqylpy_exception-3.0/gqylpy_exception.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-09 10:02:15.000000 gqylpy_exception-3.0/gqylpy_exception.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 10:02:15.476002 gqylpy_exception-3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-02-09 10:02:03.000000 gqylpy_exception-3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:21:49.337370 gqylpy_exception-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-05-13 01:21:43.000000 gqylpy_exception-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-13 01:21:49.337370 gqylpy_exception-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-13 01:21:43.000000 gqylpy_exception-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:21:49.337370 gqylpy_exception-3.0.1/gqylpy_exception/
+-rw-r--r--   0 runner    (1001) docker     (127)     7685 2024-05-13 01:21:43.000000 gqylpy_exception-3.0.1/gqylpy_exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11152 2024-05-13 01:21:43.000000 gqylpy_exception-3.0.1/gqylpy_exception/g exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 01:21:49.337370 gqylpy_exception-3.0.1/gqylpy_exception.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-13 01:21:49.000000 gqylpy_exception-3.0.1/gqylpy_exception.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 01:21:49.000000 gqylpy_exception-3.0.1/gqylpy_exception.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 01:21:49.000000 gqylpy_exception-3.0.1/gqylpy_exception.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 01:21:49.000000 gqylpy_exception-3.0.1/gqylpy_exception.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 01:21:49.337370 gqylpy_exception-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-13 01:21:43.000000 gqylpy_exception-3.0.1/setup.py
```

### Comparing `gqylpy_exception-3.0/LICENSE` & `gqylpy_exception-3.0.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
+   Copyright (c) 2022-2024 GQYLPY <http://gqylpy.com>. All rights reserved.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `gqylpy_exception-3.0/PKG-INFO` & `gqylpy_exception-3.0.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gqylpy_exception
-Version: 3.0
-Summary: 在执行 raise 语句的同时创建异常类，无需提前定义异常类，方便快捷。
+Version: 3.0.1
+Summary: Raise exceptions while creating exception classes on the fly, without the need to predefine them beforehand.
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-exception
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,42 +18,44 @@
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: Artistic Software
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8, <4
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img alt="LOGO" src="http://gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-exception.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-exception/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_exception)](https://pypi.org/project/gqylpy_exception)
 [![License](https://img.shields.io/pypi/l/gqylpy_exception)](https://github.com/gqylpy/gqylpy-exception/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/gqylpy_exception)](https://pepy.tech/project/gqylpy_exception)
 
 # gqylpy-exception
+English | [中文](https://github.com/gqylpy/gqylpy-exception/blob/master/README_CN.md)
 
-
-> 在执行 `raise` 语句的同时创建异常类，无需提前定义异常类，方便快捷。例如，你想抛出一个名为 `NotUnderstandError` 的异常，
-> 导入 `import gqylpy_exception as ge` 后直接执行 `raise ge.NotUnderstandError` 即可。
+Raise exceptions while creating exception classes on the fly, without the need to predefine them beforehand. For instance, if you want to raise an exception named `NotUnderstandError`, simply import `import gqylpy_exception as ge` and execute `raise ge.NotUnderstandError` directly for convenience and efficiency.
 
 <kbd>pip3 install gqylpy_exception</kbd>
 
+###### Using `gqylpy_exception` to Create Exception Classes
 
-###### 使用 `gqylpy_exception` 创建异常类
 ```python
 import gqylpy_exception as ge
 
 raise ge.AnError(...)
 ```
-`gqylpy_exception` 可以创建任意名称的异常类。`AnError` 不是 `gqylpy_exception` 中内置的，它是在你的代码执行到 `ge.` 
-时创建的，魔化方法 `__getattr__` 的特性。
 
-还有一种用法，导入即创建：
+With `gqylpy_exception`, you can create exception classes with arbitrary names. `AnError` is not predefined in `gqylpy_exception`; it is dynamically created when your code executes `ge.` due to the magic method `__getattr__`.
+
+Alternatively, you can also create exceptions upon import:
+
 ```python
 from gqylpy_exception import AnError
 
 raise AnError(...)
 ```
-最后，`gqylpy_exception` 不会重复创建异常类，创建过的异常类将存入 `ge.__history__` 字典，当你再次创建时从这个字典中取值。
+
+Lastly, `gqylpy_exception` avoids duplicate creation of exception classes. Once an exception class has been created, it is stored in the `ge.__history__` dictionary. When you attempt to create the same exception again, it will be retrieved from this dictionary.
```

### Comparing `gqylpy_exception-3.0/gqylpy_exception/__init__.py` & `gqylpy_exception-3.0.1/gqylpy_exception/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Create the exception class while executing the `raise` statement, you no longer
 need to define an exception class in advance, Convenient and Fast.
 
     >>> import gqylpy_exception as ge
     >>> raise ge.AnError(...)
 
-    @version: 3.0
+    @version: 3.0.1
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/gqylpy-exception
 
 ────────────────────────────────────────────────────────────────────────────────
-Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
+Copyright (c) 2022-2024 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `gqylpy_exception-3.0/gqylpy_exception/g exception.py` & `gqylpy_exception-3.0.1/gqylpy_exception/g exception.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
+Copyright (c) 2022-2024 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     https://www.apache.org/licenses/LICENSE-2.0
 
@@ -48,15 +48,15 @@
 
 
 class MasqueradeClass(type):
     """
     Masquerade one class as another (default masquerade as first parent class).
     Warning, masquerade the class can cause unexpected problems, use caution.
     """
-    __module__   = builtins.__name__
+    __module__ = builtins.__name__
 
     __qualname__ = type.__qualname__
     # Warning, masquerade (modify) this attribute will cannot create the
     # portable serialized representation. In practice, however, this metaclass
     # often does not need to be serialized, so we try to ignore it.
 
     def __new__(mcs, __name__: str, __bases__: tuple, __dict__: dict):
@@ -125,28 +125,28 @@
         return __history__[ename]
 
     if ename[:2] == ename[-2:] == '__' and ename[2] != '_' and ename[-3] != '_':
         # Some special modules may attempt to call non-built-in magic method,
         # such as `copy`, `pickle`. Compatible for this purpose.
         raise AttributeError(f'"{__package__}" has no attribute "{ename}".')
 
-    eclass = getattr(builtins, ename, None)
-    if isinstance(eclass, type) and issubclass(eclass, BaseException):
-        return eclass
+    etype = getattr(builtins, ename, None)
+    if isinstance(etype, type) and issubclass(etype, BaseException):
+        return etype
 
     if ename[-5:] != 'Error':
         warnings.warn(
             f'strange exception class "{ename}", exception class name should '
             'end with "Error".', stacklevel=2
         )
 
-    eclass = type(ename, (GqylpyError,), {})
-    dict.__setitem__(__history__, ename, eclass)
+    etype = type(ename, (GqylpyError,), {})
+    dict.__setitem__(__history__, ename, etype)
 
-    return eclass
+    return etype
 
 
 def stderr(einfo: str) -> None:
     now: str = time.strftime('%F %T', time.localtime())
     sys.stderr.write(f'[{now}] {einfo}\n')
 
 
@@ -193,33 +193,33 @@
         self.local: bool = self.__class__ is TryExcept
 
     def __call__(self, func: Function) -> Closure:
         try:
             core = func.__closure__[1].cell_contents.core.__func__
         except (TypeError, IndexError, AttributeError):
             if asyncio.iscoroutinefunction(func):
-                self.core = self.core_async
+                self.core = self.acore
         else:
-            if core in (TryExcept.core_async, Retry.core_async):
-                self.core = self.core_async
+            if core in (TryExcept.acore, Retry.acore):
+                self.core = self.acore
 
         @functools.wraps(func, updated=('__dict__', '__globals__'))
         def inner(*a, **kw) -> Any:
             return self.core(func, *a, **kw)
 
         return inner
 
     def core(self, func: Function, *a, **kw) -> Any:
         try:
             return func(*a, **kw)
         except self.etype as e:
             self.exception_handling(func, e, *a, **kw)
         return self.ereturn
 
-    async def core_async(self, func: Function, *a, **kw) -> Any:
+    async def acore(self, func: Function, *a, **kw) -> Any:
         try:
             return await func(*a, **kw)
         except self.etype as e:
             self.exception_handling(func, e, *a, **kw)
         return self.ereturn
 
     def exception_handling(
@@ -320,15 +320,15 @@
                 count += 1
                 self.exception_handling(func, e, count=count)
                 if count == self.count:
                     raise e
 
             time.sleep(self.cycle)
 
-    async def core_async(self, func: Function, *a, **kw) -> Any:
+    async def acore(self, func: Function, *a, **kw) -> Any:
         count = 0
 
         while True:
             try:
                 return await func(*a, **kw)
             except self.etype as e:
                 count += 1
```

### Comparing `gqylpy_exception-3.0/gqylpy_exception.egg-info/PKG-INFO` & `gqylpy_exception-3.0.1/gqylpy_exception.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gqylpy_exception
-Version: 3.0
-Summary: 在执行 raise 语句的同时创建异常类，无需提前定义异常类，方便快捷。
+Version: 3.0.1
+Summary: Raise exceptions while creating exception classes on the fly, without the need to predefine them beforehand.
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/gqylpy-exception
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,42 +18,44 @@
 Classifier: Topic :: Software Development :: Widget Sets
 Classifier: Topic :: Artistic Software
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8, <4
+Classifier: Programming Language :: Python :: 3.13
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img alt="LOGO" src="http://gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/gqylpy-exception.svg?style=flat-square")](https://github.com/gqylpy/gqylpy-exception/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/gqylpy_exception)](https://pypi.org/project/gqylpy_exception)
 [![License](https://img.shields.io/pypi/l/gqylpy_exception)](https://github.com/gqylpy/gqylpy-exception/blob/master/LICENSE)
 [![Downloads](https://static.pepy.tech/badge/gqylpy_exception)](https://pepy.tech/project/gqylpy_exception)
 
 # gqylpy-exception
+English | [中文](https://github.com/gqylpy/gqylpy-exception/blob/master/README_CN.md)
 
-
-> 在执行 `raise` 语句的同时创建异常类，无需提前定义异常类，方便快捷。例如，你想抛出一个名为 `NotUnderstandError` 的异常，
-> 导入 `import gqylpy_exception as ge` 后直接执行 `raise ge.NotUnderstandError` 即可。
+Raise exceptions while creating exception classes on the fly, without the need to predefine them beforehand. For instance, if you want to raise an exception named `NotUnderstandError`, simply import `import gqylpy_exception as ge` and execute `raise ge.NotUnderstandError` directly for convenience and efficiency.
 
 <kbd>pip3 install gqylpy_exception</kbd>
 
+###### Using `gqylpy_exception` to Create Exception Classes
 
-###### 使用 `gqylpy_exception` 创建异常类
 ```python
 import gqylpy_exception as ge
 
 raise ge.AnError(...)
 ```
-`gqylpy_exception` 可以创建任意名称的异常类。`AnError` 不是 `gqylpy_exception` 中内置的，它是在你的代码执行到 `ge.` 
-时创建的，魔化方法 `__getattr__` 的特性。
 
-还有一种用法，导入即创建：
+With `gqylpy_exception`, you can create exception classes with arbitrary names. `AnError` is not predefined in `gqylpy_exception`; it is dynamically created when your code executes `ge.` due to the magic method `__getattr__`.
+
+Alternatively, you can also create exceptions upon import:
+
 ```python
 from gqylpy_exception import AnError
 
 raise AnError(...)
 ```
-最后，`gqylpy_exception` 不会重复创建异常类，创建过的异常类将存入 `ge.__history__` 字典，当你再次创建时从这个字典中取值。
+
+Lastly, `gqylpy_exception` avoids duplicate creation of exception classes. Once an exception class has been created, it is stored in the `ge.__history__` dictionary. When you attempt to create the same exception again, it will be retrieved from this dictionary.
```

### Comparing `gqylpy_exception-3.0/setup.py` & `gqylpy_exception-3.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,19 +14,22 @@
     name=g.__name__,
     version=version,
     author=author,
     author_email=email,
     license='Apache 2.0',
     url='http://gqylpy.com',
     project_urls={'Source': source},
-    description='在执行 raise 语句的同时创建异常类，无需提前定义异常类，方便快捷。',
+    description='''
+        Raise exceptions while creating exception classes on the fly, without
+        the need to predefine them beforehand.
+    '''.strip().replace('\n       ', ''),
     long_description=open('README.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     packages=[g.__name__],
-    python_requires='>=3.8, <4',
+    python_requires='>=3.8',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: Chinese (Simplified)',
         'Natural Language :: English',
         'Operating System :: OS Independent',
@@ -34,10 +37,11 @@
         'Topic :: Software Development :: Bug Tracking',
         'Topic :: Software Development :: Widget Sets',
         'Topic :: Artistic Software',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
-        'Programming Language :: Python :: 3.12'
+        'Programming Language :: Python :: 3.12',
+        'Programming Language :: Python :: 3.13'
     ]
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

