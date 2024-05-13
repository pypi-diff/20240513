# Comparing `tmp/llama_cpp_haystack-0.3.0.tar.gz` & `tmp/llama_cpp_haystack-0.4.0.tar.gz`

## Comparing `llama_cpp_haystack-0.3.0.tar` & `llama_cpp_haystack-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/examples/llama_cpp_generator_example.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/examples/rag_pipeline_example.py
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/pydoc/config.yml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/src/haystack_integrations/components/generators/llama_cpp/__init__.py
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/src/haystack_integrations/components/generators/llama_cpp/generator.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     9046 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/tests/test_generator.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/tests/models/.gitignore
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/README.md
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     9936 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/examples/llama_cpp_generator_example.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/examples/rag_pipeline_example.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/pydoc/config.yml
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/src/haystack_integrations/components/generators/llama_cpp/__init__.py
+-rw-r--r--   0        0        0     4493 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/src/haystack_integrations/components/generators/llama_cpp/generator.py
+-rw-r--r--   0        0        0     5743 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/src/haystack_integrations/components/generators/llama_cpp/chat/chat_generator.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0    19797 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/tests/test_chat_generator.py
+-rw-r--r--   0        0        0     9046 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/tests/test_generator.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/tests/models/.gitignore
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/README.md
+-rw-r--r--   0        0        0     4187 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9999 2020-02-02 00:00:00.000000 llama_cpp_haystack-0.4.0/PKG-INFO
```

### Comparing `llama_cpp_haystack-0.3.0/examples/rag_pipeline_example.py` & `llama_cpp_haystack-0.4.0/examples/rag_pipeline_example.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 
 doc_store = InMemoryDocumentStore(embedding_similarity_function="cosine")
 doc_embedder = SentenceTransformersDocumentEmbedder(model="sentence-transformers/all-MiniLM-L6-v2")
 
 
 # Indexing Pipeline
 indexing_pipeline = Pipeline()
-indexing_pipeline.add_component(instance=doc_embedder, name="DocEmbedder")
-indexing_pipeline.add_component(instance=DocumentWriter(document_store=doc_store), name="DocWriter")
-indexing_pipeline.connect(connect_from="DocEmbedder", connect_to="DocWriter")
+indexing_pipeline.add_component(instance=doc_embedder, name="doc_embedder")
+indexing_pipeline.add_component(instance=DocumentWriter(document_store=doc_store), name="doc_writer")
+indexing_pipeline.connect("doc_embedder", "doc_writer")
 
-indexing_pipeline.run({"DocEmbedder": {"documents": docs}})
+indexing_pipeline.run({"doc_embedder": {"documents": docs}})
 
 
 # RAG Pipeline
 prompt_template = """GPT4 Correct User: Answer the question using the provided context.
 Question: {{question}}
 Context:
 {% for doc in documents %}
@@ -46,15 +46,15 @@
 GPT4 Correct Assistant:
 """
 rag_pipeline = Pipeline()
 
 text_embedder = SentenceTransformersTextEmbedder(model="sentence-transformers/all-MiniLM-L6-v2")
 
 model_path = "openchat-3.5-1210.Q3_K_S.gguf"
-generator = LlamaCppGenerator(model_path=model_path, n_ctx=4096, n_batch=128)
+generator = LlamaCppGenerator(model=model_path, n_ctx=4096, n_batch=128)
 
 rag_pipeline.add_component(
     instance=text_embedder,
     name="text_embedder",
 )
 rag_pipeline.add_component(instance=InMemoryEmbeddingRetriever(document_store=doc_store, top_k=3), name="retriever")
 rag_pipeline.add_component(instance=PromptBuilder(template=prompt_template), name="prompt_builder")
```

### Comparing `llama_cpp_haystack-0.3.0/pydoc/config.yml` & `llama_cpp_haystack-0.4.0/pydoc/config.yml`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,20 @@
     expression:
     documented_only: true
     do_not_filter_modules: false
     skip_empty_modules: true
   - type: smart
   - type: crossref
 renderer:
-  type: haystack_pydoc_tools.renderers.ReadmePreviewRenderer
+  type: haystack_pydoc_tools.renderers.ReadmeIntegrationRenderer
   excerpt: Llama.cpp integration for Haystack
   category_slug: integrations-api
   title: Llama.cpp
   slug: integrations-llama-cpp
   order: 140
   markdown:
     descriptive_class_title: false
+    classdef_code_block: false
     descriptive_module_title: true
     add_method_class_prefix: true
     add_member_class_prefix: false
     filename: _readme_llama_cpp.md
```

