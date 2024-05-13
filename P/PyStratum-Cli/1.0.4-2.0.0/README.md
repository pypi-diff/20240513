# Comparing `tmp/PyStratum-Cli-1.0.4.tar.gz` & `tmp/pystratum_cli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PyStratum-Cli-1.0.4.tar", last modified: Mon Oct 26 11:27:26 2020, max compression
+gzip compressed data, was "pystratum_cli-2.0.0.tar", last modified: Mon May 13 10:05:27 2024, max compression
```

## Comparing `PyStratum-Cli-1.0.4.tar` & `pystratum_cli-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,58 @@
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 11:27:26.977824 PyStratum-Cli-1.0.4/
--rw-rw-r--   0 water     (1000) water     (1000)     4804 2020-10-26 11:27:26.977824 PyStratum-Cli-1.0.4/PKG-INFO
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 11:27:26.975824 PyStratum-Cli-1.0.4/PyStratum_Cli.egg-info/
--rw-rw-r--   0 water     (1000) water     (1000)     4804 2020-10-26 11:27:26.000000 PyStratum-Cli-1.0.4/PyStratum_Cli.egg-info/PKG-INFO
--rw-rw-r--   0 water     (1000) water     (1000)      951 2020-10-26 11:27:26.000000 PyStratum-Cli-1.0.4/PyStratum_Cli.egg-info/SOURCES.txt
--rw-rw-r--   0 water     (1000) water     (1000)        1 2020-10-26 11:27:26.000000 PyStratum-Cli-1.0.4/PyStratum_Cli.egg-info/dependency_links.txt
--rw-rw-r--   0 water     (1000) water     (1000)       50 2020-10-26 11:27:26.000000 PyStratum-Cli-1.0.4/PyStratum_Cli.egg-info/entry_points.txt
--rw-rw-r--   0 water     (1000) water     (1000)       40 2020-10-26 11:27:26.000000 PyStratum-Cli-1.0.4/PyStratum_Cli.egg-info/requires.txt
--rw-rw-r--   0 water     (1000) water     (1000)       19 2020-10-26 11:27:26.000000 PyStratum-Cli-1.0.4/PyStratum_Cli.egg-info/top_level.txt
--rw-rw-r--   0 water     (1000) water     (1000)     3855 2020-10-15 10:35:05.000000 PyStratum-Cli-1.0.4/README.rst
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 11:27:26.975824 PyStratum-Cli-1.0.4/pystratum_cli/
--rw-rw-r--   0 water     (1000) water     (1000)      180 2020-10-15 09:30:00.000000 PyStratum-Cli-1.0.4/pystratum_cli/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 11:27:26.975824 PyStratum-Cli-1.0.4/pystratum_cli/application/
--rw-rw-r--   0 water     (1000) water     (1000)     1341 2020-10-26 11:27:17.000000 PyStratum-Cli-1.0.4/pystratum_cli/application/StratumApplication.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-15 09:29:54.000000 PyStratum-Cli-1.0.4/pystratum_cli/application/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 11:27:26.976824 PyStratum-Cli-1.0.4/pystratum_cli/command/
--rw-rw-r--   0 water     (1000) water     (1000)     2828 2020-10-15 21:34:39.000000 PyStratum-Cli-1.0.4/pystratum_cli/command/BaseCommand.py
--rw-rw-r--   0 water     (1000) water     (1000)      962 2020-10-15 09:36:19.000000 PyStratum-Cli-1.0.4/pystratum_cli/command/ConstantsCommand.py
--rw-rw-r--   0 water     (1000) water     (1000)     1125 2020-10-15 09:36:19.000000 PyStratum-Cli-1.0.4/pystratum_cli/command/RoutineLoaderCommand.py
--rw-rw-r--   0 water     (1000) water     (1000)     1038 2020-10-15 09:36:19.000000 PyStratum-Cli-1.0.4/pystratum_cli/command/RoutineWrapperCommand.py
--rw-rw-r--   0 water     (1000) water     (1000)     1328 2020-10-15 09:36:19.000000 PyStratum-Cli-1.0.4/pystratum_cli/command/StratumCommand.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2016-07-27 08:24:17.000000 PyStratum-Cli-1.0.4/pystratum_cli/command/__init__.py
--rw-rw-r--   0 water     (1000) water     (1000)       38 2020-10-26 11:27:26.977824 PyStratum-Cli-1.0.4/setup.cfg
--rw-rw-r--   0 water     (1000) water     (1000)     1325 2020-10-26 11:27:17.000000 PyStratum-Cli-1.0.4/setup.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 11:27:26.974824 PyStratum-Cli-1.0.4/test/
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 11:27:26.976824 PyStratum-Cli-1.0.4/test/Application/
--rw-rw-r--   0 water     (1000) water     (1000)     3064 2020-10-15 09:04:39.000000 PyStratum-Cli-1.0.4/test/Application/StratumApplicationNoneTest.py
--rw-rw-r--   0 water     (1000) water     (1000)     3199 2020-10-15 09:11:15.000000 PyStratum-Cli-1.0.4/test/Application/StratumApplicationVoidTest.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-15 08:05:44.000000 PyStratum-Cli-1.0.4/test/Application/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 11:27:26.977824 PyStratum-Cli-1.0.4/test/Backend/
--rw-rw-r--   0 water     (1000) water     (1000)      138 2020-10-15 08:54:14.000000 PyStratum-Cli-1.0.4/test/Backend/NoneBackend.py
--rw-rw-r--   0 water     (1000) water     (1000)     2654 2020-10-15 09:39:41.000000 PyStratum-Cli-1.0.4/test/Backend/VoidBackend.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-15 08:03:14.000000 PyStratum-Cli-1.0.4/test/Backend/__init__.py
-drwxrwxr-x   0 water     (1000) water     (1000)        0 2020-10-26 11:27:26.977824 PyStratum-Cli-1.0.4/test/Worker/
--rw-rw-r--   0 water     (1000) water     (1000)     1014 2020-10-15 09:10:25.000000 PyStratum-Cli-1.0.4/test/Worker/VoidConstantWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)     1283 2020-10-15 09:10:25.000000 PyStratum-Cli-1.0.4/test/Worker/VoidRoutineLoaderWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)     1089 2020-10-15 09:10:25.000000 PyStratum-Cli-1.0.4/test/Worker/VoidRoutineWrapperGeneratorWorker.py
--rw-rw-r--   0 water     (1000) water     (1000)        0 2020-10-15 08:54:37.000000 PyStratum-Cli-1.0.4/test/Worker/__init__.py
+-rw-r--r--   0        0        0     1096 2017-03-05 12:09:12.000000 pystratum_cli-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     3855 2024-05-13 09:37:05.994052 pystratum_cli-2.0.0/README.rst
+-rw-r--r--   0        0        0     1274 2024-05-13 10:05:27.903219 pystratum_cli-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      180 2024-05-12 15:21:38.895655 pystratum_cli-2.0.0/pystratum_cli/__init__.py
+-rw-r--r--   0        0        0     1531 2024-05-13 09:55:11.302661 pystratum_cli-2.0.0/pystratum_cli/application/StratumApplication.py
+-rw-r--r--   0        0        0        0 2020-10-15 09:29:54.000000 pystratum_cli-2.0.0/pystratum_cli/application/__init__.py
+-rw-r--r--   0        0        0     2647 2024-05-13 09:00:12.573550 pystratum_cli-2.0.0/pystratum_cli/command/BaseCommand.py
+-rw-r--r--   0        0        0     1097 2024-05-12 10:42:15.210261 pystratum_cli-2.0.0/pystratum_cli/command/ConstantsCommand.py
+-rw-r--r--   0        0        0     1360 2024-05-12 10:41:44.694601 pystratum_cli-2.0.0/pystratum_cli/command/RoutineLoaderCommand.py
+-rw-r--r--   0        0        0     1271 2024-05-13 09:13:32.679046 pystratum_cli-2.0.0/pystratum_cli/command/RoutineWrapperCommand.py
+-rw-r--r--   0        0        0     1463 2024-05-12 10:28:53.917977 pystratum_cli-2.0.0/pystratum_cli/command/StratumCommand.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:17.000000 pystratum_cli-2.0.0/pystratum_cli/command/__init__.py
+-rw-r--r--   0        0        0     2732 2024-05-13 09:13:45.837332 pystratum_cli-2.0.0/test/Application/StratumApplicationNoneTest.py
+-rw-r--r--   0        0        0     2867 2024-05-12 10:42:45.269912 pystratum_cli-2.0.0/test/Application/StratumApplicationVoidTest.py
+-rw-r--r--   0        0        0        0 2020-10-15 08:05:44.000000 pystratum_cli-2.0.0/test/Application/__init__.py
+-rw-r--r--   0        0        0      138 2020-10-15 08:54:14.000000 pystratum_cli-2.0.0/test/Backend/NoneBackend.py
+-rw-r--r--   0        0        0     2430 2024-05-12 10:40:17.874724 pystratum_cli-2.0.0/test/Backend/VoidBackend.py
+-rw-r--r--   0        0        0        0 2020-10-15 08:03:14.000000 pystratum_cli-2.0.0/test/Backend/__init__.py
+-rw-r--r--   0        0        0     1002 2024-05-12 10:36:26.867737 pystratum_cli-2.0.0/test/Worker/VoidConstantWorker.py
+-rw-r--r--   0        0        0     1197 2024-05-12 10:40:17.870723 pystratum_cli-2.0.0/test/Worker/VoidRoutineLoaderWorker.py
+-rw-r--r--   0        0        0     1057 2024-05-12 10:40:58.385598 pystratum_cli-2.0.0/test/Worker/VoidRoutineWrapperGeneratorWorker.py
+-rw-r--r--   0        0        0        0 2020-10-15 08:54:37.000000 pystratum_cli-2.0.0/test/Worker/__init__.py
+-rw-r--r--   0        0        0        0 2016-07-27 08:24:17.000000 pystratum_cli-2.0.0/test/__init__.py
+-rw-r--r--   0        0        0     7882 2024-05-13 09:14:19.143057 pystratum_cli-2.0.0/test/coverage.xml
+-rw-r--r--   0        0        0       28 2020-10-15 09:15:54.000000 pystratum_cli-2.0.0/test/etc/credentials.cfg
+-rw-r--r--   0        0        0       57 2020-10-15 08:54:14.000000 pystratum_cli-2.0.0/test/etc/none.cfg
+-rw-r--r--   0        0        0       98 2020-10-15 09:14:09.000000 pystratum_cli-2.0.0/test/etc/void.cfg
+-rw-r--r--   0        0        0    19445 2024-05-13 09:14:19.063055 pystratum_cli-2.0.0/test/html/coverage_html.js
+-rw-r--r--   0        0        0    14286 2024-05-12 10:02:51.975233 pystratum_cli-2.0.0/test/html/d_39050f025938d602_StratumApplication_py.html
+-rw-r--r--   0        0        0     4784 2024-05-12 10:02:51.976233 pystratum_cli-2.0.0/test/html/d_39050f025938d602___init___py.html
+-rw-r--r--   0        0        0     6621 2024-05-12 10:02:51.973233 pystratum_cli-2.0.0/test/html/d_a07595fffca26847___init___py.html
+-rw-r--r--   0        0        0    26415 2024-05-12 10:02:51.981233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_BaseCommand_py.html
+-rw-r--r--   0        0        0    11658 2024-05-12 10:02:51.983233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_ConstantsCommand_py.html
+-rw-r--r--   0        0        0    12394 2024-05-12 10:02:51.985233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_RoutineLoaderCommand_py.html
+-rw-r--r--   0        0        0    11752 2024-05-12 10:02:51.987233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_RoutineWrapperCommand_py.html
+-rw-r--r--   0        0        0    16264 2024-05-12 10:02:51.989233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822_StratumCommand_py.html
+-rw-r--r--   0        0        0     4712 2024-05-12 10:02:51.990233 pystratum_cli-2.0.0/test/html/d_f2c028ab8bfec822___init___py.html
+-rw-r--r--   0        0        0     1732 2024-05-13 09:14:19.063055 pystratum_cli-2.0.0/test/html/favicon_32.png
+-rw-r--r--   0        0        0     6355 2024-05-13 09:14:19.061055 pystratum_cli-2.0.0/test/html/index.html
+-rw-r--r--   0        0        0      731 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/jquery.ba-throttle-debounce.min.js
+-rw-r--r--   0        0        0     3065 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/jquery.hotkeys.js
+-rw-r--r--   0        0        0     1502 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/jquery.isonscreen.js
+-rw-r--r--   0        0        0    95785 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/jquery.min.js
+-rw-r--r--   0        0        0    12795 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/jquery.tablesorter.min.js
+-rw-r--r--   0        0        0      112 2024-05-13 09:14:19.063055 pystratum_cli-2.0.0/test/html/keybd_closed.png
+-rw-r--r--   0        0        0      112 2024-05-13 09:14:19.063055 pystratum_cli-2.0.0/test/html/keybd_open.png
+-rw-r--r--   0        0        0     4586 2024-05-13 09:13:47.082359 pystratum_cli-2.0.0/test/html/pystratum_cli___init___py.html
+-rw-r--r--   0        0        0    14042 2024-05-13 09:13:47.086360 pystratum_cli-2.0.0/test/html/pystratum_cli_application_StratumApplication_py.html
+-rw-r--r--   0        0        0     2693 2024-05-13 09:13:47.087360 pystratum_cli-2.0.0/test/html/pystratum_cli_application___init___py.html
+-rw-r--r--   0        0        0    23484 2024-05-13 09:13:47.092360 pystratum_cli-2.0.0/test/html/pystratum_cli_command_BaseCommand_py.html
+-rw-r--r--   0        0        0    10469 2024-05-13 09:13:47.094360 pystratum_cli-2.0.0/test/html/pystratum_cli_command_ConstantsCommand_py.html
+-rw-r--r--   0        0        0    11682 2024-05-13 09:13:47.097360 pystratum_cli-2.0.0/test/html/pystratum_cli_command_RoutineLoaderCommand_py.html
+-rw-r--r--   0        0        0    10860 2024-05-13 09:13:47.100360 pystratum_cli-2.0.0/test/html/pystratum_cli_command_RoutineWrapperCommand_py.html
+-rw-r--r--   0        0        0    15079 2024-05-13 09:13:47.103360 pystratum_cli-2.0.0/test/html/pystratum_cli_command_StratumCommand_py.html
+-rw-r--r--   0        0        0     2685 2024-05-13 09:13:47.104360 pystratum_cli-2.0.0/test/html/pystratum_cli_command___init___py.html
+-rw-r--r--   0        0        0     2280 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/status.json
+-rw-r--r--   0        0        0    11692 2024-05-13 09:14:19.062055 pystratum_cli-2.0.0/test/html/style.css
+-rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 pystratum_cli-2.0.0/PKG-INFO
```

### Comparing `PyStratum-Cli-1.0.4/README.rst` & `pystratum_cli-2.0.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 PyStratum CLI
 =============
 The frontend of PyStratum.
 
 +-----------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------+
 | Social                                                                                                                      | Release                                                                                            | Tests                                                                                               | Code                                                                                                     |
 +=============================================================================================================================+====================================================================================================+=====================================================================================================+==========================================================================================================+
