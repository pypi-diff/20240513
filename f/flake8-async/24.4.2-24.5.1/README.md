# Comparing `tmp/flake8_async-24.4.2.tar.gz` & `tmp/flake8_async-24.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_async-24.4.2.tar", last modified: Wed Apr 24 18:40:17 2024, max compression
+gzip compressed data, was "flake8_async-24.5.1.tar", last modified: Mon May 13 08:36:34 2024, max compression
```

## Comparing `flake8_async-24.4.2.tar` & `flake8_async-24.5.1.tar`

### file list

```diff
@@ -1,120 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.211190 flake8_async-24.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-24 18:40:10.000000 flake8_async-24.4.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-24 18:40:10.000000 flake8_async-24.4.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-24 18:40:10.000000 flake8_async-24.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-24 18:40:10.000000 flake8_async-24.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-04-24 18:40:17.211190 flake8_async-24.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14390 2024-04-24 18:40:14.000000 flake8_async-24.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.191189 flake8_async-24.4.2/flake8_async/
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.195190 flake8_async-24.4.2/flake8_async/visitors/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/flake8asyncvisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor101.py
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor102.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor103_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor105.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor111.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor118.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor2xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    32798 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor91x.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitor_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12111 2024-04-24 18:40:10.000000 flake8_async-24.4.2/flake8_async/visitors/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.207190 flake8_async-24.4.2/flake8_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22912 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 18:40:17.000000 flake8_async-24.4.2/flake8_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-04-24 18:40:10.000000 flake8_async-24.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 18:40:17.211190 flake8_async-24.4.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-04-24 18:40:10.000000 flake8_async-24.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.199190 flake8_async-24.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.199190 flake8_async-24.4.2/tests/autofix_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    28720 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/autofix_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:40:17.207190 flake8_async-24.4.2/tests/eval_files/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/anyio_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async100_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async100_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async101.py
--rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102_aclose.py
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102_aclose_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async102_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async103.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async103_all_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async103_both_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async103_no_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async103_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async104.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async104_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async104_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async105.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async105_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async106.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async109.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async110.py
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async111.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async112.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async113.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async113_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async113_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async114.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async115.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async116.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async118.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async119.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async210.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async211.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async212.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async22x.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async22x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async232.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async232_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async23x.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async23x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async240.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async250.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async250_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async251.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async251_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async900.py
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    23988 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/async91x_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/no_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/noqa_no_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/eval_files/trio_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_all_visitors_imported.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_changelog_and_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_config_and_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_exception_on_invalid_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    29043 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_flake8_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_formatting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3407 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/test_messages_documented.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tests/trio_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-24 18:40:10.000000 flake8_async-24.4.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:36:34.093896 flake8_async-24.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-13 08:36:26.000000 flake8_async-24.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-13 08:36:26.000000 flake8_async-24.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-13 08:36:26.000000 flake8_async-24.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 08:36:26.000000 flake8_async-24.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-05-13 08:36:34.093896 flake8_async-24.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14548 2024-05-13 08:36:31.000000 flake8_async-24.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:36:34.077896 flake8_async-24.5.1/flake8_async/
+-rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:36:34.081896 flake8_async-24.5.1/flake8_async/visitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9138 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/flake8asyncvisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15025 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/visitor101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/visitor102.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/visitor103_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/visitor105.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/visitor111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/visitor118.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/visitor2xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36306 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/visitor91x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/visitor_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12683 2024-05-13 08:36:26.000000 flake8_async-24.5.1/flake8_async/visitors/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:36:34.093896 flake8_async-24.5.1/flake8_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23272 2024-05-13 08:36:34.000000 flake8_async-24.5.1/flake8_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-13 08:36:34.000000 flake8_async-24.5.1/flake8_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:36:34.000000 flake8_async-24.5.1/flake8_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 08:36:34.000000 flake8_async-24.5.1/flake8_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 08:36:33.000000 flake8_async-24.5.1/flake8_async.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 08:36:34.000000 flake8_async-24.5.1/flake8_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 08:36:34.000000 flake8_async-24.5.1/flake8_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-05-13 08:36:26.000000 flake8_async-24.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 08:36:34.093896 flake8_async-24.5.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-05-13 08:36:26.000000 flake8_async-24.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:36:34.085896 flake8_async-24.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:36:34.085896 flake8_async-24.5.1/tests/autofix_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2938 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/autofix_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/autofix_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/autofix_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12002 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/autofix_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28741 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/autofix_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/autofix_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/autofix_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/autofix_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 08:36:34.093896 flake8_async-24.5.1/tests/eval_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/anyio_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async100_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async102_aclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async102_aclose_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async102_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async102_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async102_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async103.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async103_all_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async103_both_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async103_no_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async103_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async104.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async104_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async104_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async105.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async105_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async106.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async109.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10415 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async111.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async111_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async111_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async112.py
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async112_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async112_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async113.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async113_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async113_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async114.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async115.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async116.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async118.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async119.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async210.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async211.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async212.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async22x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async22x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async232_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async23x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async23x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async250.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async250_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async251.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async251_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async900.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10872 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24009 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async912.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async912_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/async91x_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/no_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/noqa_no_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/eval_files/trio_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/test_all_visitors_imported.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/test_changelog_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12107 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/test_config_and_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/test_exception_on_invalid_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29840 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/test_flake8_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/test_formatting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3407 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/test_messages_documented.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tests/trio_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-13 08:36:26.000000 flake8_async-24.5.1/tox.ini
```

### Comparing `flake8_async-24.4.2/CHANGELOG.md` & `flake8_async-24.5.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 24.5.1
+- Add ASYNC912: no checkpoints in with statement are guaranteed to run.
+- ASYNC100 now properly treats async for comprehensions as checkpoints.
+- ASYNC100 now supports autofixing on asyncio.
+
 ## 24.4.2
 - Add ASYNC119: yield in contextmanager in async generator.
 
 ## 24.4.1
 - ASYNC91X fix internal error caused by multiple `try/except` incorrectly sharing state.
 
 ## 24.3.6
```

### Comparing `flake8_async-24.4.2/CONTRIBUTING.md` & `flake8_async-24.5.1/CONTRIBUTING.md`

 * *Files 14% similar despite different names*

```diff
@@ -40,19 +40,23 @@
 #### `TRIOxxx:`
 You can instead of `error` specify the error code.
 
 ### `# ARG`
 With `# ARG` lines you can also specify command-line arguments that should be passed to the plugin when parsing a file. Can be specified multiple times for several different arguments.  
 Generated tests will by default `--select` the error code of the file, which will enable any visitors that can generate that code (and if those visitors can raise other codes they might be raised too). This can be overridden by adding an `# ARG --select=...` line.
 
