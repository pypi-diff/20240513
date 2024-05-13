# Comparing `tmp/spiceai-0.3.4.tar.gz` & `tmp/spiceai-0.3.5.tar.gz`

## Comparing `spiceai-0.3.4.tar` & `spiceai-0.3.5.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.4/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.4/scripts/mytoml.toml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.4/scripts/prompt.txt
--rw-r--r--   0        0        0     6011 2020-02-02 00:00:00.000000 spiceai-0.3.4/scripts/run.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.4/spice/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.4/spice/errors.py
--rw-r--r--   0        0        0     6508 2020-02-02 00:00:00.000000 spiceai-0.3.4/spice/models.py
--rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.4/spice/providers.py
--rw-r--r--   0        0        0    35065 2020-02-02 00:00:00.000000 spiceai-0.3.4/spice/spice.py
--rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.4/spice/spice_message.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 spiceai-0.3.4/spice/utils.py
--rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.4/spice/wrapped_clients.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.4/tests/__init__.py
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 spiceai-0.3.4/tests/conftest.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 spiceai-0.3.4/tests/test_spice.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.4/LICENSE
--rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.4/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0    28879 2020-02-02 00:00:00.000000 spiceai-0.3.5/tags
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 spiceai-0.3.5/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 spiceai-0.3.5/.ropeproject/globalnames
+-rw-r--r--   0        0        0    89341 2020-02-02 00:00:00.000000 spiceai-0.3.5/.ropeproject/history
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 spiceai-0.3.5/scripts/mytoml.toml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 spiceai-0.3.5/scripts/prompt.txt
+-rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 spiceai-0.3.5/scripts/run.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/errors.py
+-rw-r--r--   0        0        0     6897 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/models.py
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/providers.py
+-rw-r--r--   0        0        0    35065 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/spice.py
+-rw-r--r--   0        0        0     7622 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/spice_message.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/utils.py
+-rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 spiceai-0.3.5/spice/wrapped_clients.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spiceai-0.3.5/tests/__init__.py
+-rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 spiceai-0.3.5/tests/conftest.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 spiceai-0.3.5/tests/test_spice.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 spiceai-0.3.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 spiceai-0.3.5/LICENSE
+-rw-r--r--   0        0        0     5903 2020-02-02 00:00:00.000000 spiceai-0.3.5/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 spiceai-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     6445 2020-02-02 00:00:00.000000 spiceai-0.3.5/PKG-INFO
```

### Comparing `spiceai-0.3.4/.github/workflows/ruff.yml` & `spiceai-0.3.5/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/scripts/run.py` & `spiceai-0.3.5/scripts/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 async def basic_example():
     client = Spice()
 
     messages: List[SpiceMessage] = [
         {"role": "system", "content": "You are a helpful assistant."},
         {"role": "user", "content": "list 5 random words"},
     ]
-    response = await client.get_response(messages=messages, model="gpt-4-0125-preview")
+    response = await client.get_response(messages=messages, model="gpt-4o")
 
     print(response.text)
 
 
 async def streaming_example():
     # You can set a default model for the client instead of passing it with each call
     client = Spice(default_text_model="claude-3-opus-20240229")
```

### Comparing `spiceai-0.3.4/spice/errors.py` & `spiceai-0.3.5/spice/errors.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/spice/models.py` & `spiceai-0.3.5/spice/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,20 @@
 
 
 @dataclass
 class UnknownModel(TextModel, EmbeddingModel, TranscriptionModel):
     pass
 
 
+GPT_4o = TextModel("gpt-4o", OPEN_AI, input_cost=500, output_cost=1500, context_length=128000)
+"""Warning: This model always points to OpenAI's latest GPT-4o model, so the input and output costs may incorrect. We recommend using specific versions of GPT-4o instead."""
+
+GPT_4o_2024_05_13 = TextModel("gpt-4o-2024-05-13", OPEN_AI, input_cost=500, output_cost=1500, context_length=128000)
+
+
 GPT_4_TURBO = TextModel("gpt-4-turbo", OPEN_AI, input_cost=1000, output_cost=3000, context_length=128000)
 """Warning: This model always points to OpenAI's latest GPT-4-Turbo model, so the input and output costs may incorrect. We recommend using specific versions of GPT-4-Turbo instead."""
 
 GPT_4_TURBO_2024_04_09 = TextModel(
     "gpt-4-turbo-2024-04-09", OPEN_AI, input_cost=1000, output_cost=3000, context_length=128000
 )
```

### Comparing `spiceai-0.3.4/spice/providers.py` & `spiceai-0.3.5/spice/providers.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/spice/spice.py` & `spiceai-0.3.5/spice/spice.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/spice/spice_message.py` & `spiceai-0.3.5/spice/spice_message.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/spice/utils.py` & `spiceai-0.3.5/spice/utils.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/spice/wrapped_clients.py` & `spiceai-0.3.5/spice/wrapped_clients.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/tests/conftest.py` & `spiceai-0.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/tests/test_spice.py` & `spiceai-0.3.5/tests/test_spice.py`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/LICENSE` & `spiceai-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/README.md` & `spiceai-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `spiceai-0.3.4/pyproject.toml` & `spiceai-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.hatch]
 
 [tool.hatch.build.targets.wheel]
 packages=["spice"]
 
 [project]
 name = "spiceai"
-version = "0.3.4"
+version = "0.3.5"
 license = {text = "Apache-2.0"}
 description = "A Python library for building AI-powered applications."
 readme = "README.md"
 dependencies = [
     "python-dotenv",
     "openai",
     "anthropic",
```

### Comparing `spiceai-0.3.4/PKG-INFO` & `spiceai-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: spiceai
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Python library for building AI-powered applications.
 License: Apache-2.0
 License-File: LICENSE
 Requires-Dist: anthropic
 Requires-Dist: httpx
 Requires-Dist: jinja2
 Requires-Dist: openai
```

