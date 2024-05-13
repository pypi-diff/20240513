# Comparing `tmp/b3denv-0.0.8.tar.gz` & `tmp/b3denv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b3denv-0.0.8.tar", last modified: Mon Sep 25 18:46:12 2023, max compression
+gzip compressed data, was "b3denv-0.0.9.tar", last modified: Mon Sep 25 19:16:57 2023, max compression
```

## Comparing `b3denv-0.0.8.tar` & `b3denv-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-09-25 18:46:12.581066 b3denv-0.0.8/
--rw-r--r--   0 robstenson   (501) staff       (20)    11341 2023-08-04 15:38:30.000000 b3denv-0.0.8/LICENSE
--rw-r--r--   0 robstenson   (501) staff       (20)      476 2023-09-25 18:46:12.580935 b3denv-0.0.8/PKG-INFO
--rw-r--r--   0 robstenson   (501) staff       (20)     2589 2023-09-25 18:27:08.000000 b3denv-0.0.8/README.md
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-09-25 18:46:12.580022 b3denv-0.0.8/b3denv/
--rw-r--r--   0 robstenson   (501) staff       (20)    11372 2023-09-25 18:45:15.000000 b3denv-0.0.8/b3denv/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)       62 2022-11-09 19:31:16.000000 b3denv-0.0.8/b3denv/__main__.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-09-25 18:46:12.580762 b3denv-0.0.8/b3denv.egg-info/
--rw-r--r--   0 robstenson   (501) staff       (20)      476 2023-09-25 18:46:12.000000 b3denv-0.0.8/b3denv.egg-info/PKG-INFO
--rw-r--r--   0 robstenson   (501) staff       (20)      217 2023-09-25 18:46:12.000000 b3denv-0.0.8/b3denv.egg-info/SOURCES.txt
--rw-r--r--   0 robstenson   (501) staff       (20)        1 2023-09-25 18:46:12.000000 b3denv-0.0.8/b3denv.egg-info/dependency_links.txt
--rw-r--r--   0 robstenson   (501) staff       (20)       39 2023-09-25 18:46:12.000000 b3denv-0.0.8/b3denv.egg-info/entry_points.txt
--rw-r--r--   0 robstenson   (501) staff       (20)        7 2023-09-25 18:46:12.000000 b3denv-0.0.8/b3denv.egg-info/top_level.txt
--rw-r--r--   0 robstenson   (501) staff       (20)       38 2023-09-25 18:46:12.581112 b3denv-0.0.8/setup.cfg
--rw-r--r--   0 robstenson   (501) staff       (20)      745 2023-09-25 18:45:15.000000 b3denv-0.0.8/setup.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-09-25 19:16:57.199032 b3denv-0.0.9/
+-rw-r--r--   0 robstenson   (501) staff       (20)    11341 2023-08-04 15:38:30.000000 b3denv-0.0.9/LICENSE
+-rw-r--r--   0 robstenson   (501) staff       (20)      476 2023-09-25 19:16:57.198914 b3denv-0.0.9/PKG-INFO
+-rw-r--r--   0 robstenson   (501) staff       (20)     2589 2023-09-25 18:27:08.000000 b3denv-0.0.9/README.md
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-09-25 19:16:57.197923 b3denv-0.0.9/b3denv/
+-rw-r--r--   0 robstenson   (501) staff       (20)    11559 2023-09-25 19:13:30.000000 b3denv-0.0.9/b3denv/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)       62 2022-11-09 19:31:16.000000 b3denv-0.0.9/b3denv/__main__.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-09-25 19:16:57.198767 b3denv-0.0.9/b3denv.egg-info/
+-rw-r--r--   0 robstenson   (501) staff       (20)      476 2023-09-25 19:16:57.000000 b3denv-0.0.9/b3denv.egg-info/PKG-INFO
+-rw-r--r--   0 robstenson   (501) staff       (20)      217 2023-09-25 19:16:57.000000 b3denv-0.0.9/b3denv.egg-info/SOURCES.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)        1 2023-09-25 19:16:57.000000 b3denv-0.0.9/b3denv.egg-info/dependency_links.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)       39 2023-09-25 19:16:57.000000 b3denv-0.0.9/b3denv.egg-info/entry_points.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)        7 2023-09-25 19:16:57.000000 b3denv-0.0.9/b3denv.egg-info/top_level.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)       38 2023-09-25 19:16:57.199069 b3denv-0.0.9/setup.cfg
+-rw-r--r--   0 robstenson   (501) staff       (20)      745 2023-09-25 19:06:58.000000 b3denv-0.0.9/setup.py
```

### Comparing `b3denv-0.0.8/LICENSE` & `b3denv-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `b3denv-0.0.8/README.md` & `b3denv-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `b3denv-0.0.8/b3denv/__init__.py` & `b3denv-0.0.9/b3denv/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,20 +21,23 @@
         try:
             p1 = subprocess.Popen(["which", "python"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             out, err = p1.communicate()
             which_python = out.strip()
             p2 = subprocess.Popen([which_python, "-c", "import sysconfig;print(sysconfig.get_config_var('installed_base'))"], stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             out, err = p2.communicate()
             installed_base = out.strip()
+            if isinstance(installed_base, bytes):
+                installed_base = installed_base.decode("utf-8")
+            #print("Installed base", installed_base)
             if on_mac():
                 d1 = os.path.dirname(os.path.dirname(os.path.dirname(os.path.dirname(installed_base))))
                 if "Blender" in os.path.basename(d1):
                     blender = d1
         except Exception as e:
-            print("failed", e)
+            #print("failed", e)
             pass
     
     if not blender:
         if on_mac():
             blender = "/Applications/Blender.app/"
         elif on_windows():
             folder = "C:\\Program Files\\Blender Foundation"
@@ -253,15 +256,15 @@
 
 def for_alias(s):
     if on_windows():
         s = '"' + os.path.abspath(s).replace('\\', '/') + '"'
         s = s.replace("C:", "/c")
     return s
 
-version = "0.0.8"
+version = "0.0.9"
 
 def print_header():
     print(
 """ _   ___   _             
 | |_|_  |_| |___ ___ _ _ 
 | . |_  | . | -_|   | | |
 |___|___|___|___|_|_|\_/ v""" + version)
@@ -274,15 +277,16 @@
     arg_count = len(argv)
     
     for a in argv:
         args.append(a)
     
     if arg_count == 2:
         if "-v" in args or "--version" in args:
-            return version
+            print(version)
+            return
 
     if arg_count == 1:
         print_header()
         return
 
     action = args[1]
```

### Comparing `b3denv-0.0.8/setup.py` & `b3denv-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ### Help with setting up bpy/blender/blender addons
 
 More info available at: [coldtype.xyz](https://coldtype.xyz)
 """
 
 setuptools.setup(
     name="b3denv",
-    version="0.0.8",
+    version="0.0.9",
     author="Rob Stenson / Coldtype",
     author_email="rob@goodhertz.com",
     description="Help with blender python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/coldtype/b3denv",
     packages=[
```

