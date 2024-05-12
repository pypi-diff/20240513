# Comparing `tmp/aioclock-0.0.6.tar.gz` & `tmp/aioclock-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioclock-0.0.6.tar", max compression
+gzip compressed data, was "aioclock-0.0.7.tar", max compression
```

## Comparing `aioclock-0.0.6.tar` & `aioclock-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2024-05-02 18:41:41.101644 aioclock-0.0.6/LICENSE
--rw-r--r--   0        0        0     3674 2024-05-02 18:41:41.101644 aioclock-0.0.6/README.md
--rw-r--r--   0        0        0      299 2024-05-02 18:41:41.101644 aioclock-0.0.6/aioclock/__init__.py
--rw-r--r--   0        0        0     2495 2024-05-02 18:41:41.101644 aioclock-0.0.6/aioclock/app.py
--rw-r--r--   0        0        0     1182 2024-05-02 18:41:41.101644 aioclock-0.0.6/aioclock/group.py
--rw-r--r--   0        0        0       55 2024-05-02 18:41:41.105644 aioclock-0.0.6/aioclock/logger.py
--rw-r--r--   0        0        0      122 2024-05-02 18:41:41.105644 aioclock-0.0.6/aioclock/provider.py
--rw-r--r--   0        0        0      800 2024-05-02 18:41:41.105644 aioclock-0.0.6/aioclock/task.py
--rw-r--r--   0        0        0     7712 2024-05-02 18:41:41.105644 aioclock-0.0.6/aioclock/triggers.py
--rw-r--r--   0        0        0     1042 2024-05-02 18:41:41.105644 aioclock-0.0.6/aioclock/types.py
--rw-r--r--   0        0        0      862 2024-05-02 18:41:41.105644 aioclock-0.0.6/aioclock/utils.py
--rw-r--r--   0        0        0     1966 2024-05-02 18:42:05.373782 aioclock-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4617 1970-01-01 00:00:00.000000 aioclock-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-12 22:38:17.081409 aioclock-0.0.7/LICENSE
+-rw-r--r--   0        0        0     3311 2024-05-12 22:38:17.081409 aioclock-0.0.7/README.md
+-rw-r--r--   0        0        0      299 2024-05-12 22:38:17.081409 aioclock-0.0.7/aioclock/__init__.py
+-rw-r--r--   0        0        0     4561 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/app.py
+-rw-r--r--   0        0        0     2146 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/group.py
+-rw-r--r--   0        0        0       55 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/logger.py
+-rw-r--r--   0        0        0      245 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/provider.py
+-rw-r--r--   0        0        0     1374 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/task.py
+-rw-r--r--   0        0        0    12544 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/triggers.py
+-rw-r--r--   0        0        0     1042 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/types.py
+-rw-r--r--   0        0        0      862 2024-05-12 22:38:17.085409 aioclock-0.0.7/aioclock/utils.py
+-rw-r--r--   0        0        0     2014 2024-05-12 22:38:39.689321 aioclock-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4254 1970-01-01 00:00:00.000000 aioclock-0.0.7/PKG-INFO
```

### Comparing `aioclock-0.0.6/LICENSE` & `aioclock-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.6/README.md` & `aioclock-0.0.7/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -15,26 +15,30 @@
 
 - Async: 100% Async, very light, fast and resource friendly
 - Scheduling: Keep scheduling tasks for yoo
 - Group: Group your task, for better code maintainability
 - Trigger: Already defined and easily extendable triggers, to trigger your scheduler to be started
 - Easy syntax: Library's syntax is very easy and enjoyable, no confusing hierarchy
 - Pydantic v2 validation: Validate all your trigger on startup using pydantic 2. Fastest to fail possible!
-- **Soon**: Processor handlers, with pub/sub logic.
+- **Soon**: Running the task dispatcher (scheduler) on different process by default, so CPU intensive stuff on task won't delay the scheduling
+- **Soon**: Backend support, to allow horizontal scalling, by synchronizing, maybe using Redis
 
 ## Getting started
 
 To Install aioclock, simply do
 
 ```
 pip install aioclock
 ```
 
