# Comparing `tmp/llm_taxi-0.0.0.tar.gz` & `tmp/llm_taxi-0.1.0.tar.gz`

## Comparing `llm_taxi-0.0.0.tar` & `llm_taxi-0.1.0.tar`

### file list

```diff
@@ -1,6 +1,25 @@
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 llm_taxi-0.0.0/.python-version
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 llm_taxi-0.0.0/src/llm_taxi/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 llm_taxi-0.0.0/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_taxi-0.0.0/README.md
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 llm_taxi-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 llm_taxi-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/.python-version
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/pyrightconfig.json
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/requirements-dev.lock
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/requirements.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/conversation.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/factory.py
+-rw-r--r--   0        0        0      715 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/__init__.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/anthropic.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/base.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/dashscope.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/deepinfra.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/deepseek.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/google.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/groq.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/mistral.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/openai.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/openrouter.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/perplexity.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/src/llm_taxi/llms/together.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/tests/test_llm.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 llm_taxi-0.1.0/PKG-INFO
```

