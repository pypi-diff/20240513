# Comparing `tmp/scottbrian_locking-1.1.0.tar.gz` & `tmp/scottbrian_locking-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scottbrian_locking-1.1.0.tar", last modified: Mon Feb  6 21:57:58 2023, max compression
+gzip compressed data, was "scottbrian_locking-2.0.0.tar", last modified: Mon May 13 02:28:36 2024, max compression
```

## Comparing `scottbrian_locking-1.1.0.tar` & `scottbrian_locking-2.0.0.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-02-06 21:57:58.981795 scottbrian_locking-1.1.0/
--rw-rw-rw-   0        0        0     1945 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/.gitignore
-drwxrwxrwx   0        0        0        0 2023-02-06 21:57:58.956790 scottbrian_locking-1.1.0/.idea/
--rw-rw-rw-   0        0        0       50 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/.idea/.gitignore
-drwxrwxrwx   0        0        0        0 2023-02-06 21:57:58.958790 scottbrian_locking-1.1.0/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      527 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-rw-rw-   0        0        0      174 2022-01-24 23:37:11.000000 scottbrian_locking-1.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      209 2022-01-24 23:37:11.000000 scottbrian_locking-1.1.0/.idea/misc.xml
--rw-rw-rw-   0        0        0      295 2022-01-24 23:37:11.000000 scottbrian_locking-1.1.0/.idea/modules.xml
--rw-rw-rw-   0        0        0      492 2022-01-25 23:42:35.000000 scottbrian_locking-1.1.0/.idea/scottbrian_locking.iml
--rw-rw-rw-   0        0        0      185 2022-01-24 23:37:11.000000 scottbrian_locking-1.1.0/.idea/vcs.xml
--rw-rw-rw-   0        0        0      636 2022-01-25 20:13:50.000000 scottbrian_locking-1.1.0/.readthedocs.yml
--rw-rw-rw-   0        0        0     1092 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      472 2022-01-27 00:26:05.000000 scottbrian_locking-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2706 2023-02-06 21:57:58.981795 scottbrian_locking-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1665 2023-01-29 21:52:05.000000 scottbrian_locking-1.1.0/README.rst
--rw-rw-rw-   0        0        0     5202 2023-01-29 16:15:21.000000 scottbrian_locking-1.1.0/conftest.py
-drwxrwxrwx   0        0        0        0 2023-02-06 21:57:58.959790 scottbrian_locking-1.1.0/docs/
--rw-rw-rw-   0        0        0       42 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-02-06 21:57:58.964792 scottbrian_locking-1.1.0/docs/source/
--rw-rw-rw-   0        0        0        0 2022-01-26 20:25:53.000000 scottbrian_locking-1.1.0/docs/source/_static
--rw-rw-rw-   0        0        0     2381 2023-01-29 22:19:29.000000 scottbrian_locking-1.1.0/docs/source/conf.py
--rw-rw-rw-   0        0        0      429 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/docs/source/index.rst
--rw-rw-rw-   0        0        0       37 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/docs/source/se_lock_link.rst
--rw-rw-rw-   0        0        0      181 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/mypy.ini
--rw-rw-rw-   0        0        0      356 2023-01-29 22:23:09.000000 scottbrian_locking-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      582 2022-01-25 20:19:54.000000 scottbrian_locking-1.1.0/pytest.ini
--rw-rw-rw-   0        0        0     1283 2023-02-06 21:57:58.982796 scottbrian_locking-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      183 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-06 21:57:58.933974 scottbrian_locking-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-06 21:57:58.969793 scottbrian_locking-1.1.0/src/scottbrian_locking/
--rw-rw-rw-   0        0        0      141 2023-01-29 21:52:05.000000 scottbrian_locking-1.1.0/src/scottbrian_locking/__init__.py
--rw-rw-rw-   0        0        0      112 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/src/scottbrian_locking/__init__.pyi
--rw-rw-rw-   0        0        0      112 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/src/scottbrian_locking/py.typed
--rw-rw-rw-   0        0        0    35512 2023-01-29 22:18:21.000000 scottbrian_locking-1.1.0/src/scottbrian_locking/se_lock.py
-drwxrwxrwx   0        0        0        0 2023-02-06 21:57:58.976794 scottbrian_locking-1.1.0/src/scottbrian_locking.egg-info/
--rw-rw-rw-   0        0        0     2706 2023-02-06 21:57:58.000000 scottbrian_locking-1.1.0/src/scottbrian_locking.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      971 2023-02-06 21:57:58.000000 scottbrian_locking-1.1.0/src/scottbrian_locking.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-06 21:57:58.000000 scottbrian_locking-1.1.0/src/scottbrian_locking.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-01-25 20:24:35.000000 scottbrian_locking-1.1.0/src/scottbrian_locking.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       35 2023-02-06 21:57:58.000000 scottbrian_locking-1.1.0/src/scottbrian_locking.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-02-06 21:57:58.000000 scottbrian_locking-1.1.0/src/scottbrian_locking.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-06 21:57:58.935649 scottbrian_locking-1.1.0/tests/
-drwxrwxrwx   0        0        0        0 2023-02-06 21:57:58.980796 scottbrian_locking-1.1.0/tests/test_scottbrian_locking/
--rw-rw-rw-   0        0        0       40 2022-01-24 23:33:01.000000 scottbrian_locking-1.1.0/tests/test_scottbrian_locking/__init__.py
--rw-rw-rw-   0        0        0     5448 2023-01-29 16:26:55.000000 scottbrian_locking-1.1.0/tests/test_scottbrian_locking/conftest.py
--rw-rw-rw-   0        0        0    37119 2023-01-29 16:26:55.000000 scottbrian_locking-1.1.0/tests/test_scottbrian_locking/test_se_lock.py
--rw-rw-rw-   0        0        0     3519 2023-01-29 21:56:20.000000 scottbrian_locking-1.1.0/tox.ini
+drwxrwxrwx   0        0        0        0 2024-05-13 02:28:36.480392 scottbrian_locking-2.0.0/
+-rw-rw-rw-   0        0        0     1945 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-13 02:28:36.449895 scottbrian_locking-2.0.0/.idea/
+-rw-rw-rw-   0        0        0       50 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/.idea/.gitignore
+drwxrwxrwx   0        0        0        0 2024-05-13 02:28:36.452897 scottbrian_locking-2.0.0/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      527 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-rw-rw-   0        0        0      174 2022-01-24 23:37:11.000000 scottbrian_locking-2.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      430 2023-12-28 02:51:45.000000 scottbrian_locking-2.0.0/.idea/misc.xml
+-rw-rw-rw-   0        0        0      295 2022-01-24 23:37:11.000000 scottbrian_locking-2.0.0/.idea/modules.xml
+-rw-rw-rw-   0        0        0      552 2023-11-20 13:23:51.000000 scottbrian_locking-2.0.0/.idea/scottbrian_locking.iml
+-rw-rw-rw-   0        0        0      185 2022-01-24 23:37:11.000000 scottbrian_locking-2.0.0/.idea/vcs.xml
+-rw-rw-rw-   0        0        0      636 2022-01-25 20:13:50.000000 scottbrian_locking-2.0.0/.readthedocs.yml
+-rw-rw-rw-   0        0        0     1092 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      472 2022-01-27 00:26:05.000000 scottbrian_locking-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4050 2024-05-13 02:28:36.479393 scottbrian_locking-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1883 2024-05-11 17:34:13.000000 scottbrian_locking-2.0.0/README.rst
+-rw-rw-rw-   0        0        0      431 2023-11-24 14:22:31.000000 scottbrian_locking-2.0.0/conftest.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:28:36.453896 scottbrian_locking-2.0.0/docs/
+-rw-rw-rw-   0        0        0       42 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 02:28:36.459898 scottbrian_locking-2.0.0/docs/source/
+-rw-rw-rw-   0        0        0        0 2022-01-26 20:25:53.000000 scottbrian_locking-2.0.0/docs/source/_static
+-rw-rw-rw-   0        0        0     2381 2023-11-20 19:24:52.000000 scottbrian_locking-2.0.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      429 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0       83 2024-05-11 17:50:15.000000 scottbrian_locking-2.0.0/docs/source/se_lock_link.rst
+-rw-rw-rw-   0        0        0      181 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/mypy.ini
+-rw-rw-rw-   0        0        0     1117 2024-05-13 01:26:04.000000 scottbrian_locking-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0      582 2022-01-25 20:19:54.000000 scottbrian_locking-2.0.0/pytest.ini
+-rw-rw-rw-   0        0        0       42 2024-05-13 02:28:36.480392 scottbrian_locking-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      183 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:28:36.427997 scottbrian_locking-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-13 02:28:36.464899 scottbrian_locking-2.0.0/src/scottbrian_locking/
+-rw-rw-rw-   0        0        0      141 2023-11-20 19:24:52.000000 scottbrian_locking-2.0.0/src/scottbrian_locking/__init__.py
+-rw-rw-rw-   0        0        0      112 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/src/scottbrian_locking/__init__.pyi
+-rw-rw-rw-   0        0        0      112 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/src/scottbrian_locking/py.typed
+-rw-rw-rw-   0        0        0    62896 2024-05-11 18:45:44.000000 scottbrian_locking-2.0.0/src/scottbrian_locking/se_lock.py
+drwxrwxrwx   0        0        0        0 2024-05-13 02:28:36.477392 scottbrian_locking-2.0.0/src/scottbrian_locking.egg-info/
+-rw-rw-rw-   0        0        0     4050 2024-05-13 02:28:36.000000 scottbrian_locking-2.0.0/src/scottbrian_locking.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      920 2024-05-13 02:28:36.000000 scottbrian_locking-2.0.0/src/scottbrian_locking.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-13 02:28:36.000000 scottbrian_locking-2.0.0/src/scottbrian_locking.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-13 02:28:36.000000 scottbrian_locking-2.0.0/src/scottbrian_locking.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-13 02:28:36.000000 scottbrian_locking-2.0.0/src/scottbrian_locking.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-13 02:28:36.428997 scottbrian_locking-2.0.0/tests/
+drwxrwxrwx   0        0        0        0 2024-05-13 02:28:36.475391 scottbrian_locking-2.0.0/tests/test_scottbrian_locking/
+-rw-rw-rw-   0        0        0       40 2022-01-24 23:33:01.000000 scottbrian_locking-2.0.0/tests/test_scottbrian_locking/__init__.py
+-rw-rw-rw-   0        0        0     5411 2024-04-24 23:54:46.000000 scottbrian_locking-2.0.0/tests/test_scottbrian_locking/conftest.py
+-rw-rw-rw-   0        0        0   144170 2024-05-10 20:56:28.000000 scottbrian_locking-2.0.0/tests/test_scottbrian_locking/test_se_lock.py
+-rw-rw-rw-   0        0        0     3842 2024-05-08 01:08:03.000000 scottbrian_locking-2.0.0/tox.ini
```

### Comparing `scottbrian_locking-1.1.0/.gitignore` & `scottbrian_locking-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scottbrian_locking-1.1.0/.idea/inspectionProfiles/Project_Default.xml` & `scottbrian_locking-2.0.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `scottbrian_locking-1.1.0/.readthedocs.yml` & `scottbrian_locking-2.0.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scottbrian_locking-1.1.0/LICENSE` & `scottbrian_locking-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scottbrian_locking-1.1.0/PKG-INFO` & `scottbrian_locking-2.0.0/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,18 @@
-Metadata-Version: 2.1
-Name: scottbrian_locking
-Version: 1.1.0
-Summary: Parallel processing tools
-Home-page: https://github.com/ScottBrian/scottbrian_locking.git
-Author: Scott Tuttle
-Author-email: sbtuttle@outlook.com
-License: MIT
-Project-URL: Documentation, https://scottbrian-locking.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/ScottBrian/scottbrian_locking.git
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Recovery Tools
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ==================
 scottbrian-locking
 ==================
 
 Intro
 =====
 
-The SELock is a shared/exclusive lock that you can use to safely read
-and write shared resources in a multi-threaded application.
+The SELock is a shared/exclusive lock that you can use to coordinate
+read and write access to a resource in a multithreaded application.
 
-:Example: use SELock to coordinate access to a shared resource
+:Example: use SELock to coordinate access to a resource
 
 >>> from scottbrian_locking import se_lock as sel
 >>> a_lock = sel.SELock()
 >>> # Get lock in exclusive mode
 >>> with sel.SELockExcl(a_lock):
 ...     msg = 'lock obtained exclusive'
 >>> print(msg)
@@ -78,14 +53,21 @@
 * 1.0.0
     * Initial release
 
 * 1.1.0
     * Add RELockObtain context manager
     * support python 3.11
 
+* 2.0.0
+    * Add obtain_tf to context manager
+    * Add allow_recursive_obtain
+    * Delete setup.cfg
+    * Make consistent log and error messages
+    * Support python 3.12
+    * Drop support for python < 3.12
 
 Meta
 ====
 
 Scott Tuttle
 
 Distributed under the MIT license. See ``LICENSE`` for more information.
```

