# Comparing `tmp/42-taskmaster-1.0.1.tar.gz` & `tmp/42_taskmaster-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "42-taskmaster-1.0.1.tar", last modified: Fri Apr  5 08:54:22 2024, max compression
+gzip compressed data, was "42_taskmaster-1.0.2.tar", last modified: Mon May 13 13:13:13 2024, max compression
```

## Comparing `42-taskmaster-1.0.1.tar` & `42_taskmaster-1.0.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/42_taskmaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 08:54:22.000000 42-taskmaster-1.0.1/42_taskmaster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.877982 42-taskmaster-1.0.1/taskmaster/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/taskmaster/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/_default.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/gui/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    28363 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/service.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3712 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/taskmaster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/taskmaster/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7963 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/utils/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/utils/log_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/taskmaster/utils/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 08:54:22.881981 42-taskmaster-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/tests/test_log_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    19039 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/tests/test_service_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-04-05 08:54:18.000000 42-taskmaster-1.0.1/tests/test_subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:13:13.213828 42_taskmaster-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:13:13.213828 42_taskmaster-1.0.2/42_taskmaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-13 13:13:13.000000 42_taskmaster-1.0.2/42_taskmaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-13 13:13:13.000000 42_taskmaster-1.0.2/42_taskmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:13:13.000000 42_taskmaster-1.0.2/42_taskmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-13 13:13:13.000000 42_taskmaster-1.0.2/42_taskmaster.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 13:13:13.000000 42_taskmaster-1.0.2/42_taskmaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 13:13:13.000000 42_taskmaster-1.0.2/42_taskmaster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-13 13:13:13.213828 42_taskmaster-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:13:13.213828 42_taskmaster-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:13:13.209828 42_taskmaster-1.0.2/taskmaster/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:13:13.213828 42_taskmaster-1.0.2/taskmaster/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/gui/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/gui/_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/gui/_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8944 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/gui/_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/gui/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/gui/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28681 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/service.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3764 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/taskmaster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:13:13.213828 42_taskmaster-1.0.2/taskmaster/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7963 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/utils/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/utils/log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/taskmaster/utils/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:13:13.213828 42_taskmaster-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/tests/test_log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19104 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/tests/test_service_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9201 2024-05-13 13:12:56.000000 42_taskmaster-1.0.2/tests/test_subprocess.py
```

### Comparing `42-taskmaster-1.0.1/42_taskmaster.egg-info/PKG-INFO` & `42_taskmaster-1.0.2/42_taskmaster.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: 42-taskmaster
-Version: 1.0.1
+Version: 1.0.2
 Summary: A process manager project for 42
 Author-email: Timothee Lafay <tlafay@student.42lyon.fr>, Theo Nard <tnard@student.42lyon.fr>
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Unix
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: Cerberus==1.3.5
 Requires-Dist: PyYAML==6.0.1
 
 <!-- PROJECT LOGO -->
 <br />
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1 Name: 42-taskmaster Version: 1.0.1 Summary: A process
+Metadata-Version: 2.1 Name: 42-taskmaster Version: 1.0.2 Summary: A process
 manager project for 42 Author-email: Timothee Lafay
 student.42lyon.fr>, Theo Nard
 student.42lyon.fr> Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.11 Description-Content-Type: text/markdown