-| .. image:: https://badges.gitter.im/SetBased/py-stratum.svg                                                                 | .. image:: https://badge.fury.io/py/PyStratum-Cli.svg                                              | .. image:: https://travis-ci.org/DatabaseStratum/py-stratum-cli.svg?branch=master                   | .. image:: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-cli/badges/quality-score.png?b=master |
-|   :target: https://gitter.im/SetBased/py-stratum?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge  |   :target: https://badge.fury.io/py/PyStratum-Cli                                                  |   :target: https://travis-ci.org/DatabaseStratum/py-stratum-cli                                     |   :target: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-cli/?branch=master                    |
-|                                                                                                                             |                                                                                                    | .. image:: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-cli/badges/coverage.png?b=master |                                                                                                          |
-|                                                                                                                             |                                                                                                    |   :target: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-cli/?branch=master               |                                                                                                          |
+| .. image:: https://badges.gitter.im/SetBased/py-stratum.svg                                                                 | .. image:: https://badge.fury.io/py/PyStratum-Cli.svg                                              | .. image:: https://github.com/DatabaseStratum/py-stratum-cli/actions/workflows/unit.yml/badge.svg   | .. image:: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-cli/badges/quality-score.png?b=master |
+|   :target: https://gitter.im/SetBased/py-stratum?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge  |   :target: https://badge.fury.io/py/PyStratum-Cli                                                  |   :target: https://github.com/DatabaseStratum/py-stratum-cli/actions/workflows/unit.yml             |   :target: https://scrutinizer-ci.com/g/DatabaseStratum/py-stratum-cli/?branch=master                    |
+|                                                                                                                             |                                                                                                    | .. image:: https://codecov.io/gh/DatabaseStratum/py-stratum-cli/branch/master/graph/badge.svg       |                                                                                                          |
+|                                                                                                                             |                                                                                                    |   :target: https://codecov.io/gh/DatabaseStratum/py-stratum-cli                                     |                                                                                                          |
 +-----------------------------------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------+-----------------------------------------------------------------------------------------------------+----------------------------------------------------------------------------------------------------------+
 
 Overview
 ========
 PyStratum is a tool and library for loading and invoking stored procedures from Python code.
 
 The documentation of PyStratum is available at https://stratum.readthedocs.io/.
