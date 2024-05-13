# Comparing `tmp/pystratum_cli-2.0.0.tar.gz` & `tmp/pystratum_cli-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystratum_cli-2.0.0.tar", last modified: Mon May 13 10:05:27 2024, max compression
+gzip compressed data, was "pystratum_cli-2.0.1.tar", last modified: Mon May 13 10:29:09 2024, max compression
```

## Comparing `pystratum_cli-2.0.0.tar` & `pystratum_cli-2.0.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1096 2017-03-05 12:09:12.000000 pystratum_cli-2.0.0/LICENSE.md
--rw-r--r--   0        0        0     3855 2024-05-13 09:37:05.994052 pystratum_cli-2.0.0/README.rst
--rw-r--r--   0        0        0     1274 2024-05-13 10:05:27.903219 pystratum_cli-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      180 2024-05-12 15:21:38.895655 pystratum_cli-2.0.0/pystratum_cli/__init__.py
--rw-r--r--   0        0        0     1531 2024-05-13 09:55:11.302661 pystratum_cli-2.0.0/pystratum_cli/application/StratumApplication.py
--rw-r--r--   0        0        0        0 2020-10-15 09:29:54.000000 pystratum_cli-2.0.0/pystratum_cli/application/__init__.py
--rw-r--r--   0        0        0     2647 2024-05-13 09:00:12.573550 pystratum_cli-2.0.0/pystratum_cli/command/BaseCommand.py
--rw-r--r--   0        0        0     1097 2024-05-12 10:42:15.210261 pystratum_cli-2.0.0/pystratum_cli/command/ConstantsCommand.py
--rw-r--r--   0        0        0     1360 2024-05-12 10:41:44.694601 pystratum_cli-2.0.0/pystratum_cli/command/RoutineLoaderCommand.py
--rw-r--r--   0        0        0     1271 2024-05-13 09:13:32.679046 pystratum_cli-2.0.0/pystratum_cli/command/RoutineWrapperCommand.py
--rw-r--r--   0        0        0     1463 2024-05-12 10:28:53.917977 pystratum_cli-2.0.0/pystratum_cli/command/StratumCommand.py
--rw-r--r--   0        0        0        0 2016-07-27 08:24:17.000000 pystratum_cli-2.0.0/pystratum_cli/command/__init__.py
--rw-r--r--   0        0        0     2732 2024-05-13 09:13:45.837332 pystratum_cli-2.0.0/test/Application/StratumApplicationNoneTest.py
--rw-r--r--   0        0        0     2867 2024-05-12 10:42:45.269912 pystratum_cli-2.0.0/test/Application/StratumApplicationVoidTest.py
--rw-r--r--   0        0        0        0 2020-10-15 08:05:44.000000 pystratum_cli-2.0.0/test/Application/__init__.py
--rw-r--r--   0        0        0      138 2020-10-15 08:54:14.000000 pystratum_cli-2.0.0/test/Backend/NoneBackend.py
--rw-r--r--   0        0        0     2430 2024-05-12 10:40:17.874724 pystratum_cli-2.0.0/test/Backend/VoidBackend.py
--rw-r--r--   0        0        0        0 2020-10-15 08:03:14.000000 pystratum_cli-2.0.0/test/Backend/__init__.py
--rw-r--r--   0        0        0     1002 2024-05-12 10:36:26.867737 pystratum_cli-2.0.0/test/Worker/VoidConstantWorker.py
--rw-r--r--   0        0        0     1197 2024-05-12 10:40:17.870723 pystratum_cli-2.0.0/test/Worker/VoidRoutineLoaderWorker.py
--rw-r--r--   0        0        0     1057 2024-05-12 10:40:58.385598 pystratum_cli-2.0.0/test/Worker/VoidRoutineWrapperGeneratorWorker.py
--rw-r--r--   0        0        0        0 2020-10-15 08:54:37.000000 pystratum_cli-2.0.0/test/Worker/__init__.py
--rw-r--r--   0        0        0        0 2016-07-27 08:24:17.000000 pystratum_cli-2.0.0/test/__init__.py
--rw-r--r--   0        0        0     7882 2024-05-13 09:14:19.143057 pystratum_cli-2.0.0/test/coverage.xml
--rw-r--r--   0        0        0       28 2020-10-15 09:15:54.000000 pystratum_cli-2.0.0/test/etc/credentials.cfg
--rw-r--r--   0        0        0       57 2020-10-15 08:54:14.000000 pystratum_cli-2.0.0/test/etc/none.cfg
--rw-r--r--   0        0        0       98 2020-10-15 09:14:09.000000 pystratum_cli-2.0.0/test/etc/void.cfg
--rw-r--r--   0        0        0    19445 2024-05-13 09:14:19.063055 pystratum_cli-2.0.0/test/html/coverage_html.js
--rw-r--r--   0        0        0    14286 2024-05-12 10:02:51.975233 pystratum_cli-2.0.0/test/html/d_39050f025938d602_StratumApplication_py.html
--rw-r--r--   0        0        0     4784 2024-05-12 10:02:51.976233 pystratum_cli-2.0.0/test/html/d_39050f025938d602___init___py.html
--rw-r--r--   0        0        0     6621 2024-05-12 10:02:51.973233 pystratum_cli-2.0.0/test/html/d_a07595fffca26847___init___py.html
--rw-r--r--   0        0        0    26415 2024-05-12 10:02:51.981233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_BaseCommand_py.html
--rw-r--r--   0        0        0    11658 2024-05-12 10:02:51.983233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_ConstantsCommand_py.html
--rw-r--r--   0        0        0    12394 2024-05-12 10:02:51.985233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_RoutineLoaderCommand_py.html
--rw-r--r--   0        0        0    11752 2024-05-12 10:02:51.987233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_RoutineWrapperCommand_py.html
--rw-r--r--   0        0        0    16264 2024-05-12 10:02:51.989233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_StratumCommand_py.html
--rw-r--r--   0        0        0     4712 2024-05-12 10:02:51.990233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822___init___py.html
--rw-r--r--   0        0        0     1732 2024-05-13 09:14:19.063055 pystratum_cli-2.0.0/test/html/favicon_32.png
--rw-r--r--   0        0        0     6355 2024-05-13 09:14:19.061055 pystratum_cli-2.0.0/test/html/index.html
--rw-r--r--   0        0        0      731 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/jquery.ba-throttle-debounce.min.js
--rw-r--r--   0        0        0     3065 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/jquery.hotkeys.js
--rw-r--r--   0        0        0     1502 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/jquery.isonscreen.js
--rw-r--r--   0        0        0    95785 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/jquery.min.js
--rw-r--r--   0        0        0    12795 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/jquery.tablesorter.min.js
--rw-r--r--   0        0        0      112 2024-05-13 09:14:19.063055 pystratum_cli-2.0.0/test/html/keybd_closed.png
--rw-r--r--   0        0        0      112 2024-05-13 09:14:19.063055 pystratum_cli-2.0.0/test/html/keybd_open.png
--rw-r--r--   0        0        0     4586 2024-05-13 09:13:47.082359 pystratum_cli-2.0.0/test/html/pystratum_cli___init___py.html
--rw-r--r--   0        0        0    14042 2024-05-13 09:13:47.086360 pystratum_cli-2.0.0/test/html/pystratum_cli_application_StratumApplication_py.html
--rw-r--r--   0        0        0     2693 2024-05-13 09:13:47.087360 pystratum_cli-2.0.0/test/html/pystratum_cli_application___init___py.html
--rw-r--r--   0        0        0    23484 2024-05-13 09:13:47.092360 pystratum_cli-2.0.0/test/html/pystratum_cli_command_BaseCommand_py.html
--rw-r--r--   0        0        0    10469 2024-05-13 09:13:47.094360 pystratum_cli-2.0.0/test/html/pystratum_cli_command_ConstantsCommand_py.html
--rw-r--r--   0        0        0    11682 2024-05-13 09:13:47.097360 pystratum_cli-2.0.0/test/html/pystratum_cli_command_RoutineLoaderCommand_py.html
--rw-r--r--   0        0        0    10860 2024-05-13 09:13:47.100360 pystratum_cli-2.0.0/test/html/pystratum_cli_command_RoutineWrapperCommand_py.html
--rw-r--r--   0        0        0    15079 2024-05-13 09:13:47.103360 pystratum_cli-2.0.0/test/html/pystratum_cli_command_StratumCommand_py.html
--rw-r--r--   0        0        0     2685 2024-05-13 09:13:47.104360 pystratum_cli-2.0.0/test/html/pystratum_cli_command___init___py.html
--rw-r--r--   0        0        0     2280 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/status.json
--rw-r--r--   0        0        0    11692 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/style.css
--rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 pystratum_cli-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1096 2017-03-05 12:09:12.000000 pystratum_cli-2.0.1/LICENSE.md
+-rw-r--r--   0        0        0     3855 2024-05-13 09:37:05.994052 pystratum_cli-2.0.1/README.rst
+-rw-r--r--   0        0        0     1242 2024-05-13 10:29:09.179489 pystratum_cli-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      180 2024-05-12 15:21:38.895655 pystratum_cli-2.0.1/pystratum_cli/__init__.py
+-rw-r--r--   0        0        0     1531 2024-05-13 10:29:04.599388 pystratum_cli-2.0.1/pystratum_cli/application/StratumApplication.py
+-rw-r--r--   0        0        0        0 2020-10-15 09:29:54.000000 pystratum_cli-2.0.1/pystratum_cli/application/__init__.py
+-rw-r--r--   0        0        0     2647 2024-05-13 09:00:12.573550 pystratum_cli-2.0.1/pystratum_cli/command/BaseCommand.py
+-rw-r--r--   0        0        0     1097 2024-05-12 10:42:15.210261 pystratum_cli-2.0.1/pystratum_cli/command/ConstantsCommand.py
+-rw-r--r--   0        0        0     1360 2024-05-12 10:41:44.694601 pystratum_cli-2.0.1/pystratum_cli/command/RoutineLoaderCommand.py
+-rw-r--r--   0        0        0     1271 2024-05-13 09:13:32.679046 pystratum_cli-2.0.1/pystratum_cli/command/RoutineWrapperCommand.py
+-rw-r--r--   0        0        0     1463 2024-05-12 10:28:53.917977 pystratum_cli-2.0.1/pystratum_cli/command/StratumCommand.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:17.000000 pystratum_cli-2.0.1/pystratum_cli/command/__init__.py
+-rw-r--r--   0        0        0     2732 2024-05-13 09:13:45.837332 pystratum_cli-2.0.1/test/Application/StratumApplicationNoneTest.py
+-rw-r--r--   0        0        0     2867 2024-05-12 10:42:45.269912 pystratum_cli-2.0.1/test/Application/StratumApplicationVoidTest.py
+-rw-r--r--   0        0        0        0 2020-10-15 08:05:44.000000 pystratum_cli-2.0.1/test/Application/__init__.py
+-rw-r--r--   0        0        0      138 2020-10-15 08:54:14.000000 pystratum_cli-2.0.1/test/Backend/NoneBackend.py
+-rw-r--r--   0        0        0     2430 2024-05-12 10:40:17.874724 pystratum_cli-2.0.1/test/Backend/VoidBackend.py
+-rw-r--r--   0        0        0        0 2020-10-15 08:03:14.000000 pystratum_cli-2.0.1/test/Backend/__init__.py
+-rw-r--r--   0        0        0     1002 2024-05-12 10:36:26.867737 pystratum_cli-2.0.1/test/Worker/VoidConstantWorker.py
+-rw-r--r--   0        0        0     1197 2024-05-12 10:40:17.870723 pystratum_cli-2.0.1/test/Worker/VoidRoutineLoaderWorker.py
+-rw-r--r--   0        0        0     1057 2024-05-12 10:40:58.385598 pystratum_cli-2.0.1/test/Worker/VoidRoutineWrapperGeneratorWorker.py
+-rw-r--r--   0        0        0        0 2020-10-15 08:54:37.000000 pystratum_cli-2.0.1/test/Worker/__init__.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:17.000000 pystratum_cli-2.0.1/test/__init__.py
+-rw-r--r--   0        0        0     7882 2024-05-13 09:14:19.143057 pystratum_cli-2.0.1/test/coverage.xml
+-rw-r--r--   0        0        0       28 2020-10-15 09:15:54.000000 pystratum_cli-2.0.1/test/etc/credentials.cfg
+-rw-r--r--   0        0        0       57 2020-10-15 08:54:14.000000 pystratum_cli-2.0.1/test/etc/none.cfg
+-rw-r--r--   0        0        0       98 2020-10-15 09:14:09.000000 pystratum_cli-2.0.1/test/etc/void.cfg
+-rw-r--r--   0        0        0    19445 2024-05-13 09:14:19.063055 pystratum_cli-2.0.1/test/html/coverage_html.js
+-rw-r--r--   0        0        0    14286 2024-05-12 10:02:51.975233 pystratum_cli-2.0.1/test/html/d_39050f025938d602_StratumApplication_py.html
+-rw-r--r--   0        0        0     4784 2024-05-12 10:02:51.976233 pystratum_cli-2.0.1/test/html/d_39050f025938d602___init___py.html
+-rw-r--r--   0        0        0     6621 2024-05-12 10:02:51.973233 pystratum_cli-2.0.1/test/html/d_a07595fffca26847___init___py.html
+-rw-r--r--   0        0        0    26415 2024-05-12 10:02:51.981233 pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822_BaseCommand_py.html
+-rw-r--r--   0        0        0    11658 2024-05-12 10:02:51.983233 pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822_ConstantsCommand_py.html
+-rw-r--r--   0        0        0    12394 2024-05-12 10:02:51.985233 pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822_RoutineLoaderCommand_py.html
+-rw-r--r--   0        0        0    11752 2024-05-12 10:02:51.987233 pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822_RoutineWrapperCommand_py.html
+-rw-r--r--   0        0        0    16264 2024-05-12 10:02:51.989233 pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822_StratumCommand_py.html
+-rw-r--r--   0        0        0     4712 2024-05-12 10:02:51.990233 pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822___init___py.html
+-rw-r--r--   0        0        0     1732 2024-05-13 09:14:19.063055 pystratum_cli-2.0.1/test/html/favicon_32.png
+-rw-r--r--   0        0        0     6355 2024-05-13 09:14:19.061055 pystratum_cli-2.0.1/test/html/index.html
+-rw-r--r--   0        0        0      731 2024-05-13 09:14:19.062055 pystratum_cli-2.0.1/test/html/jquery.ba-throttle-debounce.min.js
+-rw-r--r--   0        0        0     3065 2024-05-13 09:14:19.062055 pystratum_cli-2.0.1/test/html/jquery.hotkeys.js
+-rw-r--r--   0        0        0     1502 2024-05-13 09:14:19.062055 pystratum_cli-2.0.1/test/html/jquery.isonscreen.js
+-rw-r--r--   0        0        0    95785 2024-05-13 09:14:19.062055 pystratum_cli-2.0.1/test/html/jquery.min.js
+-rw-r--r--   0        0        0    12795 2024-05-13 09:14:19.062055 pystratum_cli-2.0.1/test/html/jquery.tablesorter.min.js
+-rw-r--r--   0        0        0      112 2024-05-13 09:14:19.063055 pystratum_cli-2.0.1/test/html/keybd_closed.png
+-rw-r--r--   0        0        0      112 2024-05-13 09:14:19.063055 pystratum_cli-2.0.1/test/html/keybd_open.png
+-rw-r--r--   0        0        0     4586 2024-05-13 09:13:47.082359 pystratum_cli-2.0.1/test/html/pystratum_cli___init___py.html
+-rw-r--r--   0        0        0    14042 2024-05-13 09:13:47.086360 pystratum_cli-2.0.1/test/html/pystratum_cli_application_StratumApplication_py.html
+-rw-r--r--   0        0        0     2693 2024-05-13 09:13:47.087360 pystratum_cli-2.0.1/test/html/pystratum_cli_application___init___py.html
+-rw-r--r--   0        0        0    23484 2024-05-13 09:13:47.092360 pystratum_cli-2.0.1/test/html/pystratum_cli_command_BaseCommand_py.html
+-rw-r--r--   0        0        0    10469 2024-05-13 09:13:47.094360 pystratum_cli-2.0.1/test/html/pystratum_cli_command_ConstantsCommand_py.html
+-rw-r--r--   0        0        0    11682 2024-05-13 09:13:47.097360 pystratum_cli-2.0.1/test/html/pystratum_cli_command_RoutineLoaderCommand_py.html
+-rw-r--r--   0        0        0    10860 2024-05-13 09:13:47.100360 pystratum_cli-2.0.1/test/html/pystratum_cli_command_RoutineWrapperCommand_py.html
+-rw-r--r--   0        0        0    15079 2024-05-13 09:13:47.103360 pystratum_cli-2.0.1/test/html/pystratum_cli_command_StratumCommand_py.html
+-rw-r--r--   0        0        0     2685 2024-05-13 09:13:47.104360 pystratum_cli-2.0.1/test/html/pystratum_cli_command___init___py.html
+-rw-r--r--   0        0        0     2280 2024-05-13 09:14:19.062055 pystratum_cli-2.0.1/test/html/status.json
+-rw-r--r--   0        0        0    11692 2024-05-13 09:14:19.062055 pystratum_cli-2.0.1/test/html/style.css
+-rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 pystratum_cli-2.0.1/PKG-INFO
```

### Comparing `pystratum_cli-2.0.0/LICENSE.md` & `pystratum_cli-2.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/README.rst` & `pystratum_cli-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/pyproject.toml` & `pystratum_cli-2.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "PyStratum-Cli"
-version = "2.0.0"
+version = "2.0.1"
 description = "PyStratum Cli: The frontend of PyStratum"
 keywords = [
     "PyStratum",
     "CLI",
 ]
 readme = "README.rst"
 authors = [
@@ -31,26 +31,24 @@
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/DatabaseStratum/py-stratum-cli"
 
+[project.scripts]
+pystratum = "pystratum_cli:main"
+
 [project.optional-dependencies]
 dev = [
     "build~=1.2.1",
     "coverage~=5.3",
     "twine~=5.0.0",
 ]
 
-[options.entry_points]
-console_scripts = [
-    "pystratum = pystratum_cli:main",
-]
-
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [tool]
```

### Comparing `pystratum_cli-2.0.0/pystratum_cli/application/StratumApplication.py` & `pystratum_cli-2.0.1/pystratum_cli/application/StratumApplication.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     """
 
     # ------------------------------------------------------------------------------------------------------------------
     def __init__(self):
         """
         Object constructor
         """
-        Application.__init__(self, 'pystratum', '2.0.0')
+        Application.__init__(self, 'pystratum', '2.0.1')
 
         self.add(ConstantsCommand())
         self.add(RoutineLoaderCommand())
         self.add(StratumCommand())
         self.add(RoutineWrapperCommand())
 
     # ------------------------------------------------------------------------------------------------------------------
```

### Comparing `pystratum_cli-2.0.0/pystratum_cli/command/BaseCommand.py` & `pystratum_cli-2.0.1/pystratum_cli/command/BaseCommand.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/pystratum_cli/command/ConstantsCommand.py` & `pystratum_cli-2.0.1/pystratum_cli/command/ConstantsCommand.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/pystratum_cli/command/RoutineLoaderCommand.py` & `pystratum_cli-2.0.1/pystratum_cli/command/RoutineLoaderCommand.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/pystratum_cli/command/RoutineWrapperCommand.py` & `pystratum_cli-2.0.1/pystratum_cli/command/RoutineWrapperCommand.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/pystratum_cli/command/StratumCommand.py` & `pystratum_cli-2.0.1/pystratum_cli/command/StratumCommand.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/Application/StratumApplicationNoneTest.py` & `pystratum_cli-2.0.1/test/Application/StratumApplicationNoneTest.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/Application/StratumApplicationVoidTest.py` & `pystratum_cli-2.0.1/test/Application/StratumApplicationVoidTest.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/Backend/VoidBackend.py` & `pystratum_cli-2.0.1/test/Backend/VoidBackend.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/Worker/VoidConstantWorker.py` & `pystratum_cli-2.0.1/test/Worker/VoidConstantWorker.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/Worker/VoidRoutineLoaderWorker.py` & `pystratum_cli-2.0.1/test/Worker/VoidRoutineLoaderWorker.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/Worker/VoidRoutineWrapperGeneratorWorker.py` & `pystratum_cli-2.0.1/test/Worker/VoidRoutineWrapperGeneratorWorker.py`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/coverage.xml` & `pystratum_cli-2.0.1/test/coverage.xml`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/coverage_html.js` & `pystratum_cli-2.0.1/test/html/coverage_html.js`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/d_39050f025938d602_StratumApplication_py.html` & `pystratum_cli-2.0.1/test/html/d_39050f025938d602_StratumApplication_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/d_39050f025938d602___init___py.html` & `pystratum_cli-2.0.1/test/html/d_39050f025938d602___init___py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/d_a07595fffca26847___init___py.html` & `pystratum_cli-2.0.1/test/html/d_a07595fffca26847___init___py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_BaseCommand_py.html` & `pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822_BaseCommand_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_ConstantsCommand_py.html` & `pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822_ConstantsCommand_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_RoutineLoaderCommand_py.html` & `pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822_RoutineLoaderCommand_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_RoutineWrapperCommand_py.html` & `pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822_RoutineWrapperCommand_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_StratumCommand_py.html` & `pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822_StratumCommand_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822___init___py.html` & `pystratum_cli-2.0.1/test/html/d_f2c028ab8bfec822___init___py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/favicon_32.png` & `pystratum_cli-2.0.1/test/html/favicon_32.png`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/index.html` & `pystratum_cli-2.0.1/test/html/index.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/jquery.ba-throttle-debounce.min.js` & `pystratum_cli-2.0.1/test/html/jquery.ba-throttle-debounce.min.js`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/jquery.hotkeys.js` & `pystratum_cli-2.0.1/test/html/jquery.hotkeys.js`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/jquery.isonscreen.js` & `pystratum_cli-2.0.1/test/html/jquery.isonscreen.js`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/jquery.min.js` & `pystratum_cli-2.0.1/test/html/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/jquery.tablesorter.min.js` & `pystratum_cli-2.0.1/test/html/jquery.tablesorter.min.js`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/pystratum_cli___init___py.html` & `pystratum_cli-2.0.1/test/html/pystratum_cli___init___py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/pystratum_cli_application_StratumApplication_py.html` & `pystratum_cli-2.0.1/test/html/pystratum_cli_application_StratumApplication_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/pystratum_cli_application___init___py.html` & `pystratum_cli-2.0.1/test/html/pystratum_cli_application___init___py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/pystratum_cli_command_BaseCommand_py.html` & `pystratum_cli-2.0.1/test/html/pystratum_cli_command_BaseCommand_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/pystratum_cli_command_ConstantsCommand_py.html` & `pystratum_cli-2.0.1/test/html/pystratum_cli_command_ConstantsCommand_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/pystratum_cli_command_RoutineLoaderCommand_py.html` & `pystratum_cli-2.0.1/test/html/pystratum_cli_command_RoutineLoaderCommand_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/pystratum_cli_command_RoutineWrapperCommand_py.html` & `pystratum_cli-2.0.1/test/html/pystratum_cli_command_RoutineWrapperCommand_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/pystratum_cli_command_StratumCommand_py.html` & `pystratum_cli-2.0.1/test/html/pystratum_cli_command_StratumCommand_py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/pystratum_cli_command___init___py.html` & `pystratum_cli-2.0.1/test/html/pystratum_cli_command___init___py.html`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/status.json` & `pystratum_cli-2.0.1/test/html/status.json`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/test/html/style.css` & `pystratum_cli-2.0.1/test/html/style.css`

 * *Files identical despite different names*

### Comparing `pystratum_cli-2.0.0/PKG-INFO` & `pystratum_cli-2.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyStratum-Cli
-Version: 2.0.0
+Version: 2.0.1
 Summary: PyStratum Cli: The frontend of PyStratum
 Keywords: PyStratum,CLI
 Author-Email: Set Based IT Consultancy <info@setbased.nl>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

