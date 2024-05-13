# Comparing `tmp/botifyme-0.1.5.tar.gz` & `tmp/botifyme-0.1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botifyme-0.1.5.tar", max compression
+gzip compressed data, was "botifyme-0.1.5.1.tar", max compression
```

## Comparing `botifyme-0.1.5.tar` & `botifyme-0.1.5.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11357 2024-02-22 03:29:19.473931 botifyme-0.1.5/LICENSE
--rw-r--r--   0        0        0      443 2024-02-22 03:29:19.474338 botifyme-0.1.5/README.md
--rw-r--r--   0        0        0      162 2024-04-23 20:15:22.599781 botifyme-0.1.5/botifyme/__init__.py
--rw-r--r--   0        0        0     3116 2024-05-07 07:16:45.246003 botifyme-0.1.5/botifyme/__main__.py
--rw-r--r--   0        0        0     1438 2024-04-23 20:15:22.599920 botifyme-0.1.5/botifyme/agent.py
--rw-r--r--   0        0        0    11826 2024-05-04 06:02:47.291215 botifyme-0.1.5/botifyme/config.py
--rw-r--r--   0        0        0     1045 2024-02-22 03:29:19.476022 botifyme-0.1.5/botifyme/registry.py
--rw-r--r--   0        0        0     4075 2024-05-03 05:36:25.537048 botifyme-0.1.5/botifyme/runtime.py
--rw-r--r--   0        0        0      475 2024-04-23 20:15:22.600500 botifyme-0.1.5/botifyme/utils/__init__.py
--rw-r--r--   0        0        0     3533 2024-03-14 23:09:57.824589 botifyme-0.1.5/botifyme/utils/tools.py
--rw-r--r--   0        0        0     3640 2024-04-23 22:21:27.280737 botifyme-0.1.5/botifyme/workflow.py
--rw-r--r--   0        0        0      869 2024-05-07 07:17:12.262768 botifyme-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1594 1970-01-01 00:00:00.000000 botifyme-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-22 03:29:19.473931 botifyme-0.1.5.1/LICENSE
+-rw-r--r--   0        0        0      443 2024-02-22 03:29:19.474338 botifyme-0.1.5.1/README.md
+-rw-r--r--   0        0        0      176 2024-05-07 17:57:33.544067 botifyme-0.1.5.1/botifyme/__init__.py
+-rw-r--r--   0        0        0     3083 2024-05-07 17:09:06.222220 botifyme-0.1.5.1/botifyme/__main__.py
+-rw-r--r--   0        0        0     1438 2024-04-23 20:15:22.599920 botifyme-0.1.5.1/botifyme/agent.py
+-rw-r--r--   0        0        0     1128 2024-05-07 22:15:59.427766 botifyme-0.1.5.1/botifyme/cli/__init__.py
+-rw-r--r--   0        0        0    15349 2024-05-08 01:51:38.856042 botifyme-0.1.5.1/botifyme/config.py
+-rw-r--r--   0        0        0     1045 2024-02-22 03:29:19.476022 botifyme-0.1.5.1/botifyme/registry.py
+-rw-r--r--   0        0        0     4362 2024-05-07 22:25:37.073207 botifyme-0.1.5.1/botifyme/runtime.py
+-rw-r--r--   0        0        0      475 2024-04-23 20:15:22.600500 botifyme-0.1.5.1/botifyme/utils/__init__.py
+-rw-r--r--   0        0        0     3533 2024-03-14 23:09:57.824589 botifyme-0.1.5.1/botifyme/utils/tools.py
+-rw-r--r--   0        0        0     3640 2024-04-23 22:21:27.280737 botifyme-0.1.5.1/botifyme/workflow.py
+-rw-r--r--   0        0        0      872 2024-05-13 04:26:34.566131 botifyme-0.1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1547 1970-01-01 00:00:00.000000 botifyme-0.1.5.1/PKG-INFO
```

### Comparing `botifyme-0.1.5/LICENSE` & `botifyme-0.1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.5/botifyme/__main__.py` & `botifyme-0.1.5.1/botifyme/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,20 +34,19 @@
                 elif isinstance(output, str):
                     with open(
                         os.path.join(temp_dir, "output.txt"), "w", encoding="utf-8"
                     ) as f:
                         f.write(output)
 
             except Exception as e:
-                # with open(
-                #     os.path.join(temp_dir, "error.log"), "w", encoding="utf-8"
-                # ) as f:
-                #     f.write(str(e))
+                with open(
+                    os.path.join(temp_dir, "error.log"), "w", encoding="utf-8"
+                ) as f:
+                    f.write(str(e))
 
-                print(e)
                 return e
 
 
 def list_tools():
     """
     List all the tools that are available in the tool registry.
     """