```

### Comparing `PyStratum-Cli-1.0.4/pystratum_cli/command/BaseCommand.py` & `pystratum_cli-2.0.0/pystratum_cli/command/BaseCommand.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
 from configparser import ConfigParser
+from typing import Optional
 
-from cleo import Command, Input, Output
+from cleo.commands.command import Command
+from cleo.io.io import IO
 from pystratum_backend.Backend import Backend
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 
 class BaseCommand(Command):
     """
     Base command for other commands of PyStratum.
     """
 
@@ -17,23 +19,19 @@
         Object constructor.
         """
         super().__init__()
 
         self._config = ConfigParser()
         """
         The configuration object.
-
-        :type: ConfigParser 
         """
 
-        self._io = None
+        self._io: Optional[StratumIO] = None
         """
         The Output decorator.
-
-        :type: StratumStyle|None 
         """
 
     # ------------------------------------------------------------------------------------------------------------------
     def _create_backend_factory(self) -> Backend:
         """
         Creates the PyStratum Style object.
         """
@@ -44,42 +42,38 @@
         module = __import__(module_name)
         for comp in parts[1:]:
             module = getattr(module, comp)
 
         return module()
 
     # ------------------------------------------------------------------------------------------------------------------
-    def _read_config_file(self, input_object: Input) -> None:
+    def _read_config_file(self) -> None:
         """
         Reads the PyStratum configuration file.
 
         :rtype: ConfigParser
         """
-        config_filename = input_object.get_argument('config_file')
+        config_filename = self.argument('config_file')
         self._config.read(config_filename)
 
         if 'database' in self._config and 'supplement' in self._config['database']:
             path = os.path.join(os.path.dirname(config_filename), self._config.get('database', 'supplement'))
             config_supplement = ConfigParser()
             config_supplement.read(path)
 
             if 'database' in config_supplement:
                 options = config_supplement.options('database')
                 for option in options:
                     self._config['database'][option] = config_supplement['database'][option]
 
     # ------------------------------------------------------------------------------------------------------------------
-    def execute(self, input_object: Input, output_object: Output) -> int:
+    def execute(self, io: IO) -> int:
         """
         Executes this command.
 
