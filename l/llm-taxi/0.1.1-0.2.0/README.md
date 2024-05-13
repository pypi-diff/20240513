# Comparing `tmp/llm_taxi-0.1.1.tar.gz` & `tmp/llm_taxi-0.2.0.tar.gz`

## Comparing `llm_taxi-0.1.1.tar` & `llm_taxi-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/.python-version
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/pyrightconfig.json
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/requirements-dev.lock
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/requirements.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/conversation.py
--rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/factory.py
--rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/__init__.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/anthropic.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/base.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/dashscope.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/deepinfra.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/deepseek.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/google.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/groq.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/mistral.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/openai.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/openrouter.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/perplexity.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/src/llm_taxi/llms/together.py
--rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/tests/test_llm.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/README.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 llm_taxi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/.python-version
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/pyrightconfig.json
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/requirements-dev.lock
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/requirements.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/__init__.py
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/cli.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/conversation.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/factory.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/__init__.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/anthropic.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/base.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/dashscope.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/deepinfra.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/deepseek.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/google.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/groq.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/mistral.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/openai.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/openrouter.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/perplexity.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/src/llm_taxi/llms/together.py
+-rw-r--r--   0        0        0     1158 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/tests/test_llm.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 llm_taxi-0.2.0/PKG-INFO
```

### Comparing `llm_taxi-0.1.1/requirements-dev.lock` & `llm_taxi-0.2.0/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.1/requirements.lock` & `llm_taxi-0.2.0/requirements.lock`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.1/src/llm_taxi/factory.py` & `llm_taxi-0.2.0/src/llm_taxi/factory.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.1/src/llm_taxi/llms/__init__.py` & `llm_taxi-0.2.0/src/llm_taxi/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.1/src/llm_taxi/llms/anthropic.py` & `llm_taxi-0.2.0/src/llm_taxi/llms/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from collections.abc import AsyncGenerator
-from typing import Any, Literal, cast
+from typing import Any, ClassVar, Literal, cast
 
 from anthropic import AsyncAnthropic
 from anthropic._types import NOT_GIVEN, NotGiven
 from anthropic.types import MessageParam
 
 from llm_taxi.conversation import Message, Role
 from llm_taxi.llms.base import LLM
 
 
 class Anthropic(LLM):
-    env_vars: dict[str, str] = {
+    env_vars: ClassVar[dict[str, str]] = {
         "api_key": "ANTHROPIC_API_KEY",
     }
 
     def _init_client(self, **kwargs) -> Any:
         return AsyncAnthropic(**kwargs)
 
     def _convert_messages(self, messages: list[Message]) -> list[Any]:
```

### Comparing `llm_taxi-0.1.1/src/llm_taxi/llms/base.py` & `llm_taxi-0.2.0/src/llm_taxi/llms/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import abc
 from collections.abc import AsyncGenerator
-from typing import Any
+from typing import Any, ClassVar
 
 from llm_taxi.conversation import Message
 
 
 class LLM(metaclass=abc.ABCMeta):