```

### Comparing `botifyme-0.1.5/botifyme/agent.py` & `botifyme-0.1.5.1/botifyme/agent.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.5/botifyme/config.py` & `botifyme-0.1.5.1/botifyme/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 import functools
+import httpx
 from loguru import logger
 import inspect
-from typing import Any, Dict, Union, Callable, ParamSpec, TypeVar, List, Optional
+from typing import (
+    Any,
+    Dict,
+    Union,
+    Callable,
+    ParamSpec,
+    TypeVar,
+    List,
+    Optional,
+    get_origin,
+)
 from pydantic import BaseModel
 from docstring_parser import parse
 from slugify import slugify
 
+
 P = ParamSpec("P")
 R = TypeVar("R", bound=Callable[..., Any])
 
 workflow_registry: Dict[str, "WorkflowConfig"] = {}
 task_registry: Dict[str, Any] = {}
 tool_registry: Dict[str, "Tool"] = {}
 
@@ -230,34 +242,47 @@
         input_params.append(_param)
 
     # Parse output paramters from return type
     output_params: List[Param] = []
     return_annotation = sig.return_annotation
 
     if return_annotation != inspect.Signature.empty:
-        if issubclass(return_annotation, str):
-            _param = Param(
-                name="output",
-                description="The output of the function.",
-                data_type="string",
-                default_value="",
-                required=True,
-            )
-            output_params.append(_param)
 
-        elif issubclass(return_annotation, BaseModel):
-            for field_name, model_field in return_annotation.model_fields.items():
+        if inspect.isclass(return_annotation):
+            if issubclass(return_annotation, str):
+                _param = Param(
+                    name="output",
+                    description="The output of the function.",
+                    data_type="string",
+                    default_value="",
+                    required=True,
+                )
+                output_params.append(_param)
+
+            elif issubclass(return_annotation, BaseModel):
+                for field_name, model_field in return_annotation.model_fields.items():
+                    _param = Param(
+                        name=field_name,
+                        description="",
+                        data_type=get_json_datatype_from_python_type(
+                            model_field.annotation
+                        ),
+                        default_value=model_field.default,
+                        required=model_field.is_required(),
+                    )
+                    output_params.append(_param)
+
+        if get_origin(return_annotation) is not None:
+            if issubclass(get_origin(return_annotation), list):
                 _param = Param(
-                    name=field_name,
-                    description="",
-                    data_type=get_json_datatype_from_python_type(
-                        model_field.annotation
-                    ),
-                    default_value=model_field.default,
-                    required=model_field.is_required(),
+                    name="output",
+                    description="The output of the function.",
+                    data_type="array",
+                    default_value=[],
+                    required=True,
                 )
                 output_params.append(_param)
 
     func_details = {}
     func_details["name"] = func.__name__
     func_details["description"] = parsed_docstring.short_description
     func_details["input_params"] = input_params
@@ -354,16 +379,21 @@
 
 
 def execute_workflow_async(slug: str, kwargs: Dict[str, Any]) -> WorkflowRun:
 
     return WorkflowRun(id=slug, status="success")
 
 
-def execute_workflow(slug: str, *args, kwargs: Dict[str, Any], func) -> R:
-    return func(**kwargs)
+def execute_workflow(slug: str, kwargs: Dict[str, Any], func) -> R:
+
+    response = httpx.post(f"http://localhost:8000/workflows/{slug}", json=kwargs)
+    logger.info(response.json())
+    output = func(**kwargs)
+    logger.info(output)
+    return output
 
 
 def workflow(
     name: str,
     description: str,
     agents: List[Union[BaseModel, str]] = [],
     tasks: List[Union[BaseModel, str]] = [],
@@ -395,18 +425,117 @@
         )
         workflow_registry[name] = config
 
         is_async_fn = inspect.iscoroutinefunction(func)
 
         @functools.wraps(func)
         def wrapped(*args: P.args, **kwargs: P.kwargs) -> Union[R, WorkflowRun]:
-            logger.info(f"Calling {name}: {description}")
+
+            print("----------")
+            frames = inspect.stack()
+            for frame in frames:
+                print(frame.filename, frame.lineno, frame.function)
+                print("---")
+            print("----------")
+
+            logger.info("Executing workflow: " + name)
+            kwargs.update(zip(func.__code__.co_varnames, args))
             if is_async_fn:
                 return execute_workflow_async(slug=name, kwargs=kwargs)
 
             return execute_workflow(slug=name, kwargs=kwargs, func=func)
 
         # pylint: disable=protected-access
         wrapped.__config = config  # type: ignore
         return wrapped
 
     return decorator