-        :param input_object:  The input object.
-        :param output_object: The output object.
+        :param io: The input/output object.
         """
-        self.input = input_object
-        self.output = output_object
-
-        self._io = StratumStyle(input_object, output_object)
+        self._io = StratumIO(io.input, io.output, io.error_output)
 
         return self.handle()
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Cli-1.0.4/pystratum_cli/command/ConstantsCommand.py` & `pystratum_cli-2.0.0/pystratum_cli/command/ConstantsCommand.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from cleo.helpers import argument
+
 from pystratum_cli.command.BaseCommand import BaseCommand
 
 
 class ConstantsCommand(BaseCommand):
     """
     Generates constants based on database IDs.
-
-    constants
-        {config_file : The stratum configuration file}
     """
+    name = 'constants'
+    description = 'Generates constants based on database IDs.'
+    arguments = [argument(name='config_file', description='The stratum configuration file.')]
 
     # ------------------------------------------------------------------------------------------------------------------
     def handle(self) -> int:
         """
         Executes constants command when StratumCommand is activated.
         """
-        self._read_config_file(self.input)
+        self._read_config_file()
 
         factory = self._create_backend_factory()
         worker = factory.create_constant_worker(self._config, self._io)
 
         if not worker:
             self._io.title('Constants')
             self._io.error('Constants command is not implemented by the backend')
```

### Comparing `PyStratum-Cli-1.0.4/pystratum_cli/command/RoutineLoaderCommand.py` & `pystratum_cli-2.0.0/pystratum_cli/command/RoutineWrapperCommand.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,32 @@
+from cleo.helpers import argument
+
 from pystratum_cli.command.BaseCommand import BaseCommand
 
 
-class RoutineLoaderCommand(BaseCommand):
+class RoutineWrapperCommand(BaseCommand):
     """
