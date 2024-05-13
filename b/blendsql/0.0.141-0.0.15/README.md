# Comparing `tmp/blendsql-0.0.141.tar.gz` & `tmp/blendsql-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blendsql-0.0.141.tar", last modified: Fri May 10 17:30:06 2024, max compression
+gzip compressed data, was "blendsql-0.0.15.tar", last modified: Mon May 13 21:39:37 2024, max compression
```

## Comparing `blendsql-0.0.141.tar` & `blendsql-0.0.15.tar`

### file list

```diff
@@ -1,69 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.479534 blendsql-0.0.141/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-10 17:30:02.000000 blendsql-0.0.141/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26517 2024-05-10 17:30:06.479534 blendsql-0.0.141/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24889 2024-05-10 17:30:02.000000 blendsql-0.0.141/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.471534 blendsql-0.0.141/blendsql/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/_dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/_grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/_program.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/_smoothie.py
--rw-r--r--   0 runner    (1001) docker     (127)    27335 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/_sqlglot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/blend_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    40768 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/blendsql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/db/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/db/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/db/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/ingredients/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/ingredients/builtin/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/ingredients/builtin/dt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/dt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/dt/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/dt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/ingredients/builtin/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/llm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/ingredients/builtin/llm/join/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/llm/join/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/llm/join/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/ingredients/builtin/llm/map/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/llm/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/llm/map/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/ingredients/builtin/llm/qa/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/llm/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/llm/qa/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/llm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/ingredients/builtin/llm/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/llm/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/builtin/llm/validate/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/ingredients/ingredient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/models/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/models/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/models/local/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/models/local/_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.475534 blendsql-0.0.141/blendsql/models/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/models/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/models/remote/_openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-10 17:30:02.000000 blendsql-0.0.141/blendsql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.479534 blendsql-0.0.141/blendsql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26517 2024-05-10 17:30:06.000000 blendsql-0.0.141/blendsql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-10 17:30:06.000000 blendsql-0.0.141/blendsql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 17:30:06.000000 blendsql-0.0.141/blendsql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-10 17:30:06.000000 blendsql-0.0.141/blendsql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-10 17:30:06.000000 blendsql-0.0.141/blendsql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-10 17:30:06.000000 blendsql-0.0.141/blendsql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-10 17:30:02.000000 blendsql-0.0.141/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 17:30:06.479534 blendsql-0.0.141/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-05-10 17:30:02.000000 blendsql-0.0.141/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:06.479534 blendsql-0.0.141/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 17:30:02.000000 blendsql-0.0.141/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-10 17:30:02.000000 blendsql-0.0.141/tests/test_generic_blendsql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-05-10 17:30:02.000000 blendsql-0.0.141/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    16381 2024-05-10 17:30:02.000000 blendsql-0.0.141/tests/test_multi_table_blendsql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14557 2024-05-10 17:30:02.000000 blendsql-0.0.141/tests/test_single_table_blendsql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-05-10 17:30:02.000000 blendsql-0.0.141/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.787083 blendsql-0.0.15/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 21:39:33.000000 blendsql-0.0.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    29129 2024-05-13 21:39:37.787083 blendsql-0.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27308 2024-05-13 21:39:33.000000 blendsql-0.0.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.771083 blendsql-0.0.15/blendsql/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/_dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3343 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/_smoothie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27468 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/_sqlglot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38968 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/blend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/blend_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.775083 blendsql-0.0.15/blendsql/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/db/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/db/_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/db/_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/db/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.775083 blendsql-0.0.15/blendsql/grammars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/_cfg_grammar.lark
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/_peg_grammar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.775083 blendsql-0.0.15/blendsql/grammars/minEarley/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17048 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/earley.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6777 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/earley_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10247 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/earley_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32720 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/earley_forest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/grammars/minEarley/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.775083 blendsql-0.0.15/blendsql/ingredients/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.775083 blendsql-0.0.15/blendsql/ingredients/builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/ingredients/builtin/join/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/join/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/join/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/ingredients/builtin/map/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/map/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/ingredients/builtin/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/qa/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/ingredients/builtin/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/builtin/validate/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14470 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/ingredients/ingredient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/models/local/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/local/_llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/local/_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/models/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/models/remote/_openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/nl_to_blendsql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/blendsql/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/prompts/_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-13 21:39:33.000000 blendsql-0.0.15/blendsql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.787083 blendsql-0.0.15/blendsql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29129 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 21:39:37.000000 blendsql-0.0.15/blendsql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-13 21:39:33.000000 blendsql-0.0.15/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.767083 blendsql-0.0.15/research/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/research/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.779083 blendsql-0.0.15/research/prompts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/prompts/end_to_end_program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/prompts/parser_program.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/bridge_content_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8180 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/dataset_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/fetaqa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/fetaqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/fetaqa/fetaqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/feverous/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/feverous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/feverous/feverous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/hybridqa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/hybridqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5634 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/hybridqa/hybridqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/normalizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/ottqa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/ottqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/ottqa/ottqa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/sql/all_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21210 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/sql/extraction_from_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18590 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/sql/process_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.783083 blendsql-0.0.15/research/utils/wikitq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/wikitq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/wikitq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-13 21:39:33.000000 blendsql-0.0.15/research/utils/wikitq/wikitq.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:39:37.791082 blendsql-0.0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-13 21:39:33.000000 blendsql-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:37.787083 blendsql-0.0.15/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_end_to_end.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_generic_blendsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17415 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_multi_table_blendsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15715 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/test_single_table_blendsql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-13 21:39:33.000000 blendsql-0.0.15/tests/utils.py
```

### Comparing `blendsql-0.0.141/LICENSE` & `blendsql-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.141/PKG-INFO` & `blendsql-0.0.15/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
 Name: blendsql
-Version: 0.0.141
-Summary: Orchestrate SQLite logic and LLM reasoning within a unified dialect.
+Version: 0.0.15
+Summary: Query language to blend SQL logic and LLM reasoning across multi-modal data.
 Home-page: https://github.com/parkervg/blendsql
 Author: Parker Glenn
 Author-email: parkervg5@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: guidance>=0.1.0
 Requires-Dist: pyparsing==3.1.1
-Requires-Dist: pandas>=2.0.0
+Requires-Dist: pandas==1.5.3
 Requires-Dist: bottleneck>=1.3.6
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: sqlglot==18.13.0
+Requires-Dist: sqlalchemy>=2.0.0
 Requires-Dist: platformdirs
-Requires-Dist: pre-commit
 Requires-Dist: attrs
 Requires-Dist: tqdm
-Requires-Dist: dateparser
 Requires-Dist: colorama
-Requires-Dist: fiscalyear
 Requires-Dist: tabulate
 Requires-Dist: typeguard
+Provides-Extra: nl-to-blendsql
+Requires-Dist: exrex; extra == "nl-to-blendsql"
+Requires-Dist: lark; extra == "nl-to-blendsql"
 Provides-Extra: research
 Requires-Dist: datasets==2.16.1; extra == "research"
 Requires-Dist: nltk; extra == "research"
 Requires-Dist: wikiextractor; extra == "research"
 Requires-Dist: rouge_score; extra == "research"
 Requires-Dist: rapidfuzz; extra == "research"
 Requires-Dist: records; extra == "research"
 Requires-Dist: SQLAlchemy; extra == "research"
 Requires-Dist: recognizers-text; extra == "research"
 Requires-Dist: recognizers-text-suite; extra == "research"
 Requires-Dist: emoji==1.7.0; extra == "research"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: huggingface_hub; extra == "test"
+Requires-Dist: pre-commit; extra == "test"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings; extra == "docs"
 Requires-Dist: mkdocs-section-index; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 Requires-Dist: mkdocs-jupyter; extra == "docs"
+Provides-Extra: demo
+Requires-Dist: chainlit; extra == "demo"
 
 <div align="right">
 <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" /></a>
 <a><img src="https://img.shields.io/github/last-commit/parkervg/blendsql?color=green"/></a>
 <a><img src="https://img.shields.io/badge/PRs-Welcome-Green"/></a>
 <br>
 </div>
@@ -57,17 +61,28 @@
 </picture>
 <p align="center">
     <i> SQL 🤝 LLMs </i>
   </p>
 <b>Check out our <a href="https://parkervg.github.io/blendsql/" target="_blank">online documentation</a> for a more comprehensive overview.</b>
 
 <i>Results from the paper are available [here](https://github.com/parkervg/blendsql/tree/research-paper/research/paper-results)</i>
+
 </div>
 <br/>
 
+### Features
+
+- Supports many DBMS 💾
+  - Currently, SQLite and PostgreSQL are functional - more to come! 
+- Easily extendable to [multi-modal usecases](./examples/vqa-ingredient.ipynb) 🖼️
+- Smart parsing optimizes what is passed to external functions 🧠
+  - Traverses abstract syntax tree with [sqlglot](https://github.com/tobymao/sqlglot) to minimize LLM function calls 🌳
+- Constrained decoding with [guidance](https://github.com/guidance-ai/guidance) 🚀
+- LLM function caching, built on [diskcache](https://grantjenks.com/docs/diskcache/) 🔑
+
 ## Intro
 BlendSQL is a *superset of SQLite* for problem decomposition and hybrid question-answering with LLMs. 
 
 As a result, we can *Blend* together...
 
 - 🥤 ...operations over heterogeneous data sources (e.g. tables, text, images)
 - 🥤 ...the structured & interpretable reasoning of SQL with the generalizable reasoning of LLMs
@@ -77,59 +92,64 @@
 **Now, the user is given the control to oversee all calls (LLM + SQL) within a unified query language.**
 
 ![comparison](docs/img/comparison.jpg)
 
 For example, imagine we have the following tables.
 
 ### `w`
+
 | **date** | **rival**                 | **city**  | **venue**                   | **score** |
-|----------|---------------------------|-----------|-----------------------------|-----------|
+| -------- | ------------------------- | --------- | --------------------------- | --------- |
 | 31 may   | nsw waratahs              | sydney    | agricultural society ground | 11-0      |
 | 5 jun    | northern districts        | newcastle | sports ground               | 29-0      |
 | 7 jun    | nsw waratahs              | sydney    | agricultural society ground | 21-2      |
 | 11 jun   | western districts         | bathurst  | bathurst ground             | 11-0      |
 | 12 jun   | wallaroo & university nsw | sydney    | cricket ground              | 23-10     |
 
 ### `documents`
+
 | **title**                      | **content**                                       |
-|--------------------------------|---------------------------------------------------|
+| ------------------------------ | ------------------------------------------------- |
 | sydney                         | sydney ( /ˈsɪdni/ ( listen ) sid-nee ) is the ... |
 | new south wales waratahs       | the new south wales waratahs ( /ˈwɒrətɑːz/ or ... |
 | sydney showground (moore park) | the former sydney showground ( moore park ) at... |
 | sydney cricket ground          | the sydney cricket ground ( scg ) is a sports ... |
 | newcastle, new south wales     | the newcastle ( /ˈnuːkɑːsəl/ new-kah-səl ) met... |
 | bathurst, new south wales      | bathurst /ˈbæθərst/ is a city in the central t... |
 
 BlendSQL allows us to ask the following questions by injecting "ingredients", which are callable functions denoted by double curly brackets (`{{`, `}}`).
-The below examples work out of the box, but you are able to design your own ingredients as well! 
+The below examples work out of the box, but you are able to design your own ingredients as well!
+
+_What was the result of the game played 120 miles west of Sydney?_
 
-*What was the result of the game played 120 miles west of Sydney?*
 ```sql
 SELECT * FROM w
     WHERE city = {{
         LLMQA(
             'Which city is located 120 miles west of Sydney?',
             (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
             options='w::city'
         )
     }}
 ```
 
-*Which venues in Sydney saw more than 30 points scored?*
+_Which venues in Sydney saw more than 30 points scored?_
+
 ```sql
 SELECT DISTINCT venue FROM w
     WHERE city = 'sydney' AND {{
         LLMMap(
             'More than 30 total points?',
             'w::score'
         )
     }} = TRUE
 ```
 
-*Show all NSW Waratahs games and a description of the team.*
+_Show all NSW Waratahs games and a description of the team._
+
 ```sql
 SELECT date, rival, score, documents.content AS "Team Description" FROM w
     JOIN {{
         LLMJoin(
             left_on='documents::title',
             right_on='w::rival'
         )
@@ -140,72 +160,76 @@
 
 <p>
 <details>
 <summary> <b> <a href="https://hybridqa.github.io/" target="_blank"> HybridQA </a> </b> </summary>
 
 For this setting, our database contains 2 tables: a table from Wikipedia `w`, and a collection of unstructured Wikipedia articles in the table `documents`.
 
-*What is the state flower of the smallest state by area ?*
+_What is the state flower of the smallest state by area ?_
+
 ```sql
-SELECT "common name" AS 'State Flower' FROM w 
+SELECT "common name" AS 'State Flower' FROM w
 WHERE state = {{
     LLMQA(
         'Which is the smallest state by area?',
         (SELECT title, content FROM documents),
         options='w::state'
     )
 }}
 ```
 
-*Who were the builders of the mosque in Herat with fire temples ?*
+_Who were the builders of the mosque in Herat with fire temples ?_
+
 ```sql
 {{
     LLMQA(
-        'Name of the builders?',
+        'Who were the builders of the mosque?',
         (
-            SELECT title AS 'Building', content FROM documents
-                WHERE title = {{
-                    LLMQA(
-                        'Align the name to the correct title.',
-                        (SELECT name FROM w WHERE city = 'herat' AND remarks LIKE '%fire temple%'),
-                        options='documents::title'
-                    )
-                }}
-        ) 
+            SELECT documents.title AS 'Building', documents.content FROM documents
+            JOIN {{
+                LLMJoin(
+                    left_on='w::name',
+                    right_on='documents::title'
+                )
+            }}
+            WHERE w.city = 'herat' AND w.remarks LIKE '%fire temple%'
+        )
     )
 }}
 ```
 
-*What is the capacity of the venue that was named in honor of Juan Antonio Samaranch in 2010 after his death ?*
+_What is the capacity of the venue that was named in honor of Juan Antonio Samaranch in 2010 after his death ?_
+
 ```sql
 SELECT capacity FROM w WHERE venue = {{
     LLMQA(
         'Which venue is named in honor of Juan Antonio Samaranch?',
         (SELECT title AS 'Venue', content FROM documents),
         options='w::venue'
     )
 }}
-```    
+```
 
 </details>
 </p>
 
 <p>
 <details>
 <summary> <b> <a href="https://ott-qa.github.io/" target="_blank"> OTT-QA </a> </b> </summary>
 
 Unlike HybridQA, these questions are open-domain, where we don't know in advance where the answer of a given open question appears in a passage or a table.
 
 As a result, we need to play the role of both the retriever (to select relevant context) and reader (to read from relevant contexts and return the given answer).
 
 As the underlying database consists of 400K tables and 5M documents, it's important to set `LIMIT` clauses appropriately to ensure reasonable execution times.
 
-The examples below also demonstrate how BlendSQL unpacks [CTE statements](https://www.sqlite.org/lang_with.html) to ensure we only pass necessary data into the BlendSQL ingredient calls. 
+The examples below also demonstrate how BlendSQL unpacks [CTE statements](https://www.sqlite.org/lang_with.html) to ensure we only pass necessary data into the BlendSQL ingredient calls.
+
+_When was the third highest paid Rangers F.C . player born ?_
 
-*When was the third highest paid Rangers F.C . player born ?*
 ```sql
 {{
     LLMQA(
         'When was the Rangers Player born?',
         (
             WITH t AS (
                 SELECT player FROM (
@@ -216,40 +240,42 @@
                 SELECT * FROM documents JOIN t WHERE documents MATCH t.player || ' OR rangers OR fc' ORDER BY rank LIMIT 5
             ) SELECT d.content, t.player AS 'Rangers Player' FROM d JOIN t
         )
     )
 }}
 ```
 
-*In which Track Cycling World Championships event was the person born in Matanzas , Cuba ranked highest ?*
+_In which Track Cycling World Championships event was the person born in Matanzas , Cuba ranked highest ?_
+
 ```sql
 {{
     LLMQA(
         'In what event was the cyclist ranked highest?',
         (
             SELECT * FROM (
                 SELECT * FROM "./Cuba at the UCI Track Cycling World Championships (2)"
             ) as w WHERE w.name = {{
                 LLMQA(
                     "Which cyclist was born in Matanzas, Cuba?",
                     (
-                        SELECT * FROM documents 
-                            WHERE documents MATCH 'matanzas AND (cycling OR track OR born)' 
+                        SELECT * FROM documents
+                            WHERE documents MATCH 'matanzas AND (cycling OR track OR born)'
                             ORDER BY rank LIMIT 3
                     ),
                     options="w::name"
                 )
             }}
         ),
         options='w::event'
     )
 }}
 ```
 
-*Who is the director the Togolese film that was a 30 minute film that was shot in 16mm ?*
+_Who is the director the Togolese film that was a 30 minute film that was shot in 16mm ?_
+
 ```sql
 SELECT director FROM "./List of African films (4)" as w
 WHERE title = {{
     LLMQA(
         'What is the name of the Togolese film that was 30 minutes and shot in 16mm?',
         (SELECT * FROM documents WHERE documents MATCH 'togolese OR 30 OR 16mm OR film' ORDER BY rank LIMIT 5),
         options='w::title'
@@ -262,41 +288,44 @@
 
 <p>
 <details>
 <summary> <b> <a href="https://fever.ai/dataset/feverous.html" target="_blank"> FEVEROUS </a> </b> </summary>
 
 Here, we deal not with questions, but truth claims given a context of unstructured and structured data.
 
-These claims should be judged as "SUPPORTS" or "REFUTES". Using BlendSQL, we can formulate this determination of truth as a function over facts. 
+These claims should be judged as "SUPPORTS" or "REFUTES". Using BlendSQL, we can formulate this determination of truth as a function over facts.
+
+_Oyedaea is part of the family Asteraceae in the order Asterales._
 
-*Oyedaea is part of the family Asteraceae in the order Asterales.*
 ```sql
 SELECT EXISTS (
     SELECT * FROM w0 WHERE "family:" = 'asteraceae' AND "order:" = 'asterales'
-) 
+)
 ```
 
-*The 2006-07 San Jose Sharks season, the 14th season of operation (13th season of play) for the National Hockey League (NHL) franchise, scored the most points in the Pacific Division.*
+_The 2006-07 San Jose Sharks season, the 14th season of operation (13th season of play) for the National Hockey League (NHL) franchise, scored the most points in the Pacific Division._
+
 ```sql
 SELECT (
     {{
         LLMValidate(
-            'Is the Sharks 2006-07 season the 14th season (13th season of play)?', 
+            'Is the Sharks 2006-07 season the 14th season (13th season of play)?',
             (SELECT * FROM documents)
         )
     }}
 ) AND (
     SELECT (SELECT filledcolumnname FROM w0 ORDER BY pts DESC LIMIT 1) = 'san jose sharks'
 )
 ```
 
-*Saunders College of Business, which is accredited by the Association to Advance Collegiate Schools of Business International, is one of the colleges of Rochester Institute of Technology established in 1910 and is currently under the supervision of Dean Jacqueline R. Mozrall.*
+_Saunders College of Business, which is accredited by the Association to Advance Collegiate Schools of Business International, is one of the colleges of Rochester Institute of Technology established in 1910 and is currently under the supervision of Dean Jacqueline R. Mozrall._
+
 ```sql
 SELECT EXISTS(
-    SELECT * FROM w0 
+    SELECT * FROM w0
     WHERE "parent institution" = 'rochester institute of technology'
     AND "established" = '1910'
     AND "dean" = 'jacqueline r. mozrall'
 ) AND (
     {{
         LLMValidate(
             'Is Saunders College of Business (SCB) accredited by the Association to Advance Collegiate Schools of Business International (AACSB)?',
@@ -306,299 +335,339 @@
 )
 ```
 
 </details>
 </p>
 
 ## Table of Contents
-* [Install](#install)
-* [Quickstart](#quickstart)
-* [FAQ](#faq)
-* [Documentation](#documentation)
-  * [Execute a BlendSQL Query](#execute-a-blendsql-query)
-    * [Smoothie](#smoothie)
-  * [Ingredients](#ingredients)
-    * [MapIngredient](#mapingredient)
-    * [QAIngredient](#qaingredient)
-      * [Constrained Decoding with 'options'](#constrained-decoding-with-options)
-    * [JoinIngredient](#joiningredient)
-    * [StringIngredient](#stringingredient)
-  * [LLMs](#llms)
-  * [Databases](#databases)
-* [Appendix](#appendix)
-
-### Features 
-- Smart parsing optimizes what is passed to external functions 🧠
-  - Traverses abstract syntax tree with [sqlglot](https://github.com/tobymao/sqlglot) to minimize LLM function calls 🌳
-- LLM function caching, built on [diskcache](https://grantjenks.com/docs/diskcache/) 🔑 
-- Constrained decoding with [guidance](https://github.com/guidance-ai/guidance) 🚀
 
+- [Install](#install)
+- [Quickstart](#quickstart)
+- [FAQ](#faq)
+- [Documentation](#documentation)
+  - [Execute a BlendSQL Query](#execute-a-blendsql-query)
+    - [Smoothie](#smoothie)
+  - [Ingredients](#ingredients)
+    - [MapIngredient](#mapingredient)
+    - [QAIngredient](#qaingredient)
+      - [Constrained Decoding with 'options'](#constrained-decoding-with-options)
+    - [JoinIngredient](#joiningredient)
+    - [StringIngredient](#stringingredient)
+  - [Parsing Natural Language to BlendSQL](#parsing-natural-language-to-blendsql)
+  - [LLMs](#llms)
+  - [Databases](#databases)
+- [Appendix](#appendix)
 
 For a technical walkthrough of how a BlendSQL query is executed, check out [technical_walkthrough.md](./docs/technical_walkthrough.md).
 
 ## Install
+
 ```
 pip install blendsql
 ```
 
 ## Quickstart
 
 ```python
-from blendsql import blend, LLMQA, LLMMap
+from blendsql import blend, LLMQA
 from blendsql.db import SQLite
 from blendsql.models import OpenaiLLM
+from blendsql.utils import fetch_from_hub
 
 blendsql = """
-SELECT merchant FROM transactions WHERE 
-     {{LLMMap('is this a pizza shop?', 'transactions::merchant')}} = TRUE
-     AND parent_category = 'Food'
+SELECT * FROM w
+WHERE city = {{
+    LLMQA(
+        'Which city is located 120 miles west of Sydney?',
+        (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
+        options='w::city'
+    )
+}}
 """
 # Make our smoothie - the executed BlendSQL script
 smoothie = blend(
     query=blendsql,
-    blender=OpenaiLLM("gpt-3.5-turbo-0613"),
-    ingredients={LLMMap, LLMQA},
-    db=SQLite(db_path="transactions.db"),
-    verbose=True
+    db=SQLite(fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+    blender=OpenaiLLM("gpt-3.5-turbo"),
+    ingredients={LLMQA},
 )
-
+print(smoothie.df)
+print(smoothie.meta.prompts)
 ```
 
 ### FAQ
 
+#### How does BlendSQL execute a query?
+> BlendSQL handles traversal of the SQL AST and creation of temporary tables to execute a given query. 
+> This allows BlendSQL to be DBMS-agnostic, and extendable into both SQLite, PostgreSQL, and other DBMS.
+
 #### Why not just implement BlendSQL as a [user-defined function in SQLite](https://www.sqlite.org/c3ref/c_deterministic.html#sqlitedeterministic)?
-> LLMs are expensive, both in terms of $ cost and compute time. When applying them to SQLite databases, we want to take special care in ensuring we're not applying them to contexts where they're not required. 
+
+> LLMs are expensive, both in terms of $ cost and compute time. When applying them to SQLite databases, we want to take special care in ensuring we're not applying them to contexts where they're not required.
 > This is [not easily achievable with UDFs](https://sqlite.org/forum/info/649ad4c62fd4b4e8cb5d6407107b8c8a9a0afaaf95a87805e5a8403a79e6616c), even when marked as a [deterministic function](https://www.sqlite.org/c3ref/c_deterministic.html#sqlitedeterministic).
-> 
+>
 > BlendSQL is specifically designed to enforce an order-of-operations that 1) prioritizes vanilla SQL operations first, and 2) caches results from LLM ingredients so they don't need to be recomputed.
 > For example:
-> ```sql 
-> SELECT {{LLMMap('What state is this NBA team from?', 'w::team')} FROM w 
->    WHERE num_championships > 3 
+>
+> ```sql
+> SELECT {{LLMMap('What state is this NBA team from?', 'w::team')} FROM w
+>    WHERE num_championships > 3
 >    ORDER BY {{LLMMap('What state is this NBA team from?', 'w::team')}
-> 
+>
 > ```
+>
 > BlendSQL makes sure to only pass those `team` values from rows which satisfy the condition `num_championship > 3` to the LLM. Additionally, since we assume the function is deterministic, we make a single LLM call and cache the results, despite the ingredient function being used twice.
 
+#### So I get how to write BlendSQL queries. But why would I use this over vanilla SQLite?
 
- #### So I get how to write BlendSQL queries. But why would I use this over vanilla SQLite? 
-> Certain ingredients, like [LLMJoin](#joiningredient), will likely give seasoned SQL experts a headache at first. However, BlendSQL's real strength comes from it's use as an *intermediate representation for reasoning over structured + unstructured with LLMs*. Some examples of this can be found above [here](#more-examples-from-popular-qa-datasets).
+> Certain ingredients, like [LLMJoin](#joiningredient), will likely give seasoned SQL experts a headache at first. However, BlendSQL's real strength comes from it's use as an _intermediate representation for reasoning over structured + unstructured with LLMs_. Some examples of this can be found above [here](#more-examples-from-popular-qa-datasets).
 
 <hr>
 
 ### Citation
+
 ```bibtex
 @article{glenn2024blendsql,
-      title={BlendSQL: A Scalable Dialect for Unifying Hybrid Question Answering in Relational Algebra}, 
+      title={BlendSQL: A Scalable Dialect for Unifying Hybrid Question Answering in Relational Algebra},
       author={Parker Glenn and Parag Pravin Dakle and Liang Wang and Preethi Raghavan},
       year={2024},
       eprint={2402.17882},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
 ```
 
 # Documentation
 
-> [!WARNING]
-> WIP, will be updated
+
+## Databases
+
+Since BlendSQL relies on the package [sqlglot](https://github.com/tobymao/sqlglot) for query optimization (which supports a [wide variety of SQL dialects](https://github.com/tobymao/sqlglot/blob/main/sqlglot/dialects/__init__.py)) and the notion of [temporary tables](https://en.wikibooks.org/wiki/Structured_Query_Language/Temporary_Table), it can easily integrate with many different SQL dialects. 
+
+Currently, the following are supported.
+
+### SQLite
+A SQLite database connection.
+Can be initialized via a path to the database file.
+
+Example:
+```python
+from blendsql.db import SQLite
+db = SQLite("./path/to/database.db")
+```
+
+### PostgreSQL
+A PostgreSQL database connection.
+Can be initialized via the SQLAlchemy input string.
+https://docs.sqlalchemy.org/en/20/core/engines.html#postgresql
+
+Example:
+```python
+from blendsql.db import PostgreSQL
+db = PostgreSQL("user:password@localhost/mydatabase")
+```
 
 ## Execute a BlendSQL Query
-The `blend()` function is used to execute a BlendSQL query against a database and return the final result, in addition to the intermediate reasoning steps taken.
 
-::: blendsql.blendsql.blend
-  handler: python
+The `blend()` function is used to execute a BlendSQL query against a database and return the final result, in addition to the intermediate reasoning steps taken.
 
 ```python
-from blendsql import blend, LLMMap, LLMQA, LLMJoin
+from blendsql import blend, LLMQA
 from blendsql.db import SQLite
 from blendsql.models import OpenaiLLM
+from blendsql.utils import fetch_from_hub
 
 blendsql = """
 SELECT * FROM w
 WHERE city = {{
     LLMQA(
         'Which city is located 120 miles west of Sydney?',
         (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
         options='w::city'
     )
-}} 
+}}
 """
-db = SQLite(db_path)
+# Make our smoothie - the executed BlendSQL script
 smoothie = blend(
     query=blendsql,
-    db=db,
-    ingredients={LLMMap, LLMQA, LLMJoin},
-    blender=AzureOpenaiLLM("gpt-4"),
-    # Optional args below
-    infer_gen_constraints=True,
-    silence_db_exec_errors=False,
-    verbose=True,
-    blender_args={
-        "few_shot": True,
-        "temperature": 0.01
-    }
+    db=SQLite(fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+    blender=OpenaiLLM("gpt-3.5-turbo"),
+    ingredients={LLMQA},
 )
+print(smoothie.df)
+print(smoothie.meta.prompts)
 ```
 
+### Smoothie
 
-### Smoothie 
 The [smoothie.py](./blendsql/_smoothie.py) object defines the output of an executed BlendSQL script.
 
 ```python
 @dataclass
 class Smoothie:
     df: pd.DataFrame
     meta: SmoothieMeta
-    
+
 @dataclass
 class SmoothieMeta:
     process_time_seconds: float
     num_values_passed: int  # Number of values passed to a Map/Join/QA ingredient
     num_prompt_tokens: int  # Number of prompt tokens (counting user and assistant, i.e. input/output)
     prompts: List[str] # Log of prompts submitted to model
     example_map_outputs: List[Any]  # outputs from a Map ingredient, for debugging
     ingredients: List[Ingredient]
     query: str
     db_path: str
     contains_ingredient: bool = True
 
 def blend(*args, **kwargs) -> Smoothie:
-  ... 
+  ...
 ```
+
 <hr>
 
-## Ingredients 
+## Ingredients
 
 ![ingredients](docs/img/ingredients.jpg)
 
-Ingredients are at the core of a BlendSQL script. 
+Ingredients are at the core of a BlendSQL script.
 
 They are callable functions that perform one the task paradigms defined in [ingredient.py](./blendsql/ingredients/ingredient.py).
 
-At their core, these are not a new concept. [User-defined functions (UDFs)](https://docs.databricks.com/en/udf/index.html), or [Application-Defined Functions in SQLite](https://www.sqlite.org/appfunc.html) have existed for quite some time. 
+At their core, these are not a new concept. [User-defined functions (UDFs)](https://docs.databricks.com/en/udf/index.html), or [Application-Defined Functions in SQLite](https://www.sqlite.org/appfunc.html) have existed for quite some time.
 
 However, ingredients in BlendSQL are intended to be optimized towards LLM-based functions, defining an order of operations for traversing the AST such that the minimal amount of data is passed into your expensive GPT-4/Llama 2/Mistral 7b/etc. prompt.
 
 Ingredient calls are denoted by wrapping them in double curly brackets, `{{ingredient}}`.
 
 The following ingredient types are valid.
 
 ### MapIngredient
+
 This type of ingredient applies a function on a given table/column pair to create a new column containing the function output.
 
 For example, take the following query.
 
-```sql 
+```sql
 SELECT merchant FROM transactions
     WHERE {{LLMMap('Is this a pizza shop?', 'transactions::merchant')}} = TRUE
 ```
 
 `LLMMap` is one of our builtin MapIngredients. For each of the distinct values in the "merchant" column of the "transactions" table, it will create a column containing the function output.
 
 | merchant | Is this a pizza shop? |
-|----------|-----------------------|
+| -------- | --------------------- |
 | Domino's | 1                     |
 | Safeway  | 0                     |
 | Target   | 0                     |
 
 The temporary table shown above is then combined with the original "transactions" table with an `INNER JOIN` on the "merchant" column.
 
 ### JoinIngredient
+
 Handles the logic of semantic `JOIN` clauses between tables.
 
 For example:
+
 ```sql
 SELECT Capitals.name, State.name FROM Capitals
     JOIN {{
         LLMJoin(
-            'Align state to capital', 
-            left_on='States::name', 
+            'Align state to capital',
+            left_on='States::name',
             right_on='Capitals::name'
         )
     }}
 ```
+
 The above example hints at a database schema that would make [E.F Codd](https://en.wikipedia.org/wiki/Edgar_F._Codd) very angry: why do we have two separate tables `States` and `Capitals` with no foreign key to join the two?
 
 BlendSQL was built to interact with tables "in-the-wild", and many (such as those on Wikipedia) do not have these convenient properties of well-designed relational models.
 
 For this reason, we can leverage the internal knowledge of a pre-trained LLM to do the `JOIN` operation for us.
 
 ### QAIngredient
+
 Sometimes, simply selecting data from a given database is not enough to sufficiently answer a user's question.
 
 The `QAIngredient` is designed to return data of variable types, and is best used in cases when we either need:
-1) Unstructured, free-text responses ("Give me a summary of all my spending in coffe")
-2) Complex, unintuitive relationships extracted from table subsets ("How many consecutive days did I spend in coffee?")
+
+1. Unstructured, free-text responses ("Give me a summary of all my spending in coffe")
+2. Complex, unintuitive relationships extracted from table subsets ("How many consecutive days did I spend in coffee?")
 
 The following query demonstrates usage of the builtin `LLMQA` ingredient.
 
 ```sql
 {{
     LLMQA(
-        'How many consecutive days did I buy stocks in Financials?', 
+        'How many consecutive days did I buy stocks in Financials?',
         (
             SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
               FROM account_history
               LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
               WHERE Sector = "Financials"
               ORDER BY "Run Date" LIMIT 5
         )
     )
-}} 
+}}
 ```
-This is slightly more complicated than the rest of the ingredients. 
+
+This is slightly more complicated than the rest of the ingredients.
 
 Behind the scenes, we wrap the call to `LLMQA` in a trivial `CASE` clause, ensuring that the ingredient's output gets returned.
-```sql 
-SELECT CASE WHEN FALSE THEN FALSE 
+
+```sql
+SELECT CASE WHEN FALSE THEN FALSE
   WHEN TRUE then {{QAIngredient}}
   END
 ```
+
 The LLM gets both the question asked, alongside the subset of the SQL database fetched by our subquery.
 
 | **"Run Date"** | **Symbol** | **Sector** |
-|----------------|------------|------------|
+| -------------- | ---------- | ---------- |
 | 2022-01-14     | HBAN       | Financials |
 | 2022-01-20     | AIG        | Financials |
 | 2022-01-24     | AIG        | Financials |
 | 2022-01-24     | NTRS       | Financials |
 | 2022-01-25     | HBAN       | Financials |
 
-
 From examining this table, we see that we bought stocks in the Financials sector 2 consecutive days (2022-01-24, and 2022-01-25).
 The LLM answers the question in an end-to-end manner, returning the result `2`.
 
 The `QAIngredient` can be used as a standalone end-to-end QA tool, or as a component within a larger BlendSQL query.
 
-For example, the BlendSQL query below translates to the valid (but rather confusing) question: 
+For example, the BlendSQL query below translates to the valid (but rather confusing) question:
 
 "Show me stocks in my portfolio, whose price is greater than the number of consecutive days I bought Financial stocks multiplied by 10. Only display those companies which offer a media streaming service."
+
 ```sql
  SELECT Symbol, "Last Price" FROM portfolio WHERE "Last Price" > {{
   LLMQA(
-        'How many consecutive days did I buy stocks in Financials?', 
+        'How many consecutive days did I buy stocks in Financials?',
         (
             SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
               FROM account_history
               LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
               WHERE Sector = "Financials"
               ORDER BY "Run Date" LIMIT 5
         )
     )
   }} * 10
   AND {{LLMMap('Offers a media streaming service?', 'portfolio::Description')}} = 1
 ```
+
 #### Constrained Decoding with `options`
+
 Perhaps we want the answer to the above question in a different format. We call our LLM ingredient in a constrained setting by passing a `options` argument, where we provide either semicolon-separated options, or a reference to a column.
 
 ```sql
 {{
     LLMQA(
-        'How many consecutive days did I buy stocks in Financials?', 
+        'How many consecutive days did I buy stocks in Financials?',
         (
             SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
               FROM account_history
               LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
               WHERE Sector = "Financials"
               ORDER BY "Run Date" LIMIT 5
         )
@@ -607,27 +676,28 @@
 }}
 ```
 
 Running the above BlendSQL query, we get the output `two consecutive days!`.
 
 This `options` argument can also be a reference to a given column.
 
-For example (from the [HybridQA dataset](https://hybridqa.github.io/)): 
+For example (from the [HybridQA dataset](https://hybridqa.github.io/)):
 
-```sql 
+```sql
  SELECT capacity FROM w WHERE venue = {{
         LLMQA(
             'Which venue is named in honor of Juan Antonio Samaranch?',
             (SELECT title, content FROM documents WHERE content LIKE '%venue%'),
             options='w::venue'
         )
 }}
 ```
 
 Or, from our running example:
+
 ```sql
 {{
   LLMQA(
       'Which did i buy the most?',
       (
         SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
           FROM account_history
@@ -639,56 +709,84 @@
   )
 }}
 ```
 
 The above BlendSQL will yield the result `AIG`, since it appears in the `Symbol` column from `account_history`.
 
 ### StringIngredient
+
 This is the simplest type of ingredient. This will output a string to be placed directly into the SQL query.
 
 We have the `DT` function as a builtin StringIngredient.
 
-```sql 
+```sql
 SELECT merchant FROM transactions
     WHERE {{DT('transactions::date', start='q2')}}
 ```
 
 This will call a Python function that uses `datetime` to interpret the absolute dates which the relative phrase "q2" most likely refers to.
 
 We do not create any new tables or perform any joins with a StringIngredient; instead, we simply get the following SQL query.
 
 > [!NOTE]
 > The below SQL interpretation of the `DT` function assumes we're calling it in December, 2022. The phrase 'q2' will be interpreted differently in, say, March 1998.
 
-```sql 
+```sql
 SELECT merchant FROM transactions
     WHERE date > '2022-09-30' AND date < '2022-12-01'
 ```
 
-<hr> 
- 
+<hr>
+
+## Parsing Natural Language to BlendSQL
 
-## LLMs
+```python
+from blendsql import nl_to_blendsql, LLMMap
+from blendsql.models import TransformersLLM
+from blendsql.db import SQLite
+from blendsql.utils import fetch_from_hub
 
+model = TransformersLLM("Qwen/Qwen1.5-0.5B")
+db = SQLite(fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db"))
 
-<hr> 
+query = nl_to_blendsql(
+    question="Which venues in Sydney saw more than 30 points scored?",
+    model=model,
+    ingredients={LLMMap},
+    serialized_db=db.to_serialized(num_rows=3, use_tables=["w", "documents"]),
+    verbose=True,
+    max_grammar_corrections=5,
+)
+```
 
-## Databases
+### Grammar-Based Correction
 
+If you use the grammar prompting feature of BlendSQL, please cite the original grammar prompting paper below.
 
-<hr> 
+```bibtex
+@article{wang2024grammar,
+  title={Grammar prompting for domain-specific language generation with large language models},
+  author={Wang, Bailin and Wang, Zi and Wang, Xuezhi and Cao, Yuan and A Saurous, Rif and Kim, Yoon},
+  journal={Advances in Neural Information Processing Systems},
+  volume={36},
+  year={2024}
+}
+```
+
+<hr>
 ### Appendix
-#### Run Line Profiling 
+#### Run Line Profiling
 First uncomment `@profile` above `blend()` in `blendsql.py`.
 Make sure you've run `pip install line_profiler` first. This installs the tool here: https://github.com/pyutils/line_profiler
 
 `PYTHONPATH=$PWD:$PYTHONPATH kernprof -lv examples/benchmarks/with_blendsql.py`
 
 #### Benchmarks
-The below benchmarks were done on my local M1 Macbook Pro. by running the scripts found in `examples/benchmarks`. 
+
+The below benchmarks were done on my local M1 Macbook Pro. by running the scripts found in `examples/benchmarks`.
 'Lines of Code' is a rough estimate of the user-written code for each usecase.
 
-| **Name**                     | **Description**                                                 | **Runtime/s (Across 10 runs)** | **Lines of Code** |
-|------------------------------|-----------------------------------------------------------------|-------------------------------------------------|-------------------|
-| BlendSQL                     |                                                     |5.685 +/- 0.930                                 | 9                 |
-| SQL + LLM Calls       | Filtering what we can with SQL, then running LLM calls.         | 9.083 +/- 2.061                                 | 106               |
-| Naive SQL + LLM Calls | Runing LLM calls on entire table, regardless of SQL conditions. | 64.809 +/- 6.225                                | 106               |
+| **Name**              | **Description**                                                 | **Runtime/s (Across 10 runs)** | **Lines of Code** |
+| --------------------- | --------------------------------------------------------------- | ------------------------------ | ----------------- |
+| BlendSQL              |                                                                 | 5.685 +/- 0.930                | 9                 |
+| SQL + LLM Calls       | Filtering what we can with SQL, then running LLM calls.         | 9.083 +/- 2.061                | 106               |
+| Naive SQL + LLM Calls | Runing LLM calls on entire table, regardless of SQL conditions. | 64.809 +/- 6.225               | 106               |
```

#### html2text {}

```diff
@@ -1,207 +1,230 @@
-Metadata-Version: 2.1 Name: blendsql Version: 0.0.141 Summary: Orchestrate
-SQLite logic and LLM reasoning within a unified dialect. Home-page: https://
+Metadata-Version: 2.1 Name: blendsql Version: 0.0.15 Summary: Query language to
+blend SQL logic and LLM reasoning across multi-modal data. Home-page: https://
 github.com/parkervg/blendsql Author: Parker Glenn Author-email:
 parkervg5@gmail.com License: Apache License 2.0 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: guidance>=0.1.0 Requires-Dist:
-pyparsing==3.1.1 Requires-Dist: pandas>=2.0.0 Requires-Dist: bottleneck>=1.3.6
+pyparsing==3.1.1 Requires-Dist: pandas==1.5.3 Requires-Dist: bottleneck>=1.3.6
 Requires-Dist: python-dotenv==1.0.1 Requires-Dist: sqlglot==18.13.0 Requires-
-Dist: platformdirs Requires-Dist: pre-commit Requires-Dist: attrs Requires-
-Dist: tqdm Requires-Dist: dateparser Requires-Dist: colorama Requires-Dist:
-fiscalyear Requires-Dist: tabulate Requires-Dist: typeguard Provides-Extra:
+Dist: sqlalchemy>=2.0.0 Requires-Dist: platformdirs Requires-Dist: attrs
+Requires-Dist: tqdm Requires-Dist: colorama Requires-Dist: tabulate Requires-
+Dist: typeguard Provides-Extra: nl-to-blendsql Requires-Dist: exrex; extra ==
+"nl-to-blendsql" Requires-Dist: lark; extra == "nl-to-blendsql" Provides-Extra:
 research Requires-Dist: datasets==2.16.1; extra == "research" Requires-Dist:
 nltk; extra == "research" Requires-Dist: wikiextractor; extra == "research"
 Requires-Dist: rouge_score; extra == "research" Requires-Dist: rapidfuzz; extra
 == "research" Requires-Dist: records; extra == "research" Requires-Dist:
 SQLAlchemy; extra == "research" Requires-Dist: recognizers-text; extra ==
 "research" Requires-Dist: recognizers-text-suite; extra == "research" Requires-
 Dist: emoji==1.7.0; extra == "research" Provides-Extra: test Requires-Dist:
 pytest; extra == "test" Requires-Dist: huggingface_hub; extra == "test"
-Provides-Extra: docs Requires-Dist: mkdocs-material; extra == "docs" Requires-
-Dist: mkdocstrings; extra == "docs" Requires-Dist: mkdocs-section-index; extra
-== "docs" Requires-Dist: mkdocstrings-python; extra == "docs" Requires-Dist:
-mkdocs-jupyter; extra == "docs"
+Requires-Dist: pre-commit; extra == "test" Provides-Extra: docs Requires-Dist:
+mkdocs-material; extra == "docs" Requires-Dist: mkdocstrings; extra == "docs"
+Requires-Dist: mkdocs-section-index; extra == "docs" Requires-Dist:
+mkdocstrings-python; extra == "docs" Requires-Dist: mkdocs-jupyter; extra ==
+"docs" Provides-Extra: demo Requires-Dist: chainlit; extra == "demo"
             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e___2_._0_-_b_l_u_e_._s_v_g_][https://
       img.shields.io/github/last-commit/parkervg/blendsql?color=green][https://
                                         img.shields.io/badge/PRs-Welcome-Green]
                                   [blendsql]
                                  SQL ð¤ LLMs
  CChheecckk oouutt oouurr _oo_nn_ll_ii_nn_ee_ _dd_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ffoorr aa mmoorree ccoommpprreehheennssiivvee oovveerrvviieeww.. Results
 from the paper are available [here](https://github.com/parkervg/blendsql/tree/
                     research-paper/research/paper-results)
 
-## Intro BlendSQL is a *superset of SQLite* for problem decomposition and
-hybrid question-answering with LLMs. As a result, we can *Blend* together... -
-ð¥¤ ...operations over heterogeneous data sources (e.g. tables, text, images)
-- ð¥¤ ...the structured & interpretable reasoning of SQL with the
-generalizable reasoning of LLMs It can be viewed as an inversion of the typical
-text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a SQL
-program. **Now, the user is given the control to oversee all calls (LLM + SQL)
-within a unified query language.** ![comparison](docs/img/comparison.jpg) For
-example, imagine we have the following tables. ### `w` | **date** | **rival** |
-**city** | **venue** | **score** | |----------|---------------------------|----
--------|-----------------------------|-----------| | 31 may | nsw waratahs |
-sydney | agricultural society ground | 11-0 | | 5 jun | northern districts |
-newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney |
-agricultural society ground | 21-2 | | 11 jun | western districts | bathurst |
-bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
-cricket ground | 23-10 | ### `documents` | **title** | **content** | |---------
------------------------|---------------------------------------------------| |
+### Features - Supports many DBMS ð¾ - Currently, SQLite and PostgreSQL are
+functional - more to come! - Easily extendable to [multi-modal usecases](./
+examples/vqa-ingredient.ipynb) ð¼ï¸ - Smart parsing optimizes what is passed
+to external functions ð§  - Traverses abstract syntax tree with [sqlglot]
+(https://github.com/tobymao/sqlglot) to minimize LLM function calls ð³ -
+Constrained decoding with [guidance](https://github.com/guidance-ai/guidance)
+ð - LLM function caching, built on [diskcache](https://grantjenks.com/docs/
+diskcache/) ð ## Intro BlendSQL is a *superset of SQLite* for problem
+decomposition and hybrid question-answering with LLMs. As a result, we can
+*Blend* together... - ð¥¤ ...operations over heterogeneous data sources (e.g.
+tables, text, images) - ð¥¤ ...the structured & interpretable reasoning of SQL
+with the generalizable reasoning of LLMs It can be viewed as an inversion of
+the typical text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a
+SQL program. **Now, the user is given the control to oversee all calls (LLM +
+SQL) within a unified query language.** ![comparison](docs/img/comparison.jpg)
+For example, imagine we have the following tables. ### `w` | **date** |
+**rival** | **city** | **venue** | **score** | | -------- | -------------------
+------ | --------- | --------------------------- | --------- | | 31 may | nsw
+waratahs | sydney | agricultural society ground | 11-0 | | 5 jun | northern
+districts | newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney
+| agricultural society ground | 21-2 | | 11 jun | western districts | bathurst
+| bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
+cricket ground | 23-10 | ### `documents` | **title** | **content** | | --------
+---------------------- | ------------------------------------------------- | |
 sydney | sydney ( /ËsÉªdni/ ( listen ) sid-nee ) is the ... | | new south
 wales waratahs | the new south wales waratahs ( /ËwÉrÉtÉËz/ or ... | |
 sydney showground (moore park) | the former sydney showground ( moore park )
 at... | | sydney cricket ground | the sydney cricket ground ( scg ) is a sports
 ... | | newcastle, new south wales | the newcastle ( /ËnuËkÉËsÉl/ new-kah-
 sÉl ) met... | | bathurst, new south wales | bathurst /ËbÃ¦Î¸Érst/ is a city
 in the central t... | BlendSQL allows us to ask the following questions by
 injecting "ingredients", which are callable functions denoted by double curly
 brackets (`{{`, `}}`). The below examples work out of the box, but you are able
-to design your own ingredients as well! *What was the result of the game played
-120 miles west of Sydney?* ```sql SELECT * FROM w WHERE city = {{ LLMQA( 'Which
+to design your own ingredients as well! _What was the result of the game played
+120 miles west of Sydney?_ ```sql SELECT * FROM w WHERE city = {{ LLMQA( 'Which
 city is located 120 miles west of Sydney?', (SELECT * FROM documents WHERE
-documents MATCH 'sydney OR 120'), options='w::city' ) }} ``` *Which venues in
-Sydney saw more than 30 points scored?* ```sql SELECT DISTINCT venue FROM w
+documents MATCH 'sydney OR 120'), options='w::city' ) }} ``` _Which venues in
+Sydney saw more than 30 points scored?_ ```sql SELECT DISTINCT venue FROM w
 WHERE city = 'sydney' AND {{ LLMMap( 'More than 30 total points?', 'w::score' )
-}} = TRUE ``` *Show all NSW Waratahs games and a description of the team.*
+}} = TRUE ``` _Show all NSW Waratahs games and a description of the team._
 ```sql SELECT date, rival, score, documents.content AS "Team Description" FROM
 w JOIN {{ LLMJoin( left_on='documents::title', right_on='w::rival' ) }} WHERE
 rival = 'nsw waratahs' ``` ### More Examples from Popular QA Datasets
 _HH_yy_bb_rr_ii_dd_QQ_AA_ For this setting, our database contains 2 tables: a table from
 Wikipedia `w`, and a collection of unstructured Wikipedia articles in the table
-`documents`. *What is the state flower of the smallest state by area ?* ```sql
+`documents`. _What is the state flower of the smallest state by area ?_ ```sql
 SELECT "common name" AS 'State Flower' FROM w WHERE state = {{ LLMQA( 'Which is
 the smallest state by area?', (SELECT title, content FROM documents),
-options='w::state' ) }} ``` *Who were the builders of the mosque in Herat with
-fire temples ?* ```sql {{ LLMQA( 'Name of the builders?', ( SELECT title AS
-'Building', content FROM documents WHERE title = {{ LLMQA( 'Align the name to
-the correct title.', (SELECT name FROM w WHERE city = 'herat' AND remarks LIKE
-'%fire temple%'), options='documents::title' ) }} ) ) }} ``` *What is the
-capacity of the venue that was named in honor of Juan Antonio Samaranch in 2010
-after his death ?* ```sql SELECT capacity FROM w WHERE venue = {{ LLMQA( 'Which
-venue is named in honor of Juan Antonio Samaranch?', (SELECT title AS 'Venue',
-content FROM documents), options='w::venue' ) }} ```
+options='w::state' ) }} ``` _Who were the builders of the mosque in Herat with
+fire temples ?_ ```sql {{ LLMQA( 'Who were the builders of the mosque?',
+( SELECT documents.title AS 'Building', documents.content FROM documents JOIN {
+{ LLMJoin( left_on='w::name', right_on='documents::title' ) }} WHERE w.city =
+'herat' AND w.remarks LIKE '%fire temple%' ) ) }} ``` _What is the capacity of
+the venue that was named in honor of Juan Antonio Samaranch in 2010 after his
+death ?_ ```sql SELECT capacity FROM w WHERE venue = {{ LLMQA( 'Which venue is
+named in honor of Juan Antonio Samaranch?', (SELECT title AS 'Venue', content
+FROM documents), options='w::venue' ) }} ```
 _OO_TT_TT_--_QQ_AA_ Unlike HybridQA, these questions are open-domain, where we don't know in
 advance where the answer of a given open question appears in a passage or a
 table. As a result, we need to play the role of both the retriever (to select
 relevant context) and reader (to read from relevant contexts and return the
 given answer). As the underlying database consists of 400K tables and 5M
 documents, it's important to set `LIMIT` clauses appropriately to ensure
 reasonable execution times. The examples below also demonstrate how BlendSQL
 unpacks [CTE statements](https://www.sqlite.org/lang_with.html) to ensure we
-only pass necessary data into the BlendSQL ingredient calls. *When was the
-third highest paid Rangers F.C . player born ?* ```sql {{ LLMQA( 'When was the
+only pass necessary data into the BlendSQL ingredient calls. _When was the
+third highest paid Rangers F.C . player born ?_ ```sql {{ LLMQA( 'When was the
 Rangers Player born?', ( WITH t AS ( SELECT player FROM ( SELECT * FROM "./List
 of Rangers F.C. records and statistics (0)" UNION ALL SELECT * FROM "./List of
 Rangers F.C. records and statistics (1)" ) ORDER BY trim(fee, 'Â£') DESC LIMIT
 1 OFFSET 2 ), d AS ( SELECT * FROM documents JOIN t WHERE documents MATCH
 t.player || ' OR rangers OR fc' ORDER BY rank LIMIT 5 ) SELECT d.content,
-t.player AS 'Rangers Player' FROM d JOIN t ) ) }} ``` *In which Track Cycling
+t.player AS 'Rangers Player' FROM d JOIN t ) ) }} ``` _In which Track Cycling
 World Championships event was the person born in Matanzas , Cuba ranked highest
-?* ```sql {{ LLMQA( 'In what event was the cyclist ranked highest?', ( SELECT *
+?_ ```sql {{ LLMQA( 'In what event was the cyclist ranked highest?', ( SELECT *
 FROM ( SELECT * FROM "./Cuba at the UCI Track Cycling World Championships (2)"
 ) as w WHERE w.name = {{ LLMQA( "Which cyclist was born in Matanzas, Cuba?",
 ( SELECT * FROM documents WHERE documents MATCH 'matanzas AND (cycling OR track
 OR born)' ORDER BY rank LIMIT 3 ), options="w::name" ) }} ), options='w::event'
-) }} ``` *Who is the director the Togolese film that was a 30 minute film that
-was shot in 16mm ?* ```sql SELECT director FROM "./List of African films (4)"
+) }} ``` _Who is the director the Togolese film that was a 30 minute film that
+was shot in 16mm ?_ ```sql SELECT director FROM "./List of African films (4)"
 as w WHERE title = {{ LLMQA( 'What is the name of the Togolese film that was 30
 minutes and shot in 16mm?', (SELECT * FROM documents WHERE documents MATCH
 'togolese OR 30 OR 16mm OR film' ORDER BY rank LIMIT 5), options='w::title' )
 }} ```
 _FF_EE_VV_EE_RR_OO_UU_SS_ Here, we deal not with questions, but truth claims given a context of
 unstructured and structured data. These claims should be judged as "SUPPORTS"
 or "REFUTES". Using BlendSQL, we can formulate this determination of truth as a
-function over facts. *Oyedaea is part of the family Asteraceae in the order
-Asterales.* ```sql SELECT EXISTS ( SELECT * FROM w0 WHERE "family:" =
-'asteraceae' AND "order:" = 'asterales' ) ``` *The 2006-07 San Jose Sharks
+function over facts. _Oyedaea is part of the family Asteraceae in the order
+Asterales._ ```sql SELECT EXISTS ( SELECT * FROM w0 WHERE "family:" =
+'asteraceae' AND "order:" = 'asterales' ) ``` _The 2006-07 San Jose Sharks
 season, the 14th season of operation (13th season of play) for the National
-Hockey League (NHL) franchise, scored the most points in the Pacific Division.*
+Hockey League (NHL) franchise, scored the most points in the Pacific Division._
 ```sql SELECT ( {{ LLMValidate( 'Is the Sharks 2006-07 season the 14th season
 (13th season of play)?', (SELECT * FROM documents) ) }} ) AND ( SELECT (SELECT
 filledcolumnname FROM w0 ORDER BY pts DESC LIMIT 1) = 'san jose sharks' ) ```
-*Saunders College of Business, which is accredited by the Association to
+_Saunders College of Business, which is accredited by the Association to
 Advance Collegiate Schools of Business International, is one of the colleges of
 Rochester Institute of Technology established in 1910 and is currently under
-the supervision of Dean Jacqueline R. Mozrall.* ```sql SELECT EXISTS( SELECT *
+the supervision of Dean Jacqueline R. Mozrall._ ```sql SELECT EXISTS( SELECT *
 FROM w0 WHERE "parent institution" = 'rochester institute of technology' AND
 "established" = '1910' AND "dean" = 'jacqueline r. mozrall' ) AND ( {
 { LLMValidate( 'Is Saunders College of Business (SCB) accredited by the
 Association to Advance Collegiate Schools of Business International (AACSB)?',
 (SELECT * FROM documents) ) }} ) ```
-## Table of Contents * [Install](#install) * [Quickstart](#quickstart) * [FAQ]
-(#faq) * [Documentation](#documentation) * [Execute a BlendSQL Query](#execute-
-a-blendsql-query) * [Smoothie](#smoothie) * [Ingredients](#ingredients) *
-[MapIngredient](#mapingredient) * [QAIngredient](#qaingredient) * [Constrained
-Decoding with 'options'](#constrained-decoding-with-options) * [JoinIngredient]
-(#joiningredient) * [StringIngredient](#stringingredient) * [LLMs](#llms) *
-[Databases](#databases) * [Appendix](#appendix) ### Features - Smart parsing
-optimizes what is passed to external functions ð§  - Traverses abstract syntax
-tree with [sqlglot](https://github.com/tobymao/sqlglot) to minimize LLM
-function calls ð³ - LLM function caching, built on [diskcache](https://
-grantjenks.com/docs/diskcache/) ð - Constrained decoding with [guidance]
-(https://github.com/guidance-ai/guidance) ð For a technical walkthrough of
+## Table of Contents - [Install](#install) - [Quickstart](#quickstart) - [FAQ]
+(#faq) - [Documentation](#documentation) - [Execute a BlendSQL Query](#execute-
+a-blendsql-query) - [Smoothie](#smoothie) - [Ingredients](#ingredients) -
+[MapIngredient](#mapingredient) - [QAIngredient](#qaingredient) - [Constrained
+Decoding with 'options'](#constrained-decoding-with-options) - [JoinIngredient]
+(#joiningredient) - [StringIngredient](#stringingredient) - [Parsing Natural
+Language to BlendSQL](#parsing-natural-language-to-blendsql) - [LLMs](#llms) -
+[Databases](#databases) - [Appendix](#appendix) For a technical walkthrough of
 how a BlendSQL query is executed, check out [technical_walkthrough.md](./docs/
 technical_walkthrough.md). ## Install ``` pip install blendsql ``` ##
-Quickstart ```python from blendsql import blend, LLMQA, LLMMap from blendsql.db
-import SQLite from blendsql.models import OpenaiLLM blendsql = """ SELECT
-merchant FROM transactions WHERE {{LLMMap('is this a pizza shop?',
-'transactions::merchant')}} = TRUE AND parent_category = 'Food' """ # Make our
+Quickstart ```python from blendsql import blend, LLMQA from blendsql.db import
+SQLite from blendsql.models import OpenaiLLM from blendsql.utils import
+fetch_from_hub blendsql = """ SELECT * FROM w WHERE city = {{ LLMQA( 'Which
+city is located 120 miles west of Sydney?', (SELECT * FROM documents WHERE
+documents MATCH 'sydney OR 120'), options='w::city' ) }} """ # Make our
 smoothie - the executed BlendSQL script smoothie = blend( query=blendsql,
-blender=OpenaiLLM("gpt-3.5-turbo-0613"), ingredients={LLMMap, LLMQA}, db=SQLite
-(db_path="transactions.db"), verbose=True ) ``` ### FAQ #### Why not just
+db=SQLite(fetch_from_hub
+("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+blender=OpenaiLLM("gpt-3.5-turbo"), ingredients={LLMQA}, ) print(smoothie.df)
+print(smoothie.meta.prompts) ``` ### FAQ #### How does BlendSQL execute a
+query? > BlendSQL handles traversal of the SQL AST and creation of temporary
+tables to execute a given query. > This allows BlendSQL to be DBMS-agnostic,
+and extendable into both SQLite, PostgreSQL, and other DBMS. #### Why not just
 implement BlendSQL as a [user-defined function in SQLite](https://
 www.sqlite.org/c3ref/c_deterministic.html#sqlitedeterministic)? > LLMs are
 expensive, both in terms of $ cost and compute time. When applying them to
 SQLite databases, we want to take special care in ensuring we're not applying
 them to contexts where they're not required. > This is [not easily achievable
 with UDFs](https://sqlite.org/forum/info/
 649ad4c62fd4b4e8cb5d6407107b8c8a9a0afaaf95a87805e5a8403a79e6616c), even when
 marked as a [deterministic function](https://www.sqlite.org/c3ref/
 c_deterministic.html#sqlitedeterministic). > > BlendSQL is specifically
 designed to enforce an order-of-operations that 1) prioritizes vanilla SQL
 operations first, and 2) caches results from LLM ingredients so they don't need
-to be recomputed. > For example: > ```sql > SELECT {{LLMMap('What state is this
-NBA team from?', 'w::team')} FROM w > WHERE num_championships > 3 > ORDER BY {
-{LLMMap('What state is this NBA team from?', 'w::team')} > > ``` > BlendSQL
-makes sure to only pass those `team` values from rows which satisfy the
-condition `num_championship > 3` to the LLM. Additionally, since we assume the
-function is deterministic, we make a single LLM call and cache the results,
+to be recomputed. > For example: > > ```sql > SELECT {{LLMMap('What state is
+this NBA team from?', 'w::team')} FROM w > WHERE num_championships > 3 > ORDER
+BY {{LLMMap('What state is this NBA team from?', 'w::team')} > > ``` > >
+BlendSQL makes sure to only pass those `team` values from rows which satisfy
+the condition `num_championship > 3` to the LLM. Additionally, since we assume
+the function is deterministic, we make a single LLM call and cache the results,
 despite the ingredient function being used twice. #### So I get how to write
 BlendSQL queries. But why would I use this over vanilla SQLite? > Certain
 ingredients, like [LLMJoin](#joiningredient), will likely give seasoned SQL
 experts a headache at first. However, BlendSQL's real strength comes from it's
-use as an *intermediate representation for reasoning over structured +
-unstructured with LLMs*. Some examples of this can be found above [here](#more-
+use as an _intermediate representation for reasoning over structured +
+unstructured with LLMs_. Some examples of this can be found above [here](#more-
 examples-from-popular-qa-datasets).
 ===============================================================================
 ### Citation ```bibtex @article{glenn2024blendsql, title={BlendSQL: A Scalable
 Dialect for Unifying Hybrid Question Answering in Relational Algebra}, author=
 {Parker Glenn and Parag Pravin Dakle and Liang Wang and Preethi Raghavan},
 year={2024}, eprint={2402.17882}, archivePrefix={arXiv}, primaryClass={cs.CL} }
-``` # Documentation > [!WARNING] > WIP, will be updated ## Execute a BlendSQL
-Query The `blend()` function is used to execute a BlendSQL query against a
-database and return the final result, in addition to the intermediate reasoning
-steps taken. ::: blendsql.blendsql.blend handler: python ```python from
-blendsql import blend, LLMMap, LLMQA, LLMJoin from blendsql.db import SQLite
-from blendsql.models import OpenaiLLM blendsql = """ SELECT * FROM w WHERE city
-= {{ LLMQA( 'Which city is located 120 miles west of Sydney?', (SELECT * FROM
-documents WHERE documents MATCH 'sydney OR 120'), options='w::city' ) }} """ db
-= SQLite(db_path) smoothie = blend( query=blendsql, db=db, ingredients={LLMMap,
-LLMQA, LLMJoin}, blender=AzureOpenaiLLM("gpt-4"), # Optional args below
-infer_gen_constraints=True, silence_db_exec_errors=False, verbose=True,
-blender_args={ "few_shot": True, "temperature": 0.01 } ) ``` ### Smoothie The
-[smoothie.py](./blendsql/_smoothie.py) object defines the output of an executed
-BlendSQL script. ```python @dataclass class Smoothie: df: pd.DataFrame meta:
-SmoothieMeta @dataclass class SmoothieMeta: process_time_seconds: float
-num_values_passed: int # Number of values passed to a Map/Join/QA ingredient
-num_prompt_tokens: int # Number of prompt tokens (counting user and assistant,
-i.e. input/output) prompts: List[str] # Log of prompts submitted to model
-example_map_outputs: List[Any] # outputs from a Map ingredient, for debugging
-ingredients: List[Ingredient] query: str db_path: str contains_ingredient: bool
-= True def blend(*args, **kwargs) -> Smoothie: ... ```
+``` # Documentation ## Databases Since BlendSQL relies on the package [sqlglot]
+(https://github.com/tobymao/sqlglot) for query optimization (which supports a
+[wide variety of SQL dialects](https://github.com/tobymao/sqlglot/blob/main/
+sqlglot/dialects/__init__.py)) and the notion of [temporary tables](https://
+en.wikibooks.org/wiki/Structured_Query_Language/Temporary_Table), it can easily
+integrate with many different SQL dialects. Currently, the following are
+supported. ### SQLite A SQLite database connection. Can be initialized via a
+path to the database file. Example: ```python from blendsql.db import SQLite db
+= SQLite("./path/to/database.db") ``` ### PostgreSQL A PostgreSQL database
+connection. Can be initialized via the SQLAlchemy input string. https://
+docs.sqlalchemy.org/en/20/core/engines.html#postgresql Example: ```python from
+blendsql.db import PostgreSQL db = PostgreSQL("user:password@localhost/
+mydatabase") ``` ## Execute a BlendSQL Query The `blend()` function is used to
+execute a BlendSQL query against a database and return the final result, in
+addition to the intermediate reasoning steps taken. ```python from blendsql
+import blend, LLMQA from blendsql.db import SQLite from blendsql.models import
+OpenaiLLM from blendsql.utils import fetch_from_hub blendsql = """ SELECT *
+FROM w WHERE city = {{ LLMQA( 'Which city is located 120 miles west of
+Sydney?', (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
+options='w::city' ) }} """ # Make our smoothie - the executed BlendSQL script
+smoothie = blend( query=blendsql, db=SQLite(fetch_from_hub
+("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+blender=OpenaiLLM("gpt-3.5-turbo"), ingredients={LLMQA}, ) print(smoothie.df)
+print(smoothie.meta.prompts) ``` ### Smoothie The [smoothie.py](./blendsql/
+_smoothie.py) object defines the output of an executed BlendSQL script.
+```python @dataclass class Smoothie: df: pd.DataFrame meta: SmoothieMeta
+@dataclass class SmoothieMeta: process_time_seconds: float num_values_passed:
+int # Number of values passed to a Map/Join/QA ingredient num_prompt_tokens:
+int # Number of prompt tokens (counting user and assistant, i.e. input/output)
+prompts: List[str] # Log of prompts submitted to model example_map_outputs:
+List[Any] # outputs from a Map ingredient, for debugging ingredients: List
+[Ingredient] query: str db_path: str contains_ingredient: bool = True def blend
+(*args, **kwargs) -> Smoothie: ... ```
 ===============================================================================
 ## Ingredients ![ingredients](docs/img/ingredients.jpg) Ingredients are at the
 core of a BlendSQL script. They are callable functions that perform one the
 task paradigms defined in [ingredient.py](./blendsql/ingredients/
 ingredient.py). At their core, these are not a new concept. [User-defined
 functions (UDFs)](https://docs.databricks.com/en/udf/index.html), or
 [Application-Defined Functions in SQLite](https://www.sqlite.org/appfunc.html)
@@ -213,15 +236,15 @@
 ingredient types are valid. ### MapIngredient This type of ingredient applies a
 function on a given table/column pair to create a new column containing the
 function output. For example, take the following query. ```sql SELECT merchant
 FROM transactions WHERE {{LLMMap('Is this a pizza shop?', 'transactions::
 merchant')}} = TRUE ``` `LLMMap` is one of our builtin MapIngredients. For each
 of the distinct values in the "merchant" column of the "transactions" table, it
 will create a column containing the function output. | merchant | Is this a
-pizza shop? | |----------|-----------------------| | Domino's | 1 | | Safeway |
+pizza shop? | | -------- | --------------------- | | Domino's | 1 | | Safeway |
 0 | | Target | 0 | The temporary table shown above is then combined with the
 original "transactions" table with an `INNER JOIN` on the "merchant" column.
 ### JoinIngredient Handles the logic of semantic `JOIN` clauses between tables.
 For example: ```sql SELECT Capitals.name, State.name FROM Capitals JOIN {
 { LLMJoin( 'Align state to capital', left_on='States::name',
 right_on='Capitals::name' ) }} ``` The above example hints at a database schema
 that would make [E.F Codd](https://en.wikipedia.org/wiki/Edgar_F._Codd) very
@@ -229,29 +252,29 @@
 foreign key to join the two? BlendSQL was built to interact with tables "in-
 the-wild", and many (such as those on Wikipedia) do not have these convenient
 properties of well-designed relational models. For this reason, we can leverage
 the internal knowledge of a pre-trained LLM to do the `JOIN` operation for us.
 ### QAIngredient Sometimes, simply selecting data from a given database is not
 enough to sufficiently answer a user's question. The `QAIngredient` is designed
 to return data of variable types, and is best used in cases when we either
-need: 1) Unstructured, free-text responses ("Give me a summary of all my
-spending in coffe") 2) Complex, unintuitive relationships extracted from table
+need: 1. Unstructured, free-text responses ("Give me a summary of all my
+spending in coffe") 2. Complex, unintuitive relationships extracted from table
 subsets ("How many consecutive days did I spend in coffee?") The following
 query demonstrates usage of the builtin `LLMQA` ingredient. ```sql {{ LLMQA
 ( 'How many consecutive days did I buy stocks in Financials?', ( SELECT
 account_history."Run Date", account_history.Symbol, constituents."Sector" FROM
 account_history LEFT JOIN constituents ON account_history.Symbol =
 constituents.Symbol WHERE Sector = "Financials" ORDER BY "Run Date" LIMIT 5 ) )
 }} ``` This is slightly more complicated than the rest of the ingredients.
 Behind the scenes, we wrap the call to `LLMQA` in a trivial `CASE` clause,
 ensuring that the ingredient's output gets returned. ```sql SELECT CASE WHEN
 FALSE THEN FALSE WHEN TRUE then {{QAIngredient}} END ``` The LLM gets both the
 question asked, alongside the subset of the SQL database fetched by our
-subquery. | **"Run Date"** | **Symbol** | **Sector** | |----------------|------
-------|------------| | 2022-01-14 | HBAN | Financials | | 2022-01-20 | AIG |
+subquery. | **"Run Date"** | **Symbol** | **Sector** | | -------------- | -----
+----- | ---------- | | 2022-01-14 | HBAN | Financials | | 2022-01-20 | AIG |
 Financials | | 2022-01-24 | AIG | Financials | | 2022-01-24 | NTRS | Financials
 | | 2022-01-25 | HBAN | Financials | From examining this table, we see that we
 bought stocks in the Financials sector 2 consecutive days (2022-01-24, and
 2022-01-25). The LLM answers the question in an end-to-end manner, returning
 the result `2`. The `QAIngredient` can be used as a standalone end-to-end QA
 tool, or as a component within a larger BlendSQL query. For example, the
 BlendSQL query below translates to the valid (but rather confusing) question:
@@ -292,25 +315,37 @@
 which the relative phrase "q2" most likely refers to. We do not create any new
 tables or perform any joins with a StringIngredient; instead, we simply get the
 following SQL query. > [!NOTE] > The below SQL interpretation of the `DT`
 function assumes we're calling it in December, 2022. The phrase 'q2' will be
 interpreted differently in, say, March 1998. ```sql SELECT merchant FROM
 transactions WHERE date > '2022-09-30' AND date < '2022-12-01' ```
 ===============================================================================
-## LLMs
-===============================================================================
-## Databases
+## Parsing Natural Language to BlendSQL ```python from blendsql import
+nl_to_blendsql, LLMMap from blendsql.models import TransformersLLM from
+blendsql.db import SQLite from blendsql.utils import fetch_from_hub model =
+TransformersLLM("Qwen/Qwen1.5-0.5B") db = SQLite(fetch_from_hub
+("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")) query =
+nl_to_blendsql( question="Which venues in Sydney saw more than 30 points
+scored?", model=model, ingredients={LLMMap}, serialized_db=db.to_serialized
+(num_rows=3, use_tables=["w", "documents"]), verbose=True,
+max_grammar_corrections=5, ) ``` ### Grammar-Based Correction If you use the
+grammar prompting feature of BlendSQL, please cite the original grammar
+prompting paper below. ```bibtex @article{wang2024grammar, title={Grammar
+prompting for domain-specific language generation with large language models},
+author={Wang, Bailin and Wang, Zi and Wang, Xuezhi and Cao, Yuan and A Saurous,
+Rif and Kim, Yoon}, journal={Advances in Neural Information Processing
+Systems}, volume={36}, year={2024} } ```
 ===============================================================================
 ### Appendix #### Run Line Profiling First uncomment `@profile` above `blend()`
 in `blendsql.py`. Make sure you've run `pip install line_profiler` first. This
 installs the tool here: https://github.com/pyutils/line_profiler
 `PYTHONPATH=$PWD:$PYTHONPATH kernprof -lv examples/benchmarks/with_blendsql.py`
 #### Benchmarks The below benchmarks were done on my local M1 Macbook Pro. by
 running the scripts found in `examples/benchmarks`. 'Lines of Code' is a rough
 estimate of the user-written code for each usecase. | **Name** |
-**Description** | **Runtime/s (Across 10 runs)** | **Lines of Code** | |-------
------------------------|-------------------------------------------------------
-----------|-------------------------------------------------|------------------
--| | BlendSQL | |5.685 +/- 0.930 | 9 | | SQL + LLM Calls | Filtering what we
-can with SQL, then running LLM calls. | 9.083 +/- 2.061 | 106 | | Naive SQL +
-LLM Calls | Runing LLM calls on entire table, regardless of SQL conditions. |
-64.809 +/- 6.225 | 106 |
+**Description** | **Runtime/s (Across 10 runs)** | **Lines of Code** | | ------
+--------------- | -------------------------------------------------------------
+-- | ------------------------------ | ----------------- | | BlendSQL | | 5.685
++/- 0.930 | 9 | | SQL + LLM Calls | Filtering what we can with SQL, then
+running LLM calls. | 9.083 +/- 2.061 | 106 | | Naive SQL + LLM Calls | Runing
+LLM calls on entire table, regardless of SQL conditions. | 64.809 +/- 6.225 |
+106 |
```

### Comparing `blendsql-0.0.141/README.md` & `blendsql-0.0.15/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,17 +11,28 @@
 </picture>
 <p align="center">
     <i> SQL 🤝 LLMs </i>
   </p>
 <b>Check out our <a href="https://parkervg.github.io/blendsql/" target="_blank">online documentation</a> for a more comprehensive overview.</b>
 
 <i>Results from the paper are available [here](https://github.com/parkervg/blendsql/tree/research-paper/research/paper-results)</i>
+
 </div>
 <br/>
 
+### Features
+
+- Supports many DBMS 💾
+  - Currently, SQLite and PostgreSQL are functional - more to come! 
+- Easily extendable to [multi-modal usecases](./examples/vqa-ingredient.ipynb) 🖼️
+- Smart parsing optimizes what is passed to external functions 🧠
+  - Traverses abstract syntax tree with [sqlglot](https://github.com/tobymao/sqlglot) to minimize LLM function calls 🌳
+- Constrained decoding with [guidance](https://github.com/guidance-ai/guidance) 🚀
+- LLM function caching, built on [diskcache](https://grantjenks.com/docs/diskcache/) 🔑
+
 ## Intro
 BlendSQL is a *superset of SQLite* for problem decomposition and hybrid question-answering with LLMs. 
 
 As a result, we can *Blend* together...
 
 - 🥤 ...operations over heterogeneous data sources (e.g. tables, text, images)
 - 🥤 ...the structured & interpretable reasoning of SQL with the generalizable reasoning of LLMs
@@ -31,59 +42,64 @@
 **Now, the user is given the control to oversee all calls (LLM + SQL) within a unified query language.**
 
 ![comparison](docs/img/comparison.jpg)
 
 For example, imagine we have the following tables.
 
 ### `w`
+
 | **date** | **rival**                 | **city**  | **venue**                   | **score** |
-|----------|---------------------------|-----------|-----------------------------|-----------|
+| -------- | ------------------------- | --------- | --------------------------- | --------- |
 | 31 may   | nsw waratahs              | sydney    | agricultural society ground | 11-0      |
 | 5 jun    | northern districts        | newcastle | sports ground               | 29-0      |
 | 7 jun    | nsw waratahs              | sydney    | agricultural society ground | 21-2      |
 | 11 jun   | western districts         | bathurst  | bathurst ground             | 11-0      |
 | 12 jun   | wallaroo & university nsw | sydney    | cricket ground              | 23-10     |
 
 ### `documents`
+
 | **title**                      | **content**                                       |
-|--------------------------------|---------------------------------------------------|
+| ------------------------------ | ------------------------------------------------- |
 | sydney                         | sydney ( /ˈsɪdni/ ( listen ) sid-nee ) is the ... |
 | new south wales waratahs       | the new south wales waratahs ( /ˈwɒrətɑːz/ or ... |
 | sydney showground (moore park) | the former sydney showground ( moore park ) at... |
 | sydney cricket ground          | the sydney cricket ground ( scg ) is a sports ... |
 | newcastle, new south wales     | the newcastle ( /ˈnuːkɑːsəl/ new-kah-səl ) met... |
 | bathurst, new south wales      | bathurst /ˈbæθərst/ is a city in the central t... |
 
 BlendSQL allows us to ask the following questions by injecting "ingredients", which are callable functions denoted by double curly brackets (`{{`, `}}`).
-The below examples work out of the box, but you are able to design your own ingredients as well! 
+The below examples work out of the box, but you are able to design your own ingredients as well!
+
+_What was the result of the game played 120 miles west of Sydney?_
 
-*What was the result of the game played 120 miles west of Sydney?*
 ```sql
 SELECT * FROM w
     WHERE city = {{
         LLMQA(
             'Which city is located 120 miles west of Sydney?',
             (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
             options='w::city'
         )
     }}
 ```
 
-*Which venues in Sydney saw more than 30 points scored?*
+_Which venues in Sydney saw more than 30 points scored?_
+
 ```sql
 SELECT DISTINCT venue FROM w
     WHERE city = 'sydney' AND {{
         LLMMap(
             'More than 30 total points?',
             'w::score'
         )
     }} = TRUE
 ```
 
-*Show all NSW Waratahs games and a description of the team.*
+_Show all NSW Waratahs games and a description of the team._
+
 ```sql
 SELECT date, rival, score, documents.content AS "Team Description" FROM w
     JOIN {{
         LLMJoin(
             left_on='documents::title',
             right_on='w::rival'
         )
@@ -94,72 +110,76 @@
 
 <p>
 <details>
 <summary> <b> <a href="https://hybridqa.github.io/" target="_blank"> HybridQA </a> </b> </summary>
 
 For this setting, our database contains 2 tables: a table from Wikipedia `w`, and a collection of unstructured Wikipedia articles in the table `documents`.
 
-*What is the state flower of the smallest state by area ?*
+_What is the state flower of the smallest state by area ?_
+
 ```sql
-SELECT "common name" AS 'State Flower' FROM w 
+SELECT "common name" AS 'State Flower' FROM w
 WHERE state = {{
     LLMQA(
         'Which is the smallest state by area?',
         (SELECT title, content FROM documents),
         options='w::state'
     )
 }}
 ```
 
-*Who were the builders of the mosque in Herat with fire temples ?*
+_Who were the builders of the mosque in Herat with fire temples ?_
+
 ```sql
 {{
     LLMQA(
-        'Name of the builders?',
+        'Who were the builders of the mosque?',
         (
-            SELECT title AS 'Building', content FROM documents
-                WHERE title = {{
-                    LLMQA(
-                        'Align the name to the correct title.',
-                        (SELECT name FROM w WHERE city = 'herat' AND remarks LIKE '%fire temple%'),
-                        options='documents::title'
-                    )
-                }}
-        ) 
+            SELECT documents.title AS 'Building', documents.content FROM documents
+            JOIN {{
+                LLMJoin(
+                    left_on='w::name',
+                    right_on='documents::title'
+                )
+            }}
+            WHERE w.city = 'herat' AND w.remarks LIKE '%fire temple%'
+        )
     )
 }}
 ```
 
-*What is the capacity of the venue that was named in honor of Juan Antonio Samaranch in 2010 after his death ?*
+_What is the capacity of the venue that was named in honor of Juan Antonio Samaranch in 2010 after his death ?_
+
 ```sql
 SELECT capacity FROM w WHERE venue = {{
     LLMQA(
         'Which venue is named in honor of Juan Antonio Samaranch?',
         (SELECT title AS 'Venue', content FROM documents),
         options='w::venue'
     )
 }}
-```    
+```
 
 </details>
 </p>
 
 <p>
 <details>
 <summary> <b> <a href="https://ott-qa.github.io/" target="_blank"> OTT-QA </a> </b> </summary>
 
 Unlike HybridQA, these questions are open-domain, where we don't know in advance where the answer of a given open question appears in a passage or a table.
 
 As a result, we need to play the role of both the retriever (to select relevant context) and reader (to read from relevant contexts and return the given answer).
 
 As the underlying database consists of 400K tables and 5M documents, it's important to set `LIMIT` clauses appropriately to ensure reasonable execution times.
 
-The examples below also demonstrate how BlendSQL unpacks [CTE statements](https://www.sqlite.org/lang_with.html) to ensure we only pass necessary data into the BlendSQL ingredient calls. 
+The examples below also demonstrate how BlendSQL unpacks [CTE statements](https://www.sqlite.org/lang_with.html) to ensure we only pass necessary data into the BlendSQL ingredient calls.
+
+_When was the third highest paid Rangers F.C . player born ?_
 
-*When was the third highest paid Rangers F.C . player born ?*
 ```sql
 {{
     LLMQA(
         'When was the Rangers Player born?',
         (
             WITH t AS (
                 SELECT player FROM (
@@ -170,40 +190,42 @@
                 SELECT * FROM documents JOIN t WHERE documents MATCH t.player || ' OR rangers OR fc' ORDER BY rank LIMIT 5
             ) SELECT d.content, t.player AS 'Rangers Player' FROM d JOIN t
         )
     )
 }}
 ```
 
-*In which Track Cycling World Championships event was the person born in Matanzas , Cuba ranked highest ?*
+_In which Track Cycling World Championships event was the person born in Matanzas , Cuba ranked highest ?_
+
 ```sql
 {{
     LLMQA(
         'In what event was the cyclist ranked highest?',
         (
             SELECT * FROM (
                 SELECT * FROM "./Cuba at the UCI Track Cycling World Championships (2)"
             ) as w WHERE w.name = {{
                 LLMQA(
                     "Which cyclist was born in Matanzas, Cuba?",
                     (
-                        SELECT * FROM documents 
-                            WHERE documents MATCH 'matanzas AND (cycling OR track OR born)' 
+                        SELECT * FROM documents
+                            WHERE documents MATCH 'matanzas AND (cycling OR track OR born)'
                             ORDER BY rank LIMIT 3
                     ),
                     options="w::name"
                 )
             }}
         ),
         options='w::event'
     )
 }}
 ```
 
-*Who is the director the Togolese film that was a 30 minute film that was shot in 16mm ?*
+_Who is the director the Togolese film that was a 30 minute film that was shot in 16mm ?_
+
 ```sql
 SELECT director FROM "./List of African films (4)" as w
 WHERE title = {{
     LLMQA(
         'What is the name of the Togolese film that was 30 minutes and shot in 16mm?',
         (SELECT * FROM documents WHERE documents MATCH 'togolese OR 30 OR 16mm OR film' ORDER BY rank LIMIT 5),
         options='w::title'
@@ -216,41 +238,44 @@
 
 <p>
 <details>
 <summary> <b> <a href="https://fever.ai/dataset/feverous.html" target="_blank"> FEVEROUS </a> </b> </summary>
 
 Here, we deal not with questions, but truth claims given a context of unstructured and structured data.
 
-These claims should be judged as "SUPPORTS" or "REFUTES". Using BlendSQL, we can formulate this determination of truth as a function over facts. 
+These claims should be judged as "SUPPORTS" or "REFUTES". Using BlendSQL, we can formulate this determination of truth as a function over facts.
+
+_Oyedaea is part of the family Asteraceae in the order Asterales._
 
-*Oyedaea is part of the family Asteraceae in the order Asterales.*
 ```sql
 SELECT EXISTS (
     SELECT * FROM w0 WHERE "family:" = 'asteraceae' AND "order:" = 'asterales'
-) 
+)
 ```
 
-*The 2006-07 San Jose Sharks season, the 14th season of operation (13th season of play) for the National Hockey League (NHL) franchise, scored the most points in the Pacific Division.*
+_The 2006-07 San Jose Sharks season, the 14th season of operation (13th season of play) for the National Hockey League (NHL) franchise, scored the most points in the Pacific Division._
+
 ```sql
 SELECT (
     {{
         LLMValidate(
-            'Is the Sharks 2006-07 season the 14th season (13th season of play)?', 
+            'Is the Sharks 2006-07 season the 14th season (13th season of play)?',
             (SELECT * FROM documents)
         )
     }}
 ) AND (
     SELECT (SELECT filledcolumnname FROM w0 ORDER BY pts DESC LIMIT 1) = 'san jose sharks'
 )
 ```
 
-*Saunders College of Business, which is accredited by the Association to Advance Collegiate Schools of Business International, is one of the colleges of Rochester Institute of Technology established in 1910 and is currently under the supervision of Dean Jacqueline R. Mozrall.*
+_Saunders College of Business, which is accredited by the Association to Advance Collegiate Schools of Business International, is one of the colleges of Rochester Institute of Technology established in 1910 and is currently under the supervision of Dean Jacqueline R. Mozrall._
+
 ```sql
 SELECT EXISTS(
-    SELECT * FROM w0 
+    SELECT * FROM w0
     WHERE "parent institution" = 'rochester institute of technology'
     AND "established" = '1910'
     AND "dean" = 'jacqueline r. mozrall'
 ) AND (
     {{
         LLMValidate(
             'Is Saunders College of Business (SCB) accredited by the Association to Advance Collegiate Schools of Business International (AACSB)?',
@@ -260,299 +285,339 @@
 )
 ```
 
 </details>
 </p>
 
 ## Table of Contents
-* [Install](#install)
-* [Quickstart](#quickstart)
-* [FAQ](#faq)
-* [Documentation](#documentation)
-  * [Execute a BlendSQL Query](#execute-a-blendsql-query)
-    * [Smoothie](#smoothie)
-  * [Ingredients](#ingredients)
-    * [MapIngredient](#mapingredient)
-    * [QAIngredient](#qaingredient)
-      * [Constrained Decoding with 'options'](#constrained-decoding-with-options)
-    * [JoinIngredient](#joiningredient)
-    * [StringIngredient](#stringingredient)
-  * [LLMs](#llms)
-  * [Databases](#databases)
-* [Appendix](#appendix)
-
-### Features 
-- Smart parsing optimizes what is passed to external functions 🧠
-  - Traverses abstract syntax tree with [sqlglot](https://github.com/tobymao/sqlglot) to minimize LLM function calls 🌳
-- LLM function caching, built on [diskcache](https://grantjenks.com/docs/diskcache/) 🔑 
-- Constrained decoding with [guidance](https://github.com/guidance-ai/guidance) 🚀
 
+- [Install](#install)
+- [Quickstart](#quickstart)
+- [FAQ](#faq)
+- [Documentation](#documentation)
+  - [Execute a BlendSQL Query](#execute-a-blendsql-query)
+    - [Smoothie](#smoothie)
+  - [Ingredients](#ingredients)
+    - [MapIngredient](#mapingredient)
+    - [QAIngredient](#qaingredient)
+      - [Constrained Decoding with 'options'](#constrained-decoding-with-options)
+    - [JoinIngredient](#joiningredient)
+    - [StringIngredient](#stringingredient)
+  - [Parsing Natural Language to BlendSQL](#parsing-natural-language-to-blendsql)
+  - [LLMs](#llms)
+  - [Databases](#databases)
+- [Appendix](#appendix)
 
 For a technical walkthrough of how a BlendSQL query is executed, check out [technical_walkthrough.md](./docs/technical_walkthrough.md).
 
 ## Install
+
 ```
 pip install blendsql
 ```
 
 ## Quickstart
 
 ```python
-from blendsql import blend, LLMQA, LLMMap
+from blendsql import blend, LLMQA
 from blendsql.db import SQLite
 from blendsql.models import OpenaiLLM
+from blendsql.utils import fetch_from_hub
 
 blendsql = """
-SELECT merchant FROM transactions WHERE 
-     {{LLMMap('is this a pizza shop?', 'transactions::merchant')}} = TRUE
-     AND parent_category = 'Food'
+SELECT * FROM w
+WHERE city = {{
+    LLMQA(
+        'Which city is located 120 miles west of Sydney?',
+        (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
+        options='w::city'
+    )
+}}
 """
 # Make our smoothie - the executed BlendSQL script
 smoothie = blend(
     query=blendsql,
-    blender=OpenaiLLM("gpt-3.5-turbo-0613"),
-    ingredients={LLMMap, LLMQA},
-    db=SQLite(db_path="transactions.db"),
-    verbose=True
+    db=SQLite(fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+    blender=OpenaiLLM("gpt-3.5-turbo"),
+    ingredients={LLMQA},
 )
-
+print(smoothie.df)
+print(smoothie.meta.prompts)
 ```
 
 ### FAQ
 
+#### How does BlendSQL execute a query?
+> BlendSQL handles traversal of the SQL AST and creation of temporary tables to execute a given query. 
+> This allows BlendSQL to be DBMS-agnostic, and extendable into both SQLite, PostgreSQL, and other DBMS.
+
 #### Why not just implement BlendSQL as a [user-defined function in SQLite](https://www.sqlite.org/c3ref/c_deterministic.html#sqlitedeterministic)?
-> LLMs are expensive, both in terms of $ cost and compute time. When applying them to SQLite databases, we want to take special care in ensuring we're not applying them to contexts where they're not required. 
+
+> LLMs are expensive, both in terms of $ cost and compute time. When applying them to SQLite databases, we want to take special care in ensuring we're not applying them to contexts where they're not required.
 > This is [not easily achievable with UDFs](https://sqlite.org/forum/info/649ad4c62fd4b4e8cb5d6407107b8c8a9a0afaaf95a87805e5a8403a79e6616c), even when marked as a [deterministic function](https://www.sqlite.org/c3ref/c_deterministic.html#sqlitedeterministic).
-> 
+>
 > BlendSQL is specifically designed to enforce an order-of-operations that 1) prioritizes vanilla SQL operations first, and 2) caches results from LLM ingredients so they don't need to be recomputed.
 > For example:
-> ```sql 
-> SELECT {{LLMMap('What state is this NBA team from?', 'w::team')} FROM w 
->    WHERE num_championships > 3 
+>
+> ```sql
+> SELECT {{LLMMap('What state is this NBA team from?', 'w::team')} FROM w
+>    WHERE num_championships > 3
 >    ORDER BY {{LLMMap('What state is this NBA team from?', 'w::team')}
-> 
+>
 > ```
+>
 > BlendSQL makes sure to only pass those `team` values from rows which satisfy the condition `num_championship > 3` to the LLM. Additionally, since we assume the function is deterministic, we make a single LLM call and cache the results, despite the ingredient function being used twice.
 
+#### So I get how to write BlendSQL queries. But why would I use this over vanilla SQLite?
 
- #### So I get how to write BlendSQL queries. But why would I use this over vanilla SQLite? 
-> Certain ingredients, like [LLMJoin](#joiningredient), will likely give seasoned SQL experts a headache at first. However, BlendSQL's real strength comes from it's use as an *intermediate representation for reasoning over structured + unstructured with LLMs*. Some examples of this can be found above [here](#more-examples-from-popular-qa-datasets).
+> Certain ingredients, like [LLMJoin](#joiningredient), will likely give seasoned SQL experts a headache at first. However, BlendSQL's real strength comes from it's use as an _intermediate representation for reasoning over structured + unstructured with LLMs_. Some examples of this can be found above [here](#more-examples-from-popular-qa-datasets).
 
 <hr>
 
 ### Citation
+
 ```bibtex
 @article{glenn2024blendsql,
-      title={BlendSQL: A Scalable Dialect for Unifying Hybrid Question Answering in Relational Algebra}, 
+      title={BlendSQL: A Scalable Dialect for Unifying Hybrid Question Answering in Relational Algebra},
       author={Parker Glenn and Parag Pravin Dakle and Liang Wang and Preethi Raghavan},
       year={2024},
       eprint={2402.17882},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
 ```
 
 # Documentation
 
-> [!WARNING]
-> WIP, will be updated
+
+## Databases
+
+Since BlendSQL relies on the package [sqlglot](https://github.com/tobymao/sqlglot) for query optimization (which supports a [wide variety of SQL dialects](https://github.com/tobymao/sqlglot/blob/main/sqlglot/dialects/__init__.py)) and the notion of [temporary tables](https://en.wikibooks.org/wiki/Structured_Query_Language/Temporary_Table), it can easily integrate with many different SQL dialects. 
+
+Currently, the following are supported.
+
+### SQLite
+A SQLite database connection.
+Can be initialized via a path to the database file.
+
+Example:
+```python
+from blendsql.db import SQLite
+db = SQLite("./path/to/database.db")
+```
+
+### PostgreSQL
+A PostgreSQL database connection.
+Can be initialized via the SQLAlchemy input string.
+https://docs.sqlalchemy.org/en/20/core/engines.html#postgresql
+
+Example:
+```python
+from blendsql.db import PostgreSQL
+db = PostgreSQL("user:password@localhost/mydatabase")
+```
 
 ## Execute a BlendSQL Query
-The `blend()` function is used to execute a BlendSQL query against a database and return the final result, in addition to the intermediate reasoning steps taken.
 
-::: blendsql.blendsql.blend
-  handler: python
+The `blend()` function is used to execute a BlendSQL query against a database and return the final result, in addition to the intermediate reasoning steps taken.
 
 ```python
-from blendsql import blend, LLMMap, LLMQA, LLMJoin
+from blendsql import blend, LLMQA
 from blendsql.db import SQLite
 from blendsql.models import OpenaiLLM
+from blendsql.utils import fetch_from_hub
 
 blendsql = """
 SELECT * FROM w
 WHERE city = {{
     LLMQA(
         'Which city is located 120 miles west of Sydney?',
         (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
         options='w::city'
     )
-}} 
+}}
 """
-db = SQLite(db_path)
+# Make our smoothie - the executed BlendSQL script
 smoothie = blend(
     query=blendsql,
-    db=db,
-    ingredients={LLMMap, LLMQA, LLMJoin},
-    blender=AzureOpenaiLLM("gpt-4"),
-    # Optional args below
-    infer_gen_constraints=True,
-    silence_db_exec_errors=False,
-    verbose=True,
-    blender_args={
-        "few_shot": True,
-        "temperature": 0.01
-    }
+    db=SQLite(fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+    blender=OpenaiLLM("gpt-3.5-turbo"),
+    ingredients={LLMQA},
 )
+print(smoothie.df)
+print(smoothie.meta.prompts)
 ```
 
+### Smoothie
 
-### Smoothie 
 The [smoothie.py](./blendsql/_smoothie.py) object defines the output of an executed BlendSQL script.
 
 ```python
 @dataclass
 class Smoothie:
     df: pd.DataFrame
     meta: SmoothieMeta
-    
+
 @dataclass
 class SmoothieMeta:
     process_time_seconds: float
     num_values_passed: int  # Number of values passed to a Map/Join/QA ingredient
     num_prompt_tokens: int  # Number of prompt tokens (counting user and assistant, i.e. input/output)
     prompts: List[str] # Log of prompts submitted to model
     example_map_outputs: List[Any]  # outputs from a Map ingredient, for debugging
     ingredients: List[Ingredient]
     query: str
     db_path: str
     contains_ingredient: bool = True
 
 def blend(*args, **kwargs) -> Smoothie:
-  ... 
+  ...
 ```
+
 <hr>
 
-## Ingredients 
+## Ingredients
 
 ![ingredients](docs/img/ingredients.jpg)
 
-Ingredients are at the core of a BlendSQL script. 
+Ingredients are at the core of a BlendSQL script.
 
 They are callable functions that perform one the task paradigms defined in [ingredient.py](./blendsql/ingredients/ingredient.py).
 
-At their core, these are not a new concept. [User-defined functions (UDFs)](https://docs.databricks.com/en/udf/index.html), or [Application-Defined Functions in SQLite](https://www.sqlite.org/appfunc.html) have existed for quite some time. 
+At their core, these are not a new concept. [User-defined functions (UDFs)](https://docs.databricks.com/en/udf/index.html), or [Application-Defined Functions in SQLite](https://www.sqlite.org/appfunc.html) have existed for quite some time.
 
 However, ingredients in BlendSQL are intended to be optimized towards LLM-based functions, defining an order of operations for traversing the AST such that the minimal amount of data is passed into your expensive GPT-4/Llama 2/Mistral 7b/etc. prompt.
 
 Ingredient calls are denoted by wrapping them in double curly brackets, `{{ingredient}}`.
 
 The following ingredient types are valid.
 
 ### MapIngredient
+
 This type of ingredient applies a function on a given table/column pair to create a new column containing the function output.
 
 For example, take the following query.
 
-```sql 
+```sql
 SELECT merchant FROM transactions
     WHERE {{LLMMap('Is this a pizza shop?', 'transactions::merchant')}} = TRUE
 ```
 
 `LLMMap` is one of our builtin MapIngredients. For each of the distinct values in the "merchant" column of the "transactions" table, it will create a column containing the function output.
 
 | merchant | Is this a pizza shop? |
-|----------|-----------------------|
+| -------- | --------------------- |
 | Domino's | 1                     |
 | Safeway  | 0                     |
 | Target   | 0                     |
 
 The temporary table shown above is then combined with the original "transactions" table with an `INNER JOIN` on the "merchant" column.
 
 ### JoinIngredient
+
 Handles the logic of semantic `JOIN` clauses between tables.
 
 For example:
+
 ```sql
 SELECT Capitals.name, State.name FROM Capitals
     JOIN {{
         LLMJoin(
-            'Align state to capital', 
-            left_on='States::name', 
+            'Align state to capital',
+            left_on='States::name',
             right_on='Capitals::name'
         )
     }}
 ```
+
 The above example hints at a database schema that would make [E.F Codd](https://en.wikipedia.org/wiki/Edgar_F._Codd) very angry: why do we have two separate tables `States` and `Capitals` with no foreign key to join the two?
 
 BlendSQL was built to interact with tables "in-the-wild", and many (such as those on Wikipedia) do not have these convenient properties of well-designed relational models.
 
 For this reason, we can leverage the internal knowledge of a pre-trained LLM to do the `JOIN` operation for us.
 
 ### QAIngredient
+
 Sometimes, simply selecting data from a given database is not enough to sufficiently answer a user's question.
 
 The `QAIngredient` is designed to return data of variable types, and is best used in cases when we either need:
-1) Unstructured, free-text responses ("Give me a summary of all my spending in coffe")
-2) Complex, unintuitive relationships extracted from table subsets ("How many consecutive days did I spend in coffee?")
+
+1. Unstructured, free-text responses ("Give me a summary of all my spending in coffe")
+2. Complex, unintuitive relationships extracted from table subsets ("How many consecutive days did I spend in coffee?")
 
 The following query demonstrates usage of the builtin `LLMQA` ingredient.
 
 ```sql
 {{
     LLMQA(
-        'How many consecutive days did I buy stocks in Financials?', 
+        'How many consecutive days did I buy stocks in Financials?',
         (
             SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
               FROM account_history
               LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
               WHERE Sector = "Financials"
               ORDER BY "Run Date" LIMIT 5
         )
     )
-}} 
+}}
 ```
-This is slightly more complicated than the rest of the ingredients. 
+
+This is slightly more complicated than the rest of the ingredients.
 
 Behind the scenes, we wrap the call to `LLMQA` in a trivial `CASE` clause, ensuring that the ingredient's output gets returned.
-```sql 
-SELECT CASE WHEN FALSE THEN FALSE 
+
+```sql
+SELECT CASE WHEN FALSE THEN FALSE
   WHEN TRUE then {{QAIngredient}}
   END
 ```
+
 The LLM gets both the question asked, alongside the subset of the SQL database fetched by our subquery.
 
 | **"Run Date"** | **Symbol** | **Sector** |
-|----------------|------------|------------|
+| -------------- | ---------- | ---------- |
 | 2022-01-14     | HBAN       | Financials |
 | 2022-01-20     | AIG        | Financials |
 | 2022-01-24     | AIG        | Financials |
 | 2022-01-24     | NTRS       | Financials |
 | 2022-01-25     | HBAN       | Financials |
 
-
 From examining this table, we see that we bought stocks in the Financials sector 2 consecutive days (2022-01-24, and 2022-01-25).
 The LLM answers the question in an end-to-end manner, returning the result `2`.
 
 The `QAIngredient` can be used as a standalone end-to-end QA tool, or as a component within a larger BlendSQL query.
 
-For example, the BlendSQL query below translates to the valid (but rather confusing) question: 
+For example, the BlendSQL query below translates to the valid (but rather confusing) question:
 
 "Show me stocks in my portfolio, whose price is greater than the number of consecutive days I bought Financial stocks multiplied by 10. Only display those companies which offer a media streaming service."
+
 ```sql
  SELECT Symbol, "Last Price" FROM portfolio WHERE "Last Price" > {{
   LLMQA(
-        'How many consecutive days did I buy stocks in Financials?', 
+        'How many consecutive days did I buy stocks in Financials?',
         (
             SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
               FROM account_history
               LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
               WHERE Sector = "Financials"
               ORDER BY "Run Date" LIMIT 5
         )
     )
   }} * 10
   AND {{LLMMap('Offers a media streaming service?', 'portfolio::Description')}} = 1
 ```
+
 #### Constrained Decoding with `options`
+
 Perhaps we want the answer to the above question in a different format. We call our LLM ingredient in a constrained setting by passing a `options` argument, where we provide either semicolon-separated options, or a reference to a column.
 
 ```sql
 {{
     LLMQA(
-        'How many consecutive days did I buy stocks in Financials?', 
+        'How many consecutive days did I buy stocks in Financials?',
         (
             SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
               FROM account_history
               LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
               WHERE Sector = "Financials"
               ORDER BY "Run Date" LIMIT 5
         )
@@ -561,27 +626,28 @@
 }}
 ```
 
 Running the above BlendSQL query, we get the output `two consecutive days!`.
 
 This `options` argument can also be a reference to a given column.
 
-For example (from the [HybridQA dataset](https://hybridqa.github.io/)): 
+For example (from the [HybridQA dataset](https://hybridqa.github.io/)):
 
-```sql 
+```sql
  SELECT capacity FROM w WHERE venue = {{
         LLMQA(
             'Which venue is named in honor of Juan Antonio Samaranch?',
             (SELECT title, content FROM documents WHERE content LIKE '%venue%'),
             options='w::venue'
         )
 }}
 ```
 
 Or, from our running example:
+
 ```sql
 {{
   LLMQA(
       'Which did i buy the most?',
       (
         SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
           FROM account_history
@@ -593,56 +659,84 @@
   )
 }}
 ```
 
 The above BlendSQL will yield the result `AIG`, since it appears in the `Symbol` column from `account_history`.
 
 ### StringIngredient
+
 This is the simplest type of ingredient. This will output a string to be placed directly into the SQL query.
 
 We have the `DT` function as a builtin StringIngredient.
 
-```sql 
+```sql
 SELECT merchant FROM transactions
     WHERE {{DT('transactions::date', start='q2')}}
 ```
 
 This will call a Python function that uses `datetime` to interpret the absolute dates which the relative phrase "q2" most likely refers to.
 
 We do not create any new tables or perform any joins with a StringIngredient; instead, we simply get the following SQL query.
 
 > [!NOTE]
 > The below SQL interpretation of the `DT` function assumes we're calling it in December, 2022. The phrase 'q2' will be interpreted differently in, say, March 1998.
 
-```sql 
+```sql
 SELECT merchant FROM transactions
     WHERE date > '2022-09-30' AND date < '2022-12-01'
 ```
 
-<hr> 
- 
+<hr>
+
+## Parsing Natural Language to BlendSQL
 
-## LLMs
+```python
+from blendsql import nl_to_blendsql, LLMMap
+from blendsql.models import TransformersLLM
+from blendsql.db import SQLite
+from blendsql.utils import fetch_from_hub
 
+model = TransformersLLM("Qwen/Qwen1.5-0.5B")
+db = SQLite(fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db"))
 
-<hr> 
+query = nl_to_blendsql(
+    question="Which venues in Sydney saw more than 30 points scored?",
+    model=model,
+    ingredients={LLMMap},
+    serialized_db=db.to_serialized(num_rows=3, use_tables=["w", "documents"]),
+    verbose=True,
+    max_grammar_corrections=5,
+)
+```
 
-## Databases
+### Grammar-Based Correction
 
+If you use the grammar prompting feature of BlendSQL, please cite the original grammar prompting paper below.
 
-<hr> 
+```bibtex
+@article{wang2024grammar,
+  title={Grammar prompting for domain-specific language generation with large language models},
+  author={Wang, Bailin and Wang, Zi and Wang, Xuezhi and Cao, Yuan and A Saurous, Rif and Kim, Yoon},
+  journal={Advances in Neural Information Processing Systems},
+  volume={36},
+  year={2024}
+}
+```
+
+<hr>
 ### Appendix
-#### Run Line Profiling 
+#### Run Line Profiling
 First uncomment `@profile` above `blend()` in `blendsql.py`.
 Make sure you've run `pip install line_profiler` first. This installs the tool here: https://github.com/pyutils/line_profiler
 
 `PYTHONPATH=$PWD:$PYTHONPATH kernprof -lv examples/benchmarks/with_blendsql.py`
 
 #### Benchmarks
-The below benchmarks were done on my local M1 Macbook Pro. by running the scripts found in `examples/benchmarks`. 
+
+The below benchmarks were done on my local M1 Macbook Pro. by running the scripts found in `examples/benchmarks`.
 'Lines of Code' is a rough estimate of the user-written code for each usecase.
 
-| **Name**                     | **Description**                                                 | **Runtime/s (Across 10 runs)** | **Lines of Code** |
-|------------------------------|-----------------------------------------------------------------|-------------------------------------------------|-------------------|
-| BlendSQL                     |                                                     |5.685 +/- 0.930                                 | 9                 |
-| SQL + LLM Calls       | Filtering what we can with SQL, then running LLM calls.         | 9.083 +/- 2.061                                 | 106               |
-| Naive SQL + LLM Calls | Runing LLM calls on entire table, regardless of SQL conditions. | 64.809 +/- 6.225                                | 106               |
+| **Name**              | **Description**                                                 | **Runtime/s (Across 10 runs)** | **Lines of Code** |
+| --------------------- | --------------------------------------------------------------- | ------------------------------ | ----------------- |
+| BlendSQL              |                                                                 | 5.685 +/- 0.930                | 9                 |
+| SQL + LLM Calls       | Filtering what we can with SQL, then running LLM calls.         | 9.083 +/- 2.061                | 106               |
+| Naive SQL + LLM Calls | Runing LLM calls on entire table, regardless of SQL conditions. | 64.809 +/- 6.225               | 106               |
```

#### html2text {}

```diff
@@ -3,183 +3,204 @@
                                         img.shields.io/badge/PRs-Welcome-Green]
                                   [blendsql]
                                  SQL ð¤ LLMs
  CChheecckk oouutt oouurr _oo_nn_ll_ii_nn_ee_ _dd_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ffoorr aa mmoorree ccoommpprreehheennssiivvee oovveerrvviieeww.. Results
 from the paper are available [here](https://github.com/parkervg/blendsql/tree/
                     research-paper/research/paper-results)
 
-## Intro BlendSQL is a *superset of SQLite* for problem decomposition and
-hybrid question-answering with LLMs. As a result, we can *Blend* together... -
-ð¥¤ ...operations over heterogeneous data sources (e.g. tables, text, images)
-- ð¥¤ ...the structured & interpretable reasoning of SQL with the
-generalizable reasoning of LLMs It can be viewed as an inversion of the typical
-text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a SQL
-program. **Now, the user is given the control to oversee all calls (LLM + SQL)
-within a unified query language.** ![comparison](docs/img/comparison.jpg) For
-example, imagine we have the following tables. ### `w` | **date** | **rival** |
-**city** | **venue** | **score** | |----------|---------------------------|----
--------|-----------------------------|-----------| | 31 may | nsw waratahs |
-sydney | agricultural society ground | 11-0 | | 5 jun | northern districts |
-newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney |
-agricultural society ground | 21-2 | | 11 jun | western districts | bathurst |
-bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
-cricket ground | 23-10 | ### `documents` | **title** | **content** | |---------
------------------------|---------------------------------------------------| |
+### Features - Supports many DBMS ð¾ - Currently, SQLite and PostgreSQL are
+functional - more to come! - Easily extendable to [multi-modal usecases](./
+examples/vqa-ingredient.ipynb) ð¼ï¸ - Smart parsing optimizes what is passed
+to external functions ð§  - Traverses abstract syntax tree with [sqlglot]
+(https://github.com/tobymao/sqlglot) to minimize LLM function calls ð³ -
+Constrained decoding with [guidance](https://github.com/guidance-ai/guidance)
+ð - LLM function caching, built on [diskcache](https://grantjenks.com/docs/
+diskcache/) ð ## Intro BlendSQL is a *superset of SQLite* for problem
+decomposition and hybrid question-answering with LLMs. As a result, we can
+*Blend* together... - ð¥¤ ...operations over heterogeneous data sources (e.g.
+tables, text, images) - ð¥¤ ...the structured & interpretable reasoning of SQL
+with the generalizable reasoning of LLMs It can be viewed as an inversion of
+the typical text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a
+SQL program. **Now, the user is given the control to oversee all calls (LLM +
+SQL) within a unified query language.** ![comparison](docs/img/comparison.jpg)
+For example, imagine we have the following tables. ### `w` | **date** |
+**rival** | **city** | **venue** | **score** | | -------- | -------------------
+------ | --------- | --------------------------- | --------- | | 31 may | nsw
+waratahs | sydney | agricultural society ground | 11-0 | | 5 jun | northern
+districts | newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney
+| agricultural society ground | 21-2 | | 11 jun | western districts | bathurst
+| bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
+cricket ground | 23-10 | ### `documents` | **title** | **content** | | --------
+---------------------- | ------------------------------------------------- | |
 sydney | sydney ( /ËsÉªdni/ ( listen ) sid-nee ) is the ... | | new south
 wales waratahs | the new south wales waratahs ( /ËwÉrÉtÉËz/ or ... | |
 sydney showground (moore park) | the former sydney showground ( moore park )
 at... | | sydney cricket ground | the sydney cricket ground ( scg ) is a sports
 ... | | newcastle, new south wales | the newcastle ( /ËnuËkÉËsÉl/ new-kah-
 sÉl ) met... | | bathurst, new south wales | bathurst /ËbÃ¦Î¸Érst/ is a city
 in the central t... | BlendSQL allows us to ask the following questions by
 injecting "ingredients", which are callable functions denoted by double curly
 brackets (`{{`, `}}`). The below examples work out of the box, but you are able
-to design your own ingredients as well! *What was the result of the game played
-120 miles west of Sydney?* ```sql SELECT * FROM w WHERE city = {{ LLMQA( 'Which
+to design your own ingredients as well! _What was the result of the game played
+120 miles west of Sydney?_ ```sql SELECT * FROM w WHERE city = {{ LLMQA( 'Which
 city is located 120 miles west of Sydney?', (SELECT * FROM documents WHERE
-documents MATCH 'sydney OR 120'), options='w::city' ) }} ``` *Which venues in
-Sydney saw more than 30 points scored?* ```sql SELECT DISTINCT venue FROM w
+documents MATCH 'sydney OR 120'), options='w::city' ) }} ``` _Which venues in
+Sydney saw more than 30 points scored?_ ```sql SELECT DISTINCT venue FROM w
 WHERE city = 'sydney' AND {{ LLMMap( 'More than 30 total points?', 'w::score' )
-}} = TRUE ``` *Show all NSW Waratahs games and a description of the team.*
+}} = TRUE ``` _Show all NSW Waratahs games and a description of the team._
 ```sql SELECT date, rival, score, documents.content AS "Team Description" FROM
 w JOIN {{ LLMJoin( left_on='documents::title', right_on='w::rival' ) }} WHERE
 rival = 'nsw waratahs' ``` ### More Examples from Popular QA Datasets
 _HH_yy_bb_rr_ii_dd_QQ_AA_ For this setting, our database contains 2 tables: a table from
 Wikipedia `w`, and a collection of unstructured Wikipedia articles in the table
-`documents`. *What is the state flower of the smallest state by area ?* ```sql
+`documents`. _What is the state flower of the smallest state by area ?_ ```sql
 SELECT "common name" AS 'State Flower' FROM w WHERE state = {{ LLMQA( 'Which is
 the smallest state by area?', (SELECT title, content FROM documents),
-options='w::state' ) }} ``` *Who were the builders of the mosque in Herat with
-fire temples ?* ```sql {{ LLMQA( 'Name of the builders?', ( SELECT title AS
-'Building', content FROM documents WHERE title = {{ LLMQA( 'Align the name to
-the correct title.', (SELECT name FROM w WHERE city = 'herat' AND remarks LIKE
-'%fire temple%'), options='documents::title' ) }} ) ) }} ``` *What is the
-capacity of the venue that was named in honor of Juan Antonio Samaranch in 2010
-after his death ?* ```sql SELECT capacity FROM w WHERE venue = {{ LLMQA( 'Which
-venue is named in honor of Juan Antonio Samaranch?', (SELECT title AS 'Venue',
-content FROM documents), options='w::venue' ) }} ```
+options='w::state' ) }} ``` _Who were the builders of the mosque in Herat with
+fire temples ?_ ```sql {{ LLMQA( 'Who were the builders of the mosque?',
+( SELECT documents.title AS 'Building', documents.content FROM documents JOIN {
+{ LLMJoin( left_on='w::name', right_on='documents::title' ) }} WHERE w.city =
+'herat' AND w.remarks LIKE '%fire temple%' ) ) }} ``` _What is the capacity of
+the venue that was named in honor of Juan Antonio Samaranch in 2010 after his
+death ?_ ```sql SELECT capacity FROM w WHERE venue = {{ LLMQA( 'Which venue is
+named in honor of Juan Antonio Samaranch?', (SELECT title AS 'Venue', content
+FROM documents), options='w::venue' ) }} ```
 _OO_TT_TT_--_QQ_AA_ Unlike HybridQA, these questions are open-domain, where we don't know in
 advance where the answer of a given open question appears in a passage or a
 table. As a result, we need to play the role of both the retriever (to select
 relevant context) and reader (to read from relevant contexts and return the
 given answer). As the underlying database consists of 400K tables and 5M
 documents, it's important to set `LIMIT` clauses appropriately to ensure
 reasonable execution times. The examples below also demonstrate how BlendSQL
 unpacks [CTE statements](https://www.sqlite.org/lang_with.html) to ensure we
-only pass necessary data into the BlendSQL ingredient calls. *When was the
-third highest paid Rangers F.C . player born ?* ```sql {{ LLMQA( 'When was the
+only pass necessary data into the BlendSQL ingredient calls. _When was the
+third highest paid Rangers F.C . player born ?_ ```sql {{ LLMQA( 'When was the
 Rangers Player born?', ( WITH t AS ( SELECT player FROM ( SELECT * FROM "./List
 of Rangers F.C. records and statistics (0)" UNION ALL SELECT * FROM "./List of
 Rangers F.C. records and statistics (1)" ) ORDER BY trim(fee, 'Â£') DESC LIMIT
 1 OFFSET 2 ), d AS ( SELECT * FROM documents JOIN t WHERE documents MATCH
 t.player || ' OR rangers OR fc' ORDER BY rank LIMIT 5 ) SELECT d.content,
-t.player AS 'Rangers Player' FROM d JOIN t ) ) }} ``` *In which Track Cycling
+t.player AS 'Rangers Player' FROM d JOIN t ) ) }} ``` _In which Track Cycling
 World Championships event was the person born in Matanzas , Cuba ranked highest
-?* ```sql {{ LLMQA( 'In what event was the cyclist ranked highest?', ( SELECT *
+?_ ```sql {{ LLMQA( 'In what event was the cyclist ranked highest?', ( SELECT *
 FROM ( SELECT * FROM "./Cuba at the UCI Track Cycling World Championships (2)"
 ) as w WHERE w.name = {{ LLMQA( "Which cyclist was born in Matanzas, Cuba?",
 ( SELECT * FROM documents WHERE documents MATCH 'matanzas AND (cycling OR track
 OR born)' ORDER BY rank LIMIT 3 ), options="w::name" ) }} ), options='w::event'
-) }} ``` *Who is the director the Togolese film that was a 30 minute film that
-was shot in 16mm ?* ```sql SELECT director FROM "./List of African films (4)"
+) }} ``` _Who is the director the Togolese film that was a 30 minute film that
+was shot in 16mm ?_ ```sql SELECT director FROM "./List of African films (4)"
 as w WHERE title = {{ LLMQA( 'What is the name of the Togolese film that was 30
 minutes and shot in 16mm?', (SELECT * FROM documents WHERE documents MATCH
 'togolese OR 30 OR 16mm OR film' ORDER BY rank LIMIT 5), options='w::title' )
 }} ```
 _FF_EE_VV_EE_RR_OO_UU_SS_ Here, we deal not with questions, but truth claims given a context of
 unstructured and structured data. These claims should be judged as "SUPPORTS"
 or "REFUTES". Using BlendSQL, we can formulate this determination of truth as a
-function over facts. *Oyedaea is part of the family Asteraceae in the order
-Asterales.* ```sql SELECT EXISTS ( SELECT * FROM w0 WHERE "family:" =
-'asteraceae' AND "order:" = 'asterales' ) ``` *The 2006-07 San Jose Sharks
+function over facts. _Oyedaea is part of the family Asteraceae in the order
+Asterales._ ```sql SELECT EXISTS ( SELECT * FROM w0 WHERE "family:" =
+'asteraceae' AND "order:" = 'asterales' ) ``` _The 2006-07 San Jose Sharks
 season, the 14th season of operation (13th season of play) for the National
-Hockey League (NHL) franchise, scored the most points in the Pacific Division.*
+Hockey League (NHL) franchise, scored the most points in the Pacific Division._
 ```sql SELECT ( {{ LLMValidate( 'Is the Sharks 2006-07 season the 14th season
 (13th season of play)?', (SELECT * FROM documents) ) }} ) AND ( SELECT (SELECT
 filledcolumnname FROM w0 ORDER BY pts DESC LIMIT 1) = 'san jose sharks' ) ```
-*Saunders College of Business, which is accredited by the Association to
+_Saunders College of Business, which is accredited by the Association to
 Advance Collegiate Schools of Business International, is one of the colleges of
 Rochester Institute of Technology established in 1910 and is currently under
-the supervision of Dean Jacqueline R. Mozrall.* ```sql SELECT EXISTS( SELECT *
+the supervision of Dean Jacqueline R. Mozrall._ ```sql SELECT EXISTS( SELECT *
 FROM w0 WHERE "parent institution" = 'rochester institute of technology' AND
 "established" = '1910' AND "dean" = 'jacqueline r. mozrall' ) AND ( {
 { LLMValidate( 'Is Saunders College of Business (SCB) accredited by the
 Association to Advance Collegiate Schools of Business International (AACSB)?',
 (SELECT * FROM documents) ) }} ) ```
-## Table of Contents * [Install](#install) * [Quickstart](#quickstart) * [FAQ]
-(#faq) * [Documentation](#documentation) * [Execute a BlendSQL Query](#execute-
-a-blendsql-query) * [Smoothie](#smoothie) * [Ingredients](#ingredients) *
-[MapIngredient](#mapingredient) * [QAIngredient](#qaingredient) * [Constrained
-Decoding with 'options'](#constrained-decoding-with-options) * [JoinIngredient]
-(#joiningredient) * [StringIngredient](#stringingredient) * [LLMs](#llms) *
-[Databases](#databases) * [Appendix](#appendix) ### Features - Smart parsing
-optimizes what is passed to external functions ð§  - Traverses abstract syntax
-tree with [sqlglot](https://github.com/tobymao/sqlglot) to minimize LLM
-function calls ð³ - LLM function caching, built on [diskcache](https://
-grantjenks.com/docs/diskcache/) ð - Constrained decoding with [guidance]
-(https://github.com/guidance-ai/guidance) ð For a technical walkthrough of
+## Table of Contents - [Install](#install) - [Quickstart](#quickstart) - [FAQ]
+(#faq) - [Documentation](#documentation) - [Execute a BlendSQL Query](#execute-
+a-blendsql-query) - [Smoothie](#smoothie) - [Ingredients](#ingredients) -
+[MapIngredient](#mapingredient) - [QAIngredient](#qaingredient) - [Constrained
+Decoding with 'options'](#constrained-decoding-with-options) - [JoinIngredient]
+(#joiningredient) - [StringIngredient](#stringingredient) - [Parsing Natural
+Language to BlendSQL](#parsing-natural-language-to-blendsql) - [LLMs](#llms) -
+[Databases](#databases) - [Appendix](#appendix) For a technical walkthrough of
 how a BlendSQL query is executed, check out [technical_walkthrough.md](./docs/
 technical_walkthrough.md). ## Install ``` pip install blendsql ``` ##
-Quickstart ```python from blendsql import blend, LLMQA, LLMMap from blendsql.db
-import SQLite from blendsql.models import OpenaiLLM blendsql = """ SELECT
-merchant FROM transactions WHERE {{LLMMap('is this a pizza shop?',
-'transactions::merchant')}} = TRUE AND parent_category = 'Food' """ # Make our
+Quickstart ```python from blendsql import blend, LLMQA from blendsql.db import
+SQLite from blendsql.models import OpenaiLLM from blendsql.utils import
+fetch_from_hub blendsql = """ SELECT * FROM w WHERE city = {{ LLMQA( 'Which
+city is located 120 miles west of Sydney?', (SELECT * FROM documents WHERE
+documents MATCH 'sydney OR 120'), options='w::city' ) }} """ # Make our
 smoothie - the executed BlendSQL script smoothie = blend( query=blendsql,
-blender=OpenaiLLM("gpt-3.5-turbo-0613"), ingredients={LLMMap, LLMQA}, db=SQLite
-(db_path="transactions.db"), verbose=True ) ``` ### FAQ #### Why not just
+db=SQLite(fetch_from_hub
+("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+blender=OpenaiLLM("gpt-3.5-turbo"), ingredients={LLMQA}, ) print(smoothie.df)
+print(smoothie.meta.prompts) ``` ### FAQ #### How does BlendSQL execute a
+query? > BlendSQL handles traversal of the SQL AST and creation of temporary
+tables to execute a given query. > This allows BlendSQL to be DBMS-agnostic,
+and extendable into both SQLite, PostgreSQL, and other DBMS. #### Why not just
 implement BlendSQL as a [user-defined function in SQLite](https://
 www.sqlite.org/c3ref/c_deterministic.html#sqlitedeterministic)? > LLMs are
 expensive, both in terms of $ cost and compute time. When applying them to
 SQLite databases, we want to take special care in ensuring we're not applying
 them to contexts where they're not required. > This is [not easily achievable
 with UDFs](https://sqlite.org/forum/info/
 649ad4c62fd4b4e8cb5d6407107b8c8a9a0afaaf95a87805e5a8403a79e6616c), even when
 marked as a [deterministic function](https://www.sqlite.org/c3ref/
 c_deterministic.html#sqlitedeterministic). > > BlendSQL is specifically
 designed to enforce an order-of-operations that 1) prioritizes vanilla SQL
 operations first, and 2) caches results from LLM ingredients so they don't need
-to be recomputed. > For example: > ```sql > SELECT {{LLMMap('What state is this
-NBA team from?', 'w::team')} FROM w > WHERE num_championships > 3 > ORDER BY {
-{LLMMap('What state is this NBA team from?', 'w::team')} > > ``` > BlendSQL
-makes sure to only pass those `team` values from rows which satisfy the
-condition `num_championship > 3` to the LLM. Additionally, since we assume the
-function is deterministic, we make a single LLM call and cache the results,
+to be recomputed. > For example: > > ```sql > SELECT {{LLMMap('What state is
+this NBA team from?', 'w::team')} FROM w > WHERE num_championships > 3 > ORDER
+BY {{LLMMap('What state is this NBA team from?', 'w::team')} > > ``` > >
+BlendSQL makes sure to only pass those `team` values from rows which satisfy
+the condition `num_championship > 3` to the LLM. Additionally, since we assume
+the function is deterministic, we make a single LLM call and cache the results,
 despite the ingredient function being used twice. #### So I get how to write
 BlendSQL queries. But why would I use this over vanilla SQLite? > Certain
 ingredients, like [LLMJoin](#joiningredient), will likely give seasoned SQL
 experts a headache at first. However, BlendSQL's real strength comes from it's
-use as an *intermediate representation for reasoning over structured +
-unstructured with LLMs*. Some examples of this can be found above [here](#more-
+use as an _intermediate representation for reasoning over structured +
+unstructured with LLMs_. Some examples of this can be found above [here](#more-
 examples-from-popular-qa-datasets).
 ===============================================================================
 ### Citation ```bibtex @article{glenn2024blendsql, title={BlendSQL: A Scalable
 Dialect for Unifying Hybrid Question Answering in Relational Algebra}, author=
 {Parker Glenn and Parag Pravin Dakle and Liang Wang and Preethi Raghavan},
 year={2024}, eprint={2402.17882}, archivePrefix={arXiv}, primaryClass={cs.CL} }
-``` # Documentation > [!WARNING] > WIP, will be updated ## Execute a BlendSQL
-Query The `blend()` function is used to execute a BlendSQL query against a
-database and return the final result, in addition to the intermediate reasoning
-steps taken. ::: blendsql.blendsql.blend handler: python ```python from
-blendsql import blend, LLMMap, LLMQA, LLMJoin from blendsql.db import SQLite
-from blendsql.models import OpenaiLLM blendsql = """ SELECT * FROM w WHERE city
-= {{ LLMQA( 'Which city is located 120 miles west of Sydney?', (SELECT * FROM
-documents WHERE documents MATCH 'sydney OR 120'), options='w::city' ) }} """ db
-= SQLite(db_path) smoothie = blend( query=blendsql, db=db, ingredients={LLMMap,
-LLMQA, LLMJoin}, blender=AzureOpenaiLLM("gpt-4"), # Optional args below
-infer_gen_constraints=True, silence_db_exec_errors=False, verbose=True,
-blender_args={ "few_shot": True, "temperature": 0.01 } ) ``` ### Smoothie The
-[smoothie.py](./blendsql/_smoothie.py) object defines the output of an executed
-BlendSQL script. ```python @dataclass class Smoothie: df: pd.DataFrame meta:
-SmoothieMeta @dataclass class SmoothieMeta: process_time_seconds: float
-num_values_passed: int # Number of values passed to a Map/Join/QA ingredient
-num_prompt_tokens: int # Number of prompt tokens (counting user and assistant,
-i.e. input/output) prompts: List[str] # Log of prompts submitted to model
-example_map_outputs: List[Any] # outputs from a Map ingredient, for debugging
-ingredients: List[Ingredient] query: str db_path: str contains_ingredient: bool
-= True def blend(*args, **kwargs) -> Smoothie: ... ```
+``` # Documentation ## Databases Since BlendSQL relies on the package [sqlglot]
+(https://github.com/tobymao/sqlglot) for query optimization (which supports a
+[wide variety of SQL dialects](https://github.com/tobymao/sqlglot/blob/main/
+sqlglot/dialects/__init__.py)) and the notion of [temporary tables](https://
+en.wikibooks.org/wiki/Structured_Query_Language/Temporary_Table), it can easily
+integrate with many different SQL dialects. Currently, the following are
+supported. ### SQLite A SQLite database connection. Can be initialized via a
+path to the database file. Example: ```python from blendsql.db import SQLite db
+= SQLite("./path/to/database.db") ``` ### PostgreSQL A PostgreSQL database
+connection. Can be initialized via the SQLAlchemy input string. https://
+docs.sqlalchemy.org/en/20/core/engines.html#postgresql Example: ```python from
+blendsql.db import PostgreSQL db = PostgreSQL("user:password@localhost/
+mydatabase") ``` ## Execute a BlendSQL Query The `blend()` function is used to
+execute a BlendSQL query against a database and return the final result, in
+addition to the intermediate reasoning steps taken. ```python from blendsql
+import blend, LLMQA from blendsql.db import SQLite from blendsql.models import
+OpenaiLLM from blendsql.utils import fetch_from_hub blendsql = """ SELECT *
+FROM w WHERE city = {{ LLMQA( 'Which city is located 120 miles west of
+Sydney?', (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
+options='w::city' ) }} """ # Make our smoothie - the executed BlendSQL script
+smoothie = blend( query=blendsql, db=SQLite(fetch_from_hub
+("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+blender=OpenaiLLM("gpt-3.5-turbo"), ingredients={LLMQA}, ) print(smoothie.df)
+print(smoothie.meta.prompts) ``` ### Smoothie The [smoothie.py](./blendsql/
+_smoothie.py) object defines the output of an executed BlendSQL script.
+```python @dataclass class Smoothie: df: pd.DataFrame meta: SmoothieMeta
+@dataclass class SmoothieMeta: process_time_seconds: float num_values_passed:
+int # Number of values passed to a Map/Join/QA ingredient num_prompt_tokens:
+int # Number of prompt tokens (counting user and assistant, i.e. input/output)
+prompts: List[str] # Log of prompts submitted to model example_map_outputs:
+List[Any] # outputs from a Map ingredient, for debugging ingredients: List
+[Ingredient] query: str db_path: str contains_ingredient: bool = True def blend
+(*args, **kwargs) -> Smoothie: ... ```
 ===============================================================================
 ## Ingredients ![ingredients](docs/img/ingredients.jpg) Ingredients are at the
 core of a BlendSQL script. They are callable functions that perform one the
 task paradigms defined in [ingredient.py](./blendsql/ingredients/
 ingredient.py). At their core, these are not a new concept. [User-defined
 functions (UDFs)](https://docs.databricks.com/en/udf/index.html), or
 [Application-Defined Functions in SQLite](https://www.sqlite.org/appfunc.html)
@@ -191,15 +212,15 @@
 ingredient types are valid. ### MapIngredient This type of ingredient applies a
 function on a given table/column pair to create a new column containing the
 function output. For example, take the following query. ```sql SELECT merchant
 FROM transactions WHERE {{LLMMap('Is this a pizza shop?', 'transactions::
 merchant')}} = TRUE ``` `LLMMap` is one of our builtin MapIngredients. For each
 of the distinct values in the "merchant" column of the "transactions" table, it
 will create a column containing the function output. | merchant | Is this a
-pizza shop? | |----------|-----------------------| | Domino's | 1 | | Safeway |
+pizza shop? | | -------- | --------------------- | | Domino's | 1 | | Safeway |
 0 | | Target | 0 | The temporary table shown above is then combined with the
 original "transactions" table with an `INNER JOIN` on the "merchant" column.
 ### JoinIngredient Handles the logic of semantic `JOIN` clauses between tables.
 For example: ```sql SELECT Capitals.name, State.name FROM Capitals JOIN {
 { LLMJoin( 'Align state to capital', left_on='States::name',
 right_on='Capitals::name' ) }} ``` The above example hints at a database schema
 that would make [E.F Codd](https://en.wikipedia.org/wiki/Edgar_F._Codd) very
@@ -207,29 +228,29 @@
 foreign key to join the two? BlendSQL was built to interact with tables "in-
 the-wild", and many (such as those on Wikipedia) do not have these convenient
 properties of well-designed relational models. For this reason, we can leverage
 the internal knowledge of a pre-trained LLM to do the `JOIN` operation for us.
 ### QAIngredient Sometimes, simply selecting data from a given database is not
 enough to sufficiently answer a user's question. The `QAIngredient` is designed
 to return data of variable types, and is best used in cases when we either
-need: 1) Unstructured, free-text responses ("Give me a summary of all my
-spending in coffe") 2) Complex, unintuitive relationships extracted from table
+need: 1. Unstructured, free-text responses ("Give me a summary of all my
+spending in coffe") 2. Complex, unintuitive relationships extracted from table
 subsets ("How many consecutive days did I spend in coffee?") The following
 query demonstrates usage of the builtin `LLMQA` ingredient. ```sql {{ LLMQA
 ( 'How many consecutive days did I buy stocks in Financials?', ( SELECT
 account_history."Run Date", account_history.Symbol, constituents."Sector" FROM
 account_history LEFT JOIN constituents ON account_history.Symbol =
 constituents.Symbol WHERE Sector = "Financials" ORDER BY "Run Date" LIMIT 5 ) )
 }} ``` This is slightly more complicated than the rest of the ingredients.
 Behind the scenes, we wrap the call to `LLMQA` in a trivial `CASE` clause,
 ensuring that the ingredient's output gets returned. ```sql SELECT CASE WHEN
 FALSE THEN FALSE WHEN TRUE then {{QAIngredient}} END ``` The LLM gets both the
 question asked, alongside the subset of the SQL database fetched by our
-subquery. | **"Run Date"** | **Symbol** | **Sector** | |----------------|------
-------|------------| | 2022-01-14 | HBAN | Financials | | 2022-01-20 | AIG |
+subquery. | **"Run Date"** | **Symbol** | **Sector** | | -------------- | -----
+----- | ---------- | | 2022-01-14 | HBAN | Financials | | 2022-01-20 | AIG |
 Financials | | 2022-01-24 | AIG | Financials | | 2022-01-24 | NTRS | Financials
 | | 2022-01-25 | HBAN | Financials | From examining this table, we see that we
 bought stocks in the Financials sector 2 consecutive days (2022-01-24, and
 2022-01-25). The LLM answers the question in an end-to-end manner, returning
 the result `2`. The `QAIngredient` can be used as a standalone end-to-end QA
 tool, or as a component within a larger BlendSQL query. For example, the
 BlendSQL query below translates to the valid (but rather confusing) question:
@@ -270,25 +291,37 @@
 which the relative phrase "q2" most likely refers to. We do not create any new
 tables or perform any joins with a StringIngredient; instead, we simply get the
 following SQL query. > [!NOTE] > The below SQL interpretation of the `DT`
 function assumes we're calling it in December, 2022. The phrase 'q2' will be
 interpreted differently in, say, March 1998. ```sql SELECT merchant FROM
 transactions WHERE date > '2022-09-30' AND date < '2022-12-01' ```
 ===============================================================================
-## LLMs
-===============================================================================
-## Databases
+## Parsing Natural Language to BlendSQL ```python from blendsql import
+nl_to_blendsql, LLMMap from blendsql.models import TransformersLLM from
+blendsql.db import SQLite from blendsql.utils import fetch_from_hub model =
+TransformersLLM("Qwen/Qwen1.5-0.5B") db = SQLite(fetch_from_hub
+("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")) query =
+nl_to_blendsql( question="Which venues in Sydney saw more than 30 points
+scored?", model=model, ingredients={LLMMap}, serialized_db=db.to_serialized
+(num_rows=3, use_tables=["w", "documents"]), verbose=True,
+max_grammar_corrections=5, ) ``` ### Grammar-Based Correction If you use the
+grammar prompting feature of BlendSQL, please cite the original grammar
+prompting paper below. ```bibtex @article{wang2024grammar, title={Grammar
+prompting for domain-specific language generation with large language models},
+author={Wang, Bailin and Wang, Zi and Wang, Xuezhi and Cao, Yuan and A Saurous,
+Rif and Kim, Yoon}, journal={Advances in Neural Information Processing
+Systems}, volume={36}, year={2024} } ```
 ===============================================================================
 ### Appendix #### Run Line Profiling First uncomment `@profile` above `blend()`
 in `blendsql.py`. Make sure you've run `pip install line_profiler` first. This
 installs the tool here: https://github.com/pyutils/line_profiler
 `PYTHONPATH=$PWD:$PYTHONPATH kernprof -lv examples/benchmarks/with_blendsql.py`
 #### Benchmarks The below benchmarks were done on my local M1 Macbook Pro. by
 running the scripts found in `examples/benchmarks`. 'Lines of Code' is a rough
 estimate of the user-written code for each usecase. | **Name** |
-**Description** | **Runtime/s (Across 10 runs)** | **Lines of Code** | |-------
------------------------|-------------------------------------------------------
-----------|-------------------------------------------------|------------------
--| | BlendSQL | |5.685 +/- 0.930 | 9 | | SQL + LLM Calls | Filtering what we
-can with SQL, then running LLM calls. | 9.083 +/- 2.061 | 106 | | Naive SQL +
-LLM Calls | Runing LLM calls on entire table, regardless of SQL conditions. |
-64.809 +/- 6.225 | 106 |
+**Description** | **Runtime/s (Across 10 runs)** | **Lines of Code** | | ------
+--------------- | -------------------------------------------------------------
+-- | ------------------------------ | ----------------- | | BlendSQL | | 5.685
++/- 0.930 | 9 | | SQL + LLM Calls | Filtering what we can with SQL, then
+running LLM calls. | 9.083 +/- 2.061 | 106 | | Naive SQL + LLM Calls | Runing
+LLM calls on entire table, regardless of SQL conditions. | 64.809 +/- 6.225 |
+106 |
```

### Comparing `blendsql-0.0.141/blendsql/_dialect.py` & `blendsql-0.0.15/blendsql/_dialect.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.141/blendsql/_grammar.py` & `blendsql-0.0.15/blendsql/grammars/_peg_grammar.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import pyparsing
 import pyparsing as pp
 
 pp.ParserElement.enable_packrat()
 
-"""Define pyparsing grammar to extract positional + named args from function."""
+"""Defines PEG (parsing expression grammar) in pyparsing 
+grammar to extract positional + named args from function.
+
+Since we use sqlglot for the main SQLite parsing, we only need to define the BlendSQL
+operations (between "{{", "}}") below.
+"""
 grammar = pp.Forward()
 blendsql_function_name = pp.Word(pp.alphanums + "_")
 nums = pp.Word(pp.nums)
 
 # Parse action to remove opening and closing quotes
 single_qs = pp.QuotedString(quoteChar='"', multiline=True, escChar="\\")
 double_qs = pp.QuotedString(quoteChar="'", multiline=True, escChar="\\")
```

### Comparing `blendsql-0.0.141/blendsql/_program.py` & `blendsql-0.0.15/blendsql/_program.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 """
 Contains base class for guidance programs for LLMs.
 https://github.com/guidance-ai/guidance
 """
 from typing import Optional
-from guidance.models import Model, Chat
+from guidance.models import Model as GuidanceModel
+from guidance.models import Chat as GuidanceChatModel
 from guidance import user, system, assistant
 from contextlib import nullcontext
 import inspect
 import ast
 import textwrap
 
 
-def get_contexts(model: Model):
+def get_contexts(model: GuidanceModel):
     usercontext = nullcontext()
     systemcontext = nullcontext()
     assistantcontext = nullcontext()
-    if isinstance(model, Chat):
+    if isinstance(model, GuidanceChatModel):
         usercontext = user()
         systemcontext = system()
         assistantcontext = assistant()
     return (usercontext, systemcontext, assistantcontext)
 
 
 class Program:
+    """
+    TODO: how to add streaming?
+        if isinstance(res, ModelStream):
+        # Fetch actual model by iterating
+        # https://github.com/guidance-ai/guidance/blob/main/tests/models/test_model.py#L85
+        for idx, event in enumerate(res):
+            print(Fore.LIGHTCYAN_EX + str(event) + Fore.RESET)
+            res = event
+    """
+
     def __new__(
         self,
-        model: Model,
+        model: GuidanceModel,
         gen_kwargs: Optional[dict] = None,
         few_shot: bool = True,
         **kwargs,
     ):
         self.model = model
-        self.gen_kwargs = gen_kwargs if gen_kwargs is not None else {}
+        self.gen_kwargs = gen_kwargs
+        self.gen_kwargs = {} if gen_kwargs is None else gen_kwargs
         self.few_shot = few_shot
-        assert isinstance(
-            self.model, Model
-        ), f"GuidanceProgram needs a guidance.models.Model object!\nGot {type(self.model)}"
         (
             self.usercontext,
             self.systemcontext,
             self.assistantcontext,
         ) = get_contexts(self.model)
         return self.__call__(self, **kwargs)
 
@@ -62,22 +71,23 @@
         >>> class CorrectionProgram(Program):
         >>>     def __call__(self, question: str, **kwargs):
         >>>         return self.model + PROMPT.format(question)
 
     Some helpful refs:
         - https://github.com/universe-proton/universe-topology/issues/15
     """
-    call_content = textwrap.dedent(inspect.getsource(program.__call__))
+    source_func = program.__call__
+    call_content = textwrap.dedent(inspect.getsource(source_func))
     root = ast.parse(call_content)
     root_names = {node.id for node in ast.walk(root) if isinstance(node, ast.Name)}
-    co_varnames = set(program.__call__.__code__.co_varnames)
+    co_varnames = set(source_func.__code__.co_varnames)
     names_to_resolve = sorted(root_names.difference(co_varnames))
     resolved_names = ""
     if len(names_to_resolve) > 0:
-        globals_as_dict = dict(inspect.getmembers(program.__call__))["__globals__"]
+        globals_as_dict = dict(inspect.getmembers(source_func))["__globals__"]
         for name in names_to_resolve:
             if name in globals_as_dict:
                 val = globals_as_dict[name]
-                # Ignore functions
+                # Ignore functions - we really only want scalars here
                 if not callable(val):
                     resolved_names += f"{val}\n"
     return f"{call_content}{resolved_names}"
```

### Comparing `blendsql-0.0.141/blendsql/_smoothie.py` & `blendsql-0.0.15/blendsql/_smoothie.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from dataclasses import dataclass
-from typing import List, Any, Collection
+from typing import List, Collection
 import pandas as pd
 
 from .ingredients import Ingredient
 
 """
 Defines output of an executed BlendSQL script
 """
 
 
 @dataclass
 class SmoothieMeta:
-    process_time_seconds: float
     num_values_passed: int  # Number of values passed to a Map/Join/QA ingredient
     num_prompt_tokens: int  # Number of prompt tokens (counting user and assistant, i.e. input/output)
     prompts: List[str]  # Log of prompts submitted to model
-    example_map_outputs: List[Any]  # outputs from a Map ingredient, for debugging
     ingredients: Collection[Ingredient]
     query: str
     db_path: str
     contains_ingredient: bool = True
+    process_time_seconds: float = None
 
 
 @dataclass
 class Smoothie:
     df: pd.DataFrame
     meta: SmoothieMeta
```

### Comparing `blendsql-0.0.141/blendsql/_sqlglot.py` & `blendsql-0.0.15/blendsql/_sqlglot.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,16 +81,17 @@
             if "query" in where_arg.args and isinstance(
                 where_arg.args["query"], exp.Boolean
             ):
                 return None
     # Don't check *all* predicates here
     # Since 'WHERE a = TRUE' is valid and should be kept
     elif isinstance(node, exp.In):
-        if isinstance(node.args["query"], exp.Boolean):
-            return None
+        if "query" in node.args:
+            if isinstance(node.args["query"], exp.Boolean):
+                return None
     return node
 
 
 def prune_with(node):
     """
     Removes any exp.With nodes.
 
@@ -319,15 +320,17 @@
     return list(literals)
 
 
 def get_reversed_subqueries(node):
     """Iterates through all subqueries (either parentheses or select).
     Reverses all EXCEPT for CTEs, which should remain in order.
     """
+    # First, fetch all common table expressions
     r = [i for i in node.find_all(SUBQUERY_EXP + (exp.Paren,)) if is_in_cte(i)]
+    # Then, add (reversed) other subqueries
     return (
         r
         + [i for i in node.find_all(SUBQUERY_EXP + (exp.Paren,)) if not is_in_cte(i)][
             ::-1
         ]
     )
```

### Comparing `blendsql-0.0.141/blendsql/blendsql.py` & `blendsql-0.0.15/blendsql/blend.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,33 +11,31 @@
     List,
     Set,
     Tuple,
     Generator,
     Optional,
     Callable,
     Collection,
-    Any,
 )
 from sqlite3 import OperationalError
 import sqlglot.expressions
 from attr import attrs, attrib
 from functools import partial
 from sqlglot import exp
 from colorama import Fore
 import string
 
 from .utils import (
     sub_tablename,
     get_temp_session_table,
     get_temp_subquery_table,
-    delete_session_tables,
     recover_blendsql,
     get_tablename_colname,
 )
-from .db.sqlite import SQLite
+from .db import Database
 from .db.utils import double_quote_escape, single_quote_escape
 from ._sqlglot import (
     MODIFIERS,
     get_first_child,
     get_reversed_subqueries,
     replace_join_with_ingredient_single_ingredient,
     replace_join_with_ingredient_multiple_ingredient,
@@ -46,29 +44,29 @@
     replace_subquery_with_direct_alias_call,
     maybe_set_subqueries_to_true,
     SubqueryContextManager,
     remove_ctes,
     is_in_cte,
 )
 from ._dialect import _parse_one, FTS5SQLite
-from ._grammar import grammar
+from .grammars._peg_grammar import grammar
 from .ingredients.ingredient import Ingredient, IngredientException
 from ._smoothie import Smoothie, SmoothieMeta
 from ._constants import (
     IngredientType,
     IngredientKwarg,
 )
 from .models._model import Model
 
 
 @attrs
 class Kitchen(list):
     """Superset of list. A collection of ingredients."""
 
-    db: SQLite = attrib()
+    db: Database = attrib()
     session_uuid: str = attrib()
 
     added_ingredient_names: set = attrib(init=False)
 
     def __attrs_post_init__(self):
         self.added_ingredient_names = set()
 
@@ -284,28 +282,31 @@
     return (query, ingredient_alias_to_parsed_dict, tables_in_ingredients)
 
 
 def set_subquery_to_alias(
     subquery: exp.Expression,
     aliasname: str,
     query: exp.Expression,
-    db: SQLite,
+    db: Database,
     blender: Model,
     ingredient_alias_to_parsed_dict: Dict[str, dict],
     **kwargs,
 ) -> exp.Expression:
     str_subquery = recover_blendsql(subquery.sql(dialect=FTS5SQLite))
-    disambiguate_and_submit_blend(
-        ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
-        query=str_subquery,
-        db=db,
-        blender=blender,
-        aliasname=aliasname,
-        **kwargs,
-    ).df.to_sql(aliasname, db.con, if_exists="replace", index=False)
+    db.to_temp_table(
+        df=disambiguate_and_submit_blend(
+            ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
+            query=str_subquery,
+            db=db,
+            blender=blender,
+            aliasname=aliasname,
+            **kwargs,
+        ).df,
+        tablename=aliasname,
+    )
     # Now, we need to remove subquery and instead insert direct reference to aliasname
     # Example:
     #   `SELECT Symbol FROM (SELECT DISTINCT Symbol FROM portfolio) AS w`
     #   Should become: `SELECT Symbol FROM w`
     return query.transform(
         replace_subquery_with_direct_alias_call,
         subquery=subquery.parent,
@@ -377,512 +378,513 @@
     Used to disambiguate anonymized BlendSQL function and execute in a recursive context.
     """
     for alias, d in ingredient_alias_to_parsed_dict.items():
         query = re.sub(re.escape(alias), d["raw"], query)
     logging.debug(
         Fore.CYAN + f"Executing `{query}` and setting to `{aliasname}`..." + Fore.RESET
     )
-    return blend(query=query, **kwargs)
+    return _blend(query=query, **kwargs)
 
 
-def blend(
+def _blend(
     query: str,
-    db: SQLite,
+    db: Database,
     blender: Optional[Model] = None,
     ingredients: Optional[Collection[Ingredient]] = None,
     verbose: bool = False,
     blender_args: Optional[Dict[str, str]] = None,
-    infer_gen_constraints: bool = False,
+    infer_gen_constraints: bool = True,
     table_to_title: Optional[Dict[str, str]] = None,
-    silence_db_exec_errors: bool = True,
-    # User shouldn't interact with below
+    schema_qualify: bool = True,
     _prev_passed_values: int = 0,
-    _prev_cleanup_tables: Set[str] = None,
 ) -> Smoothie:
-    """The `blend()` function is used to execute a BlendSQL query against a database and
-    return the final result, in addition to the intermediate reasoning steps taken.
-    Execution is done on a database given an ingredient context.
-
-    Args:
-        query: The BlendSQL query to execute
-        db: Database connector object
-        ingredients: List of ingredient objects, to use in interpreting BlendSQL query
-        verbose: Boolean defining whether to run in logging.debug mode
-        blender: Optionally override whatever llm argument we pass to Model ingredient.
-            Useful for research applications, where we don't (necessarily) want the parser to choose endpoints.
-        infer_gen_constraints: Optionally infer the output format of an `IngredientMap` call, given the predicate context
-            For example, in `{{LLMMap('convert to date', 'w::listing date')}} <= '1960-12-31'`
-            We can infer the output format should look like '1960-12-31'
-                and put this in the `example_outputs` kwarg
-        table_to_title: Optional mapping from table name to title of table.
-            Useful for datasets like WikiTableQuestions, where relevant info is stored in table title.
-
-    Returns:
-        smoothie: Smoothie dataclass containing pd.DataFrame output and execution metadata
+    """Invoked from blend(), this contains the recursive logic to execute
+    a BlendSQL query and return a `Smoothie` object.
     """
-    cleanup_tables = set() if _prev_cleanup_tables is None else _prev_cleanup_tables
-    if verbose:
-        logging.getLogger().setLevel(logging.DEBUG)
-    else:
-        logging.getLogger().setLevel(logging.ERROR)
+    naive_execution = False
+    session_uuid = str(uuid.uuid4())[:4]
+    if ingredients is None:
+        ingredients = []
+    # Create our Kitchen
+    kitchen = Kitchen(db=db, session_uuid=session_uuid)
+    kitchen.extend(ingredients)
+    (
+        query,
+        ingredient_alias_to_parsed_dict,
+        tables_in_ingredients,
+    ) = preprocess_blendsql(query, blender_args=blender_args, blender=blender)
     try:
-        start = time.time()
-        example_map_outputs: List[Tuple[Any, Any]] = []
-        naive_execution = False
-        session_uuid = str(uuid.uuid4())[:4]
-        if ingredients is None:
-            ingredients = []
-        # Create our Kitchen
-        kitchen = Kitchen(db=db, session_uuid=session_uuid)
-        kitchen.extend(ingredients)
-        (
-            query,
-            ingredient_alias_to_parsed_dict,
-            tables_in_ingredients,
-        ) = preprocess_blendsql(query, blender_args=blender_args, blender=blender)
-        try:
-            # Try to parse as a normal SQLite query
-            _query: exp.Expression = _parse_one(query)
-            original_query = copy.deepcopy(
-                recover_blendsql(_query.sql(dialect=FTS5SQLite))
-            )
-            query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
-        except sqlglot.errors.ParseError:
-            # If we hit an error, wrap in SQLite logic so it's able to be executed
-            _query, original_query = autowrap_query(
-                query=query,
-                kitchen=kitchen,
-                ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
-            )
-            query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
+        # Try to parse as a normal SQLite query
+        _query: exp.Expression = _parse_one(query)
+        original_query = copy.deepcopy(recover_blendsql(_query.sql(dialect=FTS5SQLite)))
+        query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
+    except sqlglot.errors.ParseError:
+        # If we hit an error, wrap in SQLite logic so it's able to be executed
+        _query, original_query = autowrap_query(
+            query=query,
+            kitchen=kitchen,
+            ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
+        )
+        query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
 
-        # Preliminary check - we can't have anything that modifies database state
-        if _query.find(MODIFIERS):
-            raise ValueError("BlendSQL query cannot have `DELETE` clause!")
-
-        # If there's no `SELECT` and just a QAIngredient, wrap it in a `SELECT CASE` query
-        if _query.find(exp.Select) is None:
-            _query, original_query = autowrap_query(
-                query=query,
-                kitchen=kitchen,
-                ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
-            )
-            query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
+    # Preliminary check - we can't have anything that modifies database state
+    if _query.find(MODIFIERS):
+        raise ValueError("BlendSQL query cannot have `DELETE` clause!")
+
+    # If there's no `SELECT` and just a QAIngredient, wrap it in a `SELECT CASE` query
+    if _query.find(exp.Select) is None:
+        _query, original_query = autowrap_query(
+            query=query,
+            kitchen=kitchen,
+            ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
+        )
+        query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
 
-        # If we don't have any ingredient calls, execute as normal SQL
-        if len(ingredients) == 0 or len(ingredient_alias_to_parsed_dict) == 0:
-            return Smoothie(
-                df=db.execute_query(query, silence_errors=silence_db_exec_errors),
-                meta=SmoothieMeta(
-                    process_time_seconds=time.time() - start,
-                    num_values_passed=0,
-                    num_prompt_tokens=0,
-                    prompts=blender.prompts if blender is not None else [],
-                    example_map_outputs=example_map_outputs,
-                    ingredients=[],
-                    query=original_query,
-                    db_path=db.db_path,
-                    contains_ingredient=False,
-                ),
-            )
-        _get_temp_session_table: Callable = partial(
-            get_temp_session_table, session_uuid
+    # If we don't have any ingredient calls, execute as normal SQL
+    if len(ingredients) == 0 or len(ingredient_alias_to_parsed_dict) == 0:
+        return Smoothie(
+            df=db.execute_query(query),
+            meta=SmoothieMeta(
+                num_values_passed=0,
+                num_prompt_tokens=0,
+                prompts=blender.prompts if blender is not None else [],
+                ingredients=[],
+                query=original_query,
+                db_path=db.db_path,
+                contains_ingredient=False,
+            ),
         )
-        # Mapping from {"QA('does this company...', 'constituents::Name')": 'does this company'...})
-        function_call_to_res: Dict[str, str] = {}
-        session_modified_tables = set()
-        # TODO: Currently, as we traverse upwards from deepest subquery,
-        #   if any lower subqueries have an ingredient, we deem the current
-        #   as inelligible for optimization. Maybe this can be improved in the future.
-        prev_subquery_has_ingredient = False
-        for subquery_idx, subquery in enumerate(get_reversed_subqueries(_query)):
-            # At this point, we should have already handled cte statements and created associated tables
-            if subquery.find(exp.With) is not None:
-                subquery = subquery.transform(remove_ctes)
-            # Only cache executed_ingredients within the same subquery
-            # The same ingredient may have different results within a different subquery context
-            executed_subquery_ingredients: Set[str] = set()
-            prev_subquery_map_columns: Set[str] = set()
-            _get_temp_subquery_table: Callable = partial(
-                get_temp_subquery_table, session_uuid, subquery_idx
-            )
-            if not isinstance(subquery, exp.Select):
-                # We need to create a select query from this subquery
-                # So we find the parent select, and grab that table
-                parent_select_tablenames = [
-                    i.name
-                    for i in subquery.find_ancestor(exp.Select).find_all(exp.Table)
-                ]
-                if len(parent_select_tablenames) == 1:
-                    subquery_str = recover_blendsql(
-                        f"SELECT * FROM {parent_select_tablenames[0]} WHERE "
-                        + get_first_child(subquery).sql(dialect=FTS5SQLite)
-                    )
-                else:
-                    logging.debug(
-                        Fore.YELLOW
-                        + "Encountered subquery without `SELECT`, and more than 1 table!\nCannot optimize yet, skipping this step."
-                    )
-                    continue
+    _get_temp_session_table: Callable = partial(get_temp_session_table, session_uuid)
+    # Mapping from {"QA('does this company...', 'constituents::Name')": 'does this company'...})
+    function_call_to_res: Dict[str, str] = {}
+    session_modified_tables = set()
+    # TODO: Currently, as we traverse upwards from deepest subquery,
+    #   if any lower subqueries have an ingredient, we deem the current
+    #   as inelligible for optimization. Maybe this can be improved in the future.
+    prev_subquery_has_ingredient = False
+    for subquery_idx, subquery in enumerate(get_reversed_subqueries(_query)):
+        # At this point, we should have already handled cte statements and created associated tables
+        if subquery.find(exp.With) is not None:
+            subquery = subquery.transform(remove_ctes)
+        # Only cache executed_ingredients within the same subquery
+        # The same ingredient may have different results within a different subquery context
+        executed_subquery_ingredients: Set[str] = set()
+        prev_subquery_map_columns: Set[str] = set()
+        _get_temp_subquery_table: Callable = partial(
+            get_temp_subquery_table, session_uuid, subquery_idx
+        )
+        if not isinstance(subquery, exp.Select):
+            # We need to create a select query from this subquery
+            # So we find the parent select, and grab that table
+            parent_select_tablenames = [
+                i.name for i in subquery.find_ancestor(exp.Select).find_all(exp.Table)
+            ]
+            if len(parent_select_tablenames) == 1:
+                subquery_str = recover_blendsql(
+                    f"SELECT * FROM {parent_select_tablenames[0]} WHERE "
+                    + get_first_child(subquery).sql(dialect=FTS5SQLite)
+                )
             else:
-                subquery_str = recover_blendsql(subquery.sql(dialect=FTS5SQLite))
+                logging.debug(
+                    Fore.YELLOW
+                    + "Encountered subquery without `SELECT`, and more than 1 table!\nCannot optimize yet, skipping this step."
+                )
+                continue
+        else:
+            subquery_str = recover_blendsql(subquery.sql(dialect=FTS5SQLite))
 
-            in_cte, table_alias_name = is_in_cte(subquery, return_name=True)
-            scm = SubqueryContextManager(
-                node=_parse_one(
-                    subquery_str, schema=db.get_sqlglot_schema()
-                ),  # Need to do this so we don't track parents into construct_abstracted_selects
-                prev_subquery_has_ingredient=prev_subquery_has_ingredient,
-                alias_to_subquery={table_alias_name: subquery} if in_cte else None,
-                tables_in_ingredients=tables_in_ingredients,
-            )
-            for tablename, abstracted_query in scm.abstracted_table_selects():
-                # If this table isn't being used in any ingredient calls, there's no
-                #   need to create a temporary session table
-                if (tablename not in tables_in_ingredients) and (
-                    scm.tablename_to_alias.get(tablename, None)
-                    not in tables_in_ingredients
-                ):
-                    continue
-                aliased_subquery = scm.alias_to_subquery.pop(tablename, None)
-                if aliased_subquery is not None:
-                    # First, we need to explicitly create the aliased subquery as a table
-                    # For example, `SELECT Symbol FROM (SELECT DISTINCT Symbol FROM portfolio) AS w WHERE w...`
-                    # We can't assign `abstracted_query` for non-existent `w`
-                    #   until we set `w` to `SELECT DISTINCT Symbol FROM portfolio`
-                    _query = set_subquery_to_alias(
-                        subquery=aliased_subquery,
-                        aliasname=tablename,
-                        query=_query,
-                        blender=blender,
-                        db=db,
-                        ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
-                        # Below are in case we need to call blend() again
-                        ingredients=ingredients,
-                        blender_args=blender_args,
-                        infer_gen_constraints=infer_gen_constraints,
-                        silence_db_exec_errors=silence_db_exec_errors,
-                        table_to_title=table_to_title,
-                        verbose=verbose,
-                        _prev_passed_values=_prev_passed_values,
-                        _prev_cleanup_tables=cleanup_tables,
-                    )
-                    query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
-                    cleanup_tables.add(tablename)
-                if abstracted_query is not None:
-                    logging.debug(
-                        Fore.CYAN
-                        + f"Executing `{abstracted_query}` and setting to `{_get_temp_subquery_table(tablename)}`..."
-                        + Fore.RESET
-                    )
-                    try:
-                        db.execute_query(abstracted_query).to_sql(
-                            _get_temp_subquery_table(tablename),
-                            db.con,
-                            if_exists="replace",
-                            index=False,
-                        )
-                        cleanup_tables.add(_get_temp_subquery_table(tablename))
-                    except OperationalError:
-                        # Fallback to naive execution
-                        naive_execution = True
-            # Be sure to handle those remaining aliases, which didn't have abstracted queries
-            for aliasname, aliased_subquery in scm.alias_to_subquery.items():
+        in_cte, table_alias_name = is_in_cte(subquery, return_name=True)
+        schema = None
+        if schema_qualify:  # Only construct sqlglot schema if we need to
+            schema = db.get_sqlglot_schema()
+        scm = SubqueryContextManager(
+            node=_parse_one(
+                subquery_str, schema=schema
+            ),  # Need to do this so we don't track parents into construct_abstracted_selects
+            prev_subquery_has_ingredient=prev_subquery_has_ingredient,
+            alias_to_subquery={table_alias_name: subquery} if in_cte else None,
+            tables_in_ingredients=tables_in_ingredients,
+        )
+        for tablename, abstracted_query in scm.abstracted_table_selects():
+            # If this table isn't being used in any ingredient calls, there's no
+            #   need to create a temporary session table
+            if (tablename not in tables_in_ingredients) and (
+                scm.tablename_to_alias.get(tablename, None) not in tables_in_ingredients
+            ):
+                continue
+            aliased_subquery = scm.alias_to_subquery.pop(tablename, None)
+            if aliased_subquery is not None:
+                # First, we need to explicitly create the aliased subquery as a table
+                # For example, `SELECT Symbol FROM (SELECT DISTINCT Symbol FROM portfolio) AS w WHERE w...`
+                # We can't assign `abstracted_query` for non-existent `w`
+                #   until we set `w` to `SELECT DISTINCT Symbol FROM portfolio`
                 _query = set_subquery_to_alias(
                     subquery=aliased_subquery,
-                    aliasname=aliasname,
+                    aliasname=tablename,
                     query=_query,
                     blender=blender,
                     db=db,
                     ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
                     # Below are in case we need to call blend() again
                     ingredients=ingredients,
                     blender_args=blender_args,
                     infer_gen_constraints=infer_gen_constraints,
-                    silence_db_exec_errors=silence_db_exec_errors,
                     table_to_title=table_to_title,
                     verbose=verbose,
                     _prev_passed_values=_prev_passed_values,
-                    _prev_cleanup_tables=cleanup_tables,
                 )
                 query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
-                cleanup_tables.add(aliasname)
-            if prev_subquery_has_ingredient:
-                scm.set_node(scm.node.transform(maybe_set_subqueries_to_true))
-
-            # After above processing of AST, sync back to string repr
-            subquery_str = scm.sql()
-            # Now, 1) Find all ingredients to execute (e.g. '{{f(a, b, c)}}')
-            # 2) Track when we've created a new table from a MapIngredient call
-            #   only at the end of parsing a subquery, we can merge to the original session_uuid table
-            tablename_to_map_out: Dict[str, List[pd.DataFrame]] = {}
-            for (
-                start,
-                end,
-                alias_function_str,
-                parsed_results_dict,
-                ingredient,
-            ) in get_sorted_grammar_matches(
-                q=subquery_str,
+            if abstracted_query is not None:
+                logging.debug(
+                    Fore.CYAN
+                    + f"Executing `{abstracted_query}` and setting to `{_get_temp_subquery_table(tablename)}`..."
+                    + Fore.RESET
+                )
+                try:
+                    db.to_temp_table(
+                        df=db.execute_query(abstracted_query),
+                        tablename=_get_temp_subquery_table(tablename),
+                    )
+                except OperationalError as e:
+                    # Fallback to naive execution
+                    logging.debug(Fore.RED + e + Fore.RESET)
+                    logging.debug(
+                        Fore.RED + "Falling back to naive execution..." + Fore.RESET
+                    )
+                    naive_execution = True
+        # Be sure to handle those remaining aliases, which didn't have abstracted queries
+        for aliasname, aliased_subquery in scm.alias_to_subquery.items():
+            _query = set_subquery_to_alias(
+                subquery=aliased_subquery,
+                aliasname=aliasname,
+                query=_query,
+                blender=blender,
+                db=db,
                 ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
-                kitchen=kitchen,
-            ):
-                prev_subquery_has_ingredient = True
-                if alias_function_str in executed_subquery_ingredients:
-                    # Don't execute same ingredient twice
-                    continue
-                executed_subquery_ingredients.add(alias_function_str)
-                kwargs_dict = parsed_results_dict["kwargs_dict"]
+                # Below are in case we need to call blend() again
+                ingredients=ingredients,
+                blender_args=blender_args,
+                infer_gen_constraints=infer_gen_constraints,
+                table_to_title=table_to_title,
+                verbose=verbose,
+                _prev_passed_values=_prev_passed_values,
+            )
+            query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
+        if prev_subquery_has_ingredient:
+            scm.set_node(scm.node.transform(maybe_set_subqueries_to_true))
 
-                if ingredient.ingredient_type == IngredientType.MAP:
-                    if infer_gen_constraints:
-                        # Latter is the winner.
-                        # So if we already define something in kwargs_dict,
-                        #   It's not overriden here
-                        kwargs_dict = (
-                            scm.infer_gen_constraints(
-                                start=start,
-                                end=end,
-                            )
-                            | kwargs_dict
+        # After above processing of AST, sync back to string repr
+        subquery_str = scm.sql()
+        # Now, 1) Find all ingredients to execute (e.g. '{{f(a, b, c)}}')
+        # 2) Track when we've created a new table from a MapIngredient call
+        #   only at the end of parsing a subquery, we can merge to the original session_uuid table
+        tablename_to_map_out: Dict[str, List[pd.DataFrame]] = {}
+        for (
+            start,
+            end,
+            alias_function_str,
+            parsed_results_dict,
+            ingredient,
+        ) in get_sorted_grammar_matches(
+            q=subquery_str,
+            ingredient_alias_to_parsed_dict=ingredient_alias_to_parsed_dict,
+            kitchen=kitchen,
+        ):
+            prev_subquery_has_ingredient = True
+            if alias_function_str in executed_subquery_ingredients:
+                # Don't execute same ingredient twice
+                continue
+            executed_subquery_ingredients.add(alias_function_str)
+            kwargs_dict = parsed_results_dict["kwargs_dict"]
+
+            if ingredient.ingredient_type == IngredientType.MAP:
+                if infer_gen_constraints:
+                    # Latter is the winner.
+                    # So if we already define something in kwargs_dict,
+                    #   It's not overriden here
+                    kwargs_dict = (
+                        scm.infer_gen_constraints(
+                            start=start,
+                            end=end,
                         )
+                        | kwargs_dict
+                    )
 
-                if table_to_title is not None:
-                    kwargs_dict["table_to_title"] = table_to_title
+            if table_to_title is not None:
+                kwargs_dict["table_to_title"] = table_to_title
 
-                # Optionally, recursively call blend() again to get subtable
-                # This applies to `context` and `options`
-                for i, unpack_kwarg in enumerate(
-                    [IngredientKwarg.CONTEXT, IngredientKwarg.OPTIONS]
+            # Optionally, recursively call blend() again to get subtable
+            # This applies to `context` and `options`
+            for i, unpack_kwarg in enumerate(
+                [IngredientKwarg.CONTEXT, IngredientKwarg.OPTIONS]
+            ):
+                unpack_value = kwargs_dict.get(
+                    unpack_kwarg,
+                    parsed_results_dict["args"][i + 1]
+                    if len(parsed_results_dict["args"]) > i + 1
+                    else parsed_results_dict["args"][i]
+                    if len(parsed_results_dict["args"]) > i
+                    else "",
+                )
+                if isinstance(unpack_value, str) and unpack_value.upper().startswith(
+                    ("SELECT", "WITH")
                 ):
-                    unpack_value = kwargs_dict.get(
-                        unpack_kwarg,
-                        parsed_results_dict["args"][i + 1]
-                        if len(parsed_results_dict["args"]) > i + 1
-                        else parsed_results_dict["args"][i]
-                        if len(parsed_results_dict["args"]) > i
-                        else "",
-                    )
-                    if unpack_value.upper().startswith(("SELECT", "WITH")):
-                        _smoothie = blend(
-                            query=unpack_value,
-                            db=db,
-                            blender=blender,
-                            ingredients=ingredients,
-                            blender_args=blender_args,
-                            infer_gen_constraints=infer_gen_constraints,
-                            silence_db_exec_errors=silence_db_exec_errors,
-                            table_to_title=table_to_title,
-                            verbose=verbose,
-                            _prev_passed_values=_prev_passed_values,
-                            _prev_cleanup_tables=cleanup_tables,
-                        )
-                        _prev_passed_values = _smoothie.meta.num_values_passed
-                        subtable = _smoothie.df
-                        if unpack_kwarg == IngredientKwarg.OPTIONS:
-                            # Here, we need to format as a flat list
-                            kwargs_dict[unpack_kwarg] = list(subtable.values.flat)
-                        else:
-                            kwargs_dict[unpack_kwarg] = subtable
-                            # Below, we can remove the optional `context` arg we passed in args
-                            parsed_results_dict["args"] = parsed_results_dict["args"][
-                                :1
-                            ]
-
-                # Execute our ingredient function
-                function_out = ingredient(
-                    *parsed_results_dict["args"],
-                    **kwargs_dict
-                    | {
-                        "get_temp_subquery_table": _get_temp_subquery_table,
-                        "get_temp_session_table": _get_temp_session_table,
-                        "aliases_to_tablenames": scm.alias_to_tablename,
-                        "prev_subquery_map_columns": prev_subquery_map_columns,
-                    },
-                )
-                # Check how to handle output, depending on ingredient type
-                if ingredient.ingredient_type == IngredientType.MAP:
-                    # Parse so we replace this function in blendsql with 1st arg
-                    #   (new_col, which is the question we asked)
-                    #  But also update our underlying table, so we can execute correctly at the end
-                    (new_col, tablename, colname, new_table) = function_out
-                    prev_subquery_map_columns.add(new_col)
-                    non_null_subset = new_table[new_table[new_col].notnull()]
-                    # These are just for logging + debugging purposes
-                    example_map_outputs.append(
-                        tuple(zip(non_null_subset[colname], non_null_subset[new_col]))
+                    _smoothie = _blend(
+                        query=unpack_value,
+                        db=db,
+                        blender=blender,
+                        ingredients=ingredients,
+                        blender_args=blender_args,
+                        infer_gen_constraints=infer_gen_constraints,
+                        table_to_title=table_to_title,
+                        verbose=verbose,
+                        _prev_passed_values=_prev_passed_values,
                     )
-                    if tablename in tablename_to_map_out:
-                        tablename_to_map_out[tablename].append(new_table)
+                    _prev_passed_values = _smoothie.meta.num_values_passed
+                    subtable = _smoothie.df
+                    if unpack_kwarg == IngredientKwarg.OPTIONS:
+                        # Here, we need to format as a flat list
+                        kwargs_dict[unpack_kwarg] = list(subtable.values.flat)
                     else:
-                        tablename_to_map_out[tablename] = [new_table]
-                    session_modified_tables.add(tablename)
-                    function_call_to_res[
-                        alias_function_str
-                    ] = f'"{double_quote_escape(tablename)}"."{double_quote_escape(new_col)}"'
-                elif ingredient.ingredient_type in (
-                    IngredientType.STRING,
-                    IngredientType.QA,
-                ):
-                    # Here, we can simply insert the function's output
-                    function_call_to_res[alias_function_str] = function_out
-                elif ingredient.ingredient_type == IngredientType.JOIN:
-                    # 1) Get the `JOIN` clause containing function
-                    # 2) Replace with just the function alias
-                    # 3) Assign `function_out` to `alias_function_str`
-                    (
-                        left_tablename,
-                        right_tablename,
-                        join_clause,
-                        temp_join_tablename,
-                    ) = function_out
-                    cleanup_tables.add(temp_join_tablename)
-                    # Special case for when we have more than 1 ingredient in `JOIN` node left at this point
-                    num_ingredients_in_join = (
-                        len(list(_query.find(exp.Join).find_all(exp.Struct))) // 2
+                        kwargs_dict[unpack_kwarg] = subtable
+                        # Below, we can remove the optional `context` arg we passed in args
+                        parsed_results_dict["args"] = parsed_results_dict["args"][:1]
+
+            # Execute our ingredient function
+            function_out = ingredient(
+                *parsed_results_dict["args"],
+                **kwargs_dict
+                | {
+                    "get_temp_subquery_table": _get_temp_subquery_table,
+                    "get_temp_session_table": _get_temp_session_table,
+                    "aliases_to_tablenames": scm.alias_to_tablename,
+                    "prev_subquery_map_columns": prev_subquery_map_columns,
+                },
+            )
+            # Check how to handle output, depending on ingredient type
+            if ingredient.ingredient_type == IngredientType.MAP:
+                # Parse so we replace this function in blendsql with 1st arg
+                #   (new_col, which is the question we asked)
+                #  But also update our underlying table, so we can execute correctly at the end
+                (new_col, tablename, colname, new_table) = function_out
+                prev_subquery_map_columns.add(new_col)
+                new_table[new_table[new_col].notnull()]
+                if tablename in tablename_to_map_out:
+                    tablename_to_map_out[tablename].append(new_table)
+                else:
+                    tablename_to_map_out[tablename] = [new_table]
+                session_modified_tables.add(tablename)
+                function_call_to_res[
+                    alias_function_str
+                ] = f'"{double_quote_escape(tablename)}"."{double_quote_escape(new_col)}"'
+            elif ingredient.ingredient_type in (
+                IngredientType.STRING,
+                IngredientType.QA,
+            ):
+                # Here, we can simply insert the function's output
+                function_call_to_res[alias_function_str] = function_out
+            elif ingredient.ingredient_type == IngredientType.JOIN:
+                # 1) Get the `JOIN` clause containing function
+                # 2) Replace with just the function alias
+                # 3) Assign `function_out` to `alias_function_str`
+                (
+                    left_tablename,
+                    right_tablename,
+                    join_clause,
+                    temp_join_tablename,
+                ) = function_out
+                # Special case for when we have more than 1 ingredient in `JOIN` node left at this point
+                num_ingredients_in_join = (
+                    len(list(_query.find(exp.Join).find_all(exp.Struct))) // 2
+                )
+                if num_ingredients_in_join > 1:
+                    # Case where we have
+                    # `SELECT * FROM w0 JOIN w0 ON {{B()}} > 1 AND {{A()}} WHERE TRUE`
+                    # Since we haven't executed and saved `{{B()}}` to temp table yet,
+                    #   we need to keep. So we get:
+                    temp_uuid = str(uuid.uuid4())
+                    _query = _query.transform(
+                        replace_join_with_ingredient_multiple_ingredient,
+                        ingredient_name=parsed_results_dict["ingredient_aliasname"],
+                        ingredient_alias=alias_function_str,
+                        temp_uuid=temp_uuid,
+                    ).transform(prune_true_where)
+                    query = recover_blendsql(_query.sql(dialect=FTS5SQLite)).replace(
+                        f'SELECT "{temp_uuid}", ', ""
                     )
-                    if num_ingredients_in_join > 1:
-                        # Case where we have
-                        # `SELECT * FROM w0 JOIN w0 ON {{B()}} > 1 AND {{A()}} WHERE TRUE`
-                        # Since we haven't executed and saved `{{B()}}` to temp table yet,
-                        #   we need to keep. So we get:
-                        temp_uuid = str(uuid.uuid4())
-                        _query = _query.transform(
-                            replace_join_with_ingredient_multiple_ingredient,
-                            ingredient_name=parsed_results_dict["ingredient_aliasname"],
-                            ingredient_alias=alias_function_str,
-                            temp_uuid=temp_uuid,
-                        ).transform(prune_true_where)
-                        query = recover_blendsql(
-                            _query.sql(dialect=FTS5SQLite)
-                        ).replace(f'SELECT "{temp_uuid}", ', "")
-                    else:
-                        # Case where we have
-                        # `SELECT * FROM w0 JOIN w0 ON w0.x > 1 AND {{A()}} WHERE TRUE`
-                        # Since we've already applied SQL operation `w0.x > 1` and set to temp table
-                        # we can remove this. So below we transform to:
-                        # `SELECT * FROM w0 {{A()}}  WHERE TRUE`
-                        # This way, `{{A()}}` can get replaced with our new join
-                        # TODO: since we're not removing predicates in other areas, probably not best to do it here.
-                        #   Should probably modify in the future.
-                        _query = _query.transform(
-                            replace_join_with_ingredient_single_ingredient,
-                            ingredient_name=parsed_results_dict["ingredient_aliasname"],
-                            ingredient_alias=alias_function_str,
-                        )
-                        query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
-                    function_call_to_res[alias_function_str] = join_clause
                 else:
-                    raise ValueError(
-                        f"Not sure what to do with ingredient_type '{ingredient.ingredient_type}' yet\n(Also, we should have never hit this error....)"
+                    # Case where we have
+                    # `SELECT * FROM w0 JOIN w0 ON w0.x > 1 AND {{A()}} WHERE TRUE`
+                    # Since we've already applied SQL operation `w0.x > 1` and set to temp table
+                    # we can remove this. So below we transform to:
+                    # `SELECT * FROM w0 {{A()}}  WHERE TRUE`
+                    # This way, `{{A()}}` can get replaced with our new join
+                    # TODO: since we're not removing predicates in other areas, probably not best to do it here.
+                    #   Should probably modify in the future.
+                    _query = _query.transform(
+                        replace_join_with_ingredient_single_ingredient,
+                        ingredient_name=parsed_results_dict["ingredient_aliasname"],
+                        ingredient_alias=alias_function_str,
                     )
-                if naive_execution:
-                    break
-            # Combine all the retrieved ingredient outputs
-            for tablename, llm_outs in tablename_to_map_out.items():
-                if len(llm_outs) > 0:
-                    # Once we finish parsing this subquery, write to our session_uuid table
-                    # Below, we differ from Binder, which seems to replace the old table
-                    # On their left join merge command: https://github.com/HKUNLP/Binder/blob/9eede69186ef3f621d2a50572e1696bc418c0e77/nsql/database.py#L196
-                    # We create a new temp table to avoid a potentially self-destructive operation
-                    base_tablename = tablename
-                    _base_table: pd.DataFrame = db.execute_query(
-                        f"SELECT * FROM '{single_quote_escape(base_tablename)}'"
+                    query = recover_blendsql(_query.sql(dialect=FTS5SQLite))
+                function_call_to_res[alias_function_str] = join_clause
+            else:
+                raise ValueError(
+                    f"Not sure what to do with ingredient_type '{ingredient.ingredient_type}' yet\n(Also, we should have never hit this error....)"
+                )
+            if naive_execution:
+                break
+        # Combine all the retrieved ingredient outputs
+        for tablename, llm_outs in tablename_to_map_out.items():
+            if len(llm_outs) > 0:
+                # Once we finish parsing this subquery, write to our session_uuid table
+                # Below, we differ from Binder, which seems to replace the old table
+                # On their left join merge command: https://github.com/HKUNLP/Binder/blob/9eede69186ef3f621d2a50572e1696bc418c0e77/nsql/database.py#L196
+                # We create a new temp table to avoid a potentially self-destructive operation
+                base_tablename = tablename
+                _base_table: pd.DataFrame = db.execute_query(
+                    f'SELECT * FROM "{double_quote_escape(base_tablename)}";'
+                )
+                base_table = _base_table
+                if db.has_temp_table(_get_temp_session_table(tablename)):
+                    base_tablename = _get_temp_session_table(tablename)
+                    base_table: pd.DataFrame = db.execute_query(
+                        f"SELECT * FROM '{single_quote_escape(base_tablename)}';",
                     )
-                    base_table = _base_table
-                    if db.has_table(_get_temp_session_table(tablename)):
-                        base_tablename = _get_temp_session_table(tablename)
-                        base_table: pd.DataFrame = db.execute_query(
-                            f"SELECT * FROM '{single_quote_escape(base_tablename)}'"
+                previously_added_columns = base_table.columns.difference(
+                    _base_table.columns
+                )
+                assert len(set([len(x) for x in llm_outs])) == 1
+                llm_out_df = pd.concat(llm_outs, axis=1)
+                llm_out_df = llm_out_df.loc[:, ~llm_out_df.columns.duplicated()]
+                # Handle duplicate columns, e.g. in test_nested_duplicate_ingredient_calls()
+                for column in previously_added_columns:
+                    if all(
+                        column in x for x in [llm_out_df.columns, base_table.columns]
+                    ):
+                        # Fill nan in llm_out_df with those values in base_table
+                        pd.testing.assert_index_equal(
+                            base_table.index, llm_out_df.index
                         )
-                    previously_added_columns = base_table.columns.difference(
-                        _base_table.columns
-                    )
-                    assert len(set([len(x) for x in llm_outs])) == 1
-                    llm_out_df = pd.concat(llm_outs, axis=1)
-                    llm_out_df = llm_out_df.loc[:, ~llm_out_df.columns.duplicated()]
-                    # Handle duplicate columns, e.g. in test_nested_duplicate_ingredient_calls()
-                    for column in previously_added_columns:
-                        if all(
-                            column in x
-                            for x in [llm_out_df.columns, base_table.columns]
-                        ):
-                            # Fill nan in llm_out_df with those values in base_table
-                            pd.testing.assert_index_equal(
-                                base_table.index, llm_out_df.index
-                            )
-                            llm_out_df[column] = llm_out_df[column].fillna(
-                                base_table[column]
-                            )
-                            base_table = base_table.drop(columns=column)
-                    llm_out_df = llm_out_df[
-                        llm_out_df.columns.difference(base_table.columns)
-                    ]
-                    pd.testing.assert_index_equal(base_table.index, llm_out_df.index)
-                    merged = base_table.merge(
-                        llm_out_df, how="left", right_index=True, left_index=True
-                    )
-                    merged.to_sql(
-                        name=_get_temp_session_table(tablename),
-                        con=db.con,
-                        if_exists="replace",
-                        index=False,
-                    )
-                    cleanup_tables.add(_get_temp_session_table(tablename))
-                    session_modified_tables.add(tablename)
+                        llm_out_df[column] = llm_out_df[column].fillna(
+                            base_table[column]
+                        )
+                        base_table = base_table.drop(columns=column)
+                llm_out_df = llm_out_df[
+                    llm_out_df.columns.difference(base_table.columns)
+                ]
+                pd.testing.assert_index_equal(base_table.index, llm_out_df.index)
+                merged = base_table.merge(
+                    llm_out_df, how="left", right_index=True, left_index=True
+                )
+                db.to_temp_table(
+                    df=merged, tablename=_get_temp_session_table(tablename)
+                )
+                session_modified_tables.add(tablename)
 
-        # Now insert the function outputs to the original query
-        for function_str, res in function_call_to_res.items():
-            query = query.replace(function_str, str(res))
-        for t in session_modified_tables:
+    # Now insert the function outputs to the original query
+    for function_str, res in function_call_to_res.items():
+        query = query.replace(function_str, str(res))
+    for t in session_modified_tables:
+        query = sub_tablename(
+            t, f'"{double_quote_escape(_get_temp_session_table(t))}"', query
+        )
+    for a, t in scm.alias_to_tablename.items():
+        if t in session_modified_tables:
             query = sub_tablename(
-                t, f'"{double_quote_escape(_get_temp_session_table(t))}"', query
+                a, f'"{double_quote_escape(_get_temp_session_table(t))}"', query
             )
-        for a, t in scm.alias_to_tablename.items():
-            if t in session_modified_tables:
-                query = sub_tablename(
-                    a, f'"{double_quote_escape(_get_temp_session_table(t))}"', query
-                )
 
-        logging.debug("")
-        logging.debug(
-            "**********************************************************************************"
-        )
-        logging.debug(Fore.LIGHTGREEN_EX + f"Final Query:\n{query}" + Fore.RESET)
-        logging.debug(
-            "**********************************************************************************"
-        )
-        logging.debug("")
+    logging.debug("")
+    logging.debug(
+        "**********************************************************************************"
+    )
+    logging.debug(Fore.LIGHTGREEN_EX + f"Final Query:\n{query}" + Fore.RESET)
+    logging.debug(
+        "**********************************************************************************"
+    )
+    logging.debug("")
 
-        df = db.execute_query(query, silence_errors=silence_db_exec_errors)
+    df = db.execute_query(query)
 
-        return Smoothie(
-            df=df,
-            meta=SmoothieMeta(
-                process_time_seconds=time.time() - start,
-                num_values_passed=sum(
-                    [
-                        i.num_values_passed
-                        for i in kitchen
-                        if hasattr(i, "num_values_passed")
-                    ]
-                )
-                + _prev_passed_values,
-                num_prompt_tokens=blender.num_prompt_tokens
-                if blender is not None
-                else 0,
-                prompts=blender.prompts if blender is not None else [],
-                example_map_outputs=example_map_outputs,
-                ingredients=ingredients,
-                query=original_query,
-                db_path=db.db_path,
-            ),
-        )
+    return Smoothie(
+        df=df,
+        meta=SmoothieMeta(
+            process_time_seconds=time.time() - start,
+            num_values_passed=sum(
+                [
+                    i.num_values_passed
+                    for i in kitchen
+                    if hasattr(i, "num_values_passed")
+                ]
+            )
+            + _prev_passed_values,
+            num_prompt_tokens=blender.num_prompt_tokens if blender is not None else 0,
+            prompts=blender.prompts if blender is not None else [],
+            ingredients=ingredients,
+            query=original_query,
+            db_path=db.db_path,
+        ),
+    )
+
+
+def blend(
+    query: str,
+    db: Database,
+    blender: Optional[Model] = None,
+    ingredients: Optional[Collection[Ingredient]] = None,
+    verbose: bool = False,
+    blender_args: Optional[Dict[str, str]] = None,
+    infer_gen_constraints: bool = True,
+    table_to_title: Optional[Dict[str, str]] = None,
+    schema_qualify: bool = True,
+) -> Smoothie:
+    """The `blend()` function is used to execute a BlendSQL query against a database and
+    return the final result, in addition to the intermediate reasoning steps taken.
+    Execution is done on a database given an ingredient context.
 
+    Args:
+        query: The BlendSQL query to execute
+        db: Database connector object
+        ingredients: List of ingredient objects, to use in interpreting BlendSQL query
+        verbose: Boolean defining whether to run in logging.debug mode
+        blender: Optionally override whatever llm argument we pass to Model ingredient.
+            Useful for research applications, where we don't (necessarily) want the parser to choose endpoints.
+        infer_gen_constraints: Optionally infer the output format of an `IngredientMap` call, given the predicate context
+            For example, in `{{LLMMap('convert to date', 'w::listing date')}} <= '1960-12-31'`
+            We can infer the output format should look like '1960-12-31'
+                and put this in the `example_outputs` kwarg
+        table_to_title: Optional mapping from table name to title of table.
+            Useful for datasets like WikiTableQuestions, where relevant info is stored in table title.
+        schema_qualify: Optional bool, determines if we run qualify_columns() from sqlglot
+            This enables us to write BlendSQL scripts over multi-table databases without manually qualifying columns ourselves
+            However, we need to call db.get_sqlglot_schema() if schema_qualify=True, which may add some latency.
+            With single-table queries, we can set this to False.
+
+    Returns:
+        smoothie: `Smoothie` dataclass containing pd.DataFrame output and execution metadata
+    """
+    if verbose:
+        logging.getLogger().setLevel(logging.DEBUG)
+    else:
+        logging.getLogger().setLevel(logging.ERROR)
+    start = time.time()
+    try:
+        smoothie = _blend(
+            query=query,
+            db=db,
+            blender=blender,
+            ingredients=ingredients,
+            blender_args=blender_args,
+            infer_gen_constraints=infer_gen_constraints,
+            table_to_title=table_to_title,
+            schema_qualify=schema_qualify,
+        )
     except Exception as error:
         raise error
     finally:
-        # In the case of a recursive `blend()` call,
+        # In the case of a recursive `_blend()` call,
         #   this logic allows temp tables to persist until
         #   the final base case is fulfilled.
-        if _prev_cleanup_tables is None:
-            delete_session_tables(db=db, cleanup_tables=cleanup_tables)
+        db._reset_connection()
+    smoothie.meta.process_time_seconds = time.time() - start
+    return smoothie
```

### Comparing `blendsql-0.0.141/blendsql/db/sqlite.py` & `blendsql-0.0.15/research/utils/feverous/feverous.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,185 +1,173 @@
-import sqlite3
-from pathlib import Path
-from sqlite3 import OperationalError
-from typing import Generator, Tuple, Union, List, Dict
-from typing import Iterable
+# Set up logging
 import logging
-from functools import lru_cache
-import pandas as pd
-from attr import attrib, attrs
-from colorama import Fore
-
-from .utils import single_quote_escape, double_quote_escape
-
-
-@attrs(auto_detect=True)
-class SQLite:
-    """
-    Class used to connect to a SQLite database.
-
-    Args:
-        db_path: Path to the db
-    """
-
-    db_path: str = attrib()
-    con: sqlite3.Connection = attrib(init=False)
-
-    all_tables: List[str] = attrib(init=False)
-    tablename_to_columns: Dict[str, Iterable] = attrib(init=False)
-
-    def __attrs_post_init__(self):
-        if not Path(self.db_path).exists():
-            raise ValueError(f"{self.db_path} does not exist")
-        try:
-            self.con = sqlite3.connect(self.db_path)
-        except OperationalError:
-            print(self.db_path)
-            raise
-        self.all_tables = None
-        self.tablename_to_columns = {}
-
-    def has_table(self, tablename: str) -> bool:
-        if (
-            self.execute_query(
-                f"SELECT count(*) FROM sqlite_master WHERE type='table' AND name='{single_quote_escape(tablename)}';"
-            ).values.item()
-            > 0
-        ):
-            return True
-        return False
-
-    def iter_tables(
-        self, use_tables: Iterable[str] = None
-    ) -> Generator[str, None, None]:
-        for tablename in self._iter_tables():
-            if use_tables is not None and tablename not in use_tables:
-                continue
-            yield tablename
+import sys
+from typing import Tuple, List
+from pathlib import Path
+import sqlite3
+import re
 
-    def iter_columns(self, tablename: str) -> Generator[str, None, None]:
-        for columname in self._get_columns(tablename=tablename):
-            yield columname
-
-    def create_clauses(self) -> Generator[Tuple[str, str], None, None]:
-        for tablename in self._iter_tables():
-            create_clause = _create_clause(con=self.con, tablename=tablename)
-            yield (tablename, create_clause)
-
-    def create_clause(self, tablename):
-        return (tablename, _create_clause(con=self.con, tablename=tablename))
-
-    def get_sqlglot_schema(self) -> dict:
-        """Returns database schema as a dictionary, in the format that
-        sqlglot.optimizer expects.
-
-        Examples:
-            >>> db.get_sqlglot_schema()
-            {"x": {"A": "INT", "B": "INT", "C": "INT", "D": "INT", "Z": "STRING"}}
-        """
-        schema = {}
-        for tablename in self._iter_tables():
-            schema[tablename] = {}
-            for _, row in self.execute_query(
-                f"""
-            SELECT name, type FROM pragma_table_info('{tablename}')
-            """
-            ).iterrows():
-                schema[tablename]['"' + row["name"] + '"'] = row["type"]
-        return schema
-
-    def to_serialized(
-        self,
-        ignore_tables: Iterable[str] = None,
-        num_rows: int = 0,
-        table_description: str = None,
-    ) -> str:
-        """Generates a string representation of a database, via `CREATE` statements.
-        This can then be passed to a LLM as context.
-
-        Args:
-            ignore_tables: Name of tables to ignore in serialization. Default is just 'documents'.
-            num_rows: How many rows per table to include in serialization
-            table_description: Optional table description to add at top
-        """
-        if ignore_tables is None:
-            ignore_tables = {"documents"}
-        serialized_db = (
-            []
-            if table_description is None
-            else [f"Table Description: {table_description}\n"]
-        )
-        for tablename, create_clause in self.create_clauses():
-            if tablename in ignore_tables:
+logging.basicConfig(
+    format="%(asctime)s - %(levelname)s - %(name)s -   %(message)s",
+    datefmt="%m/%d/%Y %H:%M:%S",
+    handlers=[logging.StreamHandler(sys.stdout)],
+    level=logging.INFO,
+)
+logger = logging.getLogger(__name__)
+
+from ..database import to_serialized
+from ..dataset import DataTrainingArguments
+from ...utils.args import ModelArguments
+from ...utils.bridge_content_encoder import (
+    get_database_matches,
+)
+from ...constants import (
+    SINGLE_TABLE_NAME,
+    CREATE_VIRTUAL_TABLE_CMD,
+    DOCS_TABLE_NAME,
+    EvalField,
+)
+from ..normalizer import prepare_df_for_neuraldb_from_table
+from blendsql.db import SQLite
+
+
+def feverous_metric_format_func(item: dict) -> dict:
+    prediction = item[EvalField.PREDICTION]
+    if prediction is not None:
+        if len(prediction) < 1:
+            pred = ""
+        else:
+            pred = prediction[0]
+    else:
+        pred = ""
+    # Map `True` to 'SUPPORTS', `False` to 'REFUTES'
+    pred = "SUPPORTS" if pred else "REFUTES"
+    return {
+        "prediction": str(pred),
+        "reference": {"seq_out": item[EvalField.GOLD_ANSWER]},
+    }
+
+
+def feverous_get_input(
+    statement: str,
+    table: dict,
+    context: List[str],
+    uid: str,
+    data_training_args: DataTrainingArguments,
+    model_args: ModelArguments,
+) -> Tuple[str, dict]:
+    # Below uid is unique for each datapoint
+    # But, might be better to consider table_id instead
+    db_path = Path(data_training_args.db_path) / "feverous" / f"{uid}.db"
+    tablename_to_description = {}
+    contains_documents = not all(len(x) == 0 for x in context.values())
+    if not db_path.is_file():
+        # Create db
+        if not db_path.parent.is_dir():
+            db_path.parent.mkdir(parents=True)
+        sqlite_conn = sqlite3.connect(db_path)
+        for idx, (table_description, header, rows) in enumerate(
+            zip(table["table_description"], table["header"], table["rows"])
+        ):
+            tablename = f"{SINGLE_TABLE_NAME}{idx}"
+            prepare_df_for_neuraldb_from_table(
+                {"header": header, "rows": rows}, add_row_id=False
+            ).to_sql(tablename, sqlite_conn)
+            tablename_to_description[tablename] = table_description
+        if contains_documents:
+            # Create virtual table to search over
+            c = sqlite_conn.cursor()
+            c.execute(CREATE_VIRTUAL_TABLE_CMD)
+            c.close()
+            # Add content
+            prepare_df_for_neuraldb_from_table(
+                {
+                    "header": ["title", "content"],
+                    "rows": [
+                        [title, content]
+                        for title, content in set(
+                            tuple(zip(context["title"], context["content"]))
+                        )
+                    ],
+                },
+                add_row_id=False,
+            ).to_sql(DOCS_TABLE_NAME, sqlite_conn, if_exists="append", index=False)
+            sqlite_conn.close()
+    db_path = str(db_path)
+    db = SQLite(db_path)
+    serialized_db = to_serialized(
+        db=db,
+        num_rows=data_training_args.num_serialized_rows,
+        tablename_to_description=tablename_to_description,
+    )
+    entire_serialized_db = to_serialized(
+        db=db,
+        num_rows=data_training_args.num_serialized_rows,
+        tablename_to_description=tablename_to_description,
+        whole_table=True,
+        truncate_content=300,
+    )
+    bridge_hints = None
+    if data_training_args.use_bridge_encoder:
+        bridge_hints = []
+        column_str_with_values = "{table}.{column} ( {values} )"
+        value_sep = " , "
+        for table_name in db.iter_tables():
+            if re.search(r"^{}_".format(DOCS_TABLE_NAME), table_name):
                 continue
-            serialized_db.append(create_clause)
-            serialized_db.append("\n")
-            if num_rows > 0:
-                get_rows_query = (
-                    f'SELECT * FROM "{double_quote_escape(tablename)}" LIMIT {num_rows}'
+            for column_name in db.iter_columns(table_name):
+                matches = get_database_matches(
+                    question=statement,
+                    table_name=table_name,
+                    column_name=column_name,
+                    db_path=db_path,
                 )
-                serialized_db.append("\n/*")
-                serialized_db.append(f"\n{num_rows} example rows:")
-                serialized_db.append(f"\n{get_rows_query}")
-            else:
-                continue
-            rows = self.execute_query(get_rows_query)
-            # Truncate long strings
-            rows = rows.apply(
-                lambda x: f"{str(x)[:50]}..."
-                if isinstance(x, str) and len(str(x)) > 50
-                else x,
-                axis=1,
+                if matches:
+                    bridge_hints.append(
+                        column_str_with_values.format(
+                            table=table_name,
+                            column=column_name,
+                            values=value_sep.join(matches),
+                        )
+                    )
+        bridge_hints = "\n".join(bridge_hints)
+    db.con.close()
+    return (
+        db_path,
+        {
+            "few_shot_prompt": open("./research/prompts/feverous/few_shot.txt").read(),
+            "ingredients_prompt": open(
+                "./research/prompts/feverous/ingredients.txt"
+            ).read(),
+            "question": statement,
+            "serialized_db": serialized_db,
+            "entire_serialized_db": entire_serialized_db,
+            "bridge_hints": bridge_hints,
+            "extra_task_description": f"Additionally, we have the table `{DOCS_TABLE_NAME}` at our disposal, which contains Wikipedia articles providing more details about the values in our table."
+            if contains_documents
+            else "",
+        },
+    )
+
+
+def feverous_pre_process_function(
+    batch: dict, data_training_args: DataTrainingArguments, model_args: ModelArguments
+) -> dict:
+    db_path, input_program_args = zip(
+        *[
+            feverous_get_input(
+                statement=statement,
+                table=table,
+                context=context,
+                uid=uid,
+                data_training_args=data_training_args,
+                model_args=model_args,
+            )
+            for statement, table, context, uid in zip(
+                batch[EvalField.QUESTION],
+                batch["table"],
+                batch["context"],
+                batch[EvalField.UID],
             )
-            serialized_db.append(f"\n{rows.to_string(index=False)}")
-            serialized_db.append("\n*/")
-        serialized_db = "\n\n".join(serialized_db).strip()
-        return serialized_db
-
-    # @profile
-    def execute_query(
-        self, query: str, return_error: bool = False, silence_errors: bool = True
-    ) -> Union[pd.DataFrame, Tuple[pd.DataFrame, str]]:
-        """
-        Execute the given query.
-        """
-        try:
-            df = pd.read_sql(query, self.con)
-            if return_error:
-                return (df, None)
-            return df
-        except Exception as e:
-            if silence_errors:
-                print(Fore.RED + "Something went wrong!" + Fore.RESET)
-                print(e)
-                if return_error:
-                    return (pd.DataFrame(), str(e))
-                return pd.DataFrame()  # Return empty pd.DataFrame
-            raise (e)
-
-    def _iter_tables(self):
-        if self.all_tables is None:
-            self.all_tables = pd.read_sql(
-                "SELECT tbl_name FROM sqlite_master WHERE type='table'", self.con
-            )["tbl_name"]
-        return self.all_tables
-
-    def _get_columns(self, tablename: str):
-        if tablename not in self.tablename_to_columns:
-            self.tablename_to_columns[tablename] = pd.read_sql(
-                f'PRAGMA table_info("{double_quote_escape(tablename)}");', self.con
-            )["name"]
-        return self.tablename_to_columns[tablename]
-
-
-@lru_cache(maxsize=1000, typed=False)
-def _create_clause(con, tablename) -> str:
-    create_clause = pd.read_sql(
-        f'SELECT sql FROM sqlite_master WHERE tbl_name = "{double_quote_escape(tablename)}"',
-        con,
+        ]
     )
-    if create_clause.size < 1:
-        logging.debug(
-            f"Expected create_clause size to be 1, got {create_clause.size}\n{create_clause}"
-        )
-        return ""
-    return create_clause.values[0][0]
+    return {"input_program_args": list(input_program_args), "db_path": list(db_path)}
```

### Comparing `blendsql-0.0.141/blendsql/ingredients/builtin/llm/join/main.py` & `blendsql-0.0.15/blendsql/ingredients/builtin/join/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Optional
 from guidance import gen
 from textwrap import dedent
 
 from blendsql.models._model import Model
 from blendsql._program import Program
 from blendsql import _constants as CONST
 from blendsql.ingredients.ingredient import JoinIngredient
@@ -13,96 +13,104 @@
         self,
         join_criteria: str,
         left_values: List[str],
         right_values: List[str],
         sep: str,
         **kwargs,
     ):
+        _model = self.model
         left_values = "\n".join(left_values)
         right_values = "\n".join(right_values)
         with self.systemcontext:
-            self.model += "You are a database expert in charge of performing a modified `LEFT JOIN` operation. This `LEFT JOIN` is based on a semantic criteria given by the user."
-            self.model += f"\nThe left and right value alignment should be separated by '{sep}', with each new `JOIN` alignment goin on a newline. If a given left value has no corresponding right value, give '-' as a response."
+            _model += "You are a database expert in charge of performing a modified `LEFT JOIN` operation. This `LEFT JOIN` is based on a semantic criteria given by the user."
+            _model += f"\nThe left and right value alignment should be separated by '{sep}', with each new `JOIN` alignment goin on a newline. If a given left value has no corresponding right value, give '-' as a response."
         with self.usercontext:
             if self.few_shot:
-                self.model += dedent(
+                _model += dedent(
                     """
                 Criteria: Join to same topics.
 
-                Left Values: 
+                Left Values:
                 joshua fields
                 bob brown
                 ron ryan
 
-                Right Values: 
+                Right Values:
                 ron ryan
                 colby mules
                 bob brown (ice hockey)
                 josh fields (pitcher)
 
-                Output: 
+                Output:
                 joshua fields;josh fields (pitcher)
                 bob brown;bob brown (ice hockey)
                 ron ryan;ron ryan
 
-                --- 
+                ---
 
                 Criteria: Align the fruit to their corresponding colors.
 
-                Left Values: 
+                Left Values:
                 apple
                 banana
                 blueberry
                 orange
 
-                Right Values: 
+                Right Values:
                 blue
                 yellow
                 red
 
-                Output: 
+                Output:
                 apple;red
                 banana;yellow
                 blueberry;blue
                 orange;-
 
                 ---
                 """
                 )
-            self.model += dedent(
+            _model += dedent(
                 f"""
                 Criteria: {join_criteria}
 
-                Left Values: {left_values}
+                Left Values:
+                {left_values}
 
-                Right Values: {right_values}
+                Right Values:
+                {right_values}
 
                 Output:
                 """
             )
         with self.assistantcontext:
-            self.model += gen(name="result", **self.gen_kwargs)
-        return self.model
+            _model += gen(name="result", **self.gen_kwargs)
+        return _model
 
 
 class LLMJoin(JoinIngredient):
+    DESCRIPTION = """
+    If we need to do a `join` operation where there is imperfect alignment between table values, use the new function:
+        `{{LLMJoin(left_on='table::column', right_on='table::column')}}`
+    """
+
     def run(
         self,
         left_values: List[str],
         right_values: List[str],
         model: Model,
-        join_criteria: str = "Join to same topics.",
+        question: Optional[str] = "Join to same topics.",
         **kwargs,
     ) -> dict:
         res = model.predict(
             program=JoinProgram,
             sep=CONST.DEFAULT_ANS_SEP,
             left_values=left_values,
             right_values=right_values,
-            join_criteria=join_criteria,
+            join_criteria=question,
             **kwargs,
         )
 
         _result = res["result"].split("\n")
         result: dict = {}
         for item in _result:
             if CONST.DEFAULT_ANS_SEP in item:
```

### Comparing `blendsql-0.0.141/blendsql/ingredients/builtin/llm/map/main.py` & `blendsql-0.0.15/blendsql/ingredients/builtin/map/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,45 +24,46 @@
         include_tf_disclaimer: bool = False,
         output_type: str = None,
         example_outputs: str = None,
         table_title: str = None,
         colname: str = None,
         **kwargs,
     ):
+        _model = self.model
         with self.systemcontext:
-            self.model += """Given a set of values from a database, answer the question row-by-row, in order."""
+            _model += """Given a set of values from a database, answer the question row-by-row, in order."""
             if include_tf_disclaimer:
-                self.model += " If the question can be answered with 'true' or 'false', select `t` for 'true' or `f` for 'false'."
-            self.model += dedent(
+                _model += " If the question can be answered with 'true' or 'false', select `t` for 'true' or `f` for 'false'."
+            _model += dedent(
                 f"""
             The answer should be a list separated by '{sep}', and have {len(values)} items in total.
             When you have given all {len(values)} answers, stop responding.
             If a given value has no appropriate answer, give '-' as a response.
             """
             )
         with self.usercontext:
             if self.few_shot:
-                self.model += dedent(
+                _model += dedent(
                     """
-                --- 
+                ---
 
                 The following values come from the column 'Home Town', in a table titled '2010\u201311 North Carolina Tar Heels men's basketball team'.
                 Q: What state is this?
                 Values:
                 `Ames, IA`
                 `Carrboro, NC`
                 `Kinston, NC`
                 `Encino, CA`
 
                 Output type: string
                 Here are some example outputs: `MA;CA;-;`
 
                 A: IA;NC;NC;CA
 
-                --- 
+                ---
 
                 The following values come from the column 'Penalties (P+P+S+S)', in a table titled 'Biathlon World Championships 2013 \u2013 Men's pursuit'.
                 Q: Total penalty count?
                 Values:
                 `1 (0+0+0+1)`
                 `10 (5+3+2+0)`
                 `6 (2+2+2+0)`
@@ -98,31 +99,36 @@
                 Output type: boolean
                 A: f;f;t;t
 
                 ---
                 """
                 )
             if table_title:
-                self.model += dedent(
+                _model += dedent(
                     f"The following values come from the column '{colname}', in a table titled '{table_title}'."
                 )
-            self.model += dedent(f"""Q: {question}\nValues:\n""")
+            _model += dedent(f"""Q: {question}\nValues:\n""")
             for value in values:
-                self.model += f"`{value}`\n"
+                _model += f"`{value}`\n"
             if output_type:
-                self.model += f"\nOutput type: {output_type}"
+                _model += f"\nOutput type: {output_type}"
             if example_outputs:
-                self.model += f"\nHere are some example outputs: {example_outputs}\n"
-            self.model += "\nA:"
+                _model += f"\nHere are some example outputs: {example_outputs}\n"
+            _model += "\nA:"
         with self.assistantcontext:
-            self.model += gen(name="result", **self.gen_kwargs)
-        return self.model
+            _model += gen(name="result", **self.gen_kwargs)
+        return _model
 
 
 class LLMMap(MapIngredient):
+    DESCRIPTION = """
+    If question-relevant column(s) contents are not suitable for SQL comparisons or calculations, map it to a new column using the scalar function:
+        `{{LLMMap('question', 'table::column')}}`
+    """
+
     def run(
         self,
         question: str,
         model: Model,
         values: List[str],
         value_limit: Union[int, None] = None,
         example_outputs: Optional[str] = None,
```

### Comparing `blendsql-0.0.141/blendsql/ingredients/builtin/llm/validate/main.py` & `blendsql-0.0.15/blendsql/ingredients/builtin/validate/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,25 +4,33 @@
 
 from blendsql.models._model import Model
 from blendsql._program import Program
 from blendsql.ingredients.ingredient import QAIngredient
 
 
 class ValidateProgram(Program):
-    def __call__(self, question: str, serialized_db: str, table_title: str = None):
+    def __call__(
+        self,
+        question: str,
+        context: pd.DataFrame = None,
+        table_title: str = None,
+        **kwargs,
+    ):
+        serialized_db = context.to_string() if context is not None else ""
+        _model = self.model
         with self.systemcontext:
-            self.model += "You are a database expert in charge of validating a claim given a context. Given a claim and associated database context, you will respond 'true' if the claim is factual given the context, and 'false' if not."
+            _model += "You are a database expert in charge of validating a claim given a context. Given a claim and associated database context, you will respond 'true' if the claim is factual given the context, and 'false' if not."
         with self.usercontext:
-            self.model += f"Claim: {question}"
+            _model += f"Claim: {question}"
             if table_title:
-                self.model += f"\nTable Description: {table_title}"
-            self.model += f"\n{serialized_db}\n\nAnswer:"
+                _model += f"\nTable Description: {table_title}"
+            _model += f"\n{serialized_db}\n\nAnswer:"
         with self.assistantcontext:
-            self.model += select(options=["true", "false"], name="result")
-        return self.model
+            _model += select(options=["true", "false"], name="result")
+        return _model
 
 
 class LLMValidate(QAIngredient):
     def run(
         self,
         question: str,
         model: Model,
@@ -33,14 +41,13 @@
         **kwargs,
     ) -> Union[str, int, float]:
         if context is not None:
             if value_limit is not None:
                 context = context.iloc[:value_limit]
         res = model.predict(
             program=ValidateProgram,
-            claim=question,
-            serialized_db=context.to_string() if context is not None else "",
-            long_answer=long_answer,
+            question=question,
+            context=context,
             table_title=None,
             **kwargs,
         )
         return int(res["result"] == "true")
```

### Comparing `blendsql-0.0.141/blendsql/ingredients/ingredient.py` & `blendsql-0.0.15/blendsql/ingredients/ingredient.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 from attr import attrs, attrib
 from abc import abstractmethod, ABC
 import pandas as pd
-from typing import Any, Iterable, Union, Dict, Tuple, Type, Callable, Set
+from typing import (
+    Any,
+    Iterable,
+    Union,
+    Dict,
+    Tuple,
+    Type,
+    Callable,
+    Set,
+    Collection,
+    Optional,
+)
 import uuid
 from typeguard import check_type
 
 from .. import utils
 from .._constants import IngredientKwarg, IngredientType
-from ..db.sqlite import SQLite
+from ..db import Database
+from ..db.utils import double_quote_escape
 
 
 class IngredientException(ValueError):
     pass
 
 
 def unpack_default_kwargs(**kwargs):
     return (
         kwargs.get("tablename"),
         kwargs.get("colname"),
     )
 
 
-def align_to_real_columns(db: SQLite, colname: str, tablename: str) -> str:
+def align_to_real_columns(db: Database, colname: str, tablename: str) -> str:
     table_columns = db.execute_query(f'SELECT * FROM "{tablename}" LIMIT 1').columns
     if colname not in table_columns:
         # Try to align with column, according to some normalization rules
         cleaned_to_original = {
             col.replace("\\n", " ").replace("\xa0", " "): col for col in table_columns
         }
         colname = cleaned_to_original[colname]
@@ -34,15 +46,15 @@
 
 @attrs
 class Ingredient(ABC):
     name: str = attrib()
     ingredient_type: str = attrib(init=False)
     allowed_output_types: Tuple[Type] = attrib(init=False)
     # Below gets passed via `Kitchen.extend()`
-    db: SQLite = attrib(init=False)
+    db: Database = attrib(init=False)
     session_uuid: str = attrib(init=False)
 
     def __repr__(self):
         return f"{self.ingredient_type} {self.name}"
 
     def __str__(self):
         return f"{self.ingredient_type} {self.name}"
@@ -55,15 +67,15 @@
         return check_type(self.run(*args, **kwargs), self.allowed_output_types)
 
     def maybe_get_temp_table(
         self, temp_table_func: Callable, tablename: str
     ) -> Tuple[str, bool]:
         temp_tablename = temp_table_func(tablename)
         _tablename = tablename
-        if self.db.has_table(temp_tablename):
+        if self.db.has_temp_table(temp_tablename):
             # We've already applied some operation to this table
             # We want to use this as our base
             _tablename = temp_tablename
         return (_tablename, True) if _tablename != tablename else (_tablename, False)
 
 
 @attrs
@@ -74,17 +86,15 @@
     ingredient_type: str = IngredientType.MAP.value
     num_values_passed: int = 0
     allowed_output_types: Tuple[Type] = (Iterable[Any],)
 
     def unpack_default_kwargs(self, **kwargs):
         return unpack_default_kwargs(**kwargs)
 
-    def __call__(
-        self, question: str = None, context: str = None, *args, **kwargs
-    ) -> tuple:
+    def __call__(self, question: str, context: str, *args, **kwargs) -> tuple:
         """Returns tuple with format (arg, tablename, colname, new_table)"""
         # Unpack kwargs
         aliases_to_tablenames: Dict[str, str] = kwargs.get("aliases_to_tablenames")
         get_temp_subquery_table: Callable = kwargs.get("get_temp_subquery_table")
         get_temp_session_table: Callable = kwargs.get("get_temp_session_table")
         prev_subquery_map_columns: Set[str] = kwargs.get("prev_subquery_map_columns")
 
@@ -104,67 +114,68 @@
         new_arg_column = question
         while (
             new_arg_column in set(self.db.iter_columns(tablename))
             or new_arg_column in prev_subquery_map_columns
         ):
             new_arg_column = "_" + new_arg_column
 
-        original_table = self.db.execute_query(
-            f"SELECT * FROM '{tablename}'", silence_errors=False
-        )
+        original_table = self.db.execute_query(f'SELECT * FROM "{tablename}"')
 
         # Get a list of values to map
         # First, check if we've already dumped some `MapIngredient` output to the main session table
         if temp_session_table_exists:
             temp_session_table = self.db.execute_query(
-                f"SELECT * FROM '{temp_session_tablename}'"
+                f'SELECT * FROM "{double_quote_escape(temp_session_tablename)}"'
             )
             colname = align_to_real_columns(
                 db=self.db, colname=colname, tablename=temp_session_tablename
             )
             # We don't need to run this function on everything,
             #   if a previous subquery already got to certain values
             if new_arg_column in temp_session_table.columns:
                 values = self.db.execute_query(
                     f'SELECT DISTINCT "{colname}" FROM "{temp_session_tablename}" WHERE "{new_arg_column}" IS NULL',
-                    silence_errors=False,
                 )[colname].tolist()
             # Base case: this is the first time we've used this particular ingredient
             # BUT, temp_session_tablename still exists
             else:
                 values = self.db.execute_query(
-                    f'SELECT DISTINCT "{colname}" FROM "{temp_session_tablename}"',
-                    silence_errors=False,
+                    f'SELECT DISTINCT "{colname}" FROM "{temp_session_tablename}"'
                 )[colname].tolist()
         else:
             colname = align_to_real_columns(
                 db=self.db, colname=colname, tablename=value_source_tablename
             )
             values = self.db.execute_query(
-                f'SELECT DISTINCT "{colname}" FROM "{value_source_tablename}"',
-                silence_errors=False,
+                f'SELECT DISTINCT "{colname}" FROM "{value_source_tablename}"'
             )[colname].tolist()
 
         # No need to run ingredient if we have no values to map onto
         if len(values) == 0:
             original_table[new_arg_column] = None
             return (new_arg_column, tablename, colname, original_table)
 
-        kwargs["values"] = values
+        kwargs[IngredientKwarg.VALUES] = values
         kwargs["original_table"] = original_table
         kwargs[IngredientKwarg.QUESTION] = question
-        mapped_values: Iterable[Any] = self._run(*args, **kwargs)
+        mapped_values: Collection[Any] = self._run(*args, **kwargs)
         self.num_values_passed += len(mapped_values)
         df_as_dict = {colname: [], new_arg_column: []}
         for value, mapped_value in zip(values, mapped_values):
             df_as_dict[colname].append(value)
             df_as_dict[new_arg_column].append(mapped_value)
         subtable = pd.DataFrame(df_as_dict)
-        if all(isinstance(x, (int, type(None))) for x in mapped_values):
-            subtable[new_arg_column] = subtable[new_arg_column].astype("Int64")
+        if kwargs.get("output_type") == "boolean":
+            subtable[new_arg_column] = subtable[new_arg_column].astype(bool)
+        else:
+            if all(
+                isinstance(x, (int, type(None))) and not isinstance(x, bool)
+                for x in mapped_values
+            ):
+                subtable[new_arg_column] = subtable[new_arg_column].astype("Int64")
         # Add new_table to original table
         new_table = original_table.merge(subtable, how="left", on=colname)
         if new_table.shape[0] != original_table.shape[0]:
             raise IngredientException(
                 f"subtable from run() needs same length as # rows from original\nOriginal has {original_table.shape[0]}, new_table has {new_table.shape[0]}"
             )
         # Now, new table has original columns + column with the name of the question we answered
@@ -185,18 +196,17 @@
 
     ingredient_type: str = IngredientType.JOIN.value
     num_values_passed: int = 0
     allowed_output_types: Tuple[Type] = (dict,)
 
     def __call__(
         self,
-        question: str = None,
-        left_on: str = None,
-        right_on: str = None,
-        join_criteria: str = None,
+        question: Optional[str] = None,
+        left_on: Optional[str] = None,
+        right_on: Optional[str] = None,
         *args,
         **kwargs,
     ) -> tuple:
         # Unpack kwargs
         aliases_to_tablenames: Dict[str, str] = kwargs.get("aliases_to_tablenames")
         get_temp_subquery_table: Callable = kwargs.get("get_temp_subquery_table")
         get_temp_session_table: Callable = kwargs.get("get_temp_session_table")
@@ -212,22 +222,25 @@
             original_lr_identifiers.append((tablename, colname))
             tablename, _ = self.maybe_get_temp_table(
                 temp_table_func=get_temp_subquery_table,
                 tablename=tablename,
             )
             values.append(
                 set(
-                    self.db.execute_query(
-                        f'SELECT DISTINCT "{colname}" FROM "{tablename}"'
-                    )[colname].tolist()
+                    [
+                        str(i)
+                        for i in self.db.execute_query(
+                            f'SELECT DISTINCT "{colname}" FROM "{tablename}"'
+                        )[colname].tolist()
+                    ]
                 )
             )
             modified_lr_identifiers.append((tablename, colname))
 
-        if join_criteria is None:
+        if question is None:
             # First, check which values we actually need to call Model on
             # We don't want to join when there's already an intuitive alignment
             mapping = {}
             left_values, right_values = values
             for l in left_values:
                 if l in right_values:
                     # Define this mapping, and remove from Model inference call
@@ -256,22 +269,19 @@
             )
 
             kwargs[IngredientKwarg.QUESTION] = question
             _mapping: Dict[str, str] = self._run(*args, **kwargs)
             mapping = mapping | _mapping
 
         # Using mapped left/right values, create intermediary mapping table
-        # This needs a new unique id. We add to the session's `cleanup_tables` after returning.
         temp_join_tablename = get_temp_session_table(str(uuid.uuid4())[:4])
         joined_values_df = pd.DataFrame(
             data={"left": mapping.keys(), "right": mapping.values()}
         )
-        joined_values_df.to_sql(
-            name=temp_join_tablename, con=self.db.con, if_exists="fail", index=False
-        )
+        self.db.to_temp_table(df=joined_values_df, tablename=temp_join_tablename)
         return (
             left_tablename,
             right_tablename,
             f"""JOIN "{temp_join_tablename}" ON "{right_tablename}"."{right_colname}" = "{temp_join_tablename}".right
                            JOIN "{left_tablename}" ON "{left_tablename}"."{left_colname}" = "{temp_join_tablename}".left
                            """,
             temp_join_tablename,
@@ -286,17 +296,17 @@
 class QAIngredient(Ingredient):
     ingredient_type: str = IngredientType.QA.value
     num_values_passed: int = 0
     allowed_output_types: Tuple[Type] = (Union[str, int, float],)
 
     def __call__(
         self,
-        question: str = None,
-        context: Union[str, pd.DataFrame] = None,
-        options: str = None,
+        question: Optional[str] = None,
+        context: Optional[Union[str, pd.DataFrame]] = None,
+        options: Optional[Union[list, str]] = None,
         *args,
         **kwargs,
     ) -> Union[str, int, float]:
         # Unpack kwargs
         aliases_to_tablenames: Dict[str, str] = kwargs.get("aliases_to_tablenames")
 
         subtable = context
```

### Comparing `blendsql-0.0.141/blendsql/models/_model.py` & `blendsql-0.0.15/blendsql/models/_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import functools
 from typing import Any, List
 import guidance
+import pandas as pd
 from attr import attrib, attrs
 from pathlib import Path
 from dotenv import load_dotenv
 from colorama import Fore
 import time
 import threading
-import re
 from diskcache import Cache
 import platformdirs
 import hashlib
 from abc import abstractmethod
 
-from blendsql._program import Program, program_to_str
+from .._program import Program, program_to_str
+from .._constants import IngredientKwarg
+from ..db.utils import truncate_df_content
+
+CONTEXT_TRUNCATION_LIMIT = 100
 
 
 class TokenTimer(threading.Thread):
     """Class to handle refreshing tokens."""
 
     def __init__(self, init_fn, refresh_interval_min: int = 30):
         super().__init__()
         self.daemon = True
         self.refresh_interval_min = refresh_interval_min
         self.init_fn = init_fn
 
     def run(self):
-        self.init_fn()
         while True:
             time.sleep(self.refresh_interval_min * 60)
             print(Fore.YELLOW + "Refreshing the access tokens..." + Fore.RESET)
             self.init_fn()
 
 
 @attrs
@@ -43,46 +46,49 @@
     refresh_interval_min: int = attrib(default=None)
     env: str = attrib(default=".")
     caching: bool = attrib(default=True)
 
     model: guidance.models.Model = attrib(init=False)
     prompts: list = attrib(init=False)
     cache: Cache = attrib(init=False)
+    run_setup_on_load: bool = attrib(default=True)
 
     gen_kwargs: dict = {}
     num_llm_calls: int = 0
     num_prompt_tokens: int = 0
 
     def __attrs_post_init__(self):
-        self.cache = Cache(
-            Path(platformdirs.user_cache_dir("blendsql"))
-            / f"{self.model_name_or_path}.diskcache"
-        )
+        if self.caching:
+            self.cache = Cache(
+                Path(platformdirs.user_cache_dir("blendsql"))
+                / f"{self.model_name_or_path}.diskcache"
+            )
         self.prompts: List[str] = []
         if self.requires_config:
             if self.env is None:
                 self.env = "."
             _env = Path(self.env)
             env_filepath = _env / ".env" if _env.is_dir() else _env
             if env_filepath.is_file():
-                load_dotenv()
+                load_dotenv(str(env_filepath))
             else:
                 raise FileNotFoundError(
                     f"{self.__class__} requires a .env file to be present at '{env_filepath}' with necessary environment variables\nPut it somewhere else? Use the `env` argument to point me to the right directory."
                 )
         if self.refresh_interval_min:
             timer = TokenTimer(
                 init_fn=self._setup, refresh_interval_min=self.refresh_interval_min
             )
             timer.start()
         if self.tokenizer is not None:
             assert hasattr(self.tokenizer, "encode") and callable(
                 self.tokenizer.encode
             ), f"`tokenizer` passed to {self.__class__} should have `encode` method!"
-        self._setup()
+        if self.run_setup_on_load:
+            self._setup()
         self.model = self._load_model()
 
     def predict(self, program: Program, **kwargs) -> dict:
         """Takes a `Program` and some kwargs, and evaluates it with context of
         current Model.
 
         Args:
@@ -96,25 +102,25 @@
             >>> llm.predict(program, **kwargs)
             {"result": '"This is Model generated output"'}
         """
         if self.caching:
             # First, check our cache
             key = self._create_key(program, **kwargs)
             if key in self.cache:
+                self.prompts.insert(
+                    -1, self.format_prompt(self.cache.get(key), **kwargs)
+                )
                 return self.cache.get(key)
         # Modify fields used for tracking Model usage
         self.num_llm_calls += 1
         model = program(model=self.model, **kwargs)
         if self.tokenizer is not None:
-            prompt = re.sub(
-                r"(?<=\>)(assistant|user|system)", "", model._current_prompt()
-            )
-            prompt = re.sub(r"\<.*?\>", "", prompt)
+            prompt = model._current_prompt()
             self.num_prompt_tokens += len(self.tokenizer.encode(prompt))
-            self.prompts.append(prompt)
+        self.prompts.insert(-1, self.format_prompt(model._variables, **kwargs))
         if self.caching:
             self.cache[key] = model._variables
         return model._variables
 
     def _create_key(self, program: Program, **kwargs) -> str:
         """Generates a hash to use in diskcache Cache.
         This way, we don't need to send our prompts to the same Model
@@ -124,28 +130,42 @@
             md5 hash used as key in diskcache
         """
         hasher = hashlib.md5()
         # Ignore partials, which create a random key within session
         options_str = str(
             sorted(
                 [
-                    (k, v)
+                    (k, sorted(v) if isinstance(v, set) else v)
                     for k, v in kwargs.items()
                     if not isinstance(v, functools.partial)
                 ]
             )
         )
         combined = "{}||{}||{}".format(
             f"{self.model_name_or_path}||{type(self)}",
             program_to_str(program),
             options_str,
         ).encode()
         hasher.update(combined)
         return hasher.hexdigest()
 
+    @staticmethod
+    def format_prompt(res, **kwargs) -> dict:
+        d = {"answer": res}
+        if IngredientKwarg.QUESTION in kwargs:
+            d[IngredientKwarg.QUESTION] = kwargs.get(IngredientKwarg.QUESTION)
+        if IngredientKwarg.CONTEXT in kwargs:
+            context = kwargs.get(IngredientKwarg.CONTEXT)
+            if isinstance(context, pd.DataFrame):
+                context = truncate_df_content(context, CONTEXT_TRUNCATION_LIMIT)
+                d[IngredientKwarg.CONTEXT] = context.to_dict(orient="records")
+        if IngredientKwarg.VALUES in kwargs:
+            d[IngredientKwarg.VALUES] = kwargs.get(IngredientKwarg.VALUES)
+        return d
+
     @abstractmethod
     def _setup(self, **kwargs) -> None:
         """Any additional setup required to get this Model up and functioning
         should go here. For example, in the AzureOpenaiLLM, we have some logic
         to refresh our client secrets every 30 min.
         """
         ...
```

### Comparing `blendsql-0.0.141/blendsql/models/local/_transformers.py` & `blendsql-0.0.15/blendsql/models/local/_transformers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import logging
-
+import importlib.util
 from guidance.models import Transformers, Model
 
 from .._model import Model
 
 logging.getLogger("guidance").setLevel(logging.CRITICAL)
 
+_has_transformers = importlib.util.find_spec("transformers") is not None
+
 
 class TransformersLLM(Model):
     """Class for Transformers local Model.
 
     Args:
         model_name_or_path: Name of the model on HuggingFace, or the path to a local model
     """
 
     def __init__(self, model_name_or_path: str, **kwargs):
-        try:
-            import transformers
-        except ImportError:
-            raise Exception(
+        if not _has_transformers:
+            raise ImportError(
                 "Please install transformers with `pip install transformers`!"
             ) from None
+        import transformers
+
         super().__init__(
             model_name_or_path=model_name_or_path,
             requires_config=False,
             tokenizer=transformers.AutoTokenizer.from_pretrained(model_name_or_path),
             **kwargs
         )
```

### Comparing `blendsql-0.0.141/blendsql/models/remote/_openai.py` & `blendsql-0.0.15/blendsql/models/remote/_openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import os
-from guidance.models import OpenAI, AzureOpenAI, Model
+from guidance.models import OpenAI, AzureOpenAI
 import tiktoken
 
 from .._model import Model
 
 logging.getLogger("openai").setLevel(logging.CRITICAL)
 logging.getLogger("guidance").setLevel(logging.CRITICAL)
 logging.getLogger("asyncio").setLevel(logging.CRITICAL)
@@ -66,15 +66,15 @@
         )
 
     def _load_model(self) -> Model:
         return AzureOpenAI(
             self.model_name_or_path,
             api_key=os.getenv("OPENAI_API_KEY"),
             azure_endpoint=os.getenv("OPENAI_API_BASE"),
-            azure_deployment=os.getenv("API_VERSION"),
+            azure_deployment=os.getenv("OPENAI_API_VERSION"),
             echo=False,
         )
 
     def _setup(self, **kwargs) -> None:
         openai_setup()
         self.model = self._load_model()
```

### Comparing `blendsql-0.0.141/blendsql/utils.py` & `blendsql-0.0.15/blendsql/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from typing import Tuple, Collection
+from typing import Tuple
 import re
-import logging
-from colorama import Fore
 from tabulate import tabulate
 from functools import partial
 
 
-from .db.sqlite import SQLite
 from ._constants import HF_REPO_ID
 
 tabulate = partial(tabulate, headers="keys", showindex="never", tablefmt="orgtbl")
 
 
 def fetch_from_hub(filename: str):
     try:
         from huggingface_hub import hf_hub_download
     except ImportError:
         raise ImportError(
             f"You need huggingface_hub to run this!\n`pip install huggingface_hub`"
         ) from None
-    return hf_hub_download(repo_id=HF_REPO_ID, filename=filename, repo_type="dataset")
+    return hf_hub_download(
+        repo_id=HF_REPO_ID, filename=filename, repo_type="dataset", force_download=True
+    )
 
 
 def get_tablename_colname(s: str) -> Tuple[str, str]:
     """Takes as input a string in the format `{tablename}::{colname}`
     Returns individual parts, but raises error if `s` is in the wrong format.
     """
     out = s.split("::")
@@ -52,42 +51,25 @@
         r"(?<=( |,|\()|\.)\"?{}\"?(?=( |,|\)|;|\.|$))".format(original_tablename),
         new_tablename,
         query,
         flags=re.IGNORECASE,
     )
 
 
-def delete_session_tables(db: SQLite, cleanup_tables: Collection[str]):
-    """Deletes the temporary tables made for the sake of a BlendSQL execution session.
-
-    Args:
-        db: Database connector
-        session_uuid: Unique string we used to identify temporary tables make during a BlendSQL session
-    """
-    if len(cleanup_tables) > 0:
-        logging.debug(
-            Fore.LIGHTMAGENTA_EX + f"Deleting temporary tables..." + Fore.RESET
-        )
-        for tablename in cleanup_tables:
-            logging.debug(Fore.MAGENTA + f"Deleting {tablename}..." + Fore.RESET)
-            db.con.execute(f"DROP TABLE '{tablename}'")
-
-
 def recover_blendsql(select_sql: str):
     """Given a SQL `SELECT` statement, recovers BlendSQL syntax from SQLGlot SQLiteDialect interpretation.
     TODO: this is hack to convert sqlglot SQLite to BlendSQL.
     Examples:
         >>> recover_blendsql("STRUCT(STRUCT(QA('can i get my car fixed here?', 'transactions::merchant')))")
         {{QA('can i get my car fixed here?', 'transactions::merchant')}}
     """
     recovered = re.sub(
-        r"(STRUCT\( ?STRUCT\()(.*?)(\)\)([^\)]|$))(,)?", r" {{\2}}\4 ", select_sql
+        r"(STRUCT\( ?STRUCT\()(.*?)(\){3})(,)?", r" {{\2)}}\4 ", select_sql
     )
-    # TODO: below is a hack for MIN(), MAX() type wrappings around an ingredient
-    return re.sub(re.escape("))}}"), ")}})", recovered)
+    return recovered
 
 
 def get_temp_subquery_table(
     session_uuid: str, subquery_idx: str, tablename: str
 ) -> str:
     """Generates temporary tablename for a subquery"""
     return f"{session_uuid}_{tablename}_{subquery_idx}"
```

### Comparing `blendsql-0.0.141/blendsql.egg-info/PKG-INFO` & `blendsql-0.0.15/blendsql.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 Metadata-Version: 2.1
 Name: blendsql
-Version: 0.0.141
-Summary: Orchestrate SQLite logic and LLM reasoning within a unified dialect.
+Version: 0.0.15
+Summary: Query language to blend SQL logic and LLM reasoning across multi-modal data.
 Home-page: https://github.com/parkervg/blendsql
 Author: Parker Glenn
 Author-email: parkervg5@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: guidance>=0.1.0
 Requires-Dist: pyparsing==3.1.1
-Requires-Dist: pandas>=2.0.0
+Requires-Dist: pandas==1.5.3
 Requires-Dist: bottleneck>=1.3.6
 Requires-Dist: python-dotenv==1.0.1
 Requires-Dist: sqlglot==18.13.0
+Requires-Dist: sqlalchemy>=2.0.0
 Requires-Dist: platformdirs
-Requires-Dist: pre-commit
 Requires-Dist: attrs
 Requires-Dist: tqdm
-Requires-Dist: dateparser
 Requires-Dist: colorama
-Requires-Dist: fiscalyear
 Requires-Dist: tabulate
 Requires-Dist: typeguard
+Provides-Extra: nl-to-blendsql
+Requires-Dist: exrex; extra == "nl-to-blendsql"
+Requires-Dist: lark; extra == "nl-to-blendsql"
 Provides-Extra: research
 Requires-Dist: datasets==2.16.1; extra == "research"
 Requires-Dist: nltk; extra == "research"
 Requires-Dist: wikiextractor; extra == "research"
 Requires-Dist: rouge_score; extra == "research"
 Requires-Dist: rapidfuzz; extra == "research"
 Requires-Dist: records; extra == "research"
 Requires-Dist: SQLAlchemy; extra == "research"
 Requires-Dist: recognizers-text; extra == "research"
 Requires-Dist: recognizers-text-suite; extra == "research"
 Requires-Dist: emoji==1.7.0; extra == "research"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: huggingface_hub; extra == "test"
+Requires-Dist: pre-commit; extra == "test"
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == "docs"
 Requires-Dist: mkdocstrings; extra == "docs"
 Requires-Dist: mkdocs-section-index; extra == "docs"
 Requires-Dist: mkdocstrings-python; extra == "docs"
 Requires-Dist: mkdocs-jupyter; extra == "docs"
+Provides-Extra: demo
+Requires-Dist: chainlit; extra == "demo"
 
 <div align="right">
 <a href="https://opensource.org/licenses/Apache-2.0"><img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" /></a>
 <a><img src="https://img.shields.io/github/last-commit/parkervg/blendsql?color=green"/></a>
 <a><img src="https://img.shields.io/badge/PRs-Welcome-Green"/></a>
 <br>
 </div>
@@ -57,17 +61,28 @@
 </picture>
 <p align="center">
     <i> SQL 🤝 LLMs </i>
   </p>
 <b>Check out our <a href="https://parkervg.github.io/blendsql/" target="_blank">online documentation</a> for a more comprehensive overview.</b>
 
 <i>Results from the paper are available [here](https://github.com/parkervg/blendsql/tree/research-paper/research/paper-results)</i>
+
 </div>
 <br/>
 
+### Features
+
+- Supports many DBMS 💾
+  - Currently, SQLite and PostgreSQL are functional - more to come! 
+- Easily extendable to [multi-modal usecases](./examples/vqa-ingredient.ipynb) 🖼️
+- Smart parsing optimizes what is passed to external functions 🧠
+  - Traverses abstract syntax tree with [sqlglot](https://github.com/tobymao/sqlglot) to minimize LLM function calls 🌳
+- Constrained decoding with [guidance](https://github.com/guidance-ai/guidance) 🚀
+- LLM function caching, built on [diskcache](https://grantjenks.com/docs/diskcache/) 🔑
+
 ## Intro
 BlendSQL is a *superset of SQLite* for problem decomposition and hybrid question-answering with LLMs. 
 
 As a result, we can *Blend* together...
 
 - 🥤 ...operations over heterogeneous data sources (e.g. tables, text, images)
 - 🥤 ...the structured & interpretable reasoning of SQL with the generalizable reasoning of LLMs
@@ -77,59 +92,64 @@
 **Now, the user is given the control to oversee all calls (LLM + SQL) within a unified query language.**
 
 ![comparison](docs/img/comparison.jpg)
 
 For example, imagine we have the following tables.
 
 ### `w`
+
 | **date** | **rival**                 | **city**  | **venue**                   | **score** |
-|----------|---------------------------|-----------|-----------------------------|-----------|
+| -------- | ------------------------- | --------- | --------------------------- | --------- |
 | 31 may   | nsw waratahs              | sydney    | agricultural society ground | 11-0      |
 | 5 jun    | northern districts        | newcastle | sports ground               | 29-0      |
 | 7 jun    | nsw waratahs              | sydney    | agricultural society ground | 21-2      |
 | 11 jun   | western districts         | bathurst  | bathurst ground             | 11-0      |
 | 12 jun   | wallaroo & university nsw | sydney    | cricket ground              | 23-10     |
 
 ### `documents`
+
 | **title**                      | **content**                                       |
-|--------------------------------|---------------------------------------------------|
+| ------------------------------ | ------------------------------------------------- |
 | sydney                         | sydney ( /ˈsɪdni/ ( listen ) sid-nee ) is the ... |
 | new south wales waratahs       | the new south wales waratahs ( /ˈwɒrətɑːz/ or ... |
 | sydney showground (moore park) | the former sydney showground ( moore park ) at... |
 | sydney cricket ground          | the sydney cricket ground ( scg ) is a sports ... |
 | newcastle, new south wales     | the newcastle ( /ˈnuːkɑːsəl/ new-kah-səl ) met... |
 | bathurst, new south wales      | bathurst /ˈbæθərst/ is a city in the central t... |
 
 BlendSQL allows us to ask the following questions by injecting "ingredients", which are callable functions denoted by double curly brackets (`{{`, `}}`).
-The below examples work out of the box, but you are able to design your own ingredients as well! 
+The below examples work out of the box, but you are able to design your own ingredients as well!
+
+_What was the result of the game played 120 miles west of Sydney?_
 
-*What was the result of the game played 120 miles west of Sydney?*
 ```sql
 SELECT * FROM w
     WHERE city = {{
         LLMQA(
             'Which city is located 120 miles west of Sydney?',
             (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
             options='w::city'
         )
     }}
 ```
 
-*Which venues in Sydney saw more than 30 points scored?*
+_Which venues in Sydney saw more than 30 points scored?_
+
 ```sql
 SELECT DISTINCT venue FROM w
     WHERE city = 'sydney' AND {{
         LLMMap(
             'More than 30 total points?',
             'w::score'
         )
     }} = TRUE
 ```
 
-*Show all NSW Waratahs games and a description of the team.*
+_Show all NSW Waratahs games and a description of the team._
+
 ```sql
 SELECT date, rival, score, documents.content AS "Team Description" FROM w
     JOIN {{
         LLMJoin(
             left_on='documents::title',
             right_on='w::rival'
         )
@@ -140,72 +160,76 @@
 
 <p>
 <details>
 <summary> <b> <a href="https://hybridqa.github.io/" target="_blank"> HybridQA </a> </b> </summary>
 
 For this setting, our database contains 2 tables: a table from Wikipedia `w`, and a collection of unstructured Wikipedia articles in the table `documents`.
 
-*What is the state flower of the smallest state by area ?*
+_What is the state flower of the smallest state by area ?_
+
 ```sql
-SELECT "common name" AS 'State Flower' FROM w 
+SELECT "common name" AS 'State Flower' FROM w
 WHERE state = {{
     LLMQA(
         'Which is the smallest state by area?',
         (SELECT title, content FROM documents),
         options='w::state'
     )
 }}
 ```
 
-*Who were the builders of the mosque in Herat with fire temples ?*
+_Who were the builders of the mosque in Herat with fire temples ?_
+
 ```sql
 {{
     LLMQA(
-        'Name of the builders?',
+        'Who were the builders of the mosque?',
         (
-            SELECT title AS 'Building', content FROM documents
-                WHERE title = {{
-                    LLMQA(
-                        'Align the name to the correct title.',
-                        (SELECT name FROM w WHERE city = 'herat' AND remarks LIKE '%fire temple%'),
-                        options='documents::title'
-                    )
-                }}
-        ) 
+            SELECT documents.title AS 'Building', documents.content FROM documents
+            JOIN {{
+                LLMJoin(
+                    left_on='w::name',
+                    right_on='documents::title'
+                )
+            }}
+            WHERE w.city = 'herat' AND w.remarks LIKE '%fire temple%'
+        )
     )
 }}
 ```
 
-*What is the capacity of the venue that was named in honor of Juan Antonio Samaranch in 2010 after his death ?*
+_What is the capacity of the venue that was named in honor of Juan Antonio Samaranch in 2010 after his death ?_
+
 ```sql
 SELECT capacity FROM w WHERE venue = {{
     LLMQA(
         'Which venue is named in honor of Juan Antonio Samaranch?',
         (SELECT title AS 'Venue', content FROM documents),
         options='w::venue'
     )
 }}
-```    
+```
 
 </details>
 </p>
 
 <p>
 <details>
 <summary> <b> <a href="https://ott-qa.github.io/" target="_blank"> OTT-QA </a> </b> </summary>
 
 Unlike HybridQA, these questions are open-domain, where we don't know in advance where the answer of a given open question appears in a passage or a table.
 
 As a result, we need to play the role of both the retriever (to select relevant context) and reader (to read from relevant contexts and return the given answer).
 
 As the underlying database consists of 400K tables and 5M documents, it's important to set `LIMIT` clauses appropriately to ensure reasonable execution times.
 
-The examples below also demonstrate how BlendSQL unpacks [CTE statements](https://www.sqlite.org/lang_with.html) to ensure we only pass necessary data into the BlendSQL ingredient calls. 
+The examples below also demonstrate how BlendSQL unpacks [CTE statements](https://www.sqlite.org/lang_with.html) to ensure we only pass necessary data into the BlendSQL ingredient calls.
+
+_When was the third highest paid Rangers F.C . player born ?_
 
-*When was the third highest paid Rangers F.C . player born ?*
 ```sql
 {{
     LLMQA(
         'When was the Rangers Player born?',
         (
             WITH t AS (
                 SELECT player FROM (
@@ -216,40 +240,42 @@
                 SELECT * FROM documents JOIN t WHERE documents MATCH t.player || ' OR rangers OR fc' ORDER BY rank LIMIT 5
             ) SELECT d.content, t.player AS 'Rangers Player' FROM d JOIN t
         )
     )
 }}
 ```
 
-*In which Track Cycling World Championships event was the person born in Matanzas , Cuba ranked highest ?*
+_In which Track Cycling World Championships event was the person born in Matanzas , Cuba ranked highest ?_
+
 ```sql
 {{
     LLMQA(
         'In what event was the cyclist ranked highest?',
         (
             SELECT * FROM (
                 SELECT * FROM "./Cuba at the UCI Track Cycling World Championships (2)"
             ) as w WHERE w.name = {{
                 LLMQA(
                     "Which cyclist was born in Matanzas, Cuba?",
                     (
-                        SELECT * FROM documents 
-                            WHERE documents MATCH 'matanzas AND (cycling OR track OR born)' 
+                        SELECT * FROM documents
+                            WHERE documents MATCH 'matanzas AND (cycling OR track OR born)'
                             ORDER BY rank LIMIT 3
                     ),
                     options="w::name"
                 )
             }}
         ),
         options='w::event'
     )
 }}
 ```
 
-*Who is the director the Togolese film that was a 30 minute film that was shot in 16mm ?*
+_Who is the director the Togolese film that was a 30 minute film that was shot in 16mm ?_
+
 ```sql
 SELECT director FROM "./List of African films (4)" as w
 WHERE title = {{
     LLMQA(
         'What is the name of the Togolese film that was 30 minutes and shot in 16mm?',
         (SELECT * FROM documents WHERE documents MATCH 'togolese OR 30 OR 16mm OR film' ORDER BY rank LIMIT 5),
         options='w::title'
@@ -262,41 +288,44 @@
 
 <p>
 <details>
 <summary> <b> <a href="https://fever.ai/dataset/feverous.html" target="_blank"> FEVEROUS </a> </b> </summary>
 
 Here, we deal not with questions, but truth claims given a context of unstructured and structured data.
 
-These claims should be judged as "SUPPORTS" or "REFUTES". Using BlendSQL, we can formulate this determination of truth as a function over facts. 
+These claims should be judged as "SUPPORTS" or "REFUTES". Using BlendSQL, we can formulate this determination of truth as a function over facts.
+
+_Oyedaea is part of the family Asteraceae in the order Asterales._
 
-*Oyedaea is part of the family Asteraceae in the order Asterales.*
 ```sql
 SELECT EXISTS (
     SELECT * FROM w0 WHERE "family:" = 'asteraceae' AND "order:" = 'asterales'
-) 
+)
 ```
 
-*The 2006-07 San Jose Sharks season, the 14th season of operation (13th season of play) for the National Hockey League (NHL) franchise, scored the most points in the Pacific Division.*
+_The 2006-07 San Jose Sharks season, the 14th season of operation (13th season of play) for the National Hockey League (NHL) franchise, scored the most points in the Pacific Division._
+
 ```sql
 SELECT (
     {{
         LLMValidate(
-            'Is the Sharks 2006-07 season the 14th season (13th season of play)?', 
+            'Is the Sharks 2006-07 season the 14th season (13th season of play)?',
             (SELECT * FROM documents)
         )
     }}
 ) AND (
     SELECT (SELECT filledcolumnname FROM w0 ORDER BY pts DESC LIMIT 1) = 'san jose sharks'
 )
 ```
 
-*Saunders College of Business, which is accredited by the Association to Advance Collegiate Schools of Business International, is one of the colleges of Rochester Institute of Technology established in 1910 and is currently under the supervision of Dean Jacqueline R. Mozrall.*
+_Saunders College of Business, which is accredited by the Association to Advance Collegiate Schools of Business International, is one of the colleges of Rochester Institute of Technology established in 1910 and is currently under the supervision of Dean Jacqueline R. Mozrall._
+
 ```sql
 SELECT EXISTS(
-    SELECT * FROM w0 
+    SELECT * FROM w0
     WHERE "parent institution" = 'rochester institute of technology'
     AND "established" = '1910'
     AND "dean" = 'jacqueline r. mozrall'
 ) AND (
     {{
         LLMValidate(
             'Is Saunders College of Business (SCB) accredited by the Association to Advance Collegiate Schools of Business International (AACSB)?',
@@ -306,299 +335,339 @@
 )
 ```
 
 </details>
 </p>
 
 ## Table of Contents
-* [Install](#install)
-* [Quickstart](#quickstart)
-* [FAQ](#faq)
-* [Documentation](#documentation)
-  * [Execute a BlendSQL Query](#execute-a-blendsql-query)
-    * [Smoothie](#smoothie)
-  * [Ingredients](#ingredients)
-    * [MapIngredient](#mapingredient)
-    * [QAIngredient](#qaingredient)
-      * [Constrained Decoding with 'options'](#constrained-decoding-with-options)
-    * [JoinIngredient](#joiningredient)
-    * [StringIngredient](#stringingredient)
-  * [LLMs](#llms)
-  * [Databases](#databases)
-* [Appendix](#appendix)
-
-### Features 
-- Smart parsing optimizes what is passed to external functions 🧠
-  - Traverses abstract syntax tree with [sqlglot](https://github.com/tobymao/sqlglot) to minimize LLM function calls 🌳
-- LLM function caching, built on [diskcache](https://grantjenks.com/docs/diskcache/) 🔑 
-- Constrained decoding with [guidance](https://github.com/guidance-ai/guidance) 🚀
 
+- [Install](#install)
+- [Quickstart](#quickstart)
+- [FAQ](#faq)
+- [Documentation](#documentation)
+  - [Execute a BlendSQL Query](#execute-a-blendsql-query)
+    - [Smoothie](#smoothie)
+  - [Ingredients](#ingredients)
+    - [MapIngredient](#mapingredient)
+    - [QAIngredient](#qaingredient)
+      - [Constrained Decoding with 'options'](#constrained-decoding-with-options)
+    - [JoinIngredient](#joiningredient)
+    - [StringIngredient](#stringingredient)
+  - [Parsing Natural Language to BlendSQL](#parsing-natural-language-to-blendsql)
+  - [LLMs](#llms)
+  - [Databases](#databases)
+- [Appendix](#appendix)
 
 For a technical walkthrough of how a BlendSQL query is executed, check out [technical_walkthrough.md](./docs/technical_walkthrough.md).
 
 ## Install
+
 ```
 pip install blendsql
 ```
 
 ## Quickstart
 
 ```python
-from blendsql import blend, LLMQA, LLMMap
+from blendsql import blend, LLMQA
 from blendsql.db import SQLite
 from blendsql.models import OpenaiLLM
+from blendsql.utils import fetch_from_hub
 
 blendsql = """
-SELECT merchant FROM transactions WHERE 
-     {{LLMMap('is this a pizza shop?', 'transactions::merchant')}} = TRUE
-     AND parent_category = 'Food'
+SELECT * FROM w
+WHERE city = {{
+    LLMQA(
+        'Which city is located 120 miles west of Sydney?',
+        (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
+        options='w::city'
+    )
+}}
 """
 # Make our smoothie - the executed BlendSQL script
 smoothie = blend(
     query=blendsql,
-    blender=OpenaiLLM("gpt-3.5-turbo-0613"),
-    ingredients={LLMMap, LLMQA},
-    db=SQLite(db_path="transactions.db"),
-    verbose=True
+    db=SQLite(fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+    blender=OpenaiLLM("gpt-3.5-turbo"),
+    ingredients={LLMQA},
 )
-
+print(smoothie.df)
+print(smoothie.meta.prompts)
 ```
 
 ### FAQ
 
+#### How does BlendSQL execute a query?
+> BlendSQL handles traversal of the SQL AST and creation of temporary tables to execute a given query. 
+> This allows BlendSQL to be DBMS-agnostic, and extendable into both SQLite, PostgreSQL, and other DBMS.
+
 #### Why not just implement BlendSQL as a [user-defined function in SQLite](https://www.sqlite.org/c3ref/c_deterministic.html#sqlitedeterministic)?
-> LLMs are expensive, both in terms of $ cost and compute time. When applying them to SQLite databases, we want to take special care in ensuring we're not applying them to contexts where they're not required. 
+
+> LLMs are expensive, both in terms of $ cost and compute time. When applying them to SQLite databases, we want to take special care in ensuring we're not applying them to contexts where they're not required.
 > This is [not easily achievable with UDFs](https://sqlite.org/forum/info/649ad4c62fd4b4e8cb5d6407107b8c8a9a0afaaf95a87805e5a8403a79e6616c), even when marked as a [deterministic function](https://www.sqlite.org/c3ref/c_deterministic.html#sqlitedeterministic).
-> 
+>
 > BlendSQL is specifically designed to enforce an order-of-operations that 1) prioritizes vanilla SQL operations first, and 2) caches results from LLM ingredients so they don't need to be recomputed.
 > For example:
-> ```sql 
-> SELECT {{LLMMap('What state is this NBA team from?', 'w::team')} FROM w 
->    WHERE num_championships > 3 
+>
+> ```sql
+> SELECT {{LLMMap('What state is this NBA team from?', 'w::team')} FROM w
+>    WHERE num_championships > 3
 >    ORDER BY {{LLMMap('What state is this NBA team from?', 'w::team')}
-> 
+>
 > ```
+>
 > BlendSQL makes sure to only pass those `team` values from rows which satisfy the condition `num_championship > 3` to the LLM. Additionally, since we assume the function is deterministic, we make a single LLM call and cache the results, despite the ingredient function being used twice.
 
+#### So I get how to write BlendSQL queries. But why would I use this over vanilla SQLite?
 
- #### So I get how to write BlendSQL queries. But why would I use this over vanilla SQLite? 
-> Certain ingredients, like [LLMJoin](#joiningredient), will likely give seasoned SQL experts a headache at first. However, BlendSQL's real strength comes from it's use as an *intermediate representation for reasoning over structured + unstructured with LLMs*. Some examples of this can be found above [here](#more-examples-from-popular-qa-datasets).
+> Certain ingredients, like [LLMJoin](#joiningredient), will likely give seasoned SQL experts a headache at first. However, BlendSQL's real strength comes from it's use as an _intermediate representation for reasoning over structured + unstructured with LLMs_. Some examples of this can be found above [here](#more-examples-from-popular-qa-datasets).
 
 <hr>
 
 ### Citation
+
 ```bibtex
 @article{glenn2024blendsql,
-      title={BlendSQL: A Scalable Dialect for Unifying Hybrid Question Answering in Relational Algebra}, 
+      title={BlendSQL: A Scalable Dialect for Unifying Hybrid Question Answering in Relational Algebra},
       author={Parker Glenn and Parag Pravin Dakle and Liang Wang and Preethi Raghavan},
       year={2024},
       eprint={2402.17882},
       archivePrefix={arXiv},
       primaryClass={cs.CL}
 }
 ```
 
 # Documentation
 
-> [!WARNING]
-> WIP, will be updated
+
+## Databases
+
+Since BlendSQL relies on the package [sqlglot](https://github.com/tobymao/sqlglot) for query optimization (which supports a [wide variety of SQL dialects](https://github.com/tobymao/sqlglot/blob/main/sqlglot/dialects/__init__.py)) and the notion of [temporary tables](https://en.wikibooks.org/wiki/Structured_Query_Language/Temporary_Table), it can easily integrate with many different SQL dialects. 
+
+Currently, the following are supported.
+
+### SQLite
+A SQLite database connection.
+Can be initialized via a path to the database file.
+
+Example:
+```python
+from blendsql.db import SQLite
+db = SQLite("./path/to/database.db")
+```
+
+### PostgreSQL
+A PostgreSQL database connection.
+Can be initialized via the SQLAlchemy input string.
+https://docs.sqlalchemy.org/en/20/core/engines.html#postgresql
+
+Example:
+```python
+from blendsql.db import PostgreSQL
+db = PostgreSQL("user:password@localhost/mydatabase")
+```
 
 ## Execute a BlendSQL Query
-The `blend()` function is used to execute a BlendSQL query against a database and return the final result, in addition to the intermediate reasoning steps taken.
 
-::: blendsql.blendsql.blend
-  handler: python
+The `blend()` function is used to execute a BlendSQL query against a database and return the final result, in addition to the intermediate reasoning steps taken.
 
 ```python
-from blendsql import blend, LLMMap, LLMQA, LLMJoin
+from blendsql import blend, LLMQA
 from blendsql.db import SQLite
 from blendsql.models import OpenaiLLM
+from blendsql.utils import fetch_from_hub
 
 blendsql = """
 SELECT * FROM w
 WHERE city = {{
     LLMQA(
         'Which city is located 120 miles west of Sydney?',
         (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
         options='w::city'
     )
-}} 
+}}
 """
-db = SQLite(db_path)
+# Make our smoothie - the executed BlendSQL script
 smoothie = blend(
     query=blendsql,
-    db=db,
-    ingredients={LLMMap, LLMQA, LLMJoin},
-    blender=AzureOpenaiLLM("gpt-4"),
-    # Optional args below
-    infer_gen_constraints=True,
-    silence_db_exec_errors=False,
-    verbose=True,
-    blender_args={
-        "few_shot": True,
-        "temperature": 0.01
-    }
+    db=SQLite(fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+    blender=OpenaiLLM("gpt-3.5-turbo"),
+    ingredients={LLMQA},
 )
+print(smoothie.df)
+print(smoothie.meta.prompts)
 ```
 
+### Smoothie
 
-### Smoothie 
 The [smoothie.py](./blendsql/_smoothie.py) object defines the output of an executed BlendSQL script.
 
 ```python
 @dataclass
 class Smoothie:
     df: pd.DataFrame
     meta: SmoothieMeta
-    
+
 @dataclass
 class SmoothieMeta:
     process_time_seconds: float
     num_values_passed: int  # Number of values passed to a Map/Join/QA ingredient
     num_prompt_tokens: int  # Number of prompt tokens (counting user and assistant, i.e. input/output)
     prompts: List[str] # Log of prompts submitted to model
     example_map_outputs: List[Any]  # outputs from a Map ingredient, for debugging
     ingredients: List[Ingredient]
     query: str
     db_path: str
     contains_ingredient: bool = True
 
 def blend(*args, **kwargs) -> Smoothie:
-  ... 
+  ...
 ```
+
 <hr>
 
-## Ingredients 
+## Ingredients
 
 ![ingredients](docs/img/ingredients.jpg)
 
-Ingredients are at the core of a BlendSQL script. 
+Ingredients are at the core of a BlendSQL script.
 
 They are callable functions that perform one the task paradigms defined in [ingredient.py](./blendsql/ingredients/ingredient.py).
 
-At their core, these are not a new concept. [User-defined functions (UDFs)](https://docs.databricks.com/en/udf/index.html), or [Application-Defined Functions in SQLite](https://www.sqlite.org/appfunc.html) have existed for quite some time. 
+At their core, these are not a new concept. [User-defined functions (UDFs)](https://docs.databricks.com/en/udf/index.html), or [Application-Defined Functions in SQLite](https://www.sqlite.org/appfunc.html) have existed for quite some time.
 
 However, ingredients in BlendSQL are intended to be optimized towards LLM-based functions, defining an order of operations for traversing the AST such that the minimal amount of data is passed into your expensive GPT-4/Llama 2/Mistral 7b/etc. prompt.
 
 Ingredient calls are denoted by wrapping them in double curly brackets, `{{ingredient}}`.
 
 The following ingredient types are valid.
 
 ### MapIngredient
+
 This type of ingredient applies a function on a given table/column pair to create a new column containing the function output.
 
 For example, take the following query.
 
-```sql 
+```sql
 SELECT merchant FROM transactions
     WHERE {{LLMMap('Is this a pizza shop?', 'transactions::merchant')}} = TRUE
 ```
 
 `LLMMap` is one of our builtin MapIngredients. For each of the distinct values in the "merchant" column of the "transactions" table, it will create a column containing the function output.
 
 | merchant | Is this a pizza shop? |
-|----------|-----------------------|
+| -------- | --------------------- |
 | Domino's | 1                     |
 | Safeway  | 0                     |
 | Target   | 0                     |
 
 The temporary table shown above is then combined with the original "transactions" table with an `INNER JOIN` on the "merchant" column.
 
 ### JoinIngredient
+
 Handles the logic of semantic `JOIN` clauses between tables.
 
 For example:
+
 ```sql
 SELECT Capitals.name, State.name FROM Capitals
     JOIN {{
         LLMJoin(
-            'Align state to capital', 
-            left_on='States::name', 
+            'Align state to capital',
+            left_on='States::name',
             right_on='Capitals::name'
         )
     }}
 ```
+
 The above example hints at a database schema that would make [E.F Codd](https://en.wikipedia.org/wiki/Edgar_F._Codd) very angry: why do we have two separate tables `States` and `Capitals` with no foreign key to join the two?
 
 BlendSQL was built to interact with tables "in-the-wild", and many (such as those on Wikipedia) do not have these convenient properties of well-designed relational models.
 
 For this reason, we can leverage the internal knowledge of a pre-trained LLM to do the `JOIN` operation for us.
 
 ### QAIngredient
+
 Sometimes, simply selecting data from a given database is not enough to sufficiently answer a user's question.
 
 The `QAIngredient` is designed to return data of variable types, and is best used in cases when we either need:
-1) Unstructured, free-text responses ("Give me a summary of all my spending in coffe")
-2) Complex, unintuitive relationships extracted from table subsets ("How many consecutive days did I spend in coffee?")
+
+1. Unstructured, free-text responses ("Give me a summary of all my spending in coffe")
+2. Complex, unintuitive relationships extracted from table subsets ("How many consecutive days did I spend in coffee?")
 
 The following query demonstrates usage of the builtin `LLMQA` ingredient.
 
 ```sql
 {{
     LLMQA(
-        'How many consecutive days did I buy stocks in Financials?', 
+        'How many consecutive days did I buy stocks in Financials?',
         (
             SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
               FROM account_history
               LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
               WHERE Sector = "Financials"
               ORDER BY "Run Date" LIMIT 5
         )
     )
-}} 
+}}
 ```
-This is slightly more complicated than the rest of the ingredients. 
+
+This is slightly more complicated than the rest of the ingredients.
 
 Behind the scenes, we wrap the call to `LLMQA` in a trivial `CASE` clause, ensuring that the ingredient's output gets returned.
-```sql 
-SELECT CASE WHEN FALSE THEN FALSE 
+
+```sql
+SELECT CASE WHEN FALSE THEN FALSE
   WHEN TRUE then {{QAIngredient}}
   END
 ```
+
 The LLM gets both the question asked, alongside the subset of the SQL database fetched by our subquery.
 
 | **"Run Date"** | **Symbol** | **Sector** |
-|----------------|------------|------------|
+| -------------- | ---------- | ---------- |
 | 2022-01-14     | HBAN       | Financials |
 | 2022-01-20     | AIG        | Financials |
 | 2022-01-24     | AIG        | Financials |
 | 2022-01-24     | NTRS       | Financials |
 | 2022-01-25     | HBAN       | Financials |
 
-
 From examining this table, we see that we bought stocks in the Financials sector 2 consecutive days (2022-01-24, and 2022-01-25).
 The LLM answers the question in an end-to-end manner, returning the result `2`.
 
 The `QAIngredient` can be used as a standalone end-to-end QA tool, or as a component within a larger BlendSQL query.
 
-For example, the BlendSQL query below translates to the valid (but rather confusing) question: 
+For example, the BlendSQL query below translates to the valid (but rather confusing) question:
 
 "Show me stocks in my portfolio, whose price is greater than the number of consecutive days I bought Financial stocks multiplied by 10. Only display those companies which offer a media streaming service."
+
 ```sql
  SELECT Symbol, "Last Price" FROM portfolio WHERE "Last Price" > {{
   LLMQA(
-        'How many consecutive days did I buy stocks in Financials?', 
+        'How many consecutive days did I buy stocks in Financials?',
         (
             SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
               FROM account_history
               LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
               WHERE Sector = "Financials"
               ORDER BY "Run Date" LIMIT 5
         )
     )
   }} * 10
   AND {{LLMMap('Offers a media streaming service?', 'portfolio::Description')}} = 1
 ```
+
 #### Constrained Decoding with `options`
+
 Perhaps we want the answer to the above question in a different format. We call our LLM ingredient in a constrained setting by passing a `options` argument, where we provide either semicolon-separated options, or a reference to a column.
 
 ```sql
 {{
     LLMQA(
-        'How many consecutive days did I buy stocks in Financials?', 
+        'How many consecutive days did I buy stocks in Financials?',
         (
             SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
               FROM account_history
               LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
               WHERE Sector = "Financials"
               ORDER BY "Run Date" LIMIT 5
         )
@@ -607,27 +676,28 @@
 }}
 ```
 
 Running the above BlendSQL query, we get the output `two consecutive days!`.
 
 This `options` argument can also be a reference to a given column.
 
-For example (from the [HybridQA dataset](https://hybridqa.github.io/)): 
+For example (from the [HybridQA dataset](https://hybridqa.github.io/)):
 
-```sql 
+```sql
  SELECT capacity FROM w WHERE venue = {{
         LLMQA(
             'Which venue is named in honor of Juan Antonio Samaranch?',
             (SELECT title, content FROM documents WHERE content LIKE '%venue%'),
             options='w::venue'
         )
 }}
 ```
 
 Or, from our running example:
+
 ```sql
 {{
   LLMQA(
       'Which did i buy the most?',
       (
         SELECT account_history."Run Date", account_history.Symbol, constituents."Sector"
           FROM account_history
@@ -639,56 +709,84 @@
   )
 }}
 ```
 
 The above BlendSQL will yield the result `AIG`, since it appears in the `Symbol` column from `account_history`.
 
 ### StringIngredient
+
 This is the simplest type of ingredient. This will output a string to be placed directly into the SQL query.
 
 We have the `DT` function as a builtin StringIngredient.
 
-```sql 
+```sql
 SELECT merchant FROM transactions
     WHERE {{DT('transactions::date', start='q2')}}
 ```
 
 This will call a Python function that uses `datetime` to interpret the absolute dates which the relative phrase "q2" most likely refers to.
 
 We do not create any new tables or perform any joins with a StringIngredient; instead, we simply get the following SQL query.
 
 > [!NOTE]
 > The below SQL interpretation of the `DT` function assumes we're calling it in December, 2022. The phrase 'q2' will be interpreted differently in, say, March 1998.
 
-```sql 
+```sql
 SELECT merchant FROM transactions
     WHERE date > '2022-09-30' AND date < '2022-12-01'
 ```
 
-<hr> 
- 
+<hr>
+
+## Parsing Natural Language to BlendSQL
 
-## LLMs
+```python
+from blendsql import nl_to_blendsql, LLMMap
+from blendsql.models import TransformersLLM
+from blendsql.db import SQLite
+from blendsql.utils import fetch_from_hub
 
+model = TransformersLLM("Qwen/Qwen1.5-0.5B")
+db = SQLite(fetch_from_hub("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db"))
 
-<hr> 
+query = nl_to_blendsql(
+    question="Which venues in Sydney saw more than 30 points scored?",
+    model=model,
+    ingredients={LLMMap},
+    serialized_db=db.to_serialized(num_rows=3, use_tables=["w", "documents"]),
+    verbose=True,
+    max_grammar_corrections=5,
+)
+```
 
-## Databases
+### Grammar-Based Correction
 
+If you use the grammar prompting feature of BlendSQL, please cite the original grammar prompting paper below.
 
-<hr> 
+```bibtex
+@article{wang2024grammar,
+  title={Grammar prompting for domain-specific language generation with large language models},
+  author={Wang, Bailin and Wang, Zi and Wang, Xuezhi and Cao, Yuan and A Saurous, Rif and Kim, Yoon},
+  journal={Advances in Neural Information Processing Systems},
+  volume={36},
+  year={2024}
+}
+```
+
+<hr>
 ### Appendix
-#### Run Line Profiling 
+#### Run Line Profiling
 First uncomment `@profile` above `blend()` in `blendsql.py`.
 Make sure you've run `pip install line_profiler` first. This installs the tool here: https://github.com/pyutils/line_profiler
 
 `PYTHONPATH=$PWD:$PYTHONPATH kernprof -lv examples/benchmarks/with_blendsql.py`
 
 #### Benchmarks
-The below benchmarks were done on my local M1 Macbook Pro. by running the scripts found in `examples/benchmarks`. 
+
+The below benchmarks were done on my local M1 Macbook Pro. by running the scripts found in `examples/benchmarks`.
 'Lines of Code' is a rough estimate of the user-written code for each usecase.
 
-| **Name**                     | **Description**                                                 | **Runtime/s (Across 10 runs)** | **Lines of Code** |
-|------------------------------|-----------------------------------------------------------------|-------------------------------------------------|-------------------|
-| BlendSQL                     |                                                     |5.685 +/- 0.930                                 | 9                 |
-| SQL + LLM Calls       | Filtering what we can with SQL, then running LLM calls.         | 9.083 +/- 2.061                                 | 106               |
-| Naive SQL + LLM Calls | Runing LLM calls on entire table, regardless of SQL conditions. | 64.809 +/- 6.225                                | 106               |
+| **Name**              | **Description**                                                 | **Runtime/s (Across 10 runs)** | **Lines of Code** |
+| --------------------- | --------------------------------------------------------------- | ------------------------------ | ----------------- |
+| BlendSQL              |                                                                 | 5.685 +/- 0.930                | 9                 |
+| SQL + LLM Calls       | Filtering what we can with SQL, then running LLM calls.         | 9.083 +/- 2.061                | 106               |
+| Naive SQL + LLM Calls | Runing LLM calls on entire table, regardless of SQL conditions. | 64.809 +/- 6.225               | 106               |
```

#### html2text {}

```diff
@@ -1,207 +1,230 @@
-Metadata-Version: 2.1 Name: blendsql Version: 0.0.141 Summary: Orchestrate
-SQLite logic and LLM reasoning within a unified dialect. Home-page: https://
+Metadata-Version: 2.1 Name: blendsql Version: 0.0.15 Summary: Query language to
+blend SQL logic and LLM reasoning across multi-modal data. Home-page: https://
 github.com/parkervg/blendsql Author: Parker Glenn Author-email:
 parkervg5@gmail.com License: Apache License 2.0 Description-Content-Type: text/
 markdown License-File: LICENSE Requires-Dist: guidance>=0.1.0 Requires-Dist:
-pyparsing==3.1.1 Requires-Dist: pandas>=2.0.0 Requires-Dist: bottleneck>=1.3.6
+pyparsing==3.1.1 Requires-Dist: pandas==1.5.3 Requires-Dist: bottleneck>=1.3.6
 Requires-Dist: python-dotenv==1.0.1 Requires-Dist: sqlglot==18.13.0 Requires-
-Dist: platformdirs Requires-Dist: pre-commit Requires-Dist: attrs Requires-
-Dist: tqdm Requires-Dist: dateparser Requires-Dist: colorama Requires-Dist:
-fiscalyear Requires-Dist: tabulate Requires-Dist: typeguard Provides-Extra:
+Dist: sqlalchemy>=2.0.0 Requires-Dist: platformdirs Requires-Dist: attrs
+Requires-Dist: tqdm Requires-Dist: colorama Requires-Dist: tabulate Requires-
+Dist: typeguard Provides-Extra: nl-to-blendsql Requires-Dist: exrex; extra ==
+"nl-to-blendsql" Requires-Dist: lark; extra == "nl-to-blendsql" Provides-Extra:
 research Requires-Dist: datasets==2.16.1; extra == "research" Requires-Dist:
 nltk; extra == "research" Requires-Dist: wikiextractor; extra == "research"
 Requires-Dist: rouge_score; extra == "research" Requires-Dist: rapidfuzz; extra
 == "research" Requires-Dist: records; extra == "research" Requires-Dist:
 SQLAlchemy; extra == "research" Requires-Dist: recognizers-text; extra ==
 "research" Requires-Dist: recognizers-text-suite; extra == "research" Requires-
 Dist: emoji==1.7.0; extra == "research" Provides-Extra: test Requires-Dist:
 pytest; extra == "test" Requires-Dist: huggingface_hub; extra == "test"
-Provides-Extra: docs Requires-Dist: mkdocs-material; extra == "docs" Requires-
-Dist: mkdocstrings; extra == "docs" Requires-Dist: mkdocs-section-index; extra
-== "docs" Requires-Dist: mkdocstrings-python; extra == "docs" Requires-Dist:
-mkdocs-jupyter; extra == "docs"
+Requires-Dist: pre-commit; extra == "test" Provides-Extra: docs Requires-Dist:
+mkdocs-material; extra == "docs" Requires-Dist: mkdocstrings; extra == "docs"
+Requires-Dist: mkdocs-section-index; extra == "docs" Requires-Dist:
+mkdocstrings-python; extra == "docs" Requires-Dist: mkdocs-jupyter; extra ==
+"docs" Provides-Extra: demo Requires-Dist: chainlit; extra == "demo"
             _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e___2_._0_-_b_l_u_e_._s_v_g_][https://
       img.shields.io/github/last-commit/parkervg/blendsql?color=green][https://
                                         img.shields.io/badge/PRs-Welcome-Green]
                                   [blendsql]
                                  SQL ð¤ LLMs
  CChheecckk oouutt oouurr _oo_nn_ll_ii_nn_ee_ _dd_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ffoorr aa mmoorree ccoommpprreehheennssiivvee oovveerrvviieeww.. Results
 from the paper are available [here](https://github.com/parkervg/blendsql/tree/
                     research-paper/research/paper-results)
 
-## Intro BlendSQL is a *superset of SQLite* for problem decomposition and
-hybrid question-answering with LLMs. As a result, we can *Blend* together... -
-ð¥¤ ...operations over heterogeneous data sources (e.g. tables, text, images)
-- ð¥¤ ...the structured & interpretable reasoning of SQL with the
-generalizable reasoning of LLMs It can be viewed as an inversion of the typical
-text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a SQL
-program. **Now, the user is given the control to oversee all calls (LLM + SQL)
-within a unified query language.** ![comparison](docs/img/comparison.jpg) For
-example, imagine we have the following tables. ### `w` | **date** | **rival** |
-**city** | **venue** | **score** | |----------|---------------------------|----
--------|-----------------------------|-----------| | 31 may | nsw waratahs |
-sydney | agricultural society ground | 11-0 | | 5 jun | northern districts |
-newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney |
-agricultural society ground | 21-2 | | 11 jun | western districts | bathurst |
-bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
-cricket ground | 23-10 | ### `documents` | **title** | **content** | |---------
------------------------|---------------------------------------------------| |
+### Features - Supports many DBMS ð¾ - Currently, SQLite and PostgreSQL are
+functional - more to come! - Easily extendable to [multi-modal usecases](./
+examples/vqa-ingredient.ipynb) ð¼ï¸ - Smart parsing optimizes what is passed
+to external functions ð§  - Traverses abstract syntax tree with [sqlglot]
+(https://github.com/tobymao/sqlglot) to minimize LLM function calls ð³ -
+Constrained decoding with [guidance](https://github.com/guidance-ai/guidance)
+ð - LLM function caching, built on [diskcache](https://grantjenks.com/docs/
+diskcache/) ð ## Intro BlendSQL is a *superset of SQLite* for problem
+decomposition and hybrid question-answering with LLMs. As a result, we can
+*Blend* together... - ð¥¤ ...operations over heterogeneous data sources (e.g.
+tables, text, images) - ð¥¤ ...the structured & interpretable reasoning of SQL
+with the generalizable reasoning of LLMs It can be viewed as an inversion of
+the typical text-to-SQL paradigm, where a user calls a LLM, and the LLM calls a
+SQL program. **Now, the user is given the control to oversee all calls (LLM +
+SQL) within a unified query language.** ![comparison](docs/img/comparison.jpg)
+For example, imagine we have the following tables. ### `w` | **date** |
+**rival** | **city** | **venue** | **score** | | -------- | -------------------
+------ | --------- | --------------------------- | --------- | | 31 may | nsw
+waratahs | sydney | agricultural society ground | 11-0 | | 5 jun | northern
+districts | newcastle | sports ground | 29-0 | | 7 jun | nsw waratahs | sydney
+| agricultural society ground | 21-2 | | 11 jun | western districts | bathurst
+| bathurst ground | 11-0 | | 12 jun | wallaroo & university nsw | sydney |
+cricket ground | 23-10 | ### `documents` | **title** | **content** | | --------
+---------------------- | ------------------------------------------------- | |
 sydney | sydney ( /ËsÉªdni/ ( listen ) sid-nee ) is the ... | | new south
 wales waratahs | the new south wales waratahs ( /ËwÉrÉtÉËz/ or ... | |
 sydney showground (moore park) | the former sydney showground ( moore park )
 at... | | sydney cricket ground | the sydney cricket ground ( scg ) is a sports
 ... | | newcastle, new south wales | the newcastle ( /ËnuËkÉËsÉl/ new-kah-
 sÉl ) met... | | bathurst, new south wales | bathurst /ËbÃ¦Î¸Érst/ is a city
 in the central t... | BlendSQL allows us to ask the following questions by
 injecting "ingredients", which are callable functions denoted by double curly
 brackets (`{{`, `}}`). The below examples work out of the box, but you are able
-to design your own ingredients as well! *What was the result of the game played
-120 miles west of Sydney?* ```sql SELECT * FROM w WHERE city = {{ LLMQA( 'Which
+to design your own ingredients as well! _What was the result of the game played
+120 miles west of Sydney?_ ```sql SELECT * FROM w WHERE city = {{ LLMQA( 'Which
 city is located 120 miles west of Sydney?', (SELECT * FROM documents WHERE
-documents MATCH 'sydney OR 120'), options='w::city' ) }} ``` *Which venues in
-Sydney saw more than 30 points scored?* ```sql SELECT DISTINCT venue FROM w
+documents MATCH 'sydney OR 120'), options='w::city' ) }} ``` _Which venues in
+Sydney saw more than 30 points scored?_ ```sql SELECT DISTINCT venue FROM w
 WHERE city = 'sydney' AND {{ LLMMap( 'More than 30 total points?', 'w::score' )
-}} = TRUE ``` *Show all NSW Waratahs games and a description of the team.*
+}} = TRUE ``` _Show all NSW Waratahs games and a description of the team._
 ```sql SELECT date, rival, score, documents.content AS "Team Description" FROM
 w JOIN {{ LLMJoin( left_on='documents::title', right_on='w::rival' ) }} WHERE
 rival = 'nsw waratahs' ``` ### More Examples from Popular QA Datasets
 _HH_yy_bb_rr_ii_dd_QQ_AA_ For this setting, our database contains 2 tables: a table from
 Wikipedia `w`, and a collection of unstructured Wikipedia articles in the table
-`documents`. *What is the state flower of the smallest state by area ?* ```sql
+`documents`. _What is the state flower of the smallest state by area ?_ ```sql
 SELECT "common name" AS 'State Flower' FROM w WHERE state = {{ LLMQA( 'Which is
 the smallest state by area?', (SELECT title, content FROM documents),
-options='w::state' ) }} ``` *Who were the builders of the mosque in Herat with
-fire temples ?* ```sql {{ LLMQA( 'Name of the builders?', ( SELECT title AS
-'Building', content FROM documents WHERE title = {{ LLMQA( 'Align the name to
-the correct title.', (SELECT name FROM w WHERE city = 'herat' AND remarks LIKE
-'%fire temple%'), options='documents::title' ) }} ) ) }} ``` *What is the
-capacity of the venue that was named in honor of Juan Antonio Samaranch in 2010
-after his death ?* ```sql SELECT capacity FROM w WHERE venue = {{ LLMQA( 'Which
-venue is named in honor of Juan Antonio Samaranch?', (SELECT title AS 'Venue',
-content FROM documents), options='w::venue' ) }} ```
+options='w::state' ) }} ``` _Who were the builders of the mosque in Herat with
+fire temples ?_ ```sql {{ LLMQA( 'Who were the builders of the mosque?',
+( SELECT documents.title AS 'Building', documents.content FROM documents JOIN {
+{ LLMJoin( left_on='w::name', right_on='documents::title' ) }} WHERE w.city =
+'herat' AND w.remarks LIKE '%fire temple%' ) ) }} ``` _What is the capacity of
+the venue that was named in honor of Juan Antonio Samaranch in 2010 after his
+death ?_ ```sql SELECT capacity FROM w WHERE venue = {{ LLMQA( 'Which venue is
+named in honor of Juan Antonio Samaranch?', (SELECT title AS 'Venue', content
+FROM documents), options='w::venue' ) }} ```
 _OO_TT_TT_--_QQ_AA_ Unlike HybridQA, these questions are open-domain, where we don't know in
 advance where the answer of a given open question appears in a passage or a
 table. As a result, we need to play the role of both the retriever (to select
 relevant context) and reader (to read from relevant contexts and return the
 given answer). As the underlying database consists of 400K tables and 5M
 documents, it's important to set `LIMIT` clauses appropriately to ensure
 reasonable execution times. The examples below also demonstrate how BlendSQL
 unpacks [CTE statements](https://www.sqlite.org/lang_with.html) to ensure we
-only pass necessary data into the BlendSQL ingredient calls. *When was the
-third highest paid Rangers F.C . player born ?* ```sql {{ LLMQA( 'When was the
+only pass necessary data into the BlendSQL ingredient calls. _When was the
+third highest paid Rangers F.C . player born ?_ ```sql {{ LLMQA( 'When was the
 Rangers Player born?', ( WITH t AS ( SELECT player FROM ( SELECT * FROM "./List
 of Rangers F.C. records and statistics (0)" UNION ALL SELECT * FROM "./List of
 Rangers F.C. records and statistics (1)" ) ORDER BY trim(fee, 'Â£') DESC LIMIT
 1 OFFSET 2 ), d AS ( SELECT * FROM documents JOIN t WHERE documents MATCH
 t.player || ' OR rangers OR fc' ORDER BY rank LIMIT 5 ) SELECT d.content,
-t.player AS 'Rangers Player' FROM d JOIN t ) ) }} ``` *In which Track Cycling
+t.player AS 'Rangers Player' FROM d JOIN t ) ) }} ``` _In which Track Cycling
 World Championships event was the person born in Matanzas , Cuba ranked highest
-?* ```sql {{ LLMQA( 'In what event was the cyclist ranked highest?', ( SELECT *
+?_ ```sql {{ LLMQA( 'In what event was the cyclist ranked highest?', ( SELECT *
 FROM ( SELECT * FROM "./Cuba at the UCI Track Cycling World Championships (2)"
 ) as w WHERE w.name = {{ LLMQA( "Which cyclist was born in Matanzas, Cuba?",
 ( SELECT * FROM documents WHERE documents MATCH 'matanzas AND (cycling OR track
 OR born)' ORDER BY rank LIMIT 3 ), options="w::name" ) }} ), options='w::event'
-) }} ``` *Who is the director the Togolese film that was a 30 minute film that
-was shot in 16mm ?* ```sql SELECT director FROM "./List of African films (4)"
+) }} ``` _Who is the director the Togolese film that was a 30 minute film that
+was shot in 16mm ?_ ```sql SELECT director FROM "./List of African films (4)"
 as w WHERE title = {{ LLMQA( 'What is the name of the Togolese film that was 30
 minutes and shot in 16mm?', (SELECT * FROM documents WHERE documents MATCH
 'togolese OR 30 OR 16mm OR film' ORDER BY rank LIMIT 5), options='w::title' )
 }} ```
 _FF_EE_VV_EE_RR_OO_UU_SS_ Here, we deal not with questions, but truth claims given a context of
 unstructured and structured data. These claims should be judged as "SUPPORTS"
 or "REFUTES". Using BlendSQL, we can formulate this determination of truth as a
-function over facts. *Oyedaea is part of the family Asteraceae in the order
-Asterales.* ```sql SELECT EXISTS ( SELECT * FROM w0 WHERE "family:" =
-'asteraceae' AND "order:" = 'asterales' ) ``` *The 2006-07 San Jose Sharks
+function over facts. _Oyedaea is part of the family Asteraceae in the order
+Asterales._ ```sql SELECT EXISTS ( SELECT * FROM w0 WHERE "family:" =
+'asteraceae' AND "order:" = 'asterales' ) ``` _The 2006-07 San Jose Sharks
 season, the 14th season of operation (13th season of play) for the National
-Hockey League (NHL) franchise, scored the most points in the Pacific Division.*
+Hockey League (NHL) franchise, scored the most points in the Pacific Division._
 ```sql SELECT ( {{ LLMValidate( 'Is the Sharks 2006-07 season the 14th season
 (13th season of play)?', (SELECT * FROM documents) ) }} ) AND ( SELECT (SELECT
 filledcolumnname FROM w0 ORDER BY pts DESC LIMIT 1) = 'san jose sharks' ) ```
-*Saunders College of Business, which is accredited by the Association to
+_Saunders College of Business, which is accredited by the Association to
 Advance Collegiate Schools of Business International, is one of the colleges of
 Rochester Institute of Technology established in 1910 and is currently under
-the supervision of Dean Jacqueline R. Mozrall.* ```sql SELECT EXISTS( SELECT *
+the supervision of Dean Jacqueline R. Mozrall._ ```sql SELECT EXISTS( SELECT *
 FROM w0 WHERE "parent institution" = 'rochester institute of technology' AND
 "established" = '1910' AND "dean" = 'jacqueline r. mozrall' ) AND ( {
 { LLMValidate( 'Is Saunders College of Business (SCB) accredited by the
 Association to Advance Collegiate Schools of Business International (AACSB)?',
 (SELECT * FROM documents) ) }} ) ```
-## Table of Contents * [Install](#install) * [Quickstart](#quickstart) * [FAQ]
-(#faq) * [Documentation](#documentation) * [Execute a BlendSQL Query](#execute-
-a-blendsql-query) * [Smoothie](#smoothie) * [Ingredients](#ingredients) *
-[MapIngredient](#mapingredient) * [QAIngredient](#qaingredient) * [Constrained
-Decoding with 'options'](#constrained-decoding-with-options) * [JoinIngredient]
-(#joiningredient) * [StringIngredient](#stringingredient) * [LLMs](#llms) *
-[Databases](#databases) * [Appendix](#appendix) ### Features - Smart parsing
-optimizes what is passed to external functions ð§  - Traverses abstract syntax
-tree with [sqlglot](https://github.com/tobymao/sqlglot) to minimize LLM
-function calls ð³ - LLM function caching, built on [diskcache](https://
-grantjenks.com/docs/diskcache/) ð - Constrained decoding with [guidance]
-(https://github.com/guidance-ai/guidance) ð For a technical walkthrough of
+## Table of Contents - [Install](#install) - [Quickstart](#quickstart) - [FAQ]
+(#faq) - [Documentation](#documentation) - [Execute a BlendSQL Query](#execute-
+a-blendsql-query) - [Smoothie](#smoothie) - [Ingredients](#ingredients) -
+[MapIngredient](#mapingredient) - [QAIngredient](#qaingredient) - [Constrained
+Decoding with 'options'](#constrained-decoding-with-options) - [JoinIngredient]
+(#joiningredient) - [StringIngredient](#stringingredient) - [Parsing Natural
+Language to BlendSQL](#parsing-natural-language-to-blendsql) - [LLMs](#llms) -
+[Databases](#databases) - [Appendix](#appendix) For a technical walkthrough of
 how a BlendSQL query is executed, check out [technical_walkthrough.md](./docs/
 technical_walkthrough.md). ## Install ``` pip install blendsql ``` ##
-Quickstart ```python from blendsql import blend, LLMQA, LLMMap from blendsql.db
-import SQLite from blendsql.models import OpenaiLLM blendsql = """ SELECT
-merchant FROM transactions WHERE {{LLMMap('is this a pizza shop?',
-'transactions::merchant')}} = TRUE AND parent_category = 'Food' """ # Make our
+Quickstart ```python from blendsql import blend, LLMQA from blendsql.db import
+SQLite from blendsql.models import OpenaiLLM from blendsql.utils import
+fetch_from_hub blendsql = """ SELECT * FROM w WHERE city = {{ LLMQA( 'Which
+city is located 120 miles west of Sydney?', (SELECT * FROM documents WHERE
+documents MATCH 'sydney OR 120'), options='w::city' ) }} """ # Make our
 smoothie - the executed BlendSQL script smoothie = blend( query=blendsql,
-blender=OpenaiLLM("gpt-3.5-turbo-0613"), ingredients={LLMMap, LLMQA}, db=SQLite
-(db_path="transactions.db"), verbose=True ) ``` ### FAQ #### Why not just
+db=SQLite(fetch_from_hub
+("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+blender=OpenaiLLM("gpt-3.5-turbo"), ingredients={LLMQA}, ) print(smoothie.df)
+print(smoothie.meta.prompts) ``` ### FAQ #### How does BlendSQL execute a
+query? > BlendSQL handles traversal of the SQL AST and creation of temporary
+tables to execute a given query. > This allows BlendSQL to be DBMS-agnostic,
+and extendable into both SQLite, PostgreSQL, and other DBMS. #### Why not just
 implement BlendSQL as a [user-defined function in SQLite](https://
 www.sqlite.org/c3ref/c_deterministic.html#sqlitedeterministic)? > LLMs are
 expensive, both in terms of $ cost and compute time. When applying them to
 SQLite databases, we want to take special care in ensuring we're not applying
 them to contexts where they're not required. > This is [not easily achievable
 with UDFs](https://sqlite.org/forum/info/
 649ad4c62fd4b4e8cb5d6407107b8c8a9a0afaaf95a87805e5a8403a79e6616c), even when
 marked as a [deterministic function](https://www.sqlite.org/c3ref/
 c_deterministic.html#sqlitedeterministic). > > BlendSQL is specifically
 designed to enforce an order-of-operations that 1) prioritizes vanilla SQL
 operations first, and 2) caches results from LLM ingredients so they don't need
-to be recomputed. > For example: > ```sql > SELECT {{LLMMap('What state is this
-NBA team from?', 'w::team')} FROM w > WHERE num_championships > 3 > ORDER BY {
-{LLMMap('What state is this NBA team from?', 'w::team')} > > ``` > BlendSQL
-makes sure to only pass those `team` values from rows which satisfy the
-condition `num_championship > 3` to the LLM. Additionally, since we assume the
-function is deterministic, we make a single LLM call and cache the results,
+to be recomputed. > For example: > > ```sql > SELECT {{LLMMap('What state is
+this NBA team from?', 'w::team')} FROM w > WHERE num_championships > 3 > ORDER
+BY {{LLMMap('What state is this NBA team from?', 'w::team')} > > ``` > >
+BlendSQL makes sure to only pass those `team` values from rows which satisfy
+the condition `num_championship > 3` to the LLM. Additionally, since we assume
+the function is deterministic, we make a single LLM call and cache the results,
 despite the ingredient function being used twice. #### So I get how to write
 BlendSQL queries. But why would I use this over vanilla SQLite? > Certain
 ingredients, like [LLMJoin](#joiningredient), will likely give seasoned SQL
 experts a headache at first. However, BlendSQL's real strength comes from it's
-use as an *intermediate representation for reasoning over structured +
-unstructured with LLMs*. Some examples of this can be found above [here](#more-
+use as an _intermediate representation for reasoning over structured +
+unstructured with LLMs_. Some examples of this can be found above [here](#more-
 examples-from-popular-qa-datasets).
 ===============================================================================
 ### Citation ```bibtex @article{glenn2024blendsql, title={BlendSQL: A Scalable
 Dialect for Unifying Hybrid Question Answering in Relational Algebra}, author=
 {Parker Glenn and Parag Pravin Dakle and Liang Wang and Preethi Raghavan},
 year={2024}, eprint={2402.17882}, archivePrefix={arXiv}, primaryClass={cs.CL} }
-``` # Documentation > [!WARNING] > WIP, will be updated ## Execute a BlendSQL
-Query The `blend()` function is used to execute a BlendSQL query against a
-database and return the final result, in addition to the intermediate reasoning
-steps taken. ::: blendsql.blendsql.blend handler: python ```python from
-blendsql import blend, LLMMap, LLMQA, LLMJoin from blendsql.db import SQLite
-from blendsql.models import OpenaiLLM blendsql = """ SELECT * FROM w WHERE city
-= {{ LLMQA( 'Which city is located 120 miles west of Sydney?', (SELECT * FROM
-documents WHERE documents MATCH 'sydney OR 120'), options='w::city' ) }} """ db
-= SQLite(db_path) smoothie = blend( query=blendsql, db=db, ingredients={LLMMap,
-LLMQA, LLMJoin}, blender=AzureOpenaiLLM("gpt-4"), # Optional args below
-infer_gen_constraints=True, silence_db_exec_errors=False, verbose=True,
-blender_args={ "few_shot": True, "temperature": 0.01 } ) ``` ### Smoothie The
-[smoothie.py](./blendsql/_smoothie.py) object defines the output of an executed
-BlendSQL script. ```python @dataclass class Smoothie: df: pd.DataFrame meta:
-SmoothieMeta @dataclass class SmoothieMeta: process_time_seconds: float
-num_values_passed: int # Number of values passed to a Map/Join/QA ingredient
-num_prompt_tokens: int # Number of prompt tokens (counting user and assistant,
-i.e. input/output) prompts: List[str] # Log of prompts submitted to model
-example_map_outputs: List[Any] # outputs from a Map ingredient, for debugging
-ingredients: List[Ingredient] query: str db_path: str contains_ingredient: bool
-= True def blend(*args, **kwargs) -> Smoothie: ... ```
+``` # Documentation ## Databases Since BlendSQL relies on the package [sqlglot]
+(https://github.com/tobymao/sqlglot) for query optimization (which supports a
+[wide variety of SQL dialects](https://github.com/tobymao/sqlglot/blob/main/
+sqlglot/dialects/__init__.py)) and the notion of [temporary tables](https://
+en.wikibooks.org/wiki/Structured_Query_Language/Temporary_Table), it can easily
+integrate with many different SQL dialects. Currently, the following are
+supported. ### SQLite A SQLite database connection. Can be initialized via a
+path to the database file. Example: ```python from blendsql.db import SQLite db
+= SQLite("./path/to/database.db") ``` ### PostgreSQL A PostgreSQL database
+connection. Can be initialized via the SQLAlchemy input string. https://
+docs.sqlalchemy.org/en/20/core/engines.html#postgresql Example: ```python from
+blendsql.db import PostgreSQL db = PostgreSQL("user:password@localhost/
+mydatabase") ``` ## Execute a BlendSQL Query The `blend()` function is used to
+execute a BlendSQL query against a database and return the final result, in
+addition to the intermediate reasoning steps taken. ```python from blendsql
+import blend, LLMQA from blendsql.db import SQLite from blendsql.models import
+OpenaiLLM from blendsql.utils import fetch_from_hub blendsql = """ SELECT *
+FROM w WHERE city = {{ LLMQA( 'Which city is located 120 miles west of
+Sydney?', (SELECT * FROM documents WHERE documents MATCH 'sydney OR 120'),
+options='w::city' ) }} """ # Make our smoothie - the executed BlendSQL script
+smoothie = blend( query=blendsql, db=SQLite(fetch_from_hub
+("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")),
+blender=OpenaiLLM("gpt-3.5-turbo"), ingredients={LLMQA}, ) print(smoothie.df)
+print(smoothie.meta.prompts) ``` ### Smoothie The [smoothie.py](./blendsql/
+_smoothie.py) object defines the output of an executed BlendSQL script.
+```python @dataclass class Smoothie: df: pd.DataFrame meta: SmoothieMeta
+@dataclass class SmoothieMeta: process_time_seconds: float num_values_passed:
+int # Number of values passed to a Map/Join/QA ingredient num_prompt_tokens:
+int # Number of prompt tokens (counting user and assistant, i.e. input/output)
+prompts: List[str] # Log of prompts submitted to model example_map_outputs:
+List[Any] # outputs from a Map ingredient, for debugging ingredients: List
+[Ingredient] query: str db_path: str contains_ingredient: bool = True def blend
+(*args, **kwargs) -> Smoothie: ... ```
 ===============================================================================
 ## Ingredients ![ingredients](docs/img/ingredients.jpg) Ingredients are at the
 core of a BlendSQL script. They are callable functions that perform one the
 task paradigms defined in [ingredient.py](./blendsql/ingredients/
 ingredient.py). At their core, these are not a new concept. [User-defined
 functions (UDFs)](https://docs.databricks.com/en/udf/index.html), or
 [Application-Defined Functions in SQLite](https://www.sqlite.org/appfunc.html)
@@ -213,15 +236,15 @@
 ingredient types are valid. ### MapIngredient This type of ingredient applies a
 function on a given table/column pair to create a new column containing the
 function output. For example, take the following query. ```sql SELECT merchant
 FROM transactions WHERE {{LLMMap('Is this a pizza shop?', 'transactions::
 merchant')}} = TRUE ``` `LLMMap` is one of our builtin MapIngredients. For each
 of the distinct values in the "merchant" column of the "transactions" table, it
 will create a column containing the function output. | merchant | Is this a
-pizza shop? | |----------|-----------------------| | Domino's | 1 | | Safeway |
+pizza shop? | | -------- | --------------------- | | Domino's | 1 | | Safeway |
 0 | | Target | 0 | The temporary table shown above is then combined with the
 original "transactions" table with an `INNER JOIN` on the "merchant" column.
 ### JoinIngredient Handles the logic of semantic `JOIN` clauses between tables.
 For example: ```sql SELECT Capitals.name, State.name FROM Capitals JOIN {
 { LLMJoin( 'Align state to capital', left_on='States::name',
 right_on='Capitals::name' ) }} ``` The above example hints at a database schema
 that would make [E.F Codd](https://en.wikipedia.org/wiki/Edgar_F._Codd) very
@@ -229,29 +252,29 @@
 foreign key to join the two? BlendSQL was built to interact with tables "in-
 the-wild", and many (such as those on Wikipedia) do not have these convenient
 properties of well-designed relational models. For this reason, we can leverage
 the internal knowledge of a pre-trained LLM to do the `JOIN` operation for us.
 ### QAIngredient Sometimes, simply selecting data from a given database is not
 enough to sufficiently answer a user's question. The `QAIngredient` is designed
 to return data of variable types, and is best used in cases when we either
-need: 1) Unstructured, free-text responses ("Give me a summary of all my
-spending in coffe") 2) Complex, unintuitive relationships extracted from table
+need: 1. Unstructured, free-text responses ("Give me a summary of all my
+spending in coffe") 2. Complex, unintuitive relationships extracted from table
 subsets ("How many consecutive days did I spend in coffee?") The following
 query demonstrates usage of the builtin `LLMQA` ingredient. ```sql {{ LLMQA
 ( 'How many consecutive days did I buy stocks in Financials?', ( SELECT
 account_history."Run Date", account_history.Symbol, constituents."Sector" FROM
 account_history LEFT JOIN constituents ON account_history.Symbol =
 constituents.Symbol WHERE Sector = "Financials" ORDER BY "Run Date" LIMIT 5 ) )
 }} ``` This is slightly more complicated than the rest of the ingredients.
 Behind the scenes, we wrap the call to `LLMQA` in a trivial `CASE` clause,
 ensuring that the ingredient's output gets returned. ```sql SELECT CASE WHEN
 FALSE THEN FALSE WHEN TRUE then {{QAIngredient}} END ``` The LLM gets both the
 question asked, alongside the subset of the SQL database fetched by our
-subquery. | **"Run Date"** | **Symbol** | **Sector** | |----------------|------
-------|------------| | 2022-01-14 | HBAN | Financials | | 2022-01-20 | AIG |
+subquery. | **"Run Date"** | **Symbol** | **Sector** | | -------------- | -----
+----- | ---------- | | 2022-01-14 | HBAN | Financials | | 2022-01-20 | AIG |
 Financials | | 2022-01-24 | AIG | Financials | | 2022-01-24 | NTRS | Financials
 | | 2022-01-25 | HBAN | Financials | From examining this table, we see that we
 bought stocks in the Financials sector 2 consecutive days (2022-01-24, and
 2022-01-25). The LLM answers the question in an end-to-end manner, returning
 the result `2`. The `QAIngredient` can be used as a standalone end-to-end QA
 tool, or as a component within a larger BlendSQL query. For example, the
 BlendSQL query below translates to the valid (but rather confusing) question:
@@ -292,25 +315,37 @@
 which the relative phrase "q2" most likely refers to. We do not create any new
 tables or perform any joins with a StringIngredient; instead, we simply get the
 following SQL query. > [!NOTE] > The below SQL interpretation of the `DT`
 function assumes we're calling it in December, 2022. The phrase 'q2' will be
 interpreted differently in, say, March 1998. ```sql SELECT merchant FROM
 transactions WHERE date > '2022-09-30' AND date < '2022-12-01' ```
 ===============================================================================
-## LLMs
-===============================================================================
-## Databases
+## Parsing Natural Language to BlendSQL ```python from blendsql import
+nl_to_blendsql, LLMMap from blendsql.models import TransformersLLM from
+blendsql.db import SQLite from blendsql.utils import fetch_from_hub model =
+TransformersLLM("Qwen/Qwen1.5-0.5B") db = SQLite(fetch_from_hub
+("1884_New_Zealand_rugby_union_tour_of_New_South_Wales_1.db")) query =
+nl_to_blendsql( question="Which venues in Sydney saw more than 30 points
+scored?", model=model, ingredients={LLMMap}, serialized_db=db.to_serialized
+(num_rows=3, use_tables=["w", "documents"]), verbose=True,
+max_grammar_corrections=5, ) ``` ### Grammar-Based Correction If you use the
+grammar prompting feature of BlendSQL, please cite the original grammar
+prompting paper below. ```bibtex @article{wang2024grammar, title={Grammar
+prompting for domain-specific language generation with large language models},
+author={Wang, Bailin and Wang, Zi and Wang, Xuezhi and Cao, Yuan and A Saurous,
+Rif and Kim, Yoon}, journal={Advances in Neural Information Processing
+Systems}, volume={36}, year={2024} } ```
 ===============================================================================
 ### Appendix #### Run Line Profiling First uncomment `@profile` above `blend()`
 in `blendsql.py`. Make sure you've run `pip install line_profiler` first. This
 installs the tool here: https://github.com/pyutils/line_profiler
 `PYTHONPATH=$PWD:$PYTHONPATH kernprof -lv examples/benchmarks/with_blendsql.py`
 #### Benchmarks The below benchmarks were done on my local M1 Macbook Pro. by
 running the scripts found in `examples/benchmarks`. 'Lines of Code' is a rough
 estimate of the user-written code for each usecase. | **Name** |
-**Description** | **Runtime/s (Across 10 runs)** | **Lines of Code** | |-------
------------------------|-------------------------------------------------------
-----------|-------------------------------------------------|------------------
--| | BlendSQL | |5.685 +/- 0.930 | 9 | | SQL + LLM Calls | Filtering what we
-can with SQL, then running LLM calls. | 9.083 +/- 2.061 | 106 | | Naive SQL +
-LLM Calls | Runing LLM calls on entire table, regardless of SQL conditions. |
-64.809 +/- 6.225 | 106 |
+**Description** | **Runtime/s (Across 10 runs)** | **Lines of Code** | | ------
+--------------- | -------------------------------------------------------------
+-- | ------------------------------ | ----------------- | | BlendSQL | | 5.685
++/- 0.930 | 9 | | SQL + LLM Calls | Filtering what we can with SQL, then
+running LLM calls. | 9.083 +/- 2.061 | 106 | | Naive SQL + LLM Calls | Runing
+LLM calls on entire table, regardless of SQL conditions. | 64.809 +/- 6.225 |
+106 |
```

### Comparing `blendsql-0.0.141/pyproject.toml` & `blendsql-0.0.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.141/setup.py` & `blendsql-0.0.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,52 +24,53 @@
         "console_scripts": ["blendsql=blendsql.blend_cli:main"],
     },
     name="blendsql",
     version=find_version("blendsql", "__init__.py"),
     url="https://github.com/parkervg/blendsql",
     author="Parker Glenn",
     author_email="parkervg5@gmail.com",
-    description="Orchestrate SQLite logic and LLM reasoning within a unified dialect.",
+    description="Query language to blend SQL logic and LLM reasoning across multi-modal data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
     packages=find_packages(exclude=["examples", "research", "img"]),
+    data_files=["blendsql/grammars/_cfg_grammar.lark"],
     install_requires=[
         "guidance>=0.1.0",
         "pyparsing==3.1.1",
-        "pandas>=2.0.0",
+        "pandas==1.5.3",
         "bottleneck>=1.3.6",
         "python-dotenv==1.0.1",
         "sqlglot==18.13.0",
+        "sqlalchemy>=2.0.0",
         "platformdirs",
-        "pre-commit",
         "attrs",
         "tqdm",
-        "dateparser",
         "colorama",
-        "fiscalyear",
         "tabulate",
         "typeguard",
     ],
     extras_require={
+        "nl_to_blendsql": ["exrex", "lark"],
         "research": [
             "datasets==2.16.1",
             "nltk",
             "wikiextractor",
             "rouge_score",
             "rapidfuzz",
             "records",
             "SQLAlchemy",
             "recognizers-text",
             "recognizers-text-suite",
             "emoji==1.7.0",
         ],
-        "test": ["pytest", "huggingface_hub"],
+        "test": ["pytest", "huggingface_hub", "pre-commit"],
         "docs": [
             "mkdocs-material",
             "mkdocstrings",
             "mkdocs-section-index",
             "mkdocstrings-python",
             "mkdocs-jupyter",
         ],
+        "demo": ["chainlit"],
     },
 )
```

### Comparing `blendsql-0.0.141/tests/test_generic_blendsql.py` & `blendsql-0.0.15/tests/test_generic_blendsql.py`

 * *Files identical despite different names*

### Comparing `blendsql-0.0.141/tests/test_model.py` & `blendsql-0.0.15/tests/test_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,19 +62,19 @@
 
 
 def test_simple_cache():
     a = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)[
         "uuid"
     ]
 
-    b = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)[
-        "uuid"
-    ]
+    model_b = DummyModel(MODEL_A)
+    b = model_b.predict(program=DummyProgram, question=TEST_QUESTION)["uuid"]
 
     assert a == b
+    assert model_b.num_llm_calls == 0
 
 
 def test_different_models():
     a = DummyModel(MODEL_A).predict(program=DummyProgram, question=TEST_QUESTION)[
         "uuid"
     ]
 
@@ -113,19 +113,19 @@
     global TEST_GLOBAL
     TEST_GLOBAL = "This is the same value"
     a = DummyModel(MODEL_A).predict(
         program=DummyProgramWithGlobal, question=TEST_QUESTION
     )["uuid"]
 
     TEST_GLOBAL = "This is the same value"
-    b = DummyModel(MODEL_A).predict(
-        program=DummyProgramWithGlobal, question=TEST_QUESTION
-    )["uuid"]
+    model_b = DummyModel(MODEL_A)
+    b = model_b.predict(program=DummyProgramWithGlobal, question=TEST_QUESTION)["uuid"]
 
     assert a == b
+    assert model_b.num_llm_calls == 0
 
 
 def test_different_global_vars():
     global TEST_GLOBAL
     TEST_GLOBAL = "This is one value"
     a = DummyModel(MODEL_A).predict(
         program=DummyProgramWithGlobal, question=TEST_QUESTION
@@ -133,7 +133,19 @@
 
     TEST_GLOBAL = "This is a different value"
     b = DummyModel(MODEL_A).predict(
         program=DummyProgramWithGlobal, question=TEST_QUESTION
     )["uuid"]
 
     assert a != b
+
+
+def test_with_set_vars():
+    a = DummyModel(MODEL_A).predict(
+        program=DummyProgram, question=TEST_QUESTION, random_set={"a", "b", "c"}
+    )["uuid"]
+
+    b = DummyModel(MODEL_A).predict(
+        program=DummyProgram, question=TEST_QUESTION, random_set={"b", "c", "a"}
+    )["uuid"]
+
+    assert a == b
```

### Comparing `blendsql-0.0.141/tests/test_multi_table_blendsql.py` & `blendsql-0.0.15/tests/test_multi_table_blendsql.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,26 +37,26 @@
     """
     blendsql = """
     SELECT Symbol, "North America", "Japan" FROM geographic
         WHERE geographic.Symbol IN (
             SELECT Symbol FROM portfolio
             WHERE {{starts_with('A', 'portfolio::Description')}} = 1
             AND portfolio.Symbol in (
-                SELECT Symbol FROM constituents 
+                SELECT Symbol FROM constituents
                 WHERE constituents.Sector = 'Information Technology'
             )
         )
     """
     sql = """
     SELECT Symbol, "North America", "Japan" FROM geographic
         WHERE geographic.Symbol IN (
             SELECT Symbol FROM portfolio
             WHERE portfolio.Description LIKE "A%"
             AND Symbol in (
-                SELECT Symbol FROM constituents 
+                SELECT Symbol FROM constituents
                 WHERE constituents.Sector = 'Information Technology'
             )
         )
     """
     smoothie = blend(
         query=blendsql,
         db=db,
@@ -145,26 +145,26 @@
     """
     )
     assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
 
 
 def test_select_multi_exec(db, ingredients):
     blendsql = """
-    SELECT "Run Date", Account, Action, ROUND("Amount ($)", 2) AS 'Total Dividend Payout ($$)', Name 
-        FROM account_history 
-        LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol 
+    SELECT "Run Date", Account, Action, ROUND("Amount ($)", 2) AS 'Total Dividend Payout ($$)', Name
+        FROM account_history
+        LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
         WHERE constituents.Sector = {{select_first_sorted(options='constituents::Sector')}}
         AND lower(account_history.Action) like "%dividend%"
     """
     sql = """
     SELECT "Run Date", Account, Action, ROUND("Amount ($)", 2) AS 'Total Dividend Payout ($$)', Name
         FROM account_history
         LEFT JOIN constituents ON account_history.Symbol = constituents.Symbol
         WHERE constituents.Sector = (
-            SELECT Sector FROM constituents 
+            SELECT Sector FROM constituents
             ORDER BY Sector LIMIT 1
         )
         AND lower(account_history.Action) like "%dividend%"
     """
     smoothie = blend(
         query=blendsql,
         db=db,
@@ -172,27 +172,27 @@
     )
     sql_df = db.execute_query(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
 
 
 def test_complex_multi_exec(db, ingredients):
     blendsql = """
-    SELECT DISTINCT constituents.Symbol as Symbol FROM constituents
-    LEFT JOIN fundamentals ON constituents.Symbol = fundamentals.FPS_SYMBOL
+    SELECT DISTINCT constituents.Symbol, Action FROM constituents
+    LEFT JOIN account_history ON constituents.Symbol = account_history.Symbol
     LEFT JOIN portfolio on constituents.Symbol = portfolio.Symbol
-    WHERE fundamentals.MARKET_DAY_DT > '2023-02-23'
+    WHERE account_history."Run Date" > '2021-02-23'
     AND ({{get_length('n_length', 'constituents::Name')}} > 3 OR {{starts_with('A', 'portfolio::Symbol')}})
     AND portfolio.Symbol IS NOT NULL
-    ORDER BY {{get_length('n_length', 'constituents::Name')}} LIMIT 1
+    ORDER BY LENGTH(constituents.Name) LIMIT 1
     """
     sql = """
-    SELECT DISTINCT constituents.Symbol as Symbol FROM constituents
-    LEFT JOIN fundamentals ON constituents.Symbol = fundamentals.FPS_SYMBOL
+    SELECT DISTINCT constituents.Symbol, Action FROM constituents
+    LEFT JOIN account_history ON constituents.Symbol = account_history.Symbol
     LEFT JOIN portfolio on constituents.Symbol = portfolio.Symbol
-    WHERE fundamentals.MARKET_DAY_DT > '2023-02-23'
+    WHERE account_history."Run Date" > '2021-02-23'
     AND (LENGTH(constituents.Name) > 3 OR portfolio.Symbol LIKE "A%")
     AND portfolio.Symbol IS NOT NULL
     ORDER BY LENGTH(constituents.Name) LIMIT 1
     """
     smoothie = blend(
         query=blendsql,
         db=db,
@@ -200,34 +200,33 @@
     )
     sql_df = db.execute_query(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
 
 
 def test_complex_not_qualified_multi_exec(db, ingredients):
     """Same test as test_complex_multi_exec(), but without qualifying columns if we don't need to.
-    i.e. MARKET_DAY_DT and Symbol don't have tablename preceding them.
     commit fefbc0a
     """
     blendsql = """
-    SELECT DISTINCT constituents.Symbol as Symbol FROM constituents
-    LEFT JOIN fundamentals ON constituents.Symbol = fundamentals.FPS_SYMBOL
+    SELECT DISTINCT constituents.Symbol, Action FROM constituents
+    LEFT JOIN account_history ON constituents.Symbol = account_history.Symbol
     LEFT JOIN portfolio on constituents.Symbol = portfolio.Symbol
-    WHERE MARKET_DAY_DT > '2023-02-23'
+    WHERE "Run Date" > '2021-02-23'
     AND ({{get_length('n_length', 'constituents::Name')}} > 3 OR {{starts_with('A', 'portfolio::Symbol')}})
-    AND Symbol IS NOT NULL
-    ORDER BY {{get_length('n_length', 'constituents::Name')}} LIMIT 1
+    AND portfolio.Symbol IS NOT NULL
+    ORDER BY LENGTH(Name) LIMIT 1
     """
     sql = """
-    SELECT DISTINCT constituents.Symbol as Symbol FROM constituents
-    LEFT JOIN fundamentals ON constituents.Symbol = fundamentals.FPS_SYMBOL
+    SELECT DISTINCT constituents.Symbol, Action FROM constituents
+    LEFT JOIN account_history ON constituents.Symbol = account_history.Symbol
     LEFT JOIN portfolio on constituents.Symbol = portfolio.Symbol
-    WHERE MARKET_DAY_DT > '2023-02-23'
+    WHERE "Run Date" > '2021-02-23'
     AND (LENGTH(constituents.Name) > 3 OR portfolio.Symbol LIKE "A%")
-    AND Symbol IS NOT NULL
-    ORDER BY LENGTH(constituents.Name) LIMIT 1
+    AND portfolio.Symbol IS NOT NULL
+    ORDER BY LENGTH(Name) LIMIT 1
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
     sql_df = db.execute_query(sql)
@@ -238,15 +237,15 @@
     blendsql = """
     SELECT Account, Quantity FROM returns
     JOIN {{
         do_join(
             left_on='account_history::Account',
             right_on='returns::Annualized Returns'
         )
-    }} 
+    }}
     """
     sql = """
     SELECT Account, Quantity FROM returns JOIN account_history ON returns."Annualized Returns" = account_history."Account"
     """
     smoothie = blend(
         query=blendsql,
         db=db,
@@ -255,15 +254,15 @@
     sql_df = db.execute_query(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
 
 
 def test_qa_equals_multi_exec(db, ingredients):
     blendsql = """
     SELECT Action FROM account_history
-    WHERE Symbol = {{return_aapl()}} 
+    WHERE Symbol = {{return_aapl()}}
     """
     sql = """
     SELECT Action FROM account_history
     WHERE Symbol = "AAPL"
     """
     smoothie = blend(
         query=blendsql,
@@ -334,15 +333,15 @@
 
 def test_cte_qa_multi_exec(db, ingredients):
     blendsql = """
    {{
         get_table_size(
             (
                 WITH a AS (
-                    SELECT * FROM (SELECT DISTINCT * FROM portfolio) as w 
+                    SELECT * FROM (SELECT DISTINCT * FROM portfolio) as w
                         WHERE {{starts_with('F', 'w::Symbol')}} = TRUE
                 ) SELECT * FROM a WHERE LENGTH(a.Symbol) > 2
             )
         )
     }}
     """
     sql = """
@@ -369,15 +368,15 @@
 
 def test_cte_qa_named_multi_exec(db, ingredients):
     blendsql = """
    {{
         get_table_size(
             (
                 WITH a AS (
-                    SELECT * FROM (SELECT DISTINCT * FROM portfolio) as w 
+                    SELECT * FROM (SELECT DISTINCT * FROM portfolio) as w
                         WHERE {{starts_with('F', 'w::Symbol')}} = TRUE
                 ) SELECT * FROM a WHERE LENGTH(a.Symbol) > 2
             )
         )
     }}
     """
     sql = """
@@ -405,15 +404,15 @@
 def test_ingredient_in_select_with_join_multi_exec(db, ingredients):
     """If the query only has an ingredient in the `SELECT` statement, and `JOIN` clause,
     we should run the `JOIN` statement first, and then call the ingredient.
 
     commit de4a7bc
     """
     blendsql = """
-    SELECT {{get_length('n_length', 'constituents::Name')}} 
+    SELECT {{get_length('n_length', 'constituents::Name')}}
         FROM constituents JOIN account_history ON account_history.Symbol = constituents.Symbol
         WHERE account_history.Action like "%dividend%"
     """
     sql = """
     SELECT LENGTH(constituents.Name)
         FROM constituents JOIN account_history ON account_history.Symbol = constituents.Symbol
         WHERE account_history.Action like "%dividend%"
@@ -424,15 +423,48 @@
         ingredients=ingredients,
     )
     sql_df = db.execute_query(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
     # Make sure we only pass what's necessary to our ingredient
     passed_to_ingredient = db.execute_query(
         """
-    SELECT COUNT(DISTINCT constituents.Name)  
+    SELECT COUNT(DISTINCT constituents.Name)
+    FROM constituents JOIN account_history ON account_history.Symbol = constituents.Symbol
+    WHERE account_history.Action like "%dividend%"
+    """
+    )
+    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+
+
+def test_ingredient_in_select_with_join_multi_select_multi_exec(db, ingredients):
+    """A modified version of the above
+
+    commit de4a7bc
+    """
+    blendsql = """
+    SELECT {{get_length('n_length', 'constituents::Name')}}, Action
+        FROM constituents JOIN account_history ON account_history.Symbol = constituents.Symbol
+        WHERE Action like "%dividend%"
+    """
+    sql = """
+    SELECT LENGTH(constituents.Name), Action
+        FROM constituents JOIN account_history ON account_history.Symbol = constituents.Symbol
+        WHERE Action like "%dividend%"
+    """
+    smoothie = blend(
+        query=blendsql,
+        db=db,
+        ingredients=ingredients,
+    )
+    sql_df = db.execute_query(sql)
+    assert_equality(smoothie=smoothie, sql_df=sql_df)
+    # Make sure we only pass what's necessary to our ingredient
+    passed_to_ingredient = db.execute_query(
+        """
+    SELECT COUNT(DISTINCT constituents.Name)
     FROM constituents JOIN account_history ON account_history.Symbol = constituents.Symbol
     WHERE account_history.Action like "%dividend%"
     """
     )
     assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
```

### Comparing `blendsql-0.0.141/tests/test_single_table_blendsql.py` & `blendsql-0.0.15/tests/test_single_table_blendsql.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,26 +339,57 @@
     )
     sql_df = db.execute_query(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
 
 
 def test_ingredient_in_select_stmt(db, ingredients):
     blendsql = """
-    SELECT MAX({{get_length('length', 'transactions::merchant')}}) as l FROM transactions
+    SELECT MAX({{get_length('length', 'transactions::merchant')}}) as l FROM transactions 
     """
     sql = """
     SELECT MAX(LENGTH(merchant)) as l FROM transactions
     """
     smoothie = blend(
         query=blendsql,
         db=db,
         ingredients=ingredients,
     )
     sql_df = db.execute_query(sql)
     assert_equality(smoothie=smoothie, sql_df=sql_df)
+    # Make sure we only pass what's necessary to our ingredient
+    passed_to_ingredient = db.execute_query(
+        """
+    SELECT COUNT(DISTINCT merchant) FROM transactions 
+    """
+    )
+    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
+
+
+def test_ingredient_in_select_stmt_with_filter(db, ingredients):
+    # commit de4a7bc
+    blendsql = """
+    SELECT MAX({{get_length('length', 'transactions::merchant')}}) as l FROM transactions WHERE child_category = 'Restaurants & Dining'
+    """
+    sql = """
+    SELECT MAX(LENGTH(merchant)) as l FROM transactions WHERE child_category = 'Restaurants & Dining'
+    """
+    smoothie = blend(
+        query=blendsql,
+        db=db,
+        ingredients=ingredients,
+    )
+    sql_df = db.execute_query(sql)
+    assert_equality(smoothie=smoothie, sql_df=sql_df)
+    # Make sure we only pass what's necessary to our ingredient
+    passed_to_ingredient = db.execute_query(
+        """
+    SELECT COUNT(DISTINCT merchant) FROM transactions WHERE child_category = 'Restaurants & Dining'
+    """
+    )
+    assert smoothie.meta.num_values_passed == passed_to_ingredient.values[0].item()
 
 
 def test_nested_duplicate_map_calls(db, ingredients):
     blendsql = """
     SELECT merchant FROM transactions WHERE {{get_length('length', 'transactions::merchant')}} > (SELECT {{get_length('length', 'transactions::merchant')}} FROM transactions WHERE merchant = 'Paypal')
     """
     sql = """
```

### Comparing `blendsql-0.0.141/tests/utils.py` & `blendsql-0.0.15/tests/utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,59 @@
 import pandas as pd
 from typing import Iterable, Any, List, Union
 from blendsql.ingredients import MapIngredient, QAIngredient, JoinIngredient
 from blendsql.db.utils import single_quote_escape
 
 
 class starts_with(MapIngredient):
-    def run(self, question: str, values: List[str], **kwargs) -> Iterable[bool]:
+    def run(self, question: str, values: List[str], **kwargs) -> List[bool]:
         """Simple test function, equivalent to the following in SQL:
             `LIKE '{arg}%`
         This allows us to compare the output of a BlendSQL script with a SQL script easily.
         """
-        mapped_values = [int(i.startswith(question)) for i in values]
+        mapped_values = [bool(i.startswith(question)) for i in values]
         return mapped_values
 
 
 class get_length(MapIngredient):
     def run(self, question: str, values: List[str], **kwargs) -> Iterable[int]:
         """Simple test function, equivalent to the following in SQL:
             `LENGTH '{arg}%`
         This allows us to compare the output of a BlendSQL script with a SQL script easily.
         """
         mapped_values = [len(i) for i in values]
         return mapped_values
 
 
 class select_first_sorted(QAIngredient):
-    def run(self, question: str, options: set, **kwargs) -> Iterable[Any]:
+    def run(self, options: set, **kwargs) -> Iterable[Any]:
         """Simple test function, equivalent to the following in SQL:
         `ORDER BY {colname} LIMIT 1`
         """
         chosen_value = sorted(options)[0]
         return f"'{chosen_value}'"
 
 
 class return_aapl(QAIngredient):
-    def run(
-        self, question: str, options: str = None, **kwargs
-    ) -> Union[str, int, float]:
+    def run(self, **kwargs) -> Union[str, int, float]:
         """Executes to return the string 'AAPL'"""
         return "'AAPL'"
 
 
 class get_table_size(QAIngredient):
-    def run(
-        self, context: pd.DataFrame, options: set = None, **kwargs
-    ) -> Union[str, int, float]:
+    def run(self, context: pd.DataFrame, **kwargs) -> Union[str, int, float]:
         """Returns the length of the context subtable passed to it."""
         return len(context)
 
 
 class select_first_option(QAIngredient):
     def run(
-        self, question: str, context: pd.DataFrame, options: set = None, **kwargs
+        self, question: str, context: pd.DataFrame, options: set, **kwargs
     ) -> Union[str, int, float]:
         """Returns the first item in the (ordered) options set"""
-        assert options is not None
         return f"'{single_quote_escape(sorted(list(options))[0])}'"
 
 
 class do_join(JoinIngredient):
     """A very silly, overcomplicated way to do a traditional SQL join.
     But useful for testing.
     """
```