### Comparing `llama_cpp_haystack-0.3.0/src/haystack_integrations/components/generators/llama_cpp/generator.py` & `llama_cpp_haystack-0.4.0/src/haystack_integrations/components/generators/llama_cpp/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,22 @@
 
 logger = logging.getLogger(__name__)
 
 
 @component
 class LlamaCppGenerator:
     """
-    Generator for using a model with Llama.cpp.
-    This component provides an interface to generate text using a quantized model (GGUF) using llama.cpp.
+    Provides an interface to generate text using LLM via llama.cpp.
+
+    [llama.cpp](https://github.com/ggerganov/llama.cpp) is a project written in C/C++ for efficient inference of LLMs.
+    It employs the quantized GGUF format, suitable for running these models on standard machines (even without GPUs).
 
     Usage example:
     ```python
-    from llama_cpp_haystack import LlamaCppGenerator
+    from haystack_integrations.components.generators.llama_cpp import LlamaCppGenerator
     generator = LlamaCppGenerator(model="zephyr-7b-beta.Q4_0.gguf", n_ctx=2048, n_batch=512)
 
     print(generator.run("Who is the best American actor?", generation_kwargs={"max_tokens": 128}))
     # {'replies': ['John Cusack'], 'meta': [{"object": "text_completion", ...}]}
     ```
     """
 
@@ -29,36 +31,32 @@
         model: str,
         n_ctx: Optional[int] = 0,
         n_batch: Optional[int] = 512,
         model_kwargs: Optional[Dict[str, Any]] = None,
         generation_kwargs: Optional[Dict[str, Any]] = None,
     ):
         """
-        :param model: The path of a quantized model for text generation,
-            for example, "zephyr-7b-beta.Q4_0.gguf".
+        :param model: The path of a quantized model for text generation, for example, "zephyr-7b-beta.Q4_0.gguf".
             If the model path is also specified in the `model_kwargs`, this parameter will be ignored.
         :param n_ctx: The number of tokens in the context. When set to 0, the context will be taken from the model.
-            If the n_ctx is also specified in the `model_kwargs`, this parameter will be ignored.
-        :param n_batch: Prompt processing maximum batch size. Defaults to 512.
-            If the n_batch is also specified in the `model_kwargs`, this parameter will be ignored.
+        :param n_batch: Prompt processing maximum batch size.
         :param model_kwargs: Dictionary containing keyword arguments used to initialize the LLM for text generation.
             These keyword arguments provide fine-grained control over the model loading.
             In case of duplication, these kwargs override `model`, `n_ctx`, and `n_batch` init parameters.
-            See Llama.cpp's [documentation](https://llama-cpp-python.readthedocs.io/en/latest/api-reference/#llama_cpp.Llama.__init__)
-            for more information on the available kwargs.
+            For more information on the available kwargs, see
+            [llama.cpp documentation](https://llama-cpp-python.readthedocs.io/en/latest/api-reference/#llama_cpp.Llama.__init__).
         :param generation_kwargs:  A dictionary containing keyword arguments to customize text generation.
-            Some examples: `max_tokens`, `temperature`, `top_k`, `top_p`,...
-            See Llama.cpp's  documentation for more information:
-                https://llama-cpp-python.readthedocs.io/en/latest/api-reference/#llama_cpp.Llama.create_completion
+            For more information on the available kwargs, see
+            [llama.cpp documentation](https://llama-cpp-python.readthedocs.io/en/latest/api-reference/#llama_cpp.Llama.create_completion).
         """
 
         model_kwargs = model_kwargs or {}
         generation_kwargs = generation_kwargs or {}
 
-        # check if the huggingface_pipeline_kwargs contain the essential parameters
+        # check if the model_kwargs contain the essential parameters
         # otherwise, populate them with values from init parameters
         model_kwargs.setdefault("model_path", model)
         model_kwargs.setdefault("n_ctx", n_ctx)
         model_kwargs.setdefault("n_batch", n_batch)
 
         self.model_path = model
         self.n_ctx = n_ctx