-    Command for loading stored routines into a database instance from pseudo SQL files.
-
-    loader
-        {config_file : The audit configuration file}
-        {file_names?* : Sources with stored routines}
+    Command for generating a class with wrapper methods for invoking stored routines in a database instance.
     """
+    name = 'wrapper'
+    description = ('Command for generating a class with wrapper methods for invoking stored routines in a database '
+                   'instance.')
+    arguments = [argument(name='config_file', description='The stratum configuration file.')]
 
     # ------------------------------------------------------------------------------------------------------------------
     def handle(self) -> int:
         """
         Executes constants command when StratumCommand is activated.
         """
-        self._read_config_file(self.input)
+        self._read_config_file()
 
         factory = self._create_backend_factory()
-        worker = factory.create_routine_loader_worker(self._config, self._io)
-        file_names = self.input.get_argument('file_names')
+        worker = factory.create_routine_wrapper_generator_worker(self._config, self._io)
 
         if not worker:
-            self._io.title('Loader')
-            self._io.error('Loader command is not implemented by the backend')
+            self._io.title('Wrapper')
+            self._io.error('<error>Wrapper command is not implemented by the backend</>')
             return -1
 
-        return worker.execute(file_names)
+        return worker.execute()
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Cli-1.0.4/test/Application/StratumApplicationNoneTest.py` & `pystratum_cli-2.0.0/test/Application/StratumApplicationNoneTest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from cleo import CommandTester
+from cleo.testers.command_tester import CommandTester
 
 from pystratum_cli import StratumApplication
 
 
 class StratumApplicationNoneTest(TestCase):
     """
     Test with the none backend.