-Requires-Dist: Cerberus==1.3.5 Requires-Dist: PyYAML==6.0.1
+Operating System :: Unix Requires-Python: >=3.11 Description-Content-Type:
+text/markdown Requires-Dist: Cerberus==1.3.5 Requires-Dist: PyYAML==6.0.1
                                     _[_L_o_g_o_]
                            ******** 4422 -- TTaasskkmmaasstteerr ********
                     Services management and monitoring tool
 ## About The Project Taskmaster is a job control manager project for 42 school.
 It allows its users to control a number of processes on operating systems.
 Inspired by the [Supervisor](https://github.com/Supervisor/supervisor) ###
 Prerequisites Create a virtual environment using the following command: * venv
```

### Comparing `42-taskmaster-1.0.1/42_taskmaster.egg-info/SOURCES.txt` & `42_taskmaster-1.0.2/42_taskmaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/PKG-INFO` & `42_taskmaster-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: 42-taskmaster
-Version: 1.0.1
+Version: 1.0.2
 Summary: A process manager project for 42
 Author-email: Timothee Lafay <tlafay@student.42lyon.fr>, Theo Nard <tnard@student.42lyon.fr>
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Unix
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: Cerberus==1.3.5
 Requires-Dist: PyYAML==6.0.1
 
 <!-- PROJECT LOGO -->
 <br />
```

#### html2text {}

```diff
@@ -1,14 +1,13 @@
-Metadata-Version: 2.1 Name: 42-taskmaster Version: 1.0.1 Summary: A process
+Metadata-Version: 2.1 Name: 42-taskmaster Version: 1.0.2 Summary: A process
 manager project for 42 Author-email: Timothee Lafay
 student.42lyon.fr>, Theo Nard
 student.42lyon.fr> Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.11 Description-Content-Type: text/markdown
-Requires-Dist: Cerberus==1.3.5 Requires-Dist: PyYAML==6.0.1
+Operating System :: Unix Requires-Python: >=3.11 Description-Content-Type:
+text/markdown Requires-Dist: Cerberus==1.3.5 Requires-Dist: PyYAML==6.0.1
                                     _[_L_o_g_o_]
                            ******** 4422 -- TTaasskkmmaasstteerr ********
                     Services management and monitoring tool
 ## About The Project Taskmaster is a job control manager project for 42 school.
 It allows its users to control a number of processes on operating systems.
 Inspired by the [Supervisor](https://github.com/Supervisor/supervisor) ###
 Prerequisites Create a virtual environment using the following command: * venv
```

### Comparing `42-taskmaster-1.0.1/README.md` & `42_taskmaster-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/pyproject.toml` & `42_taskmaster-1.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [project]
 
 name = "42-taskmaster"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name = "Timothee Lafay", email = "tlafay@student.42lyon.fr" },
     { name = "Theo Nard", email = "tnard@student.42lyon.fr" },
 ]
 description = "A process manager project for 42"
 requires-python = ">=3.11"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    "Operating System :: Unix",
 ]
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [tool.setuptools.packages.find]
```

### Comparing `42-taskmaster-1.0.1/taskmaster/gui/_configuration.py` & `42_taskmaster-1.0.2/taskmaster/gui/_configuration.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/taskmaster/gui/_default.py` & `42_taskmaster-1.0.2/taskmaster/gui/_default.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/taskmaster/gui/_log.py` & `42_taskmaster-1.0.2/taskmaster/gui/_log.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/taskmaster/gui/_services.py` & `42_taskmaster-1.0.2/taskmaster/gui/_services.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/taskmaster/gui/_utils.py` & `42_taskmaster-1.0.2/taskmaster/gui/_utils.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/taskmaster/gui/gui.py` & `42_taskmaster-1.0.2/taskmaster/gui/gui.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/taskmaster/gui/table.py` & `42_taskmaster-1.0.2/taskmaster/gui/table.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/taskmaster/service.py` & `42_taskmaster-1.0.2/taskmaster/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,24 +47,28 @@
         self._stdout = stdout
         self._stderr = stderr
         self._user = user
         self._env = env
         self._process: Process | None = None
         self._state: SubProcess.State = self.State.STOPPED
         self._retries: int = 0
+        self.__killing: bool = False
         self._email: Email | None = email
 
     async def delete(self) -> None:
         """
         Destructor for the SubProcess class.
         """
+        self.__killing = True
         try:
             if self._process and self._process.returncode is None:
+                logger.info(f"Terminating process {self._parent_name}")
                 self._process.terminate()
                 await self._process.wait()
