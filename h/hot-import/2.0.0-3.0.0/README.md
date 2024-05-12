# Comparing `tmp/hot-import-2.0.0.tar.gz` & `tmp/hot-import-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hot-import-2.0.0.tar", last modified: Mon Dec  4 11:52:11 2023, max compression
+gzip compressed data, was "hot-import-3.0.0.tar", last modified: Sun May 12 22:08:55 2024, max compression
```

## Comparing `hot-import-2.0.0.tar` & `hot-import-3.0.0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-12-04 11:52:11.397552 hot-import-2.0.0/
--rw-rw-rw-   0        0        0     2235 2023-12-04 11:52:11.397552 hot-import-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1660 2023-12-04 11:50:20.000000 hot-import-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-12-04 11:52:11.387546 hot-import-2.0.0/hot_import/
--rw-rw-rw-   0        0        0       27 2023-12-03 22:27:06.000000 hot-import-2.0.0/hot_import/__init__.py
--rw-rw-rw-   0        0        0     8433 2023-12-04 11:39:57.000000 hot-import-2.0.0/hot_import/hot_import.py
-drwxrwxrwx   0        0        0        0 2023-12-04 11:52:11.395552 hot-import-2.0.0/hot_import.egg-info/
--rw-rw-rw-   0        0        0     2235 2023-12-04 11:52:11.000000 hot-import-2.0.0/hot_import.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-12-04 11:52:11.000000 hot-import-2.0.0/hot_import.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-04 11:52:11.000000 hot-import-2.0.0/hot_import.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-12-04 11:52:11.000000 hot-import-2.0.0/hot_import.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-12-04 11:52:11.000000 hot-import-2.0.0/hot_import.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-04 11:52:11.398545 hot-import-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1179 2023-12-04 11:51:30.000000 hot-import-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:08:55.387014 hot-import-3.0.0/
+-rw-rw-rw-   0        0        0     1143 2024-05-12 21:42:57.000000 hot-import-3.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1422 2024-05-12 22:08:55.386016 hot-import-3.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      816 2024-05-12 22:06:36.000000 hot-import-3.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-12 22:08:55.352130 hot-import-3.0.0/hot_import/
+-rw-rw-rw-   0        0        0       27 2023-12-03 22:42:50.000000 hot-import-3.0.0/hot_import/__init__.py
+-rw-rw-rw-   0        0        0     7533 2023-12-04 20:00:33.000000 hot-import-3.0.0/hot_import/hot_import.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:08:55.380015 hot-import-3.0.0/hot_import.egg-info/
+-rw-rw-rw-   0        0        0     1422 2024-05-12 22:08:55.000000 hot-import-3.0.0/hot_import.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-05-12 22:08:55.000000 hot-import-3.0.0/hot_import.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-12 22:08:55.000000 hot-import-3.0.0/hot_import.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-12 22:08:55.000000 hot-import-3.0.0/hot_import.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-12 22:08:55.000000 hot-import-3.0.0/hot_import.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-12 22:08:55.387014 hot-import-3.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2024-05-12 22:07:27.000000 hot-import-3.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-12 22:08:55.384015 hot-import-3.0.0/test_import/
+-rw-rw-rw-   0        0        0       21 2023-12-03 22:42:50.000000 hot-import-3.0.0/test_import/__init__.py
+-rw-rw-rw-   0        0        0      502 2024-05-12 21:47:02.000000 hot-import-3.0.0/test_import/test.py
```

### Comparing `hot-import-2.0.0/hot_import/hot_import.py` & `hot-import-3.0.0/hot_import/hot_import.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+# from easy_events import EasyEvents, Parameters
 from inspect import getmembers, getfile, ismethod, getsource
 
 import importlib, types
 
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 
 import sys, os
 
 import time, shutil
 
-
 class Mod:
     def __init__(self, functions: dict, name: str):
         for key, value in functions.items():
             setattr(self, key, value)
 
         setattr(self, "__name__", name)
 
@@ -65,15 +65,18 @@
                 new_mod = importlib.import_module(specific_module)
 
             dico = getmembers(new_mod)
             mod = specific_module.rsplit(".", 1)[-1]
             self.functions_mods[mod] = {dico[i][0]: dico[i][1] for i in range(len(dico))}
             self.functions = {**self.functions, **self.functions_mods[mod]}
 
-        if self.auto_update and self.module:
+        if not self.module:
+            self.module = Mod(self.functions, self.module_name)
+
+        elif self.auto_update:
             self.module.___update___(self.functions, self.module_name)
 
         else:
             self.module = Mod(self.functions, self.module_name)
 
     def import_code(self, code, module_name):
         module = types.ModuleType(module_name)
@@ -121,53 +124,37 @@
                 except Exception as e:
                     pass
 
         self._call_event(self.module)
 
 
 class HotImport():
-    def __init__(self, modules: list = [], auto_update: bool = True, globals=None):
-        self.modules_importer = {}
-        caller_module = sys._getframe(1).f_globals["__name__"]
-        self.modules_importer[caller_module] = sys.modules[caller_module]
-
-        self.globals = globals
+    def __init__(self, modules: list = [], auto_update: bool = True):
+        # EasyEvents.__init__(self, str_only=False, default_event=False)        
         self.modules = []
         self.functions = {}