@@ -15,66 +15,62 @@
         """
         Test stratum command with none backend.
         """
         application = StratumApplication()
 
         command = application.find('stratum')
         command_tester = CommandTester(command)
-        status = command_tester.execute([('command', command.get_name()),
-                                         ('config_file', 'test/etc/none.cfg')])
-        output = command_tester.get_display()
+        status = command_tester.execute('test/etc/none.cfg')
+        output = command_tester.io.fetch_output()
 
         self.assertEqual(0, status)
         self.assertEqual('', output)
 
     # ------------------------------------------------------------------------------------------------------------------
     def test_command_constants(self) -> None:
         """
         Test constants command with none backend.
         """
         application = StratumApplication()
 
-        command = application.find('constant')
+        command = application.find('constants')
         command_tester = CommandTester(command)
-        status = command_tester.execute([('command', command.get_name()),
-                                         ('config_file', 'test/etc/none.cfg')])
-        output = command_tester.get_display()
+        status = command_tester.execute('test/etc/none.cfg')
+        output = command_tester.io.fetch_output()
 
         self.assertEqual(-1, status)
         self.assertIn('Constants', output)
         self.assertIn('ERROR', output)
 
     # ------------------------------------------------------------------------------------------------------------------
     def test_command_loader(self) -> None:
         """
         Test constants command with none backend.
         """
         application = StratumApplication()
 
         command = application.find('loader')
         command_tester = CommandTester(command)
-        status = command_tester.execute([('command', command.get_name()),
-                                         ('config_file', 'test/etc/none.cfg')])
-        output = command_tester.get_display()
+        status = command_tester.execute('test/etc/none.cfg')
+        output = command_tester.io.fetch_output()
 
         self.assertEqual(-1, status)
         self.assertIn('Loader', output)
         self.assertIn('ERROR', output)
 
     # ------------------------------------------------------------------------------------------------------------------
     def test_command_wrapper(self) -> None:
         """
         Test constants command with none backend.
         """
         application = StratumApplication()
 
         command = application.find('wrapper')
         command_tester = CommandTester(command)