### Comparing `scottbrian_locking-1.1.0/docs/source/conf.py` & `scottbrian_locking-2.0.0/docs/source/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'scottbrian_locking'
 copyright = '2021, 2023, Scott Tuttle'
 author = 'Scott Tuttle'
 
 # The full version, including alpha/beta/rc tags
-release = '1.1.0'
+release = '2.0.0'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `scottbrian_locking-1.1.0/pytest.ini` & `scottbrian_locking-2.0.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `scottbrian_locking-1.1.0/src/scottbrian_locking.egg-info/SOURCES.txt` & `scottbrian_locking-2.0.0/src/scottbrian_locking.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 .gitignore
 .readthedocs.yml
-LICENSE
+LICENSE.txt
 MANIFEST.in
 README.rst
 conftest.py
 mypy.ini
 pyproject.toml
 pytest.ini
-setup.cfg
 setup.py
 tox.ini
 .idea/.gitignore
 .idea/misc.xml
 .idea/modules.xml
 .idea/scottbrian_locking.iml
 .idea/vcs.xml
@@ -25,13 +24,12 @@
 src/scottbrian_locking/__init__.py
 src/scottbrian_locking/__init__.pyi
 src/scottbrian_locking/py.typed
 src/scottbrian_locking/se_lock.py
 src/scottbrian_locking.egg-info/PKG-INFO
 src/scottbrian_locking.egg-info/SOURCES.txt
 src/scottbrian_locking.egg-info/dependency_links.txt
