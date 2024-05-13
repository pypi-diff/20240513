# Comparing `tmp/umpire-0.7.0.tar.gz` & `tmp/umpire-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umpire-0.7.0.tar", last modified: Tue May  7 13:17:59 2024, max compression
+gzip compressed data, was "umpire-0.7.1.tar", last modified: Mon May 13 13:50:53 2024, max compression
```

## Comparing `umpire-0.7.0.tar` & `umpire-0.7.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-07 13:17:59.481830 umpire-0.7.0/
--rwx------   0 mperttula   (502) staff       (20)     1081 2019-04-25 16:17:36.000000 umpire-0.7.0/LICENSE
--rw-r--r--   0 mperttula   (502) staff       (20)      310 2024-05-07 13:17:59.477768 umpire-0.7.0/PKG-INFO
--rwxr-xr-x   0 mperttula   (502) staff       (20)     3267 2024-05-07 13:13:16.000000 umpire-0.7.0/README.md
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-07 13:17:59.476269 umpire-0.7.0/Umpire.egg-info/
--rw-r--r--   0 mperttula   (502) staff       (20)      310 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/PKG-INFO
--rw-r--r--   0 mperttula   (502) staff       (20)      732 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/SOURCES.txt
--rw-r--r--   0 mperttula   (502) staff       (20)        1 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/dependency_links.txt
--rw-r--r--   0 mperttula   (502) staff       (20)       47 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/entry_points.txt
--rw-r--r--   0 mperttula   (502) staff       (20)       29 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/requires.txt
--rw-r--r--   0 mperttula   (502) staff       (20)        7 2024-05-07 13:17:59.000000 umpire-0.7.0/Umpire.egg-info/top_level.txt
--rw-r--r--   0 mperttula   (502) staff       (20)       38 2024-05-07 13:17:59.482244 umpire-0.7.0/setup.cfg
--rwxr-xr-x   0 mperttula   (502) staff       (20)      820 2024-05-07 13:13:16.000000 umpire-0.7.0/setup.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-07 13:17:59.374060 umpire-0.7.0/umpire/
--rwx------   0 mperttula   (502) staff       (20)        0 2019-04-25 16:17:36.000000 umpire-0.7.0/umpire/__init__.py
--rwxr-xr-x   0 mperttula   (502) staff       (20)    15314 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/cache.py
--rwx------   0 mperttula   (502) staff       (20)      703 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/config.py
--rwxr-xr-x   0 mperttula   (502) staff       (20)    12568 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/deploy.py
--rwxr-xr-x   0 mperttula   (502) staff       (20)     8459 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/fetch.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-07 13:17:59.376355 umpire-0.7.0/umpire/test/
--rwx------   0 mperttula   (502) staff       (20)        0 2019-04-25 16:17:36.000000 umpire-0.7.0/umpire/test/__init__.py
-drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-07 13:17:59.475080 umpire-0.7.0/umpire/test/deploy_tests/
--rwx------   0 mperttula   (502) staff       (20)        0 2019-04-25 16:17:36.000000 umpire-0.7.0/umpire/test/deploy_tests/__init__.py
--rwx------   0 mperttula   (502) staff       (20)     2996 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc1_full_deploy.py
--rwx------   0 mperttula   (502) staff       (20)     2674 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc2_deploy_from_existing_cache.py
--rwx------   0 mperttula   (502) staff       (20)     2786 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc3_fresh_deploy_from_cleared_cache.py
--rwx------   0 mperttula   (502) staff       (20)     2682 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc4_existing_deploy_from_cleared_cache.py
--rwx------   0 mperttula   (502) staff       (20)     2047 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc5_no_extract_copy.py
--rwx------   0 mperttula   (502) staff       (20)     4696 2021-06-02 14:40:13.000000 umpire-0.7.0/umpire/test/deploy_tests/tc6_keep_updated.py
--rwxr-xr-x   0 mperttula   (502) staff       (20)     5285 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/umpire.py
--rw-r--r--   0 mperttula   (502) staff       (20)     1812 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/unpack.py
--rwxr-xr-x   0 mperttula   (502) staff       (20)     1436 2024-05-07 13:13:16.000000 umpire-0.7.0/umpire/update.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:50:53.391780 umpire-0.7.1/
+-rwx------   0 mperttula   (502) staff       (20)     1081 2019-04-25 16:17:36.000000 umpire-0.7.1/LICENSE
+-rw-r--r--   0 mperttula   (502) staff       (20)      310 2024-05-13 13:50:53.390905 umpire-0.7.1/PKG-INFO
+-rwxr-xr-x   0 mperttula   (502) staff       (20)     3267 2024-05-07 13:13:16.000000 umpire-0.7.1/README.md
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:50:53.389925 umpire-0.7.1/Umpire.egg-info/
+-rw-r--r--   0 mperttula   (502) staff       (20)      310 2024-05-13 13:50:53.000000 umpire-0.7.1/Umpire.egg-info/PKG-INFO
+-rw-r--r--   0 mperttula   (502) staff       (20)      732 2024-05-13 13:50:53.000000 umpire-0.7.1/Umpire.egg-info/SOURCES.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)        1 2024-05-13 13:50:53.000000 umpire-0.7.1/Umpire.egg-info/dependency_links.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)       47 2024-05-13 13:50:53.000000 umpire-0.7.1/Umpire.egg-info/entry_points.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)       29 2024-05-13 13:50:53.000000 umpire-0.7.1/Umpire.egg-info/requires.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)        7 2024-05-13 13:50:53.000000 umpire-0.7.1/Umpire.egg-info/top_level.txt
+-rw-r--r--   0 mperttula   (502) staff       (20)       38 2024-05-13 13:50:53.392013 umpire-0.7.1/setup.cfg
+-rwxr-xr-x   0 mperttula   (502) staff       (20)      820 2024-05-13 13:50:28.000000 umpire-0.7.1/setup.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:50:53.292401 umpire-0.7.1/umpire/
+-rwx------   0 mperttula   (502) staff       (20)        0 2019-04-25 16:17:36.000000 umpire-0.7.1/umpire/__init__.py
+-rwxr-xr-x   0 mperttula   (502) staff       (20)    15314 2024-05-07 13:13:16.000000 umpire-0.7.1/umpire/cache.py
+-rwx------   0 mperttula   (502) staff       (20)      703 2021-06-02 14:40:13.000000 umpire-0.7.1/umpire/config.py
+-rwxr-xr-x   0 mperttula   (502) staff       (20)    12568 2024-05-07 13:13:16.000000 umpire-0.7.1/umpire/deploy.py
+-rwxr-xr-x   0 mperttula   (502) staff       (20)     8459 2024-05-07 13:13:16.000000 umpire-0.7.1/umpire/fetch.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:50:53.293556 umpire-0.7.1/umpire/test/
+-rwx------   0 mperttula   (502) staff       (20)        0 2019-04-25 16:17:36.000000 umpire-0.7.1/umpire/test/__init__.py
+drwxr-xr-x   0 mperttula   (502) staff       (20)        0 2024-05-13 13:50:53.388730 umpire-0.7.1/umpire/test/deploy_tests/
+-rwx------   0 mperttula   (502) staff       (20)        0 2019-04-25 16:17:36.000000 umpire-0.7.1/umpire/test/deploy_tests/__init__.py
+-rwx------   0 mperttula   (502) staff       (20)     2996 2021-06-02 14:40:13.000000 umpire-0.7.1/umpire/test/deploy_tests/tc1_full_deploy.py
+-rwx------   0 mperttula   (502) staff       (20)     2674 2021-06-02 14:40:13.000000 umpire-0.7.1/umpire/test/deploy_tests/tc2_deploy_from_existing_cache.py
+-rwx------   0 mperttula   (502) staff       (20)     2786 2021-06-02 14:40:13.000000 umpire-0.7.1/umpire/test/deploy_tests/tc3_fresh_deploy_from_cleared_cache.py
+-rwx------   0 mperttula   (502) staff       (20)     2682 2021-06-02 14:40:13.000000 umpire-0.7.1/umpire/test/deploy_tests/tc4_existing_deploy_from_cleared_cache.py
+-rwx------   0 mperttula   (502) staff       (20)     2047 2021-06-02 14:40:13.000000 umpire-0.7.1/umpire/test/deploy_tests/tc5_no_extract_copy.py
+-rwx------   0 mperttula   (502) staff       (20)     4696 2021-06-02 14:40:13.000000 umpire-0.7.1/umpire/test/deploy_tests/tc6_keep_updated.py
+-rwxr-xr-x   0 mperttula   (502) staff       (20)     5284 2024-05-13 13:50:28.000000 umpire-0.7.1/umpire/umpire.py
+-rw-r--r--   0 mperttula   (502) staff       (20)     1812 2024-05-07 13:13:16.000000 umpire-0.7.1/umpire/unpack.py
+-rwxr-xr-x   0 mperttula   (502) staff       (20)     1436 2024-05-07 13:13:16.000000 umpire-0.7.1/umpire/update.py
```

### Comparing `umpire-0.7.0/LICENSE` & `umpire-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/README.md` & `umpire-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/Umpire.egg-info/SOURCES.txt` & `umpire-0.7.1/Umpire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/setup.py` & `umpire-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from os import path
 # this_directory = path.abspath(path.dirname(__file__))
 # with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
 #     long_description = f.read()
 
 setup(name='Umpire',
-      version='0.7.0',
+      version='0.7.1',
       description='Generic dependency resolver.',
       long_description='',
       long_description_content_type='text/markdown',
       author='Signiant SRE',
       author_email='sre@signiant.com',
       url='https://www.signiant.com',
       packages=find_packages(),
```

### Comparing `umpire-0.7.0/umpire/cache.py` & `umpire-0.7.1/umpire/cache.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/config.py` & `umpire-0.7.1/umpire/config.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/deploy.py` & `umpire-0.7.1/umpire/deploy.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/fetch.py` & `umpire-0.7.1/umpire/fetch.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/test/deploy_tests/tc1_full_deploy.py` & `umpire-0.7.1/umpire/test/deploy_tests/tc1_full_deploy.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/test/deploy_tests/tc2_deploy_from_existing_cache.py` & `umpire-0.7.1/umpire/test/deploy_tests/tc2_deploy_from_existing_cache.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/test/deploy_tests/tc3_fresh_deploy_from_cleared_cache.py` & `umpire-0.7.1/umpire/test/deploy_tests/tc3_fresh_deploy_from_cleared_cache.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/test/deploy_tests/tc4_existing_deploy_from_cleared_cache.py` & `umpire-0.7.1/umpire/test/deploy_tests/tc4_existing_deploy_from_cleared_cache.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/test/deploy_tests/tc5_no_extract_copy.py` & `umpire-0.7.1/umpire/test/deploy_tests/tc5_no_extract_copy.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/test/deploy_tests/tc6_keep_updated.py` & `umpire-0.7.1/umpire/test/deploy_tests/tc6_keep_updated.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/umpire.py` & `umpire-0.7.1/umpire/umpire.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
         parser = argparse.ArgumentParser(description='Umpire reads a properly formatted JSON deployment file to deploy files.')
         parser.add_argument('-c', '--clear-cache', help='Clear umpire cache', dest='clear', action='store_true', required=False)
         parser.add_argument('-r', '--repair-cache', help='Removes lock files from the cache', dest='repair', action='store_true', required=False)
         parser.add_argument('-v', '--version', help='Displays the current version of Umpire', dest='version',  action='store_true', required=False)
         parser.add_argument('UMPIRE_FILE', help='Umpire json manifest file', nargs='?')
-        parser.add_argument('-d', '--debpug', help='Run without creating keys or updating keys', dest='debug', action='store_true',
+        parser.add_argument('-d', '--debug', help='Run without creating keys or updating keys', dest='debug', action='store_true',
                             required=False)
         args = parser.parse_args()
 
 
         log_level = logging.INFO
         if args.debug:
             print('DEBUG logging requested')
```

### Comparing `umpire-0.7.0/umpire/unpack.py` & `umpire-0.7.1/umpire/unpack.py`

 * *Files identical despite different names*

### Comparing `umpire-0.7.0/umpire/update.py` & `umpire-0.7.1/umpire/update.py`

 * *Files identical despite different names*

