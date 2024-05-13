# Comparing `tmp/kubeinfra-0.0.1a3.tar.gz` & `tmp/kubeinfra-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubeinfra-0.0.1a3.tar", max compression
+gzip compressed data, was "kubeinfra-0.0.1a4.tar", max compression
```

## Comparing `kubeinfra-0.0.1a3.tar` & `kubeinfra-0.0.1a4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       11 2024-05-13 05:36:29.658053 kubeinfra-0.0.1a3/README.md
--rw-r--r--   0        0        0     2414 2024-05-13 05:56:27.467619 kubeinfra-0.0.1a3/kubeinfra/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 08:54:56.058848 kubeinfra-0.0.1a3/kubeinfra/cli/__init__.py
--rw-r--r--   0        0        0      184 2024-05-12 08:54:56.059502 kubeinfra-0.0.1a3/kubeinfra/cli/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2802 2024-05-12 08:54:56.059252 kubeinfra-0.0.1a3/kubeinfra/cli/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     1666 2024-05-13 05:35:40.940381 kubeinfra-0.0.1a3/kubeinfra/cli/cli.py
--rw-r--r--   0        0        0        0 2024-05-12 08:54:56.061195 kubeinfra-0.0.1a3/kubeinfra/commands/__init__.py
--rw-r--r--   0        0        0      190 2024-05-12 08:54:56.065047 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      185 2024-05-13 02:42:11.732495 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     7333 2024-05-12 08:54:56.062099 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/chat.cpython-311.pyc
--rw-r--r--   0        0        0     6848 2024-05-13 02:42:11.733367 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/chat.cpython-312.pyc
--rw-r--r--   0        0        0     7805 2024-05-12 08:54:56.064241 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/complete.cpython-311.pyc
--rw-r--r--   0        0        0     7189 2024-05-13 02:42:11.736672 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/complete.cpython-312.pyc
--rw-r--r--   0        0        0     2450 2024-05-12 08:54:56.063176 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/embeddings.cpython-311.pyc
--rw-r--r--   0        0        0     2110 2024-05-13 02:42:11.737143 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/embeddings.cpython-312.pyc
--rw-r--r--   0        0        0    10030 2024-05-12 08:54:56.063454 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/files.cpython-311.pyc
--rw-r--r--   0        0        0     8705 2024-05-13 02:42:11.738167 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/files.cpython-312.pyc
--rw-r--r--   0        0        0    16007 2024-05-12 08:54:56.061856 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/finetune.cpython-311.pyc
--rw-r--r--   0        0        0    14266 2024-05-13 02:42:11.742232 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/finetune.cpython-312.pyc
--rw-r--r--   0        0        0     6278 2024-05-12 08:54:56.063315 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/image.cpython-311.pyc
--rw-r--r--   0        0        0     5579 2024-05-13 02:42:11.742959 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/image.cpython-312.pyc
--rw-r--r--   0        0        0    10173 2024-05-12 08:54:56.064107 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     8829 2024-05-13 02:42:11.743922 kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/models.cpython-312.pyc
--rw-r--r--   0        0        0     4392 2024-05-12 08:54:56.065302 kubeinfra-0.0.1a3/kubeinfra/commands/chat.py
--rw-r--r--   0        0        0     5849 2024-05-13 05:35:40.930157 kubeinfra-0.0.1a3/kubeinfra/commands/complete.py
--rw-r--r--   0        0        0     1182 2024-05-12 08:54:56.065517 kubeinfra-0.0.1a3/kubeinfra/commands/embeddings.py
--rw-r--r--   0        0        0     5905 2024-05-12 08:54:56.060860 kubeinfra-0.0.1a3/kubeinfra/commands/files.py
--rw-r--r--   0        0        0    11262 2024-05-12 08:54:56.066080 kubeinfra-0.0.1a3/kubeinfra/commands/finetune.py
--rw-r--r--   0        0        0     4019 2024-05-13 05:35:40.911922 kubeinfra-0.0.1a3/kubeinfra/commands/image.py
--rw-r--r--   0        0        0     6221 2024-05-12 08:54:56.061115 kubeinfra-0.0.1a3/kubeinfra/commands/models.py
--rw-r--r--   0        0        0     9544 2024-05-13 05:35:40.937393 kubeinfra-0.0.1a3/kubeinfra/complete.py
--rw-r--r--   0        0        0     1889 2024-05-12 08:54:56.059927 kubeinfra-0.0.1a3/kubeinfra/embeddings.py
--rw-r--r--   0        0        0     2647 2024-05-13 05:35:40.932625 kubeinfra-0.0.1a3/kubeinfra/error.py
--rw-r--r--   0        0        0    13449 2024-05-13 05:35:40.914117 kubeinfra-0.0.1a3/kubeinfra/files.py
--rw-r--r--   0        0        0    12222 2024-05-12 08:54:56.067084 kubeinfra-0.0.1a3/kubeinfra/finetune.py
--rw-r--r--   0        0        0   280722 2024-05-12 08:54:56.066787 kubeinfra-0.0.1a3/kubeinfra/image-0.png
--rw-r--r--   0        0        0     1110 2024-05-12 08:54:56.067284 kubeinfra-0.0.1a3/kubeinfra/image.py
--rw-r--r--   0        0        0   323993 2024-05-13 05:35:40.925821 kubeinfra-0.0.1a3/kubeinfra/models.json
--rw-r--r--   0        0        0     3083 2024-05-12 08:54:56.049007 kubeinfra-0.0.1a3/kubeinfra/models.py
--rw-r--r--   0        0        0        0 2024-05-12 08:54:56.045650 kubeinfra-0.0.1a3/kubeinfra/tools/__init__.py
--rw-r--r--   0        0        0      187 2024-05-12 08:54:56.047719 kubeinfra-0.0.1a3/kubeinfra/tools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      182 2024-05-13 02:42:11.601564 kubeinfra-0.0.1a3/kubeinfra/tools/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5094 2024-05-12 08:54:56.046794 kubeinfra-0.0.1a3/kubeinfra/tools/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0        0        0     4633 2024-05-13 02:42:11.602781 kubeinfra-0.0.1a3/kubeinfra/tools/__pycache__/conversation.cpython-312.pyc
--rw-r--r--   0        0        0     2734 2024-05-13 05:35:40.931512 kubeinfra-0.0.1a3/kubeinfra/tools/conversation.py
--rw-r--r--   0        0        0     3064 2024-05-13 05:35:40.934189 kubeinfra-0.0.1a3/kubeinfra/types.py
--rw-r--r--   0        0        0     5064 2024-05-13 05:35:40.909542 kubeinfra-0.0.1a3/kubeinfra/utils.py
--rw-r--r--   0        0        0      160 2024-05-12 08:54:56.048492 kubeinfra-0.0.1a3/kubeinfra/version.py
--rw-r--r--   0        0        0      447 2024-05-13 06:24:45.395286 kubeinfra-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 kubeinfra-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-05-13 05:36:29.658053 kubeinfra-0.0.1a4/README.md
+-rw-r--r--   0        0        0     2392 2024-05-13 06:58:07.329916 kubeinfra-0.0.1a4/kubeinfra/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:54:56.058848 kubeinfra-0.0.1a4/kubeinfra/cli/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-12 08:54:56.059502 kubeinfra-0.0.1a4/kubeinfra/cli/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2802 2024-05-12 08:54:56.059252 kubeinfra-0.0.1a4/kubeinfra/cli/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     1666 2024-05-13 05:35:40.940381 kubeinfra-0.0.1a4/kubeinfra/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:54:56.061195 kubeinfra-0.0.1a4/kubeinfra/commands/__init__.py
+-rw-r--r--   0        0        0      190 2024-05-12 08:54:56.065047 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      185 2024-05-13 02:42:11.732495 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7333 2024-05-12 08:54:56.062099 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/chat.cpython-311.pyc
+-rw-r--r--   0        0        0     6848 2024-05-13 02:42:11.733367 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/chat.cpython-312.pyc
+-rw-r--r--   0        0        0     7805 2024-05-12 08:54:56.064241 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/complete.cpython-311.pyc
+-rw-r--r--   0        0        0     7189 2024-05-13 02:42:11.736672 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/complete.cpython-312.pyc
+-rw-r--r--   0        0        0     2450 2024-05-12 08:54:56.063176 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/embeddings.cpython-311.pyc
+-rw-r--r--   0        0        0     2110 2024-05-13 02:42:11.737143 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/embeddings.cpython-312.pyc
+-rw-r--r--   0        0        0    10030 2024-05-12 08:54:56.063454 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/files.cpython-311.pyc
+-rw-r--r--   0        0        0     8705 2024-05-13 02:42:11.738167 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/files.cpython-312.pyc
+-rw-r--r--   0        0        0    16007 2024-05-12 08:54:56.061856 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/finetune.cpython-311.pyc
+-rw-r--r--   0        0        0    14266 2024-05-13 02:42:11.742232 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/finetune.cpython-312.pyc
+-rw-r--r--   0        0        0     6278 2024-05-12 08:54:56.063315 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/image.cpython-311.pyc
+-rw-r--r--   0        0        0     5579 2024-05-13 02:42:11.742959 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/image.cpython-312.pyc
+-rw-r--r--   0        0        0    10173 2024-05-12 08:54:56.064107 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     8829 2024-05-13 02:42:11.743922 kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/models.cpython-312.pyc
+-rw-r--r--   0        0        0     4394 2024-05-13 06:58:22.709311 kubeinfra-0.0.1a4/kubeinfra/commands/chat.py
+-rw-r--r--   0        0        0     5849 2024-05-13 05:35:40.930157 kubeinfra-0.0.1a4/kubeinfra/commands/complete.py
+-rw-r--r--   0        0        0     1182 2024-05-12 08:54:56.065517 kubeinfra-0.0.1a4/kubeinfra/commands/embeddings.py
+-rw-r--r--   0        0        0     5905 2024-05-12 08:54:56.060860 kubeinfra-0.0.1a4/kubeinfra/commands/files.py
+-rw-r--r--   0        0        0    11262 2024-05-12 08:54:56.066080 kubeinfra-0.0.1a4/kubeinfra/commands/finetune.py
+-rw-r--r--   0        0        0     4019 2024-05-13 05:35:40.911922 kubeinfra-0.0.1a4/kubeinfra/commands/image.py
+-rw-r--r--   0        0        0     6221 2024-05-12 08:54:56.061115 kubeinfra-0.0.1a4/kubeinfra/commands/models.py
+-rw-r--r--   0        0        0     9545 2024-05-13 06:58:37.526154 kubeinfra-0.0.1a4/kubeinfra/complete.py
+-rw-r--r--   0        0        0     1889 2024-05-12 08:54:56.059927 kubeinfra-0.0.1a4/kubeinfra/embeddings.py
+-rw-r--r--   0        0        0     2647 2024-05-13 05:35:40.932625 kubeinfra-0.0.1a4/kubeinfra/error.py
+-rw-r--r--   0        0        0    13449 2024-05-13 05:35:40.914117 kubeinfra-0.0.1a4/kubeinfra/files.py
+-rw-r--r--   0        0        0    12222 2024-05-12 08:54:56.067084 kubeinfra-0.0.1a4/kubeinfra/finetune.py
+-rw-r--r--   0        0        0   280722 2024-05-12 08:54:56.066787 kubeinfra-0.0.1a4/kubeinfra/image-0.png
+-rw-r--r--   0        0        0     1110 2024-05-12 08:54:56.067284 kubeinfra-0.0.1a4/kubeinfra/image.py
+-rw-r--r--   0        0        0   323993 2024-05-13 05:35:40.925821 kubeinfra-0.0.1a4/kubeinfra/models.json
+-rw-r--r--   0        0        0     3083 2024-05-12 08:54:56.049007 kubeinfra-0.0.1a4/kubeinfra/models.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:54:56.045650 kubeinfra-0.0.1a4/kubeinfra/tools/__init__.py
+-rw-r--r--   0        0        0      187 2024-05-12 08:54:56.047719 kubeinfra-0.0.1a4/kubeinfra/tools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      182 2024-05-13 02:42:11.601564 kubeinfra-0.0.1a4/kubeinfra/tools/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5094 2024-05-12 08:54:56.046794 kubeinfra-0.0.1a4/kubeinfra/tools/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0        0        0     4633 2024-05-13 02:42:11.602781 kubeinfra-0.0.1a4/kubeinfra/tools/__pycache__/conversation.cpython-312.pyc
+-rw-r--r--   0        0        0     2734 2024-05-13 05:35:40.931512 kubeinfra-0.0.1a4/kubeinfra/tools/conversation.py
+-rw-r--r--   0        0        0     3064 2024-05-13 05:35:40.934189 kubeinfra-0.0.1a4/kubeinfra/types.py
+-rw-r--r--   0        0        0     5064 2024-05-13 05:35:40.909542 kubeinfra-0.0.1a4/kubeinfra/utils.py
+-rw-r--r--   0        0        0      160 2024-05-12 08:54:56.048492 kubeinfra-0.0.1a4/kubeinfra/version.py
+-rw-r--r--   0        0        0      447 2024-05-13 06:58:47.101187 kubeinfra-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 kubeinfra-0.0.1a4/PKG-INFO
```

### Comparing `kubeinfra-0.0.1a3/kubeinfra/__init__.py` & `kubeinfra-0.0.1a4/kubeinfra/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 api_base_openai = urllib.parse.urljoin(api_base, "/v1")
 api_base_complete = urllib.parse.urljoin(api_base, "/v1/chat/completions")
 api_base_files = urllib.parse.urljoin(api_base, "/v1/files/")
 api_base_finetune = urllib.parse.urljoin(api_base, "/v1/fine-tunes/")
 api_base_instances = urllib.parse.urljoin(api_base, "instances/")
 api_base_embeddings = urllib.parse.urljoin(api_base, "api/v1/embeddings")
 