-    env_vars: dict[str, str] = {}
+    env_vars: ClassVar[dict[str, str]] = {}
 
     def __init__(
         self,
         *,
         model: str,
         api_key: str,
         base_url: str | None = None,
```

### Comparing `llm_taxi-0.1.1/src/llm_taxi/llms/google.py` & `llm_taxi-0.2.0/src/llm_taxi/llms/google.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import itertools
 from collections.abc import AsyncGenerator
-from typing import Any
+from typing import Any, ClassVar
 
 from llm_taxi.conversation import Message, Role
 from llm_taxi.llms import LLM
 
 
 class Google(LLM):
-    env_vars: dict[str, str] = {
+    env_vars: ClassVar[dict[str, str]] = {
         "api_key": "GOOGLE_API_KEY",
     }
 
     def __init__(
         self,
         *,
         model: str,
@@ -33,15 +33,15 @@
         genai.configure(api_key=api_key, **client_kwargs)
 
         self._call_kwargs.pop("model", None)
 
     def _init_client(self, **kwargs) -> Any:
         from google import generativeai as genai
 
-        return genai.GenerativeModel(self.model)
+        return genai.GenerativeModel(self.model, **kwargs)
 
     def _convert_messages(self, messages: list[Message]) -> list[Any]:
         role_mappping = {
             Role.System: "user",
             Role.User: "user",
             Role.Assistant: "model",
         }
```

### Comparing `llm_taxi-0.1.1/src/llm_taxi/llms/groq.py` & `llm_taxi-0.2.0/src/llm_taxi/llms/groq.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Any
+from typing import Any, ClassVar
 
 from groq import AsyncGroq
 from groq.types.chat.completion_create_params import Message as GroqMessage
 
 from llm_taxi.conversation import Message
 from llm_taxi.llms.openai import OpenAI
 
 
 class Groq(OpenAI):
-    env_vars: dict[str, str] = {
+    env_vars: ClassVar[dict[str, str]] = {
         "api_key": "GROQ_API_KEY",
     }
 
     def _init_client(self, **kwargs) -> Any:
         return AsyncGroq(**kwargs)
 
     def _convert_messages(self, messages: list[Message]) -> list[Any]:
```

### Comparing `llm_taxi-0.1.1/src/llm_taxi/llms/mistral.py` & `llm_taxi-0.2.0/src/llm_taxi/llms/mistral.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from collections.abc import AsyncGenerator
-from typing import Any
+from typing import Any, ClassVar
 
 from mistralai.async_client import MistralAsyncClient
 from mistralai.models.chat_completion import ChatMessage
 
 from llm_taxi.conversation import Message
 from llm_taxi.llms.openai import OpenAI
 
 
 class Mistral(OpenAI):
-    env_vars: dict[str, str] = {
+    env_vars: ClassVar[dict[str, str]] = {
         "api_key": "MISTRAL_API_KEY",
     }
 
     def _init_client(self, **kwargs) -> Any:
         kwargs.pop("base_url", None)
 
         return MistralAsyncClient(**kwargs)
```

### Comparing `llm_taxi-0.1.1/src/llm_taxi/llms/openai.py` & `llm_taxi-0.2.0/src/llm_taxi/llms/openai.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections.abc import AsyncGenerator
-from typing import Any
+from typing import Any, ClassVar
 
 from llm_taxi.conversation import Message
 from llm_taxi.llms import LLM
 
 
 class OpenAI(LLM):
-    env_vars: dict[str, str] = {
+    env_vars: ClassVar[dict[str, str]] = {
         "api_key": "OPENAI_API_KEY",
     }
 
     def _init_client(self, **kwargs) -> Any:
         from openai import AsyncClient
 
         return AsyncClient(**kwargs)
```

### Comparing `llm_taxi-0.1.1/tests/test_llm.py` & `llm_taxi-0.2.0/tests/test_llm.py`

 * *Files identical despite different names*

### Comparing `llm_taxi-0.1.1/pyproject.toml` & `llm_taxi-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [project]
 name = "llm-taxi"
-version = "0.1.1"
-description = "Add your description here"
+version = "0.2.0"
+description = "Call LLM as easily as calling a taxi."
 authors = [{ name = "Yevgnen Koh", email = "wherejoystarts@gmail.com" }]
 dependencies = [
     "openai>=1.28.1",
     "pydantic>=2.7.1",
     "google-generativeai>=0.5.2",
     "together>=1.1.5",
     "groq>=0.5.0",
     "anthropic>=0.25.8",
     "mistralai>=0.1.8",
     "httpx[socks]<0.26.0",
 ]
 readme = "README.md"
 requires-python = ">= 3.10"
 
+[project.scripts]
+llm-taxi = "llm_taxi.cli:main"
+
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [tool.rye]
 managed = true
 dev-dependencies = []
```