+                logger.debug(f"Process {self._parent_name} terminated.")
         except ProcessLookupError as e:
             logger.error(f"Failed to terminate process {self._parent_name}: {e}")
 
     @property
     def state(self) -> State:
         """
         Gets the state of the subprocess.
@@ -160,14 +164,16 @@
                 f"Process {self._parent_name}-{self._process.pid} is already running."
             )
             return self
 
         success: bool = False
 
         while not success:
+            if self.__killing:
+                return self
             try:
                 if self._cmd is None:
                     raise ValueError("Command is not provided.")
                 self._process = await asyncio.create_subprocess_exec(
                     *self._cmd.split(),
                     cwd=self._workingdir,
                     env=self._env,
@@ -187,15 +193,17 @@
                     await asyncio.sleep(0.1)
                 if starttime == 0 or await self._poll() is None:
                     logger.info(
                         f"Process {self._parent_name}-{self._process.pid} is now running."
                     )
                     self._state = self.State.RUNNING
                     if self._email:
-                        asyncio.create_task(self._email.send_start(self._parent_name, self._state.name))
+                        asyncio.create_task(
+                            self._email.send_start(self._parent_name, self._state.name)
+                        )
                     success = True
                 else:
                     logger.error(
                         f"Process {self._parent_name}-{self._process.pid} has exited before {starttime} seconds."
                     )
                     retries -= 1
 
@@ -243,18 +251,22 @@
         )
         await self._process.wait()
         logger.info(f"Process {self._parent_name}-{self._process.pid} ended.")
         if self.retries > 0 and self.retries >= startretries:
             logger.error(f"{self._parent_name}: Max retry attempt exceeded")
             self.state = SubProcess.State.FATAL
         else:
-            logger.info(f"{self._parent_name}: Process exited with code {self._process.returncode}")
+            logger.info(
+                f"{self._parent_name}: Process exited with code {self._process.returncode}"
+            )
             self.state = SubProcess.State.EXITED
         if self._email:
-            asyncio.create_task(self._email.send_exited(self._parent_name, self._state.name))
+            asyncio.create_task(
+                self._email.send_exited(self._parent_name, self._state.name)
+            )
         return self
 
     async def stop(self, stopsignal: str | Signal, stoptime: int) -> Self:
         """
         Tries to stop the process using the given signal.
         If the process is not stopped after stoptime seconds, it will be killed
         """
@@ -274,15 +286,17 @@
         logger.info(f"Process {self._parent_name}: sending signal {stopsignal.name}")
         self._state = self.State.STOPPING
         for _ in range(stoptime * 10):
             await asyncio.sleep(0.1)
             if await self._poll():
                 break
         if not await self._poll():
-            logger.warning(f"Process {self._parent_name} unresponsive: killing forcefully")
+            logger.warning(
+                f"Process {self._parent_name} unresponsive: killing forcefully"
+            )
             self._process.kill()
         self.retries = 0
         self._state = self.State.STOPPED
         logger.info(f"Process {self._parent_name} stopped successfully.")
         if self._email:
             asyncio.create_task(
                 self._email.send_stop(self._parent_name, self._state.name)
@@ -302,14 +316,18 @@
         When a process is in the EXITED state, it will automatically restart:
         - never if its autorestart parameter is set to false.
         - unconditionally if its autorestart parameter is set to true.
         - conditionally if its autorestart parameter is set to unexpected.
             If it exited with an exit code that doesn't match one of the exit codes defined in the exitcodes
             configuration parameter for the process, it will be restarted.
         """
+
+        if self.__killing:
+            return self
+
         if self._process is None:
             logger.warning(f"Process {self._parent_name} is not running.")
             return self
 
         if self.state != self.State.EXITED:
             logger.warning(
                 f"Process {self._parent_name} with pid {self._process.pid} is not exited."
@@ -571,25 +589,24 @@
             )
             self._processes.append(subprocess)
 
     async def start(self) -> None:
         """
         Starts the service.
         """