+
+
+class Task(BaseModel):
+    """
+    Base class for all tools.
+
+    Attributes:
+        name (str): The name of the tool.
+        description (str): The description of the tool.
+    """
+
+    name: str
+    description: str
+    slug: str
+    func: Callable[..., Any]
+    input_params: List[Param]
+    output_params: List[Param]
+    agents: List[str]
+    depends_on: List[str]
+
+    class Config:
+        """Pydantic configuration."""
+
+        frozen = True
+
+
+def task(
+    name: str,
+    agents: List[str],
+    description: Optional[str] = None,
+    depends_on: Optional[List[str]] = None,
+) -> Callable[[Callable[P, R]], Callable[P, R]]:
+    """
+    Creates a decorator that logs the call details of the function it decorates,
+    and stores the function in a global registry under the provided name.
+
+    Args:
+    name (str): The name of the tool.
+    description (str): A brief description of what the tool does.
+    agents (List[str]): The agents that are used to execute the task.
+
+    Returns:
+    Callable: A decorator that enhances functions with logging and registration capabilities.
+    """
+
+    def decorator(func: Callable[P, R]) -> Callable[P, R]:
+
+        func_details = get_function_details(func)
+        func_name = func_details["name"]
+        slug = slugify(func_name)
+
+        config = Task(
+            name=name,
+            description=(
+                description if description else str(func_details["description"])
+            ),
+            agents=agents,
+            slug=slug,
+            func=func,
+            depends_on=depends_on or [],
+            input_params=func_details.get("input_params", {}),
+            output_params=func_details.get("output_params", {}),
+        )
+
+        task_registry[slug] = config
+
+        @functools.wraps(func)
+        def wrapped(*args: P.args, **kwargs: P.kwargs) -> R:
+
+            print("==----------")
+            frames = inspect.stack()
+            for frame in frames:
+                print(
+                    frame.filename,
+                    frame.lineno,
+                    frame.function,
+                    frame.code_context,
+                )
+                print("---")
+            print("==----------")
+
+            logger.info("Executing task: " + name)
+            result = func(*args, **kwargs)
+            return result
+
+        # pylint: disable=protected-access
+        wrapped.__config = config  # type: ignore
+        return wrapped
+
+    return decorator
```

### Comparing `botifyme-0.1.5/botifyme/registry.py` & `botifyme-0.1.5.1/botifyme/registry.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.5/botifyme/runtime.py` & `botifyme-0.1.5.1/botifyme/runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import os
 import json
 from typing import Callable, List
 from botifyme.config import (
     AgentInstanceRegistry,
-    get_tool,
-    get_function_details,
     tool_registry,
     workflow_registry,
+    task_registry,
     WorkflowConfig,
     Agent,
 )
 import importlib.util
 
 
 def list_workflows() -> List[WorkflowConfig]:
@@ -92,14 +91,22 @@
     # Create or clear the 'workflows' directory
     if not os.path.exists(botifyme_config_dir):
         os.makedirs(botifyme_config_dir)
     else:
         for file in os.listdir(botifyme_config_dir):
             os.remove(os.path.join(botifyme_config_dir, file))
 
+    tasks_config = []
+    for _, task in task_registry.items():
+        task_config = task.model_dump(
+            exclude={"func"}, exclude_unset=True, exclude_none=True
+        )
+        tasks_config.append(task_config)
+    write_config_file(tasks_config, os.path.join(botifyme_config_dir, "tasks.json"))
+
     # Save tool configuration to `tools.json`
     tools_config = []
     for _, tool in tool_registry.items():
         tool_config = tool.model_dump(
             exclude={"func"}, exclude_unset=True, exclude_none=True
         )
         tools_config.append(tool_config)
```

### Comparing `botifyme-0.1.5/botifyme/utils/tools.py` & `botifyme-0.1.5.1/botifyme/utils/tools.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.5/botifyme/workflow.py` & `botifyme-0.1.5.1/botifyme/workflow.py`

 * *Files identical despite different names*

### Comparing `botifyme-0.1.5/pyproject.toml` & `botifyme-0.1.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "botifyme"
-version = "0.1.5"
+version = "0.1.5.1"
 description = "Toolkit for building Autonomous AI agents"
 authors = ["Arun Reddy <arun@botifyme.dev>"]
 license = "Apache License 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 openai = "^1.1.2"
 tenacity = "^8.2.3"
 typer = {extras = ["all"], version = "^0.9.0"}
 requests = "^2.31.0"
 pyyaml = "^6.0.1"
 httpx = "^0.26.0"
 toml = "^0.10.2"
```

### Comparing `botifyme-0.1.5/PKG-INFO` & `botifyme-0.1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: botifyme
-Version: 0.1.5
+Version: 0.1.5.1
 Summary: Toolkit for building Autonomous AI agents
 License: Apache-2.0
 Author: Arun Reddy
 Author-email: arun@botifyme.dev
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: autoregistry (>=1.1.2,<2.0.0)
 Requires-Dist: cloudpickle (>=3.0.0,<4.0.0)
 Requires-Dist: docstring-parser (>=0.15,<0.16)
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
```