-src/scottbrian_locking.egg-info/not-zip-safe
 src/scottbrian_locking.egg-info/requires.txt
 src/scottbrian_locking.egg-info/top_level.txt
 tests/test_scottbrian_locking/__init__.py
 tests/test_scottbrian_locking/conftest.py
 tests/test_scottbrian_locking/test_se_lock.py
```

### Comparing `scottbrian_locking-1.1.0/tests/test_scottbrian_locking/conftest.py` & `scottbrian_locking-2.0.0/tests/test_scottbrian_locking/conftest.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,32 +21,35 @@
 # type aliases
 ########################################################################
 OptIntFloat = Optional[Union[int, float]]
 
 ########################################################################
 # logging
 ########################################################################
-logging.basicConfig(filename='Lock.log',
-                    filemode='w',
-                    level=logging.DEBUG,
-                    format='%(asctime)s '
-                           '[%(levelname)8s] '
-                           '%(filename)s:'
-                           '%(funcName)s:'
-                           '%(lineno)d '
-                           '%(message)s')
+logging.basicConfig(
+    filename="Lock.log",
+    filemode="w",
+    level=logging.DEBUG,
+    format="%(asctime)s "
+    "[%(levelname)8s] "
+    "%(filename)s:"
+    "%(funcName)s:"
+    "%(lineno)d "
+    "%(message)s",
+)
 
 logger = logging.getLogger(__name__)
 
 
 ########################################################################
 # Thread exceptions
 # The following fixture depends on the following pytest specification:
 # -p no:threadexception
 