-print("############")
 default_text_model = "mistralai/Mistral-7B-Instruct-v0.2"
 default_image_model = "runwayml/stable-diffusion-v1-5"
 default_embedding_model = "kubeinfracomputer/bert-base-uncased"
 log_level = "WARNING"
 
 MISSING_API_KEY_MESSAGE = """KUBEINFRA_API_KEY not found.
 Please set it as an environment variable or set it as kubeinfra.api_key
```

### Comparing `kubeinfra-0.0.1a3/kubeinfra/cli/__pycache__/cli.cpython-311.pyc` & `kubeinfra-0.0.1a4/kubeinfra/cli/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/cli/cli.py` & `kubeinfra-0.0.1a4/kubeinfra/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/chat.cpython-311.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/chat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/chat.cpython-312.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/chat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/complete.cpython-311.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/complete.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/complete.cpython-312.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/complete.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/embeddings.cpython-311.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/embeddings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/embeddings.cpython-312.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/embeddings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/files.cpython-311.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/files.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/files.cpython-312.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/files.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/finetune.cpython-311.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/finetune.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/finetune.cpython-312.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/finetune.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/image.cpython-311.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/image.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/image.cpython-312.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/image.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/models.cpython-311.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/__pycache__/models.cpython-312.pyc` & `kubeinfra-0.0.1a4/kubeinfra/commands/__pycache__/models.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/chat.py` & `kubeinfra-0.0.1a4/kubeinfra/commands/chat.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             return line[1:]
         else:
             return "say " + line
 
     def do_say(self, arg: str) -> None:
         self._convo.push_human_turn(arg)
         output = ""
-        print("######",self.args)
+#         print("######",self.args)
         try:
             for token in self.infer.create_openai_streaming(
                 prompt=self._convo.get_raw_prompt(),
                 model=self.args.model,
                 max_tokens=self.args.max_tokens,
                 stop=self.args.stop,
                 temperature=self.args.temperature,
```

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/complete.py` & `kubeinfra-0.0.1a4/kubeinfra/commands/complete.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/embeddings.py` & `kubeinfra-0.0.1a4/kubeinfra/commands/embeddings.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/files.py` & `kubeinfra-0.0.1a4/kubeinfra/commands/files.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/finetune.py` & `kubeinfra-0.0.1a4/kubeinfra/commands/finetune.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/image.py` & `kubeinfra-0.0.1a4/kubeinfra/commands/image.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/commands/models.py` & `kubeinfra-0.0.1a4/kubeinfra/commands/models.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/complete.py` & `kubeinfra-0.0.1a4/kubeinfra/complete.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             model = kubeinfra.default_text_model
         
         openai_client = OpenAI(
             api_key=kubeinfra.api_key,
             base_url=kubeinfra.api_base_openai,
         )
         messages = Conversation.get_messages(prompt)
-        print("[+]", len(messages))
+        #print("[+]", len(messages))
 
         for item in openai_client.chat.completions.create(
             model=model,
             messages=messages,
             stream=True
         ):
             text = item.choices[0].delta.content
```

### Comparing `kubeinfra-0.0.1a3/kubeinfra/embeddings.py` & `kubeinfra-0.0.1a4/kubeinfra/embeddings.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/error.py` & `kubeinfra-0.0.1a4/kubeinfra/error.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/files.py` & `kubeinfra-0.0.1a4/kubeinfra/files.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/finetune.py` & `kubeinfra-0.0.1a4/kubeinfra/finetune.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/image-0.png` & `kubeinfra-0.0.1a4/kubeinfra/image-0.png`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/image.py` & `kubeinfra-0.0.1a4/kubeinfra/image.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/models.json` & `kubeinfra-0.0.1a4/kubeinfra/models.json`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/models.py` & `kubeinfra-0.0.1a4/kubeinfra/models.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/tools/__pycache__/conversation.cpython-311.pyc` & `kubeinfra-0.0.1a4/kubeinfra/tools/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/tools/__pycache__/conversation.cpython-312.pyc` & `kubeinfra-0.0.1a4/kubeinfra/tools/__pycache__/conversation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/tools/conversation.py` & `kubeinfra-0.0.1a4/kubeinfra/tools/conversation.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/types.py` & `kubeinfra-0.0.1a4/kubeinfra/types.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/kubeinfra/utils.py` & `kubeinfra-0.0.1a4/kubeinfra/utils.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a3/PKG-INFO` & `kubeinfra-0.0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kubeinfra
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: 
 Author: liuf
 Author-email: liuf@kubesphere.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