-        status = command_tester.execute([('command', command.get_name()),
-                                         ('config_file', 'test/etc/none.cfg')])
-        output = command_tester.get_display()
+        status = command_tester.execute('test/etc/none.cfg')
+        output = command_tester.io.fetch_output()
 
         self.assertEqual(-1, status)
         self.assertIn('Wrapper', output)
         self.assertIn('ERROR', output)
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Cli-1.0.4/test/Application/StratumApplicationVoidTest.py` & `pystratum_cli-2.0.0/test/Application/StratumApplicationVoidTest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
 
-from cleo import CommandTester
+from cleo.testers.command_tester import CommandTester
 
 from pystratum_cli import StratumApplication
 
 
 class StratumApplicationVoidTest(TestCase):
     """
     Test with the void backend.
@@ -15,69 +15,65 @@
         """
         Test stratum command with void backend.
         """
         application = StratumApplication()
 
         command = application.find('stratum')
         command_tester = CommandTester(command)
-        status = command_tester.execute([('command', command.get_name()),
-                                         ('config_file', 'test/etc/void.cfg')])
-        output = command_tester.get_display()
+        status = command_tester.execute('test/etc/void.cfg')
+        output = command_tester.io.fetch_output()
 
         self.assertEqual(0, status)
         self.assertIn('Constants', output)
         self.assertIn('Loader', output)
         self.assertIn('Wrapper', output)
         self.assertNotIn('ERROR', output)
 
     # ------------------------------------------------------------------------------------------------------------------
     def test_command_constants(self) -> None:
         """
         Test constants command with void backend.
         """
         application = StratumApplication()
 
-        command = application.find('constant')
+        command = application.find('constants')
         command_tester = CommandTester(command)
-        status = command_tester.execute([('command', command.get_name()),
-                                         ('config_file', 'test/etc/void.cfg')])
-        output = command_tester.get_display()
+        status = command_tester.execute('test/etc/void.cfg')
+        output = command_tester.io.fetch_output()
 
         self.assertEqual(0, status)
         self.assertIn('Constants', output)
         self.assertNotIn('ERROR', output)
 
     # ------------------------------------------------------------------------------------------------------------------
     def test_command_loader(self) -> None:
         """
         Test constants command with void backend.
         """
         application = StratumApplication()
 
         command = application.find('loader')
         command_tester = CommandTester(command)
-        status = command_tester.execute([('command', command.get_name()),
-                                         ('config_file', 'test/etc/void.cfg')])
-        output = command_tester.get_display()
+        status = command_tester.execute('test/etc/void.cfg')
+        output = command_tester.io.fetch_output()
 
         self.assertEqual(0, status)
         self.assertIn('Loader', output)
         self.assertNotIn('ERROR', output)
 
     # ------------------------------------------------------------------------------------------------------------------
     def test_command_wrapper(self) -> None:
         """
         Test constants command with void backend.
         """
         application = StratumApplication()
 
         command = application.find('wrapper')
         command_tester = CommandTester(command)
-        status = command_tester.execute([('command', command.get_name()),
-                                         ('config_file', 'test/etc/void.cfg')])
-        output = command_tester.get_display()
+        status = command_tester.execute('test/etc/void.cfg')
+        output = command_tester.io.fetch_output()
 
         self.assertEqual(0, status)
         self.assertIn('Wrapper', output)
         self.assertNotIn('ERROR', output)
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Cli-1.0.4/test/Backend/VoidBackend.py` & `pystratum_cli-2.0.0/test/Backend/VoidBackend.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,57 +1,51 @@
 from configparser import ConfigParser
 from typing import Optional
 
 from pystratum_backend.Backend import Backend
 from pystratum_backend.ConstantWorker import ConstantWorker
 from pystratum_backend.RoutineLoaderWorker import RoutineLoaderWorker
 from pystratum_backend.RoutineWrapperGeneratorWorker import RoutineWrapperGeneratorWorker
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 from test.Worker.VoidConstantWorker import VoidConstantWorker
 from test.Worker.VoidRoutineLoaderWorker import VoidRoutineLoaderWorker
 from test.Worker.VoidRoutineWrapperGeneratorWorker import VoidRoutineWrapperGeneratorWorker
 
 
 class VoidBackend(Backend):
     """
     Backend with empty implementations.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def create_constant_worker(self, settings: ConfigParser, io: StratumStyle) -> Optional[ConstantWorker]:
