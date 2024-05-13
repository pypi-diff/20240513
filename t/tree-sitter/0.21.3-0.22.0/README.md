# Comparing `tmp/tree-sitter-0.21.3.tar.gz` & `tmp/tree-sitter-0.22.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-sitter-0.21.3.tar", last modified: Tue Mar 26 10:25:10 2024, max compression
+gzip compressed data, was "tree-sitter-0.22.0.tar", last modified: Mon May 13 19:37:28 2024, max compression
```

## Comparing `tree-sitter-0.21.3.tar` & `tree-sitter-0.22.0.tar`

### file list

```diff
@@ -1,67 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:25:10.595966 tree-sitter-0.21.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-26 10:24:58.000000 tree-sitter-0.21.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-26 10:24:58.000000 tree-sitter-0.21.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-03-26 10:25:10.595966 tree-sitter-0.21.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-03-26 10:24:58.000000 tree-sitter-0.21.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-03-26 10:24:58.000000 tree-sitter-0.21.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 10:25:10.595966 tree-sitter-0.21.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-03-26 10:24:58.000000 tree-sitter-0.21.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:25:10.587967 tree-sitter-0.21.3/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-03-26 10:24:58.000000 tree-sitter-0.21.3/tree_sitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14184 2024-03-26 10:24:58.000000 tree-sitter-0.21.3/tree_sitter/_binding.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   107273 2024-03-26 10:24:58.000000 tree-sitter-0.21.3/tree_sitter/binding.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:25:10.587967 tree-sitter-0.21.3/tree_sitter/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:25:10.587967 tree-sitter-0.21.3/tree_sitter/core/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:25:10.587967 tree-sitter-0.21.3/tree_sitter/core/lib/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:25:10.591966 tree-sitter-0.21.3/tree_sitter/core/lib/include/tree_sitter/
--rw-r--r--   0 runner    (1001) docker     (127)    39713 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/include/tree_sitter/api.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:25:10.595966 tree-sitter-0.21.3/tree_sitter/core/lib/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/alloc.c
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/alloc.h
--rw-r--r--   0 runner    (1001) docker     (127)    10361 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/array.h
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/atomic.h
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/clock.h
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/error_costs.h
--rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/get_changed_ranges.c
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/get_changed_ranges.h
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/host.h
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/language.c
--rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/language.h
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/length.h
--rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/lexer.c
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/lexer.h
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/lib.c
--rw-r--r--   0 runner    (1001) docker     (127)    21690 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/node.c
--rw-r--r--   0 runner    (1001) docker     (127)    72817 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/parser.c
--rw-r--r--   0 runner    (1001) docker     (127)     5534 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/parser.h
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/point.h
--rw-r--r--   0 runner    (1001) docker     (127)   141258 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/query.c
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/reduce_action.h
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/reusable_node.h
--rw-r--r--   0 runner    (1001) docker     (127)    28201 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/stack.c
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/stack.h
--rw-r--r--   0 runner    (1001) docker     (127)    35141 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/subtree.c
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/subtree.h
--rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/tree.c
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/tree.h
--rw-r--r--   0 runner    (1001) docker     (127)    22725 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/tree_cursor.c
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/tree_cursor.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:25:10.595966 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/ICU_SHA
--rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/ptypes.h
--rw-r--r--   0 runner    (1001) docker     (127)    14865 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/umachine.h
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/urename.h
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/utf.h
--rw-r--r--   0 runner    (1001) docker     (127)    23878 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/utf16.h
--rw-r--r--   0 runner    (1001) docker     (127)    31698 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/utf8.h
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode.h
--rw-r--r--   0 runner    (1001) docker     (127)    53246 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/wasm_store.c
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-26 10:25:03.000000 tree-sitter-0.21.3/tree_sitter/core/lib/src/wasm_store.h
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:24:58.000000 tree-sitter-0.21.3/tree_sitter/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:25:10.591966 tree-sitter-0.21.3/tree_sitter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-03-26 10:25:10.000000 tree-sitter-0.21.3/tree_sitter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2024-03-26 10:25:10.000000 tree-sitter-0.21.3/tree_sitter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 10:25:10.000000 tree-sitter-0.21.3/tree_sitter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-26 10:25:10.000000 tree-sitter-0.21.3/tree_sitter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.694662 tree-sitter-0.22.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-13 19:37:28.694662 tree-sitter-0.22.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 19:37:28.694662 tree-sitter-0.22.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/binding/
+-rw-r--r--   0 runner    (1001) docker     (127)    11697 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/language.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7311 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/lookahead_iterator.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/lookahead_names_iterator.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/module.c
+-rw-r--r--   0 runner    (1001) docker     (127)    30759 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/node.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16982 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26415 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/query.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/range.c
+-rw-r--r--   0 runner    (1001) docker     (127)     7633 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/tree.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13643 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/binding/tree_cursor.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/core/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/core/lib/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter/core/lib/include/tree_sitter/
+-rw-r--r--   0 runner    (1001) docker     (127)    40024 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/include/tree_sitter/api.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.694662 tree-sitter-0.22.0/tree_sitter/core/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/alloc.c
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/alloc.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10420 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/atomic.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/clock.h
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/error_costs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15514 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/get_changed_ranges.c
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/get_changed_ranges.h
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/host.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/language.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8368 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/language.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/length.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/lexer.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/lexer.h
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/lib.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22016 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/node.c
+-rw-r--r--   0 runner    (1001) docker     (127)    73664 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/parser.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/parser.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/point.h
+-rw-r--r--   0 runner    (1001) docker     (127)   141258 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/query.c
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/reduce_action.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/reusable_node.h
+-rw-r--r--   0 runner    (1001) docker     (127)    28201 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/stack.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/stack.h
+-rw-r--r--   0 runner    (1001) docker     (127)    35490 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/subtree.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/subtree.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5137 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/tree.c
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/tree.h
+-rw-r--r--   0 runner    (1001) docker     (127)    22905 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/tree_cursor.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/tree_cursor.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.694662 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/ICU_SHA
+-rw-r--r--   0 runner    (1001) docker     (127)    21001 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/ptypes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14865 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/umachine.h
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/urename.h
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/utf.h
+-rw-r--r--   0 runner    (1001) docker     (127)    23878 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/utf16.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31698 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/utf8.h
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode.h
+-rw-r--r--   0 runner    (1001) docker     (127)    59477 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/wasm_store.c
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-13 19:37:24.000000 tree-sitter-0.22.0/tree_sitter/core/lib/src/wasm_store.h
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:22.000000 tree-sitter-0.22.0/tree_sitter/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 19:37:28.686662 tree-sitter-0.22.0/tree_sitter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-05-13 19:37:28.000000 tree-sitter-0.22.0/tree_sitter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-13 19:37:28.000000 tree-sitter-0.22.0/tree_sitter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 19:37:28.000000 tree-sitter-0.22.0/tree_sitter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-13 19:37:28.000000 tree-sitter-0.22.0/tree_sitter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 19:37:28.000000 tree-sitter-0.22.0/tree_sitter.egg-info/top_level.txt
```

### Comparing `tree-sitter-0.21.3/LICENSE` & `tree-sitter-0.22.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/PKG-INFO` & `tree-sitter-0.22.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 Metadata-Version: 2.1
 Name: tree-sitter
-Version: 0.21.3
-Summary: Python bindings for the Tree-Sitter parsing library
+Version: 0.22.0
+Summary: Python bindings to the Tree-sitter parsing library
 Author-email: Max Brunsfeld <maxbrunsfeld@gmail.com>
 Project-URL: Homepage, https://tree-sitter.github.io/tree-sitter/
 Project-URL: Source, https://github.com/tree-sitter/py-tree-sitter
