# Comparing `tmp/kubeinfra-0.0.1a1.tar.gz` & `tmp/kubeinfra-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubeinfra-0.0.1a1.tar", max compression
+gzip compressed data, was "kubeinfra-0.0.1a2.tar", max compression
```

## Comparing `kubeinfra-0.0.1a1.tar` & `kubeinfra-0.0.1a2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       11 2024-05-13 05:36:29.658053 kubeinfra-0.0.1a1/README.md
--rw-r--r--   0        0        0     2414 2024-05-13 05:56:27.467619 kubeinfra-0.0.1a1/kubeinfra/__init__.py
--rw-r--r--   0        0        0        0 2024-05-12 08:54:56.058848 kubeinfra-0.0.1a1/kubeinfra/cli/__init__.py
--rw-r--r--   0        0        0      184 2024-05-12 08:54:56.059502 kubeinfra-0.0.1a1/kubeinfra/cli/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2802 2024-05-12 08:54:56.059252 kubeinfra-0.0.1a1/kubeinfra/cli/__pycache__/cli.cpython-311.pyc
--rw-r--r--   0        0        0     1666 2024-05-13 05:35:40.940381 kubeinfra-0.0.1a1/kubeinfra/cli/cli.py
--rw-r--r--   0        0        0        0 2024-05-12 08:54:56.061195 kubeinfra-0.0.1a1/kubeinfra/commands/__init__.py
--rw-r--r--   0        0        0      190 2024-05-12 08:54:56.065047 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      185 2024-05-13 02:42:11.732495 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     7333 2024-05-12 08:54:56.062099 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/chat.cpython-311.pyc
--rw-r--r--   0        0        0     6848 2024-05-13 02:42:11.733367 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/chat.cpython-312.pyc
--rw-r--r--   0        0        0     7805 2024-05-12 08:54:56.064241 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/complete.cpython-311.pyc
--rw-r--r--   0        0        0     7189 2024-05-13 02:42:11.736672 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/complete.cpython-312.pyc
--rw-r--r--   0        0        0     2450 2024-05-12 08:54:56.063176 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/embeddings.cpython-311.pyc
--rw-r--r--   0        0        0     2110 2024-05-13 02:42:11.737143 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/embeddings.cpython-312.pyc
--rw-r--r--   0        0        0    10030 2024-05-12 08:54:56.063454 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/files.cpython-311.pyc
--rw-r--r--   0        0        0     8705 2024-05-13 02:42:11.738167 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/files.cpython-312.pyc
--rw-r--r--   0        0        0    16007 2024-05-12 08:54:56.061856 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/finetune.cpython-311.pyc
--rw-r--r--   0        0        0    14266 2024-05-13 02:42:11.742232 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/finetune.cpython-312.pyc
--rw-r--r--   0        0        0     6278 2024-05-12 08:54:56.063315 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/image.cpython-311.pyc
--rw-r--r--   0        0        0     5579 2024-05-13 02:42:11.742959 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/image.cpython-312.pyc
--rw-r--r--   0        0        0    10173 2024-05-12 08:54:56.064107 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     8829 2024-05-13 02:42:11.743922 kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/models.cpython-312.pyc
--rw-r--r--   0        0        0     4392 2024-05-12 08:54:56.065302 kubeinfra-0.0.1a1/kubeinfra/commands/chat.py
--rw-r--r--   0        0        0     5849 2024-05-13 05:35:40.930157 kubeinfra-0.0.1a1/kubeinfra/commands/complete.py
--rw-r--r--   0        0        0     1182 2024-05-12 08:54:56.065517 kubeinfra-0.0.1a1/kubeinfra/commands/embeddings.py
--rw-r--r--   0        0        0     5905 2024-05-12 08:54:56.060860 kubeinfra-0.0.1a1/kubeinfra/commands/files.py
--rw-r--r--   0        0        0    11262 2024-05-12 08:54:56.066080 kubeinfra-0.0.1a1/kubeinfra/commands/finetune.py
--rw-r--r--   0        0        0     4019 2024-05-13 05:35:40.911922 kubeinfra-0.0.1a1/kubeinfra/commands/image.py
--rw-r--r--   0        0        0     6221 2024-05-12 08:54:56.061115 kubeinfra-0.0.1a1/kubeinfra/commands/models.py
--rw-r--r--   0        0        0     9544 2024-05-13 05:35:40.937393 kubeinfra-0.0.1a1/kubeinfra/complete.py
--rw-r--r--   0        0        0     1889 2024-05-12 08:54:56.059927 kubeinfra-0.0.1a1/kubeinfra/embeddings.py
--rw-r--r--   0        0        0     2647 2024-05-13 05:35:40.932625 kubeinfra-0.0.1a1/kubeinfra/error.py
--rw-r--r--   0        0        0    13449 2024-05-13 05:35:40.914117 kubeinfra-0.0.1a1/kubeinfra/files.py
--rw-r--r--   0        0        0    12222 2024-05-12 08:54:56.067084 kubeinfra-0.0.1a1/kubeinfra/finetune.py
--rw-r--r--   0        0        0   280722 2024-05-12 08:54:56.066787 kubeinfra-0.0.1a1/kubeinfra/image-0.png
--rw-r--r--   0        0        0     1110 2024-05-12 08:54:56.067284 kubeinfra-0.0.1a1/kubeinfra/image.py
--rw-r--r--   0        0        0   323993 2024-05-13 05:35:40.925821 kubeinfra-0.0.1a1/kubeinfra/models.json
--rw-r--r--   0        0        0     3083 2024-05-12 08:54:56.049007 kubeinfra-0.0.1a1/kubeinfra/models.py
--rw-r--r--   0        0        0        0 2024-05-12 08:54:56.045650 kubeinfra-0.0.1a1/kubeinfra/tools/__init__.py
--rw-r--r--   0        0        0      187 2024-05-12 08:54:56.047719 kubeinfra-0.0.1a1/kubeinfra/tools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      182 2024-05-13 02:42:11.601564 kubeinfra-0.0.1a1/kubeinfra/tools/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0        0        0     5094 2024-05-12 08:54:56.046794 kubeinfra-0.0.1a1/kubeinfra/tools/__pycache__/conversation.cpython-311.pyc
--rw-r--r--   0        0        0     4633 2024-05-13 02:42:11.602781 kubeinfra-0.0.1a1/kubeinfra/tools/__pycache__/conversation.cpython-312.pyc
--rw-r--r--   0        0        0     2734 2024-05-13 05:35:40.931512 kubeinfra-0.0.1a1/kubeinfra/tools/conversation.py
--rw-r--r--   0        0        0     3064 2024-05-13 05:35:40.934189 kubeinfra-0.0.1a1/kubeinfra/types.py
--rw-r--r--   0        0        0     5064 2024-05-13 05:35:40.909542 kubeinfra-0.0.1a1/kubeinfra/utils.py
--rw-r--r--   0        0        0      160 2024-05-12 08:54:56.048492 kubeinfra-0.0.1a1/kubeinfra/version.py
--rw-r--r--   0        0        0      389 2024-05-13 06:01:09.748953 kubeinfra-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0      541 1970-01-01 00:00:00.000000 kubeinfra-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0       11 2024-05-13 05:36:29.658053 kubeinfra-0.0.1a2/README.md
+-rw-r--r--   0        0        0     2414 2024-05-13 05:56:27.467619 kubeinfra-0.0.1a2/kubeinfra/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:54:56.058848 kubeinfra-0.0.1a2/kubeinfra/cli/__init__.py
+-rw-r--r--   0        0        0      184 2024-05-12 08:54:56.059502 kubeinfra-0.0.1a2/kubeinfra/cli/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2802 2024-05-12 08:54:56.059252 kubeinfra-0.0.1a2/kubeinfra/cli/__pycache__/cli.cpython-311.pyc
+-rw-r--r--   0        0        0     1666 2024-05-13 05:35:40.940381 kubeinfra-0.0.1a2/kubeinfra/cli/cli.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:54:56.061195 kubeinfra-0.0.1a2/kubeinfra/commands/__init__.py
+-rw-r--r--   0        0        0      190 2024-05-12 08:54:56.065047 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      185 2024-05-13 02:42:11.732495 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     7333 2024-05-12 08:54:56.062099 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/chat.cpython-311.pyc
+-rw-r--r--   0        0        0     6848 2024-05-13 02:42:11.733367 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/chat.cpython-312.pyc
+-rw-r--r--   0        0        0     7805 2024-05-12 08:54:56.064241 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/complete.cpython-311.pyc
+-rw-r--r--   0        0        0     7189 2024-05-13 02:42:11.736672 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/complete.cpython-312.pyc
+-rw-r--r--   0        0        0     2450 2024-05-12 08:54:56.063176 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/embeddings.cpython-311.pyc
+-rw-r--r--   0        0        0     2110 2024-05-13 02:42:11.737143 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/embeddings.cpython-312.pyc
+-rw-r--r--   0        0        0    10030 2024-05-12 08:54:56.063454 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/files.cpython-311.pyc
+-rw-r--r--   0        0        0     8705 2024-05-13 02:42:11.738167 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/files.cpython-312.pyc
+-rw-r--r--   0        0        0    16007 2024-05-12 08:54:56.061856 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/finetune.cpython-311.pyc
+-rw-r--r--   0        0        0    14266 2024-05-13 02:42:11.742232 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/finetune.cpython-312.pyc
+-rw-r--r--   0        0        0     6278 2024-05-12 08:54:56.063315 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/image.cpython-311.pyc
+-rw-r--r--   0        0        0     5579 2024-05-13 02:42:11.742959 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/image.cpython-312.pyc
+-rw-r--r--   0        0        0    10173 2024-05-12 08:54:56.064107 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     8829 2024-05-13 02:42:11.743922 kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/models.cpython-312.pyc
+-rw-r--r--   0        0        0     4392 2024-05-12 08:54:56.065302 kubeinfra-0.0.1a2/kubeinfra/commands/chat.py
+-rw-r--r--   0        0        0     5849 2024-05-13 05:35:40.930157 kubeinfra-0.0.1a2/kubeinfra/commands/complete.py
+-rw-r--r--   0        0        0     1182 2024-05-12 08:54:56.065517 kubeinfra-0.0.1a2/kubeinfra/commands/embeddings.py
+-rw-r--r--   0        0        0     5905 2024-05-12 08:54:56.060860 kubeinfra-0.0.1a2/kubeinfra/commands/files.py
+-rw-r--r--   0        0        0    11262 2024-05-12 08:54:56.066080 kubeinfra-0.0.1a2/kubeinfra/commands/finetune.py
+-rw-r--r--   0        0        0     4019 2024-05-13 05:35:40.911922 kubeinfra-0.0.1a2/kubeinfra/commands/image.py
+-rw-r--r--   0        0        0     6221 2024-05-12 08:54:56.061115 kubeinfra-0.0.1a2/kubeinfra/commands/models.py
+-rw-r--r--   0        0        0     9544 2024-05-13 05:35:40.937393 kubeinfra-0.0.1a2/kubeinfra/complete.py
+-rw-r--r--   0        0        0     1889 2024-05-12 08:54:56.059927 kubeinfra-0.0.1a2/kubeinfra/embeddings.py
+-rw-r--r--   0        0        0     2647 2024-05-13 05:35:40.932625 kubeinfra-0.0.1a2/kubeinfra/error.py
+-rw-r--r--   0        0        0    13449 2024-05-13 05:35:40.914117 kubeinfra-0.0.1a2/kubeinfra/files.py
+-rw-r--r--   0        0        0    12222 2024-05-12 08:54:56.067084 kubeinfra-0.0.1a2/kubeinfra/finetune.py
+-rw-r--r--   0        0        0   280722 2024-05-12 08:54:56.066787 kubeinfra-0.0.1a2/kubeinfra/image-0.png
+-rw-r--r--   0        0        0     1110 2024-05-12 08:54:56.067284 kubeinfra-0.0.1a2/kubeinfra/image.py
+-rw-r--r--   0        0        0   323993 2024-05-13 05:35:40.925821 kubeinfra-0.0.1a2/kubeinfra/models.json
+-rw-r--r--   0        0        0     3083 2024-05-12 08:54:56.049007 kubeinfra-0.0.1a2/kubeinfra/models.py
+-rw-r--r--   0        0        0        0 2024-05-12 08:54:56.045650 kubeinfra-0.0.1a2/kubeinfra/tools/__init__.py
+-rw-r--r--   0        0        0      187 2024-05-12 08:54:56.047719 kubeinfra-0.0.1a2/kubeinfra/tools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      182 2024-05-13 02:42:11.601564 kubeinfra-0.0.1a2/kubeinfra/tools/__pycache__/__init__.cpython-312.pyc
+-rw-r--r--   0        0        0     5094 2024-05-12 08:54:56.046794 kubeinfra-0.0.1a2/kubeinfra/tools/__pycache__/conversation.cpython-311.pyc
+-rw-r--r--   0        0        0     4633 2024-05-13 02:42:11.602781 kubeinfra-0.0.1a2/kubeinfra/tools/__pycache__/conversation.cpython-312.pyc
+-rw-r--r--   0        0        0     2734 2024-05-13 05:35:40.931512 kubeinfra-0.0.1a2/kubeinfra/tools/conversation.py
+-rw-r--r--   0        0        0     3064 2024-05-13 05:35:40.934189 kubeinfra-0.0.1a2/kubeinfra/types.py
+-rw-r--r--   0        0        0     5064 2024-05-13 05:35:40.909542 kubeinfra-0.0.1a2/kubeinfra/utils.py
+-rw-r--r--   0        0        0      160 2024-05-12 08:54:56.048492 kubeinfra-0.0.1a2/kubeinfra/version.py
+-rw-r--r--   0        0        0      387 2024-05-13 06:15:18.135007 kubeinfra-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 kubeinfra-0.0.1a2/PKG-INFO
```

### Comparing `kubeinfra-0.0.1a1/kubeinfra/__init__.py` & `kubeinfra-0.0.1a2/kubeinfra/__init__.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/cli/__pycache__/cli.cpython-311.pyc` & `kubeinfra-0.0.1a2/kubeinfra/cli/__pycache__/cli.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/cli/cli.py` & `kubeinfra-0.0.1a2/kubeinfra/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/chat.cpython-311.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/chat.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/chat.cpython-312.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/chat.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/complete.cpython-311.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/complete.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/complete.cpython-312.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/complete.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/embeddings.cpython-311.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/embeddings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/embeddings.cpython-312.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/embeddings.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/files.cpython-311.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/files.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/files.cpython-312.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/files.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/finetune.cpython-311.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/finetune.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/finetune.cpython-312.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/finetune.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/image.cpython-311.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/image.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/image.cpython-312.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/image.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/models.cpython-311.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/__pycache__/models.cpython-312.pyc` & `kubeinfra-0.0.1a2/kubeinfra/commands/__pycache__/models.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/chat.py` & `kubeinfra-0.0.1a2/kubeinfra/commands/chat.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/complete.py` & `kubeinfra-0.0.1a2/kubeinfra/commands/complete.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/embeddings.py` & `kubeinfra-0.0.1a2/kubeinfra/commands/embeddings.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/files.py` & `kubeinfra-0.0.1a2/kubeinfra/commands/files.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/finetune.py` & `kubeinfra-0.0.1a2/kubeinfra/commands/finetune.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/image.py` & `kubeinfra-0.0.1a2/kubeinfra/commands/image.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/commands/models.py` & `kubeinfra-0.0.1a2/kubeinfra/commands/models.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/complete.py` & `kubeinfra-0.0.1a2/kubeinfra/complete.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/embeddings.py` & `kubeinfra-0.0.1a2/kubeinfra/embeddings.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/error.py` & `kubeinfra-0.0.1a2/kubeinfra/error.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/files.py` & `kubeinfra-0.0.1a2/kubeinfra/files.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/finetune.py` & `kubeinfra-0.0.1a2/kubeinfra/finetune.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/image-0.png` & `kubeinfra-0.0.1a2/kubeinfra/image-0.png`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/image.py` & `kubeinfra-0.0.1a2/kubeinfra/image.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/models.json` & `kubeinfra-0.0.1a2/kubeinfra/models.json`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/models.py` & `kubeinfra-0.0.1a2/kubeinfra/models.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/tools/__pycache__/conversation.cpython-311.pyc` & `kubeinfra-0.0.1a2/kubeinfra/tools/__pycache__/conversation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/tools/__pycache__/conversation.cpython-312.pyc` & `kubeinfra-0.0.1a2/kubeinfra/tools/__pycache__/conversation.cpython-312.pyc`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/tools/conversation.py` & `kubeinfra-0.0.1a2/kubeinfra/tools/conversation.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/types.py` & `kubeinfra-0.0.1a2/kubeinfra/types.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/kubeinfra/utils.py` & `kubeinfra-0.0.1a2/kubeinfra/utils.py`

 * *Files identical despite different names*

### Comparing `kubeinfra-0.0.1a1/PKG-INFO` & `kubeinfra-0.0.1a2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 Metadata-Version: 2.1
 Name: kubeinfra
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: 
 Author: liuf
 Author-email: liuf@kubesphere.io
-Requires-Python: >=3.12,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.5,<4.0.0)
 Requires-Dist: openai (>=1.28.0,<2.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: sseclient (>=0.0.27,<0.0.28)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
```