-AioClock is very user friendly and easy to use, it's type stated library to use easily.
-AioClock always have a trigger, that trigger the events.
+## Help
+
+See [documentation](https://ManiMozaffar.github.io/aioclock/) for more details.
+
+## A Sample Example
 
 ```python
 import asyncio
 
 from aioclock import AioClock, At, Depends, Every, Forever, Once, OnShutDown, OnStartUp
 from aioclock.group import Group
 
@@ -87,17 +91,7 @@
     print("Going offline. Remember, if your code is running, you better go catch it!")
 
 
 # main.py
 if __name__ == "__main__":
     asyncio.run(app.serve())
 ```
-
-## TODOs
-
-Ideally, producer and consumer should be on seperate process.
-Because a function having CPU bound task, doesn't mean the task should be produced with delays.
-So AioClock is aiming to give the user ability to easily setup how many process they want to use, and by default use 2 process, where one is consumer and one is producer. Producer doesn't need to be more than 1 process, unless the trigger is CPU intensive.
-
-## Contribution
-
-Feel free to contribute, we welcome new ideas, bug fixes or anything!
```

### Comparing `aioclock-0.0.6/aioclock/group.py` & `aioclock-0.0.7/aioclock/group.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,17 +7,53 @@
 from aioclock.provider import get_provider
 from aioclock.task import Task
 from aioclock.triggers import BaseTrigger
 
 
 class Group:
     def __init__(self, *, tasks: Union[list[Task], None] = None):
+        """
+        Group of tasks that will be run together.
+
+        Best use case is to have a good modularity and separation of concerns.
+        For example, you can have a group of tasks that are responsible for sending emails.
+        And another group of tasks that are responsible for sending notifications.
+
+        Example:
+        ```python
+
+        from aioclock import Group, AioClock, Forever
+
+        email_group = Group()
+
+        # consider this as different file
+        @email_group.task(trigger=Forever())
+        async def send_email():
+            ...
+
+        # app.py
+        aio_clock = AioClock()
+        aio_clock.include_group(email_group)
+        ```
+
+        """
         self._tasks: list[Task] = tasks or []
 
     def task(self, *, trigger: BaseTrigger):
+        """Function used to decorate tasks, to be registered inside AioClock.
+
+        Example:
+        ```python
+        from aioclock import Group, Forever
+        @group.task(trigger=Forever())
+        async def send_email():
+            ...
+        ```
+        """
+
         def decorator(func: Callable[..., Any]) -> Callable[..., Any]:
             @wraps(func)
             async def wrapper(*args, **kwargs) -> Any:
                 return await func(*args, **kwargs)
 
             self._tasks.append(
                 Task(
```

### Comparing `aioclock-0.0.6/aioclock/types.py` & `aioclock-0.0.7/aioclock/types.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.6/aioclock/utils.py` & `aioclock-0.0.7/aioclock/utils.py`

 * *Files identical despite different names*

### Comparing `aioclock-0.0.6/pyproject.toml` & `aioclock-0.0.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aioclock"
-version = "0.0.6"
+version = "0.0.7"
 description = "An asyncio-based scheduling framework designed for execution of periodic task with integrated support for dependency injection, enabling efficient and flexiable task management"
 authors = ["Mani Mozaffar <fmani.mozaffar@gmail.com>"]
 repository = "https://github.com/ManiMozaffar/aioclock"
 documentation = "https://ManiMozaffar.github.io/aioclock/"
 readme = "README.md"
 packages = [{ include = "aioclock" }]
 
@@ -20,19 +20,20 @@
 rich = "^13.7.1"
 pyright = "1.1.350"
 
 [tool.pyright]
 typeCheckingMode = "basic"
 
 
-
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.2.7"
 mkdocstrings = { extras = ["python"], version = "^0.23.0" }
+mkdocs-simple-hooks = "^0.1.5"
+black = "^24.4.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.pytest.ini_options]
```

### Comparing `aioclock-0.0.6/PKG-INFO` & `aioclock-0.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioclock
-Version: 0.0.6
+Version: 0.0.7
 Summary: An asyncio-based scheduling framework designed for execution of periodic task with integrated support for dependency injection, enabling efficient and flexiable task management
 Home-page: https://github.com/ManiMozaffar/aioclock
 Author: Mani Mozaffar
 Author-email: fmani.mozaffar@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -35,26 +35,30 @@
 
 - Async: 100% Async, very light, fast and resource friendly
 - Scheduling: Keep scheduling tasks for yoo
 - Group: Group your task, for better code maintainability
 - Trigger: Already defined and easily extendable triggers, to trigger your scheduler to be started
 - Easy syntax: Library's syntax is very easy and enjoyable, no confusing hierarchy
 - Pydantic v2 validation: Validate all your trigger on startup using pydantic 2. Fastest to fail possible!
-- **Soon**: Processor handlers, with pub/sub logic.
+- **Soon**: Running the task dispatcher (scheduler) on different process by default, so CPU intensive stuff on task won't delay the scheduling
+- **Soon**: Backend support, to allow horizontal scalling, by synchronizing, maybe using Redis
 
 ## Getting started
 
 To Install aioclock, simply do
 
 ```
 pip install aioclock
 ```
 
-AioClock is very user friendly and easy to use, it's type stated library to use easily.
-AioClock always have a trigger, that trigger the events.
+## Help
+
+See [documentation](https://ManiMozaffar.github.io/aioclock/) for more details.
+
+## A Sample Example
 
 ```python
 import asyncio
 
 from aioclock import AioClock, At, Depends, Every, Forever, Once, OnShutDown, OnStartUp
 from aioclock.group import Group
 
@@ -108,17 +112,7 @@
 
 
 # main.py
 if __name__ == "__main__":
     asyncio.run(app.serve())
 ```
 
-## TODOs
-
-Ideally, producer and consumer should be on seperate process.
-Because a function having CPU bound task, doesn't mean the task should be produced with delays.
-So AioClock is aiming to give the user ability to easily setup how many process they want to use, and by default use 2 process, where one is consumer and one is producer. Producer doesn't need to be more than 1 process, unless the trigger is CPU intensive.
-
-## Contribution
-
-Feel free to contribute, we welcome new ideas, bug fixes or anything!
-
```