+Project-URL: Documentation, https://tree-sitter.github.io/py-tree-sitter/
 Keywords: incremental,parsing,tree-sitter
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: tests
 License-File: LICENSE
 
 # Python Tree-sitter
 
 [![CI][ci]](https://github.com/tree-sitter/py-tree-sitter/actions/workflows/ci.yml)
 [![pypi][pypi]](https://pypi.org/project/tree-sitter/)
+[![docs][docs]](https://tree-sitter.github.io/py-tree-sitter/)
 
 This module provides Python bindings to the [tree-sitter] parsing library.
 
 ## Installation
 
 The package has no library dependencies and provides pre-compiled wheels for all major platforms.
 
@@ -51,53 +55,15 @@
 
 Then, you can load it as a `Language` object:
 
 ```python
 import tree_sitter_python as tspython
 from tree_sitter import Language, Parser
 
-PY_LANGUAGE = Language(tspython.language(), "python")
-```
-
-#### Build from source
-
-> [!WARNING]
-> This method of loading languages is deprecated and will be removed in `v0.22.0`.
-> You should only use it if you need languages that have not updated their bindings.
-> Keep in mind that you will need a C compiler in this case.
-
-First you'll need a Tree-sitter language implementation for each language that you want to parse.
-
-```sh
-git clone https://github.com/tree-sitter/tree-sitter-go
-git clone https://github.com/tree-sitter/tree-sitter-javascript
-git clone https://github.com/tree-sitter/tree-sitter-python
-```
-
-Use the `Language.build_library` method to compile these into a library that's
-usable from Python. This function will return immediately if the library has
-already been compiled since the last time its source code was modified:
-
-```python
-from tree_sitter import Language, Parser
-
-Language.build_library(
-    # Store the library in the `build` directory
-    "build/my-languages.so",
-    # Include one or more languages
-    ["vendor/tree-sitter-go", "vendor/tree-sitter-javascript", "vendor/tree-sitter-python"],
-)
-```
-
-Load the languages into your app as `Language` objects:
-
-```python
-GO_LANGUAGE = Language("build/my-languages.so", "go")
-JS_LANGUAGE = Language("build/my-languages.so", "javascript")
-PY_LANGUAGE = Language("build/my-languages.so", "python")
+PY_LANGUAGE = Language(tspython.language())
 ```
 
 ### Basic parsing
 
 Create a `Parser` and configure it to use a language:
 
 ```python
@@ -111,27 +77,27 @@
 tree = parser.parse(
     bytes(
         """
 def foo():
     if bar:
         baz()
 """,
-        "utf8",
+        "utf8"
     )
 )
 ```
 
 If you have your source code in some data structure other than a bytes object,
 you can pass a "read" callable to the parse function.
 
 The read callable can use either the byte offset or point tuple to read from
 buffer and return source code as bytes object. An empty bytes object or None
-terminates parsing for that line. The bytes must encode the source as UTF-8.
+terminates parsing for that line. The bytes must be encoded as UTF-8 or UTF-16.
 
-For example, to use the byte offset:
+For example, to use the byte offset with UTF-8 encoding:
 
 ```python
 src = bytes(
     """
 def foo():
     if bar:
         baz()
@@ -140,15 +106,15 @@
 )
 
 
 def read_callable_byte_offset(byte_offset, point):
     return src[byte_offset : byte_offset + 1]
 
 
-tree = parser.parse(read_callable_byte_offset)
+tree = parser.parse(read_callable_byte_offset, encoding="utf8")
 ```
 
 And to use the point:
 
 ```python
 src_lines = ["\n", "def foo():\n", "    if bar:\n", "        baz()\n"]
 
@@ -156,15 +122,15 @@
 def read_callable_point(byte_offset, point):
     row, column = point
     if row >= len(src_lines) or column >= len(src_lines[row]):
         return None
     return src_lines[row][column:].encode("utf8")
 
 
-tree = parser.parse(read_callable_point)
+tree = parser.parse(read_callable_point, encoding="utf8")
 ```
 
 Inspect the resulting `Tree`:
 
 ```python
 root_node = tree.root_node
 assert root_node.type == 'module'
@@ -206,14 +172,35 @@
                     "consequence: (block "
                         "(expression_statement (call "
                             "function: (identifier) "
                             "arguments: (argument_list))))))))"
 )
 ```
 
+Or, to use the byte offset with UTF-16 encoding:
+
+```python
+parser.set_language(JAVASCRIPT)
+source_code = bytes("'😎' && '🐍'", "utf16")
+
+def read(byte_position, _):
+    return source_code[byte_position: byte_position + 2]
+
+tree = parser.parse(read, encoding="utf16")
+root_node = tree.root_node
+statement_node = root_node.children[0]
+binary_node = statement_node.children[0]
+snake_node = binary_node.children[2]
+snake = source_code[snake_node.start_byte:snake_node.end_byte]
+
+assert binary_node.type == "binary_expression"
+assert snake_node.type == "string"
+assert snake.decode("utf16") == "'🐍'"
+```
+
 ### Walking syntax trees
 
 If you need to traverse a large number of nodes efficiently, you can use
 a `TreeCursor`:
 
 ```python
 cursor = tree.walk()
@@ -340,9 +327,10 @@
 
 [tree-sitter]: https://tree-sitter.github.io/tree-sitter/
 [issue]: https://github.com/tree-sitter/py-tree-sitter/issues/new
 [tree-sitter-python]: https://github.com/tree-sitter/tree-sitter-python
 [tree query]: https://tree-sitter.github.io/tree-sitter/using-parsers#query-syntax
 [ci]: https://img.shields.io/github/actions/workflow/status/tree-sitter/py-tree-sitter/ci.yml?logo=github&label=CI
 [pypi]: https://img.shields.io/pypi/v/tree-sitter?logo=pypi&logoColor=ffd242&label=PyPI
+[docs]: https://img.shields.io/github/deployments/tree-sitter/py-tree-sitter/github-pages?logo=sphinx&label=Docs
 [examples/walk_tree.py]: https://github.com/tree-sitter/py-tree-sitter/blob/master/examples/walk_tree.py
 [examples/usage.py]: https://github.com/tree-sitter/py-tree-sitter/blob/master/examples/usage.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tree-sitter-0.21.3/README.md` & `tree-sitter-0.22.0/tree_sitter.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,35 @@
+Metadata-Version: 2.1
+Name: tree-sitter
+Version: 0.22.0
+Summary: Python bindings to the Tree-sitter parsing library
+Author-email: Max Brunsfeld <maxbrunsfeld@gmail.com>
+Project-URL: Homepage, https://tree-sitter.github.io/tree-sitter/
+Project-URL: Source, https://github.com/tree-sitter/py-tree-sitter
+Project-URL: Documentation, https://tree-sitter.github.io/py-tree-sitter/
+Keywords: incremental,parsing,tree-sitter
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: C
+Classifier: Programming Language :: Python
+Classifier: Topic :: Software Development :: Compilers
+Classifier: Topic :: Text Processing :: Linguistic
+Classifier: Typing :: Typed
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: tests
+License-File: LICENSE
+
 # Python Tree-sitter
 
 [![CI][ci]](https://github.com/tree-sitter/py-tree-sitter/actions/workflows/ci.yml)
 [![pypi][pypi]](https://pypi.org/project/tree-sitter/)
+[![docs][docs]](https://tree-sitter.github.io/py-tree-sitter/)
 
 This module provides Python bindings to the [tree-sitter] parsing library.
 
 ## Installation
 
 The package has no library dependencies and provides pre-compiled wheels for all major platforms.
 
@@ -31,53 +55,15 @@
 
 Then, you can load it as a `Language` object:
 
 ```python
 import tree_sitter_python as tspython
 from tree_sitter import Language, Parser
 
-PY_LANGUAGE = Language(tspython.language(), "python")
-```
-
-#### Build from source
-
-> [!WARNING]
-> This method of loading languages is deprecated and will be removed in `v0.22.0`.
-> You should only use it if you need languages that have not updated their bindings.
-> Keep in mind that you will need a C compiler in this case.
-
-First you'll need a Tree-sitter language implementation for each language that you want to parse.
-
-```sh
-git clone https://github.com/tree-sitter/tree-sitter-go
-git clone https://github.com/tree-sitter/tree-sitter-javascript
-git clone https://github.com/tree-sitter/tree-sitter-python
-```
-
-Use the `Language.build_library` method to compile these into a library that's
-usable from Python. This function will return immediately if the library has
-already been compiled since the last time its source code was modified:
-
-```python
-from tree_sitter import Language, Parser
-
-Language.build_library(
-    # Store the library in the `build` directory
-    "build/my-languages.so",
-    # Include one or more languages
-    ["vendor/tree-sitter-go", "vendor/tree-sitter-javascript", "vendor/tree-sitter-python"],
-)
-```
-
-Load the languages into your app as `Language` objects:
-
-```python
-GO_LANGUAGE = Language("build/my-languages.so", "go")
-JS_LANGUAGE = Language("build/my-languages.so", "javascript")
-PY_LANGUAGE = Language("build/my-languages.so", "python")
+PY_LANGUAGE = Language(tspython.language())
 ```
 
 ### Basic parsing
 
 Create a `Parser` and configure it to use a language:
 
 ```python
@@ -91,27 +77,27 @@
 tree = parser.parse(
     bytes(
         """
 def foo():
     if bar:
         baz()
 """,
-        "utf8",
+        "utf8"
     )
 )
 ```
 
 If you have your source code in some data structure other than a bytes object,
 you can pass a "read" callable to the parse function.
 
 The read callable can use either the byte offset or point tuple to read from
 buffer and return source code as bytes object. An empty bytes object or None
-terminates parsing for that line. The bytes must encode the source as UTF-8.
+terminates parsing for that line. The bytes must be encoded as UTF-8 or UTF-16.
 
-For example, to use the byte offset:
+For example, to use the byte offset with UTF-8 encoding:
 
 ```python
 src = bytes(
     """
 def foo():
     if bar:
         baz()
@@ -120,15 +106,15 @@
 )
 
 
 def read_callable_byte_offset(byte_offset, point):
     return src[byte_offset : byte_offset + 1]
 
 
-tree = parser.parse(read_callable_byte_offset)
+tree = parser.parse(read_callable_byte_offset, encoding="utf8")
 ```
 
 And to use the point:
 
 ```python
 src_lines = ["\n", "def foo():\n", "    if bar:\n", "        baz()\n"]
 
@@ -136,15 +122,15 @@
 def read_callable_point(byte_offset, point):
     row, column = point
     if row >= len(src_lines) or column >= len(src_lines[row]):
         return None
     return src_lines[row][column:].encode("utf8")
 
 
-tree = parser.parse(read_callable_point)
+tree = parser.parse(read_callable_point, encoding="utf8")
 ```
 
 Inspect the resulting `Tree`:
 
 ```python
 root_node = tree.root_node
 assert root_node.type == 'module'
@@ -186,14 +172,35 @@
                     "consequence: (block "
                         "(expression_statement (call "
                             "function: (identifier) "
                             "arguments: (argument_list))))))))"
 )
 ```
 
+Or, to use the byte offset with UTF-16 encoding:
+
+```python
+parser.set_language(JAVASCRIPT)
+source_code = bytes("'😎' && '🐍'", "utf16")
+
+def read(byte_position, _):
+    return source_code[byte_position: byte_position + 2]
+
+tree = parser.parse(read, encoding="utf16")
+root_node = tree.root_node
+statement_node = root_node.children[0]
+binary_node = statement_node.children[0]
+snake_node = binary_node.children[2]
+snake = source_code[snake_node.start_byte:snake_node.end_byte]
+
+assert binary_node.type == "binary_expression"
+assert snake_node.type == "string"
+assert snake.decode("utf16") == "'🐍'"
+```
+
 ### Walking syntax trees
 
 If you need to traverse a large number of nodes efficiently, you can use
 a `TreeCursor`:
 
 ```python
 cursor = tree.walk()
@@ -320,9 +327,10 @@
 
 [tree-sitter]: https://tree-sitter.github.io/tree-sitter/
 [issue]: https://github.com/tree-sitter/py-tree-sitter/issues/new
 [tree-sitter-python]: https://github.com/tree-sitter/tree-sitter-python
 [tree query]: https://tree-sitter.github.io/tree-sitter/using-parsers#query-syntax
 [ci]: https://img.shields.io/github/actions/workflow/status/tree-sitter/py-tree-sitter/ci.yml?logo=github&label=CI
 [pypi]: https://img.shields.io/pypi/v/tree-sitter?logo=pypi&logoColor=ffd242&label=PyPI
+[docs]: https://img.shields.io/github/deployments/tree-sitter/py-tree-sitter/github-pages?logo=sphinx&label=Docs
 [examples/walk_tree.py]: https://github.com/tree-sitter/py-tree-sitter/blob/master/examples/walk_tree.py
 [examples/usage.py]: https://github.com/tree-sitter/py-tree-sitter/blob/master/examples/usage.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tree-sitter-0.21.3/pyproject.toml` & `tree-sitter-0.22.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,63 @@
 [build-system]
 requires = ["setuptools>=43"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tree-sitter"
-version = "0.21.3"
-description = "Python bindings for the Tree-Sitter parsing library"
+version = "0.22.0"
+description = "Python bindings to the Tree-sitter parsing library"
 keywords = ["incremental", "parsing", "tree-sitter"]
 classifiers = [
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: C",
     "Programming Language :: Python",
     "Topic :: Software Development :: Compilers",
     "Topic :: Text Processing :: Linguistic",
     "Typing :: Typed",
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 readme = "README.md"
 
 [project.urls]
 Homepage = "https://tree-sitter.github.io/tree-sitter/"
 Source = "https://github.com/tree-sitter/py-tree-sitter"
+Documentation = "https://tree-sitter.github.io/py-tree-sitter/"
 
 [[project.authors]]
 name = "Max Brunsfeld"
 email = "maxbrunsfeld@gmail.com"
 
+[project.optional-dependencies]
+docs = ["sphinx~=7.3", "sphinx-book-theme"]
+tests = [
+    "tree-sitter-html",
+    "tree-sitter-javascript",
+    "tree-sitter-json",
+    "tree-sitter-python",
+    "tree-sitter-rust",
+]
+
 [tool.ruff]
-target-version = "py38"
+target-version = "py39"
 line-length = 100
 indent-width = 4
 extend-exclude = [
     ".github",
     "__pycache__",
-    "tests/fixtures",
+    "setup.py",
     "tree_sitter/core",
 ]
 
 [tool.ruff.format]
 quote-style = "double"
 indent-style = "space"
 
 [tool.cibuildwheel]
 build-frontend = "build"
+test-extras = ["tests"]
 test-command = "python -munittest discover -s {project}/tests"
 
-[tool.cibuildwheel.environment]
-PYTHONWARNINGS = "ignore:::tree_sitter"
+[tool.mypy]
+exclude = ["tree_sitter/core"]
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/include/tree_sitter/api.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/include/tree_sitter/api.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #ifndef TREE_SITTER_API_H_
 #define TREE_SITTER_API_H_
 
+#ifndef TREE_SITTER_HIDE_SYMBOLS
 #if defined(__GNUC__) || defined(__clang__)
 #pragma GCC visibility push(default)
 #endif
+#endif
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 #include <stdlib.h>
 #include <stdint.h>
@@ -99,15 +101,15 @@
   const void *id;
   const TSTree *tree;
 } TSNode;
 
 typedef struct TSTreeCursor {
   const void *tree;
   const void *id;
-  uint32_t context[2];
+  uint32_t context[3];
 } TSTreeCursor;
 
 typedef struct TSQueryCapture {
   TSNode node;
   uint32_t index;
 } TSQueryCapture;
 
@@ -542,18 +544,25 @@
 /**
  * Get the parse state after this node.
 */
 TSStateId ts_node_next_parse_state(TSNode self);
 
 /**
  * Get the node's immediate parent.
+ * Prefer [`ts_node_child_containing_descendant`] for
+ * iterating over the node's ancestors.
  */
 TSNode ts_node_parent(TSNode self);
 
 /**
+ * Get the node's child that contains `descendant`.
+ */
+TSNode ts_node_child_containing_descendant(TSNode self, TSNode descendant);
+
+/**
  * Get the node's child at the given index, where zero represents the first
  * child.
  */
 TSNode ts_node_child(TSNode self, uint32_t child_index);
 
 /**
  * Get the field name for node's child at the given index, where zero represents
@@ -1251,12 +1260,14 @@
 	void (*new_free)(void *)
 );
 
 #ifdef __cplusplus
 }
 #endif
 
+#ifndef TREE_SITTER_HIDE_SYMBOLS
 #if defined(__GNUC__) || defined(__clang__)
 #pragma GCC visibility pop
 #endif
+#endif
 
 #endif  // TREE_SITTER_API_H_
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/alloc.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/alloc.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/array.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/array.h`

 * *Files 1% similar despite different names*

```diff
@@ -62,17 +62,20 @@
 #define array_push(self, element)                            \
   (_array__grow((Array *)(self), 1, array_elem_size(self)), \
    (self)->contents[(self)->size++] = (element))
 
 /// Increase the array's size by `count` elements.
 /// New elements are zero-initialized.
 #define array_grow_by(self, count) \
-  (_array__grow((Array *)(self), count, array_elem_size(self)), \
-   memset((self)->contents + (self)->size, 0, (count) * array_elem_size(self)), \
-   (self)->size += (count))
+  do { \
+    if ((count) == 0) break; \
+    _array__grow((Array *)(self), count, array_elem_size(self)); \
+    memset((self)->contents + (self)->size, 0, (count) * array_elem_size(self)); \
+    (self)->size += (count); \
+  } while (0)
 
 /// Append all elements from one array to the end of another.
 #define array_push_all(self, other)                                       \
   array_extend((self), (other)->size, (other)->contents)
 
 /// Append `count` elements to the end of the array, reading their values from the
 /// `contents` pointer.
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/atomic.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/atomic.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/clock.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/clock.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/get_changed_ranges.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/get_changed_ranges.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/get_changed_ranges.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/get_changed_ranges.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/host.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/host.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/language.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/language.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/language.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/language.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/length.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/length.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/lexer.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/lexer.c`

 * *Files 0% similar despite different names*

```diff
@@ -361,15 +361,15 @@
   uint32_t current_lookahead_end_byte = self->current_position.bytes + 1;
 
   // In order to determine that a byte sequence is invalid UTF8 or UTF16,
   // the character decoding algorithm may have looked at the following byte.
   // Therefore, the next byte *after* the current (invalid) character
   // affects the interpretation of the current character.
   if (self->data.lookahead == TS_DECODE_ERROR) {
-    current_lookahead_end_byte++;
+    current_lookahead_end_byte += 4; // the maximum number of bytes read to identify an invalid code point
   }
 
   if (current_lookahead_end_byte > *lookahead_end_byte) {
     *lookahead_end_byte = current_lookahead_end_byte;
   }
 }
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/lexer.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/lexer.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/node.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/node.c`

 * *Files 2% similar despite different names*

```diff
@@ -435,15 +435,22 @@
 
 const char *ts_node_grammar_type(TSNode self) {
   TSSymbol symbol = ts_subtree_symbol(ts_node__subtree(self));
   return ts_language_symbol_name(self.tree->language, symbol);
 }
 
 char *ts_node_string(TSNode self) {
-  return ts_subtree_string(ts_node__subtree(self), self.tree->language, false);
+  TSSymbol alias_symbol = ts_node__alias(&self);
+  return ts_subtree_string(
+    ts_node__subtree(self),
+    alias_symbol,
+    ts_language_symbol_metadata(self.tree->language, alias_symbol).visible,
+    self.tree->language,
+    false
+  );
 }
 
 bool ts_node_eq(TSNode self, TSNode other) {
   return self.tree == other.tree && self.id == other.id;
 }
 
 bool ts_node_is_null(TSNode self) {
@@ -494,41 +501,43 @@
   }
   uint16_t symbol = ts_node_grammar_symbol(self);
   return ts_language_next_state(language, state, symbol);
 }
 
 TSNode ts_node_parent(TSNode self) {
   TSNode node = ts_tree_root_node(self.tree);
-  uint32_t end_byte = ts_node_end_byte(self);
   if (node.id == self.id) return ts_node__null();
 
-  TSNode last_visible_node = node;
-  bool did_descend = true;
-  while (did_descend) {
-    did_descend = false;
+  while (true) {
+   TSNode next_node = ts_node_child_containing_descendant(node, self);
+   if (ts_node_is_null(next_node)) break;
+   node = next_node;
+  }
 
-    TSNode child;
-    NodeChildIterator iterator = ts_node_iterate_children(&node);
-    while (ts_node_child_iterator_next(&iterator, &child)) {
+  return node;
+}
+
+TSNode ts_node_child_containing_descendant(TSNode self, TSNode subnode) {
+  uint32_t start_byte = ts_node_start_byte(subnode);
+  uint32_t end_byte = ts_node_end_byte(subnode);
+
+  do {
+    NodeChildIterator iter = ts_node_iterate_children(&self);
+    do {
       if (
-        ts_node_start_byte(child) > ts_node_start_byte(self) ||
-        child.id == self.id
-      ) break;
-      if (iterator.position.bytes >= end_byte) {
-        node = child;
-        if (ts_node__is_relevant(child, true)) {
-          last_visible_node = node;
-        }
-        did_descend = true;
-        break;
+        !ts_node_child_iterator_next(&iter, &self)
+        || ts_node_start_byte(self) > start_byte
+        || self.id == subnode.id
+      ) {
+        return ts_node__null();
       }
-    }
-  }
+    } while (iter.position.bytes < end_byte || ts_node_child_count(self) == 0);
+  } while (!ts_node__is_relevant(self, true));
 
-  return last_visible_node;
+  return self;
 }
 
 TSNode ts_node_child(TSNode self, uint32_t child_index) {
   return ts_node__child(self, child_index, true);
 }
 
 TSNode ts_node_named_child(TSNode self, uint32_t child_index) {
@@ -633,14 +642,17 @@
 
     TSNode child;
     uint32_t index = 0;
     NodeChildIterator iterator = ts_node_iterate_children(&result);
     while (ts_node_child_iterator_next(&iterator, &child)) {
       if (ts_node__is_relevant(child, true)) {
         if (index == child_index) {
+          if (ts_node_is_extra(child)) {
+            return NULL;
+          }
           const char *field_name = ts_node__field_name_from_language(result, iterator.structural_child_index - 1);
           if (field_name) return field_name;
           return inherited_field_name;
         }
         index++;
       } else {
         uint32_t grandchild_index = child_index - index;
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/parser.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/parser.c`

 * *Files 1% similar despite different names*

```diff
@@ -106,14 +106,15 @@
   TSDuration timeout_duration;
   unsigned accept_count;
   unsigned operation_count;
   const volatile size_t *cancellation_flag;
   Subtree old_tree;
   TSRangeArray included_range_differences;
   unsigned included_range_difference_index;
+  bool has_scanner_error;
 };
 
 typedef struct {
   unsigned cost;
   unsigned node_count;
   int dynamic_precedence;
   bool is_in_error;
@@ -333,62 +334,79 @@
         break;
     }
   }
 
   return false;
 }
 
+static bool ts_parser__call_main_lex_fn(TSParser *self, TSLexMode lex_mode) {
+  if (ts_language_is_wasm(self->language)) {
+    return ts_wasm_store_call_lex_main(self->wasm_store, lex_mode.lex_state);
+  } else {
+    return self->language->lex_fn(&self->lexer.data, lex_mode.lex_state);
+  }
+}
+
+static bool ts_parser__call_keyword_lex_fn(TSParser *self, TSLexMode lex_mode) {
+  if (ts_language_is_wasm(self->language)) {
+    return ts_wasm_store_call_lex_keyword(self->wasm_store, 0);
+  } else {
+    return self->language->keyword_lex_fn(&self->lexer.data, 0);
+  }
+}
+
 static void ts_parser__external_scanner_create(
   TSParser *self
 ) {
   if (self->language && self->language->external_scanner.states) {
     if (ts_language_is_wasm(self->language)) {
       self->external_scanner_payload = (void *)(uintptr_t)ts_wasm_store_call_scanner_create(
         self->wasm_store
       );
+      if (ts_wasm_store_has_error(self->wasm_store)) {
+        self->has_scanner_error = true;
+      }
     } else if (self->language->external_scanner.create) {
       self->external_scanner_payload = self->language->external_scanner.create();
     }
   }
 }
 
 static void ts_parser__external_scanner_destroy(
   TSParser *self
 ) {
-  if (self->language && self->external_scanner_payload) {
-    if (ts_language_is_wasm(self->language)) {
-      if (self->wasm_store) {
-        ts_wasm_store_call_scanner_destroy(
-          self->wasm_store,
-          (uintptr_t)self->external_scanner_payload
-        );
-      }
-    } else if (self->language->external_scanner.destroy) {
-      self->language->external_scanner.destroy(
-        self->external_scanner_payload
-      );
-    }
-    self->external_scanner_payload = NULL;
+  if (
+    self->language &&
+    self->external_scanner_payload &&
+    self->language->external_scanner.destroy &&
+    !ts_language_is_wasm(self->language)
+  ) {
+    self->language->external_scanner.destroy(
+      self->external_scanner_payload
+    );
   }
+  self->external_scanner_payload = NULL;
 }
 
 static unsigned ts_parser__external_scanner_serialize(
   TSParser *self
 ) {
   if (ts_language_is_wasm(self->language)) {
     return ts_wasm_store_call_scanner_serialize(
       self->wasm_store,
       (uintptr_t)self->external_scanner_payload,
       self->lexer.debug_buffer
     );
   } else {
-    return self->language->external_scanner.serialize(
+    uint32_t length = self->language->external_scanner.serialize(
       self->external_scanner_payload,
       self->lexer.debug_buffer
     );
+    assert(length <= TREE_SITTER_SERIALIZATION_BUFFER_SIZE);
+    return length;
   }
 }
 
 static void ts_parser__external_scanner_deserialize(
   TSParser *self,
   Subtree external_token
 ) {
@@ -402,34 +420,40 @@
   if (ts_language_is_wasm(self->language)) {
     ts_wasm_store_call_scanner_deserialize(
       self->wasm_store,
       (uintptr_t)self->external_scanner_payload,
       data,
       length
     );
+    if (ts_wasm_store_has_error(self->wasm_store)) {
+      self->has_scanner_error = true;
+    }
   } else {
     self->language->external_scanner.deserialize(
       self->external_scanner_payload,
       data,
       length
     );
   }
 }
 
 static bool ts_parser__external_scanner_scan(
   TSParser *self,
   TSStateId external_lex_state
 ) {
-
   if (ts_language_is_wasm(self->language)) {
-    return ts_wasm_store_call_scanner_scan(
+    bool result = ts_wasm_store_call_scanner_scan(
       self->wasm_store,
       (uintptr_t)self->external_scanner_payload,
       external_lex_state * self->language->external_token_count
     );
+    if (ts_wasm_store_has_error(self->wasm_store)) {
+      self->has_scanner_error = true;
+    }
+    return result;
   } else {
     const bool *valid_external_tokens = ts_language_enabled_external_tokens(
       self->language,
       external_lex_state
     );
     return self->language->external_scanner.scan(
       self->external_scanner_payload,
@@ -510,14 +534,15 @@
         lex_mode.external_lex_state,
         current_position.extent.row,
         current_position.extent.column
       );
       ts_lexer_start(&self->lexer);
       ts_parser__external_scanner_deserialize(self, external_token);
       found_token = ts_parser__external_scanner_scan(self, lex_mode.external_lex_state);
+      if (self->has_scanner_error) return NULL_SUBTREE;
       ts_lexer_finish(&self->lexer, &lookahead_end_byte);
 
       if (found_token) {
         external_scanner_state_len = ts_parser__external_scanner_serialize(self);
         external_scanner_state_changed = !ts_external_scanner_state_eq(
           ts_subtree_external_scanner_state(external_token),
           self->lexer.debug_buffer,
@@ -560,19 +585,15 @@
     LOG(
       "lex_internal state:%d, row:%u, column:%u",
       lex_mode.lex_state,
       current_position.extent.row,
       current_position.extent.column
     );
     ts_lexer_start(&self->lexer);
-    if (ts_language_is_wasm(self->language)) {
-      found_token = ts_wasm_store_call_lex_main(self->wasm_store, lex_mode.lex_state);
-    } else {
-      found_token = self->language->lex_fn(&self->lexer.data, lex_mode.lex_state);
-    }
+    found_token = ts_parser__call_main_lex_fn(self, lex_mode);
     ts_lexer_finish(&self->lexer, &lookahead_end_byte);
     if (found_token) break;
 
     if (!error_mode) {
       error_mode = true;
       lex_mode = self->language->lex_modes[ERROR_STATE];
       ts_lexer_reset(&self->lexer, start_position);
@@ -622,19 +643,15 @@
     if (found_external_token) {
       symbol = self->language->external_scanner.symbol_map[symbol];
     } else if (symbol == self->language->keyword_capture_token && symbol != 0) {
       uint32_t end_byte = self->lexer.token_end_position.bytes;
       ts_lexer_reset(&self->lexer, self->lexer.token_start_position);
       ts_lexer_start(&self->lexer);
 
-      if (ts_language_is_wasm(self->language)) {
-        is_keyword = ts_wasm_store_call_lex_keyword(self->wasm_store, 0);
-      } else {
-        is_keyword = self->language->keyword_lex_fn(&self->lexer.data, 0);
-      }
+      is_keyword = ts_parser__call_keyword_lex_fn(self, lex_mode);
 
       if (
         is_keyword &&
         self->lexer.token_end_position.bytes == end_byte &&
         ts_language_has_actions(self->language, parse_state, self->lexer.data.result_symbol)
       ) {
         symbol = self->lexer.data.result_symbol;
@@ -816,22 +833,22 @@
 
   if (ts_subtree_error_cost(left) < ts_subtree_error_cost(right)) {
     LOG("select_smaller_error symbol:%s, over_symbol:%s", TREE_NAME(left), TREE_NAME(right));
     return false;
   }
 
   if (ts_subtree_dynamic_precedence(right) > ts_subtree_dynamic_precedence(left)) {
-    LOG("select_higher_precedence symbol:%s, prec:%" PRId32 ", over_symbol:%s, other_prec:%u",
+    LOG("select_higher_precedence symbol:%s, prec:%" PRId32 ", over_symbol:%s, other_prec:%" PRId32,
         TREE_NAME(right), ts_subtree_dynamic_precedence(right), TREE_NAME(left),
         ts_subtree_dynamic_precedence(left));
     return true;
   }
 
   if (ts_subtree_dynamic_precedence(left) > ts_subtree_dynamic_precedence(right)) {
-    LOG("select_higher_precedence symbol:%s, prec:%" PRId32 ", over_symbol:%s, other_prec:%u",
+    LOG("select_higher_precedence symbol:%s, prec:%" PRId32 ", over_symbol:%s, other_prec:%" PRId32,
         TREE_NAME(left), ts_subtree_dynamic_precedence(left), TREE_NAME(right),
         ts_subtree_dynamic_precedence(right));
     return false;
   }
 
   if (ts_subtree_error_cost(left) > 0) return true;
 
@@ -1523,14 +1540,15 @@
 
   bool needs_lex = !lookahead.ptr;
   for (;;) {
     // Otherwise, re-run the lexer.
     if (needs_lex) {
       needs_lex = false;
       lookahead = ts_parser__lex(self, version, state);
+      if (self->has_scanner_error) return false;
 
       if (lookahead.ptr) {
         ts_parser__set_cached_token(self, position, last_external_token, lookahead);
         ts_language_table_entry(self->language, state, ts_subtree_symbol(lookahead), &table_entry);
       }
 
       // When parsing a non-terminal extra, a null lookahead indicates the
@@ -1807,14 +1825,15 @@
   }
 
   return min_error_cost;
 }
 
 static bool ts_parser_has_outstanding_parse(TSParser *self) {
   return (
+    self->external_scanner_payload ||
     ts_stack_state(self->stack, 0) != 1 ||
     ts_stack_node_count_since_error(self->stack, 0) != 0
   );
 }
 
 // Parser - Public
 
@@ -1826,14 +1845,17 @@
   self->tree_pool = ts_subtree_pool_new(32);
   self->stack = ts_stack_new(&self->tree_pool);
   self->finished_tree = NULL_SUBTREE;
   self->reusable_node = reusable_node_new();
   self->dot_graph_file = NULL;
   self->cancellation_flag = NULL;
   self->timeout_duration = 0;
+  self->language = NULL;
+  self->has_scanner_error = false;
+  self->external_scanner_payload = NULL;
   self->end_clock = clock_null();
   self->operation_count = 0;
   self->old_tree = NULL_SUBTREE;
   self->included_range_differences = (TSRangeArray) array_new();
   self->included_range_difference_index = 0;
   ts_parser__set_cached_token(self, 0, NULL_SUBTREE, NULL_SUBTREE);
   return self;
@@ -1866,15 +1888,15 @@
 }
 
 const TSLanguage *ts_parser_language(const TSParser *self) {
   return self->language;
 }
 
 bool ts_parser_set_language(TSParser *self, const TSLanguage *language) {
-  ts_parser__external_scanner_destroy(self);
+  ts_parser_reset(self);
   ts_language_delete(self->language);
   self->language = NULL;
 
   if (language) {
     if (
       language->version > TREE_SITTER_LANGUAGE_VERSION ||
       language->version < TREE_SITTER_MIN_COMPATIBLE_LANGUAGE_VERSION
@@ -1885,16 +1907,14 @@
         !self->wasm_store ||
         !ts_wasm_store_start(self->wasm_store, &self->lexer.data, language)
       ) return false;
     }
   }
 
   self->language = ts_language_copy(language);
-  ts_parser__external_scanner_create(self);
-  ts_parser_reset(self);
   return true;
 }
 
 TSLogger ts_parser_logger(const TSParser *self) {
   return self->lexer.logger;
 }
 
@@ -1943,16 +1963,17 @@
 }
 
 const TSRange *ts_parser_included_ranges(const TSParser *self, uint32_t *count) {
   return ts_lexer_included_ranges(&self->lexer, count);
 }
 
 void ts_parser_reset(TSParser *self) {
-  if (self->language && self->language->external_scanner.deserialize) {
-    self->language->external_scanner.deserialize(self->external_scanner_payload, NULL, 0);
+  ts_parser__external_scanner_destroy(self);
+  if (self->wasm_store) {
+    ts_wasm_store_reset(self->wasm_store);
   }
 
   if (self->old_tree.ptr) {
     ts_subtree_release(&self->tree_pool, self->old_tree);
     self->old_tree = NULL_SUBTREE;
   }
 
@@ -1961,56 +1982,59 @@
   ts_stack_clear(self->stack);
   ts_parser__set_cached_token(self, 0, NULL_SUBTREE, NULL_SUBTREE);
   if (self->finished_tree.ptr) {
     ts_subtree_release(&self->tree_pool, self->finished_tree);
     self->finished_tree = NULL_SUBTREE;
   }
   self->accept_count = 0;
+  self->has_scanner_error = false;
 }
 
 TSTree *ts_parser_parse(
   TSParser *self,
   const TSTree *old_tree,
   TSInput input
 ) {
+  TSTree *result = NULL;
   if (!self->language || !input.read) return NULL;
 
   if (ts_language_is_wasm(self->language)) {
-    if (self->wasm_store) {
-      ts_wasm_store_start(self->wasm_store, &self->lexer.data, self->language);
-    } else {
-      return NULL;
-    }
+    if (!self->wasm_store) return NULL;
+    ts_wasm_store_start(self->wasm_store, &self->lexer.data, self->language);
   }
 
   ts_lexer_set_input(&self->lexer, input);
-
   array_clear(&self->included_range_differences);
   self->included_range_difference_index = 0;
 
   if (ts_parser_has_outstanding_parse(self)) {
     LOG("resume_parsing");
-  } else if (old_tree) {
-    ts_subtree_retain(old_tree->root);
-    self->old_tree = old_tree->root;
-    ts_range_array_get_changed_ranges(
-      old_tree->included_ranges, old_tree->included_range_count,
-      self->lexer.included_ranges, self->lexer.included_range_count,
-      &self->included_range_differences
-    );
-    reusable_node_reset(&self->reusable_node, old_tree->root);
-    LOG("parse_after_edit");
-    LOG_TREE(self->old_tree);
-    for (unsigned i = 0; i < self->included_range_differences.size; i++) {
-      TSRange *range = &self->included_range_differences.contents[i];
-      LOG("different_included_range %u - %u", range->start_byte, range->end_byte);
-    }
   } else {
-    reusable_node_clear(&self->reusable_node);
-    LOG("new_parse");
+    ts_parser__external_scanner_create(self);
+    if (self->has_scanner_error) goto exit;
+
+    if (old_tree) {
+      ts_subtree_retain(old_tree->root);
+      self->old_tree = old_tree->root;
+      ts_range_array_get_changed_ranges(
+        old_tree->included_ranges, old_tree->included_range_count,
+        self->lexer.included_ranges, self->lexer.included_range_count,
+        &self->included_range_differences
+      );
+      reusable_node_reset(&self->reusable_node, old_tree->root);
+      LOG("parse_after_edit");
+      LOG_TREE(self->old_tree);
+      for (unsigned i = 0; i < self->included_range_differences.size; i++) {
+        TSRange *range = &self->included_range_differences.contents[i];
+        LOG("different_included_range %u - %u", range->start_byte, range->end_byte);
+      }
+    } else {
+      reusable_node_clear(&self->reusable_node);
+      LOG("new_parse");
+    }
   }
 
   self->operation_count = 0;
   if (self->timeout_duration) {
     self->end_clock = clock_after(clock_now(), self->timeout_duration);
   } else {
     self->end_clock = clock_null();
@@ -2031,15 +2055,19 @@
           version,
           ts_stack_version_count(self->stack),
           ts_stack_state(self->stack, version),
           ts_stack_position(self->stack, version).extent.row,
           ts_stack_position(self->stack, version).extent.column
         );
 
-        if (!ts_parser__advance(self, version, allow_node_reuse)) return NULL;
+        if (!ts_parser__advance(self, version, allow_node_reuse)) {
+          if (self->has_scanner_error) goto exit;
+          return NULL;
+        }
+
         LOG_STACK();
 
         position = ts_stack_position(self->stack, version).bytes;
         if (position > last_position || (version > 0 && position == last_position)) {
           last_position = position;
           break;
         }
@@ -2070,21 +2098,23 @@
   } while (version_count != 0);
 
   assert(self->finished_tree.ptr);
   ts_subtree_balance(self->finished_tree, &self->tree_pool, self->language);
   LOG("done");
   LOG_TREE(self->finished_tree);
 
-  TSTree *result = ts_tree_new(
+  result = ts_tree_new(
     self->finished_tree,
     self->language,
     self->lexer.included_ranges,
     self->lexer.included_range_count
   );
   self->finished_tree = NULL_SUBTREE;
+
+exit:
   ts_parser_reset(self);
   return result;
 }
 
 TSTree *ts_parser_parse_string(
   TSParser *self,
   const TSTree *old_tree,
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/parser.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/parser.h`

 * *Files 19% similar despite different names*

```diff
@@ -82,14 +82,19 @@
   TSParseAction action;
   struct {
     uint8_t count;
     bool reusable;
   } entry;
 } TSParseActionEntry;
 
+typedef struct {
+  int32_t start;
+  int32_t end;
+} TSCharacterRange;
+
 struct TSLanguage {
   uint32_t version;
   uint32_t symbol_count;
   uint32_t alias_count;
   uint32_t token_count;
   uint32_t external_token_count;
   uint32_t state_count;
@@ -121,14 +126,32 @@
     bool (*scan)(void *, TSLexer *, const bool *symbol_whitelist);
     unsigned (*serialize)(void *, char *);
     void (*deserialize)(void *, const char *, unsigned);
   } external_scanner;
   const TSStateId *primary_state_ids;
 };
 
+static inline bool set_contains(TSCharacterRange *ranges, uint32_t len, int32_t lookahead) {
+  uint32_t index = 0;
+  uint32_t size = len - index;
+  while (size > 1) {
+    uint32_t half_size = size / 2;
+    uint32_t mid_index = index + half_size;
+    TSCharacterRange *range = &ranges[mid_index];
+    if (lookahead >= range->start && lookahead <= range->end) {
+      return true;
+    } else if (lookahead > range->end) {
+      index = mid_index;
+    }
+    size -= half_size;
+  }
+  TSCharacterRange *range = &ranges[index];
+  return (lookahead >= range->start && lookahead <= range->end);
+}
+
 /*
  *  Lexer Macros
  */
 
 #ifdef _MSC_VER
 #define UNUSED __pragma(warning(suppress : 4101))
 #else
@@ -150,14 +173,25 @@
 
 #define ADVANCE(state_value) \
   {                          \
     state = state_value;     \
     goto next_state;         \
   }
 
+#define ADVANCE_MAP(...)                                              \
+  {                                                                   \
+    static const uint16_t map[] = { __VA_ARGS__ };                    \
+    for (uint32_t i = 0; i < sizeof(map) / sizeof(map[0]); i += 2) {  \
+      if (map[i] == lookahead) {                                      \
+        state = map[i + 1];                                           \
+        goto next_state;                                              \
+      }                                                               \
+    }                                                                 \
+  }
+
 #define SKIP(state_value) \
   {                       \
     skip = true;          \
     state = state_value;  \
     goto next_state;      \
   }
 
@@ -199,22 +233,23 @@
   {{                                  \
     .shift = {                        \
       .type = TSParseActionTypeShift, \
       .extra = true                   \
     }                                 \
   }}
 
-#define REDUCE(symbol_val, child_count_val, ...) \
-  {{                                             \
-    .reduce = {                                  \
-      .type = TSParseActionTypeReduce,           \
-      .symbol = symbol_val,                      \
-      .child_count = child_count_val,            \
-      __VA_ARGS__                                \
-    },                                           \
+#define REDUCE(symbol_name, children, precedence, prod_id) \
+  {{                                                       \
+    .reduce = {                                            \
+      .type = TSParseActionTypeReduce,                     \
+      .symbol = symbol_name,                               \
+      .child_count = children,                             \
+      .dynamic_precedence = precedence,                    \
+      .production_id = prod_id                             \
+    },                                                     \
   }}
 
 #define RECOVER()                    \
   {{                                 \
     .type = TSParseActionTypeRecover \
   }}
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/point.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/point.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/query.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/query.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/reduce_action.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/reduce_action.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/reusable_node.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/reusable_node.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/stack.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/stack.c`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/stack.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/stack.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/subtree.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/subtree.c`

 * *Files 2% similar despite different names*

```diff
@@ -886,17 +886,23 @@
           cursor += snprintf(*writer, limit, "\"%s\"", symbol_name);
         }
       } else {
         cursor += snprintf(*writer, limit, "(%s", symbol_name);
       }
     }
   } else if (is_root) {
-    TSSymbol symbol = ts_subtree_symbol(self);
+    TSSymbol symbol = alias_symbol ? alias_symbol : ts_subtree_symbol(self);
     const char *symbol_name = ts_language_symbol_name(language, symbol);
-    cursor += snprintf(*writer, limit, "(\"%s\")", symbol_name);
+    if (ts_subtree_child_count(self) > 0) {
+      cursor += snprintf(*writer, limit, "(%s", symbol_name);
+    } else if (ts_subtree_named(self)) {
+      cursor += snprintf(*writer, limit, "(%s)", symbol_name);
+    } else {
+      cursor += snprintf(*writer, limit, "(\"%s\")", symbol_name);
+    }
   }
 
   if (ts_subtree_child_count(self)) {
     const TSSymbol *alias_sequence = ts_language_alias_sequence(language, self.ptr->production_id);
     const TSFieldMapEntry *field_map, *field_map_end;
     ts_language_field_map(
       language,
@@ -943,28 +949,30 @@
   if (is_visible) cursor += snprintf(*writer, limit, ")");
 
   return cursor - string;
 }
 
 char *ts_subtree_string(
   Subtree self,
+  TSSymbol alias_symbol,
+  bool alias_is_named,
   const TSLanguage *language,
   bool include_all
 ) {
   char scratch_string[1];
   size_t size = ts_subtree__write_to_string(
     self, scratch_string, 1,
     language, include_all,
-    0, false, ROOT_FIELD
+    alias_symbol, alias_is_named, ROOT_FIELD
   ) + 1;
   char *result = ts_malloc(size * sizeof(char));
   ts_subtree__write_to_string(
     self, result, size,
     language, include_all,
-    0, false, ROOT_FIELD
+    alias_symbol, alias_is_named, ROOT_FIELD
   );
   return result;
 }
 
 void ts_subtree__print_dot_graph(const Subtree *self, uint32_t start_offset,
                                  const TSLanguage *language, TSSymbol alias_symbol,
                                  FILE *f) {
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/subtree.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/subtree.h`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,15 @@
 void ts_subtree_release(SubtreePool *, Subtree);
 int ts_subtree_compare(Subtree, Subtree, SubtreePool *);
 void ts_subtree_set_symbol(MutableSubtree *, TSSymbol, const TSLanguage *);
 void ts_subtree_summarize(MutableSubtree, const Subtree *, uint32_t, const TSLanguage *);
 void ts_subtree_summarize_children(MutableSubtree, const TSLanguage *);
 void ts_subtree_balance(Subtree, SubtreePool *, const TSLanguage *);
 Subtree ts_subtree_edit(Subtree, const TSInputEdit *edit, SubtreePool *);
-char *ts_subtree_string(Subtree, const TSLanguage *, bool include_all);
+char *ts_subtree_string(Subtree, TSSymbol, bool, const TSLanguage *, bool include_all);
 void ts_subtree_print_dot_graph(Subtree, const TSLanguage *, FILE *);
 Subtree ts_subtree_last_external_token(Subtree);
 const ExternalScannerState *ts_subtree_external_scanner_state(Subtree self);
 bool ts_subtree_external_scanner_state_eq(Subtree, Subtree);
 
 #define SUBTREE_GET(self, name) ((self).data.is_inline ? (self).data.name : (self).ptr->name)
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/tree.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/tree.c`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,16 @@
   *length = self->included_range_count;
   TSRange *ranges = ts_calloc(self->included_range_count, sizeof(TSRange));
   memcpy(ranges, self->included_ranges, self->included_range_count * sizeof(TSRange));
   return ranges;
 }
 
 TSRange *ts_tree_get_changed_ranges(const TSTree *old_tree, const TSTree *new_tree, uint32_t *length) {
-  TreeCursor cursor1 = {NULL, array_new()};
-  TreeCursor cursor2 = {NULL, array_new()};
+  TreeCursor cursor1 = {NULL, array_new(), 0};
+  TreeCursor cursor2 = {NULL, array_new(), 0};
   ts_tree_cursor_init(&cursor1, ts_tree_root_node(old_tree));
   ts_tree_cursor_init(&cursor2, ts_tree_root_node(new_tree));
 
   TSRangeArray included_range_differences = array_new();
   ts_range_array_get_changed_ranges(
     old_tree->included_ranges, old_tree->included_range_count,
     new_tree->included_ranges, new_tree->included_range_count,
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/tree.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/tree.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/tree_cursor.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/tree_cursor.c`

 * *Files 2% similar despite different names*

```diff
@@ -147,25 +147,26 @@
 
   return true;
 }
 
 // TSTreeCursor - lifecycle
 
 TSTreeCursor ts_tree_cursor_new(TSNode node) {
-  TSTreeCursor self = {NULL, NULL, {0, 0}};
+  TSTreeCursor self = {NULL, NULL, {0, 0, 0}};
   ts_tree_cursor_init((TreeCursor *)&self, node);
   return self;
 }
 
 void ts_tree_cursor_reset(TSTreeCursor *_self, TSNode node) {
   ts_tree_cursor_init((TreeCursor *)_self, node);
 }
 
 void ts_tree_cursor_init(TreeCursor *self, TSNode node) {
   self->tree = node.tree;
+  self->root_alias_symbol = node.context[3];
   array_clear(&self->stack);
   array_push(&self->stack, ((TreeCursorEntry) {
     .subtree = (const Subtree *)node.id,
     .position = {
       ts_node_start_byte(node),
       ts_node_start_point(node)
     },
@@ -470,15 +471,15 @@
   TreeCursorEntry *last_entry = array_back(&self->stack);
   return last_entry->descendant_index;
 }
 
 TSNode ts_tree_cursor_current_node(const TSTreeCursor *_self) {
   const TreeCursor *self = (const TreeCursor *)_self;
   TreeCursorEntry *last_entry = array_back(&self->stack);
-  TSSymbol alias_symbol = 0;
+  TSSymbol alias_symbol = self->root_alias_symbol;
   if (self->stack.size > 1 && !ts_subtree_extra(*last_entry->subtree)) {
     TreeCursorEntry *parent_entry = &self->stack.contents[self->stack.size - 2];
     alias_symbol = ts_language_alias_at(
       self->tree->language,
       parent_entry->subtree->ptr->production_id,
       last_entry->structural_child_index
     );
@@ -693,19 +694,21 @@
 }
 
 TSTreeCursor ts_tree_cursor_copy(const TSTreeCursor *_cursor) {
   const TreeCursor *cursor = (const TreeCursor *)_cursor;
   TSTreeCursor res = {NULL, NULL, {0, 0}};
   TreeCursor *copy = (TreeCursor *)&res;
   copy->tree = cursor->tree;
+  copy->root_alias_symbol = cursor->root_alias_symbol;
   array_init(&copy->stack);
   array_push_all(&copy->stack, &cursor->stack);
   return res;
 }
 
 void ts_tree_cursor_reset_to(TSTreeCursor *_dst, const TSTreeCursor *_src) {
   const TreeCursor *cursor = (const TreeCursor *)_src;
   TreeCursor *copy = (TreeCursor *)_dst;
   copy->tree = cursor->tree;
+  copy->root_alias_symbol = cursor->root_alias_symbol;
   array_clear(&copy->stack);
   array_push_all(&copy->stack, &cursor->stack);
 }
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/tree_cursor.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/tree_cursor.h`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
   uint32_t structural_child_index;
   uint32_t descendant_index;
 } TreeCursorEntry;
 
 typedef struct {
   const TSTree *tree;
   Array(TreeCursorEntry) stack;
+  TSSymbol root_alias_symbol;
 } TreeCursor;
 
 typedef enum {
   TreeCursorStepNone,
   TreeCursorStepHidden,
   TreeCursorStepVisible,
 } TreeCursorStep;
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/LICENSE` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/README.md` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/README.md`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/umachine.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/umachine.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/utf16.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/utf16.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode/utf8.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode/utf8.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/unicode.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/unicode.h`

 * *Files identical despite different names*

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/wasm_store.c` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/wasm_store.c`

 * *Files 5% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 #include "./array.h"
 #include "./atomic.h"
 #include "./language.h"
 #include "./lexer.h"
 #include "./wasm_store.h"
 #include "./wasm/wasm-stdlib.h"
 
+#define array_len(a) (sizeof(a) / sizeof(a[0]))
+
 // The following symbols from the C and C++ standard libraries are available
 // for external scanners to use.
 const char *STDLIB_SYMBOLS[] = {
   #include "./stdlib-symbols.txt"
 };
 
-#define STDLIB_SYMBOL_COUNT (sizeof(STDLIB_SYMBOLS) / sizeof(STDLIB_SYMBOLS[0]))
-
 // The contents of the `dylink.0` custom section of a wasm module,
 // as specified by the current WebAssembly dynamic linking ABI proposal.
 typedef struct {
   uint32_t memory_size;
   uint32_t memory_align;
   uint32_t table_size;
   uint32_t table_align;
@@ -66,31 +66,45 @@
   int32_t scanner_create_fn_index;
   int32_t scanner_destroy_fn_index;
   int32_t scanner_serialize_fn_index;
   int32_t scanner_deserialize_fn_index;
   int32_t scanner_scan_fn_index;
 } LanguageWasmInstance;
 
+typedef struct {
+  uint32_t reset_heap;
+  uint32_t proc_exit;
+  uint32_t abort;
+  uint32_t assert_fail;
+  uint32_t notify_memory_growth;
+  uint32_t debug_message;
+  uint32_t at_exit;
+  uint32_t args_get;
+  uint32_t args_sizes_get;
+} BuiltinFunctionIndices;
+
 // TSWasmStore - A struct that allows a given `Parser` to use wasm-backed
 // languages. This struct is mutable, and can only be used by one parser at a
 // time.
 struct TSWasmStore {
   wasm_engine_t *engine;
   wasmtime_store_t *store;
   wasmtime_table_t function_table;
   wasmtime_memory_t memory;
   TSLexer *current_lexer;
   LanguageWasmInstance *current_instance;
   Array(LanguageWasmInstance) language_instances;
   uint32_t current_memory_offset;
-  uint32_t current_memory_size;
   uint32_t current_function_table_offset;
-  uint16_t *fn_indices;
+  uint32_t *stdlib_fn_indices;
+  BuiltinFunctionIndices builtin_fn_indices;
+  wasmtime_global_t stack_pointer_global;
   wasm_globaltype_t *const_i32_type;
-  wasm_globaltype_t *var_i32_type;
+  bool has_error;
+  uint32_t lexer_address;
 };
 
 typedef Array(char) StringData;
 
 // LanguageInWasmMemory - The memory layout of a `TSLanguage` when compiled to
 // wasm32. This is used to copy static language data out of the wasm memory.
 typedef struct {
@@ -143,37 +157,16 @@
   int32_t is_at_included_range_start;
   int32_t eof;
 } LexerInWasmMemory;
 
 static volatile uint32_t NEXT_LANGUAGE_ID;
 
 // Linear memory layout:
-// [ <-- stack | built-in data | heap --> | static data ]
-#define STACK_SIZE (64 * 1024)
-#define HEAP_SIZE (1024 * 1024)
-#define INITIAL_MEMORY_SIZE (4 * 1024 * 1024 / MEMORY_PAGE_SIZE)
-#define MAX_MEMORY_SIZE 32768
-#define SERIALIZATION_BUFFER_ADDRESS (STACK_SIZE)
-#define LEXER_ADDRESS (SERIALIZATION_BUFFER_ADDRESS + TREE_SITTER_SERIALIZATION_BUFFER_SIZE)
-#define HEAP_START_ADDRESS (LEXER_ADDRESS + sizeof(LexerInWasmMemory))
-#define DATA_START_ADDRESS (HEAP_START_ADDRESS + HEAP_SIZE)
-
-enum FunctionIx {
-  NULL_IX = 0,
-  PROC_EXIT_IX,
-  ABORT_IX,
-  ASSERT_FAIL_IX,
-  NOTIFY_MEMORY_GROWTH_IX,
-  AT_EXIT_IX,
-  LEXER_ADVANCE_IX,
-  LEXER_MARK_END_IX,
-  LEXER_GET_COLUMN_IX,
-  LEXER_IS_AT_INCLUDED_RANGE_START_IX,
-  LEXER_EOF_IX,
-};
+// [ <-- stack | stdlib statics | lexer | language statics --> | serialization_buffer | heap --> ]
+#define MAX_MEMORY_SIZE (128 * 1024 * 1024 / MEMORY_PAGE_SIZE)
 
 /************************
  * WasmDylinkMemoryInfo
  ***********************/
 
 static uint8_t read_u8(const uint8_t **p, const uint8_t *end) {
   return *(*p)++;
@@ -243,35 +236,40 @@
   return false;
 }
 
 /*******************************************
  * Native callbacks exposed to wasm modules
  *******************************************/
 
- static wasm_trap_t *callback__exit(
+ static wasm_trap_t *callback__abort(
   void *env,
   wasmtime_caller_t* caller,
   wasmtime_val_raw_t *args_and_results,
   size_t args_and_results_len
 ) {
-  fprintf(stderr, "wasm module called exit");
-  abort();
+  return wasmtime_trap_new("wasm module called abort", 24);
 }
 
-static wasm_trap_t *callback__notify_memory_growth(
+static wasm_trap_t *callback__debug_message(
   void *env,
   wasmtime_caller_t* caller,
   wasmtime_val_raw_t *args_and_results,
   size_t args_and_results_len
 ) {
-  fprintf(stderr, "wasm module called exit");
-  abort();
+  wasmtime_context_t *context = wasmtime_caller_context(caller);
+  TSWasmStore *store = env;
+  assert(args_and_results_len == 2);
+  uint32_t string_address = args_and_results[0].i32;
+  uint32_t value = args_and_results[1].i32;
+  uint8_t *memory = wasmtime_memory_data(context, &store->memory);
+  printf("DEBUG: %s %u\n", &memory[string_address], value);
+  return NULL;
 }
 
-static wasm_trap_t *callback__at_exit(
+static wasm_trap_t *callback__noop(
   void *env,
   wasmtime_caller_t* caller,
   wasmtime_val_raw_t *args_and_results,
   size_t args_and_results_len
 ) {
   return NULL;
 }
@@ -287,15 +285,15 @@
 
   TSWasmStore *store = env;
   TSLexer *lexer = store->current_lexer;
   bool skip = args_and_results[1].i32;
   lexer->advance(lexer, skip);
 
   uint8_t *memory = wasmtime_memory_data(context, &store->memory);
-  memcpy(&memory[LEXER_ADDRESS], &lexer->lookahead, sizeof(lexer->lookahead));
+  memcpy(&memory[store->lexer_address], &lexer->lookahead, sizeof(lexer->lookahead));
   return NULL;
 }
 
 static wasm_trap_t *callback__lexer_mark_end(
   void *env,
   wasmtime_caller_t* caller,
   wasmtime_val_raw_t *args_and_results,
@@ -343,20 +341,19 @@
   TSLexer *lexer = store->current_lexer;
   bool result = lexer->eof(lexer);
   args_and_results[0].i32 = result;
   return NULL;
 }
 
 typedef struct {
+  uint32_t *storage_location;
   wasmtime_func_unchecked_callback_t callback;
   wasm_functype_t *type;
 } FunctionDefinition;
 
-#define array_len(a) (sizeof(a) / sizeof(a[0]))
-
 static void *copy(const void *data, size_t size) {
   void *result = ts_malloc(size);
   memcpy(result, data, size);
   return result;
 }
 
 static void *copy_unsized_static_array(
@@ -423,25 +420,14 @@
   wasm_valtype_t* ps[4] = {p1, p2, p3, p4};
   wasm_valtype_vec_t params, results;
   wasm_valtype_vec_new(&params, 4, ps);
   wasm_valtype_vec_new_empty(&results);
   return wasm_functype_new(&params, &results);
 }
 
-static wasmtime_extern_t get_builtin_func_extern(
-  wasmtime_context_t *context,
-  wasmtime_table_t *table,
-  unsigned index
-) {
-  wasmtime_val_t val;
-  bool exists = wasmtime_table_get(context, table, index, &val);
-  assert(exists);
-  return (wasmtime_extern_t) {.kind = WASMTIME_EXTERN_FUNC, .of.func = val.of.funcref};
-}
-
 #define format(output, ...) \
   do { \
     size_t message_length = snprintf((char *)NULL, 0, __VA_ARGS__); \
     *output = ts_malloc(message_length + 1); \
     snprintf(*output, message_length + 1, __VA_ARGS__); \
   } while (0)
 
@@ -459,14 +445,27 @@
 
 void language_id_delete(WasmLanguageId *self) {
   if (atomic_dec(&self->ref_count) == 0) {
     ts_free(self);
   }
 }
 
+static wasmtime_extern_t get_builtin_extern(
+  wasmtime_table_t *table,
+  unsigned index
+) {
+  return (wasmtime_extern_t) {
+    .kind = WASMTIME_EXTERN_FUNC,
+    .of.func = (wasmtime_func_t) {
+      .store_id = table->store_id,
+      .index = index
+    }
+  };
+}
+
 static bool ts_wasm_store__provide_builtin_import(
   TSWasmStore *self,
   const wasm_name_t *import_name,
   wasmtime_extern_t *import
 ) {
   wasmtime_error_t *error = NULL;
   wasmtime_context_t *context = wasmtime_store_context(self->store);
@@ -480,43 +479,39 @@
     *import = (wasmtime_extern_t) {.kind = WASMTIME_EXTERN_GLOBAL, .of.global = global};
   } else if (name_eq(import_name, "__table_base")) {
     wasmtime_val_t value = WASM_I32_VAL(self->current_function_table_offset);
     wasmtime_global_t global;
     error = wasmtime_global_new(context, self->const_i32_type, &value, &global);
     assert(!error);
     *import = (wasmtime_extern_t) {.kind = WASMTIME_EXTERN_GLOBAL, .of.global = global};
-  } else if (name_eq(import_name, "__heap_base")) {
-    wasmtime_val_t value = WASM_I32_VAL(HEAP_START_ADDRESS);
-    wasmtime_global_t global;
-    error = wasmtime_global_new(context, self->var_i32_type, &value, &global);
-    assert(!error);
-    *import = (wasmtime_extern_t) {.kind = WASMTIME_EXTERN_GLOBAL, .of.global = global};
   } else if (name_eq(import_name, "__stack_pointer")) {
-    wasmtime_val_t value = WASM_I32_VAL(STACK_SIZE);
-    wasmtime_global_t global;
-    error = wasmtime_global_new(context, self->var_i32_type, &value, &global);
-    assert(!error);
-    *import = (wasmtime_extern_t) {.kind = WASMTIME_EXTERN_GLOBAL, .of.global = global};
+    *import = (wasmtime_extern_t) {.kind = WASMTIME_EXTERN_GLOBAL, .of.global = self->stack_pointer_global};
   } else if (name_eq(import_name, "__indirect_function_table")) {
     *import = (wasmtime_extern_t) {.kind = WASMTIME_EXTERN_TABLE, .of.table = self->function_table};
   } else if (name_eq(import_name, "memory")) {
     *import = (wasmtime_extern_t) {.kind = WASMTIME_EXTERN_MEMORY, .of.memory = self->memory};
   }
 
   // Builtin functions
   else if (name_eq(import_name, "__assert_fail")) {
-    *import = get_builtin_func_extern(context, &self->function_table, ASSERT_FAIL_IX);
+    *import = get_builtin_extern(&self->function_table, self->builtin_fn_indices.assert_fail);
   } else if (name_eq(import_name, "__cxa_atexit")) {
-    *import = get_builtin_func_extern(context, &self->function_table, AT_EXIT_IX);
+    *import = get_builtin_extern(&self->function_table, self->builtin_fn_indices.at_exit);
+  } else if (name_eq(import_name, "args_get")) {
+    *import = get_builtin_extern(&self->function_table, self->builtin_fn_indices.args_get);
+  } else if (name_eq(import_name, "args_sizes_get")) {
+    *import = get_builtin_extern(&self->function_table, self->builtin_fn_indices.args_sizes_get);
   } else if (name_eq(import_name, "abort")) {
-    *import = get_builtin_func_extern(context, &self->function_table, ABORT_IX);
+    *import = get_builtin_extern(&self->function_table, self->builtin_fn_indices.abort);
   } else if (name_eq(import_name, "proc_exit")) {
-    *import = get_builtin_func_extern(context, &self->function_table, PROC_EXIT_IX);
+    *import = get_builtin_extern(&self->function_table, self->builtin_fn_indices.proc_exit);
   } else if (name_eq(import_name, "emscripten_notify_memory_growth")) {
-    *import = get_builtin_func_extern(context, &self->function_table, NOTIFY_MEMORY_GROWTH_IX);
+    *import = get_builtin_extern(&self->function_table, self->builtin_fn_indices.notify_memory_growth);
+  } else if (name_eq(import_name, "tree_sitter_debug_message")) {
+    *import = get_builtin_extern(&self->function_table, self->builtin_fn_indices.debug_message);
   } else {
     return false;
   }
 
   return true;
 }
 
@@ -524,161 +519,236 @@
   TSWasmStore *self,
   const wasm_name_t *export_name,
   wasmtime_extern_t *export,
   wasm_trap_t **trap
 ) {
   if (
     name_eq(export_name, "_initialize") ||
-    name_eq(export_name, "__wasm_apply_data_relocs")
+    name_eq(export_name, "__wasm_apply_data_relocs") ||
+    name_eq(export_name, "__wasm_call_ctors")
   ) {
     wasmtime_context_t *context = wasmtime_store_context(self->store);
     wasmtime_func_t initialization_func = export->of.func;
     wasmtime_error_t *error = wasmtime_func_call(context, &initialization_func, NULL, 0, NULL, 0, trap);
     assert(!error);
     return true;
   } else {
     return false;
   }
 }
 
 TSWasmStore *ts_wasm_store_new(TSWasmEngine *engine, TSWasmError *wasm_error) {
-  TSWasmStore *self = ts_malloc(sizeof(TSWasmStore));
+  TSWasmStore *self = ts_calloc(1, sizeof(TSWasmStore));
   wasmtime_store_t *store = wasmtime_store_new(engine, self, NULL);
   wasmtime_context_t *context = wasmtime_store_context(store);
   wasmtime_error_t *error = NULL;
   wasm_trap_t *trap = NULL;
   wasm_message_t message = WASM_EMPTY_VEC;
   wasm_exporttype_vec_t export_types = WASM_EMPTY_VEC;
   wasmtime_extern_t *imports = NULL;
+  wasmtime_module_t *stdlib_module = NULL;
+  wasm_memorytype_t *memory_type = NULL;
+  wasm_tabletype_t *table_type = NULL;
 
-  // Initialize store's memory
-  wasm_limits_t memory_limits = {.min = INITIAL_MEMORY_SIZE, .max = MAX_MEMORY_SIZE};
-  wasm_memorytype_t *memory_type = wasm_memorytype_new(&memory_limits);
-  wasmtime_memory_t memory;
-  error = wasmtime_memory_new(context, memory_type, &memory);
+  // Define functions called by scanners via function pointers on the lexer.
+  LexerInWasmMemory lexer = {
+    .lookahead = 0,
+    .result_symbol = 0,
+  };
+  FunctionDefinition lexer_definitions[] = {
+    {
+      (uint32_t *)&lexer.advance,
+      callback__lexer_advance,
+      wasm_functype_new_2_0(wasm_valtype_new_i32(), wasm_valtype_new_i32())
+    },
+    {
+      (uint32_t *)&lexer.mark_end,
+      callback__lexer_mark_end,
+      wasm_functype_new_1_0(wasm_valtype_new_i32())
+    },
+    {
+      (uint32_t *)&lexer.get_column,
+      callback__lexer_get_column,
+      wasm_functype_new_1_1(wasm_valtype_new_i32(), wasm_valtype_new_i32())
+    },
+    {
+      (uint32_t *)&lexer.is_at_included_range_start,
+      callback__lexer_is_at_included_range_start,
+      wasm_functype_new_1_1(wasm_valtype_new_i32(), wasm_valtype_new_i32())
+    },
+    {
+      (uint32_t *)&lexer.eof,
+      callback__lexer_eof,
+      wasm_functype_new_1_1(wasm_valtype_new_i32(), wasm_valtype_new_i32())
+    },
+  };
+
+  // Define builtin functions that can be imported by scanners.
+  BuiltinFunctionIndices builtin_fn_indices;
+  FunctionDefinition builtin_definitions[] = {
+    {
+      &builtin_fn_indices.proc_exit,
+      callback__abort,
+      wasm_functype_new_1_0(wasm_valtype_new_i32())
+    },
+    {
+      &builtin_fn_indices.abort,
+      callback__abort,
+      wasm_functype_new_0_0()
+    },
+    {
+      &builtin_fn_indices.assert_fail,
+      callback__abort,
+      wasm_functype_new_4_0(wasm_valtype_new_i32(), wasm_valtype_new_i32(), wasm_valtype_new_i32(), wasm_valtype_new_i32())
+    },
+    {
+      &builtin_fn_indices.notify_memory_growth,
+      callback__noop,
+      wasm_functype_new_1_0(wasm_valtype_new_i32())
+    },
+    {
+      &builtin_fn_indices.debug_message,
+      callback__debug_message,
+      wasm_functype_new_2_0(wasm_valtype_new_i32(), wasm_valtype_new_i32())
+    },
+    {
+      &builtin_fn_indices.at_exit,
+      callback__noop,
+      wasm_functype_new_3_1(wasm_valtype_new_i32(), wasm_valtype_new_i32(), wasm_valtype_new_i32(), wasm_valtype_new_i32())
+    },
+    {
+      &builtin_fn_indices.args_get,
+      callback__noop,
+      wasm_functype_new_2_1(wasm_valtype_new_i32(), wasm_valtype_new_i32(), wasm_valtype_new_i32())
+    },
+    {
+      &builtin_fn_indices.args_sizes_get,
+      callback__noop,
+      wasm_functype_new_2_1(wasm_valtype_new_i32(), wasm_valtype_new_i32(), wasm_valtype_new_i32())
+    },
+  };
+
+  // Create all of the wasm functions.
+  unsigned builtin_definitions_len = array_len(builtin_definitions);
+  unsigned lexer_definitions_len = array_len(lexer_definitions);
+  for (unsigned i = 0; i < builtin_definitions_len; i++) {
+    FunctionDefinition *definition = &builtin_definitions[i];
+    wasmtime_func_t func;
+    wasmtime_func_new_unchecked(context, definition->type, definition->callback, self, NULL, &func);
+    *definition->storage_location = func.index;
+    wasm_functype_delete(definition->type);
+  }
+  for (unsigned i = 0; i < lexer_definitions_len; i++) {
+    FunctionDefinition *definition = &lexer_definitions[i];
+    wasmtime_func_t func;
+    wasmtime_func_new_unchecked(context, definition->type, definition->callback, self, NULL, &func);
+    *definition->storage_location = func.index;
+    wasm_functype_delete(definition->type);
+  }
+
+  // Compile the stdlib module.
+  error = wasmtime_module_new(engine, STDLIB_WASM, STDLIB_WASM_LEN, &stdlib_module);
   if (error) {
     wasmtime_error_message(error, &message);
-    wasm_error->kind = TSWasmErrorKindAllocate;
+    wasm_error->kind = TSWasmErrorKindCompile;
     format(
       &wasm_error->message,
-      "failed to allocate wasm memory: %.*s",
+      "failed to compile wasm stdlib: %.*s",
       (int)message.size, message.data
     );
     goto error;
   }
-  wasm_memorytype_delete(memory_type);
 
-  // Initialize lexer struct with function pointers in wasm memory.
-  uint8_t *memory_data = wasmtime_memory_data(context, &memory);
-  LexerInWasmMemory lexer = {
-    .lookahead = 0,
-    .result_symbol = 0,
-    .advance = LEXER_ADVANCE_IX,
-    .mark_end = LEXER_MARK_END_IX,
-    .get_column = LEXER_GET_COLUMN_IX,
-    .is_at_included_range_start = LEXER_IS_AT_INCLUDED_RANGE_START_IX,
-    .eof = LEXER_EOF_IX,
-  };
-  memcpy(&memory_data[LEXER_ADDRESS], &lexer, sizeof(lexer));
+  // Retrieve the stdlib module's imports.
+  wasm_importtype_vec_t import_types = WASM_EMPTY_VEC;
+  wasmtime_module_imports(stdlib_module, &import_types);
 
-  // Define builtin functions.
-  FunctionDefinition definitions[] = {
-    [NULL_IX] = {NULL, NULL},
-    [PROC_EXIT_IX] = {callback__exit, wasm_functype_new_1_0(wasm_valtype_new_i32())},
-    [ABORT_IX] = {callback__exit, wasm_functype_new_0_0()},
-    [ASSERT_FAIL_IX] = {callback__exit, wasm_functype_new_4_0(wasm_valtype_new_i32(), wasm_valtype_new_i32(), wasm_valtype_new_i32(), wasm_valtype_new_i32())},
-    [NOTIFY_MEMORY_GROWTH_IX] = {callback__notify_memory_growth, wasm_functype_new_1_0(wasm_valtype_new_i32())},
-    [AT_EXIT_IX] = {callback__at_exit, wasm_functype_new_3_1(wasm_valtype_new_i32(), wasm_valtype_new_i32(), wasm_valtype_new_i32(), wasm_valtype_new_i32())},
-    [LEXER_ADVANCE_IX] = {callback__lexer_advance, wasm_functype_new_2_0(wasm_valtype_new_i32(), wasm_valtype_new_i32())},
-    [LEXER_MARK_END_IX] = {callback__lexer_mark_end, wasm_functype_new_1_0(wasm_valtype_new_i32())},
-    [LEXER_GET_COLUMN_IX] = {callback__lexer_get_column, wasm_functype_new_1_1(wasm_valtype_new_i32(), wasm_valtype_new_i32())},
-    [LEXER_IS_AT_INCLUDED_RANGE_START_IX] = {callback__lexer_is_at_included_range_start, wasm_functype_new_1_1(wasm_valtype_new_i32(), wasm_valtype_new_i32())},
-    [LEXER_EOF_IX] = {callback__lexer_eof, wasm_functype_new_1_1(wasm_valtype_new_i32(), wasm_valtype_new_i32())},
-  };
-  unsigned definitions_len = array_len(definitions);
+  // Find the initial number of memory pages needed by the stdlib.
+  const wasm_memorytype_t *stdlib_memory_type;
+  for (unsigned i = 0; i < import_types.size; i++) {
+    wasm_importtype_t *import_type = import_types.data[i];
+    const wasm_name_t *import_name = wasm_importtype_name(import_type);
+    if (name_eq(import_name, "memory")) {
+      const wasm_externtype_t *type = wasm_importtype_type(import_type);
+      stdlib_memory_type = wasm_externtype_as_memorytype_const(type);
+    }
+  }
+  if (!stdlib_memory_type) {
+    wasm_error->kind = TSWasmErrorKindCompile;
+    format(
+      &wasm_error->message,
+      "wasm stdlib is missing the 'memory' import"
+    );
+    goto error;
+  }
 
-  // Add builtin functions to the store's function table.
-  wasmtime_table_t function_table;
-  wasm_limits_t table_limits = {.min = definitions_len, .max = wasm_limits_max_default};
-  wasm_tabletype_t *table_type = wasm_tabletype_new(wasm_valtype_new(WASM_FUNCREF), &table_limits);
-  wasmtime_val_t initializer = {.kind = WASMTIME_FUNCREF};
-  error = wasmtime_table_new(context, table_type, &initializer, &function_table);
+  // Initialize store's memory
+  uint64_t initial_memory_pages = wasmtime_memorytype_minimum(stdlib_memory_type);
+  wasm_limits_t memory_limits = {.min = initial_memory_pages, .max = MAX_MEMORY_SIZE};
+  memory_type = wasm_memorytype_new(&memory_limits);
+  wasmtime_memory_t memory;
+  error = wasmtime_memory_new(context, memory_type, &memory);
   if (error) {
     wasmtime_error_message(error, &message);
     wasm_error->kind = TSWasmErrorKindAllocate;
     format(
       &wasm_error->message,
-      "failed to allocate wasm table: %.*s",
+      "failed to allocate wasm memory: %.*s",
       (int)message.size, message.data
     );
     goto error;
   }
-  wasm_tabletype_delete(table_type);
+  wasm_memorytype_delete(memory_type);
+  memory_type = NULL;
 
-  uint32_t prev_size;
-  error = wasmtime_table_grow(context, &function_table, definitions_len, &initializer, &prev_size);
+  // Initialize store's function table
+  wasm_limits_t table_limits = {.min = 1, .max = wasm_limits_max_default};
+  table_type = wasm_tabletype_new(wasm_valtype_new(WASM_FUNCREF), &table_limits);
+  wasmtime_val_t initializer = {.kind = WASMTIME_FUNCREF};
+  wasmtime_table_t function_table;
+  error = wasmtime_table_new(context, table_type, &initializer, &function_table);
   if (error) {
     wasmtime_error_message(error, &message);
     wasm_error->kind = TSWasmErrorKindAllocate;
     format(
       &wasm_error->message,
-      "failed to grow wasm table to initial size: %.*s",
+      "failed to allocate wasm table: %.*s",
       (int)message.size, message.data
     );
     goto error;
   }
+  wasm_tabletype_delete(table_type);
+  table_type = NULL;
 
-  for (unsigned i = 1; i < definitions_len; i++) {
-    FunctionDefinition *definition = &definitions[i];
-    wasmtime_func_t func;
-    wasmtime_func_new_unchecked(context, definition->type, definition->callback, self, NULL, &func);
-    wasmtime_val_t func_val = {.kind = WASMTIME_FUNCREF, .of.funcref = func};
-    error = wasmtime_table_set(context, &function_table, i, &func_val);
-    assert(!error);
-    wasm_functype_delete(definition->type);
-  }
+  unsigned stdlib_symbols_len = array_len(STDLIB_SYMBOLS);
+
+  // Define globals for the stack and heap start addresses.
+  wasm_globaltype_t *const_i32_type = wasm_globaltype_new(wasm_valtype_new_i32(), WASM_CONST);
+  wasm_globaltype_t *var_i32_type = wasm_globaltype_new(wasm_valtype_new_i32(), WASM_VAR);
+
+  wasmtime_val_t stack_pointer_value = WASM_I32_VAL(0);
+  wasmtime_global_t stack_pointer_global;
+  error = wasmtime_global_new(context, var_i32_type, &stack_pointer_value, &stack_pointer_global);
+  assert(!error);
 
   *self = (TSWasmStore) {
-    .store = store,
     .engine = engine,
+    .store = store,
     .memory = memory,
-    .language_instances = array_new(),
     .function_table = function_table,
+    .language_instances = array_new(),
+    .stdlib_fn_indices = ts_calloc(stdlib_symbols_len, sizeof(uint32_t)),
+    .builtin_fn_indices = builtin_fn_indices,
+    .stack_pointer_global = stack_pointer_global,
     .current_memory_offset = 0,
-    .fn_indices = ts_calloc(STDLIB_SYMBOL_COUNT, sizeof(uint16_t)),
-    .current_memory_size = 64 * MEMORY_PAGE_SIZE,
-    .current_function_table_offset = definitions_len,
-    .const_i32_type = wasm_globaltype_new(wasm_valtype_new_i32(), WASM_CONST),
-    .var_i32_type = wasm_globaltype_new(wasm_valtype_new_i32(), WASM_VAR),
+    .current_function_table_offset = 0,
+    .const_i32_type = const_i32_type,
   };
 
-  WasmDylinkInfo dylink_info;
-  if (!wasm_dylink_info__parse(STDLIB_WASM, STDLIB_WASM_LEN, &dylink_info)) {
-    wasm_error->kind = TSWasmErrorKindParse;
-    format(&wasm_error->message, "failed to parse wasm stdlib");
-    goto error;
-  }
-
-  wasmtime_module_t *stdlib_module;
-  error = wasmtime_module_new(engine, STDLIB_WASM, STDLIB_WASM_LEN, &stdlib_module);
-  if (error) {
-    wasmtime_error_message(error, &message);
-    wasm_error->kind = TSWasmErrorKindCompile;
-    format(
-      &wasm_error->message,
-      "failed to compile wasm stdlib: %.*s",
-      (int)message.size, message.data
-    );
-    goto error;
-  }
-
-  wasmtime_instance_t instance;
-  wasm_importtype_vec_t import_types = WASM_EMPTY_VEC;
-  wasmtime_module_imports(stdlib_module, &import_types);
-
+  // Set up the imports for the stdlib module.
   imports = ts_calloc(import_types.size, sizeof(wasmtime_extern_t));
   for (unsigned i = 0; i < import_types.size; i++) {
     wasm_importtype_t *type = import_types.data[i];
     const wasm_name_t *import_name = wasm_importtype_name(type);
     if (!ts_wasm_store__provide_builtin_import(self, import_name, &imports[i])) {
       wasm_error->kind = TSWasmErrorKindInstantiate;
       format(
@@ -686,14 +756,16 @@
         "unexpected import in wasm stdlib: %.*s\n",
         (int)import_name->size, import_name->data
       );
       goto error;
     }
   }
 
+  // Instantiate the stdlib module.
+  wasmtime_instance_t instance;
   error = wasmtime_instance_new(context, stdlib_module, imports, import_types.size, &instance, &trap);
   ts_free(imports);
   imports = NULL;
   if (error) {
     wasmtime_error_message(error, &message);
     wasm_error->kind = TSWasmErrorKindInstantiate;
     format(
@@ -711,33 +783,35 @@
       "trapped when instantiating wasm stdlib module: %.*s",
       (int)message.size, message.data
     );
     goto error;
   }
   wasm_importtype_vec_delete(&import_types);
 
-  self->current_memory_offset = DATA_START_ADDRESS + dylink_info.memory_size;
-  self->current_function_table_offset += dylink_info.table_size;
-
-  for (unsigned i = 0; i < STDLIB_SYMBOL_COUNT; i++) {
-    self->fn_indices[i] = UINT16_MAX;
-  }
-
   // Process the stdlib module's exports.
+  for (unsigned i = 0; i < stdlib_symbols_len; i++) {
+    self->stdlib_fn_indices[i] = UINT32_MAX;
+  }
   wasmtime_module_exports(stdlib_module, &export_types);
   for (unsigned i = 0; i < export_types.size; i++) {
     wasm_exporttype_t *export_type = export_types.data[i];
     const wasm_name_t *name = wasm_exporttype_name(export_type);
 
     char *export_name;
     size_t name_len;
     wasmtime_extern_t export = {.kind = WASM_EXTERN_GLOBAL};
     bool exists = wasmtime_instance_export_nth(context, &instance, i, &export_name, &name_len, &export);
     assert(exists);
 
+    if (export.kind == WASMTIME_EXTERN_GLOBAL) {
+      if (name_eq(name, "__stack_pointer")) {
+        self->stack_pointer_global = export.of.global;
+      }
+    }
+
     if (export.kind == WASMTIME_EXTERN_FUNC) {
       if (ts_wasm_store__call_module_initializer(self, name, &export, &trap)) {
         if (trap) {
           wasm_trap_message(trap, &message);
           wasm_error->kind = TSWasmErrorKindInstantiate;
           format(
             &wasm_error->message,
@@ -745,54 +819,108 @@
             (int)message.size, message.data
           );
           goto error;
         }
         continue;
       }
 
-      for (unsigned j = 0; j < array_len(STDLIB_SYMBOLS); j++) {
+      if (name_eq(name, "reset_heap")) {
+        self->builtin_fn_indices.reset_heap = export.of.func.index;
+        continue;
+      }
+
+      for (unsigned j = 0; j < stdlib_symbols_len; j++) {
         if (name_eq(name, STDLIB_SYMBOLS[j])) {
-          self->fn_indices[j] = export.of.func.index;
+          self->stdlib_fn_indices[j] = export.of.func.index;
           break;
         }
       }
     }
   }
 
-  for (unsigned i = 0; i < STDLIB_SYMBOL_COUNT; i++) {
-    if (self->fn_indices[i] == UINT16_MAX) {
+  if (self->builtin_fn_indices.reset_heap == UINT32_MAX) {
+    wasm_error->kind = TSWasmErrorKindInstantiate;
+    format(
+      &wasm_error->message,
+      "missing malloc reset function in wasm stdlib"
+    );
+    goto error;
+  }
+
+  for (unsigned i = 0; i < stdlib_symbols_len; i++) {
+    if (self->stdlib_fn_indices[i] == UINT32_MAX) {
       wasm_error->kind = TSWasmErrorKindInstantiate;
       format(
         &wasm_error->message,
         "missing exported symbol in wasm stdlib: %s",
         STDLIB_SYMBOLS[i]
       );
       goto error;
     }
   }
 
   wasm_exporttype_vec_delete(&export_types);
+  wasmtime_module_delete(stdlib_module);
+
+  // Add all of the lexer callback functions to the function table. Store their function table
+  // indices on the in-memory lexer.
+  uint32_t table_index;
+  error = wasmtime_table_grow(context, &function_table, lexer_definitions_len, &initializer, &table_index);
+  if (error) {
+    wasmtime_error_message(error, &message);
+    wasm_error->kind = TSWasmErrorKindAllocate;
+    format(
+      &wasm_error->message,
+      "failed to grow wasm table to initial size: %.*s",
+      (int)message.size, message.data
+    );
+    goto error;
+  }
+  for (unsigned i = 0; i < lexer_definitions_len; i++) {
+    FunctionDefinition *definition = &lexer_definitions[i];
+    wasmtime_func_t func = {function_table.store_id, *definition->storage_location};
+    wasmtime_val_t func_val = {.kind = WASMTIME_FUNCREF, .of.funcref = func};
+    error = wasmtime_table_set(context, &function_table, table_index, &func_val);
+    assert(!error);
+    *(int32_t *)(definition->storage_location) = table_index;
+    table_index++;
+  }
+
+  self->current_function_table_offset = table_index;
+  self->lexer_address = initial_memory_pages * MEMORY_PAGE_SIZE;
+  self->current_memory_offset = self->lexer_address + sizeof(LexerInWasmMemory);
+
+  // Grow the memory enough to hold the builtin lexer and serialization buffer.
+  uint32_t new_pages_needed = (self->current_memory_offset - self->lexer_address - 1) / MEMORY_PAGE_SIZE + 1;
+  uint64_t prev_memory_size;
+  wasmtime_memory_grow(context, &memory, new_pages_needed, &prev_memory_size);
+
+  uint8_t *memory_data = wasmtime_memory_data(context, &memory);
+  memcpy(&memory_data[self->lexer_address], &lexer, sizeof(lexer));
   return self;
 
 error:
   ts_free(self);
+  if (stdlib_module) wasmtime_module_delete(stdlib_module);
   if (store) wasmtime_store_delete(store);
+  if (import_types.size) wasm_importtype_vec_delete(&import_types);
+  if (memory_type) wasm_memorytype_delete(memory_type);
+  if (table_type) wasm_tabletype_delete(table_type);
   if (trap) wasm_trap_delete(trap);
   if (error) wasmtime_error_delete(error);
   if (message.size) wasm_byte_vec_delete(&message);
   if (export_types.size) wasm_exporttype_vec_delete(&export_types);
   if (imports) ts_free(imports);
   return NULL;
 }
 
 void ts_wasm_store_delete(TSWasmStore *self) {
   if (!self) return;
-  ts_free(self->fn_indices);
+  ts_free(self->stdlib_fn_indices);
   wasm_globaltype_delete(self->const_i32_type);
-  wasm_globaltype_delete(self->var_i32_type);
   wasmtime_store_delete(self->store);
   wasm_engine_delete(self->engine);
   for (unsigned i = 0; i < self->language_instances.size; i++) {
     LanguageWasmInstance *instance = &self->language_instances.contents[i];
     language_id_delete(instance->language_id);
   }
   array_delete(&self->language_instances);
@@ -806,14 +934,22 @@
     if (!id->is_language_deleted) {
       result++;
     }
   }
   return result;
 }
 
+static uint32_t ts_wasm_store__heap_address(TSWasmStore *self) {
+  return self->current_memory_offset + TREE_SITTER_SERIALIZATION_BUFFER_SIZE;
+}
+
+static uint32_t ts_wasm_store__serialization_buffer_address(TSWasmStore *self) {
+  return self->current_memory_offset;
+}
+
 static bool ts_wasm_store__instantiate(
   TSWasmStore *self,
   wasmtime_module_t *module,
   const char *language_name,
   const WasmDylinkInfo *dylink_info,
   wasmtime_instance_t *result,
   int32_t *language_address,
@@ -832,26 +968,26 @@
   error = wasmtime_table_grow(context, &self->function_table, dylink_info->table_size, &initializer, &prev_table_size);
   if (error) {
     format(error_message, "invalid function table size %u", dylink_info->table_size);
     goto error;
   }
 
   // Grow the memory to make room for the new data.
-  uint32_t needed_memory_size = self->current_memory_offset + dylink_info->memory_size;
-  if (needed_memory_size > self->current_memory_size) {
+  uint32_t needed_memory_size = ts_wasm_store__heap_address(self) + dylink_info->memory_size;
+  uint32_t current_memory_size = wasmtime_memory_data_size(context, &self->memory);
+  if (needed_memory_size > current_memory_size) {
     uint32_t pages_to_grow = (
-      needed_memory_size - self->current_memory_size + MEMORY_PAGE_SIZE - 1) /
+      needed_memory_size - current_memory_size + MEMORY_PAGE_SIZE - 1) /
       MEMORY_PAGE_SIZE;
     uint64_t prev_memory_size;
     error = wasmtime_memory_grow(context, &self->memory, pages_to_grow, &prev_memory_size);
     if (error) {
       format(error_message, "invalid memory size %u", dylink_info->memory_size);
       goto error;
     }
-    self->current_memory_size += pages_to_grow * MEMORY_PAGE_SIZE;
   }
 
   // Construct the language function name as string.
   format(&language_function_name, "tree_sitter_%s", language_name);
 
   const uint64_t store_id = self->function_table.store_id;
 
@@ -871,15 +1007,15 @@
     if (ts_wasm_store__provide_builtin_import(self, import_name, &imports[i])) {
       continue;
     }
 
     bool defined_in_stdlib = false;
     for (unsigned j = 0; j < array_len(STDLIB_SYMBOLS); j++) {
       if (name_eq(import_name, STDLIB_SYMBOLS[j])) {
-        uint16_t address = self->fn_indices[j];
+        uint16_t address = self->stdlib_fn_indices[j];
         imports[i] = (wasmtime_extern_t) {.kind = WASMTIME_EXTERN_FUNC, .of.func = {store_id, address}};
         defined_in_stdlib = true;
         break;
       }
     }
 
     if (!defined_in_stdlib) {
@@ -1142,18 +1278,29 @@
   };
 
   if (language->field_count > 0 && language->production_id_count > 0) {
     language->field_map_slices = copy(
       &memory[wasm_language.field_map_slices],
       wasm_language.production_id_count * sizeof(TSFieldMapSlice)
     );
-    const TSFieldMapSlice last_field_map_slice = language->field_map_slices[language->production_id_count - 1];
+
+    // Determine the number of field map entries by finding the greatest index
+    // in any of the slices.
+    uint32_t field_map_entry_count = 0;
+    for (uint32_t i = 0; i < wasm_language.production_id_count; i++) {
+      TSFieldMapSlice slice = language->field_map_slices[i];
+      uint32_t slice_end = slice.index + slice.length;
+      if (slice_end > field_map_entry_count) {
+        field_map_entry_count = slice_end;
+      }
+    }
+
     language->field_map_entries = copy(
       &memory[wasm_language.field_map_entries],
-      (last_field_map_slice.index + last_field_map_slice.length) * sizeof(TSFieldMapEntry)
+      field_map_entry_count * sizeof(TSFieldMapEntry)
     );
     language->field_names = copy_strings(
       memory,
       wasm_language.field_names,
       wasm_language.field_count + 1,
       &field_name_buffer
     );
@@ -1322,25 +1469,45 @@
       .scanner_scan_fn_index = wasm_language.external_scanner.scan,
     }));
   }
 
   return true;
 }
 
+void ts_wasm_store_reset_heap(TSWasmStore *self) {
+  wasmtime_context_t *context = wasmtime_store_context(self->store);
+  wasmtime_func_t func = {
+    self->function_table.store_id,
+    self->builtin_fn_indices.reset_heap
+  };
+  wasm_trap_t *trap = NULL;
+  wasmtime_val_t args[1] = {
+    {.of.i32 = ts_wasm_store__heap_address(self), .kind = WASMTIME_I32},
+  };
+
+  wasmtime_error_t *error = wasmtime_func_call(context, &func, args, 1, NULL, 0, &trap);
+  assert(!error);
+  assert(!trap);
+}
+
 bool ts_wasm_store_start(TSWasmStore *self, TSLexer *lexer, const TSLanguage *language) {
   uint32_t instance_index;
   if (!ts_wasm_store_add_language(self, language, &instance_index)) return false;
   self->current_lexer = lexer;
   self->current_instance = &self->language_instances.contents[instance_index];
+  self->has_error = false;
+  ts_wasm_store_reset_heap(self);
   return true;
 }
 
-void ts_wasm_store_stop(TSWasmStore *self) {
+void ts_wasm_store_reset(TSWasmStore *self) {
   self->current_lexer = NULL;
   self->current_instance = NULL;
+  self->has_error = false;
+  ts_wasm_store_reset_heap(self);
 }
 
 static void ts_wasm_store__call(
   TSWasmStore *self,
   int32_t function_index,
   wasmtime_val_raw_t *args_and_results,
   size_t args_and_results_len
@@ -1350,47 +1517,57 @@
   bool succeeded = wasmtime_table_get(context, &self->function_table, function_index, &value);
   assert(succeeded);
   assert(value.kind == WASMTIME_FUNCREF);
   wasmtime_func_t func = value.of.funcref;
 
   wasm_trap_t *trap = NULL;
   wasmtime_error_t *error = wasmtime_func_call_unchecked(context, &func, args_and_results, args_and_results_len, &trap);
-  assert(!error);
-  if (trap) {
-    wasm_message_t message;
-    wasm_trap_message(trap, &message);
-    fprintf(
-      stderr,
-      "trap when calling wasm lexing function %u: %.*s\n",
-      function_index,
-      (int)message.size, message.data
-    );
-    abort();
+  if (error) {
+    // wasm_message_t message;
+    // wasmtime_error_message(error, &message);
+    // fprintf(
+    //   stderr,
+    //   "error in wasm module: %.*s\n",
+    //   (int)message.size, message.data
+    // );
+    wasmtime_error_delete(error);
+    self->has_error = true;
+  } else if (trap) {
+    // wasm_message_t message;
+    // wasm_trap_message(trap, &message);
+    // fprintf(
+    //   stderr,
+    //   "trap in wasm module: %.*s\n",
+    //   (int)message.size, message.data
+    // );
+    wasm_trap_delete(trap);
+    self->has_error = true;
   }
 }
 
 static bool ts_wasm_store__call_lex_function(TSWasmStore *self, unsigned function_index, TSStateId state) {
   wasmtime_context_t *context = wasmtime_store_context(self->store);
   uint8_t *memory_data = wasmtime_memory_data(context, &self->memory);
   memcpy(
-    &memory_data[LEXER_ADDRESS],
+    &memory_data[self->lexer_address],
     &self->current_lexer->lookahead,
     sizeof(self->current_lexer->lookahead)
   );
 
   wasmtime_val_raw_t args[2] = {
-    {.i32 = LEXER_ADDRESS},
+    {.i32 = self->lexer_address},
     {.i32 = state},
   };
   ts_wasm_store__call(self, function_index, args, 2);
+  if (self->has_error) return false;
   bool result = args[0].i32;
 
   memcpy(
     &self->current_lexer->lookahead,
-    &memory_data[LEXER_ADDRESS],
+    &memory_data[self->lexer_address],
     sizeof(self->current_lexer->lookahead) + sizeof(self->current_lexer->result_symbol)
   );
   return result;
 }
 
 bool ts_wasm_store_call_lex_main(TSWasmStore *self, TSStateId state) {
   return ts_wasm_store__call_lex_function(
@@ -1407,104 +1584,120 @@
     state
   );
 }
 
 uint32_t ts_wasm_store_call_scanner_create(TSWasmStore *self) {
   wasmtime_val_raw_t args[1] = {{.i32 = 0}};
   ts_wasm_store__call(self, self->current_instance->scanner_create_fn_index, args, 1);
+  if (self->has_error) return 0;
   return args[0].i32;
 }
 
 void ts_wasm_store_call_scanner_destroy(TSWasmStore *self, uint32_t scanner_address) {
-  wasmtime_val_raw_t args[1] = {{.i32 = scanner_address}};
-  ts_wasm_store__call(self, self->current_instance->scanner_destroy_fn_index, args, 1);
+  if (self->current_instance) {
+    wasmtime_val_raw_t args[1] = {{.i32 = scanner_address}};
+    ts_wasm_store__call(self, self->current_instance->scanner_destroy_fn_index, args, 1);
+  }
 }
 
 bool ts_wasm_store_call_scanner_scan(
   TSWasmStore *self,
   uint32_t scanner_address,
   uint32_t valid_tokens_ix
 ) {
   wasmtime_context_t *context = wasmtime_store_context(self->store);
   uint8_t *memory_data = wasmtime_memory_data(context, &self->memory);
 
   memcpy(
-    &memory_data[LEXER_ADDRESS],
+    &memory_data[self->lexer_address],
     &self->current_lexer->lookahead,
     sizeof(self->current_lexer->lookahead)
   );
 
   uint32_t valid_tokens_address =
     self->current_instance->external_states_address +
     (valid_tokens_ix * sizeof(bool));
   wasmtime_val_raw_t args[3] = {
     {.i32 = scanner_address},
-    {.i32 = LEXER_ADDRESS},
+    {.i32 = self->lexer_address},
     {.i32 = valid_tokens_address}
   };
   ts_wasm_store__call(self, self->current_instance->scanner_scan_fn_index, args, 3);
+  if (self->has_error) return false;
 
   memcpy(
     &self->current_lexer->lookahead,
-    &memory_data[LEXER_ADDRESS],
+    &memory_data[self->lexer_address],
     sizeof(self->current_lexer->lookahead) + sizeof(self->current_lexer->result_symbol)
   );
   return args[0].i32;
 }
 
 uint32_t ts_wasm_store_call_scanner_serialize(
   TSWasmStore *self,
   uint32_t scanner_address,
   char *buffer
 ) {
   wasmtime_context_t *context = wasmtime_store_context(self->store);
   uint8_t *memory_data = wasmtime_memory_data(context, &self->memory);
+  uint32_t serialization_buffer_address = ts_wasm_store__serialization_buffer_address(self);
 
   wasmtime_val_raw_t args[2] = {
     {.i32 = scanner_address},
-    {.i32 = SERIALIZATION_BUFFER_ADDRESS},
+    {.i32 = serialization_buffer_address},
   };
   ts_wasm_store__call(self, self->current_instance->scanner_serialize_fn_index, args, 2);
+  if (self->has_error) return 0;
+
   uint32_t length = args[0].i32;
+  if (length > TREE_SITTER_SERIALIZATION_BUFFER_SIZE) {
+      self->has_error = true;
+      return 0;
+  }
 
   if (length > 0) {
     memcpy(
       ((Lexer *)self->current_lexer)->debug_buffer,
-      &memory_data[SERIALIZATION_BUFFER_ADDRESS],
+      &memory_data[serialization_buffer_address],
       length
     );
   }
   return length;
 }
 
 void ts_wasm_store_call_scanner_deserialize(
   TSWasmStore *self,
   uint32_t scanner_address,
   const char *buffer,
   unsigned length
 ) {
   wasmtime_context_t *context = wasmtime_store_context(self->store);
   uint8_t *memory_data = wasmtime_memory_data(context, &self->memory);
+  uint32_t serialization_buffer_address = ts_wasm_store__serialization_buffer_address(self);
 
   if (length > 0) {
     memcpy(
-      &memory_data[SERIALIZATION_BUFFER_ADDRESS],
+      &memory_data[serialization_buffer_address],
       buffer,
       length
     );
   }
 
   wasmtime_val_raw_t args[3] = {
     {.i32 = scanner_address},
-    {.i32 = SERIALIZATION_BUFFER_ADDRESS},
+    {.i32 = serialization_buffer_address},
     {.i32 = length},
   };
   ts_wasm_store__call(self, self->current_instance->scanner_deserialize_fn_index, args, 3);
 }
 
+bool ts_wasm_store_has_error(const TSWasmStore *self) {
+  return self->has_error;
+}
+
 bool ts_language_is_wasm(const TSLanguage *self) {
   return self->lex_fn == ts_wasm_store__sentinel_lex_fn;
 }
 
 static inline LanguageWasmModule *ts_language__wasm_module(const TSLanguage *self) {
   return (LanguageWasmModule *)self->keyword_lex_fn;
 }
@@ -1565,15 +1758,15 @@
 ) {
   (void)self;
   (void)lexer;
   (void)language;
   return false;
 }
 
-void ts_wasm_store_stop(TSWasmStore *self) {
+void ts_wasm_store_reset(TSWasmStore *self) {
   (void)self;
 }
 
 bool ts_wasm_store_call_lex_main(TSWasmStore *self, TSStateId state) {
   (void)self;
   (void)state;
   return false;
@@ -1628,14 +1821,19 @@
 ) {
   (void)self;
   (void)scanner_address;
   (void)buffer;
   (void)length;
 }
 
+bool ts_wasm_store_has_error(const TSWasmStore *self) {
+  (void)self;
+  return false;
+}
+
 bool ts_language_is_wasm(const TSLanguage *self) {
   (void)self;
   return false;
 }
 
 void ts_wasm_language_retain(const TSLanguage *self) {
   (void)self;
```

### Comparing `tree-sitter-0.21.3/tree_sitter/core/lib/src/wasm_store.h` & `tree-sitter-0.22.0/tree_sitter/core/lib/src/wasm_store.h`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 extern "C" {
 #endif
 
 #include "tree_sitter/api.h"
 #include "./parser.h"
 
 bool ts_wasm_store_start(TSWasmStore *, TSLexer *, const TSLanguage *);
-void ts_wasm_store_stop(TSWasmStore *);
+void ts_wasm_store_reset(TSWasmStore *);
+bool ts_wasm_store_has_error(const TSWasmStore *);
 
 bool ts_wasm_store_call_lex_main(TSWasmStore *, TSStateId);
 bool ts_wasm_store_call_lex_keyword(TSWasmStore *, TSStateId);
 
 uint32_t ts_wasm_store_call_scanner_create(TSWasmStore *);
 void ts_wasm_store_call_scanner_destroy(TSWasmStore *, uint32_t);
 bool ts_wasm_store_call_scanner_scan(TSWasmStore *, uint32_t, uint32_t);
```

### Comparing `tree-sitter-0.21.3/tree_sitter.egg-info/PKG-INFO` & `tree-sitter-0.22.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,12 @@
-Metadata-Version: 2.1
-Name: tree-sitter
-Version: 0.21.3
-Summary: Python bindings for the Tree-Sitter parsing library
-Author-email: Max Brunsfeld <maxbrunsfeld@gmail.com>
-Project-URL: Homepage, https://tree-sitter.github.io/tree-sitter/
-Project-URL: Source, https://github.com/tree-sitter/py-tree-sitter
-Keywords: incremental,parsing,tree-sitter
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: C
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development :: Compilers
-Classifier: Topic :: Text Processing :: Linguistic
-Classifier: Typing :: Typed
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Python Tree-sitter
 
 [![CI][ci]](https://github.com/tree-sitter/py-tree-sitter/actions/workflows/ci.yml)
 [![pypi][pypi]](https://pypi.org/project/tree-sitter/)
+[![docs][docs]](https://tree-sitter.github.io/py-tree-sitter/)
 
 This module provides Python bindings to the [tree-sitter] parsing library.
 
 ## Installation
 
 The package has no library dependencies and provides pre-compiled wheels for all major platforms.
 
@@ -51,53 +32,15 @@
 
 Then, you can load it as a `Language` object:
 
 ```python
 import tree_sitter_python as tspython
 from tree_sitter import Language, Parser
 
-PY_LANGUAGE = Language(tspython.language(), "python")
-```
-
-#### Build from source
-
-> [!WARNING]
-> This method of loading languages is deprecated and will be removed in `v0.22.0`.
-> You should only use it if you need languages that have not updated their bindings.
-> Keep in mind that you will need a C compiler in this case.
-
-First you'll need a Tree-sitter language implementation for each language that you want to parse.
-
-```sh
-git clone https://github.com/tree-sitter/tree-sitter-go
-git clone https://github.com/tree-sitter/tree-sitter-javascript
-git clone https://github.com/tree-sitter/tree-sitter-python
-```
-
-Use the `Language.build_library` method to compile these into a library that's
-usable from Python. This function will return immediately if the library has
-already been compiled since the last time its source code was modified:
-
-```python
-from tree_sitter import Language, Parser
-
-Language.build_library(
-    # Store the library in the `build` directory
-    "build/my-languages.so",
-    # Include one or more languages
-    ["vendor/tree-sitter-go", "vendor/tree-sitter-javascript", "vendor/tree-sitter-python"],
-)
-```
-
-Load the languages into your app as `Language` objects:
-
-```python
-GO_LANGUAGE = Language("build/my-languages.so", "go")
-JS_LANGUAGE = Language("build/my-languages.so", "javascript")
-PY_LANGUAGE = Language("build/my-languages.so", "python")
+PY_LANGUAGE = Language(tspython.language())
 ```
 
 ### Basic parsing
 
 Create a `Parser` and configure it to use a language:
 
 ```python
@@ -111,27 +54,27 @@
 tree = parser.parse(
     bytes(
         """
 def foo():
     if bar:
         baz()
 """,
-        "utf8",
+        "utf8"
     )
 )
 ```
 
 If you have your source code in some data structure other than a bytes object,
 you can pass a "read" callable to the parse function.
 
 The read callable can use either the byte offset or point tuple to read from
 buffer and return source code as bytes object. An empty bytes object or None
-terminates parsing for that line. The bytes must encode the source as UTF-8.
+terminates parsing for that line. The bytes must be encoded as UTF-8 or UTF-16.
 
-For example, to use the byte offset:
+For example, to use the byte offset with UTF-8 encoding:
 
 ```python
 src = bytes(
     """
 def foo():
     if bar:
         baz()
@@ -140,15 +83,15 @@
 )
 
 
 def read_callable_byte_offset(byte_offset, point):
     return src[byte_offset : byte_offset + 1]
 
 
-tree = parser.parse(read_callable_byte_offset)
+tree = parser.parse(read_callable_byte_offset, encoding="utf8")
 ```
 
 And to use the point:
 
 ```python
 src_lines = ["\n", "def foo():\n", "    if bar:\n", "        baz()\n"]
 
@@ -156,15 +99,15 @@
 def read_callable_point(byte_offset, point):
     row, column = point
     if row >= len(src_lines) or column >= len(src_lines[row]):
         return None
     return src_lines[row][column:].encode("utf8")
 
 
-tree = parser.parse(read_callable_point)
+tree = parser.parse(read_callable_point, encoding="utf8")
 ```
 
 Inspect the resulting `Tree`:
 
 ```python
 root_node = tree.root_node
 assert root_node.type == 'module'
@@ -206,14 +149,35 @@
                     "consequence: (block "
                         "(expression_statement (call "
                             "function: (identifier) "
                             "arguments: (argument_list))))))))"
 )
 ```
 
+Or, to use the byte offset with UTF-16 encoding:
+
+```python
+parser.set_language(JAVASCRIPT)
+source_code = bytes("'😎' && '🐍'", "utf16")
+
+def read(byte_position, _):
+    return source_code[byte_position: byte_position + 2]
+
+tree = parser.parse(read, encoding="utf16")
+root_node = tree.root_node
+statement_node = root_node.children[0]
+binary_node = statement_node.children[0]
+snake_node = binary_node.children[2]
+snake = source_code[snake_node.start_byte:snake_node.end_byte]
+
+assert binary_node.type == "binary_expression"
+assert snake_node.type == "string"
+assert snake.decode("utf16") == "'🐍'"
+```
+
 ### Walking syntax trees
 
 If you need to traverse a large number of nodes efficiently, you can use
 a `TreeCursor`:
 
 ```python
 cursor = tree.walk()
@@ -340,9 +304,10 @@
 
 [tree-sitter]: https://tree-sitter.github.io/tree-sitter/
 [issue]: https://github.com/tree-sitter/py-tree-sitter/issues/new
 [tree-sitter-python]: https://github.com/tree-sitter/tree-sitter-python
 [tree query]: https://tree-sitter.github.io/tree-sitter/using-parsers#query-syntax
 [ci]: https://img.shields.io/github/actions/workflow/status/tree-sitter/py-tree-sitter/ci.yml?logo=github&label=CI
 [pypi]: https://img.shields.io/pypi/v/tree-sitter?logo=pypi&logoColor=ffd242&label=PyPI
+[docs]: https://img.shields.io/github/deployments/tree-sitter/py-tree-sitter/github-pages?logo=sphinx&label=Docs
 [examples/walk_tree.py]: https://github.com/tree-sitter/py-tree-sitter/blob/master/examples/walk_tree.py
 [examples/usage.py]: https://github.com/tree-sitter/py-tree-sitter/blob/master/examples/usage.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tree-sitter-0.21.3/tree_sitter.egg-info/SOURCES.txt` & `tree-sitter-0.22.0/tree_sitter.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 tree_sitter/__init__.py
-tree_sitter/_binding.pyi
-tree_sitter/binding.c
+tree_sitter/__init__.pyi
 tree_sitter/py.typed
 tree_sitter.egg-info/PKG-INFO
 tree_sitter.egg-info/SOURCES.txt
 tree_sitter.egg-info/dependency_links.txt
+tree_sitter.egg-info/requires.txt
 tree_sitter.egg-info/top_level.txt
+tree_sitter/binding/language.c
+tree_sitter/binding/lookahead_iterator.c
+tree_sitter/binding/lookahead_names_iterator.c
+tree_sitter/binding/module.c
+tree_sitter/binding/node.c
+tree_sitter/binding/parser.c
+tree_sitter/binding/query.c
+tree_sitter/binding/range.c
+tree_sitter/binding/tree.c
+tree_sitter/binding/tree_cursor.c
 tree_sitter/core/lib/include/tree_sitter/api.h
 tree_sitter/core/lib/src/alloc.c
 tree_sitter/core/lib/src/alloc.h
 tree_sitter/core/lib/src/array.h
 tree_sitter/core/lib/src/atomic.h
 tree_sitter/core/lib/src/clock.h
 tree_sitter/core/lib/src/error_costs.h
```