-
         self.observer = Observer()
-        self.callback_function = None
-        self.ignore = [
-            "__builtins__", "__cached__", "__file__",
-            "__loader__", "__name__", "__package__",
-            "__spec__", "__path__", "__doc__"
-        ]
-
+        self.callback_function = self.modul_on_update
         observed = []
+        caller_module = sys._getframe(1).f_globals["__name__"]
+        self.module_importer = sys.modules[caller_module]
 
         for module in modules:
-            caller_module = None
-
             if not callable(module):
                 pat = os.path.abspath(module.__file__).replace("\\", "/").rsplit("/", 1)[0]
-                caller_module = sys._getframe(1).f_globals[module.__name__]
             else:
                 pat = getfile(module).replace("\\", "/").rsplit("/", 1)[0]
                 name = module.__module__.rsplit(".", 1)[0]
                 self.functions[f"{name}.{module.__name__}"] = module
-                caller_module = sys._getframe(1).f_globals[name]
 
             if pat not in observed:
                 event_handler = self.add_handler(Module(module, event_handler=self.call_event, auto_update=auto_update))
                 self.observer.schedule(event_handler, path=pat, recursive=True)
                 observed.append(pat)
 
-                if caller_module:
-                    self.modules_importer[caller_module.__name__] = sys.modules[caller_module.__name__]
-
         self.observer.start()
 
     def add_handler(self, handler: Module):
         self.modules.append(handler)
         return handler
 
     def get_module(self, module: str):
@@ -175,61 +162,45 @@
             module = module.__name__
 
         for mod in self.modules:
             if mod.module_name == module:
                 return mod.module
 
     def get_function(self, function: str):
-        for mod in self.modules:
-            if mod.functions.get(function.__name__):
-                return mod.functions.get(function.__name__)
+        mod = self.get_module(function.__module__.rsplit(".", 1)[0])
+        if mod:
+            return getattr(mod, function.__name__)
 
     def join_observer(self):
         self.observer.join()
 
     def stop_observer(self):
         self.observer.stop()
 
     def call_event(self, module):
-        self.module_on_update(module)
-
+        # self.functions[f"{module.__module__}.{module.__name__}"] = module
         if self.callback_function:
             self.callback_function(module)
 
     def on_update(self, callback: callable = None):
         def add_debug(func):
             self.callback_function = func
             return func
 
         if callable(callback):
             return add_debug(callback)
 
         return add_debug
+    
+    def modul_on_update(self, module:Mod):
+        module_imported = sys.modules[module.__name__]
 
-    def module_on_update(self, module):
-        """
-        updated = False
-        for k, v in self.modules_importer.items():
-            if k == module.__name__:
-                for new_name, new_var in module.__dict__.items():
-                    # if new_name not in self.ignore:
-                    mod =  self.modules_importer.get("__main__")
-
-                    print(vars(mod))
-                    vars(mod)[new_name] = new_var
-        """
-        for k, v in self.functions.items():
-            if k.startswith(f"{module.__name__}."):
-                new_name = k.rsplit(".", 1)[-1]
-                mod = self.modules_importer.get("__main__")
-                self.functions[k] = getattr(module, new_name)
-                vars(mod)[new_name] = self.functions[k]
-                # print(self.functions[k])
-
-        """
-        # self.globals[new_name] = self.functions[k]
-        for old_name in vars(self.module_importer).keys():
+        for old_name, f in vars(module_imported).items():
             old_func = old_name.split(".")[-1]
-            for new_name, new_var in vars(module).items():
+            for new_name, new_val in vars(module).items():
                 if old_func == new_name:
-                    vars(self.module_importer)[new_name] = new_var
-        """
+                    vars(module_imported)[new_name] = new_val
+                    for main_var, main_val in vars(self.module_importer).items():
+                        if main_val == f:
+                            vars(self.module_importer)[main_var] = new_val
+                        
+        #print(f"\nUpdated : {module.__name__}")
```

### Comparing `hot-import-2.0.0/setup.py` & `hot-import-3.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,36 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as stream:
     long_description = stream.read()
 
-# long_description = "An universal wrapper (and useful tool) to make event / commands in python"
-
 setup(
     name='hot-import',
-    version="2.0.0",
+    version="3.0.0",
     url='https://github.com/ThePhoenix78/hot-import',
     download_url='https://github.com/ThePhoenix78/hot-import/tarball/master',
     license='MIT',
-    author='ThePhoenix78',
+    author='ThePoenix78, GalTech',
     author_email='thephoenix788@gmail.com',
-    description='hot-reload for python packages ',
+    description='hot-reload for python packages',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=[
         "hot-reload",
         "live reload",
         "live update",
         "hot reload"
     ],
     install_requires=[
-        # "easy-events>=3.1.1",
         "watchdog"
     ],
     setup_requires=[
         'wheel'
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(),
-    # packages=["sdist", "bdist_wheel"]
-    python_requires='>=3.6',
+    python_requires='>=3.10',
 )
```

