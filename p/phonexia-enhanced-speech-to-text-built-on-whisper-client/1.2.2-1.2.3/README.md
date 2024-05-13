# Comparing `tmp/phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2.tar.gz` & `tmp/phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2.tar", max compression
+gzip compressed data, was "phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3.tar", max compression
```

## Comparing `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2.tar` & `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     8232 2024-05-01 05:34:07.388529 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2/phonexia_enhanced_speech_to_text_built_on_whisper_client.py
--rw-r--r--   0        0        0     1118 2024-05-01 05:34:07.388529 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2/pypi-README.md
--rw-r--r--   0        0        0     2062 2024-05-01 05:34:25.137745 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     8232 2024-05-13 11:07:44.890236 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/phonexia_enhanced_speech_to_text_built_on_whisper_client.py
+-rw-r--r--   0        0        0     1118 2024-05-13 11:07:44.890236 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/pypi-README.md
+-rw-r--r--   0        0        0     2062 2024-05-13 11:08:20.704742 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2118 1970-01-01 00:00:00.000000 phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/PKG-INFO
```

### Comparing `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2/phonexia_enhanced_speech_to_text_built_on_whisper_client.py` & `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/phonexia_enhanced_speech_to_text_built_on_whisper_client.py`

 * *Files identical despite different names*

### Comparing `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2/pypi-README.md` & `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/pypi-README.md`

 * *Files identical despite different names*

### Comparing `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2/pyproject.toml` & `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phonexia-enhanced-speech-to-text-built-on-whisper-client"
-version = "1.2.2"
+version = "1.2.3"
 description = "Client for communication with Phonexia Enhanced Speech To Text Built On Whisper microservice."
 readme = "pypi-README.md"
 keywords = ["grpc", "transcription", "STT", "ASR", "speech to text", "speech", "language", "microservice"]
 authors = ["Phonexia <info@phonexia.com>"]
 
 [tool.poetry.urls]
 Homepage = "https://phonexia.com"
```

### Comparing `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.2/PKG-INFO` & `phonexia_enhanced_speech_to_text_built_on_whisper_client-1.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phonexia-enhanced-speech-to-text-built-on-whisper-client
-Version: 1.2.2
+Version: 1.2.3
 Summary: Client for communication with Phonexia Enhanced Speech To Text Built On Whisper microservice.
 Keywords: grpc,transcription,STT,ASR,speech to text,speech,language,microservice
 Author: Phonexia
 Author-email: info@phonexia.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