@@ -72,20 +70,21 @@
             self.model = Llama(**self.model_kwargs)
 
     @component.output_types(replies=List[str], meta=List[Dict[str, Any]])
     def run(self, prompt: str, generation_kwargs: Optional[Dict[str, Any]] = None):
         """
         Run the text generation model on the given prompt.
 
-        :param prompt: A string representing the prompt.
-        :param generation_kwargs: A dictionary containing keyword arguments to customize text generation.
-            Some examples: `max_tokens`, `temperature`, `top_k`, `top_p`,...
-            See Llama.cpp's  documentation for more information:
-                https://llama-cpp-python.readthedocs.io/en/latest/api-reference/#llama_cpp.Llama.create_completion
-        :return: A dictionary of the returned responses and metadata.
+        :param prompt: the prompt to be sent to the generative model.
+        :param generation_kwargs:  A dictionary containing keyword arguments to customize text generation.
+            For more information on the available kwargs, see
+            [llama.cpp documentation](https://llama-cpp-python.readthedocs.io/en/latest/api-reference/#llama_cpp.Llama.create_completion).
+        :returns: A dictionary with the following keys:
+            - `replies`: the list of replies generated by the model.
+            - `meta`: metadata about the request.
         """
         if self.model is None:
             error_msg = "The model has not been loaded. Please call warm_up() before running."
             raise RuntimeError(error_msg)
 
         if not prompt:
             return {"replies": []}
```

### Comparing `llama_cpp_haystack-0.3.0/tests/test_generator.py` & `llama_cpp_haystack-0.4.0/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `llama_cpp_haystack-0.3.0/.gitignore` & `llama_cpp_haystack-0.4.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -130,7 +130,8 @@
 .pyre/
 
 # IDEs
 .vscode
 
 # Docs generation artifacts
 _readme_*.md
+.idea
```

### Comparing `llama_cpp_haystack-0.3.0/LICENSE.txt` & `llama_cpp_haystack-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llama_cpp_haystack-0.3.0/README.md` & `llama_cpp_haystack-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `llama_cpp_haystack-0.3.0/pyproject.toml` & `llama_cpp_haystack-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 license = "Apache-2.0"
 keywords = []
 authors = [
     { name = "deepset GmbH", email = "info@deepset.ai" },
     { name = "Ashwin Mathur", email = "" },
 ]
 classifiers = [
+  "License :: OSI Approved :: Apache Software License",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
@@ -47,14 +48,15 @@
 git_describe_command = 'git describe --tags --match="integrations/llama_cpp-v[0-9]*"'
 
 [tool.hatch.envs.default]
 dependencies = [
     "coverage[toml]>=6.5",
     "pytest",
     "haystack-pydoc-tools",
+    "transformers[sentencepiece]"
 ]
 [tool.hatch.envs.default.scripts]
 test = "pytest {args:tests}"
 test-cov = "coverage run -m pytest {args:tests}"
 cov-report = [
     "- coverage combine",
     "coverage report",
@@ -97,20 +99,20 @@
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.ruff.isort]
 known-first-party = ["src"]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 line-length = 120
 skip-string-normalization = true
 
 [tool.ruff]
-target-version = "py37"
+target-version = "py38"
 line-length = 120
 select = [
     "A",
     "ARG",
     "B",
     "C",
     "DTZ",
@@ -154,30 +156,29 @@
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 # Examples can print their output
 "examples/**" = ["T201"]
 "tests/**" = ["T201"]
 
 [tool.coverage.run]
-source_pkgs = ["llama_cpp_haystack", "tests"]
+source = ["haystack_integrations"]
 branch = true
-parallel = true
+parallel = false
 
 
-[tool.coverage.paths]
-llama_cpp_haystack = ["src/haystack_integrations", "*/llama-cpp-haystack/src"]
-tests = ["tests", "*/llama-cpp-haystack/tests"]
-
 [tool.coverage.report]
+omit = ["*/tests/*", "*/__init__.py"]
+show_missing=true
 exclude_lines = [
-    "no cov",
-    "if __name__ == .__main__.:",
-    "if TYPE_CHECKING:",
+  "no cov",
+  "if __name__ == .__main__.:",
+  "if TYPE_CHECKING:",
 ]
 
+
 [tool.pytest.ini_options]
 markers = [
     "integration: marks tests as slow (deselect with '-m \"not integration\"')",
 ]
 addopts = [
     "--import-mode=importlib",
 ]
```

### Comparing `llama_cpp_haystack-0.3.0/PKG-INFO` & `llama_cpp_haystack-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: llama-cpp-haystack
-Version: 0.3.0
+Version: 0.4.0
 Summary: An integration between the llama.cpp LLM framework and Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/llama_cpp#readme
 Project-URL: Issues, https://github.com/deepset-ai/haystack-core-integrations/issues
 Project-URL: Source, https://github.com/deepset-ai/haystack-core-integrations/tree/main/integrations/llama_cpp
 Author: Ashwin Mathur
 Author-email: deepset GmbH <info@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