-        for process in self._processes:
-            if (
-                process.state != SubProcess.State.RUNNING
-                and process.state != SubProcess.State.STARTING
-                and process.state != SubProcess.State.STOPPING
-            ):
-                if process._process:
-                    logger.debug(
-                        f"Removing process {process._parent_name} with pid {process._process.pid} from processes"
-                    )
-                self._processes.remove(process)
+        self._processes = [
+            process
+            for process in self._processes
+            if process.state
+            not in [
+                SubProcess.State.RUNNING,
+                SubProcess.State.STARTING,
+                SubProcess.State.STOPPING,
+            ]
+        ]
 
         self._create_subprocesses(num=self._config.numprocs - len(self._processes))
         self._start_tasks: List[asyncio.Task] = []
         self._wait_tasks: List[asyncio.Task] = []
         for process in self._processes:
             self._start_tasks += [
                 asyncio.create_task(
@@ -824,15 +841,17 @@
 
         config = dict(self._config)
 
         self._email = email
 
         # If the service is not in the new config, remove it
         for service in self._services.copy():
-            if service.config.name not in [service.get("name") for service in config["services"]]:
+            if service.config.name not in [
+                service.get("name") for service in config["services"]
+            ]:
                 tasks.append(asyncio.create_task(service.delete()))
                 self._services.remove(service)
 
         # If the service is still in the new config, update it
         for service in self._services:
             for service_config in config["services"]:
                 if service.config.name == service_config.get("name"):
@@ -841,15 +860,17 @@
                     break
 
         # If the service is not in the old config, add it
         for service_config in config["services"]:
             if service_config.get("name") not in [
                 service.config.name for service in self._services
             ]:
-                self._services.append(Service(email=self._email, **dict(service_config)))
+                self._services.append(
+                    Service(email=self._email, **dict(service_config))
+                )
 
         tasks.append(asyncio.create_task(self.autostart()))
         self._config = self.Config(**config)
         return self.config
 
     def flush(self, service_name: str) -> None:
         """
```

### Comparing `42-taskmaster-1.0.1/taskmaster/taskmaster.py` & `42_taskmaster-1.0.2/taskmaster/taskmaster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import curses
 import asyncio
 import signal
 import argparse
 from .utils.email import Email
 from typing import Any
+import os
 
 from .service import ServiceHandler
 
 from .utils.logger import logger
 from .gui.gui import Gui
 from .utils.config import Config, generate_config
 
@@ -31,14 +32,15 @@
     logger.info("Initializing signal handler.")
     signal.signal(signal.SIGINT, signal_handler)
     signal.signal(signal.SIGHUP, reload_config)
 
 
 async def interfaces(stdscr, config) -> None:
     logger.info("Starting taskmaster.")
+    logger.warning(f"PID: {os.getpid()}")
     global need_reload, need_exit
     try:
         if config.email:
             email = Email(config)
             asyncio.create_task(email.send("hello", "Taskmaster started."))
         else:
             email = None
```

### Comparing `42-taskmaster-1.0.1/taskmaster/utils/config.py` & `42_taskmaster-1.0.2/taskmaster/utils/config.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/taskmaster/utils/email.py` & `42_taskmaster-1.0.2/taskmaster/utils/email.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/taskmaster/utils/log_reader.py` & `42_taskmaster-1.0.2/taskmaster/utils/log_reader.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/taskmaster/utils/logger.py` & `42_taskmaster-1.0.2/taskmaster/utils/logger.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/tests/test_config.py` & `42_taskmaster-1.0.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/tests/test_log_reader.py` & `42_taskmaster-1.0.2/tests/test_log_reader.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/tests/test_service.py` & `42_taskmaster-1.0.2/tests/test_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,27 +273,21 @@
     async def test_start_when_stopping_doesnt_work(self):
         config = Config(
             "./tests/config_templates/valid/test_start_when_stopping.yml"
         ).services[0]
         service = Service(**config)
         asyncio.create_task(service.start())
         await asyncio.sleep(0.1)
-        self.assertEqual(
-            service.status.get("process_1"), SubProcess.State.RUNNING
-        )
+        self.assertEqual(service.status.get("process_1"), SubProcess.State.RUNNING)
         asyncio.create_task(service.stop())
         await asyncio.sleep(0.1)
-        self.assertEqual(
-            service.status.get("process_1"), SubProcess.State.STOPPING
-        )
+        self.assertEqual(service.status.get("process_1"), SubProcess.State.STOPPING)
         asyncio.create_task(service.start())
         await asyncio.sleep(0.1)
-        self.assertEqual(
-            service.status.get("process_1"), SubProcess.State.STOPPING
-        )
+        self.assertEqual(service.status.get("process_1"), SubProcess.State.RUNNING)
 
     async def test_reload_remove_subprocesses(self):
         config = Config("./tests/config_templates/valid/test_reload.yml").services[0]
         service = Service(**config)
         await service.start()
         await asyncio.sleep(0.1)
         self.assertEqual(service.status.get("process_1"), SubProcess.State.RUNNING)
@@ -327,43 +321,49 @@
         await asyncio.sleep(0.1)
         self.assertEqual(service.status.get("process_1"), SubProcess.State.RUNNING)
         service.config = config
         await service.reload()
         self.assertEqual(service.status.get("process_1"), SubProcess.State.RUNNING)
 
     async def test_send_email_on_start_one_proc(self):
-        config = Config("./tests/config_templates/valid/test_send_email.yml").services[0]
+        config = Config("./tests/config_templates/valid/test_send_email.yml").services[
+            0
+        ]
         email_mock = AsyncMock(name="taskmaster.utils.email.Email")
         with patch("taskmaster.utils.email.Email", email_mock):
             service = Service(email=email_mock, **config)
             await service.start()
             await asyncio.sleep(0.1)
             self.assertEqual(service.status.get("process_1"), SubProcess.State.RUNNING)
             self.assertEqual(email_mock.send_start.call_count, 1)
             email_mock.send_start.assert_called_with(
                 config.get("name"), SubProcess.State.RUNNING.name
             )
 
     async def test_send_email_on_start_multiple_procs(self):
-        config = Config("./tests/config_templates/valid/test_send_email.yml").services[0]
+        config = Config("./tests/config_templates/valid/test_send_email.yml").services[
+            0
+        ]
         config["numprocs"] = 8
         email_mock = AsyncMock(name="taskmaster.utils.email.Email")
         with patch("taskmaster.utils.email.Email", email_mock):
             service = Service(email=email_mock, **config)
             await service.start()
             await asyncio.sleep(0.1)
             self.assertEqual(service.status.get("process_1"), SubProcess.State.RUNNING)
             self.assertEqual(service.status.get("process_2"), SubProcess.State.RUNNING)
             self.assertEqual(email_mock.send_start.call_count, 8)
             email_mock.send_start.assert_called_with(
                 config.get("name"), SubProcess.State.RUNNING.name
             )
 
     async def test_send_email_on_stop_one_proc(self):
-        config = Config("./tests/config_templates/valid/test_send_email.yml").services[0]
+        config = Config("./tests/config_templates/valid/test_send_email.yml").services[
+            0
+        ]
         email_mock = AsyncMock(name="taskmaster.utils.email.Email")
         with patch("taskmaster.utils.email.Email", email_mock):
             service = Service(email=email_mock, **config)
             await service.start()
             await asyncio.sleep(0.1)
             self.assertEqual(service.status.get("process_1"), SubProcess.State.RUNNING)
             await service.stop()
@@ -371,15 +371,17 @@
             self.assertEqual(service.status.get("process_1"), SubProcess.State.STOPPED)
             self.assertEqual(email_mock.send_stop.call_count, 1)
             email_mock.send_stop.assert_called_with(
                 config.get("name"), SubProcess.State.STOPPED.name
             )
 
     async def test_send_email_on_stop_multiple_procs(self):
-        config = Config("./tests/config_templates/valid/test_send_email.yml").services[0]
+        config = Config("./tests/config_templates/valid/test_send_email.yml").services[
+            0
+        ]
         config["numprocs"] = 8
         email_mock = AsyncMock(name="taskmaster.utils.email.Email")
         with patch("taskmaster.utils.email.Email", email_mock):
             service = Service(email=email_mock, **config)
             await service.start()
             await asyncio.sleep(0.1)
             self.assertEqual(service.status.get("process_1"), SubProcess.State.RUNNING)
@@ -388,15 +390,17 @@
             self.assertEqual(service.status.get("process_1"), SubProcess.State.STOPPED)
             self.assertEqual(email_mock.send_stop.call_count, 8)
             email_mock.send_stop.assert_called_with(
                 config.get("name"), SubProcess.State.STOPPED.name
             )
 
     async def test_send_email_on_fatal_one_proc(self):
-        config = Config("./tests/config_templates/valid/test_send_email.yml").services[0]
+        config = Config("./tests/config_templates/valid/test_send_email.yml").services[
+            0
+        ]
         config["autorestart"] = "never"
         config["startretries"] = 0
         config["starttime"] = 10
         config["cmd"] = "dontexist"
         email_mock = AsyncMock(name="taskmaster.utils.email.Email")
         with patch("taskmaster.utils.email.Email", email_mock):
             service = Service(email=email_mock, **config)
@@ -405,15 +409,17 @@
             self.assertEqual(service.status.get("process_1"), SubProcess.State.FATAL)
             self.assertEqual(email_mock.send_exited.call_count, 1)
             email_mock.send_exited.assert_called_with(
                 config.get("name"), SubProcess.State.FATAL.name
             )
 
     async def test_send_email_on_fatal_multiple_procs(self):
-        config = Config("./tests/config_templates/valid/test_send_email.yml").services[0]
+        config = Config("./tests/config_templates/valid/test_send_email.yml").services[
+            0
+        ]
         config["numprocs"] = 8
         config["autorestart"] = "never"
         config["startretries"] = 0
         config["starttime"] = 10
         config["cmd"] = "dontexist"
         email_mock = AsyncMock(name="taskmaster.utils.email.Email")
         with patch("taskmaster.utils.email.Email", email_mock):
```

### Comparing `42-taskmaster-1.0.1/tests/test_service_handler.py` & `42_taskmaster-1.0.2/tests/test_service_handler.py`

 * *Files identical despite different names*

### Comparing `42-taskmaster-1.0.1/tests/test_subprocess.py` & `42_taskmaster-1.0.2/tests/test_subprocess.py`

 * *Files identical despite different names*