-### `# NOANYIO` and `# NOTRIO`
-Eval files are also evaluated where ~all instances of "trio" is replaced with "anyio" and `--anyio` is prepended to the argument list, to check for compatibility with the [anyio](https://github.com/agronholm/anyio) library - unless they are marked with `# NOANYIO`.
-If a file is marked with `# NOTRIO` it will not replace instances of "trio" with "anyio", and the file will not be run by the normal `eval_files` test generator.
-#### `# ANYIO_NO_ERROR`
-A file which is marked with this will ignore all `# error` or `# TRIO...` comments when running with anyio. Use when an error is trio-specific and replacing "trio" with "anyio" should silence all errors.
+### Library parametrization
+Eval files are evaluated with each supported library. It does this by replacing all instances of the `BASE_LIBRARY` ("trio" by default) with the two other libraries, and setting the corresponding flag (`--anyio` or `--asyncio`).
+### `# BASE_LIBRARY anyio` / `# BASE_LIBRARY asyncio`
+Defaults to `trio`. Used to specify the primary library an eval file is testing.
+
+#### `# ANYIO_NO_ERROR`, `# TRIO_NO_ERROR`, `# ASYNCIO_NO_ERROR`
+A file which is marked with this will ignore all `# error` or `# TRIO...` comments when running with anyio. Use when an error is library-specific and replacing all instances means the file should no longer raise any errors.
+### `# NOANYIO`, `# NOTRIO`, `#NOASYNCIO`
+Disables checking a file with the specified library. Should be used somewhat sparingly, and always have a comment motivating its use.
 
 ## Running pytest outside tox
 If you don't want to bother with tox to quickly test stuff, you'll need to install the following dependencies:
 ```
 pip install -e .
 pip install pytest pytest-cov hypothesis hypothesmith flake8
 ```
```

### Comparing `flake8_async-24.4.2/LICENSE` & `flake8_async-24.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/PKG-INFO` & `flake8_async-24.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.4.2
+Version: 24.5.1
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Home-page: https://github.com/python-trio/flake8-async
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flake8
@@ -85,14 +85,15 @@
 - **ASYNC251**: `time.sleep(...)` should not be called from async function. Use `[trio/anyio/asyncio].sleep(...)`.
 
 ### Warnings disabled by default
 - **ASYNC900**: Async generator without `@asynccontextmanager` not allowed. You might want to enable this on a codebase since async generators are inherently unsafe and cleanup logic might not be performed. See https://github.com/python-trio/flake8-async/issues/211 and https://discuss.python.org/t/using-exceptiongroup-at-anthropic-experience-report/20888/6 for discussion.
 - **ASYNC910**: Exit or `return` from async function with no guaranteed checkpoint or exception since function definition. You might want to enable this on a codebase to make it easier to reason about checkpoints, and make the logic of ASYNC911 correct.
 - **ASYNC911**: Exit, `yield` or `return` from async iterable with no guaranteed checkpoint since possible function entry (yield or function definition)
   Checkpoints are `await`, `async for`, and `async with` (on one of enter/exit).
+- **ASYNC912**: Timeout/Cancelscope has no awaits that are guaranteed to run. If the scope has no checkpoints at all, then `ASYNC100` will be raised instead.
 
 ### Removed Warnings
 - **TRIOxxx**: All error codes are now renamed ASYNCxxx
 - **TRIO107**: Renamed to TRIO910
 - **TRIO108**: Renamed to TRIO911
 - **TRIO117**: Don't raise or catch `trio.[NonBase]MultiError`, prefer `[exceptiongroup.]BaseExceptionGroup`. `MultiError` was removed in trio==0.24.0.
 
@@ -106,15 +107,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.4.2
+  rev: 24.5.1
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
@@ -221,14 +222,19 @@
     arbitrary_other_function(my_blocking_call=None)
 ```
 
 
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 24.5.1
+- Add ASYNC912: no checkpoints in with statement are guaranteed to run.
+- ASYNC100 now properly treats async for comprehensions as checkpoints.
+- ASYNC100 now supports autofixing on asyncio.
+
 ## 24.4.2
 - Add ASYNC119: yield in contextmanager in async generator.
 
 ## 24.4.1
 - ASYNC91X fix internal error caused by multiple `try/except` incorrectly sharing state.
 
 ## 24.3.6
```

### Comparing `flake8_async-24.4.2/README.md` & `flake8_async-24.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 - **ASYNC251**: `time.sleep(...)` should not be called from async function. Use `[trio/anyio/asyncio].sleep(...)`.
 
 ### Warnings disabled by default
 - **ASYNC900**: Async generator without `@asynccontextmanager` not allowed. You might want to enable this on a codebase since async generators are inherently unsafe and cleanup logic might not be performed. See https://github.com/python-trio/flake8-async/issues/211 and https://discuss.python.org/t/using-exceptiongroup-at-anthropic-experience-report/20888/6 for discussion.
 - **ASYNC910**: Exit or `return` from async function with no guaranteed checkpoint or exception since function definition. You might want to enable this on a codebase to make it easier to reason about checkpoints, and make the logic of ASYNC911 correct.
 - **ASYNC911**: Exit, `yield` or `return` from async iterable with no guaranteed checkpoint since possible function entry (yield or function definition)
   Checkpoints are `await`, `async for`, and `async with` (on one of enter/exit).
+- **ASYNC912**: Timeout/Cancelscope has no awaits that are guaranteed to run. If the scope has no checkpoints at all, then `ASYNC100` will be raised instead.
 
 ### Removed Warnings
 - **TRIOxxx**: All error codes are now renamed ASYNCxxx
 - **TRIO107**: Renamed to TRIO910
 - **TRIO108**: Renamed to TRIO911
 - **TRIO117**: Don't raise or catch `trio.[NonBase]MultiError`, prefer `[exceptiongroup.]BaseExceptionGroup`. `MultiError` was removed in trio==0.24.0.
 
@@ -81,15 +82,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.4.2
+  rev: 24.5.1
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
```

### Comparing `flake8_async-24.4.2/flake8_async/__init__.py` & `flake8_async-24.5.1/flake8_async/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     from flake8.options.manager import OptionManager
 
     from .base import Error
 
 
 # CalVer: YY.month.patch, e.g. first release of July 2022 == "22.7.1"
-__version__ = "24.4.2"
+__version__ = "24.5.1"
 
 
 # taken from https://github.com/Zac-HD/shed
 @functools.lru_cache
 def _get_git_repo_root(cwd: str | None = None) -> str:
     return subprocess.run(
         ["git", "rev-parse", "--show-toplevel"],
```

### Comparing `flake8_async-24.4.2/flake8_async/base.py` & `flake8_async-24.5.1/flake8_async/base.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/flake8_async/runner.py` & `flake8_async-24.5.1/flake8_async/runner.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/flake8_async/visitors/__init__.py` & `flake8_async-24.5.1/flake8_async/visitors/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 utility_visitors_cst: set[type[Flake8AsyncVisitor_cst]] = set()
 
 # Import all files with visitors so their decorators run, filling the above containers
 # This has to be done at the end to avoid circular imports
 from . import (
     visitor2xx,
     visitor91x,
-    visitor100,
     visitor101,
     visitor102,
     visitor103_104,
     visitor105,
     visitor111,
     visitor118,
     visitor_utility,
```

### Comparing `flake8_async-24.4.2/flake8_async/visitors/flake8asyncvisitor.py` & `flake8_async-24.5.1/flake8_async/visitors/flake8asyncvisitor.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,19 @@
     ):
         if error_code is None:
             assert (
                 len(self.error_codes) == 1
             ), "No error code defined, but class has multiple codes"
             error_code = next(iter(self.error_codes))
         # don't emit an error if this code is disabled in a multi-code visitor
-        elif strip_error_subidentifier(error_code) not in self.options.enabled_codes:
+        elif (
+            (ec_no_sub := strip_error_subidentifier(error_code))
+            not in self.options.enabled_codes
+            and ec_no_sub not in self.options.autofix_codes
+        ):
             return
 
         self.__state.problems.append(
             Error(
                 strip_error_subidentifier(error_code),
                 node.lineno,
                 node.col_offset,
@@ -213,15 +217,19 @@
         if error_code is None:
             assert (
                 len(self.error_codes) == 1
             ), "No error code defined, but class has multiple codes"
             error_code = next(iter(self.error_codes))
         # don't emit an error if this code is disabled in a multi-code visitor
         # TODO: write test for only one of 910/911 enabled/autofixed
-        elif strip_error_subidentifier(error_code) not in self.options.enabled_codes:
+        elif (
+            (ec_no_sub := strip_error_subidentifier(error_code))
+            not in self.options.enabled_codes
+            and ec_no_sub not in self.options.autofix_codes
+        ):
             return False  # pragma: no cover
 
         if self.is_noqa(node, error_code):
             return False
 
         # pyright + get_metadata is acting up
         pos = self.get_metadata(PositionProvider, node).start  # type: ignore
@@ -233,15 +241,15 @@
                 self.error_codes[error_code],
                 *args,
             )
         )
         return True
 
     def should_autofix(self, node: cst.CSTNode, code: str | None = None) -> bool:
-        if code is None:
+        if code is None:  # pragma: no cover
             assert len(self.error_codes) == 1
             code = next(iter(self.error_codes))
         # this does not currently need to check for `noqa`s, as error() does that
         # and no codes tries to autofix if there's no error. This might change if/when
         # "printing an error" and "autofixing" becomes independent. See issue #192
         return code in self.options.autofix_codes
```

### Comparing `flake8_async-24.4.2/flake8_async/visitors/helpers.py` & `flake8_async-24.5.1/flake8_async/visitors/helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -47,21 +47,27 @@
 def error_class_cst(error_class: type[T_CST]) -> type[T_CST]:
     assert error_class.error_codes
     ERROR_CLASSES_CST.add(error_class)
     return error_class
 
 
 def disabled_by_default(error_class: type[T_EITHER]) -> type[T_EITHER]:
+    """Default-disables all error codes in a class."""
     assert error_class.error_codes  # type: ignore[attr-defined]
     default_disabled_error_codes.extend(
         error_class.error_codes  # type: ignore[attr-defined]
     )
     return error_class
 
 
+def disable_codes_by_default(*codes: str) -> None:
+    """Default-disables only specified codes."""
+    default_disabled_error_codes.extend(codes)
+
+
 def utility_visitor(c: type[T]) -> type[T]:
     assert not hasattr(c, "error_codes")
     c.error_codes = {}
     utility_visitors.add(c)
     return c
 
 
@@ -313,38 +319,76 @@
 
 class AttributeCall(NamedTuple):
     node: cst.Call
     base: str
     function: str
 
 
+# the custom __or__ in libcst breaks pyright type checking. It's possible to use
+# `Union` as a workaround ... except pyupgrade will automatically replace that.
+# So we have to resort to specifying one of the base classes.
+# See https://github.com/Instagram/LibCST/issues/1143
+def build_cst_matcher(attr: str) -> m.BaseExpression:
+    """Build a cst matcher structure with attributes&names matching a string `a.b.c`."""
+    if "." not in attr:
+        return m.Name(value=attr)
+    body, tail = attr.rsplit(".")
+    return m.Attribute(value=build_cst_matcher(body), attr=m.Name(value=tail))
+
+
+def identifier_to_string(attr: cst.Name | cst.Attribute) -> str:
+    if isinstance(attr, cst.Name):
+        return attr.value
+    assert isinstance(attr.value, (cst.Attribute, cst.Name))
+    return identifier_to_string(attr.value) + "." + attr.attr.value
+
+
 def with_has_call(
     node: cst.With, *names: str, base: Iterable[str] = ("trio", "anyio")
 ) -> list[AttributeCall]:
+    """Check if a with statement has a matching call, returning a list with matches.
+
+    `names` specify the names of functions to match, `base` specifies the
+    library/module(s) the function must be in.
+    The list elements in the return value are named tuples with the matched node,
+    base and function.
+
+    Examples_
+
+    `with_has_call(node, "bar", base="foo")` matches foo.bar.
+    `with_has_call(node, "bar", "bee", base=("foo", "a.b.c")` matches
+      `foo.bar`, `foo.bee`, `a.b.c.bar`, and `a.b.c.bee`.
+
+    """
+    if isinstance(base, str):
+        base = (base,)  # pragma: no cover
+
+    # build matcher, using SaveMatchedNode to save the base and the function name.
+    matcher = m.Call(
+        func=m.Attribute(
+            value=m.SaveMatchedNode(
+                m.OneOf(*(build_cst_matcher(b) for b in base)), name="base"
+            ),
+            attr=m.SaveMatchedNode(
+                oneof_names(*names),
+                name="function",
+            ),
+        )
+    )
+
     res_list: list[AttributeCall] = []
     for item in node.items:
-        if res := m.extract(
-            item.item,
-            m.Call(
-                func=m.Attribute(
-                    value=m.SaveMatchedNode(m.Name(), name="library"),
-                    attr=m.SaveMatchedNode(
-                        oneof_names(*names),
-                        name="function",
-                    ),
-                )
-            ),
-        ):
+        if res := m.extract(item.item, matcher):
             assert isinstance(item.item, cst.Call)
-            assert isinstance(res["library"], cst.Name)
+            assert isinstance(res["base"], (cst.Name, cst.Attribute))
             assert isinstance(res["function"], cst.Name)
-            if res["library"].value not in base:
-                continue
             res_list.append(
-                AttributeCall(item.item, res["library"].value, res["function"].value)
+                AttributeCall(
+                    item.item, identifier_to_string(res["base"]), res["function"].value
+                )
             )
     return res_list
 
 
 def func_has_decorator(func: cst.FunctionDef, *names: str) -> bool:
     return any(
         list_contains(
```

### Comparing `flake8_async-24.4.2/flake8_async/visitors/visitor101.py` & `flake8_async-24.5.1/flake8_async/visitors/visitor101.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/flake8_async/visitors/visitor102.py` & `flake8_async-24.5.1/flake8_async/visitors/visitor102.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/flake8_async/visitors/visitor103_104.py` & `flake8_async-24.5.1/flake8_async/visitors/visitor103_104.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/flake8_async/visitors/visitor105.py` & `flake8_async-24.5.1/flake8_async/visitors/visitor105.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/flake8_async/visitors/visitor111.py` & `flake8_async-24.5.1/flake8_async/visitors/visitor111.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,21 +8,29 @@
 from .flake8asyncvisitor import Flake8AsyncVisitor
 from .helpers import error_class, get_matching_call
 
 if TYPE_CHECKING:
     from collections.abc import Mapping
 
 
+def is_nursery_like(node: ast.expr) -> bool:
+    return bool(
+        get_matching_call(node, "open_nursery", base="trio")
+        or get_matching_call(node, "create_task_group", base="anyio")
+        or get_matching_call(node, "TaskGroup", base="asyncio")
+    )
+
+
 @error_class
 class Visitor111(Flake8AsyncVisitor):
     error_codes: Mapping[str, str] = {
         "ASYNC111": (
             "variable {2} is usable within the context manager on line {0}, but that "
-            "will close before nursery opened on line {1} - this is usually a bug.  "
-            "Nurseries should generally be the inner-most context manager."
+            "will close before nursery/taskgroup opened on line {1} - this is usually "
+            "a bug. Nursery/TaskGroup should generally be the inner-most context manager."
         ),
     }
 
     class NurseryCall(NamedTuple):
         stack_index: int
         name: str
 
@@ -44,16 +52,15 @@
             # push its line, variable, and whether it's a trio nursery
             # to the _context_managers stack,
             if isinstance(item.optional_vars, ast.Name):
                 self._context_managers.append(
                     self.TrioContextManager(
                         item.context_expr.lineno,
                         item.optional_vars.id,
-                        get_matching_call(item.context_expr, "open_nursery")
-                        is not None,
+                        is_nursery_like(item.context_expr),
                     )
                 )
 
     visit_AsyncWith = visit_With
 
     def visit_FunctionDef(
         self, node: ast.FunctionDef | ast.AsyncFunctionDef | ast.Lambda
@@ -71,15 +78,15 @@
     # stack being passed as parameters to it. (and save <X> for the error message)
     def visit_Call(self, node: ast.Call):
         self.save_state(node, "_nursery_call")
 
         if (
             isinstance(node.func, ast.Attribute)
             and isinstance(node.func.value, ast.Name)
-            and node.func.attr in ("start", "start_soon")
+            and node.func.attr in ("start", "start_soon", "create_task")
         ):
             self._nursery_call = None
             for i, cm in enumerate(self._context_managers):
                 if node.func.value.id == cm.name:
                     # don't break upon finding a nursery in case there's multiple cm's
                     # on the stack with the same name
                     if cm.is_nursery:
```

### Comparing `flake8_async-24.4.2/flake8_async/visitors/visitor118.py` & `flake8_async-24.5.1/flake8_async/visitors/visitor118.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/flake8_async/visitors/visitor2xx.py` & `flake8_async-24.5.1/flake8_async/visitors/visitor2xx.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/flake8_async/visitors/visitor91x.py` & `flake8_async-24.5.1/flake8_async/visitors/visitor91x.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,27 +14,40 @@
 import libcst as cst
 import libcst.matchers as m
 from libcst.metadata import PositionProvider
 
 from ..base import Statement
 from .flake8asyncvisitor import Flake8AsyncVisitor_cst
 from .helpers import (
-    disabled_by_default,
+    AttributeCall,
+    cancel_scope_names,
+    disable_codes_by_default,
     error_class_cst,
+    flatten_preserving_comments,
     fnmatch_qualified_name_cst,
     func_has_decorator,
     iter_guaranteed_once_cst,
+    with_has_call,
 )
 
 if TYPE_CHECKING:
     from collections.abc import Mapping, Sequence
 
 
+class ArtificialStatement(Statement):
+    """Statement that should not trigger 910/911 on function exit.
+
+    Used by loops and `with` statements.
+    """
+
+
 # Statement injected at the start of loops to track missed checkpoints.
-ARTIFICIAL_STATEMENT = Statement("artificial", -1)
+ARTIFICIAL_STATEMENT = ArtificialStatement("artificial", -1)
+# There's no particular reason why loops use a globally instanced statement, but
+# `with` does not - mostly just an artifact of them being implemented at different times.
 
 
 def func_empty_body(node: cst.FunctionDef) -> bool:
     """Check if function body consist of `pass`, `...`, and/or (doc)string literals."""
     empty_statement = m.Pass() | m.Expr(m.Ellipsis() | m.SimpleString())
 
     return m.matches(
@@ -227,48 +240,67 @@
             self.add_statement = checkpoint_statement(self.library[0])
         return updated_node
 
     # returns handled same as yield, but ofc needs to ignore types
     leave_Return = leave_Yield  # type: ignore
 
 
+disable_codes_by_default("ASYNC910", "ASYNC911", "ASYNC912")
+
+
 @error_class_cst
-@disabled_by_default
 class Visitor91X(Flake8AsyncVisitor_cst, CommonVisitors):
     error_codes: Mapping[str, str] = {
         "ASYNC910": (
             "{0} from async function with no guaranteed checkpoint or exception "
             "since function definition on line {1.lineno}."
         ),
         "ASYNC911": (
             "{0} from async iterable with no guaranteed checkpoint since {1.name} "
             "on line {1.lineno}."
         ),
+        "ASYNC912": (
+            "CancelScope with no guaranteed checkpoint. This makes it potentially "
+            "impossible to cancel."
+        ),
+        "ASYNC100": (
+            "{0}.{1} context contains no checkpoints, remove the context or add"
+            " `await {0}.lowlevel.checkpoint()`."
+        ),
     }
 
     def __init__(self, *args: Any, **kwargs: Any):
         super().__init__(*args, **kwargs)
         self.has_yield = False
         self.safe_decorator = False
         self.async_function = False
         self.uncheckpointed_statements: set[Statement] = set()
         self.comp_unknown = False
 
         self.loop_state = LoopState()
         self.try_state = TryState()
 
+        # ASYNC100
+        self.has_checkpoint_stack: list[bool] = []
+        self.node_dict: dict[cst.With, list[AttributeCall]] = {}
+
     def should_autofix(self, node: cst.CSTNode, code: str | None = None) -> bool:
+        if code is None:  # pragma: no branch
+            code = "ASYNC911" if self.has_yield else "ASYNC910"
+
         return (
             not self.noautofix
-            and super().should_autofix(
-                node, "ASYNC911" if self.has_yield else "ASYNC910"
-            )
+            and super().should_autofix(node, code)
             and self.library != ("asyncio",)
         )
 
+    def checkpoint(self) -> None:
+        self.uncheckpointed_statements = set()
+        self.has_checkpoint_stack = [True] * len(self.has_checkpoint_stack)
+
     def checkpoint_statement(self) -> cst.SimpleStatementLine:
         return checkpoint_statement(self.library[0])
 
     def visit_FunctionDef(self, node: cst.FunctionDef) -> bool:
         # don't lint functions whose bodies solely consist of pass or ellipsis
         # @overload functions are also guaranteed to be empty
         # we also ignore pytest fixtures
@@ -279,17 +311,19 @@
             node,
             "has_yield",
             "safe_decorator",
             "async_function",
             "uncheckpointed_statements",
             "loop_state",
             "try_state",
+            "has_checkpoint_stack",
             copy=True,
         )
         self.uncheckpointed_statements = set()
+        self.has_checkpoint_stack = []
         self.has_yield = self.safe_decorator = False
         self.loop_state = LoopState()
 
         self.async_function = (
             node.asynchronous is not None
             and not fnmatch_qualified_name_cst(
                 node.decorators, *self.options.no_checkpoint_warning_decorators
@@ -355,15 +389,15 @@
             ):
                 self.loop_state.nodes_needing_checkpoints.append(original_node)
                 return False
 
         any_errors = False
         # raise the actual errors
         for statement in self.uncheckpointed_statements:
-            if statement == ARTIFICIAL_STATEMENT:
+            if isinstance(statement, ArtificialStatement):
                 continue
             any_errors |= self.error_91x(original_node, statement)
 
         return any_errors
 
     def leave_Return(
         self, original_node: cst.Return, updated_node: cst.Return
@@ -372,25 +406,26 @@
             return updated_node
         if self.check_function_exit(original_node) and self.should_autofix(
             original_node
         ):
             self.add_statement = self.checkpoint_statement()
         # avoid duplicate error messages
         self.uncheckpointed_statements = set()
+        # we don't treat it as a checkpoint for ASYNC100
 
         # return original node to avoid problems with identity equality
         assert original_node.deep_equals(updated_node)
         return original_node
 
     def error_91x(
         self,
         node: cst.Return | cst.FunctionDef | cst.Yield,
         statement: Statement,
     ) -> bool:
-        assert statement != ARTIFICIAL_STATEMENT
+        assert not isinstance(statement, ArtificialStatement)
 
         if isinstance(node, cst.FunctionDef):
             msg = "exit"
         else:
             msg = node.__class__.__name__.lower()
 
         return self.error(
@@ -403,38 +438,87 @@
     def leave_Await(
         self, original_node: cst.Await, updated_node: cst.Await
     ) -> cst.Await:
         # the expression being awaited is not checkpointed
         # so only set checkpoint after the await node
 
         # all nodes are now checkpointed
-        self.uncheckpointed_statements = set()
+        self.checkpoint()
         return updated_node
 
     # raising exception means we don't need to checkpoint so we can treat it as one
     # can't use TypeVar due to libcst's built-in type checking not supporting it
     leave_Raise = leave_Await  # type: ignore
 
     # Async context managers can reasonably checkpoint on either or both of entry and
     # exit.  Given that we can't tell which, we assume "both" to avoid raising a
     # missing-checkpoint warning when there might in fact be one (i.e. a false alarm).
     def visit_With_body(self, node: cst.With):
         if getattr(node, "asynchronous", None):
-            self.uncheckpointed_statements = set()
+            self.checkpoint()
+        if res := (
+            with_has_call(node, *cancel_scope_names)
+            or with_has_call(
+                node, "timeout", "timeout_at", base=("asyncio", "asyncio.timeouts")
+            )
+        ):
+            pos = self.get_metadata(PositionProvider, node).start  # pyright: ignore
+            line: int = pos.line  # pyright: ignore
+            column: int = pos.column  # pyright: ignore
+            self.uncheckpointed_statements.add(
+                ArtificialStatement("with", line, column)
+            )
+            self.node_dict[node] = res
+            self.has_checkpoint_stack.append(False)
+        else:
+            self.has_checkpoint_stack.append(True)
 
-    leave_With_body = visit_With_body
+    def leave_With(self, original_node: cst.With, updated_node: cst.With):
+        # Uses leave_With instead of leave_With_body because we need access to both
+        # original and updated node
+        # ASYNC100
+        if not self.has_checkpoint_stack.pop():
+            autofix = len(updated_node.items) == 1
+            for res in self.node_dict[original_node]:
+                # bypass 910 & 911's should_autofix logic, which excludes asyncio
+                # (TODO: and uses self.noautofix ... which I don't remember what it's for)
+                autofix &= self.error(
+                    res.node, res.base, res.function, error_code="ASYNC100"
+                ) and super().should_autofix(res.node, code="ASYNC100")
+
+            if autofix:
+                return flatten_preserving_comments(updated_node)
+        # ASYNC912
+        else:
+            pos = self.get_metadata(  # pyright: ignore
+                PositionProvider, original_node
+            ).start  # pyright: ignore
+            line: int = pos.line  # pyright: ignore
+            column: int = pos.column  # pyright: ignore
+            s = ArtificialStatement("with", line, column)
+            if s in self.uncheckpointed_statements:
+                self.uncheckpointed_statements.remove(s)
+                for res in self.node_dict[original_node]:
+                    self.error(res.node, error_code="ASYNC912")
+        if getattr(original_node, "asynchronous", None):
+            self.checkpoint()
+        return updated_node
 
     # error if no checkpoint since earlier yield or function entry
     def leave_Yield(
         self, original_node: cst.Yield, updated_node: cst.Yield
     ) -> cst.Yield:
         if not self.async_function:
             return updated_node
         self.has_yield = True
 
+        # Treat as a checkpoint for ASYNC100, since the context we yield to
+        # may checkpoint.
+        self.has_checkpoint_stack = [True] * len(self.has_checkpoint_stack)
+
         if self.check_function_exit(original_node) and self.should_autofix(
             original_node
         ):
             self.add_statement = self.checkpoint_statement()
 
         # mark as requiring checkpoint after
         pos = self.get_metadata(PositionProvider, original_node).start  # type: ignore
@@ -601,15 +685,15 @@
         )
 
         # inject an artificial uncheckpointed statement that won't raise an error,
         # but will be marked if an error would be generated. We can then generate
         # appropriate errors if the loop doesn't checkpoint
 
         if getattr(node, "asynchronous", None):
-            self.uncheckpointed_statements = set()
+            self.checkpoint()
         else:
             self.uncheckpointed_statements = {ARTIFICIAL_STATEMENT}
 
         self.loop_state.uncheckpointed_before_continue = set()
         self.loop_state.uncheckpointed_before_break = set()
 
     visit_For_body = visit_While_body
@@ -647,15 +731,15 @@
             if ARTIFICIAL_STATEMENT in stmts:
                 stmts.remove(ARTIFICIAL_STATEMENT)
                 stmts.update(self.outer[node]["uncheckpointed_statements"])
 
         # AsyncFor guarantees checkpoint on running out of iterable
         # so reset checkpoint state at end of loop. (but not state at break)
         if getattr(node, "asynchronous", None):
-            self.uncheckpointed_statements = set()
+            self.checkpoint()
         else:
             # enter orelse with worst case:
             # loop body might execute fully before entering orelse
             # (current state of self.uncheckpointed_statements)
             # or not at all
             if not self.loop_state.body_guaranteed_once:
                 self.uncheckpointed_statements.update(
@@ -776,15 +860,15 @@
         assert self.async_function
 
         if not self.uncheckpointed_statements:
             return False
 
         # if async comprehension, checkpoint
         if node.asynchronous:
-            self.uncheckpointed_statements = set()
+            self.checkpoint()
             self.comp_unknown = False
             return False
 
         # visit the iter call, which might have await's
         node.iter.visit(self)
 
         # stop checking if the loop is not guaranteed to execute
```

### Comparing `flake8_async-24.4.2/flake8_async/visitors/visitor_utility.py` & `flake8_async-24.5.1/flake8_async/visitors/visitor_utility.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/flake8_async/visitors/visitors.py` & `flake8_async-24.5.1/flake8_async/visitors/visitors.py`

 * *Files 9% similar despite different names*

```diff
@@ -100,25 +100,37 @@
             return
         for item in node.items:
             # get variable name <X>
             if not isinstance(item.optional_vars, ast.Name):
                 continue
             var_name = item.optional_vars.id
 
-            # check for trio.open_nursery
+            # check for trio.open_nursery and anyio.create_task_group
             nursery = get_matching_call(
-                item.context_expr, "open_nursery", base=("trio",)
-            )
+                item.context_expr, "open_nursery", base="trio"
+            ) or get_matching_call(item.context_expr, "create_task_group", base="anyio")
+            start_methods: tuple[str, ...] = ("start", "start_soon")
+            if nursery is None:
+                # check for asyncio.TaskGroup
+                nursery = get_matching_call(
+                    item.context_expr, "TaskGroup", base="asyncio"
+                )
+                if nursery is None:
+                    continue
+                start_methods = ("create_task",)
+
+            body_call = node.body[0].value
+            if isinstance(body_call, ast.Await):
+                body_call = body_call.value
 
             # `isinstance(..., ast.Call)` is done in get_matching_call
-            body_call = cast("ast.Call", node.body[0].value)
+            body_call = cast("ast.Call", body_call)
 
             if (
-                nursery is not None
-                and get_matching_call(body_call, "start", "start_soon", base=var_name)
+                get_matching_call(body_call, *start_methods, base=var_name)
                 # check for presence of <X> as parameter
                 and not any(
                     (isinstance(n, ast.Name) and n.id == var_name)
                     for n in self.walk(*body_call.args, *body_call.keywords)
                 )
             ):
                 self.error(item.context_expr, var_name)
```

### Comparing `flake8_async-24.4.2/flake8_async.egg-info/PKG-INFO` & `flake8_async-24.5.1/flake8_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.4.2
+Version: 24.5.1
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Home-page: https://github.com/python-trio/flake8-async
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flake8
@@ -85,14 +85,15 @@
 - **ASYNC251**: `time.sleep(...)` should not be called from async function. Use `[trio/anyio/asyncio].sleep(...)`.
 
 ### Warnings disabled by default
 - **ASYNC900**: Async generator without `@asynccontextmanager` not allowed. You might want to enable this on a codebase since async generators are inherently unsafe and cleanup logic might not be performed. See https://github.com/python-trio/flake8-async/issues/211 and https://discuss.python.org/t/using-exceptiongroup-at-anthropic-experience-report/20888/6 for discussion.
 - **ASYNC910**: Exit or `return` from async function with no guaranteed checkpoint or exception since function definition. You might want to enable this on a codebase to make it easier to reason about checkpoints, and make the logic of ASYNC911 correct.
 - **ASYNC911**: Exit, `yield` or `return` from async iterable with no guaranteed checkpoint since possible function entry (yield or function definition)
   Checkpoints are `await`, `async for`, and `async with` (on one of enter/exit).
+- **ASYNC912**: Timeout/Cancelscope has no awaits that are guaranteed to run. If the scope has no checkpoints at all, then `ASYNC100` will be raised instead.
 
 ### Removed Warnings
 - **TRIOxxx**: All error codes are now renamed ASYNCxxx
 - **TRIO107**: Renamed to TRIO910
 - **TRIO108**: Renamed to TRIO911
 - **TRIO117**: Don't raise or catch `trio.[NonBase]MultiError`, prefer `[exceptiongroup.]BaseExceptionGroup`. `MultiError` was removed in trio==0.24.0.
 
@@ -106,15 +107,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.4.2
+  rev: 24.5.1
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
@@ -221,14 +222,19 @@
     arbitrary_other_function(my_blocking_call=None)
 ```
 
 
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 24.5.1
+- Add ASYNC912: no checkpoints in with statement are guaranteed to run.
+- ASYNC100 now properly treats async for comprehensions as checkpoints.
+- ASYNC100 now supports autofixing on asyncio.
+
 ## 24.4.2
 - Add ASYNC119: yield in contextmanager in async generator.
 
 ## 24.4.1
 - ASYNC91X fix internal error caused by multiple `try/except` incorrectly sharing state.
 
 ## 24.3.6
```

### Comparing `flake8_async-24.4.2/flake8_async.egg-info/SOURCES.txt` & `flake8_async-24.5.1/flake8_async.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 flake8_async.egg-info/entry_points.txt
 flake8_async.egg-info/not-zip-safe
 flake8_async.egg-info/requires.txt
 flake8_async.egg-info/top_level.txt
 flake8_async/visitors/__init__.py
 flake8_async/visitors/flake8asyncvisitor.py
 flake8_async/visitors/helpers.py
-flake8_async/visitors/visitor100.py
 flake8_async/visitors/visitor101.py
 flake8_async/visitors/visitor102.py
 flake8_async/visitors/visitor103_104.py
 flake8_async/visitors/visitor105.py
 flake8_async/visitors/visitor111.py
 flake8_async/visitors/visitor118.py
 flake8_async/visitors/visitor2xx.py
@@ -39,14 +38,15 @@
 tests/test_decorator.py
 tests/test_exception_on_invalid_code.py
 tests/test_flake8_async.py
 tests/test_formatting.py
 tests/test_messages_documented.py
 tests/trio_options.py
 tests/autofix_files/async100.py
+tests/autofix_files/async100_asyncio.py
 tests/autofix_files/async100_simple_autofix.py
 tests/autofix_files/async910.py
 tests/autofix_files/async911.py
 tests/autofix_files/async91x_autofix.py
 tests/autofix_files/noqa.py
 tests/autofix_files/noqa_testing.py
 tests/eval_files/anyio_trio.py
@@ -71,15 +71,19 @@
 tests/eval_files/async104_trio.py
 tests/eval_files/async105.py
 tests/eval_files/async105_anyio.py
 tests/eval_files/async106.py
 tests/eval_files/async109.py
 tests/eval_files/async110.py
 tests/eval_files/async111.py
+tests/eval_files/async111_anyio.py
+tests/eval_files/async111_asyncio.py
 tests/eval_files/async112.py
+tests/eval_files/async112_anyio.py
+tests/eval_files/async112_asyncio.py
 tests/eval_files/async113.py
 tests/eval_files/async113_anyio.py
 tests/eval_files/async113_trio.py
 tests/eval_files/async114.py
 tests/eval_files/async115.py
 tests/eval_files/async116.py
 tests/eval_files/async118.py
@@ -98,14 +102,16 @@
 tests/eval_files/async250.py
 tests/eval_files/async250_multi_library.py
 tests/eval_files/async251.py
 tests/eval_files/async251_multi_library.py
 tests/eval_files/async900.py
 tests/eval_files/async910.py
 tests/eval_files/async911.py
+tests/eval_files/async912.py
+tests/eval_files/async912_asyncio.py
 tests/eval_files/async91x_autofix.py
 tests/eval_files/async91x_noautofix.py
 tests/eval_files/no_library.py
 tests/eval_files/noqa.py
 tests/eval_files/noqa_no_autofix.py
 tests/eval_files/noqa_testing.py
 tests/eval_files/trio_anyio.py
```

### Comparing `flake8_async-24.4.2/pyproject.toml` & `flake8_async-24.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/setup.py` & `flake8_async-24.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/autofix_files/async100.py` & `flake8_async-24.5.1/tests/autofix_files/async100.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,18 +67,19 @@
             if ...:
                 await trio.sleep(1)
 
     async with random_ignored_library.fail_after(10):
         ...
 
 
-# Seems like the inner context manager 'hides' the checkpoint.
+# The outer cancelscope can get triggered in more complex cases, so
+# to avoid false positives we don't raise a warning.
 async def does_contain_checkpoints():
-    with trio.fail_after(1):  # false-alarm ASYNC100
-        with trio.CancelScope():  # or any other context manager
+    with trio.fail_after(1):
+        with trio.CancelScope():
             await trio.sleep_forever()
 
 
 async def more_nested_tests():
     with trio.fail_after(1):
         with trio.CancelScope():
             await trio.sleep_forever()
```

### Comparing `flake8_async-24.4.2/tests/autofix_files/async100_simple_autofix.py` & `flake8_async-24.5.1/tests/autofix_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/autofix_files/async910.py` & `flake8_async-24.5.1/tests/autofix_files/async910.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # AUTOFIX
+# ASYNCIO_NO_AUTOFIX
 # mypy: disable-error-code="unreachable"
 from __future__ import annotations
 
 import typing
 from typing import Any, overload
 
 import pytest
```

### Comparing `flake8_async-24.4.2/tests/autofix_files/async911.py` & `flake8_async-24.5.1/tests/autofix_files/async911.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # AUTOFIX
+# ASYNCIO_NO_AUTOFIX
 from typing import Any
 
 import pytest
 import trio
 
 _: Any = ""
```

### Comparing `flake8_async-24.4.2/tests/autofix_files/async91x_autofix.py` & `flake8_async-24.5.1/tests/autofix_files/async91x_autofix.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # AUTOFIX
+# asyncio will raise the same errors, but does not have autofix available
+# ASYNCIO_NO_AUTOFIX
 from __future__ import annotations
 
 """Docstring for file
 
 So we make sure that import is added after it.
 """
 # isort: skip_file
@@ -120,7 +122,25 @@
         ...
     while ...:
         if bar():
             continue
         break
     [... for i in range(5)]
     return
+
+
+# TODO: issue 240
+async def livelocks():
+    while True:
+        ...
+
+
+# this will autofix 910 by adding a checkpoint outside the loop, which doesn't actually
+# help, and the method still isn't guaranteed to checkpoint in case bar() always returns
+# True.
+async def no_checkpoint():  # ASYNC910: 0, "exit", Statement("function definition", lineno)
+    while bar():
+        try:
+            await foo("1")  # type: ignore[call-arg]
+        except TypeError:
+            ...
+    await trio.lowlevel.checkpoint()
```

### Comparing `flake8_async-24.4.2/tests/autofix_files/noqa.py` & `flake8_async-24.5.1/tests/autofix_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/conftest.py` & `flake8_async-24.5.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async100.py` & `flake8_async-24.5.1/tests/eval_files/async100.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,18 +67,19 @@
                 if ...:
                     await trio.sleep(1)
 
     async with random_ignored_library.fail_after(10):
         ...
 
 
-# Seems like the inner context manager 'hides' the checkpoint.
+# The outer cancelscope can get triggered in more complex cases, so
+# to avoid false positives we don't raise a warning.
 async def does_contain_checkpoints():
-    with trio.fail_after(1):  # false-alarm ASYNC100
-        with trio.CancelScope():  # or any other context manager
+    with trio.fail_after(1):
+        with trio.CancelScope():
             await trio.sleep_forever()
 
 
 async def more_nested_tests():
     with trio.fail_after(1):
         with trio.CancelScope():
             await trio.sleep_forever()
```

### Comparing `flake8_async-24.4.2/tests/eval_files/async100_asyncio.py` & `flake8_async-24.5.1/tests/eval_files/async100_asyncio.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # TRIO_NO_ERROR
 # ANYIO_NO_ERROR
 # BASE_LIBRARY asyncio
-# ASYNCIO_NO_ERROR # TODO
+
+# timeout[_at] re-exported in the main asyncio namespace in py3.11
+# mypy: disable-error-code=attr-defined
+# AUTOFIX
 
 import asyncio
 import asyncio.timeouts
 
 
 async def foo():
-    # py>=3.11 re-exports these in the main asyncio namespace
-    with asyncio.timeout_at(10):  # type: ignore[attr-defined]
-        ...
-    with asyncio.timeout_at(10):  # type: ignore[attr-defined]
+    with asyncio.timeout_at(10):  # error: 9, "asyncio", "timeout_at"
         ...
-    with asyncio.timeout(10):  # type: ignore[attr-defined]
+    with asyncio.timeout(10):  # error: 9, "asyncio", "timeout"
         ...
-    with asyncio.timeouts.timeout_at(10):
-        ...
-    with asyncio.timeouts.timeout_at(10):
+
+    with asyncio.timeouts.timeout_at(10):  # error: 9, "asyncio.timeouts", "timeout_at"
         ...
-    with asyncio.timeouts.timeout(10):
+    with asyncio.timeouts.timeout(10):  # error: 9, "asyncio.timeouts", "timeout"
         ...
```

### Comparing `flake8_async-24.4.2/tests/eval_files/async100_noautofix.py` & `flake8_async-24.5.1/tests/eval_files/async100_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async100_simple_autofix.py` & `flake8_async-24.5.1/tests/eval_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async101.py` & `flake8_async-24.5.1/tests/eval_files/async101.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async102.py` & `flake8_async-24.5.1/tests/eval_files/async102.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async102_aclose.py` & `flake8_async-24.5.1/tests/eval_files/async102_aclose.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async102_aclose_args.py` & `flake8_async-24.5.1/tests/eval_files/async102_aclose_args.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async102_anyio.py` & `flake8_async-24.5.1/tests/eval_files/async102_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async102_asyncio.py` & `flake8_async-24.5.1/tests/eval_files/async102_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async102_trio.py` & `flake8_async-24.5.1/tests/eval_files/async102_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async103.py` & `flake8_async-24.5.1/tests/eval_files/async103.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async103_all_imported.py` & `flake8_async-24.5.1/tests/eval_files/async103_all_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async103_both_imported.py` & `flake8_async-24.5.1/tests/eval_files/async103_both_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async103_trio.py` & `flake8_async-24.5.1/tests/eval_files/async103_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async104.py` & `flake8_async-24.5.1/tests/eval_files/async104.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async104_anyio.py` & `flake8_async-24.5.1/tests/eval_files/async104_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async105.py` & `flake8_async-24.5.1/tests/eval_files/async105.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async106.py` & `flake8_async-24.5.1/tests/eval_files/async106.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async109.py` & `flake8_async-24.5.1/tests/eval_files/async109.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async110.py` & `flake8_async-24.5.1/tests/eval_files/async110.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async111.py` & `flake8_async-24.5.1/tests/eval_files/async111.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # type: ignore
 # ASYNC111: Variable, from context manager opened inside nursery, passed to start[_soon] might be invalidly accessed while in use, due to context manager closing before the nursery. This is usually a bug, and nurseries should generally be the inner-most context manager.
 # It's possible there's an equivalent asyncio construction/gotcha, but methods are differently named, so this file will not raise any errors
-# ASYNCIO_NO_ERROR # no nurseries in asyncio. Though maybe the bug is relevant for TaskGroups
+# nurseries are named taskgroups in asyncio/anyio
+# ASYNCIO_NO_ERROR
+# ANYIO_NO_ERROR
 from typing import Any
 
 import trio
 import trio as noterror
 
 
 # shed/black breaks up a *ton* of lines since adding more detailed error messages, so
@@ -238,7 +240,13 @@
 b = trio.open()
 with trio.open_nursery() as nursery:
     with b as nursery:
         with open("") as f:
             nursery.start(f)
 
 # fmt: on
+
+# visitor does not care to keep track of the type of nursery/taskgroup, so we
+# raise errors on .create_task() even if it doesn't exist in trio.
+with trio.open_nursery() as nursery:
+    with open("") as f:
+        nursery.create_task(f)  # error: 28, line-1, line-2, "f", "create_task"
```

### Comparing `flake8_async-24.4.2/tests/eval_files/async112.py` & `flake8_async-24.5.1/tests/eval_files/async112.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # type: ignore
 # ASYNC112: Nursery body with only a call to nursery.start[_soon] and not passing itself as a parameter can be replaced with a regular function call.
-# ASYNCIO_NO_ERROR - # TODO: expand check to work with asyncio.TaskGroup
-# ANYIO_NO_ERROR - # TODO: expand check to work with anyio.TaskGroup
+# ASYNCIO_NO_ERROR
+# ANYIO_NO_ERROR
 import functools
 from functools import partial
 
 import trio
 import trio as noterror
 
 # error
@@ -77,17 +77,17 @@
 # fmt: on
 
 # n as a parameter to lambda is in fact not using it, but we don't parse
 with trio.open_nursery() as n:
     n.start_soon(lambda n: n + 1)
 
 
-# body isn't a call to n.start
+# body is a call to await n.start
 async def foo_1():
-    with trio.open_nursery(...) as n:
+    with trio.open_nursery(...) as n:  # error: 9, "n"
         await n.start(...)
 
 
 # not *trio*.open_nursery
 with noterror.open_nursery(...) as n:
     n.start(...)
```

### Comparing `flake8_async-24.4.2/tests/eval_files/async113.py` & `flake8_async-24.5.1/tests/eval_files/async113.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async113_trio.py` & `flake8_async-24.5.1/tests/eval_files/async113_trio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async114.py` & `flake8_async-24.5.1/tests/eval_files/async114.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async115.py` & `flake8_async-24.5.1/tests/eval_files/async115.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async116.py` & `flake8_async-24.5.1/tests/eval_files/async116.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async118.py` & `flake8_async-24.5.1/tests/eval_files/async118.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async119.py` & `flake8_async-24.5.1/tests/eval_files/async119.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async200.py` & `flake8_async-24.5.1/tests/eval_files/async200.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async210.py` & `flake8_async-24.5.1/tests/eval_files/async210.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async211.py` & `flake8_async-24.5.1/tests/eval_files/async211.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async212.py` & `flake8_async-24.5.1/tests/eval_files/async212.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async22x.py` & `flake8_async-24.5.1/tests/eval_files/async22x.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async22x_asyncio.py` & `flake8_async-24.5.1/tests/eval_files/async22x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async232.py` & `flake8_async-24.5.1/tests/eval_files/async232.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async232_asyncio.py` & `flake8_async-24.5.1/tests/eval_files/async232_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async23x.py` & `flake8_async-24.5.1/tests/eval_files/async23x.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async23x_asyncio.py` & `flake8_async-24.5.1/tests/eval_files/async23x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async240.py` & `flake8_async-24.5.1/tests/eval_files/async240.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async900.py` & `flake8_async-24.5.1/tests/eval_files/async900.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/async910.py` & `flake8_async-24.5.1/tests/eval_files/async910.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # AUTOFIX
+# ASYNCIO_NO_AUTOFIX
 # mypy: disable-error-code="unreachable"
 from __future__ import annotations
 
 import typing
 from typing import Any, overload
 
 import pytest
```

### Comparing `flake8_async-24.4.2/tests/eval_files/async911.py` & `flake8_async-24.5.1/tests/eval_files/async911.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # AUTOFIX
+# ASYNCIO_NO_AUTOFIX
 from typing import Any
 
 import pytest
 import trio
 
 _: Any = ""
```

### Comparing `flake8_async-24.4.2/tests/eval_files/async91x_autofix.py` & `flake8_async-24.5.1/tests/eval_files/async91x_autofix.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # AUTOFIX
+# asyncio will raise the same errors, but does not have autofix available
+# ASYNCIO_NO_AUTOFIX
 from __future__ import annotations
 
 """Docstring for file
 
 So we make sure that import is added after it.
 """
 # isort: skip_file
@@ -105,7 +107,24 @@
         ...
     while ...:
         if bar():
             continue
         break
     [... for i in range(5)]
     return
+
+
+# TODO: issue 240
+async def livelocks():
+    while True:
+        ...
+
+
+# this will autofix 910 by adding a checkpoint outside the loop, which doesn't actually
+# help, and the method still isn't guaranteed to checkpoint in case bar() always returns
+# True.
+async def no_checkpoint():  # ASYNC910: 0, "exit", Statement("function definition", lineno)
+    while bar():
+        try:
+            await foo("1")  # type: ignore[call-arg]
+        except TypeError:
+            ...
```

### Comparing `flake8_async-24.4.2/tests/eval_files/async91x_noautofix.py` & `flake8_async-24.5.1/tests/eval_files/async91x_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/eval_files/noqa.py` & `flake8_async-24.5.1/tests/eval_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/test_all_visitors_imported.py` & `flake8_async-24.5.1/tests/test_all_visitors_imported.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/test_changelog_and_version.py` & `flake8_async-24.5.1/tests/test_changelog_and_version.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/test_config_and_args.py` & `flake8_async-24.5.1/tests/test_config_and_args.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/test_decorator.py` & `flake8_async-24.5.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/test_exception_on_invalid_code.py` & `flake8_async-24.5.1/tests/test_exception_on_invalid_code.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tests/test_flake8_async.py` & `flake8_async-24.5.1/tests/test_flake8_async.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,28 +105,40 @@
 
 
 def check_autofix(
     test: str,
     plugin: Plugin,
     unfixed_code: str,
     generate_autofix: bool,
+    magic_markers: MagicMarkers,
     library: str = "trio",
-    base_library: str = "trio",
 ):
+    base_library = magic_markers.BASE_LIBRARY
     # the source code after it's been visited by current transformers
     visited_code = plugin.module.code
 
-    if "# AUTOFIX" not in unfixed_code:
-        # if the file is specifically marked with NOAUTOFIX, that means it has visitors
-        # that will autofix with --autofix, but the file explicitly doesn't want to check
-        # the result of doing that. THIS IS DANGEROUS
-        if "# NOAUTOFIX" in unfixed_code:
-            print(f"eval file {test} marked with dangerous marker NOAUTOFIX")
-        else:
-            assert unfixed_code == visited_code
+    # if the file is specifically marked with NOAUTOFIX, that means it has visitors
+    # that will autofix with --autofix, but the file explicitly doesn't want to check
+    # the result of doing that. THIS IS DANGEROUS
+    assert not (magic_markers.AUTOFIX and magic_markers.NOAUTOFIX)
+    if magic_markers.NOAUTOFIX:
+        print(f"eval file {test} marked with dangerous marker NOAUTOFIX")
+        return
+
+    if (
+        # not marked for autofixing
+        not magic_markers.AUTOFIX
+        # file+library does not raise errors
+        or magic_markers.library_no_error(library)
+        # code raises errors on asyncio, but does not support autofixing for it
+        or (library == "asyncio" and magic_markers.ASYNCIO_NO_AUTOFIX)
+    ):
+        assert (
+            unfixed_code == visited_code
+        ), "Code changed after visiting, but magic markers say it shouldn't change."
         return
 
     # the full generated source code, saved from a previous run
     if test not in autofix_files:
         autofix_files[test] = AUTOFIX_DIR / (test.lower() + ".py")
         autofix_files[test].write_text("")
     previous_autofixed = autofix_files[test].read_text()
@@ -192,17 +204,30 @@
     NOANYIO: bool = False
     NOTRIO: bool = False
     NOASYNCIO: bool = False
     # File should raise no errors with this library
     ANYIO_NO_ERROR: bool = False
     TRIO_NO_ERROR: bool = False
     ASYNCIO_NO_ERROR: bool = False
+
+    AUTOFIX: bool = False
+    NOAUTOFIX: bool = False
+
+    # File should not get modified when running with asyncio+autofix
+    ASYNCIO_NO_AUTOFIX: bool = False
     # eval file is written using this library, so no substitution is required
     BASE_LIBRARY: str = "trio"
 
+    def library_no_error(self, library: str) -> bool:
+        return {
+            "anyio": self.ANYIO_NO_ERROR,
+            "asyncio": self.ASYNCIO_NO_ERROR,
+            "trio": self.TRIO_NO_ERROR,
+        }[library]
+
 
 def find_magic_markers(
     content: str,
 ) -> MagicMarkers:
     found_markers = MagicMarkers()
     markers = (f.name for f in fields(found_markers))
     pattern = rf'# ({"|".join(markers)})'
@@ -296,23 +321,22 @@
     ):
         for error in errors:
             message = error.message.format(*error.args)
             assert library in message or not any(
                 lib in message for lib in ("anyio", "asyncio", "trio")
             )
 
-    # asyncio does not support autofix atm, so should not modify content
-    if autofix and not noqa and library != "asyncio":
+    if autofix and not noqa:
         check_autofix(
             test,
             plugin,
             content,
             generate_autofix,
             library=library,
-            base_library=magic_markers.BASE_LIBRARY,
+            magic_markers=magic_markers,
         )
     else:
         # make sure content isn't modified
         assert content == plugin.module.code
 
 
 # check that autofixed files raise no errors and doesn't get autofixed (again)
@@ -448,14 +472,15 @@
     "ASYNC106",
     "ASYNC111",
     "ASYNC112",
     "ASYNC115",
     "ASYNC116",
     "ASYNC117",
     "ASYNC118",
+    "ASYNC912",
 }
 
 
 class SyncTransformer(ast.NodeTransformer):
     def visit_Await(self, node: ast.Await):
         return self.generic_visit(node.value)
 
@@ -475,15 +500,15 @@
     def visit_AsyncWith(self, node: ast.AsyncWith):
         return self.replace_async(node, ast.With)
 
     def visit_AsyncFor(self, node: ast.AsyncFor):
         return self.replace_async(node, ast.For, node.target, node.iter)
 
 
-@pytest.mark.parametrize(("test", "path"), test_files)
+@pytest.mark.parametrize(("test", "path"), test_files, ids=[f[0] for f in test_files])
 def test_noerror_on_sync_code(test: str, path: Path):
     if any(e in test for e in error_codes_ignored_when_checking_transformed_sync_code):
         return
     with tokenize.open(path) as f:
         source = f.read()
     tree = SyncTransformer().visit(ast.parse(source))
```

### Comparing `flake8_async-24.4.2/tests/test_messages_documented.py` & `flake8_async-24.5.1/tests/test_messages_documented.py`

 * *Files identical despite different names*

### Comparing `flake8_async-24.4.2/tox.ini` & `flake8_async-24.5.1/tox.ini`

 * *Files identical despite different names*