+    def create_constant_worker(self, settings: ConfigParser, io: StratumIO) -> Optional[ConstantWorker]:
         """
         Creates the object that does the actual execution of the constant command for the backend.
 
-        :param ConfigParser settings: The settings from the PyStratum configuration file.
-        :param StratumStyle io: The output object.
-
-        :rtype: ConstantWorker|None
+        :param settings: The settings from the PyStratum configuration file.
+        :param io: The output object.
         """
         return VoidConstantWorker(io)
 
     # ------------------------------------------------------------------------------------------------------------------
-    def create_routine_loader_worker(self, settings: ConfigParser, io: StratumStyle) -> Optional[RoutineLoaderWorker]:
+    def create_routine_loader_worker(self, settings: ConfigParser, io: StratumIO) -> Optional[RoutineLoaderWorker]:
         """
         Creates the object that does the actual execution of the routine loader command for the backend.
 
-        :param ConfigParser settings: The settings from the PyStratum configuration file.
-        :param StratumStyle io: The output object.
-
-        :rtype: RoutineLoaderWorker|None
+        :param settings: The settings from the PyStratum configuration file.
+        :param io: The output object.
         """
         return VoidRoutineLoaderWorker(io)
 
     # ------------------------------------------------------------------------------------------------------------------
-    def create_routine_wrapper_generator_worker(self, settings: ConfigParser, io: StratumStyle) \
+    def create_routine_wrapper_generator_worker(self, settings: ConfigParser, io: StratumIO) \
             -> Optional[RoutineWrapperGeneratorWorker]:
         """
         Creates the object that does the actual execution of the routine wrapper generator command for the backend.
 
-        :param ConfigParser settings: The settings from the PyStratum configuration file.
-        :param StratumStyle io: The output object.
-
-        :rtype: RoutineWrapperGeneratorWorker|None
+        :param settings: The settings from the PyStratum configuration file.
+        :param io: The output object.
         """
         return VoidRoutineWrapperGeneratorWorker(io)
 
 # ----------------------------------------------------------------------------------------------------------------------
```

### Comparing `PyStratum-Cli-1.0.4/test/Worker/VoidConstantWorker.py` & `pystratum_cli-2.0.0/test/Worker/VoidConstantWorker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from pystratum_backend.ConstantWorker import ConstantWorker
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 
 class VoidConstantWorker(ConstantWorker):
     """
     Constant worker that does nothing.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle):
+    def __init__(self, io: StratumIO):
         """
         Object constructor.
 
         :param io: The Output decorator.
         """
-        self._io: StratumStyle = io
+        self._io: StratumIO = io
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute(self) -> int:
         """
         Does the actual execution of the constant command for the backend. Returns 0 on success. Otherwise returns
         nonzero.
```

### Comparing `PyStratum-Cli-1.0.4/test/Worker/VoidRoutineLoaderWorker.py` & `pystratum_cli-2.0.0/test/Worker/VoidRoutineLoaderWorker.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 from typing import List, Optional
 
 from pystratum_backend.RoutineLoaderWorker import RoutineLoaderWorker
-from pystratum_backend.StratumStyle import StratumStyle
+from pystratum_backend.StratumIO import StratumIO
 
 
 class VoidRoutineLoaderWorker(RoutineLoaderWorker):
     """
     Routine loader worker that does nothing.
     """
 
     # ------------------------------------------------------------------------------------------------------------------
-    def __init__(self, io: StratumStyle):
+    def __init__(self, io: StratumIO):
         """
         Object constructor.
 
         :param io: The Output decorator.
         """
-        self._io: StratumStyle = io
+        self._io: StratumIO = io
 
     # ------------------------------------------------------------------------------------------------------------------
     def execute(self, file_names: Optional[List[str]] = None) -> int:
         """
-        Does the actual execution of the routine loader command for the backend. Returns 0 on success. Otherwise
+        Does the actual execution of the routine loader command for the backend. Returns 0 on success. Otherwise,
         returns nonzero.
 
-        :param list[str]|None file_names: The sources that must be loaded. If none all sources (if required) will
-                                          loaded.
-
-        :rtype: int
+        :param file_names: The sources that must be loaded. If None all sources (if required) will be loaded.
         """
         self._io.title('Loader')
 
         return 0
 
 # ----------------------------------------------------------------------------------------------------------------------
```