+
 # For PyCharm, the above specification goes into field Additional
 # Arguments found at Run -> edit configurations
 #
 # For tox, the above specification goes into tox.ini in the
 # the string for the commands=
 # For example, in tox.ini for the pytest section:
 # [testenv:py{36, 37, 38, 39}-pytest]
@@ -74,41 +77,41 @@
 #
 ########################################################################
 class ExcHook:
     """ExcHook class."""
 
     def __init__(self) -> None:
         """Initialize the ExcHook class instance."""
-        self.exc_err_msg1 = ''
+        self.exc_err_msg1 = ""
 
     def raise_exc_if_one(self) -> None:
         """Raise an error is we have one.
 
         Raises:
             Exception: exc_msg
 
         """
         if self.exc_err_msg1:
             exc_msg = self.exc_err_msg1
-            self.exc_err_msg1 = ''
-            raise Exception(f'{exc_msg}')
+            self.exc_err_msg1 = ""
+            raise Exception(f"{exc_msg}")
 
 
-@pytest.fixture(autouse=True)  # type: ignore
+@pytest.fixture(autouse=True)
 def thread_exc(monkeypatch: Any) -> Generator[ExcHook, None, None]:
     """Instantiate and return a ThreadExc for testing.
 
     Args:
         monkeypatch: pytest fixture used to modify code for testing
 
     Yields:
         a thread exception handler
 
     """
