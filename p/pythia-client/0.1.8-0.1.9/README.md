# Comparing `tmp/pythia_client-0.1.8.tar.gz` & `tmp/pythia_client-0.1.9.tar.gz`

## Comparing `pythia_client-0.1.8.tar` & `pythia_client-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pythia_client-0.1.8/.python-version
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 pythia_client-0.1.8/CHANGELOG.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pythia_client-0.1.8/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.8/src/pythia_client/__init__.py
--rw-r--r--   0        0        0    20897 2020-02-02 00:00:00.000000 pythia_client-0.1.8/src/pythia_client/client.py
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 pythia_client-0.1.8/src/pythia_client/schema.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.8/test/__init__.py
--rw-r--r--   0        0        0     9212 2020-02-02 00:00:00.000000 pythia_client-0.1.8/test/test_client.py
--rw-r--r--   0        0        0    26093 2020-02-02 00:00:00.000000 pythia_client-0.1.8/test/samples/sample1.pdf
--rw-r--r--   0        0        0   217237 2020-02-02 00:00:00.000000 pythia_client-0.1.8/test/samples/sample2.pdf
--rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 pythia_client-0.1.8/test/samples/sample3.pdf
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pythia_client-0.1.8/.gitignore
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pythia_client-0.1.8/LICENSE
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pythia_client-0.1.8/README.md
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pythia_client-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pythia_client-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pythia_client-0.1.9/.python-version
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 pythia_client-0.1.9/CHANGELOG.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 pythia_client-0.1.9/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.9/src/pythia_client/__init__.py
+-rw-r--r--   0        0        0    20985 2020-02-02 00:00:00.000000 pythia_client-0.1.9/src/pythia_client/client.py
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 pythia_client-0.1.9/src/pythia_client/schema.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pythia_client-0.1.9/test/__init__.py
+-rw-r--r--   0        0        0     9316 2020-02-02 00:00:00.000000 pythia_client-0.1.9/test/test_client.py
+-rw-r--r--   0        0        0    26093 2020-02-02 00:00:00.000000 pythia_client-0.1.9/test/samples/sample1.pdf
+-rw-r--r--   0        0        0   217237 2020-02-02 00:00:00.000000 pythia_client-0.1.9/test/samples/sample2.pdf
+-rw-r--r--   0        0        0    21457 2020-02-02 00:00:00.000000 pythia_client-0.1.9/test/samples/sample3.pdf
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pythia_client-0.1.9/.gitignore
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 pythia_client-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 pythia_client-0.1.9/README.md
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 pythia_client-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pythia_client-0.1.9/PKG-INFO
```

### Comparing `pythia_client-0.1.8/CHANGELOG.md` & `pythia_client-0.1.9/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
+#### v0.1.9
+- Top K params for query function. Compatible with `haystack-api` v0.2.4
+
 #### v0.1.8
 - Custom system prompt params for query endpoint. Compatible with `haystack-api` v0.2.3
+
 #### v0.1.7
 - MetaJSON schema fix for Mistral models. Compatible with `haystack-api` v0.2.2
 
 #### v0.1.6
 - New intent functions: add_intent, predict_intent, delete_intent. Compatible with `haystack-api` v0.2.1
 
 #### v0.1.4
```

### Comparing `pythia_client-0.1.8/src/pythia_client/client.py` & `pythia_client-0.1.9/src/pythia_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,14 +79,15 @@
         self.delete_intent_endpoint = urljoin(str(self.url), "alie/intent")
 
     def query(
         self,
         query: str,
         chat_history: Optional[List[ChatMessage]] = None,
         filters: Optional[FilterRequest] = None,
+        top_k = None,
         group_id: str = None,
         custom_system_prompt: str = None,
     ) -> QueryResponse:
         """Query the API with a user question to get a LLM-generated answer based
             on context from the document store.
 
             Args:
@@ -129,14 +130,16 @@
             )
         ```
         """
         params = FilterRequest(filters=filters).model_dump()
         if custom_system_prompt:
             params["system_prompt"] = custom_system_prompt
         params["group_id"] = group_id if group_id else "api"
+        if top_k is not None:
+            params["top_k"] = top_k
         request = QueryRequest(
             query=query,
             chat_history=chat_history,
             params=params,
         )
         with requests.Session() as session:
             payload = json.loads(request.model_dump_json())
```

### Comparing `pythia_client-0.1.8/src/pythia_client/schema.py` & `pythia_client-0.1.9/src/pythia_client/schema.py`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.8/test/test_client.py` & `pythia_client-0.1.9/test/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,17 +107,18 @@
     assert response is not None
     assert len(response.url) >= 100
     aws_s3_response = requests.get(response.url)
     assert aws_s3_response.status_code == 200
 
 
 def test_client_query():
-    response = client.query(query="Hey how are you ?")
+    response = client.query(query="How to give port 8 a power of 1337 milliwatts ?", top_k=2)
     assert response is not None
     assert len(response.AnswerBuilder.answers[0].data.content) > 20
+    assert len(response.AnswerBuilder.answers[0].documents) == 2
 
 def test_client_query_with_custom_prompt():
     system_prompt = """Start all your answers with the word "Banana", this is really important."""
     response = client.query(query="Hey how are you ?", custom_system_prompt=system_prompt)
     assert response is not None
     generated_content = response.AnswerBuilder.answers[0].data.content
     assert "Banana" in generated_content
```

### Comparing `pythia_client-0.1.8/test/samples/sample1.pdf` & `pythia_client-0.1.9/test/samples/sample1.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.8/test/samples/sample2.pdf` & `pythia_client-0.1.9/test/samples/sample2.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.8/test/samples/sample3.pdf` & `pythia_client-0.1.9/test/samples/sample3.pdf`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.8/LICENSE` & `pythia_client-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.8/README.md` & `pythia_client-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pythia_client-0.1.8/pyproject.toml` & `pythia_client-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pythia-client"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
     "requests>=2.31",
     "pydantic>=2.6",
 ]
 requires-python = ">=3.11"
 authors = [
   {name = "Corentin Meyer", email = "contact@cmeyer.fr"},
```

### Comparing `pythia_client-0.1.8/PKG-INFO` & `pythia_client-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pythia-client
-Version: 0.1.8
+Version: 0.1.9
 Summary: Client to interact with the Pythia API
 Project-URL: Homepage, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Documentation, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Repository, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia
 Project-URL: Issues, https://gitlab.com/ale-gitlab/dto/data-science/cip-bot/project-pythia/-/issues
 Author-email: Corentin Meyer <contact@cmeyer.fr>
 Maintainer-email: Corentin Meyer <contact@cmeyer.fr>
```