-    logger.debug(f'hook before: {threading.excepthook}')
+    # logger.debug(f"hook before: {threading.excepthook}")
     exc_hook = ExcHook()
 
     def mock_threading_excepthook(args: Any) -> None:
         """Build error message from exception.
 
         Args:
             args: contains:
@@ -116,37 +119,40 @@
                       args.exc_value: Optional[BaseException]
                       args.exc_traceback: Optional[TracebackType]
 
         Raises:
             Exception: Test case thread test error
 
         """
-        exc_err_msg = (f'thread_exc excepthook: {args.exc_type}, '
-                       f'{args.exc_value}, {args.exc_traceback},'
-                       f' {args.thread}')
+        exc_err_msg = (
+            f"Test case excepthook: {args.exc_type}, "
+            f"{args.exc_value}, {args.exc_traceback},"
+            f" {args.thread}"
+        )
         traceback.print_tb(args.exc_traceback)
         logger.debug(exc_err_msg)
         current_thread = threading.current_thread()
-        logger.debug(f'excepthook current thread is {current_thread}')
+        logging.exception(f"exception caught for {current_thread}")
+        logger.debug(f"excepthook current thread is {current_thread}")
         # ExcHook.exc_err_msg1 = exc_err_msg
         exc_hook.exc_err_msg1 = exc_err_msg
-        raise Exception(f'thread_exc thread test error: {exc_err_msg}')
+        # assert False
+        raise Exception(f"Test case thread test error: {exc_err_msg}")
 
     monkeypatch.setattr(threading, "excepthook", mock_threading_excepthook)
-    logger.debug(f'hook after: {threading.excepthook}')
+    # logger.debug(f"hook after: {threading.excepthook}")
     new_hook = threading.excepthook
 
     yield exc_hook
 
-    # clean the registry in SELock class
-    # SELock._registry = {}
-
-    # clean the registry in ThreadPair class
-    # ThreadPair._registry = {}
+    # surface any remote thread uncaught exceptions
+    exc_hook.raise_exc_if_one()
 
     # the following check ensures that the test case waited via join for
     # any started threads to come home
+    if threading.active_count() > 1:
+        for thread in threading.enumerate():
+            print(f"conftest thread: {thread}")
     assert threading.active_count() == 1
-    exc_hook.raise_exc_if_one()
 
     # the following assert ensures -p no:threadexception was specified
     assert threading.excepthook == new_hook
```

### Comparing `scottbrian_locking-1.1.0/tox.ini` & `scottbrian_locking-2.0.0/tox.ini`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tox]
-envlist = {py39}, lint, mypy, mypywrapt, pytest, coverage, docs
+envlist = {py312}, lint, mypy, pytest, coverage, docs
 
-[testenv:py{39}-bandit]
+[testenv:py{312}-bandit]
 description = invoke bandit to verify security
 deps =
     bandit
 
 commands =
     bandit -r src
 
-[testenv:py{39}-safety]
+[testenv:py{312}-safety]
 description = invoke safety to verify security
 deps =
     safety
-    pip>=21.1.3
+    pip~=24.0
 
 commands =
     safety check
 
 [check-manifest]
 ignore =
     .idea/codeStyles/codeStyleConfig.xml
@@ -37,14 +37,17 @@
     check-manifest
 
 commands =
     check-manifest
 
 [flake8]
 max-doc-length = 72
+max-line-length = 88
+select = C, E, F, W, B, B950
+extend-ignore = E203, W503
 
 [testenv:lint]
 description = invoke flake8 to check style
 
 deps =
     flake8
     flake8-docstrings
@@ -57,69 +60,85 @@
     # flake8 --statistics --docstring-convention google src/scottbrian_locking/se_lock.py
     # flake8 --statistics --docstring-convention google tests/test_scottbrian_locking/test_se_lock.py
 
     # apparently, having darglint installed via deps causes flake8 to call it similar to the following calls
     # darglint -v 2 src/scottbrian_locking/
     # darglint -v 2 tests/test_scottbrian_locking/
 
-[testenv:py{39}-mypy]
-description = invoke mypy to check types
+[testenv:darglint]
+description = invoke darglint to check style
 
 deps =
-    mypy
+    darglint
+
+[darglint]
+ignore=DAR402
 
 commands =
-    mypy src/scottbrian_locking/
-    mypy tests/test_scottbrian_locking/ --cache-dir=/dev/null
 
+    darglint -v 2 src/scottbrian_utils/
+    darglint -v 2 tests/test_scottbrian_utils/
+
+[testenv:mypy]
+description = invoke mypy to check types
 
-[testenv:py{39}-pytest]
-description = invoke pytest on the package
 deps =
+    mypy
     pytest
     sybil
 
 commands =
-    pytest --import-mode=importlib --capture=tee-sys -p no:threadexception {posargs}
-    # pytest --import-mode=importlib --capture=tee-sys -p no:threadexception tests/test_scottbrian_locking/test_se_lock.py::TestSELockBasic::test_se_lock_len
-    # pytest --import-mode=importlib --capture=tee-sys {posargs}
+    mypy src/scottbrian_locking/
+    mypy tests/test_scottbrian_locking/ --cache-dir=/dev/null
+
 
-[testenv:py{39}-doctest]
+[testenv:py{312}-doctest]
 description = invoke pytest with doctest option on the package
 # need a separate doctest here instead of using doctest in the above pytest run because doctest adds the source paths
 # to sys.path which causes pytest to import from the source directory instead of from the virtual env site-packages,
 # which defeats the purpose of building the virtual env and installing the package to test the actual build
 
 deps =
     pytest
     sybil
 
 commands =
     pytest --ignore=tests -p no:threadexception
     # pytest --ignore='tests' --doctest-modules --log-cli-level=ERROR -p no:threadexception {posargs}
     # pytest --ignore='tests' --doctest-modules {posargs}
 
-[testenv:py{39}-coverage]
+[testenv:py{312}-coverage]
 description = invoke pytest-cov on the package
 
 deps =
     pytest
     pytest-cov
     sybil
 
 commands =
     pytest --cov=scottbrian_locking --cov-report=term --cov-report=html -p no:threadexception {posargs}
 
+[testenv:py{312}-pytest]
+description = invoke pytest on the package
+deps =
+    pytest
+    sybil
+
+commands =
+    pytest --import-mode=importlib --capture=tee-sys -p no:threadexception {posargs}
+    # pytest --import-mode=importlib --capture=tee-sys -p no:threadexception tests/test_scottbrian_locking/test_se_lock.py::TestSELockBasic::test_se_lock_len
+    # pytest --import-mode=importlib --capture=tee-sys {posargs}
 
 [testenv:docs]
 description = invoke sphinx-build to build the HTML docs
-basepython = 
-    python3.9
-deps = 
+basepython =
+    python3.12
+deps =
     sphinx
     sphinx-autodoc-typehints
     sphinx_rtd_theme
     pytest
+    sybil
 
 commands =
     sphinx-build -b html docs/source docs/build -W -a -E
     python -c 'import pathlib; print("documentation available under file://\{0\}".format(pathlib.Path(r"docs") / "build" / "index.html"))'
```

