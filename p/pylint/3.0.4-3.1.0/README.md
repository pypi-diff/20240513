# Comparing `tmp/pylint-3.0.4.tar.gz` & `tmp/pylint-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylint-3.0.4.tar", last modified: Fri Feb 23 20:55:33 2024, max compression
+gzip compressed data, was "pylint-3.1.0.tar", last modified: Sun Feb 25 16:48:16 2024, max compression
```

## Comparing `pylint-3.0.4.tar` & `pylint-3.1.0.tar`

### file list

```diff
@@ -1,220 +1,4552 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.418804 pylint-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    29986 2024-02-23 20:55:21.000000 pylint-3.0.4/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)    17984 2024-02-23 20:55:21.000000 pylint-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-23 20:55:21.000000 pylint-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-02-23 20:55:33.418804 pylint-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-02-23 20:55:21.000000 pylint-3.0.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.382804 pylint-3.0.4/pylint/
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/__pkginfo__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.390804 pylint-3.0.4/pylint/checkers/
--rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/bad_chained_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.390804 pylint-3.0.4/pylint/checkers/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40366 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/base/basic_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    22450 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/base/basic_error_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/base/comparison_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/base/docstring_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.390804 pylint-3.0.4/pylint/checkers/base/name_checker/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/base/name_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27219 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/base/name_checker/checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/base/name_checker/naming_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/base/pass_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/base_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.394804 pylint-3.0.4/pylint/checkers/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    91151 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/classes/class_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15125 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/classes/special_methods_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/dataclass_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     9671 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    22585 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/design_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/dunder_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/ellipsis_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    26303 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    26794 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    42302 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/lambda_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/method_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7723 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/modified_iterating_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/nested_min_max.py
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/newstyle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/non_ascii_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/raw_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.394804 pylint-3.0.4/pylint/checkers/refactoring/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/refactoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/refactoring/implicit_booleaness_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/refactoring/not_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    18659 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/refactoring/recommendation_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    97491 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/refactoring/refactoring_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    33933 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/similar.py
--rw-r--r--   0 runner    (1001) docker     (127)    16452 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/spelling.py
--rw-r--r--   0 runner    (1001) docker     (127)    33377 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    44275 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/threading_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    89543 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (127)    18490 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/unicode.py
--rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/unsupported_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    77535 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   134762 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/checkers/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.394804 pylint-3.0.4/pylint/config/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.398804 pylint-3.0.4/pylint/config/_pylint_config/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/_pylint_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/_pylint_config/generate_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/_pylint_config/help_message.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/_pylint_config/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/_pylint_config/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/_pylint_config/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    14816 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)    15085 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/arguments_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/arguments_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/callback_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/config_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/config_initialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/deprecation_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/find_default_config_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/help_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8704 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.402804 pylint-3.0.4/pylint/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29753 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/_check_docs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/bad_builtin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/broad_try_clause.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/check_elif.py
--rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/code_style.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/comparison_placement.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/confusing_elif.py
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/consider_refactoring_into_while_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/consider_ternary_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/dict_init_mutate.py
--rw-r--r--   0 runner    (1001) docker     (127)    25473 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/docparams.py
--rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/docstyle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/dunder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/empty_comment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/eq_without_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/for_any_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/magic_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/mccabe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/no_self_use.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/overlapping_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11245 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/private_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/redefined_loop_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/redefined_variable_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/set_membership.py
--rw-r--r--   0 runner    (1001) docker     (127)    20400 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/extensions/while_used.py
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.402804 pylint-3.0.4/pylint/lint/
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/lint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21528 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/lint/base_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/lint/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/lint/expand_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/lint/message_state_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/lint/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)    50018 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/lint/pylinter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/lint/report_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/lint/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/lint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.402804 pylint-3.0.4/pylint/message/
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/message/_deleted_message_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/message/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/message/message_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/message/message_definition_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6457 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/message/message_id_store.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.406804 pylint-3.0.4/pylint/pyreverse/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/diadefslib.py
--rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/diagrams.py
--rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/dot_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13480 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/mermaidjs_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/plantuml_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/printer_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/pyreverse/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.406804 pylint-3.0.4/pylint/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/base_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/collecting_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/json_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/multi_reporter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/reports_handler_mix_in.py
--rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/text.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.406804 pylint-3.0.4/pylint/reporters/ureports/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/ureports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/ureports/base_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/ureports/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/reporters/ureports/text_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.410804 pylint-3.0.4/pylint/testutils/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.410804 pylint-3.0.4/pylint/testutils/_primer/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/_primer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/_primer/package_to_lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/_primer/primer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/_primer/primer_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/_primer/primer_compare_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/_primer/primer_prepare_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/_primer/primer_run_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/checker_test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.410804 pylint-3.0.4/pylint/testutils/functional/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/functional/find_functional_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/functional/lint_module_output_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/functional/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/get_test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/global_test_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/lint_module_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/output_line.py
--rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/pyreverse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/reporter_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/testing_pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/tokenize_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/unittest_linter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/testutils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.414804 pylint-3.0.4/pylint/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/utils/ast_walker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/utils/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9632 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/utils/file_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/utils/linterstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/utils/pragma_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-02-23 20:55:21.000000 pylint-3.0.4/pylint/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.414804 pylint-3.0.4/pylint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-02-23 20:55:33.000000 pylint-3.0.4/pylint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6844 2024-02-23 20:55:33.000000 pylint-3.0.4/pylint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-23 20:55:33.000000 pylint-3.0.4/pylint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-23 20:55:33.000000 pylint-3.0.4/pylint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-23 20:55:33.000000 pylint-3.0.4/pylint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-23 20:55:33.000000 pylint-3.0.4/pylint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-02-23 20:55:21.000000 pylint-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-23 20:55:33.418804 pylint-3.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-23 20:55:33.414804 pylint-3.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    26010 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_check_parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_functional_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_import_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_numversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_pragma_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_pylint_runners.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_regr.py
--rw-r--r--   0 runner    (1001) docker     (127)    59412 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_self.py
--rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-02-23 20:55:21.000000 pylint-3.0.4/tests/test_similar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.811227 pylint-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    30701 2024-02-25 16:48:03.000000 pylint-3.1.0/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    17984 2024-02-25 16:48:03.000000 pylint-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-25 16:48:03.000000 pylint-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-02-25 16:48:16.811227 pylint-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-02-25 16:48:03.000000 pylint-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.203224 pylint-3.1.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/contact.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.203224 pylint-3.1.0/doc/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.127224 pylint-3.1.0/doc/data/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.075224 pylint-3.1.0/doc/data/messages/a/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.203224 pylint-3.1.0/doc/data/messages/a/abstract-class-instantiated/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/abstract-class-instantiated/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/abstract-class-instantiated/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.071224 pylint-3.1.0/doc/data/messages/a/abstract-method/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.203224 pylint-3.1.0/doc/data/messages/a/abstract-method/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/abstract-method/bad/abstract_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/abstract-method/bad/function_raising_not_implemented_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.203224 pylint-3.1.0/doc/data/messages/a/abstract-method/good/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/abstract-method/good/abstract_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/abstract-method/good/function_raising_not_implemented_error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.203224 pylint-3.1.0/doc/data/messages/a/access-member-before-definition/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/access-member-before-definition/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/access-member-before-definition/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.207224 pylint-3.1.0/doc/data/messages/a/anomalous-backslash-in-string/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/anomalous-backslash-in-string/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/anomalous-backslash-in-string/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.207224 pylint-3.1.0/doc/data/messages/a/anomalous-backslash-in-string/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/anomalous-backslash-in-string/good/double_escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/anomalous-backslash-in-string/good/existing_escape_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/anomalous-backslash-in-string/good/r_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/anomalous-backslash-in-string/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.207224 pylint-3.1.0/doc/data/messages/a/anomalous-unicode-escape-in-string/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/anomalous-unicode-escape-in-string/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/anomalous-unicode-escape-in-string/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.207224 pylint-3.1.0/doc/data/messages/a/arguments-differ/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/arguments-differ/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/arguments-differ/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.207224 pylint-3.1.0/doc/data/messages/a/arguments-differ/good/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/arguments-differ/good/add_option_in_base_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/arguments-differ/good/default_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/arguments-differ/good/no_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/arguments-differ/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.207224 pylint-3.1.0/doc/data/messages/a/arguments-out-of-order/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/arguments-out-of-order/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/arguments-out-of-order/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.207224 pylint-3.1.0/doc/data/messages/a/arguments-renamed/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/arguments-renamed/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/arguments-renamed/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.207224 pylint-3.1.0/doc/data/messages/a/assert-on-string-literal/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assert-on-string-literal/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assert-on-string-literal/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assert-on-string-literal/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assert-on-string-literal/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/a/assert-on-tuple/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assert-on-tuple/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assert-on-tuple/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assert-on-tuple/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/a/assigning-non-slot/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assigning-non-slot/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assigning-non-slot/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/a/assignment-from-no-return/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assignment-from-no-return/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assignment-from-no-return/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/a/assignment-from-none/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assignment-from-none/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/assignment-from-none/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/a/astroid-error/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/astroid-error/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/a/attribute-defined-outside-init/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/attribute-defined-outside-init/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/attribute-defined-outside-init/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/a/await-outside-async/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/await-outside-async/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/await-outside-async/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/a/await-outside-async/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.079224 pylint-3.1.0/doc/data/messages/b/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/b/bad-builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-builtin/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-builtin/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-builtin/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/b/bad-chained-comparison/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/b/bad-chained-comparison/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-chained-comparison/bad/parrot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-chained-comparison/bad/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.211224 pylint-3.1.0/doc/data/messages/b/bad-chained-comparison/good/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-chained-comparison/good/parrot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-chained-comparison/good/xor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-chained-comparison/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.215224 pylint-3.1.0/doc/data/messages/b/bad-classmethod-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-classmethod-argument/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-classmethod-argument/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.215224 pylint-3.1.0/doc/data/messages/b/bad-configuration-section/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-configuration-section/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.215224 pylint-3.1.0/doc/data/messages/b/bad-docstring-quotes/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-docstring-quotes/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-docstring-quotes/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-docstring-quotes/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-docstring-quotes/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-docstring-quotes/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.215224 pylint-3.1.0/doc/data/messages/b/bad-dunder-name/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-dunder-name/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-dunder-name/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-dunder-name/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.215224 pylint-3.1.0/doc/data/messages/b/bad-except-order/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-except-order/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-except-order/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.215224 pylint-3.1.0/doc/data/messages/b/bad-exception-cause/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-exception-cause/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-exception-cause/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-exception-cause/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.215224 pylint-3.1.0/doc/data/messages/b/bad-file-encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-file-encoding/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-file-encoding/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.215224 pylint-3.1.0/doc/data/messages/b/bad-format-character/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-format-character/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-format-character/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-format-character/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-format-character/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.219225 pylint-3.1.0/doc/data/messages/b/bad-format-string/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-format-string/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-format-string/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-format-string/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.219225 pylint-3.1.0/doc/data/messages/b/bad-format-string-key/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-format-string-key/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-format-string-key/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-format-string-key/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.219225 pylint-3.1.0/doc/data/messages/b/bad-indentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-indentation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-indentation/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-indentation/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.219225 pylint-3.1.0/doc/data/messages/b/bad-inline-option/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-inline-option/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-inline-option/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.219225 pylint-3.1.0/doc/data/messages/b/bad-mcs-classmethod-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-mcs-classmethod-argument/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-mcs-classmethod-argument/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.219225 pylint-3.1.0/doc/data/messages/b/bad-mcs-method-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-mcs-method-argument/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-mcs-method-argument/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.219225 pylint-3.1.0/doc/data/messages/b/bad-open-mode/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-open-mode/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-open-mode/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.219225 pylint-3.1.0/doc/data/messages/b/bad-plugin-value/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-plugin-value/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.219225 pylint-3.1.0/doc/data/messages/b/bad-reversed-sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-reversed-sequence/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-reversed-sequence/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.219225 pylint-3.1.0/doc/data/messages/b/bad-staticmethod-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-staticmethod-argument/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-staticmethod-argument/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.223224 pylint-3.1.0/doc/data/messages/b/bad-str-strip-call/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.223224 pylint-3.1.0/doc/data/messages/b/bad-str-strip-call/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-str-strip-call/bad/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-str-strip-call/bad/remove_abc_from_both_side.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-str-strip-call/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.223224 pylint-3.1.0/doc/data/messages/b/bad-str-strip-call/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-str-strip-call/good/hello_world.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-str-strip-call/good/remove_abc_from_both_side.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-str-strip-call/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.223224 pylint-3.1.0/doc/data/messages/b/bad-string-format-type/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-string-format-type/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-string-format-type/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-string-format-type/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-string-format-type/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.223224 pylint-3.1.0/doc/data/messages/b/bad-super-call/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-super-call/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-super-call/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-super-call/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-super-call/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.223224 pylint-3.1.0/doc/data/messages/b/bad-thread-instantiation/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-thread-instantiation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bad-thread-instantiation/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.223224 pylint-3.1.0/doc/data/messages/b/bare-except/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bare-except/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bare-except/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bare-except/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bare-except/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.223224 pylint-3.1.0/doc/data/messages/b/bidirectional-unicode/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bidirectional-unicode/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/bidirectional-unicode/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.227224 pylint-3.1.0/doc/data/messages/b/binary-op-exception/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/binary-op-exception/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/binary-op-exception/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.227224 pylint-3.1.0/doc/data/messages/b/boolean-datetime/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/boolean-datetime/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/boolean-datetime/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/boolean-datetime/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/boolean-datetime/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.227224 pylint-3.1.0/doc/data/messages/b/broad-exception-caught/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broad-exception-caught/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broad-exception-caught/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broad-exception-caught/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broad-exception-caught/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.227224 pylint-3.1.0/doc/data/messages/b/broad-exception-raised/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broad-exception-raised/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broad-exception-raised/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broad-exception-raised/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.227224 pylint-3.1.0/doc/data/messages/b/broken-collections-callable/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broken-collections-callable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broken-collections-callable/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broken-collections-callable/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broken-collections-callable/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.227224 pylint-3.1.0/doc/data/messages/b/broken-noreturn/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broken-noreturn/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broken-noreturn/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/b/broken-noreturn/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.083224 pylint-3.1.0/doc/data/messages/c/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.227224 pylint-3.1.0/doc/data/messages/c/c-extension-no-member/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/c-extension-no-member/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/c-extension-no-member/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.227224 pylint-3.1.0/doc/data/messages/c/catching-non-exception/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/catching-non-exception/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/catching-non-exception/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.231224 pylint-3.1.0/doc/data/messages/c/cell-var-from-loop/
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/cell-var-from-loop/bad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.231224 pylint-3.1.0/doc/data/messages/c/cell-var-from-loop/good/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/cell-var-from-loop/good/functools.partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/cell-var-from-loop/good/new_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/cell-var-from-loop/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.231224 pylint-3.1.0/doc/data/messages/c/chained-comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/chained-comparison/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/chained-comparison/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.231224 pylint-3.1.0/doc/data/messages/c/class-variable-slots-conflict/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/class-variable-slots-conflict/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/class-variable-slots-conflict/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.231224 pylint-3.1.0/doc/data/messages/c/comparison-of-constants/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/comparison-of-constants/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/comparison-of-constants/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.231224 pylint-3.1.0/doc/data/messages/c/comparison-with-callable/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/comparison-with-callable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/comparison-with-callable/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.231224 pylint-3.1.0/doc/data/messages/c/comparison-with-itself/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/comparison-with-itself/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/comparison-with-itself/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.231224 pylint-3.1.0/doc/data/messages/c/condition-evals-to-constant/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/condition-evals-to-constant/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/condition-evals-to-constant/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.231224 pylint-3.1.0/doc/data/messages/c/config-parse-error/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/config-parse-error/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.231224 pylint-3.1.0/doc/data/messages/c/confusing-consecutive-elif/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/confusing-consecutive-elif/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/confusing-consecutive-elif/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/confusing-consecutive-elif/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/confusing-consecutive-elif/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.235225 pylint-3.1.0/doc/data/messages/c/confusing-with-statement/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/confusing-with-statement/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/confusing-with-statement/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.235225 pylint-3.1.0/doc/data/messages/c/consider-alternative-union-syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-alternative-union-syntax/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-alternative-union-syntax/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-alternative-union-syntax/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.235225 pylint-3.1.0/doc/data/messages/c/consider-iterating-dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-iterating-dictionary/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-iterating-dictionary/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.235225 pylint-3.1.0/doc/data/messages/c/consider-merging-isinstance/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-merging-isinstance/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-merging-isinstance/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.235225 pylint-3.1.0/doc/data/messages/c/consider-refactoring-into-while-condition/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-refactoring-into-while-condition/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-refactoring-into-while-condition/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-refactoring-into-while-condition/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.235225 pylint-3.1.0/doc/data/messages/c/consider-swap-variables/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-swap-variables/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-swap-variables/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.235225 pylint-3.1.0/doc/data/messages/c/consider-ternary-expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-ternary-expression/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-ternary-expression/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-ternary-expression/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.235225 pylint-3.1.0/doc/data/messages/c/consider-using-alias/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-alias/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-alias/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-alias/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.235225 pylint-3.1.0/doc/data/messages/c/consider-using-any-or-all/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.235225 pylint-3.1.0/doc/data/messages/c/consider-using-any-or-all/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-any-or-all/bad/all_even.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-any-or-all/bad/any_even.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.239225 pylint-3.1.0/doc/data/messages/c/consider-using-any-or-all/good/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-any-or-all/good/all_even.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-any-or-all/good/any_even.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-any-or-all/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.239225 pylint-3.1.0/doc/data/messages/c/consider-using-assignment-expr/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-assignment-expr/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-assignment-expr/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-assignment-expr/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.239225 pylint-3.1.0/doc/data/messages/c/consider-using-augmented-assign/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-augmented-assign/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-augmented-assign/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-augmented-assign/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.239225 pylint-3.1.0/doc/data/messages/c/consider-using-dict-comprehension/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-dict-comprehension/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-dict-comprehension/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-dict-comprehension/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.239225 pylint-3.1.0/doc/data/messages/c/consider-using-dict-items/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-dict-items/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-dict-items/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.239225 pylint-3.1.0/doc/data/messages/c/consider-using-enumerate/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-enumerate/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-enumerate/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.239225 pylint-3.1.0/doc/data/messages/c/consider-using-f-string/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-f-string/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-f-string/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-f-string/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.239225 pylint-3.1.0/doc/data/messages/c/consider-using-from-import/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-from-import/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-from-import/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.243224 pylint-3.1.0/doc/data/messages/c/consider-using-generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-generator/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-generator/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-generator/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-generator/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.243224 pylint-3.1.0/doc/data/messages/c/consider-using-get/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-get/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-get/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.243224 pylint-3.1.0/doc/data/messages/c/consider-using-in/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-in/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-in/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.243224 pylint-3.1.0/doc/data/messages/c/consider-using-join/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-join/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-join/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.243224 pylint-3.1.0/doc/data/messages/c/consider-using-max-builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-max-builtin/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-max-builtin/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.243224 pylint-3.1.0/doc/data/messages/c/consider-using-min-builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-min-builtin/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-min-builtin/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.243224 pylint-3.1.0/doc/data/messages/c/consider-using-namedtuple-or-dataclass/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-namedtuple-or-dataclass/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-namedtuple-or-dataclass/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-namedtuple-or-dataclass/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.243224 pylint-3.1.0/doc/data/messages/c/consider-using-set-comprehension/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-set-comprehension/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-set-comprehension/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-set-comprehension/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.243224 pylint-3.1.0/doc/data/messages/c/consider-using-sys-exit/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-sys-exit/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-sys-exit/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.243224 pylint-3.1.0/doc/data/messages/c/consider-using-ternary/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-ternary/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-ternary/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.247225 pylint-3.1.0/doc/data/messages/c/consider-using-tuple/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-tuple/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-tuple/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-tuple/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.247225 pylint-3.1.0/doc/data/messages/c/consider-using-with/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.247225 pylint-3.1.0/doc/data/messages/c/consider-using-with/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-with/bad/close.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-with/bad/not_even_close.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-with/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-with/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/consider-using-with/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.247225 pylint-3.1.0/doc/data/messages/c/continue-in-finally/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/continue-in-finally/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/continue-in-finally/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/continue-in-finally/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/continue-in-finally/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.247225 pylint-3.1.0/doc/data/messages/c/cyclic-import/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.247225 pylint-3.1.0/doc/data/messages/c/cyclic-import/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/cyclic-import/bad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/cyclic-import/bad/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/cyclic-import/bad/bad2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/cyclic-import/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/c/cyclic-import/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.087224 pylint-3.1.0/doc/data/messages/d/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.247225 pylint-3.1.0/doc/data/messages/d/dangerous-default-value/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/dangerous-default-value/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/dangerous-default-value/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/dangerous-default-value/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.251225 pylint-3.1.0/doc/data/messages/d/deprecated-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-argument/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-argument/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-argument/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-argument/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.251225 pylint-3.1.0/doc/data/messages/d/deprecated-attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-attribute/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-attribute/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-attribute/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.251225 pylint-3.1.0/doc/data/messages/d/deprecated-class/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-class/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-class/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-class/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.251225 pylint-3.1.0/doc/data/messages/d/deprecated-decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-decorator/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-decorator/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-decorator/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-decorator/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.251225 pylint-3.1.0/doc/data/messages/d/deprecated-method/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-method/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-method/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-method/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.251225 pylint-3.1.0/doc/data/messages/d/deprecated-module/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-module/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-module/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-module/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-module/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.251225 pylint-3.1.0/doc/data/messages/d/deprecated-pragma/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-pragma/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-pragma/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.251225 pylint-3.1.0/doc/data/messages/d/deprecated-typing-alias/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-typing-alias/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-typing-alias/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/deprecated-typing-alias/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.255225 pylint-3.1.0/doc/data/messages/d/dict-init-mutate/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/dict-init-mutate/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/dict-init-mutate/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/dict-init-mutate/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.255225 pylint-3.1.0/doc/data/messages/d/dict-iter-missing-items/
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/dict-iter-missing-items/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/dict-iter-missing-items/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.255225 pylint-3.1.0/doc/data/messages/d/differing-param-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/differing-param-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/differing-param-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/differing-param-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.255225 pylint-3.1.0/doc/data/messages/d/differing-type-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/differing-type-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/differing-type-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/differing-type-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.255225 pylint-3.1.0/doc/data/messages/d/disallowed-name/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/disallowed-name/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/disallowed-name/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/disallowed-name/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.255225 pylint-3.1.0/doc/data/messages/d/docstring-first-line-empty/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/docstring-first-line-empty/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/docstring-first-line-empty/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/docstring-first-line-empty/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.255225 pylint-3.1.0/doc/data/messages/d/duplicate-argument-name/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-argument-name/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-argument-name/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.255225 pylint-3.1.0/doc/data/messages/d/duplicate-bases/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-bases/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-bases/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.255225 pylint-3.1.0/doc/data/messages/d/duplicate-code/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.259225 pylint-3.1.0/doc/data/messages/d/duplicate-code/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-code/bad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-code/bad/apple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-code/bad/orange.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-code/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.259225 pylint-3.1.0/doc/data/messages/d/duplicate-code/good/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-code/good/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-code/good/apple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-code/good/fruit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-code/good/orange.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.259225 pylint-3.1.0/doc/data/messages/d/duplicate-except/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-except/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-except/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.259225 pylint-3.1.0/doc/data/messages/d/duplicate-key/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-key/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-key/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-key/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.259225 pylint-3.1.0/doc/data/messages/d/duplicate-string-formatting-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-string-formatting-argument/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-string-formatting-argument/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.259225 pylint-3.1.0/doc/data/messages/d/duplicate-value/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-value/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/d/duplicate-value/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.087224 pylint-3.1.0/doc/data/messages/e/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.259225 pylint-3.1.0/doc/data/messages/e/else-if-used/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/else-if-used/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/else-if-used/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/else-if-used/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.259225 pylint-3.1.0/doc/data/messages/e/empty-comment/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/empty-comment/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/empty-comment/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/empty-comment/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.263225 pylint-3.1.0/doc/data/messages/e/empty-docstring/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/empty-docstring/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/empty-docstring/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.263225 pylint-3.1.0/doc/data/messages/e/eq-without-hash/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/eq-without-hash/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/eq-without-hash/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/eq-without-hash/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.263225 pylint-3.1.0/doc/data/messages/e/eval-used/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/eval-used/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/eval-used/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.263225 pylint-3.1.0/doc/data/messages/e/exec-used/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/exec-used/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/exec-used/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/exec-used/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/exec-used/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.263225 pylint-3.1.0/doc/data/messages/e/expression-not-assigned/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/expression-not-assigned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/e/expression-not-assigned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.087224 pylint-3.1.0/doc/data/messages/f/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.263225 pylint-3.1.0/doc/data/messages/f/f-string-without-interpolation/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/f-string-without-interpolation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/f-string-without-interpolation/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.263225 pylint-3.1.0/doc/data/messages/f/fatal/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/fatal/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.263225 pylint-3.1.0/doc/data/messages/f/file-ignored/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/file-ignored/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/file-ignored/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/file-ignored/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.263225 pylint-3.1.0/doc/data/messages/f/fixme/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/fixme/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/fixme/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/f/fixme/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/fixme/good/bug_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/fixme/good/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/fixme/good/no_fix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/f/forgotten-debug-statement/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/forgotten-debug-statement/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/forgotten-debug-statement/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/f/format-combined-specification/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/format-combined-specification/bad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/f/format-combined-specification/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/format-combined-specification/good/index_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/format-combined-specification/good/order_formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/f/format-needs-mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/format-needs-mapping/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/format-needs-mapping/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/f/format-string-without-interpolation/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/format-string-without-interpolation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/format-string-without-interpolation/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/f/function-redefined/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/function-redefined/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/f/function-redefined/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.091224 pylint-3.1.0/doc/data/messages/g/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/g/global-at-module-level/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/g/global-at-module-level/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/g/global-at-module-level/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/g/global-at-module-level/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/g/global-statement/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/g/global-statement/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/g/global-statement/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/g/global-variable-not-assigned/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/g/global-variable-not-assigned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/g/global-variable-not-assigned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/g/global-variable-undefined/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/g/global-variable-undefined/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/g/global-variable-undefined/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.095224 pylint-3.1.0/doc/data/messages/i/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.267225 pylint-3.1.0/doc/data/messages/i/implicit-flag-alias/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/implicit-flag-alias/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/implicit-flag-alias/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.271225 pylint-3.1.0/doc/data/messages/i/implicit-str-concat/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.271225 pylint-3.1.0/doc/data/messages/i/implicit-str-concat/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/implicit-str-concat/bad/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/implicit-str-concat/bad/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/implicit-str-concat/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.271225 pylint-3.1.0/doc/data/messages/i/implicit-str-concat/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/implicit-str-concat/good/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/implicit-str-concat/good/open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.271225 pylint-3.1.0/doc/data/messages/i/import-error/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/import-error/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/import-error/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/import-error/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.271225 pylint-3.1.0/doc/data/messages/i/import-outside-toplevel/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/import-outside-toplevel/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/import-outside-toplevel/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.271225 pylint-3.1.0/doc/data/messages/i/import-private-name/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/import-private-name/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/import-private-name/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/import-private-name/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/import-private-name/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.271225 pylint-3.1.0/doc/data/messages/i/import-self/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/import-self/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.271225 pylint-3.1.0/doc/data/messages/i/inconsistent-mro/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/inconsistent-mro/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/inconsistent-mro/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.271225 pylint-3.1.0/doc/data/messages/i/inconsistent-quotes/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/inconsistent-quotes/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/inconsistent-quotes/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/inconsistent-quotes/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.271225 pylint-3.1.0/doc/data/messages/i/inconsistent-return-statements/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/inconsistent-return-statements/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/inconsistent-return-statements/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.275225 pylint-3.1.0/doc/data/messages/i/inherit-non-class/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/inherit-non-class/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/inherit-non-class/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.275225 pylint-3.1.0/doc/data/messages/i/init-is-generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/init-is-generator/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/init-is-generator/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.275225 pylint-3.1.0/doc/data/messages/i/invalid-all-format/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-all-format/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-all-format/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.275225 pylint-3.1.0/doc/data/messages/i/invalid-all-object/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-all-object/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-all-object/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-all-object/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-all-object/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.275225 pylint-3.1.0/doc/data/messages/i/invalid-bool-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-bool-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-bool-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.275225 pylint-3.1.0/doc/data/messages/i/invalid-bytes-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-bytes-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-bytes-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.275225 pylint-3.1.0/doc/data/messages/i/invalid-character-backspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-backspace/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-backspace/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.275225 pylint-3.1.0/doc/data/messages/i/invalid-character-carriage-return/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-carriage-return/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-carriage-return/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.275225 pylint-3.1.0/doc/data/messages/i/invalid-character-esc/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-esc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-esc/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-character-nul/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-nul/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-nul/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-nul/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-character-sub/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-sub/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-sub/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-character-zero-width-space/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-zero-width-space/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-character-zero-width-space/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-characters-in-docstring/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-characters-in-docstring/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-class-object/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-class-object/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-class-object/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-enum-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-enum-extension/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-enum-extension/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-envvar-default/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-envvar-default/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-envvar-default/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-envvar-value/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-envvar-value/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-envvar-value/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-field-call/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-field-call/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-field-call/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-format-index/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-format-index/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-format-index/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-format-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-format-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-format-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.279225 pylint-3.1.0/doc/data/messages/i/invalid-getnewargs-ex-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-getnewargs-ex-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-getnewargs-ex-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.283225 pylint-3.1.0/doc/data/messages/i/invalid-getnewargs-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-getnewargs-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-getnewargs-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.283225 pylint-3.1.0/doc/data/messages/i/invalid-hash-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-hash-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-hash-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.283225 pylint-3.1.0/doc/data/messages/i/invalid-index-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-index-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-index-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.283225 pylint-3.1.0/doc/data/messages/i/invalid-length-hint-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-length-hint-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-length-hint-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.283225 pylint-3.1.0/doc/data/messages/i/invalid-length-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-length-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-length-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.283225 pylint-3.1.0/doc/data/messages/i/invalid-metaclass/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-metaclass/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-metaclass/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.283225 pylint-3.1.0/doc/data/messages/i/invalid-name/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-name/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10440 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-name/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-name/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.283225 pylint-3.1.0/doc/data/messages/i/invalid-overridden-method/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-overridden-method/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-overridden-method/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.283225 pylint-3.1.0/doc/data/messages/i/invalid-repr-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-repr-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-repr-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.283225 pylint-3.1.0/doc/data/messages/i/invalid-sequence-index/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-sequence-index/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-sequence-index/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-sequence-index/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/i/invalid-slice-index/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-slice-index/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-slice-index/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/i/invalid-slice-step/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-slice-step/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-slice-step/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/i/invalid-slots/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-slots/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-slots/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/i/invalid-slots-object/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-slots-object/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-slots-object/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-slots-object/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/i/invalid-star-assignment-target/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-star-assignment-target/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-star-assignment-target/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/i/invalid-str-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-str-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-str-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/i/invalid-unary-operand-type/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-unary-operand-type/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-unary-operand-type/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/i/invalid-unicode-codec/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/invalid-unicode-codec/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/i/isinstance-second-argument-not-valid-type/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/isinstance-second-argument-not-valid-type/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/i/isinstance-second-argument-not-valid-type/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.095224 pylint-3.1.0/doc/data/messages/k/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/k/keyword-arg-before-vararg/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/k/keyword-arg-before-vararg/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/k/keyword-arg-before-vararg/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.287225 pylint-3.1.0/doc/data/messages/k/kwarg-superseded-by-positional-arg/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/k/kwarg-superseded-by-positional-arg/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/k/kwarg-superseded-by-positional-arg/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.099224 pylint-3.1.0/doc/data/messages/l/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.291225 pylint-3.1.0/doc/data/messages/l/line-too-long/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/line-too-long/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/line-too-long/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/line-too-long/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/line-too-long/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.291225 pylint-3.1.0/doc/data/messages/l/literal-comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/literal-comparison/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/literal-comparison/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/literal-comparison/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.291225 pylint-3.1.0/doc/data/messages/l/locally-disabled/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/locally-disabled/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/locally-disabled/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.291225 pylint-3.1.0/doc/data/messages/l/logging-format-interpolation/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-format-interpolation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-format-interpolation/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-format-interpolation/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-format-interpolation/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.291225 pylint-3.1.0/doc/data/messages/l/logging-format-truncated/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-format-truncated/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-format-truncated/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.291225 pylint-3.1.0/doc/data/messages/l/logging-fstring-interpolation/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-fstring-interpolation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-fstring-interpolation/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-fstring-interpolation/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-fstring-interpolation/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.291225 pylint-3.1.0/doc/data/messages/l/logging-not-lazy/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-not-lazy/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-not-lazy/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-not-lazy/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-not-lazy/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/l/logging-too-few-args/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-too-few-args/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-too-few-args/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/l/logging-too-many-args/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-too-many-args/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-too-many-args/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/l/logging-unsupported-format/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-unsupported-format/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/logging-unsupported-format/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/l/lost-exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/lost-exception/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/l/lost-exception/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.103224 pylint-3.1.0/doc/data/messages/m/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/m/magic-value-comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/magic-value-comparison/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/magic-value-comparison/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/magic-value-comparison/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/m/method-cache-max-size-none/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/method-cache-max-size-none/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/method-cache-max-size-none/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/m/method-check-failed/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/method-check-failed/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/m/method-hidden/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/method-hidden/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/method-hidden/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/m/misplaced-bare-raise/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/misplaced-bare-raise/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/misplaced-bare-raise/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/m/misplaced-comparison-constant/
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/misplaced-comparison-constant/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/misplaced-comparison-constant/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/misplaced-comparison-constant/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.295225 pylint-3.1.0/doc/data/messages/m/misplaced-format-function/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/misplaced-format-function/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/misplaced-format-function/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.299225 pylint-3.1.0/doc/data/messages/m/misplaced-future/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/misplaced-future/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/misplaced-future/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/misplaced-future/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.299225 pylint-3.1.0/doc/data/messages/m/missing-any-param-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-any-param-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-any-param-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-any-param-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.299225 pylint-3.1.0/doc/data/messages/m/missing-class-docstring/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-class-docstring/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-class-docstring/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.299225 pylint-3.1.0/doc/data/messages/m/missing-final-newline/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.299225 pylint-3.1.0/doc/data/messages/m/missing-final-newline/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-final-newline/bad/crlf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-final-newline/bad/lf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-final-newline/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.299225 pylint-3.1.0/doc/data/messages/m/missing-final-newline/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-final-newline/good/crlf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-final-newline/good/lf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-final-newline/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.299225 pylint-3.1.0/doc/data/messages/m/missing-format-argument-key/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-format-argument-key/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-format-argument-key/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-format-argument-key/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.299225 pylint-3.1.0/doc/data/messages/m/missing-format-attribute/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-format-attribute/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-format-attribute/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.299225 pylint-3.1.0/doc/data/messages/m/missing-format-string-key/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-format-string-key/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-format-string-key/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.303225 pylint-3.1.0/doc/data/messages/m/missing-function-docstring/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-function-docstring/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-function-docstring/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.303225 pylint-3.1.0/doc/data/messages/m/missing-kwoa/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-kwoa/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-kwoa/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.303225 pylint-3.1.0/doc/data/messages/m/missing-module-docstring/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-module-docstring/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-module-docstring/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.303225 pylint-3.1.0/doc/data/messages/m/missing-param-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-param-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-param-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-param-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.303225 pylint-3.1.0/doc/data/messages/m/missing-parentheses-for-call-in-test/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-parentheses-for-call-in-test/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-parentheses-for-call-in-test/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.303225 pylint-3.1.0/doc/data/messages/m/missing-raises-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-raises-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-raises-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-raises-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.303225 pylint-3.1.0/doc/data/messages/m/missing-return-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-return-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-return-doc/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-return-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-return-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.303225 pylint-3.1.0/doc/data/messages/m/missing-return-type-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-return-type-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-return-type-doc/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-return-type-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-return-type-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.307225 pylint-3.1.0/doc/data/messages/m/missing-timeout/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-timeout/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-timeout/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-timeout/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.307225 pylint-3.1.0/doc/data/messages/m/missing-type-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-type-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-type-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-type-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.307225 pylint-3.1.0/doc/data/messages/m/missing-yield-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-yield-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-yield-doc/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-yield-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-yield-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.307225 pylint-3.1.0/doc/data/messages/m/missing-yield-type-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-yield-type-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-yield-type-doc/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-yield-type-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/missing-yield-type-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.307225 pylint-3.1.0/doc/data/messages/m/mixed-format-string/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/mixed-format-string/bad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.307225 pylint-3.1.0/doc/data/messages/m/mixed-format-string/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/mixed-format-string/good/only_named.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/mixed-format-string/good/only_ordered.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.307225 pylint-3.1.0/doc/data/messages/m/mixed-line-endings/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/mixed-line-endings/bad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.307225 pylint-3.1.0/doc/data/messages/m/mixed-line-endings/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/mixed-line-endings/good/full_crlf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/mixed-line-endings/good/full_lf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/mixed-line-endings/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.307225 pylint-3.1.0/doc/data/messages/m/modified-iterating-dict/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/modified-iterating-dict/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/modified-iterating-dict/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.311225 pylint-3.1.0/doc/data/messages/m/modified-iterating-list/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/modified-iterating-list/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/modified-iterating-list/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.311225 pylint-3.1.0/doc/data/messages/m/modified-iterating-set/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/modified-iterating-set/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/modified-iterating-set/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.311225 pylint-3.1.0/doc/data/messages/m/multiple-constructor-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/multiple-constructor-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/multiple-constructor-doc/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/multiple-constructor-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/multiple-constructor-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.311225 pylint-3.1.0/doc/data/messages/m/multiple-imports/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/multiple-imports/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/multiple-imports/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.311225 pylint-3.1.0/doc/data/messages/m/multiple-statements/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/multiple-statements/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/m/multiple-statements/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.107224 pylint-3.1.0/doc/data/messages/n/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.311225 pylint-3.1.0/doc/data/messages/n/named-expr-without-context/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/named-expr-without-context/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/named-expr-without-context/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.311225 pylint-3.1.0/doc/data/messages/n/nan-comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/nan-comparison/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/nan-comparison/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.311225 pylint-3.1.0/doc/data/messages/n/nested-min-max/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/nested-min-max/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/nested-min-max/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.311225 pylint-3.1.0/doc/data/messages/n/no-classmethod-decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-classmethod-decorator/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-classmethod-decorator/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.311225 pylint-3.1.0/doc/data/messages/n/no-else-break/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-else-break/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-else-break/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.315225 pylint-3.1.0/doc/data/messages/n/no-else-continue/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-else-continue/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-else-continue/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.315225 pylint-3.1.0/doc/data/messages/n/no-else-raise/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-else-raise/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-else-raise/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.315225 pylint-3.1.0/doc/data/messages/n/no-else-return/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-else-return/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-else-return/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.315225 pylint-3.1.0/doc/data/messages/n/no-member/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-member/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-member/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-member/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.315225 pylint-3.1.0/doc/data/messages/n/no-method-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-method-argument/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-method-argument/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.315225 pylint-3.1.0/doc/data/messages/n/no-name-in-module/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-name-in-module/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-name-in-module/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.315225 pylint-3.1.0/doc/data/messages/n/no-self-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-self-argument/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-self-argument/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.315225 pylint-3.1.0/doc/data/messages/n/no-self-use/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-self-use/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-self-use/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.315225 pylint-3.1.0/doc/data/messages/n/no-self-use/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-self-use/good/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-self-use/good/staticmethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-self-use/good/use_self.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-self-use/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.315225 pylint-3.1.0/doc/data/messages/n/no-staticmethod-decorator/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-staticmethod-decorator/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-staticmethod-decorator/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/no-value-for-parameter/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-value-for-parameter/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/no-value-for-parameter/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/non-ascii-file-name/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/non-ascii-file-name/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-ascii-file-name/bad/bàd.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-ascii-file-name/bad/not_bétter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/non-ascii-file-name/good/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-ascii-file-name/good/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-ascii-file-name/good/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-ascii-file-name/good/not_better.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-ascii-file-name/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/non-ascii-module-import/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-ascii-module-import/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-ascii-module-import/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/non-ascii-name/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-ascii-name/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-ascii-name/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/non-iterator-returned/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-iterator-returned/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-iterator-returned/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/non-parent-init-called/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-parent-init-called/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-parent-init-called/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/non-str-assignment-to-dunder-name/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-str-assignment-to-dunder-name/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/non-str-assignment-to-dunder-name/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/nonexistent-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/nonexistent-operator/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/nonexistent-operator/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.319225 pylint-3.1.0/doc/data/messages/n/nonlocal-and-global/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/nonlocal-and-global/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/nonlocal-and-global/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.323225 pylint-3.1.0/doc/data/messages/n/nonlocal-without-binding/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/nonlocal-without-binding/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/nonlocal-without-binding/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.323225 pylint-3.1.0/doc/data/messages/n/not-a-mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-a-mapping/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-a-mapping/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.323225 pylint-3.1.0/doc/data/messages/n/not-an-iterable/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-an-iterable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-an-iterable/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.323225 pylint-3.1.0/doc/data/messages/n/not-async-context-manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-async-context-manager/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-async-context-manager/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-async-context-manager/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.323225 pylint-3.1.0/doc/data/messages/n/not-callable/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-callable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-callable/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.323225 pylint-3.1.0/doc/data/messages/n/not-context-manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-context-manager/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-context-manager/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.323225 pylint-3.1.0/doc/data/messages/n/not-in-loop/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-in-loop/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/not-in-loop/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.323225 pylint-3.1.0/doc/data/messages/n/notimplemented-raised/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/notimplemented-raised/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/n/notimplemented-raised/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.107224 pylint-3.1.0/doc/data/messages/o/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.323225 pylint-3.1.0/doc/data/messages/o/overlapping-except/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/o/overlapping-except/bad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.323225 pylint-3.1.0/doc/data/messages/o/overlapping-except/good/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/o/overlapping-except/good/less_generic_first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/o/overlapping-except/good/only_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/o/overlapping-except/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/o/overlapping-except/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.327225 pylint-3.1.0/doc/data/messages/o/overridden-final-method/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/o/overridden-final-method/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/o/overridden-final-method/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/o/overridden-final-method/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/o/overridden-final-method/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/o/overridden-final-method/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.107224 pylint-3.1.0/doc/data/messages/p/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.327225 pylint-3.1.0/doc/data/messages/p/parse-error/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/parse-error/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.327225 pylint-3.1.0/doc/data/messages/p/pointless-exception-statement/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/pointless-exception-statement/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/pointless-exception-statement/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.327225 pylint-3.1.0/doc/data/messages/p/pointless-statement/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/pointless-statement/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/pointless-statement/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.327225 pylint-3.1.0/doc/data/messages/p/pointless-string-statement/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/pointless-string-statement/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/pointless-string-statement/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/pointless-string-statement/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.327225 pylint-3.1.0/doc/data/messages/p/positional-only-arguments-expected/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/positional-only-arguments-expected/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/positional-only-arguments-expected/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/positional-only-arguments-expected/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.327225 pylint-3.1.0/doc/data/messages/p/possibly-unused-variable/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/possibly-unused-variable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/possibly-unused-variable/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.327225 pylint-3.1.0/doc/data/messages/p/potential-index-error/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/potential-index-error/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/potential-index-error/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/p/prefer-typing-namedtuple/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/prefer-typing-namedtuple/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/prefer-typing-namedtuple/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/prefer-typing-namedtuple/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/prefer-typing-namedtuple/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/p/preferred-module/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/preferred-module/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/preferred-module/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/preferred-module/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/p/property-with-parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/property-with-parameters/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/property-with-parameters/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/p/protected-access/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/protected-access/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/p/protected-access/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.111224 pylint-3.1.0/doc/data/messages/r/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/r/raise-missing-from/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/raise-missing-from/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/raise-missing-from/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/raise-missing-from/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/r/raising-bad-type/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/raising-bad-type/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/raising-bad-type/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/r/raising-format-tuple/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/raising-format-tuple/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/raising-format-tuple/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/r/raising-non-exception/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/raising-non-exception/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/raising-non-exception/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/r/raw-checker-failed/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/raw-checker-failed/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/r/redeclared-assigned-name/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redeclared-assigned-name/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redeclared-assigned-name/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.331225 pylint-3.1.0/doc/data/messages/r/redefined-argument-from-local/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-argument-from-local/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-argument-from-local/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.335225 pylint-3.1.0/doc/data/messages/r/redefined-builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-builtin/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-builtin/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.335225 pylint-3.1.0/doc/data/messages/r/redefined-loop-name/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-loop-name/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-loop-name/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-loop-name/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.335225 pylint-3.1.0/doc/data/messages/r/redefined-outer-name/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-outer-name/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-outer-name/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-outer-name/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.335225 pylint-3.1.0/doc/data/messages/r/redefined-slots-in-subclass/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-slots-in-subclass/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-slots-in-subclass/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.335225 pylint-3.1.0/doc/data/messages/r/redefined-variable-type/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-variable-type/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-variable-type/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redefined-variable-type/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.335225 pylint-3.1.0/doc/data/messages/r/redundant-keyword-arg/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-keyword-arg/bad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.335225 pylint-3.1.0/doc/data/messages/r/redundant-keyword-arg/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-keyword-arg/good/only_arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-keyword-arg/good/only_kwarg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.335225 pylint-3.1.0/doc/data/messages/r/redundant-returns-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-returns-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-returns-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-returns-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.335225 pylint-3.1.0/doc/data/messages/r/redundant-typehint-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-typehint-argument/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-typehint-argument/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-typehint-argument/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.339225 pylint-3.1.0/doc/data/messages/r/redundant-u-string-prefix/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-u-string-prefix/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-u-string-prefix/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.339225 pylint-3.1.0/doc/data/messages/r/redundant-unittest-assert/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-unittest-assert/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-unittest-assert/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-unittest-assert/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-unittest-assert/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.339225 pylint-3.1.0/doc/data/messages/r/redundant-yields-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-yields-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-yields-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/redundant-yields-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.339225 pylint-3.1.0/doc/data/messages/r/reimported/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/reimported/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/reimported/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.339225 pylint-3.1.0/doc/data/messages/r/relative-beyond-top-level/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/relative-beyond-top-level/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/relative-beyond-top-level/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.339225 pylint-3.1.0/doc/data/messages/r/relative-beyond-top-level/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/relative-beyond-top-level/good/absolute_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/relative-beyond-top-level/good/fix_the_relative_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/relative-beyond-top-level/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.339225 pylint-3.1.0/doc/data/messages/r/repeated-keyword/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/repeated-keyword/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/repeated-keyword/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.339225 pylint-3.1.0/doc/data/messages/r/return-arg-in-generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-arg-in-generator/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-arg-in-generator/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-arg-in-generator/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.343225 pylint-3.1.0/doc/data/messages/r/return-in-finally/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-in-finally/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-in-finally/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-in-finally/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.343225 pylint-3.1.0/doc/data/messages/r/return-in-init/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-in-init/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-in-init/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-in-init/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.343225 pylint-3.1.0/doc/data/messages/r/return-outside-function/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-outside-function/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/r/return-outside-function/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.115224 pylint-3.1.0/doc/data/messages/s/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.343225 pylint-3.1.0/doc/data/messages/s/self-assigning-variable/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/self-assigning-variable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/self-assigning-variable/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/self-assigning-variable/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.343225 pylint-3.1.0/doc/data/messages/s/self-cls-assignment/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/self-cls-assignment/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/self-cls-assignment/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.343225 pylint-3.1.0/doc/data/messages/s/shadowed-import/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/shadowed-import/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/shadowed-import/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.343225 pylint-3.1.0/doc/data/messages/s/shallow-copy-environ/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/shallow-copy-environ/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/shallow-copy-environ/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.343225 pylint-3.1.0/doc/data/messages/s/signature-differs/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/signature-differs/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/signature-differs/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.343225 pylint-3.1.0/doc/data/messages/s/simplifiable-condition/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/simplifiable-condition/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/simplifiable-condition/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.347225 pylint-3.1.0/doc/data/messages/s/simplifiable-if-expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/simplifiable-if-expression/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/simplifiable-if-expression/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/simplifiable-if-expression/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.347225 pylint-3.1.0/doc/data/messages/s/simplifiable-if-statement/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/simplifiable-if-statement/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/simplifiable-if-statement/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.347225 pylint-3.1.0/doc/data/messages/s/simplify-boolean-expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/simplify-boolean-expression/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/simplify-boolean-expression/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.347225 pylint-3.1.0/doc/data/messages/s/single-string-used-for-slots/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/single-string-used-for-slots/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/single-string-used-for-slots/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.347225 pylint-3.1.0/doc/data/messages/s/singledispatch-method/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/singledispatch-method/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/singledispatch-method/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/singledispatch-method/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.347225 pylint-3.1.0/doc/data/messages/s/singledispatchmethod-function/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/singledispatchmethod-function/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/singledispatchmethod-function/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/singledispatchmethod-function/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.347225 pylint-3.1.0/doc/data/messages/s/singleton-comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/singleton-comparison/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/singleton-comparison/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/singleton-comparison/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.347225 pylint-3.1.0/doc/data/messages/s/star-needs-assignment-target/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/star-needs-assignment-target/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/star-needs-assignment-target/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.347225 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.351225 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/bad/fruit_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/bad/two_fruit_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/bad/two_good_fruit_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.351225 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/good/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/good/fruit_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/good/two_fruit_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/good/two_good_fruit_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/stop-iteration-return/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.351225 pylint-3.1.0/doc/data/messages/s/subclassed-final-class/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/subclassed-final-class/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/subclassed-final-class/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/subclassed-final-class/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/subclassed-final-class/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/subclassed-final-class/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.351225 pylint-3.1.0/doc/data/messages/s/subprocess-popen-preexec-fn/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/subprocess-popen-preexec-fn/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/subprocess-popen-preexec-fn/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.351225 pylint-3.1.0/doc/data/messages/s/subprocess-run-check/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/subprocess-run-check/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/subprocess-run-check/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/subprocess-run-check/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.351225 pylint-3.1.0/doc/data/messages/s/super-init-not-called/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/super-init-not-called/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/super-init-not-called/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.351225 pylint-3.1.0/doc/data/messages/s/super-with-arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/super-with-arguments/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/super-with-arguments/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.351225 pylint-3.1.0/doc/data/messages/s/super-without-brackets/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/super-without-brackets/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/super-without-brackets/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.115224 pylint-3.1.0/doc/data/messages/s/superfluous-parens/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.351225 pylint-3.1.0/doc/data/messages/s/superfluous-parens/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/superfluous-parens/bad/example_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/superfluous-parens/bad/example_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.355225 pylint-3.1.0/doc/data/messages/s/superfluous-parens/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/superfluous-parens/good/example_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/superfluous-parens/good/example_2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.355225 pylint-3.1.0/doc/data/messages/s/suppressed-message/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/suppressed-message/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/suppressed-message/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/suppressed-message/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.355225 pylint-3.1.0/doc/data/messages/s/syntax-error/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/syntax-error/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/s/syntax-error/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.119224 pylint-3.1.0/doc/data/messages/t/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.355225 pylint-3.1.0/doc/data/messages/t/too-complex/
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-complex/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-complex/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-complex/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.355225 pylint-3.1.0/doc/data/messages/t/too-few-format-args/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-few-format-args/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-few-format-args/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-few-format-args/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.355225 pylint-3.1.0/doc/data/messages/t/too-few-public-methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-few-public-methods/bad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.355225 pylint-3.1.0/doc/data/messages/t/too-few-public-methods/good/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-few-public-methods/good/dataclass_and_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-few-public-methods/good/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-few-public-methods/good/larger_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.355225 pylint-3.1.0/doc/data/messages/t/too-many-ancestors/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-ancestors/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-ancestors/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.355225 pylint-3.1.0/doc/data/messages/t/too-many-arguments/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-arguments/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-arguments/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.359225 pylint-3.1.0/doc/data/messages/t/too-many-boolean-expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-boolean-expressions/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-boolean-expressions/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.359225 pylint-3.1.0/doc/data/messages/t/too-many-branches/
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-branches/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-branches/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-branches/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.359225 pylint-3.1.0/doc/data/messages/t/too-many-format-args/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-format-args/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-format-args/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-format-args/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.359225 pylint-3.1.0/doc/data/messages/t/too-many-function-args/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-function-args/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-function-args/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.359225 pylint-3.1.0/doc/data/messages/t/too-many-instance-attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-instance-attributes/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-instance-attributes/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.359225 pylint-3.1.0/doc/data/messages/t/too-many-lines/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-lines/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-lines/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.359225 pylint-3.1.0/doc/data/messages/t/too-many-lines/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-lines/good/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-lines/good/is_palindrome.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-lines/good/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-lines/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.359225 pylint-3.1.0/doc/data/messages/t/too-many-locals/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-locals/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-locals/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-locals/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-locals/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.363225 pylint-3.1.0/doc/data/messages/t/too-many-nested-blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-nested-blocks/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-nested-blocks/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.363225 pylint-3.1.0/doc/data/messages/t/too-many-positional/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-positional/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-positional/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.363225 pylint-3.1.0/doc/data/messages/t/too-many-public-methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-public-methods/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-public-methods/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-public-methods/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-public-methods/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-public-methods/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.363225 pylint-3.1.0/doc/data/messages/t/too-many-return-statements/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-return-statements/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-return-statements/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.363225 pylint-3.1.0/doc/data/messages/t/too-many-star-expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-star-expressions/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-star-expressions/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.363225 pylint-3.1.0/doc/data/messages/t/too-many-statements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-statements/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-statements/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-statements/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.363225 pylint-3.1.0/doc/data/messages/t/too-many-try-statements/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-try-statements/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-try-statements/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/too-many-try-statements/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.363225 pylint-3.1.0/doc/data/messages/t/trailing-comma-tuple/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/trailing-comma-tuple/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/trailing-comma-tuple/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.363225 pylint-3.1.0/doc/data/messages/t/trailing-newlines/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/trailing-newlines/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/trailing-newlines/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.367225 pylint-3.1.0/doc/data/messages/t/trailing-whitespace/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/trailing-whitespace/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/trailing-whitespace/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.367225 pylint-3.1.0/doc/data/messages/t/truncated-format-string/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/truncated-format-string/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/truncated-format-string/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.367225 pylint-3.1.0/doc/data/messages/t/try-except-raise/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/try-except-raise/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/try-except-raise/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.367225 pylint-3.1.0/doc/data/messages/t/try-except-raise/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/try-except-raise/good/remove_try_except.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/try-except-raise/good/specialized_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.367225 pylint-3.1.0/doc/data/messages/t/typevar-double-variance/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/typevar-double-variance/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/typevar-double-variance/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.367225 pylint-3.1.0/doc/data/messages/t/typevar-name-incorrect-variance/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/typevar-name-incorrect-variance/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/typevar-name-incorrect-variance/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.367225 pylint-3.1.0/doc/data/messages/t/typevar-name-mismatch/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/typevar-name-mismatch/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/t/typevar-name-mismatch/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.127224 pylint-3.1.0/doc/data/messages/u/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.367225 pylint-3.1.0/doc/data/messages/u/unbalanced-dict-unpacking/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unbalanced-dict-unpacking/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unbalanced-dict-unpacking/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.367225 pylint-3.1.0/doc/data/messages/u/unbalanced-tuple-unpacking/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unbalanced-tuple-unpacking/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unbalanced-tuple-unpacking/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unbalanced-tuple-unpacking/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.367225 pylint-3.1.0/doc/data/messages/u/undefined-all-variable/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/undefined-all-variable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/undefined-all-variable/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/undefined-all-variable/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.371225 pylint-3.1.0/doc/data/messages/u/undefined-loop-variable/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/undefined-loop-variable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/undefined-loop-variable/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.371225 pylint-3.1.0/doc/data/messages/u/undefined-variable/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/undefined-variable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/undefined-variable/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.371225 pylint-3.1.0/doc/data/messages/u/unexpected-keyword-arg/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unexpected-keyword-arg/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unexpected-keyword-arg/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.371225 pylint-3.1.0/doc/data/messages/u/unexpected-line-ending-format/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unexpected-line-ending-format/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unexpected-line-ending-format/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unexpected-line-ending-format/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unexpected-line-ending-format/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.371225 pylint-3.1.0/doc/data/messages/u/unexpected-special-method-signature/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unexpected-special-method-signature/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unexpected-special-method-signature/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.371225 pylint-3.1.0/doc/data/messages/u/ungrouped-imports/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/ungrouped-imports/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/ungrouped-imports/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.371225 pylint-3.1.0/doc/data/messages/u/unhashable-member/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unhashable-member/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unhashable-member/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.371225 pylint-3.1.0/doc/data/messages/u/unidiomatic-typecheck/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unidiomatic-typecheck/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unidiomatic-typecheck/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unidiomatic-typecheck/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.371225 pylint-3.1.0/doc/data/messages/u/unknown-option-value/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unknown-option-value/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unknown-option-value/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.371225 pylint-3.1.0/doc/data/messages/u/unnecessary-comprehension/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-comprehension/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-comprehension/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-dict-index-lookup/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-dict-index-lookup/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-dict-index-lookup/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-direct-lambda-call/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-direct-lambda-call/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-direct-lambda-call/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-dunder-call/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-dunder-call/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-dunder-call/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-ellipsis/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-ellipsis/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-ellipsis/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.123224 pylint-3.1.0/doc/data/messages/u/unnecessary-lambda/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-lambda/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-lambda/bad/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-lambda/bad/print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-lambda/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-lambda/good/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-lambda/good/print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-lambda-assignment/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-lambda-assignment/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-lambda-assignment/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-list-index-lookup/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-list-index-lookup/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-list-index-lookup/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.123224 pylint-3.1.0/doc/data/messages/u/unnecessary-negation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-negation/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-negation/bad/double_not.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-negation/bad/equivalent_comparator_exists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-negation/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-negation/good/double_not.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-negation/good/equivalent_comparator_exists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.375225 pylint-3.1.0/doc/data/messages/u/unnecessary-pass/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-pass/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-pass/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unnecessary-semicolon/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-semicolon/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unnecessary-semicolon/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unpacking-non-sequence/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unpacking-non-sequence/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unpacking-non-sequence/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unreachable/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unreachable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unreachable/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unrecognize-option/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unrecognize-option/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unrecognized-inline-option/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unrecognized-inline-option/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unrecognized-inline-option/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unrecognized-option/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unrecognized-option/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unspecified-encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unspecified-encoding/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unspecified-encoding/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unsubscriptable-object/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsubscriptable-object/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsubscriptable-object/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unsupported-assignment-operation/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsupported-assignment-operation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsupported-assignment-operation/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unsupported-binary-operation/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsupported-binary-operation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsupported-binary-operation/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsupported-binary-operation/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.379225 pylint-3.1.0/doc/data/messages/u/unsupported-delete-operation/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsupported-delete-operation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsupported-delete-operation/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/unsupported-membership-test/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsupported-membership-test/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unsupported-membership-test/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/unused-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-argument/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-argument/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/unused-format-string-argument/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-format-string-argument/bad.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/unused-format-string-argument/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-format-string-argument/good/add_format_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-format-string-argument/good/remove_unused_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/unused-format-string-key/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-format-string-key/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-format-string-key/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/unused-import/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-import/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-import/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/unused-private-member/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-private-member/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-private-member/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/unused-variable/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-variable/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-variable/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/unused-wildcard-import/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-wildcard-import/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-wildcard-import/detail.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/unused-wildcard-import/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/use-a-generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-a-generator/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-a-generator/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-a-generator/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-a-generator/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/use-dict-literal/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/use-dict-literal/bad/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-dict-literal/bad/empty_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-dict-literal/bad/init_dict_from_another.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-dict-literal/bad/init_with_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-dict-literal/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.383225 pylint-3.1.0/doc/data/messages/u/use-dict-literal/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-dict-literal/good/empty_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-dict-literal/good/init_dict_from_another.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-dict-literal/good/init_with_litteral.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-dict-literal/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison-to-string/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison-to-string/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison-to-string/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison-to-string/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison-to-zero/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison-to-zero/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison-to-zero/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-comparison-to-zero/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-len/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-len/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-implicit-booleaness-not-len/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-list-literal/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-list-literal/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-list-literal/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-maxsplit-arg/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-maxsplit-arg/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-maxsplit-arg/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-maxsplit-arg/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-sequence-for-iteration/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-sequence-for-iteration/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-sequence-for-iteration/details.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-sequence-for-iteration/good/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-sequence-for-iteration/good/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-sequence-for-iteration/good/tuple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-set-for-membership/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-set-for-membership/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-set-for-membership/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-set-for-membership/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-symbolic-message-instead/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-symbolic-message-instead/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-symbolic-message-instead/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/use-yield-from/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-yield-from/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-yield-from/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-yield-from/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/use-yield-from/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/used-before-assignment/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/used-before-assignment/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/used-before-assignment/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.387225 pylint-3.1.0/doc/data/messages/u/used-prior-global-declaration/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/used-prior-global-declaration/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/used-prior-global-declaration/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/useless-else-on-loop/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-else-on-loop/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-else-on-loop/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/useless-import-alias/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-import-alias/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-import-alias/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-import-alias/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-import-alias/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/useless-object-inheritance/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-object-inheritance/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-object-inheritance/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/useless-option-value/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-option-value/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-option-value/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-option-value/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/useless-param-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-param-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-param-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-param-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/useless-parent-delegation/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-parent-delegation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-parent-delegation/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-parent-delegation/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/useless-return/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-return/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-return/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/useless-suppression/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-suppression/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-suppression/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/useless-type-doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-type-doc/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-type-doc/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-type-doc/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/useless-with-lock/
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-with-lock/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/useless-with-lock/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/using-constant-test/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-constant-test/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-constant-test/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.391225 pylint-3.1.0/doc/data/messages/u/using-f-string-in-unsupported-version/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-f-string-in-unsupported-version/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-f-string-in-unsupported-version/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-f-string-in-unsupported-version/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-f-string-in-unsupported-version/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/data/messages/u/using-final-decorator-in-unsupported-version/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-final-decorator-in-unsupported-version/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-final-decorator-in-unsupported-version/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-final-decorator-in-unsupported-version/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-final-decorator-in-unsupported-version/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/u/using-final-decorator-in-unsupported-version/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.127224 pylint-3.1.0/doc/data/messages/w/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/data/messages/w/while-used/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/while-used/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/while-used/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/while-used/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/while-used/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/data/messages/w/wildcard-import/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wildcard-import/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wildcard-import/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/data/messages/w/wrong-exception-operation/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-exception-operation/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-exception-operation/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/data/messages/w/wrong-import-order/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-import-order/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-import-order/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/data/messages/w/wrong-import-position/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-import-position/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-import-position/good.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/data/messages/w/wrong-spelling-in-comment/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-spelling-in-comment/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-spelling-in-comment/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-spelling-in-comment/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/data/messages/w/wrong-spelling-in-docstring/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-spelling-in-docstring/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-spelling-in-docstring/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/w/wrong-spelling-in-docstring/pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.131224 pylint-3.1.0/doc/data/messages/y/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/data/messages/y/yield-inside-async-function/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/y/yield-inside-async-function/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/y/yield-inside-async-function/details.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/y/yield-inside-async-function/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/y/yield-inside-async-function/related.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/data/messages/y/yield-outside-function/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/y/yield-outside-function/bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/messages/y/yield-outside-function/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/data/ruff.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.131224 pylint-3.1.0/doc/development_guide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.395225 pylint-3.1.0/doc/development_guide/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/api/pylint.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.399225 pylint-3.1.0/doc/development_guide/contributor_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/governance.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/major_release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/minor_release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/patch_release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/profiling.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/release.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.399225 pylint-3.1.0/doc/development_guide/contributor_guide/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/tests/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/tests/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/tests/launching_test.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/contributor_guide/tests/writing_test.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.399225 pylint-3.1.0/doc/development_guide/how_tos/
+-rw-r--r--   0 runner    (1001) docker     (127)    13061 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/how_tos/custom_checkers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/how_tos/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/how_tos/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/how_tos/transform_plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.399225 pylint-3.1.0/doc/development_guide/technical_reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/technical_reference/checkers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/technical_reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/development_guide/technical_reference/startup.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.399225 pylint-3.1.0/doc/exts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5412 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/exts/pylint_extensions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1525 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/exts/pylint_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16711 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/exts/pylint_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/exts/pylint_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9362 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    18453 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4826 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.403225 pylint-3.1.0/doc/media/
+-rw-r--r--   0 runner    (1001) docker     (127)   138128 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/media/ClassChecker_diagram.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/media/Tidelift_Logos_RGB_Tidelift_Shorthand_On-White_small.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30114 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/media/pyreverse_example_classes.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/media/pyreverse_example_packages.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/pyreverse.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/short_text_contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/short_text_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/symilar.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9132 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/test_messages_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9955 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.131224 pylint-3.1.0/doc/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.403225 pylint-3.1.0/doc/user_guide/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)    24318 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/checkers/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    82080 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/checkers/features.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/checkers/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.403225 pylint-3.1.0/doc/user_guide/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/configuration/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)    43960 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/configuration/all-options.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/configuration/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.403225 pylint-3.1.0/doc/user_guide/installation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/installation/badge.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/installation/command_line_installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.403225 pylint-3.1.0/doc/user_guide/installation/ide_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/installation/ide_integration/flymake-emacs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/installation/ide_integration/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/installation/ide_integration/textmate.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/installation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/installation/pre-commit-integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/installation/upgrading_pylint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/installation/with-multiple-interpreters.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.403225 pylint-3.1.0/doc/user_guide/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/messages/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/messages/message_control.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    17036 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/messages/messages_overview.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.403225 pylint-3.1.0/doc/user_guide/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/usage/output.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7979 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/user_guide/usage/run.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.407225 pylint-3.1.0/doc/whatsnew/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.407225 pylint-3.1.0/doc/whatsnew/0/
+-rw-r--r--   0 runner    (1001) docker     (127)    37309 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/0/0.x.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/0/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.407225 pylint-3.1.0/doc/whatsnew/1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.4.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21504 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.5.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.407225 pylint-3.1.0/doc/whatsnew/1/1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.6/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.6/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.6/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.407225 pylint-3.1.0/doc/whatsnew/1/1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.7/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.7/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    33477 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.7/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.407225 pylint-3.1.0/doc/whatsnew/1/1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.8/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.8/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12036 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.8/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.407225 pylint-3.1.0/doc/whatsnew/1/1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.9/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.9/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/1.9/summary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/1/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.407225 pylint-3.1.0/doc/whatsnew/2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.411225 pylint-3.1.0/doc/whatsnew/2/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11279 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.0/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.0/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.0/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.411225 pylint-3.1.0/doc/whatsnew/2/2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.1/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.1/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.1/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.411225 pylint-3.1.0/doc/whatsnew/2/2.10/
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.10/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.10/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.10/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.411225 pylint-3.1.0/doc/whatsnew/2/2.11/
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.11/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.11/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.11/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.411225 pylint-3.1.0/doc/whatsnew/2/2.12/
+-rw-r--r--   0 runner    (1001) docker     (127)    11903 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.12/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.12/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9948 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.12/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.411225 pylint-3.1.0/doc/whatsnew/2/2.13/
+-rw-r--r--   0 runner    (1001) docker     (127)    23824 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.13/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.13/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21678 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.13/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.411225 pylint-3.1.0/doc/whatsnew/2/2.14/
+-rw-r--r--   0 runner    (1001) docker     (127)    16106 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.14/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.14/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13178 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.14/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.411225 pylint-3.1.0/doc/whatsnew/2/2.15/
+-rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.15/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.411225 pylint-3.1.0/doc/whatsnew/2/2.16/
+-rw-r--r--   0 runner    (1001) docker     (127)    29895 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.16/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.411225 pylint-3.1.0/doc/whatsnew/2/2.17/
+-rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.17/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.415225 pylint-3.1.0/doc/whatsnew/2/2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.2/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.2/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.2/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.415225 pylint-3.1.0/doc/whatsnew/2/2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.3/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.3/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.3/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.415225 pylint-3.1.0/doc/whatsnew/2/2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11264 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.4/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.4/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6793 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.4/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.415225 pylint-3.1.0/doc/whatsnew/2/2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.5/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.5/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.5/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.415225 pylint-3.1.0/doc/whatsnew/2/2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.6/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.6/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.6/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.415225 pylint-3.1.0/doc/whatsnew/2/2.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.7/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.7/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.7/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.415225 pylint-3.1.0/doc/whatsnew/2/2.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.8/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.8/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.8/summary.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.415225 pylint-3.1.0/doc/whatsnew/2/2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     9850 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.9/full.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.9/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4752 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/2.9/summary.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/2/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.419225 pylint-3.1.0/doc/whatsnew/3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.419225 pylint-3.1.0/doc/whatsnew/3/3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    31655 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/3/3.0/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.419225 pylint-3.1.0/doc/whatsnew/3/3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/3/3.1/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/3/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.419225 pylint-3.1.0/doc/whatsnew/fragments/
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/fragments/_template.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/full_changelog_explanation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-25 16:48:03.000000 pylint-3.1.0/doc/whatsnew/summary_explanation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.419225 pylint-3.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-25 16:48:03.000000 pylint-3.1.0/examples/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-02-25 16:48:03.000000 pylint-3.1.0/examples/custom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-25 16:48:03.000000 pylint-3.1.0/examples/custom_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-02-25 16:48:03.000000 pylint-3.1.0/examples/deprecation_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21529 2024-02-25 16:48:03.000000 pylint-3.1.0/examples/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-25 16:48:03.000000 pylint-3.1.0/examples/pylintrc_camelcase
+-rw-r--r--   0 runner    (1001) docker     (127)    21193 2024-02-25 16:48:03.000000 pylint-3.1.0/examples/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.167224 pylint-3.1.0/pylint/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/__pkginfo__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.175224 pylint-3.1.0/pylint/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/bad_chained_comparison.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.175224 pylint-3.1.0/pylint/checkers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40429 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/base/basic_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22450 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/base/basic_error_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13874 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/base/comparison_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/base/docstring_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.175224 pylint-3.1.0/pylint/checkers/base/name_checker/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/base/name_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27539 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/base/name_checker/checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/base/name_checker/naming_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/base/pass_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/base_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.175224 pylint-3.1.0/pylint/checkers/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91151 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/classes/class_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15125 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/classes/special_methods_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/dataclass_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23346 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/design_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/dunder_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/ellipsis_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26430 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26794 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48856 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/lambda_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16368 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/method_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/modified_iterating_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/nested_min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/newstyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/non_ascii_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/raw_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.179224 pylint-3.1.0/pylint/checkers/refactoring/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/refactoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14375 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/refactoring/implicit_booleaness_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/refactoring/not_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18659 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/refactoring/recommendation_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)   100095 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/refactoring/refactoring_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33999 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/similar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16454 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/spelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35213 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44785 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/threading_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89543 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3010 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/unsupported_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77535 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   135050 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/checkers/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.179224 pylint-3.1.0/pylint/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/_breaking_changes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.183224 pylint-3.1.0/pylint/config/_pylint_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/_pylint_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/_pylint_config/generate_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/_pylint_config/help_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/_pylint_config/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/_pylint_config/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/_pylint_config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14816 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15085 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/arguments_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/arguments_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/callback_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4532 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/config_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/config_initialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/deprecation_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/find_default_config_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/help_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8774 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8736 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.187224 pylint-3.1.0/pylint/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29753 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/_check_docs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/bad_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/broad_try_clause.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/check_elif.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13688 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/code_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/comparison_placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/confusing_elif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/consider_refactoring_into_while_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/consider_ternary_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/dict_init_mutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25473 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/docparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/docstyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/dunder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/empty_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/eq_without_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/for_any_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/magic_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/mccabe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/no_self_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/overlapping_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11247 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/private_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/redefined_loop_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/redefined_variable_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/set_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20400 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/extensions/while_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/interfaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.187224 pylint-3.1.0/pylint/lint/
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21528 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/lint/base_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/lint/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6694 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/lint/expand_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17297 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/lint/message_state_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/lint/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50373 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/lint/pylinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/lint/report_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/lint/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/lint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.191224 pylint-3.1.0/pylint/message/
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7654 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/message/_deleted_message_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/message/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/message/message_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/message/message_definition_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/message/message_id_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.191224 pylint-3.1.0/pylint/pyreverse/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/diadefslib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11578 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/diagrams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/dot_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13476 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9640 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/mermaidjs_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/plantuml_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/printer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7579 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/pyreverse/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.195224 pylint-3.1.0/pylint/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/base_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/collecting_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/json_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/multi_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/reports_handler_mix_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8814 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/text.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.195224 pylint-3.1.0/pylint/reporters/ureports/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/ureports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/ureports/base_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/ureports/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/reporters/ureports/text_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.195224 pylint-3.1.0/pylint/testutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.199224 pylint-3.1.0/pylint/testutils/_primer/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/_primer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/_primer/package_to_lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/_primer/primer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/_primer/primer_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6989 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/_primer/primer_compare_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/_primer/primer_prepare_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/_primer/primer_run_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/checker_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1159 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.199224 pylint-3.1.0/pylint/testutils/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/functional/find_functional_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/functional/lint_module_output_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/functional/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/get_test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/global_test_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/lint_module_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/output_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4243 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/pyreverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/reporter_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/testing_pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/tokenize_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/unittest_linter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/testutils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.199224 pylint-3.1.0/pylint/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/utils/ast_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3406 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/utils/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9634 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/utils/file_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12440 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/utils/linterstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/utils/pragma_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12384 2024-02-25 16:48:03.000000 pylint-3.1.0/pylint/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.807227 pylint-3.1.0/pylint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-02-25 16:48:15.000000 pylint-3.1.0/pylint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)   192854 2024-02-25 16:48:16.000000 pylint-3.1.0/pylint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-25 16:48:15.000000 pylint-3.1.0/pylint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:15.000000 pylint-3.1.0/pylint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-02-25 16:48:15.000000 pylint-3.1.0/pylint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-25 16:48:15.000000 pylint-3.1.0/pylint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-02-25 16:48:03.000000 pylint-3.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.423225 pylint-3.1.0/script/
+-rw-r--r--   0 runner    (1001) docker     (127)    32986 2024-02-25 16:48:03.000000 pylint-3.1.0/script/.contributors_aliases.json
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-25 16:48:03.000000 pylint-3.1.0/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2024-02-25 16:48:03.000000 pylint-3.1.0/script/bump_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-02-25 16:48:03.000000 pylint-3.1.0/script/check_newsfragments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-25 16:48:03.000000 pylint-3.1.0/script/copyright.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-25 16:48:03.000000 pylint-3.1.0/script/create_contributor_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-02-25 16:48:03.000000 pylint-3.1.0/script/get_unused_message_id_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-25 16:48:16.811227 pylint-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.423225 pylint-3.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.423225 pylint-3.1.0/tests/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (127)    13917 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/benchmark/test_baseline_benchmarks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.427225 pylint-3.1.0/tests/checkers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.427225 pylint-3.1.0/tests/checkers/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/base/unittest_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/base/unittest_multi_naming_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4040 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/base/unittest_name_preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_base_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21855 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8867 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_non_ascii_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_refactoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13547 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_similar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21522 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_spelling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_typecheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.427225 pylint-3.1.0/tests/checkers/unittest_unicode/
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_unicode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9778 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_unicode/unittest_bad_chars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_unicode/unittest_bidirectional_unicode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_unicode/unittest_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_unicode/unittest_invalid_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12317 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6544 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/checkers/unittest_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.431225 pylint-3.1.0/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.431225 pylint-3.1.0/tests/config/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/data/logging_format_interpolation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/data/logging_format_interpolation_style.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/file_to_lint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.139224 pylint-3.1.0/tests/config/functional/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.431225 pylint-3.1.0/tests/config/functional/ini/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_deleted_message.8.out
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_deleted_message.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_deleted_message.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_interpolation_error.1.out
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_interpolation_error.ini
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_interpolation_error.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_message_control.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_message_control.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_missing_comma.4.out
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_missing_comma.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_missing_comma.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_multi_line_init_hook.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_quoted_init_hook.0.out
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/ini/pylintrc_with_quoted_init_hook.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.431225 pylint-3.1.0/tests/config/functional/setup_cfg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.431225 pylint-3.1.0/tests/config/functional/setup_cfg/do_not_read_other_tools_configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/do_not_read_other_tools_configuration/setup.4.out
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/do_not_read_other_tools_configuration/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/do_not_read_other_tools_configuration/setup.result.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.431225 pylint-3.1.0/tests/config/functional/setup_cfg/identical_name_in_flake8/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/identical_name_in_flake8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/identical_name_in_flake8/setup.result.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.435225 pylint-3.1.0/tests/config/functional/setup_cfg/issue_3630/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/issue_3630/not_setup.2.out
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/issue_3630/not_setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/issue_3630/not_setup.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/issue_3630/setup.2.out
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/issue_3630/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/issue_3630/setup.result.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.435225 pylint-3.1.0/tests/config/functional/setup_cfg/issue_4272/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/issue_4272/option_in_wrong_section.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/issue_4272/option_in_wrong_section.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/setup_cfg_with_message_control.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/setup_cfg/setup_cfg_with_message_control.result.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.435225 pylint-3.1.0/tests/config/functional/toml/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.435225 pylint-3.1.0/tests/config/functional/toml/issue_3122/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_3122/toml_with_missing_comma.4.out
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_3122/toml_with_missing_comma.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_3122/toml_with_missing_comma.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.435225 pylint-3.1.0/tests/config/functional/toml/issue_3181/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_3181/toml_decode_error.1.out
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_3181/toml_decode_error.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_3181/top_level_list_of_disable.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_3181/top_level_list_of_disable.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.439225 pylint-3.1.0/tests/config/functional/toml/issue_4580/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/correct_basic_name_group.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/correct_basic_name_group.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/correct_import_preferred_module.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/correct_import_preferred_module.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/rich_types.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/rich_types.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/top_level_disable.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/top_level_disable.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/valid_data_for_basic.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/valid_data_for_basic.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/valid_data_for_import.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4580/valid_data_for_import.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.439225 pylint-3.1.0/tests/config/functional/toml/issue_4746/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4746/loaded_plugin_does_not_exists.2.out
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4746/loaded_plugin_does_not_exists.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/issue_4746/loaded_plugin_does_not_exists.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/rich_types.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/rich_types.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_with_enable.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_with_enable.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_with_message_control.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_with_message_control.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_with_mutually_exclusive_disable_enable_all.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_with_specific_disable_before_enable_all.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_with_specific_enable_before_disable_all.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_with_unknown_option.2.out
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_with_unknown_option.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_with_unknown_option.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/toml_without_pylint.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.439225 pylint-3.1.0/tests/config/functional/toml/unknown_msgid/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/unknown_msgid/enable_unknown_msgid.4.out
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/unknown_msgid/enable_unknown_msgid.result.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/toml/unknown_msgid/enable_unknown_msgid.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.139224 pylint-3.1.0/tests/config/functional/tox/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.439225 pylint-3.1.0/tests/config/functional/tox/unrecognized_options/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/tox/unrecognized_options/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/functional/tox/unrecognized_options/tox.result.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.439225 pylint-3.1.0/tests/config/pylint_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/pylint_config/test_pylint_config_generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/pylint_config/test_pylint_config_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/pylint_config/test_pylint_config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/pylint_config/test_run_pylint_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/test_argparse_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11147 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/test_find_default_config_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/test_functional_config_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/config/test_per_directory_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.443225 pylint-3.1.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      194 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/data/ascript
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/data/clientmodule_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/data/empty_pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/data/nullable_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/data/property_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/data/suppliermodule_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.443225 pylint-3.1.0/tests/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/extensions/test_check_docs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/extensions/test_private_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.443225 pylint-3.1.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.447225 pylint-3.1.0/tests/functional/a/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.447225 pylint-3.1.0/tests/functional/a/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/abstract/abstract_abc_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/abstract/abstract_class_instantiated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/abstract/abstract_class_instantiated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/abstract/abstract_class_instantiated_in_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/abstract/abstract_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/abstract/abstract_method.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.447225 pylint-3.1.0/tests/functional/a/access/
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/access/access_attr_before_def_false_positive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/access/access_member_before_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/access/access_member_before_definition.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/access/access_to__name__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/access/access_to__name__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/access/access_to_protected_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3287 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/access/access_to_protected_members.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/access/access_to_protected_members_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.451225 pylint-3.1.0/tests/functional/a/alternative/
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/alternative/alternative_union_syntax.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/alternative/alternative_union_syntax.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/alternative/alternative_union_syntax_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/alternative/alternative_union_syntax_error.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/alternative/alternative_union_syntax_error.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/alternative/alternative_union_syntax_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/alternative/alternative_union_syntax_py37.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/alternative/alternative_union_syntax_py37.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/alternative/alternative_union_syntax_regession_8119.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/alternative/alternative_union_syntax_regession_8119.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/anomalous_backslash_escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/anomalous_backslash_escape.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/anomalous_unicode_escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/anomalous_unicode_escape.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/arguments.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/arguments.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8239 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/arguments_differ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/arguments_differ.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/arguments_differ_issue5371.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/arguments_out_of_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/arguments_out_of_order.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/arguments_renamed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/arguments_renamed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assert_on_string_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assert_on_string_literal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assert_on_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assert_on_tuple.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.451225 pylint-3.1.0/tests/functional/a/assigning/
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assigning/assigning_non_slot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assigning/assigning_non_slot.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assigning/assigning_non_slot_4509.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assigning/assigning_non_slot_4509.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.451225 pylint-3.1.0/tests/functional/a/assignment/
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assignment/assignment_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assignment/assignment_expression.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assignment/assignment_from_no_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assignment/assignment_from_no_return.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assignment/assignment_from_no_return_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assignment/assignment_from_no_return_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/assignment/assignment_from_no_return_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/async_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/async_functions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/attribute_defined_outside_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/attribute_defined_outside_init.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/attribute_defined_outside_init_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/attribute_defined_outside_init_py38.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/await_outside_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/a/await_outside_async.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.459225 pylint-3.1.0/tests/functional/b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_chained_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_chained_comparison.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.459225 pylint-3.1.0/tests/functional/b/bad_char/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_backspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_backspace.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_carriage_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_carriage_return.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_carriage_return.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_esc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_esc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_sub.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_zero_width_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_char/bad_char_zero_width_space.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_except_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_except_order.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_exception_cause.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_exception_cause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_indentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_indentation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_inline_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_inline_option.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_inline_option.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_open_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_open_mode.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_option_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_option_value.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_option_value_disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_option_value_disable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_reversed_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_reversed_sequence.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_reversed_sequence_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_reversed_sequence_py37.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_reversed_sequence_py37.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_reversed_sequence_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_staticmethod_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_staticmethod_argument.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_string_format_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_string_format_type.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_thread_instantiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bad_thread_instantiation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bare_except.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bare_except.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/base_init_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/boolean_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/boolean_datetime.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/boolean_datetime.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.463225 pylint-3.1.0/tests/functional/b/broad_exception/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_caught.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_caught.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_caught.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_caught_trystar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_caught_trystar.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_caught_trystar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_raised.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_raised.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_raised.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_raised_trystar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_raised_trystar.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/broad_exception/broad_exception_raised_trystar.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/bugfix_local_scope_metaclass_1177.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/b/builtin_module_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.467225 pylint-3.1.0/tests/functional/c/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/cached_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/cached_property.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/cell_var_from_loop_enabled_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/cell_var_from_loop_enabled_regression.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/cell_var_from_loop_enabled_regression.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5092 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/cellvar_escaping_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/cellvar_escaping_loop.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/class_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/class_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/class_members_py30.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/class_members_py30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/class_protocol_ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/class_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/class_scope.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/class_variable_slots_conflict_exempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/classes_meth_could_be_a_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/classes_protected_member_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/comparison_of_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/comparison_of_constants.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/comparison_with_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/comparison_with_callable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/comparison_with_callable_typing_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/condition_evals_to_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/condition_evals_to_constant.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/confidence_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/confidence_filter.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/confidence_filter.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/confusing_with_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/confusing_with_statement.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.475225 pylint-3.1.0/tests/functional/c/consider/
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_iterating_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_iterating_dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_join.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_join_for_non_empty_separator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_join_for_non_empty_separator.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_merging_isinstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_merging_isinstance.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_swap_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_swap_variables.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_dict_comprehension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_dict_comprehension.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_dict_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_dict_items.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_enumerate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_enumerate.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_f_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3420 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_f_string.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_generator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_get.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_in.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_in.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_min_max_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_min_max_builtin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_set_comprehension.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_set_comprehension.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_sys_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_sys_exit.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_sys_exit_exempted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_sys_exit_local_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6510 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_with.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_with.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_with_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/consider/consider_using_with_open.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/continue_in_finally.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/continue_in_finally.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/continue_in_finally.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/control_pragmas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/crash_missing_module_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/ctor_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/c/ctor_arguments.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.479225 pylint-3.1.0/tests/functional/d/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dangerous_default_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dangerous_default_value.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.479225 pylint-3.1.0/tests/functional/d/dataclass/
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_kw_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_kw_only.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_kw_only.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_parameter.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_typecheck.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_with_default_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_with_default_factory.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_with_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dataclass/dataclass_with_field.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/decorator_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/decorator_unused.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/defined_and_used_on_same_line.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.487225 pylint-3.1.0/tests/functional/d/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_attribute_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_attribute_py312.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_attribute_py312.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_class_py33.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_class_py33.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_class_py33.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_decorators.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_method_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py3.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py36.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py38.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_methods_py39.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py3.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py310.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py310.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py33.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py33.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py36.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py39.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py39_earlier_pyversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py39_earlier_pyversion.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py39_earlier_pyversion.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py4.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py4.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_py4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_redundant.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_redundant.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_redundant.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_uninstalled.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_uninstalled.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_module_uninstalled.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.487225 pylint-3.1.0/tests/functional/d/deprecated/deprecated_relative_import/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_relative_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_relative_import/dot_relative_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_relative_import/dot_relative_import.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.491226 pylint-3.1.0/tests/functional/d/deprecated/deprecated_relative_import/subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_relative_import/subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_relative_import/subpackage/dot_dot_relative_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/deprecated/deprecated_relative_import/subpackage/dot_dot_relative_import.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dict_iter_missing_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dict_iter_missing_items.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disable_msg_github_issue_1389.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disable_msg_next_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disable_msg_next_line.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disable_ungrouped_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disable_ungrouped_imports.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disable_wrong_import_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disable_wrong_import_order.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disable_wrong_import_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disabled_msgid_in_pylintrc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disabled_msgid_in_pylintrc.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disallowed_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/disallowed_name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/docstrings.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dotted_ancestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/dotted_ancestor.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.491226 pylint-3.1.0/tests/functional/d/duplicate/
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_argument_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_argument_name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_argument_name_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_argument_name_py3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_bases.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_dict_literal_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_dict_literal_key.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_except.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_except.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_string_formatting_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_string_formatting_argument.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/d/duplicate/duplicate_value.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.495226 pylint-3.1.0/tests/functional/e/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/.#emacs_file_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/.#emacs_file_lock_by_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/.#emacs_file_lock_by_conf.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/.#emacs_file_lock_redefined_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/.#emacs_file_lock_redefined_conf.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/.#emacs_file_lock_redefined_conf.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/e1101_9588_base_attr_aug_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/empty_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/empty_docstring.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/enum_self_defined_member_5138.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/enum_self_defined_member_5138.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/enum_self_defined_member_6805.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/enum_self_defined_member_6805.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/enum_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/eval_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/eval_used.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/exception_is_binary_op.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/exception_is_binary_op.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/excess_escapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/excess_escapes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/exec_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/exec_used.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/e/external_classmethod_crash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.499225 pylint-3.1.0/tests/functional/ext/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.499225 pylint-3.1.0/tests/functional/ext/bad_builtin/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/bad_builtin/bad_builtin_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/bad_builtin/bad_builtin_extension.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/bad_builtin/bad_builtin_extension.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/bad_builtin/bad_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/bad_builtin/bad_builtins.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/bad_builtin/bad_builtins.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.499225 pylint-3.1.0/tests/functional/ext/bad_dunder/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/bad_dunder/bad_dunder_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/bad_dunder/bad_dunder_name.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/bad_dunder/bad_dunder_name.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.499225 pylint-3.1.0/tests/functional/ext/broad_try_clause/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/broad_try_clause/broad_try_clause_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/broad_try_clause/broad_try_clause_extension.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/broad_try_clause/broad_try_clause_extension.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.499225 pylint-3.1.0/tests/functional/ext/check_elif/
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/check_elif/check_elif.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/check_elif/check_elif.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/check_elif/check_elif.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.503225 pylint-3.1.0/tests/functional/ext/code_style/
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_assignment_expr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_assignment_expr.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_assignment_expr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_augmented_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_augmented_assign.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_augmented_assign.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_namedtuple_or_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_namedtuple_or_dataclass.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_namedtuple_or_dataclass.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_tuple.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_consider_using_tuple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_default.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_prefer_typing_namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_prefer_typing_namedtuple.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_prefer_typing_namedtuple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_py_version_35.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/code_style/cs_py_version_35.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.503225 pylint-3.1.0/tests/functional/ext/comparison_placement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/comparison_placement/misplaced_comparison_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/comparison_placement/misplaced_comparison_constant.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/comparison_placement/misplaced_comparison_constant.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.503225 pylint-3.1.0/tests/functional/ext/confusing_elif/
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/confusing_elif/confusing_elif.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/confusing_elif/confusing_elif.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/confusing_elif/confusing_elif.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.507226 pylint-3.1.0/tests/functional/ext/consider_refactoring_into_while_condition/
+-rw-r--r--   0 runner    (1001) docker     (127)     9292 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/consider_refactoring_into_while_condition/consider_refactoring_into_while_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/consider_refactoring_into_while_condition/consider_refactoring_into_while_condition.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     4896 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/consider_refactoring_into_while_condition/consider_refactoring_into_while_condition.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/consider_refactoring_into_while_condition/consider_refactoring_into_while_condition_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/consider_refactoring_into_while_condition/consider_refactoring_into_while_condition_py38.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/consider_refactoring_into_while_condition/consider_refactoring_into_while_condition_py38.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.507226 pylint-3.1.0/tests/functional/ext/consider_ternary_expression/
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/consider_ternary_expression/consider_ternary_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/consider_ternary_expression/consider_ternary_expression.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/consider_ternary_expression/consider_ternary_expression.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/dict_init_mutate.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/dict_init_mutate.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/dict_init_mutate.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.507226 pylint-3.1.0/tests/functional/ext/docparams/
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/docparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/docparams.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/docparams.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/docparams_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/docparams_py38.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/docparams_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/missing_param_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/missing_param_doc.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/missing_param_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/missing_param_doc_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/missing_param_doc_py38.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.511226 pylint-3.1.0/tests/functional/ext/docparams/parameter/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11669 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_Google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_Google.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_Google.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9310 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_Numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_Numpy.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_Numpy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_Sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_Sphinx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_Sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_min_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_min_length.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_no_doc_rgx_check_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_no_doc_rgx_check_init.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_no_doc_rgx_check_init.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_no_doc_rgx_check_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_no_doc_rgx_check_none.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_no_doc_rgx_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_no_doc_rgx_default.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_no_doc_rgx_test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_no_doc_rgx_test_all.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/parameter/missing_param_doc_required_no_doc_rgx_test_all.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.515226 pylint-3.1.0/tests/functional/ext/docparams/raise/
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4431 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_Google.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_Google.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_Google.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_Numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_Numpy.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_Numpy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_Sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_Sphinx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_Sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_options.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required_Google.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required_Google.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required_Numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required_Numpy.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required_Sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required_Sphinx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required_exc_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required_exc_inheritance.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/raise/missing_raises_doc_required_exc_inheritance.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.523226 pylint-3.1.0/tests/functional/ext/docparams/return/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_Google.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_Google.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_Google.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_Numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_Numpy.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_Numpy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_Sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_Sphinx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_Sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required_Google.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required_Google.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required_Google.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required_Numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required_Numpy.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required_Numpy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required_Sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required_Sphinx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/return/missing_return_doc_required_Sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/useless_type_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/useless_type_doc.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/useless_type_doc.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.527226 pylint-3.1.0/tests/functional/ext/docparams/yield/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_Google.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_Google.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_Google.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_Numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_Numpy.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_Numpy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_Sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_Sphinx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required_Google.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required_Google.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required_Google.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required_Numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required_Numpy.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required_Numpy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required_Sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required_Sphinx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docparams/yield/missing_yield_doc_required_Sphinx.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.527226 pylint-3.1.0/tests/functional/ext/docstyle/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docstyle/docstyle_first_line_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docstyle/docstyle_first_line_empty.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docstyle/docstyle_first_line_empty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docstyle/docstyle_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docstyle/docstyle_quotes.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/docstyle/docstyle_quotes.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.527226 pylint-3.1.0/tests/functional/ext/empty_comment/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/empty_comment/empty_comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/empty_comment/empty_comment.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/empty_comment/empty_comment.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.527226 pylint-3.1.0/tests/functional/ext/eq_without_hash/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/eq_without_hash/eq_without_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/eq_without_hash/eq_without_hash.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/eq_without_hash/eq_without_hash.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.527226 pylint-3.1.0/tests/functional/ext/for_any_all/
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/for_any_all/for_any_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/for_any_all/for_any_all.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/for_any_all/for_any_all.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.527226 pylint-3.1.0/tests/functional/ext/magic_value_comparison/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/magic_value_comparison/magic_value_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/magic_value_comparison/magic_value_comparison.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/magic_value_comparison/magic_value_comparison.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.531226 pylint-3.1.0/tests/functional/ext/mccabe/
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/mccabe/mccabe.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/mccabe/mccabe.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/mccabe/mccabe.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.531226 pylint-3.1.0/tests/functional/ext/no_self_use/
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/no_self_use/no_self_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/no_self_use/no_self_use.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/no_self_use/no_self_use.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.531226 pylint-3.1.0/tests/functional/ext/overlapping_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/overlapping_exceptions/overlapping_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/overlapping_exceptions/overlapping_exceptions.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/overlapping_exceptions/overlapping_exceptions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/plugin_does_not_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/plugin_does_not_exists.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/plugin_does_not_exists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.531226 pylint-3.1.0/tests/functional/ext/private_import/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/private_import/private_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/private_import/private_import.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/private_import/private_import.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.531226 pylint-3.1.0/tests/functional/ext/redefined_loop_name/
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_loop_name/redefined_loop_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_loop_name/redefined_loop_name.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_loop_name/redefined_loop_name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_loop_name/reused_outer_loop_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_loop_name/reused_outer_loop_variable.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_loop_name/reused_outer_loop_variable.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.531226 pylint-3.1.0/tests/functional/ext/redefined_variable_type/
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_variable_type/redefined_variable_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_variable_type/redefined_variable_type.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_variable_type/redefined_variable_type.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_variable_type/regression_newtype_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/redefined_variable_type/regression_newtype_fstring.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.535226 pylint-3.1.0/tests/functional/ext/set_membership/
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/set_membership/use_set_membership.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/set_membership/use_set_membership.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/set_membership/use_set_membership.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.539226 pylint-3.1.0/tests/functional/ext/typing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/redundant_typehint_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/redundant_typehint_argument.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/redundant_typehint_argument.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/redundant_typehint_argument_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/redundant_typehint_argument_py310.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/redundant_typehint_argument_py310.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_callable.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_callable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_callable_deprecated_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_callable_deprecated_alias.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_callable_future_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_callable_future_import.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_callable_future_import.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_noreturn.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_noreturn.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_noreturn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_noreturn_future_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_noreturn_future_import.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_noreturn_future_import.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_noreturn_py372.py
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_broken_noreturn_py372.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_alias.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_alias.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_alias_without_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_alias_without_future.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     3496 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_alias_without_future.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_union.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_union.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_union_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_union_py310.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_union_py310.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_union_without_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_union_without_future.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_consider_using_union_without_future.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_deprecated_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_deprecated_alias.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/typing/typing_deprecated_alias.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.539226 pylint-3.1.0/tests/functional/ext/while_used/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/while_used/while_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/while_used/while_used.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/ext/while_used/while_used.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.547226 pylint-3.1.0/tests/functional/f/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/f_string_without_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/f_string_without_interpolation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/fallback_import_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/fallback_import_enabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/fallback_import_enabled.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/fallback_import_enabled.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/first_arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/first_arg.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/fixme.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/fixme.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/fixme.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/fixme_bad_formatting_1139.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/fixme_bad_formatting_1139.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/fixme_bad_formatting_1139.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/forgotten_debug_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/forgotten_debug_statement.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/formatted_string_literal_with_if.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/func_disable_linebased.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/func_disable_linebased.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/function_redefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/function_redefined.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/function_redefined_2540.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/future_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/future_unicode_literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/future_unicode_literals.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/f/future_unicode_literals.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.547226 pylint-3.1.0/tests/functional/g/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generated_members.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generated_members.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generated_members.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.551226 pylint-3.1.0/tests/functional/g/generic_alias/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_collections.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_collections.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5175 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_collections_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_collections_py37.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_collections_py37.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_collections_py37_with_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_collections_py37_with_typing.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     6738 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_collections_py37_with_typing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_mixed_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_mixed_py37.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_mixed_py37.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_mixed_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_mixed_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_mixed_py39.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_postponed_evaluation_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_postponed_evaluation_py37.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_postponed_evaluation_py37.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_related.py
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_related.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_related_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_related_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_related_py39.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_side_effects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_side_effects.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/generic_alias/generic_alias_typing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/genexp_in_class_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/genexpr_variable_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/genexpr_variable_scope.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/g/globals.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.559226 pylint-3.1.0/tests/functional/i/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.559226 pylint-3.1.0/tests/functional/i/implicit/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/implicit/implicit_flag_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/implicit/implicit_flag_alias.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/implicit/implicit_str_concat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/implicit/implicit_str_concat.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/implicit/implicit_str_concat_latin1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/implicit/implicit_str_concat_latin1.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1732 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/implicit/implicit_str_concat_multiline.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       57 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/implicit/implicit_str_concat_multiline.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/implicit/implicit_str_concat_multiline.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/implicit/implicit_str_concat_utf8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_aliasing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_aliasing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_error.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_error.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_itself.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_itself.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_outside_toplevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_outside_toplevel.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/import_outside_toplevel.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.563226 pylint-3.1.0/tests/functional/i/inconsistent/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_mro.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_mro.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes2.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes_fstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes_fstring.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes_fstring_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes_fstring_py312.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes_fstring_py312.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes_fstring_py312_311.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_quotes_fstring_py312_311.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_returns.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_returns.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_returns_noreturn.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_returns_noreturn.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inconsistent/inconsistent_returns_noreturn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inference_crash_4692.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inference_crash_4692.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inherit_non_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inherit_non_class.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/init_is_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/init_is_generator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/init_not_called.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/init_not_called.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/init_return_from_inner_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/init_subclass_classmethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/inner_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.571226 pylint-3.1.0/tests/functional/i/invalid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.571226 pylint-3.1.0/tests/functional/i/invalid/invalid_all/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_all/invalid_all_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_all/invalid_all_format.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_all/invalid_all_format_valid_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_all/invalid_all_format_valid_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_all/invalid_all_format_valid_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_all/invalid_all_format_valid_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_all/invalid_all_format_valid_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_all/invalid_all_format_valid_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_all/invalid_all_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_all/invalid_all_object.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_bool_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_bool_returned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_bytes_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_bytes_returned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_class_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_class_object.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_enum_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_enum_extension.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_envvar_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_envvar_value.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.571226 pylint-3.1.0/tests/functional/i/invalid/invalid_exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_exceptions/invalid_exceptions_caught.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_exceptions/invalid_exceptions_caught.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_exceptions/invalid_exceptions_caught.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2996 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_exceptions/invalid_exceptions_raised.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_exceptions/invalid_exceptions_raised.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_field_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_field_call.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_format_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_format_returned.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.571226 pylint-3.1.0/tests/functional/i/invalid/invalid_getnewargs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_getnewargs/invalid_getnewargs_ex_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_getnewargs/invalid_getnewargs_ex_returned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_getnewargs/invalid_getnewargs_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_getnewargs/invalid_getnewargs_returned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_hash_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_hash_returned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_index_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_index_returned.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.571226 pylint-3.1.0/tests/functional/i/invalid/invalid_length/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_length/invalid_length_hint_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_length/invalid_length_hint_returned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_length/invalid_length_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_length/invalid_length_returned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_metaclass.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_metaclass_py3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.575226 pylint-3.1.0/tests/functional/i/invalid/invalid_name/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name-module-disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_enum.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_issue_3405.py
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_issue_3405.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_issue_3405.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_module_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_module_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_multinaming_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_multinaming_style.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_multinaming_style.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_property.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name/invalid_name_property.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_overridden_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_overridden_method.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_repr_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_repr_returned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_sequence_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_sequence_index.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_slice_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_slice_index.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_star_assignment_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_star_assignment_target.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_str_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_str_returned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_unary_operand_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/invalid/invalid_unary_operand_type.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/isinstance_second_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/isinstance_second_argument.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/isinstance_second_argument_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/isinstance_second_argument_py310.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/isinstance_second_argument_py310.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/iterable_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/iterable_context.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/iterable_context_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/iterable_context_asyncio.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/iterable_context_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/iterable_context_py3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/iterable_context_py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/i/iterable_context_py36.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.575226 pylint-3.1.0/tests/functional/k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/k/keyword_arg_before_vararg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/k/keyword_arg_before_vararg.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/k/keyword_arg_before_vararg_positional_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/k/keyword_arg_before_vararg_positional_only.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/k/kwarg_superseded_by_positional_arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/k/kwarg_superseded_by_positional_arg.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.579226 pylint-3.1.0/tests/functional/l/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/lambda_use_before_assign.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.579226 pylint-3.1.0/tests/functional/l/line/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/line/line_endings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/line/line_endings.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/line/line_endings.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/line/line_too_long.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/line/line_too_long.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/line/line_too_long_end_of_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/line/line_too_long_with_utf8.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/line/line_too_long_with_utf8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/line/line_too_long_with_utf8_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/literal_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/literal_comparison.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.583226 pylint-3.1.0/tests/functional/l/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_format_interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_format_interpolation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_format_interpolation_py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_format_interpolation_py36.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_format_interpolation_py36.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_format_interpolation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_format_interpolation_style.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_fstring_interpolation_py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_fstring_interpolation_py36.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_fstring_interpolation_py36.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_fstring_interpolation_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_fstring_interpolation_py37.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_fstring_interpolation_py37.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_not_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_not_lazy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_not_lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_not_lazy_module.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_not_lazy_module.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_not_lazy_with_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_not_lazy_with_logger.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_not_lazy_with_logger.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_too_few_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_too_few_args.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_too_few_args.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_too_many_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_too_many_args.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logging/logging_too_many_args.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logical_tautology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1660 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/logical_tautology.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/loopvar_in_dict_comp.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/loopvar_in_dict_comp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/lost_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/l/lost_exception.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.591226 pylint-3.1.0/tests/functional/m/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/mapping_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/mapping_context.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/mapping_context_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/mapping_context_py3.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.595226 pylint-3.1.0/tests/functional/m/member/
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_async.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_hints.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_hints.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_hints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_ignore_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_ignore_none.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_ignore_none.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_inference_improvements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_no_hints.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_no_hints.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_no_hints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_opaque.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_opaque.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_opaque.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_typed_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/member/member_checks_typed_annotations.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/membership_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/membership_protocol.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/membership_protocol_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/membership_protocol_py3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/metaclass_attr_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/method_cache_max_size_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/method_cache_max_size_none.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/method_cache_max_size_none_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/method_cache_max_size_none_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/method_cache_max_size_none_py39.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/method_hidden.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/method_hidden.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/method_hidden_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/method_hidden_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/misplaced_bare_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/misplaced_bare_raise.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/misplaced_format_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/misplaced_format_function.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/misplaced_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/misplaced_future.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.599226 pylint-3.1.0/tests/functional/m/missing/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_class_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_class_docstring.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_docstring.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_docstring_new_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_docstring_new_style.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_final_newline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_final_newline.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_function_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_function_docstring.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_function_docstring.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_function_docstring_min_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_function_docstring_min_length.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_function_docstring_min_length.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_function_docstring_rgx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_function_docstring_rgx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_function_docstring_rgx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_kwoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_kwoa.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_module_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_module_docstring.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_module_docstring_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_module_docstring_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_parentheses_for_call_in_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_parentheses_for_call_in_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_self_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_self_argument.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/missing/missing_timeout.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/mixin_class_rgx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/mixin_class_rgx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/mixin_class_rgx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4042 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/modified_iterating.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/modified_iterating.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/module___dict__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/module___dict__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/monkeypatch_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/multiple_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/multiple_imports.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/multiple_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/multiple_statements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/multiple_statements_single_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/multiple_statements_single_line.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/m/multiple_statements_single_line.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.607226 pylint-3.1.0/tests/functional/n/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.607226 pylint-3.1.0/tests/functional/n/name/
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_final.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_final.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_final_snake_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_final_snake_case.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_final_snake_case.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_good_bad_names_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_good_bad_names_regex.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_good_bad_names_regex.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_preset_snake_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_preset_snake_case.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_preset_snake_case.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_styles.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/name/name_styles.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/namePresetCamelCase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/namePresetCamelCase.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/namePresetCamelCase.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/named_expr_without_context_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/named_expr_without_context_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/namedtuple_member_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/namedtuple_member_inference.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/names_in__all__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/names_in__all__.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nan_comparison_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nan_comparison_check.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nested_blocks_issue1088.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nested_blocks_issue1088.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nested_func_defined_in_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nested_func_defined_in_loop.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nested_min_max.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nested_min_max.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nested_min_max_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nested_min_max_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nested_min_max_py39.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/new_style_class_py_30.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/new_style_class_py_30.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.615226 pylint-3.1.0/tests/functional/n/no/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_classmethod_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_classmethod_decorator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_dummy_redefined.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_dummy_redefined.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_else_break.py
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_else_break.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_else_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_else_continue.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_else_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_else_raise.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_else_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_else_return.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_assign_same_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_assign_same_line.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_augassign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_augassign.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_binary_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_dataclasses.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_if_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_if_statements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_imports.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_imports.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_nested_namedtuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_nested_namedtuple.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_subclassed_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_member_typevar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_method_argument_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_name_in_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_name_in_module.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_name_in_module.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_self_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_self_argument.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_staticmethod_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_staticmethod_decorator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/no/no_warning_docstring.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.619226 pylint-3.1.0/tests/functional/n/non/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_ascii_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_ascii_name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_ascii_name_backward_test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_ascii_name_backward_test_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_init_parent_called.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_init_parent_called.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_iterator_returned.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_iterator_returned.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_parent_init_called.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_str_assignment_to_dunder_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non/non_str_assignment_to_dunder_name.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.619226 pylint-3.1.0/tests/functional/n/non_ascii_import/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_import/non_ascii_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_import/non_ascii_import_as_bad.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_import/non_ascii_import_as_bad.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_import/non_ascii_import_as_okay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_import/non_ascii_import_from_as.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_import/non_ascii_import_from_as.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.623226 pylint-3.1.0/tests/functional/n/non_ascii_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_assignment_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_assignment_expressions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_decorator.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_decorator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_dict_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_for_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_for_loop.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_function.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_function_argument_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_function_argument_py38.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_function_argument_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_function_argument_py39plus.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_function_argument_py39plus.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_function_argument_py39plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_inline_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_inline_var.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_kwargs_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_kwargs_py38.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_kwargs_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_kwargs_py39plus.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_kwargs_py39plus.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_kwargs_py39plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_local.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_loł.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_loł.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_pos_and_kwonly_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_pos_and_kwonly_function.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_staticmethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_staticmethod.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_try_except.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_try_except.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name/non_ascii_name_variable.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.627226 pylint-3.1.0/tests/functional/n/non_ascii_name_class/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name_class/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name_class/non_ascii_name_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name_class/non_ascii_name_class.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name_class/non_ascii_name_class_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name_class/non_ascii_name_class_attribute.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name_class/non_ascii_name_class_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name_class/non_ascii_name_class_constant.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name_class/non_ascii_name_class_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/non_ascii_name_class/non_ascii_name_class_method.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/none_dunder_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/none_dunder_protocols.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/none_dunder_protocols_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/none_dunder_protocols_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nonexistent_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nonexistent_operator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nonlocal_and_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nonlocal_and_global.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nonlocal_without_binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/nonlocal_without_binding.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/not_async_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/not_async_context_manager.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/not_async_context_manager_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/not_callable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/not_callable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/not_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/not_context_manager.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/not_in_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/n/not_in_loop.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.627226 pylint-3.1.0/tests/functional/o/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/o/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/o/object_as_class_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/o/overloaded_operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/o/overridden_final_method_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/o/overridden_final_method_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/o/overridden_final_method_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/o/overridden_final_method_regression.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.631226 pylint-3.1.0/tests/functional/p/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/pattern_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/pattern_matching.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/positional_only_arguments_expected.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/positional_only_arguments_expected.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.635226 pylint-3.1.0/tests/functional/p/postponed/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_activated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_activated_with_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_not_activated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_not_activated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_pep585.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_pep585.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_pep585.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4131 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_pep585_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_pep585_error.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_pep585_error.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_pep585_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_pep585_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/postponed/postponed_evaluation_pep585_py39.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/potential_index_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/potential_index_error.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/pragma_after_backslash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/preferred_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/preferred_module.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/preferred_module.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/property_affectation_py26.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/property_with_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/property_with_parameters.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access_access_different_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access_access_different_scopes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access_special_methods_off.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access_special_methods_off.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access_special_methods_off.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access_special_methods_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access_special_methods_on.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protected_access_special_methods_on.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protocol_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protocol_classes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protocol_classes_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/protocol_classes_abstract.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/py_version_35.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/p/py_version_35.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.639226 pylint-3.1.0/tests/functional/r/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/raise_missing_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/raise_missing_from.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.639226 pylint-3.1.0/tests/functional/r/raising/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/raising/raising_bad_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/raising/raising_bad_type.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/raising/raising_format_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/raising/raising_format_tuple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/raising/raising_non_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/raising/raising_non_exception.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/raising/raising_self.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.643226 pylint-3.1.0/tests/functional/r/recursion/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_2667.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_2836.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_2861.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_2899.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_2906.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_3152.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_3159.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_940.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_crash_2683.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_error_crash_astroid_623.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/recursion/recursion_regression_2960.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redeclared_assigned_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redeclared_assigned_name.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redeclared_assigned_name.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefine_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.643226 pylint-3.1.0/tests/functional/r/redefined/
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_argument_from_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_argument_from_local.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_builtin.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_builtin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_builtin_allowed.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_builtin_allowed.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_builtin_allowed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_except_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_except_handler.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_outer_name_type_checking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redefined/redefined_slots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redundant_u_string_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redundant_u_string_prefix.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redundant_unittest_assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/redundant_unittest_assert.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.651226 pylint-3.1.0/tests/functional/r/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_1326_crash_uninferable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_2306_enum_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_2443_duplicate_bases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_2913.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_2937_ifexp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_3091.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_3231_no_member_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_3416_unused_argument_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_3416_unused_argument_raise.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_3507_typing_alias_isinstance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_3535_double_enum_inherit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_3595_notcallable_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4083_sequence_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4221_object_instanceattr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4358_unsubscriptable_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4439.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4439.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4439.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4612_crash_pytest_fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4680.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4680.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4688_duplicated_bases_member_hints.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4688_duplicated_bases_member_hints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4723.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4723.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_4891.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_6531_crash_index_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_9074_refactor_loop_with_unary_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_9074_refactor_loop_with_unary_variable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression___file___global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression___file___global.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_implicit_none_with_no_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_implicit_none_with_no_return.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_infer_call_result_3690.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_infer_call_result_3690.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_issue_4631.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_issue_4631.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_issue_4633.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_no_member_1078.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_no_value_for_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_posonly_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_properties_in_class_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_properties_in_class_context.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_property_no_member_2641.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_property_no_member_3269.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_property_no_member_844.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression/regression_property_no_member_870.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.659226 pylint-3.1.0/tests/functional/r/regression_02/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_2567.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_2964.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_3866.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_3976.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_3979.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_4660.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_4660.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_4982.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_5030.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_5048.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_5244.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_5408.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_5408.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_5461.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_5479.py
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_5479.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_5776.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_5801.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_8067.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_8067.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_8109.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_8207.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_distutil_import_error_73.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_distutil_import_error_73.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_distutil_import_error_73.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_enum_1734.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_no_member_7631.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_node_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_node_statement_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_property_slots_2439.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_protected_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_protected_access.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/regression_02/regression_too_many_arguments_2335.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/reimport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/reimport.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/reimported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/reimported.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/renamed_import_logging_not_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/renamed_import_logging_not_lazy.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/renamed_import_logging_not_lazy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/repeated_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/repeated_keyword.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/return_in_finally.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/return_in_finally.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/return_in_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/return_in_init.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/return_outside_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/r/return_outside_function.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.663226 pylint-3.1.0/tests/functional/s/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.667226 pylint-3.1.0/tests/functional/s/self/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/self/self_assigning_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/self/self_assigning_variable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/self/self_cls_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/self/self_cls_assignment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/shadowed_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/shadowed_import.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/shallow_copy_environ.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/shallow_copy_environ.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/signature_differs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/signature_differs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.667226 pylint-3.1.0/tests/functional/s/simplifiable/
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/simplifiable/simplifiable_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/simplifiable/simplifiable_condition.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/simplifiable/simplifiable_if_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/simplifiable/simplifiable_if_expression.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4024 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/simplifiable/simplifiable_if_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/simplifiable/simplifiable_if_statement.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/simplify_chained_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/simplify_chained_comparison.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.667226 pylint-3.1.0/tests/functional/s/singledispatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singledispatch/singledispatch_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singledispatch/singledispatch_functions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singledispatch/singledispatch_method.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singledispatch/singledispatch_method_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singledispatch/singledispatch_method_py37.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singledispatch/singledispatch_method_py37.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singledispatch/singledispatch_method_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singledispatch/singledispatch_method_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singledispatch/singledispatchmethod_function_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singledispatch/singledispatchmethod_function_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singleton_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/singleton_comparison.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/slots_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/slots_checks.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/socketerror_import.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.667226 pylint-3.1.0/tests/functional/s/star/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/star/star_needs_assignment_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/star/star_needs_assignment_target.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/star/star_needs_assignment_target_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/star/star_needs_assignment_target_py38.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/star/star_needs_assignment_target_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2935 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/statement_without_effect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/statement_without_effect.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/statement_without_effect_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/statement_without_effect_py312.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/statement_without_effect_py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/statement_without_effect_py36.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/stop_iteration_inside_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/stop_iteration_inside_generator.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.671226 pylint-3.1.0/tests/functional/s/string/
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4986 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting_disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting_disable.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting_disable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting_error.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting_failed_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting_failed_inference_py35.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_formatting_py3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_log_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/string/string_log_formatting.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/subclassed_final_class_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/subclassed_final_class_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/subprocess_popen_preexec_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/subprocess_popen_preexec_fn.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/subprocess_run_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/subprocess_run_check.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.675226 pylint-3.1.0/tests/functional/s/super/
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_checks.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_init_not_called.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_init_not_called.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_init_not_called.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_init_not_called_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_init_not_called_extensions.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_init_not_called_extensions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_init_not_called_extensions_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_init_not_called_extensions_py310.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_init_not_called_extensions_py310.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_init_not_called_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_with_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_with_arguments.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_with_arguments.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_without_brackets.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/super/super_without_brackets.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/superfluous_parens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/superfluous_parens.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/superfluous_parens_walrus_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/superfluous_parens_walrus_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/suspicious_str_strip_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/suspicious_str_strip_call.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.147224 pylint-3.1.0/tests/functional/s/symlink/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.675226 pylint-3.1.0/tests/functional/s/symlink/_binding/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/symlink/_binding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/symlink/_binding/symlink_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.675226 pylint-3.1.0/tests/functional/s/symlink/symlink_module/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/symlink/symlink_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/symlink/symlink_module/symlink_module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.675226 pylint-3.1.0/tests/functional/s/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/syntax/syntax_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/syntax/syntax_error.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/syntax/syntax_error.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/syntax/syntax_error_jython.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/syntax/syntax_error_jython.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/syntax/syntax_error_jython.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/sys_stream_regression_1004.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/s/sys_stream_regression_1004.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.679226 pylint-3.1.0/tests/functional/t/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/ternary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/tokenize_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/tokenize_error.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/tokenize_error.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/tokenize_error_jython.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/tokenize_error_jython.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/tokenize_error_jython.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/tokenize_error_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/tokenize_error_py312.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/tokenize_error_py312.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.687226 pylint-3.1.0/tests/functional/t/too/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_few_public_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_few_public_methods.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_few_public_methods_37.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_few_public_methods_excluded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_few_public_methods_excluded.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_few_public_methods_excluded.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_ancestors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_ancestors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_ancestors_ignored_parents.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_ancestors_ignored_parents.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_ancestors_ignored_parents.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_arguments.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_arguments_issue_1045.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_arguments_overload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_boolean_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_boolean_expressions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_branches.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_function_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_instance_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_instance_attributes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_instance_attributes_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_lines.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_lines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_lines_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2177 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_locals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_locals.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_nested_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_nested_blocks.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_public_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_public_methods.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_return_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_return_statements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_star_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_star_expressions.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_statements.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_statements.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/too/too_many_statements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/trailing_comma_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/trailing_comma_tuple.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/trailing_newlines.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/trailing_newlines.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/trailing_whitespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/trailing_whitespaces.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/try_except_raise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/try_except_raise.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/try_except_raise_crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/try_except_raise_crash.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/try_except_raise_crash.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.691226 pylint-3.1.0/tests/functional/t/type/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typealias_naming_style_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typealias_naming_style_default.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typealias_naming_style_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typealias_naming_style_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typealias_naming_style_py312.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typealias_naming_style_py312.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typealias_naming_style_rgx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typealias_naming_style_rgx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typealias_naming_style_rgx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_double_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_double_variance.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_name_incorrect_variance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_name_incorrect_variance.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_name_mismatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_name_mismatch.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_naming_style_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_naming_style_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_naming_style_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_naming_style_py312.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_naming_style_py312.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_naming_style_rgx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_naming_style_rgx.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/type/typevar_naming_style_rgx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/typing_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/typing_use.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/t/typing_use.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.699226 pylint-3.1.0/tests/functional/u/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.699226 pylint-3.1.0/tests/functional/u/unbalanced/
+-rw-r--r--   0 runner    (1001) docker     (127)     3464 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unbalanced/unbalanced_dict_unpacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unbalanced/unbalanced_dict_unpacking.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unbalanced/unbalanced_tuple_unpacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unbalanced/unbalanced_tuple_unpacking.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unbalanced/unbalanced_tuple_unpacking_py30.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.703226 pylint-3.1.0/tests/functional/u/undefined/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_all_variable_edge_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_all_variable_edge_case.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_loop_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_loop_variable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_loop_variable_py311.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_loop_variable_py311.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_loop_variable_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8942 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_crash_on_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_py30.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_py30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_py312.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/undefined/undefined_variable_typing.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unexpected_keyword_arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unexpected_keyword_arg.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unexpected_special_method_signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unexpected_special_method_signature.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/ungrouped_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/ungrouped_imports.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/ungrouped_imports_isort_compatible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/ungrouped_imports_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/ungrouped_imports_suppression.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/ungrouped_imports_suppression.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unhashable_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unhashable_member.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unhashable_member_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unhashable_member_py312.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.703226 pylint-3.1.0/tests/functional/u/unicode/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unicode/unicode_bidi_commenting_out.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unicode/unicode_bidi_commenting_out.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unicode/unicode_bidi_early_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unicode/unicode_bidi_early_return.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unicode/unicode_bidi_pep672.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unicode/unicode_bidi_pep672.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unidiomatic_typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unidiomatic_typecheck.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/uninferable_all_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unknown_encoding_jython.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unknown_encoding_jython.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unknown_encoding_jython.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.707226 pylint-3.1.0/tests/functional/u/unnecessary/
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_comprehension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_comprehension.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dict_index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dict_index_lookup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_direct_lambda_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_direct_lambda_call.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_direct_lambda_call.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_async_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_async_py310.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_async_py310.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_async_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_async_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_py38.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_py38_pypy.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_py38_pypy.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_py38_pypy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_dunder_call_py39.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_ellipsis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_ellipsis.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_lambda.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_lambda_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_lambda_assignment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_list_index_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_list_index_lookup.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_negation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_negation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unnecessary/unnecessary_pass.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.707226 pylint-3.1.0/tests/functional/u/unpacking/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unpacking/unpacking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unpacking/unpacking_generalizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unpacking/unpacking_generalizations.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unpacking/unpacking_non_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unpacking/unpacking_non_sequence.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unpacking/unpacking_non_sequence_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unpacking/unpacking_non_sequence_py310.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unpacking/unpacking_non_sequence_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unreachable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unreachable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unrecognized_inline_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unrecognized_inline_option.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5823 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unspecified_encoding_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unspecified_encoding_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsubscriptable_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsubscriptable_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsubscriptable_value.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsubscriptable_value.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsubscriptable_value_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsubscriptable_value_py37.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.711226 pylint-3.1.0/tests/functional/u/unsupported/
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_assignment_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_assignment_operation.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_assignment_operation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_binary_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_binary_operation.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_binary_operation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_delete_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_delete_operation.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_delete_operation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_version_for_f_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_version_for_f_string.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_version_for_f_string.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_version_for_final.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_version_for_final.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unsupported/unsupported_version_for_final.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.719226 pylint-3.1.0/tests/functional/u/unused/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_argument.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_argument_py3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_argument_py3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_global_variable1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_global_variable2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_global_variable2.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_global_variable2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_global_variable3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_global_variable4.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_global_variable4.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_global_variable4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import_assigned_to.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import_class_def_keyword.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import_everything_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import_everything_disabled.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import_positional_only_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import_py30.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import_py30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_import_py39.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_name_from_wildcard_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_name_from_wildcard_import.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_name_in_string_literal_type_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_name_in_string_literal_type_annotation_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_name_in_string_literal_type_annotation_py310.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_name_in_string_literal_type_annotation_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_name_in_string_literal_type_annotation_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_name_in_string_literal_type_annotation_py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_name_in_string_literal_type_annotation_py39.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_private_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_private_member.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_typing_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4990 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_variable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_variable_after_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_variable_after_inference.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_variable_py36.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_variable_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_variable_py38.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/unused/unused_variable_py38.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.723226 pylint-3.1.0/tests/functional/u/use/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_a_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_a_generator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5591 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_implicit_booleaness_not_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_implicit_booleaness_not_comparison.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_implicit_booleaness_not_comparison_to_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_implicit_booleaness_not_comparison_to_string.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_implicit_booleaness_not_comparison_to_string.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_implicit_booleaness_not_comparison_to_zero.py
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_implicit_booleaness_not_comparison_to_zero.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_implicit_booleaness_not_comparison_to_zero.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_implicit_booleaness_not_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_implicit_booleaness_not_len.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_literal_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_literal_dict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_literal_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_literal_list.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_maxsplit_arg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_maxsplit_arg.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_sequence_for_iteration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_sequence_for_iteration.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_symbolic_message_instead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_symbolic_message_instead.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_yield_from.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/use_yield_from.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/use/used_before_assignment_except_handler_for_try_with_return_py38.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.731226 pylint-3.1.0/tests/functional/u/used/
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_488.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_class_nested_under_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_comprehension_homonyms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_conditional.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_else_continue.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_else_continue.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_else_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_else_return.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_except_handler_for_try_with_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_except_handler_for_try_with_return.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue1081.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue1081.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue2615.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue2615.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue4761.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue4761.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue626.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue626.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3686 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue85.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue85.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_issue853.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_nonlocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_nonlocal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_postponed_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_postponed_evaluation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_py310.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_py312.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_py312.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_py37.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_scoping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_scoping.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_ternary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_ternary.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_type_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_type_annotations.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5842 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_before_assignment_typing.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_prior_global_declaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/used/used_prior_global_declaration.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.735226 pylint-3.1.0/tests/functional/u/useless/
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_else_on_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_else_on_loop.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_object_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_object_inheritance.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15284 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_parent_delegation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_parent_delegation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_parent_delegation_py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_parent_delegation_py38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_return.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_return.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_suppression.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_with_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/useless/useless_with_lock.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/using_constant_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/u/using_constant_test.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.743226 pylint-3.1.0/tests/functional/w/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wildcard_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wildcard_import.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wildcard_import_allowed.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wildcard_import_allowed.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wildcard_import_allowed.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/with_used_before_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/with_used_before_assign.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/with_using_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/with_using_generator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_exception_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_exception_operation.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_exception_operation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_exception_operation_py37.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_exception_operation_py37.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_exception_operation_py37.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_order.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_order2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position13.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position14.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position14.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position7.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position8.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position9.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/w/wrong_import_position_exclude_dunder_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.743226 pylint-3.1.0/tests/functional/y/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/yield_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/yield_from_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/yield_from_iterable.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/yield_from_outside_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/yield_from_outside_func.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/yield_inside_async_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/yield_inside_async_function.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/yield_outside_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/yield_outside_func.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/functional/y/yield_return_mix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.751227 pylint-3.1.0/tests/input/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/benchmark_minimal_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_3k_removed_stuff_py_30.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_i0011.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_i0012.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_i0013.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_i0014.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_i0020.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_i0022.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.751227 pylint-3.1.0/tests/input/func_noerror_cycle/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_noerror_cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_noerror_cycle/a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_noerror_cycle/b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_return_yield_mix_py_33.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_w0122_py_30.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_w0401.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_w0401_disabled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_w0401_disabled_in_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.751227 pylint-3.1.0/tests/input/func_w0401_package/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_w0401_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_w0401_package/all_the_things.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_w0401_package/thing1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_w0401_package/thing2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/func_w0801.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/hide_code_with_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/ignore_except_pass_by_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/multiline-import
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/noext
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/not__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar1
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar2
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar3
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar4
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar5
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar6
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar_cls_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar_cls_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar_empty_func_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar_empty_func_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar_lines_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/similar_lines_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/w0401_cycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/input/w0801_same.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.751227 pylint-3.1.0/tests/lint/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/lint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/lint/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/lint/test_pylinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/lint/test_run_pylint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/lint/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/lint/unittest_expand_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42116 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/lint/unittest_lint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.755226 pylint-3.1.0/tests/message/
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/message/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/message/test_no_removed_msgid_or_symbol_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/message/unittest_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/message/unittest_message_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10805 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/message/unittest_message_definition_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/message/unittest_message_id_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.759226 pylint-3.1.0/tests/messages/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/builtin_module.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_3k_removed_stuff_py_30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_bad_cont_dictcomp_py27.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_bug113231.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_disable_linebased.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_disable_linebased_py30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_i0011.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_i0012.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_i0013.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_i0014.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_i0020.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_i0022.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_noerror_cycle.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_raw_escapes.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_return_yield_mix_py_33.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_toolonglines_py30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_typecheck_callfunc_assigment.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_typecheck_getattr_py30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_typecheck_non_callable_call.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_unicode_literal_py26.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_unicode_literal_py274.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_use_for_or_listcomp_var_py29.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_use_for_or_listcomp_var_py30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_variables_unused_name_from_wilcard_import.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0122_py_30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0312.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0332_py_30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0401.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0401_disabled.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0401_disabled_in_func.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0401_package.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0622.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0623.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0623_py_30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_w0801.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/messages/func_with_without_as_py25.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.759226 pylint-3.1.0/tests/primer/
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/primer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/primer/packages_to_prime.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/primer/test_primer_stdlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.759226 pylint-3.1.0/tests/profile/
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/profile/test_profile_against_externals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.763227 pylint-3.1.0/tests/pyreverse/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.763227 pylint-3.1.0/tests/pyreverse/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/classes_No_Name.dot
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/classes_No_Name.html
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/classes_No_Name.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/classes_No_Name.puml
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/classes_No_Name.vcg
+-rw-r--r--   0 runner    (1001) docker     (127)     2749 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/classes_colorized.dot
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/classes_colorized.puml
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/classes_no_standalone.dot
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/classes_type_check_imports.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/packages_No_Name.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/packages_No_Name.html
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/packages_No_Name.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/packages_No_Name.puml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/packages_No_Name.vcg
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/packages_colorized.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/packages_colorized.puml
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/packages_no_standalone.dot
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/data/packages_type_check_imports.dot
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.155224 pylint-3.1.0/tests/pyreverse/functional/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.155224 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.763227 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/aggregation/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/aggregation/fields.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/aggregation/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.767227 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/attributes_annotation.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/attributes_annotation.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/attributes_annotation.puml
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/attributes_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/attributes_annotation.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/line_breaks.dot
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/line_breaks.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/line_breaks.puml
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/line_breaks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/line_breaks.rc
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/method_annotation.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/annotations/method_annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.767227 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/attributes/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/attributes/_monkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/attributes/delayed_external_monkey_patching.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/attributes/delayed_external_monkey_patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/attributes/duplicates.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/attributes/duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/attributes/instance_attributes.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/attributes/instance_attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.771227 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/colorized_output/
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/colorized_output/colorized.puml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/colorized_output/colorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/colorized_output/colorized.rc
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/colorized_output/custom_colors.dot
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/colorized_output/custom_colors.puml
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/colorized_output/custom_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/colorized_output/custom_colors.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.771227 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/inheritance/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/inheritance/no_standalone.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/inheritance/no_standalone.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/inheritance/no_standalone.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/inheritance/simple_inheritance.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/inheritance/simple_inheritance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.151224 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/namespaces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.771227 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/namespaces/pep420/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/namespaces/pep420/pep420.dot
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/namespaces/pep420/pep420.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/namespaces/pep420/pep420.puml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/namespaces/pep420/pep420.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/namespaces/pep420/pep420.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.771227 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/regression/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/regression/regression_8031.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/class_diagrams/regression/regression_8031.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.771227 pylint-3.1.0/tests/pyreverse/functional/package_diagrams/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/package_diagrams/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.771227 pylint-3.1.0/tests/pyreverse/functional/package_diagrams/type_check_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/package_diagrams/type_check_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/package_diagrams/type_check_imports/mod_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/package_diagrams/type_check_imports/mod_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/package_diagrams/type_check_imports/mod_c.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/package_diagrams/type_check_imports/mod_d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/functional/package_diagrams/type_check_imports/packages.mmd
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/test_diadefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/test_diagrams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/test_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/test_printer_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/test_pyreverse_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8358 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/pyreverse/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/absimp/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/absimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/absimp/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/allow_reexport/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/allow_reexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/allow_reexport/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/application_crash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/bad_package/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/bad_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/bad_package/wrong.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/beyond_top/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.155224 pylint-3.1.0/tests/regrtest_data/beyond_top_four/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/beyond_top_four/double_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_four/double_name/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/beyond_top_four/module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_four/module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/beyond_top_four/module/double_name/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_four/module/double_name/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_four/module/double_name/function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/beyond_top_four/module/sub_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_four/module/sub_module/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/beyond_top_four/module/sub_module/sub_sub_module/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_four/module/sub_module/sub_sub_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_four/module/sub_module/sub_sub_module/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.779227 pylint-3.1.0/tests/regrtest_data/beyond_top_three/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_three/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_three/a.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/beyond_top_three/level1/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_three/level1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_three/level1/beyond_top_three.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/beyond_top_two/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_two/import_package.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/beyond_top_two/namespace_package/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/beyond_top_two/namespace_package/lower_level/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_two/namespace_package/lower_level/helper_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_two/namespace_package/plugin_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/beyond_top_two/namespace_package/top_level_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/classdoc_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/comments_pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/dataclasses_pyreverse/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/dataclasses_pyreverse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/decimal_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/descriptor_crash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.155224 pylint-3.1.0/tests/regrtest_data/directory/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/directory/ignored_subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/directory/ignored_subdirectory/failing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/directory/package/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/directory/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/directory/package/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/directory/package/subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/directory/package/subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/directory/package/subpackage/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/directory/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/directory/subdirectory/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/directory/subdirectory/subsubdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/directory/subdirectory/subsubdirectory/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/dummy/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/dummy/another.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/dummy/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/dummy_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/dummy_plugin/dummy_conf_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/dummy_plugin/dummy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/dummy_plugin.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.159224 pylint-3.1.0/tests/regrtest_data/duplicate_code/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.783227 pylint-3.1.0/tests/regrtest_data/duplicate_code/ignore_conditional_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/ignore_conditional_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/ignore_conditional_imports/file_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/ignore_conditional_imports/file_two.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.787227 pylint-3.1.0/tests/regrtest_data/duplicate_code/ignore_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/ignore_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/ignore_imports/file_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/ignore_imports/file_two.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.787227 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_all/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_all/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_all/second.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_all/third.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.787227 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_file/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_file/second.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_file/third.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.787227 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_file_double/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_file_double/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_file_double/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_file_double/second.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_file_double/third.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.787227 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_begin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_begin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_begin/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_begin/second.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.787227 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_disable_all/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_disable_all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_disable_all/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_disable_all/second.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.787227 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_end/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_end/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_end/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_end/second.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.787227 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_middle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_middle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_middle/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_line_middle/second.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.791226 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope/second.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope/third.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.791226 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope_double/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope_double/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope_double/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope_double/second.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope_double/third.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.791226 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope_second_function/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope_second_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope_second_function/first.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/raw_strings_disable_scope_second_function/second.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.791226 pylint-3.1.0/tests/regrtest_data/duplicate_code/useless_suppression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/useless_suppression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/useless_suppression/file_one.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/duplicate_code/useless_suppression/file_two.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/empty.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.791226 pylint-3.1.0/tests/regrtest_data/encoding/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/encoding/bad_missing_num.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/encoding/bad_wrong_num.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/encoding/good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/fail_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/fail_on_info_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/fail_under_minus10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/fail_under_plus7_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/fixme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/func_block_disable_msg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.159224 pylint-3.1.0/tests/regrtest_data/hang/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.791226 pylint-3.1.0/tests/regrtest_data/hang/pkg4972/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/hang/pkg4972/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.791226 pylint-3.1.0/tests/regrtest_data/hang/pkg4972/string/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/hang/pkg4972/string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/import_assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/import_package_subpackage_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/import_something.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.791226 pylint-3.1.0/tests/regrtest_data/imported_module_in_typehint/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/imported_module_in_typehint/module_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/imported_module_in_typehint/module_b.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.791226 pylint-3.1.0/tests/regrtest_data/importing_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/importing_plugin/importing_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.791226 pylint-3.1.0/tests/regrtest_data/init_wildcard/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/init_wildcard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/invalid_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/issue_5724.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/line_too_long_no_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/long_test_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/max_inferable_limit_for_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/max_inferable_limit_for_classes/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/max_inferable_limit_for_classes/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/max_inferable_limit_for_classes/nodes/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/max_inferable_limit_for_classes/other_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/module_global.py
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/no_stdout_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/numarray_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/numarray_inf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/package/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/package/AudioTime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/package/subpackage/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/package/subpackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/package/subpackage/module.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/package_all/
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/package_all/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/package_all/notmissing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.159224 pylint-3.1.0/tests/regrtest_data/pep420/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.159224 pylint-3.1.0/tests/regrtest_data/pep420/basic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.159224 pylint-3.1.0/tests/regrtest_data/pep420/basic/project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.159224 pylint-3.1.0/tests/regrtest_data/pep420/basic/project/namespace/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/pep420/basic/project/namespace/package/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/pep420/basic/project/namespace/package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.159224 pylint-3.1.0/tests/regrtest_data/pep420/wrapper/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.159224 pylint-3.1.0/tests/regrtest_data/pep420/wrapper/project/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.159224 pylint-3.1.0/tests/regrtest_data/pep420/wrapper/project/namespace/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.159224 pylint-3.1.0/tests/regrtest_data/pep420/wrapper/project/namespace/package/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/pep420/wrapper/project/namespace/package/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/pep420/wrapper/project/namespace/package/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/pep420/wrapper/project/namespace/package/logging/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/pep420/wrapper/project/namespace/package/logging/wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/pkg_mod_imports/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/pkg_mod_imports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/pkg_mod_imports/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/pkg_mod_imports/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/pkg_mod_imports/base/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/precedence_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/preferred_module/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/preferred_module/unpreferred_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/preferred_module/unpreferred_submodule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/pyi/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/pyi/foo.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.163224 pylint-3.1.0/tests/regrtest_data/regression_missing_init_3564/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/regression_missing_init_3564/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/regression_missing_init_3564/subdirectory/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/settings_project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/settings_project/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/settings_project/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/special_attr_scope_lookup_crash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/syntax_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/test_no_name_in_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/test_pylintrc_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/try_finally_disable_msg_crash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.795227 pylint-3.1.0/tests/regrtest_data/unicode/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/unicode/invisible_function.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/unicode/pep_bidirectional_utf_16_bom.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/unicode/pep_bidirectional_utf_16_le_no_bom.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/unicode/pep_bidirectional_utf_32_bom.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/unicode/pep_bidirectional_utf_32_le_no_bom.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/unused_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14042 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/very_long_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/wildcard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/regrtest_data/wrong_import_position.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.799227 pylint-3.1.0/tests/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     8190 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/reporters/unittest_json_reporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12984 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/reporters/unittest_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26010 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_check_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6361 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_functional_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_import_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_numversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_pragma_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3939 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_pylint_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_regr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59631 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_self.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10202 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/test_similar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.799227 pylint-3.1.0/tests/testutils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.799227 pylint-3.1.0/tests/testutils/_primer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.163224 pylint-3.1.0/tests/testutils/_primer/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.799227 pylint-3.1.0/tests/testutils/_primer/fixtures/batched/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/batched/expected.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/batched/main_batch0.json
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/batched/main_batch1.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/batched/pr_batch0.json
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/batched/pr_batch1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.799227 pylint-3.1.0/tests/testutils/_primer/fixtures/both_empty/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/both_empty/expected.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/both_empty/main.json
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/both_empty/pr.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.799227 pylint-3.1.0/tests/testutils/_primer/fixtures/message_changed/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/message_changed/expected.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/message_changed/expected_truncated.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/message_changed/main.json
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/message_changed/pr.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.803227 pylint-3.1.0/tests/testutils/_primer/fixtures/no_change/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/no_change/expected.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/no_change/main.json
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/fixtures/no_change/pr.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/test_package_to_lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/_primer/test_primer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.803227 pylint-3.1.0/tests/testutils/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.163224 pylint-3.1.0/tests/testutils/data/functional/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.803227 pylint-3.1.0/tests/testutils/data/functional/broken_output_ok_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/broken_output_ok_test/exec_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/broken_output_ok_test/exec_used.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.803227 pylint-3.1.0/tests/testutils/data/functional/broken_output_wrong_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/broken_output_wrong_test/exec_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/broken_output_wrong_test/exec_used.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.803227 pylint-3.1.0/tests/testutils/data/functional/no_output_ok_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/no_output_ok_test/exec_used.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.803227 pylint-3.1.0/tests/testutils/data/functional/no_output_wrong_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/no_output_wrong_test/exec_used.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.803227 pylint-3.1.0/tests/testutils/data/functional/ok_output_ok_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/ok_output_ok_test/exec_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/ok_output_ok_test/exec_used.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.803227 pylint-3.1.0/tests/testutils/data/functional/ok_output_wrong_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/ok_output_wrong_test/exec_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/ok_output_wrong_test/exec_used.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.803227 pylint-3.1.0/tests/testutils/data/functional/wrong_output_ok_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/wrong_output_ok_test/exec_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/wrong_output_ok_test/exec_used.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.803227 pylint-3.1.0/tests/testutils/data/functional/wrong_output_wrong_test/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/wrong_output_wrong_test/exec_used.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/functional/wrong_output_wrong_test/exec_used.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/init_hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/init_hook.rc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.807227 pylint-3.1.0/tests/testutils/data/m/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.807227 pylint-3.1.0/tests/testutils/data/m/max_overflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/m/max_overflow/max_overflow_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/m/max_overflow/max_overflow_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/m/max_overflow/max_overflow_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/m/minimal_messages_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/m/minimal_messages_excluded.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/m/minimal_messages_excluded.rc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/t.3.out
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/t.out
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/t.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.807227 pylint-3.1.0/tests/testutils/data/u/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.807227 pylint-3.1.0/tests/testutils/data/u/_no_issue_here/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/u/_no_issue_here/_incredibly_bold_mischief.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.807227 pylint-3.1.0/tests/testutils/data/u/use/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/u/use/use_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/u/use/using_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/u/use_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.807227 pylint-3.1.0/tests/testutils/data/u/using/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/u/using/using_len.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/u.out
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/u.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/data/v.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/dummy_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.807227 pylint-3.1.0/tests/testutils/pyreverse_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/pyreverse_data/_not_a_functest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/pyreverse_data/functest_with_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/pyreverse_data/functest_with_options.rc
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/pyreverse_data/functest_without_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/test_configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/test_functional_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/test_lint_module_output_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/test_output_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/test_pyreverse_testutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/testutils/test_testutils_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:16.807227 pylint-3.1.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/utils/unittest_ast_walker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-25 16:48:03.000000 pylint-3.1.0/tests/utils/unittest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-02-25 16:48:03.000000 pylint-3.1.0/tox.ini
```

### Comparing `pylint-3.0.4/CONTRIBUTORS.txt` & `pylint-3.1.0/CONTRIBUTORS.txt`

 * *Files 2% similar despite different names*

```diff
@@ -152,14 +152,16 @@
 - Alexander Todorov <atodorov@otb.bg>:
   * added new error conditions to 'bad-super-call',
   * Added new check for incorrect len(SEQUENCE) usage,
   * Added new extension for comparison against empty string constants,
   * Added new extension which detects comparing integers to zero,
   * Added new useless-return checker,
   * Added new try-except-raise checker
+- theirix <theirix@gmail.com>
+- crazybolillo <antonio@zoftko.com>
 - Téo Bouvard <teobouvard@gmail.com>
 - Stavros Ntentos <133706+stdedos@users.noreply.github.com>
 - Nicolas Boulenguez <nicolas@debian.org>
 - Mihai Balint <balint.mihai@gmail.com>
 - Mark Bell <mark00bell@googlemail.com>
 - Levi Gruspe <mail.levig@gmail.com>
 - Jakub Kuczys <me@jacken.men>
@@ -168,15 +170,14 @@
 - David Douard <david.douard@sdfa3.org>
 - Daniel Balparda <balparda@google.com> (Google): GPyLint maintainer (Google's pylint variant)
 - Bastien Vallet <bastien.vallet@gmail.com> (Djailla)
 - Aru Sahni <arusahni@gmail.com>: Git ignoring, regex-based ignores
 - Andreas Freimuth <andreas.freimuth@united-bits.de>: fix indentation checking with tabs
 - Alexandru Coman <fcoman@bitdefender.com>
 - jpkotta <jpkotta@gmail.com>
-- crazybolillo <antonio@zoftko.com>
 - Takahide Nojima <nozzy123nozzy@gmail.com>
 - Taewon D. Kim <kimt33@mcmaster.ca>
 - Sneaky Pete <sneakypete81@gmail.com>
 - Sergey B Kirpichev <skirpichev@gmail.com>
 - Sandro Tosi <sandro.tosi@gmail.com>: Debian packaging
 - Rogdham <contact@rogdham.net>
 - Rene Zhang <rz99@cornell.edu>
@@ -245,14 +246,15 @@
 - Alain Leufroy <alain.leufroy@logilab.fr>
 - Adam Williamson <awilliam@redhat.com>
 - xmo-odoo <xmo-odoo@users.noreply.github.com>
 - tbennett0 <tbennett0@users.noreply.github.com>
 - omarandlorraine <64254276+omarandlorraine@users.noreply.github.com>
 - craig-sh <craig-sh@users.noreply.github.com>
 - bernie gray <bfgray3@users.noreply.github.com>
+- azinneck0485 <123660683+azinneck0485@users.noreply.github.com>
 - Wes Turner <westurner@google.com> (Google): added new check 'inconsistent-quotes'
 - Tyler Thieding <tyler@thieding.com>
 - Tobias Hernstig <30827238+thernstig@users.noreply.github.com>
 - Thomas Grainger <tagrain@gmail.com>
 - Smixi <sismixx@hotmail.fr>
 - Simu Toni <simutoni@gmail.com>
 - Sergei Lebedev <185856+superbobry@users.noreply.github.com>
@@ -360,20 +362,22 @@
 - Yory <39745367+yory8@users.noreply.github.com>
 - Yoichi Nakayama <yoichi.nakayama@gmail.com>
 - Yeting Li <liyt@ios.ac.cn> (yetingli)
 - Yannack <yannack@users.noreply.github.com>
 - Yann Dirson <ydirson@free.fr>
 - Yang Yang <y4n9squared@gmail.com>
 - Xi Shen <davidshen84@gmail.com>
+- Winston H <56998716+winstxnhdw@users.noreply.github.com>
 - Will Shanks <wsha@posteo.net>
 - Viorel Știrbu <viorels@gmail.com>: intern-builtin warning.
 - VictorT <victor.taix@gmail.com>
 - Victor Jiajunsu <16359131+jiajunsu@users.noreply.github.com>
 - ViRuSTriNiTy <cradle-of-mail@gmx.de>
 - Val Lorentz <progval+github@progval.net>
+- Udi Fuchs <udifuchs@gmail.com>
 - Trevor Bekolay <tbekolay@gmail.com>
   * Added --list-msgs-enabled command
 - Tomer Chachamu <tomer.chachamu@gmail.com>: simplifiable-if-expression
 - Tomasz Magulski <tomasz@magullab.io>
 - Tom <tsarantis@proton.me>
 - Tim Hatch <tim@timhatch.com>
 - Tim Gates <tim.gates@iress.com>
@@ -390,19 +394,21 @@
 - Stanislav Levin <slev@altlinux.org>
 - Sorin Sbarnea <ssbarnea@redhat.com>
 - Slavfox <slavfoxman@gmail.com>
 - Skip Montanaro <skip@pobox.com>
 - Sigurd Spieckermann <2206639+sisp@users.noreply.github.com>
 - Shiv Venkatasubrahmanyam <shvenkat@users.noreply.github.com>
 - Sebastian Müller <mueller.seb@posteo.de>
+- Sayyed Faisal Ali <80758388+C0DE-SLAYER@users.noreply.github.com>
 - Sasha Bagan <pnlbagan@gmail.com>
 - Sardorbek Imomaliev <sardorbek.imomaliev@gmail.com>
 - Santiago Castro <bryant@montevideo.com.uy>
 - Samuel Freilich <sfreilich@google.com> (sfreilich)
 - Sam Vermeiren <88253337+PaaEl@users.noreply.github.com>
+- Ryan Ozawa <ryan.ozawa21@gmail.com>
 - Ryan McGuire <ryan@enigmacurry.com>
 - Ry4an Brase <ry4an-hg@ry4an.org>
 - Ruro <ruro.ruro@ya.ru>
 - Roman Ivanov <me@roivanov.com>
 - Robert Schweizer <robert_schweizer@gmx.de>
 - Reverb Chu <reverbc@users.noreply.github.com>
 - Renat Galimov <renat2017@gmail.com>
@@ -431,30 +437,36 @@
 - Nir Soffer <nirsof@gmail.com>
 - Niko Wenselowski <niko@nerdno.de>
 - Nikita Sobolev <mail@sobolevn.me>
 - Nick Smith <clickthisnick@users.noreply.github.com>
 - Neowizard <Neowizard@users.noreply.github.com>
 - Ned Batchelder <ned@nedbatchelder.com>
 - Natalie Serebryakova <natalie.serebryakova@Natalies-MacBook-Pro.local>
+- Naglis Jonaitis <827324+naglis@users.noreply.github.com>
 - Moody <mooodyhunter@outlook.com>
 - Mitchell Young <mitchelly@gmail.com>: minor adjustment to docparams
 - Mitar <mitar.github@tnode.com>
+- Ming Lyu <CareF.Lm@gmail.com>
 - Mikhail f. Shiryaev <mr.felixoid@gmail.com>
 - Mike Fiedler <miketheman@gmail.com> (miketheman)
 - Mike Bryant <leachim@leachim.info>
+- Mike Bernard <mdbernard@pm.me>
 - Michka Popoff <michkapopoff@gmail.com>
 - Michal Vasilek <michal@vasilek.cz>
 - Michael Scott Cuthbert <cuthbert@mit.edu>
 - Michael Kefeder <oss@multiwave.ch>
+- Michael K <michael-k@users.noreply.github.com>
 - Michael Hudson-Doyle <michael.hudson@canonical.com>
 - Michael Giuffrida <mgiuffrida@users.noreply.github.com>
 - Melvin Hazeleger <31448155+melvio@users.noreply.github.com>
+- Meltem Kenis <meltem.kenis@plentific.com>
 - Mehdi Drissi <mdrissi@hmc.edu>
 - Matěj Grabovský <mgrabovs@redhat.com>
 - Matthijs Blom <19817960+MatthijsBlom@users.noreply.github.com>
+- Matej Spiller Muys <matej.spiller-muys@bitstamp.net>
 - Matej Marušák <marusak.matej@gmail.com>
 - Markus Siebenhaar <41283549+siehar@users.noreply.github.com>
 - Marco Edward Gorelli <marcogorelli@protonmail.com>: Documented Jupyter integration
 - Marcin Kurczewski <rr-@sakuya.pl> (rr-)
 - Maik Röder <maikroeder@gmail.com>
 - Lumír 'Frenzy' Balhar <frenzy.madness@gmail.com>
 - Ludovic Aubry <ludal@logilab.fr>
@@ -525,14 +537,15 @@
 - Edward K. Ream <edreamleo@gmail.com>
 - Edgemaster <grand.edgemaster@gmail.com>
 - Eddie Darling <eddie.darling@genapsys.com>
 - Drew Risinger <drewrisinger@users.noreply.github.com>
 - Dr. Nick <das-intensity@users.noreply.github.com>
 - Don Jayamanne <don.jayamanne@yahoo.com>
 - Dmytro Kyrychuk <dmytro.kyrychuck@gmail.com>
+- Dionisio E Alonso <baco@users.noreply.github.com>
 - DetachHead <57028336+DetachHead@users.noreply.github.com>
 - Denis Laxalde <denis.laxalde@logilab.fr>
 - David Lawson <dmrlawson@gmail.com>
 - David Cain <davidjosephcain@gmail.com>
 - Danny Hermes <daniel.j.hermes@gmail.com>
 - Daniele Procida <daniele@vurt.org>
 - Daniela Plascencia <daplascen@gmail.com>
@@ -543,14 +556,15 @@
 - Daniel Dorani <ddandd@gmail.com> (doranid)
 - Daniel Brookman <53625739+dbrookman@users.noreply.github.com>
 - Dan Garrette <dhgarrette@gmail.com>
 - Damien Nozay <damien.nozay@gmail.com>
 - Cubicpath <Cubicpath@protonmail.com>
 - Craig Citro <craigcitro@gmail.com>
 - Cosmo <cosmo@cosmo.red>
+- Clément Schreiner <clement@mux.me>
 - Clément Pit-Claudel <cpitclaudel@users.noreply.github.com>
 - Christopher Zurcher <zurcher@users.noreply.github.com>
 - Christian Clauss <cclauss@me.com>
 - Carl Crowder <bitbucket@carlcrowder.com>: don't evaluate the value of arguments for 'dangerous-default-value'
 - Carey Metcalfe <carey@cmetcalfe.ca>: demoted `try-except-raise` from error to warning
 - Cameron Olechowski <camsterole@users.noreply.github.com>
 - Calin Don <calin.don@gmail.com>
@@ -576,14 +590,15 @@
 - Anentropic <ego@anentropic.com>
 - Andy Young <a7young@ucsd.edu>
 - Andy Palmer <25123779+ninezerozeronine@users.noreply.github.com>
 - Andrzej Klajnert <github@aklajnert.pl>
 - Andrew Howe <howeaj@users.noreply.github.com>
 - Andres Perez Hortal <andresperezcba@gmail.com>
 - Andre Hora <andrehora@users.noreply.github.com>
+- Aman Salwan <121633121+AmanSal1@users.noreply.github.com>
 - Alok Singh <8325708+alok@users.noreply.github.com>
 - Allan Chandler <95424144+allanc65@users.noreply.github.com> (allanc65)
   * Fixed issue 5452, false positive missing-param-doc for multi-line Google-style params
 - Alex Mor <5476113+nashcontrol@users.noreply.github.com>
 - Alex Jurkiewicz <alex@jurkiewi.cz>
 - Alex Hearn <alex.d.hearn@gmail.com>
 - Aleksander Mamla <alek.mamla@gmail.com>
```

### Comparing `pylint-3.0.4/LICENSE` & `pylint-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/PKG-INFO` & `pylint-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pylint
-Version: 3.0.4
+Version: 3.1.0
 Summary: python code static checker
 Author-email: Python Code Quality Authority <code-quality@python.org>
 License: GPL-2.0-or-later
 Project-URL: Docs: User Guide, https://pylint.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/pylint
 Project-URL: homepage, https://github.com/pylint-dev/pylint
-Project-URL: What's New, https://pylint.readthedocs.io/en/latest/whatsnew/2/
+Project-URL: What's New, https://pylint.readthedocs.io/en/latest/whatsnew/3/
 Project-URL: Bug Tracker, https://github.com/pylint-dev/pylint/issues
 Project-URL: Discord Server, https://discord.com/invite/Egy6P8AMB5
 Project-URL: Docs: Contributor Guide, https://pylint.readthedocs.io/en/latest/development_guide/contributor_guide/index.html
 Keywords: static code analysis,linter,python,lint
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -35,15 +35,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: CONTRIBUTORS.txt
 Requires-Dist: dill>=0.2; python_version < "3.11"
 Requires-Dist: dill>=0.3.6; python_version >= "3.11"
 Requires-Dist: dill>=0.3.7; python_version >= "3.12"
 Requires-Dist: platformdirs>=2.2.0
-Requires-Dist: astroid<=3.1.0-dev0,>=3.0.1
+Requires-Dist: astroid<=3.2.0-dev0,>=3.1.0
 Requires-Dist: isort!=5.13.0,<6,>=4.2.5
 Requires-Dist: mccabe<0.8,>=0.6
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Requires-Dist: tomlkit>=0.10.1
 Requires-Dist: colorama>=0.4.5; sys_platform == "win32"
 Requires-Dist: typing-extensions>=3.10.0; python_version < "3.10"
 Provides-Extra: testutils
```

### Comparing `pylint-3.0.4/README.rst` & `pylint-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/__init__.py` & `pylint-3.1.0/pylint/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/__pkginfo__.py` & `pylint-3.1.0/pylint/__pkginfo__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """This module exists for compatibility reasons.
 
 It's updated via tbump, do not modify.
 """
 
 from __future__ import annotations
 
-__version__ = "3.0.4"
+__version__ = "3.1.0"
 
 
 def get_numversion_from_version(v: str) -> tuple[int, int, int]:
     """Kept for compatibility reason.
 
     See https://github.com/pylint-dev/pylint/issues/4399
     https://github.com/pylint-dev/pylint/issues/4420,
```

### Comparing `pylint-3.0.4/pylint/checkers/__init__.py` & `pylint-3.1.0/pylint/checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/async.py` & `pylint-3.1.0/pylint/checkers/async.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/bad_chained_comparison.py` & `pylint-3.1.0/pylint/checkers/bad_chained_comparison.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/base/__init__.py` & `pylint-3.1.0/pylint/checkers/base/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/base/basic_checker.py` & `pylint-3.1.0/pylint/checkers/base/basic_checker.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,15 +476,18 @@
         # * the unique child of a try/except body
         # * a yield statement
         # * an ellipsis (which can be used on Python 3 instead of pass)
         # warn W0106 if we have any underlying function call (we can't predict
         # side effects), else pointless-statement
         if (
             isinstance(expr, (nodes.Yield, nodes.Await))
-            or (isinstance(node.parent, nodes.Try) and node.parent.body == [node])
+            or (
+                isinstance(node.parent, (nodes.Try, nodes.TryStar))
+                and node.parent.body == [node]
+            )
             or (isinstance(expr, nodes.Const) and expr.value is Ellipsis)
         ):
             return
         if isinstance(expr, nodes.NamedExpr):
             self.add_message("named-expr-without-context", node=node, confidence=HIGH)
         elif any(expr.nodes_of_class(nodes.Call)):
             self.add_message(
```

### Comparing `pylint-3.0.4/pylint/checkers/base/basic_error_checker.py` & `pylint-3.1.0/pylint/checkers/base/basic_error_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/base/comparison_checker.py` & `pylint-3.1.0/pylint/checkers/base/comparison_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/base/docstring_checker.py` & `pylint-3.1.0/pylint/checkers/base/docstring_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/base/name_checker/__init__.py` & `pylint-3.1.0/pylint/checkers/base/name_checker/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/base/name_checker/checker.py` & `pylint-3.1.0/pylint/checkers/base/name_checker/checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,17 +330,17 @@
         self._check_name("module", node.name.split(".")[-1], node)
         self._bad_names = {}
 
     def leave_module(self, _: nodes.Module) -> None:
         for all_groups in self._bad_names.values():
             if len(all_groups) < 2:
                 continue
-            groups: collections.defaultdict[
-                int, list[list[_BadNamesTuple]]
-            ] = collections.defaultdict(list)
+            groups: collections.defaultdict[int, list[list[_BadNamesTuple]]] = (
+                collections.defaultdict(list)
+            )
             min_warnings = sys.maxsize
             prevalent_group, _ = max(all_groups.items(), key=lambda item: len(item[1]))
             for group in all_groups.values():
                 groups[len(group)].append(group)
                 min_warnings = min(len(group), min_warnings)
             if len(groups[min_warnings]) > 1:
                 by_line = sorted(
@@ -405,14 +405,20 @@
         frame = node.frame()
         assign_type = node.assign_type()
 
         # Check names defined in comprehensions
         if isinstance(assign_type, nodes.Comprehension):
             self._check_name("inlinevar", node.name, node)
 
+        elif isinstance(assign_type, nodes.TypeVar):
+            self._check_name("typevar", node.name, node)
+
+        elif isinstance(assign_type, nodes.TypeAlias):
+            self._check_name("typealias", node.name, node)
+
         # Check names defined in module scope
         elif isinstance(frame, nodes.Module):
             # Check names defined in Assign nodes
             if isinstance(assign_type, nodes.Assign):
                 inferred_assign_type = utils.safe_infer(assign_type.value)
 
                 # Check TypeVar's and TypeAliases assigned alone or in tuple assignment
@@ -621,14 +627,17 @@
             keywords = node.assign_type().value.keywords
             args = node.assign_type().value.args
         elif isinstance(node.parent, nodes.Tuple):
             keywords = (
                 node.assign_type().value.elts[node.parent.elts.index(node)].keywords
             )
             args = node.assign_type().value.elts[node.parent.elts.index(node)].args
+        else:  # PEP 695 generic type nodes
+            keywords = ()
+            args = ()
 
         variance = TypeVarVariance.invariant
         name_arg = None
         for kw in keywords:
             if variance == TypeVarVariance.double_variant:
                 pass
             elif kw.arg == "covariant" and kw.value.value:
```

### Comparing `pylint-3.0.4/pylint/checkers/base/name_checker/naming_style.py` & `pylint-3.1.0/pylint/checkers/base/name_checker/naming_style.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/base/pass_checker.py` & `pylint-3.1.0/pylint/checkers/base/pass_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/base_checker.py` & `pylint-3.1.0/pylint/checkers/base_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,18 +184,18 @@
     ) -> MessageDefinition:
         if isinstance(self, (BaseTokenChecker, BaseRawFileChecker)):
             default_scope = WarningScope.LINE
         else:
             default_scope = WarningScope.NODE
         options: ExtraMessageOptions = {}
         if len(msg_tuple) == 4:
-            (msg, symbol, descr, msg_options) = msg_tuple  # type: ignore[misc]
+            (msg, symbol, descr, msg_options) = msg_tuple
             options = ExtraMessageOptions(**msg_options)
         elif len(msg_tuple) == 3:
-            (msg, symbol, descr) = msg_tuple  # type: ignore[misc]
+            (msg, symbol, descr) = msg_tuple
         else:
             error_msg = """Messages should have a msgid, a symbol and a description. Something like this :
 
 "W1234": (
     "message",
     "message-symbol",
     "Message description with detail.",
```

### Comparing `pylint-3.0.4/pylint/checkers/classes/__init__.py` & `pylint-3.1.0/pylint/checkers/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/classes/class_checker.py` & `pylint-3.1.0/pylint/checkers/classes/class_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/classes/special_methods_checker.py` & `pylint-3.1.0/pylint/checkers/classes/special_methods_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/dataclass_checker.py` & `pylint-3.1.0/pylint/checkers/dataclass_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/deprecated.py` & `pylint-3.1.0/pylint/checkers/deprecated.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,34 +7,46 @@
 from __future__ import annotations
 
 from collections.abc import Container, Iterable
 from itertools import chain
 
 import astroid
 from astroid import nodes
+from astroid.bases import Instance
 
 from pylint.checkers import utils
 from pylint.checkers.base_checker import BaseChecker
 from pylint.checkers.utils import get_import_name, infer_all, safe_infer
+from pylint.interfaces import INFERENCE
 from pylint.typing import MessageDefinitionTuple
 
 ACCEPTABLE_NODES = (
     astroid.BoundMethod,
     astroid.UnboundMethod,
     nodes.FunctionDef,
     nodes.ClassDef,
+    astroid.Attribute,
 )
 
 
 class DeprecatedMixin(BaseChecker):
     """A mixin implementing logic for checking deprecated symbols.
 
     A class implementing mixin must define "deprecated-method" Message.
     """
 
+    DEPRECATED_ATTRIBUTE_MESSAGE: dict[str, MessageDefinitionTuple] = {
+        "W4906": (
+            "Using deprecated attribute %r",
+            "deprecated-attribute",
+            "The attribute is marked as deprecated and will be removed in the future.",
+            {"shared": True},
+        ),
+    }
+
     DEPRECATED_MODULE_MESSAGE: dict[str, MessageDefinitionTuple] = {
         "W4901": (
             "Deprecated module %r",
             "deprecated-module",
             "A module marked as deprecated is imported.",
             {"old_names": [("W0402", "old-deprecated-module")], "shared": True},
         ),
@@ -72,14 +84,19 @@
             "Using deprecated decorator %s()",
             "deprecated-decorator",
             "The decorator is marked as deprecated and will be removed in the future.",
             {"old_names": [("W1513", "old-deprecated-decorator")], "shared": True},
         ),
     }
 
+    @utils.only_required_for_messages("deprecated-attribute")
+    def visit_attribute(self, node: astroid.Attribute) -> None:
+        """Called when an `astroid.Attribute` node is visited."""
+        self.check_deprecated_attribute(node)
+
     @utils.only_required_for_messages(
         "deprecated-method",
         "deprecated-argument",
         "deprecated-class",
     )
     def visit_call(self, node: nodes.Call) -> None:
         """Called when a :class:`nodes.Call` node is visited."""
@@ -185,14 +202,33 @@
 
         Returns:
             collections.abc.Container of deprecated class names.
         """
         # pylint: disable=unused-argument
         return ()
 
+    def deprecated_attributes(self) -> Iterable[str]:
+        """Callback returning the deprecated attributes."""
+        return ()
+
+    def check_deprecated_attribute(self, node: astroid.Attribute) -> None:
+        """Checks if the attribute is deprecated."""
+        inferred_expr = safe_infer(node.expr)
+        if not isinstance(inferred_expr, (nodes.ClassDef, Instance, nodes.Module)):
+            return
+        attribute_qname = ".".join((inferred_expr.qname(), node.attrname))
+        for deprecated_name in self.deprecated_attributes():
+            if attribute_qname == deprecated_name:
+                self.add_message(
+                    "deprecated-attribute",
+                    node=node,
+                    args=(attribute_qname,),
+                    confidence=INFERENCE,
+                )
+
     def check_deprecated_module(self, node: nodes.Import, mod_path: str | None) -> None:
         """Checks if the module is deprecated."""
         for mod_name in self.deprecated_modules():
             if mod_path == mod_name or mod_path and mod_path.startswith(mod_name + "."):
                 self.add_message("deprecated-module", node=node, args=mod_path)
 
     def check_deprecated_method(self, node: nodes.Call, inferred: nodes.NodeNG) -> None:
```

### Comparing `pylint-3.0.4/pylint/checkers/design_analysis.py` & `pylint-3.1.0/pylint/checkers/design_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,80 +17,88 @@
 from pylint.checkers import BaseChecker
 from pylint.checkers.utils import is_enum, only_required_for_messages
 from pylint.typing import MessageDefinitionTuple
 
 if TYPE_CHECKING:
     from pylint.lint import PyLinter
 
-MSGS: dict[
-    str, MessageDefinitionTuple
-] = {  # pylint: disable=consider-using-namedtuple-or-dataclass
-    "R0901": (
-        "Too many ancestors (%s/%s)",
-        "too-many-ancestors",
-        "Used when class has too many parent classes, try to reduce "
-        "this to get a simpler (and so easier to use) class.",
-    ),
-    "R0902": (
-        "Too many instance attributes (%s/%s)",
-        "too-many-instance-attributes",
-        "Used when class has too many instance attributes, try to reduce "
-        "this to get a simpler (and so easier to use) class.",
-    ),
-    "R0903": (
-        "Too few public methods (%s/%s)",
-        "too-few-public-methods",
-        "Used when class has too few public methods, so be sure it's "
-        "really worth it.",
-    ),
-    "R0904": (
-        "Too many public methods (%s/%s)",
-        "too-many-public-methods",
-        "Used when class has too many public methods, try to reduce "
-        "this to get a simpler (and so easier to use) class.",
-    ),
-    "R0911": (
-        "Too many return statements (%s/%s)",
-        "too-many-return-statements",
-        "Used when a function or method has too many return statement, "
-        "making it hard to follow.",
-    ),
-    "R0912": (
-        "Too many branches (%s/%s)",
-        "too-many-branches",
-        "Used when a function or method has too many branches, "
-        "making it hard to follow.",
-    ),
-    "R0913": (
-        "Too many arguments (%s/%s)",
-        "too-many-arguments",
-        "Used when a function or method takes too many arguments.",
-    ),
-    "R0914": (
-        "Too many local variables (%s/%s)",
-        "too-many-locals",
-        "Used when a function or method has too many local variables.",
-    ),
-    "R0915": (
-        "Too many statements (%s/%s)",
-        "too-many-statements",
-        "Used when a function or method has too many statements. You "
-        "should then split it in smaller functions / methods.",
-    ),
-    "R0916": (
-        "Too many boolean expressions in if statement (%s/%s)",
-        "too-many-boolean-expressions",
-        "Used when an if statement contains too many boolean expressions.",
-    ),
-}
+MSGS: dict[str, MessageDefinitionTuple] = (
+    {  # pylint: disable=consider-using-namedtuple-or-dataclass
+        "R0901": (
+            "Too many ancestors (%s/%s)",
+            "too-many-ancestors",
+            "Used when class has too many parent classes, try to reduce "
+            "this to get a simpler (and so easier to use) class.",
+        ),
+        "R0902": (
+            "Too many instance attributes (%s/%s)",
+            "too-many-instance-attributes",
+            "Used when class has too many instance attributes, try to reduce "
+            "this to get a simpler (and so easier to use) class.",
+        ),
+        "R0903": (
+            "Too few public methods (%s/%s)",
+            "too-few-public-methods",
+            "Used when class has too few public methods, so be sure it's "
+            "really worth it.",
+        ),
+        "R0904": (
+            "Too many public methods (%s/%s)",
+            "too-many-public-methods",
+            "Used when class has too many public methods, try to reduce "
+            "this to get a simpler (and so easier to use) class.",
+        ),
+        "R0911": (
+            "Too many return statements (%s/%s)",
+            "too-many-return-statements",
+            "Used when a function or method has too many return statement, "
+            "making it hard to follow.",
+        ),
+        "R0912": (
+            "Too many branches (%s/%s)",
+            "too-many-branches",
+            "Used when a function or method has too many branches, "
+            "making it hard to follow.",
+        ),
+        "R0913": (
+            "Too many arguments (%s/%s)",
+            "too-many-arguments",
+            "Used when a function or method takes too many arguments.",
+        ),
+        "R0914": (
+            "Too many local variables (%s/%s)",
+            "too-many-locals",
+            "Used when a function or method has too many local variables.",
+        ),
+        "R0915": (
+            "Too many statements (%s/%s)",
+            "too-many-statements",
+            "Used when a function or method has too many statements. You "
+            "should then split it in smaller functions / methods.",
+        ),
+        "R0916": (
+            "Too many boolean expressions in if statement (%s/%s)",
+            "too-many-boolean-expressions",
+            "Used when an if statement contains too many boolean expressions.",
+        ),
+        "R0917": (
+            "Too many positional arguments in a function call.",
+            "too-many-positional",
+            "Will be implemented in https://github.com/pylint-dev/pylint/issues/9099,"
+            "msgid/symbol pair reserved for compatibility with ruff, "
+            "see https://github.com/astral-sh/ruff/issues/8946.",
+        ),
+    }
+)
 SPECIAL_OBJ = re.compile("^_{2}[a-z]+_{2}$")
 DATACLASSES_DECORATORS = frozenset({"dataclass", "attrs"})
 DATACLASS_IMPORT = "dataclasses"
 TYPING_NAMEDTUPLE = "typing.NamedTuple"
 TYPING_TYPEDDICT = "typing.TypedDict"
+TYPING_EXTENSIONS_TYPEDDICT = "typing_extensions.TypedDict"
 
 # Set of stdlib classes to ignore when calculating number of ancestors
 STDLIB_CLASSES_IGNORE_ANCESTOR = frozenset(
     (
         "builtins.object",
         "builtins.tuple",
         "builtins.dict",
@@ -164,26 +172,31 @@
         "typing.ValuesView",
         "typing.ContextManager",
         "typing.AsyncContextManager",
         "typing.Hashable",
         "typing.Sized",
         TYPING_NAMEDTUPLE,
         TYPING_TYPEDDICT,
+        TYPING_EXTENSIONS_TYPEDDICT,
     )
 )
 
 
 def _is_exempt_from_public_methods(node: astroid.ClassDef) -> bool:
     """Check if a class is exempt from too-few-public-methods."""
 
     # If it's a typing.Namedtuple, typing.TypedDict or an Enum
     for ancestor in node.ancestors():
         if is_enum(ancestor):
             return True
-        if ancestor.qname() in (TYPING_NAMEDTUPLE, TYPING_TYPEDDICT):
+        if ancestor.qname() in (
+            TYPING_NAMEDTUPLE,
+            TYPING_TYPEDDICT,
+            TYPING_EXTENSIONS_TYPEDDICT,
+        ):
             return True
 
     # Or if it's a dataclass
     if not node.decorators:
         return False
 
     root_locals = set(node.root().locals)
```

### Comparing `pylint-3.0.4/pylint/checkers/dunder_methods.py` & `pylint-3.1.0/pylint/checkers/dunder_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     Additionally, we exclude classes that are not instantiated since these
     might be used to access the dunder methods of a base class of an instance.
     We also exclude dunder method calls on super() since
     these can't be written in an alternative manner.
     """
 
     name = "unnecessary-dunder-call"
-    priority = -1
     msgs = {
         "C2801": (
             "Unnecessarily calls dunder method %s. %s.",
             "unnecessary-dunder-call",
             "Used when a dunder method is manually called instead "
             "of using the corresponding function/method/operator.",
         ),
```

### Comparing `pylint-3.0.4/pylint/checkers/ellipsis_checker.py` & `pylint-3.1.0/pylint/checkers/ellipsis_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/exceptions.py` & `pylint-3.1.0/pylint/checkers/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,14 +563,18 @@
         "broad-exception-caught",
         "try-except-raise",
         "binary-op-exception",
         "bad-except-order",
         "catching-non-exception",
         "duplicate-except",
     )
+    def visit_trystar(self, node: nodes.TryStar) -> None:
+        """Check for empty except*."""
+        self.visit_try(node)
+
     def visit_try(self, node: nodes.Try) -> None:
         """Check for empty except."""
         self._check_try_except_raise(node)
         exceptions_classes: list[Any] = []
         nb_handlers = len(node.handlers)
         for index, handler in enumerate(node.handlers):
             if handler.type is None:
```

### Comparing `pylint-3.0.4/pylint/checkers/format.py` & `pylint-3.1.0/pylint/checkers/format.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/imports.py` & `pylint-3.1.0/pylint/checkers/imports.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     get_import_name,
     in_type_checking_block,
     is_from_fallback_block,
     is_module_ignored,
     is_sys_guard,
     node_ignores_exception,
 )
+from pylint.constants import MAX_NUMBER_OF_IMPORT_SHOWN
 from pylint.exceptions import EmptyReportError
 from pylint.graph import DotBackend, get_cycles
 from pylint.interfaces import HIGH
 from pylint.reporters.ureports.nodes import Paragraph, Section, VerbatimText
 from pylint.typing import MessageDefinitionTuple
 from pylint.utils import IsortDriver
 from pylint.utils.linterstats import LinterStats
@@ -443,17 +444,17 @@
     )
 
     def __init__(self, linter: PyLinter) -> None:
         BaseChecker.__init__(self, linter)
         self.import_graph: defaultdict[str, set[str]] = defaultdict(set)
         self._imports_stack: list[tuple[ImportNode, str]] = []
         self._first_non_import_node = None
-        self._module_pkg: dict[
-            Any, Any
-        ] = {}  # mapping of modules to the pkg they belong in
+        self._module_pkg: dict[Any, Any] = (
+            {}
+        )  # mapping of modules to the pkg they belong in
         self._allow_any_import_level: set[Any] = set()
         self.reports = (
             ("RP0401", "External dependencies", self._report_external_dependencies),
             ("RP0402", "Modules dependencies graph", self._report_dependencies_graph),
         )
         self._excluded_edges: defaultdict[str, set[str]] = defaultdict(set)
 
@@ -607,21 +608,23 @@
             met.add(package)
 
         self._imports_stack = []
         self._first_non_import_node = None
 
     def compute_first_non_import_node(
         self,
-        node: nodes.If
-        | nodes.Expr
-        | nodes.Comprehension
-        | nodes.IfExp
-        | nodes.Assign
-        | nodes.AssignAttr
-        | nodes.Try,
+        node: (
+            nodes.If
+            | nodes.Expr
+            | nodes.Comprehension
+            | nodes.IfExp
+            | nodes.Assign
+            | nodes.AssignAttr
+            | nodes.Try
+        ),
     ) -> None:
         # if the node does not contain an import instruction, and if it is the
         # first node of the module, keep a track of it (all the import positions
         # of the module will be compared to the position of this first
         # instruction)
         if self._first_non_import_node:
             return
@@ -640,21 +643,17 @@
                 and target.name.endswith("__")
                 for target in node.targets
             ]
             if all(valid_targets):
                 return
         self._first_non_import_node = node
 
-    visit_try = (
-        visit_assignattr
-    ) = (
-        visit_assign
-    ) = (
-        visit_ifexp
-    ) = visit_comprehension = visit_expr = visit_if = compute_first_non_import_node
+    visit_try = visit_assignattr = visit_assign = visit_ifexp = visit_comprehension = (
+        visit_expr
+    ) = visit_if = compute_first_non_import_node
 
     def visit_functiondef(
         self, node: nodes.FunctionDef | nodes.While | nodes.For | nodes.ClassDef
     ) -> None:
         # If it is the first non import instruction of the module, record it.
         if self._first_non_import_node:
             return
@@ -745,17 +744,15 @@
     def _is_fallback_import(
         node: ImportNode, imports: list[tuple[ImportNode, str]]
     ) -> bool:
         imports = [import_node for (import_node, _) in imports]
         return any(astroid.are_exclusive(import_node, node) for import_node in imports)
 
     # pylint: disable = too-many-statements
-    def _check_imports_order(
-        self, _module_node: nodes.Module
-    ) -> tuple[
+    def _check_imports_order(self, _module_node: nodes.Module) -> tuple[
         list[tuple[ImportNode, str]],
         list[tuple[ImportNode, str]],
         list[tuple[ImportNode, str]],
     ]:
         """Checks imports of module `node` are grouped by category.
 
         Imports must follow this order: standard, 3rd party, local
@@ -777,30 +774,35 @@
                 package = modname.split(".")[0]
             nested = not isinstance(node.parent, nodes.Module)
             ignore_for_import_order = not self.linter.is_message_enabled(
                 "wrong-import-order", node.fromlineno
             )
             import_category = isort_driver.place_module(package)
             node_and_package_import = (node, package)
+
             if import_category in {"FUTURE", "STDLIB"}:
                 std_imports.append(node_and_package_import)
                 wrong_import = (
                     third_party_not_ignored
                     or first_party_not_ignored
                     or local_not_ignored
                 )
                 if self._is_fallback_import(node, wrong_import):
                     continue
                 if wrong_import and not nested:
                     self.add_message(
                         "wrong-import-order",
                         node=node,
-                        args=(
-                            f'standard import "{node.as_string()}"',
-                            f'"{wrong_import[0][0].as_string()}"',
+                        args=(  ## TODO - this isn't right for multiple on the same line...
+                            f'standard import "{self._get_full_import_name((node, package))}"',
+                            self._get_out_of_order_string(
+                                third_party_not_ignored,
+                                first_party_not_ignored,
+                                local_not_ignored,
+                            ),
                         ),
                     )
             elif import_category == "THIRDPARTY":
                 third_party_imports.append(node_and_package_import)
                 external_imports.append(node_and_package_import)
                 if not nested:
                     if not ignore_for_import_order:
@@ -811,16 +813,18 @@
                         )
                 wrong_import = first_party_not_ignored or local_not_ignored
                 if wrong_import and not nested:
                     self.add_message(
                         "wrong-import-order",
                         node=node,
                         args=(
-                            f'third party import "{node.as_string()}"',
-                            f'"{wrong_import[0][0].as_string()}"',
+                            f'third party import "{self._get_full_import_name((node, package))}"',
+                            self._get_out_of_order_string(
+                                None, first_party_not_ignored, local_not_ignored
+                            ),
                         ),
                     )
             elif import_category == "FIRSTPARTY":
                 first_party_imports.append(node_and_package_import)
                 external_imports.append(node_and_package_import)
                 if not nested:
                     if not ignore_for_import_order:
@@ -831,29 +835,182 @@
                         )
                 wrong_import = local_not_ignored
                 if wrong_import and not nested:
                     self.add_message(
                         "wrong-import-order",
                         node=node,
                         args=(
-                            f'first party import "{node.as_string()}"',
-                            f'"{wrong_import[0][0].as_string()}"',
+                            f'first party import "{self._get_full_import_name((node, package))}"',
+                            self._get_out_of_order_string(
+                                None, None, local_not_ignored
+                            ),
                         ),
                     )
             elif import_category == "LOCALFOLDER":
                 local_imports.append((node, package))
                 if not nested:
                     if not ignore_for_import_order:
                         local_not_ignored.append((node, package))
                     else:
                         self.linter.add_ignored_message(
                             "wrong-import-order", node.fromlineno, node
                         )
         return std_imports, external_imports, local_imports
 
+    def _get_out_of_order_string(
+        self,
+        third_party_imports: list[tuple[ImportNode, str]] | None,
+        first_party_imports: list[tuple[ImportNode, str]] | None,
+        local_imports: list[tuple[ImportNode, str]] | None,
+    ) -> str:
+        # construct the string listing out of order imports used in the message
+        # for wrong-import-order
+        if third_party_imports:
+            plural = "s" if len(third_party_imports) > 1 else ""
+            if len(third_party_imports) > MAX_NUMBER_OF_IMPORT_SHOWN:
+                imports_list = (
+                    ", ".join(
+                        [
+                            f'"{self._get_full_import_name(tpi)}"'
+                            for tpi in third_party_imports[
+                                : int(MAX_NUMBER_OF_IMPORT_SHOWN // 2)
+                            ]
+                        ]
+                    )
+                    + " (...) "
+                    + ", ".join(
+                        [
+                            f'"{self._get_full_import_name(tpi)}"'
+                            for tpi in third_party_imports[
+                                int(-MAX_NUMBER_OF_IMPORT_SHOWN // 2) :
+                            ]
+                        ]
+                    )
+                )
+            else:
+                imports_list = ", ".join(
+                    [
+                        f'"{self._get_full_import_name(tpi)}"'
+                        for tpi in third_party_imports
+                    ]
+                )
+            third_party = f"third party import{plural} {imports_list}"
+        else:
+            third_party = ""
+
+        if first_party_imports:
+            plural = "s" if len(first_party_imports) > 1 else ""
+            if len(first_party_imports) > MAX_NUMBER_OF_IMPORT_SHOWN:
+                imports_list = (
+                    ", ".join(
+                        [
+                            f'"{self._get_full_import_name(tpi)}"'
+                            for tpi in first_party_imports[
+                                : int(MAX_NUMBER_OF_IMPORT_SHOWN // 2)
+                            ]
+                        ]
+                    )
+                    + " (...) "
+                    + ", ".join(
+                        [
+                            f'"{self._get_full_import_name(tpi)}"'
+                            for tpi in first_party_imports[
+                                int(-MAX_NUMBER_OF_IMPORT_SHOWN // 2) :
+                            ]
+                        ]
+                    )
+                )
+            else:
+                imports_list = ", ".join(
+                    [
+                        f'"{self._get_full_import_name(fpi)}"'
+                        for fpi in first_party_imports
+                    ]
+                )
+            first_party = f"first party import{plural} {imports_list}"
+        else:
+            first_party = ""
+
+        if local_imports:
+            plural = "s" if len(local_imports) > 1 else ""
+            if len(local_imports) > MAX_NUMBER_OF_IMPORT_SHOWN:
+                imports_list = (
+                    ", ".join(
+                        [
+                            f'"{self._get_full_import_name(tpi)}"'
+                            for tpi in local_imports[
+                                : int(MAX_NUMBER_OF_IMPORT_SHOWN // 2)
+                            ]
+                        ]
+                    )
+                    + " (...) "
+                    + ", ".join(
+                        [
+                            f'"{self._get_full_import_name(tpi)}"'
+                            for tpi in local_imports[
+                                int(-MAX_NUMBER_OF_IMPORT_SHOWN // 2) :
+                            ]
+                        ]
+                    )
+                )
+            else:
+                imports_list = ", ".join(
+                    [f'"{self._get_full_import_name(li)}"' for li in local_imports]
+                )
+            local = f"local import{plural} {imports_list}"
+        else:
+            local = ""
+
+        delimiter_third_party = (
+            (
+                ", "
+                if (first_party and local)
+                else (" and " if (first_party or local) else "")
+            )
+            if third_party
+            else ""
+        )
+        delimiter_first_party1 = (
+            (", " if (third_party and local) else " ") if first_party else ""
+        )
+        delimiter_first_party2 = ("and " if local else "") if first_party else ""
+        delimiter_first_party = f"{delimiter_first_party1}{delimiter_first_party2}"
+        msg = (
+            f"{third_party}{delimiter_third_party}"
+            f"{first_party}{delimiter_first_party}"
+            f'{local if local else ""}'
+        )
+
+        return msg
+
+    def _get_full_import_name(self, importNode: ImportNode) -> str:
+        # construct a more descriptive name of the import
+        # for: import X, this returns X
+        # for: import X.Y this returns X.Y
+        # for: from X import Y, this returns X.Y
+
+        try:
+            # this will only succeed for ImportFrom nodes, which in themselves
+            # contain the information needed to reconstruct the package
+            return f"{importNode[0].modname}.{importNode[0].names[0][0]}"
+        except AttributeError:
+            # in all other cases, the import will either be X or X.Y
+            node: str = importNode[0].names[0][0]
+            package: str = importNode[1]
+
+            if node.split(".")[0] == package:
+                # this is sufficient with one import per line, since package = X
+                # and node = X.Y or X
+                return node
+
+            # when there is a node that contains multiple imports, the "current"
+            # import being analyzed is specified by package (node is the first
+            # import on the line and therefore != package in this case)
+            return package
+
     def _get_imported_module(
         self, importnode: ImportNode, modname: str
     ) -> nodes.Module | None:
         try:
             return importnode.do_import_module(modname)
         except astroid.TooManyLevelsError:
             if _ignore_import_failure(importnode, modname, self._ignored_modules):
@@ -1077,17 +1234,19 @@
         """Check whether the import is made outside the module toplevel."""
         # If the scope of the import is a module, then obviously it is
         # not outside the module toplevel.
         if isinstance(node.scope(), nodes.Module):
             return
 
         module_names = [
-            f"{node.modname}.{name[0]}"
-            if isinstance(node, nodes.ImportFrom)
-            else name[0]
+            (
+                f"{node.modname}.{name[0]}"
+                if isinstance(node, nodes.ImportFrom)
+                else name[0]
+            )
             for name in node.names
         ]
 
         # Get the full names of all the imports that are only allowed at the module level
         scoped_imports = [
             name for name in module_names if name not in self._allow_any_import_level
         ]
```

### Comparing `pylint-3.0.4/pylint/checkers/lambda_expressions.py` & `pylint-3.1.0/pylint/checkers/lambda_expressions.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/logging.py` & `pylint-3.1.0/pylint/checkers/logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,79 +17,79 @@
 from pylint.checkers import utils
 from pylint.checkers.utils import infer_all
 from pylint.typing import MessageDefinitionTuple
 
 if TYPE_CHECKING:
     from pylint.lint import PyLinter
 
-MSGS: dict[
-    str, MessageDefinitionTuple
-] = {  # pylint: disable=consider-using-namedtuple-or-dataclass
-    "W1201": (
-        "Use %s formatting in logging functions",
-        "logging-not-lazy",
-        "Used when a logging statement has a call form of "
-        '"logging.<logging method>(format_string % (format_args...))". '
-        "Use another type of string formatting instead. "
-        "You can use % formatting but leave interpolation to "
-        "the logging function by passing the parameters as arguments. "
-        "If logging-fstring-interpolation is disabled then "
-        "you can use fstring formatting. "
-        "If logging-format-interpolation is disabled then "
-        "you can use str.format.",
-    ),
-    "W1202": (
-        "Use %s formatting in logging functions",
-        "logging-format-interpolation",
-        "Used when a logging statement has a call form of "
-        '"logging.<logging method>(format_string.format(format_args...))". '
-        "Use another type of string formatting instead. "
-        "You can use % formatting but leave interpolation to "
-        "the logging function by passing the parameters as arguments. "
-        "If logging-fstring-interpolation is disabled then "
-        "you can use fstring formatting. "
-        "If logging-not-lazy is disabled then "
-        "you can use % formatting as normal.",
-    ),
-    "W1203": (
-        "Use %s formatting in logging functions",
-        "logging-fstring-interpolation",
-        "Used when a logging statement has a call form of "
-        '"logging.<logging method>(f"...")".'
-        "Use another type of string formatting instead. "
-        "You can use % formatting but leave interpolation to "
-        "the logging function by passing the parameters as arguments. "
-        "If logging-format-interpolation is disabled then "
-        "you can use str.format. "
-        "If logging-not-lazy is disabled then "
-        "you can use % formatting as normal.",
-    ),
-    "E1200": (
-        "Unsupported logging format character %r (%#02x) at index %d",
-        "logging-unsupported-format",
-        "Used when an unsupported format character is used in a logging "
-        "statement format string.",
-    ),
-    "E1201": (
-        "Logging format string ends in middle of conversion specifier",
-        "logging-format-truncated",
-        "Used when a logging statement format string terminates before "
-        "the end of a conversion specifier.",
-    ),
-    "E1205": (
-        "Too many arguments for logging format string",
-        "logging-too-many-args",
-        "Used when a logging format string is given too many arguments.",
-    ),
-    "E1206": (
-        "Not enough arguments for logging format string",
-        "logging-too-few-args",
-        "Used when a logging format string is given too few arguments.",
-    ),
-}
+MSGS: dict[str, MessageDefinitionTuple] = (
+    {  # pylint: disable=consider-using-namedtuple-or-dataclass
+        "W1201": (
+            "Use %s formatting in logging functions",
+            "logging-not-lazy",
+            "Used when a logging statement has a call form of "
+            '"logging.<logging method>(format_string % (format_args...))". '
+            "Use another type of string formatting instead. "
+            "You can use % formatting but leave interpolation to "
+            "the logging function by passing the parameters as arguments. "
+            "If logging-fstring-interpolation is disabled then "
+            "you can use fstring formatting. "
+            "If logging-format-interpolation is disabled then "
+            "you can use str.format.",
+        ),
+        "W1202": (
+            "Use %s formatting in logging functions",
+            "logging-format-interpolation",
+            "Used when a logging statement has a call form of "
+            '"logging.<logging method>(format_string.format(format_args...))". '
+            "Use another type of string formatting instead. "
+            "You can use % formatting but leave interpolation to "
+            "the logging function by passing the parameters as arguments. "
+            "If logging-fstring-interpolation is disabled then "
+            "you can use fstring formatting. "
+            "If logging-not-lazy is disabled then "
+            "you can use % formatting as normal.",
+        ),
+        "W1203": (
+            "Use %s formatting in logging functions",
+            "logging-fstring-interpolation",
+            "Used when a logging statement has a call form of "
+            '"logging.<logging method>(f"...")".'
+            "Use another type of string formatting instead. "
+            "You can use % formatting but leave interpolation to "
+            "the logging function by passing the parameters as arguments. "
+            "If logging-format-interpolation is disabled then "
+            "you can use str.format. "
+            "If logging-not-lazy is disabled then "
+            "you can use % formatting as normal.",
+        ),
+        "E1200": (
+            "Unsupported logging format character %r (%#02x) at index %d",
+            "logging-unsupported-format",
+            "Used when an unsupported format character is used in a logging "
+            "statement format string.",
+        ),
+        "E1201": (
+            "Logging format string ends in middle of conversion specifier",
+            "logging-format-truncated",
+            "Used when a logging statement format string terminates before "
+            "the end of a conversion specifier.",
+        ),
+        "E1205": (
+            "Too many arguments for logging format string",
+            "logging-too-many-args",
+            "Used when a logging format string is given too many arguments.",
+        ),
+        "E1206": (
+            "Not enough arguments for logging format string",
+            "logging-too-few-args",
+            "Used when a logging format string is given too few arguments.",
+        ),
+    }
+)
 
 
 CHECKED_CONVENIENCE_FUNCTIONS = {
     "critical",
     "debug",
     "error",
     "exception",
```

### Comparing `pylint-3.0.4/pylint/checkers/method_args.py` & `pylint-3.1.0/pylint/checkers/method_args.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/misc.py` & `pylint-3.1.0/pylint/checkers/misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from pylint.typing import ManagedMessage
 
 if TYPE_CHECKING:
     from pylint.lint import PyLinter
 
 
 class ByIdManagedMessagesChecker(BaseRawFileChecker):
-
     """Checks for messages that are enabled or disabled by id instead of symbol."""
 
     name = "miscellaneous"
     msgs = {
         "I0023": (
             "%s",
             "use-symbolic-message-instead",
@@ -48,15 +47,14 @@
                 verb = "disable" if is_disabled else "enable"
                 txt = f"'{msgid}' is cryptic: use '# pylint: {verb}={symbol}' instead"
                 self.add_message("use-symbolic-message-instead", line=lineno, args=txt)
         self._clear_by_id_managed_msgs()
 
 
 class EncodingChecker(BaseTokenChecker, BaseRawFileChecker):
-
     """BaseChecker for encoding issues.
 
     Checks for:
     * warning notes in the code like FIXME, XXX
     * encoding issues.
     """
```

### Comparing `pylint-3.0.4/pylint/checkers/modified_iterating_checker.py` & `pylint-3.1.0/pylint/checkers/modified_iterating_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from pylint.checkers import utils
 
 if TYPE_CHECKING:
     from pylint.lint import PyLinter
 
 
 _LIST_MODIFIER_METHODS = {"append", "remove"}
-_SET_MODIFIER_METHODS = {"add", "remove"}
+_SET_MODIFIER_METHODS = {"add", "clear", "discard", "pop", "remove"}
 
 
 class ModifiedIterationChecker(checkers.BaseChecker):
     """Checks for modified iterators in for loops iterations.
 
     Currently supports `for` loops for Sets, Dictionaries and Lists.
     """
```

### Comparing `pylint-3.0.4/pylint/checkers/nested_min_max.py` & `pylint-3.1.0/pylint/checkers/nested_min_max.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/newstyle.py` & `pylint-3.1.0/pylint/checkers/newstyle.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/non_ascii_names.py` & `pylint-3.1.0/pylint/checkers/non_ascii_names.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/raw_metrics.py` & `pylint-3.1.0/pylint/checkers/raw_metrics.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/refactoring/__init__.py` & `pylint-3.1.0/pylint/checkers/refactoring/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/refactoring/implicit_booleaness_checker.py` & `pylint-3.1.0/pylint/checkers/refactoring/implicit_booleaness_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/refactoring/not_checker.py` & `pylint-3.1.0/pylint/checkers/refactoring/not_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/refactoring/recommendation_checker.py` & `pylint-3.1.0/pylint/checkers/refactoring/recommendation_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/refactoring/refactoring_checker.py` & `pylint-3.1.0/pylint/checkers/refactoring/refactoring_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -479,14 +479,20 @@
         "R1736": (
             "Unnecessary list index lookup, use '%s' instead",
             "unnecessary-list-index-lookup",
             "Emitted when iterating over an enumeration and accessing the "
             "value by index lookup. "
             "The value can be accessed directly instead.",
         ),
+        "R1737": (
+            "Use 'yield from' directly instead of yielding each element one by one",
+            "use-yield-from",
+            "Yielding directly from the iterator is faster and arguably cleaner code than yielding each element "
+            "one by one in the loop.",
+        ),
     }
     options = (
         (
             "max-nested-blocks",
             {
                 "default": 5,
                 "type": "int",
@@ -502,35 +508,52 @@
                 "metavar": "<members names>",
                 "help": "Complete name of functions that never returns. When checking "
                 "for inconsistent-return-statements if a never returning function is "
                 "called then it will be considered as an explicit return statement "
                 "and no message will be printed.",
             },
         ),
+        (
+            "suggest-join-with-non-empty-separator",
+            {
+                "default": True,
+                "type": "yn",
+                "metavar": "<y or n>",
+                "help": (
+                    "Let 'consider-using-join' be raised when the separator to "
+                    "join on would be non-empty (resulting in expected fixes "
+                    'of the type: ``"- " + "\n- ".join(items)``)'
+                ),
+            },
+        ),
     )
 
     def __init__(self, linter: PyLinter) -> None:
         super().__init__(linter)
         self._return_nodes: dict[str, list[nodes.Return]] = {}
         self._consider_using_with_stack = ConsiderUsingWithStack()
         self._init()
         self._never_returning_functions: set[str] = set()
+        self._suggest_join_with_non_empty_separator: bool = False
 
     def _init(self) -> None:
         self._nested_blocks: list[NodesWithNestedBlocks] = []
         self._elifs: list[tuple[int, int]] = []
         self._reported_swap_nodes: set[nodes.NodeNG] = set()
         self._can_simplify_bool_op: bool = False
         self._consider_using_with_stack.clear_all()
 
     def open(self) -> None:
         # do this in open since config not fully initialized in __init__
         self._never_returning_functions = set(
             self.linter.config.never_returning_functions
         )
+        self._suggest_join_with_non_empty_separator = (
+            self.linter.config.suggest_join_with_non_empty_separator
+        )
 
     @cached_property
     def _dummy_rgx(self) -> Pattern[str]:
         return self.linter.config.dummy_variables_rgx  # type: ignore[no-any-return]
 
     @staticmethod
     def _is_bool_const(node: nodes.Return | nodes.Assign) -> bool:
@@ -844,77 +867,82 @@
         self._check_superfluous_else_return(node)
         self._check_superfluous_else_raise(node)
         self._check_superfluous_else_break(node)
         self._check_superfluous_else_continue(node)
         self._check_consider_get(node)
         self._check_consider_using_min_max_builtin(node)
 
-    # pylint: disable = too-many-branches
     def _check_consider_using_min_max_builtin(self, node: nodes.If) -> None:
         """Check if the given if node can be refactored as a min/max python builtin."""
+        # This function is written expecting a test condition of form:
+        #  if a < b: # [consider-using-max-builtin]
+        #    a = b
+        #  if a > b: # [consider-using-min-builtin]
+        #    a = b
         if self._is_actual_elif(node) or node.orelse:
             # Not interested in if statements with multiple branches.
             return
 
         if len(node.body) != 1:
             return
 
+        def get_node_name(node: nodes.NodeNG) -> str:
+            """Obtain simplest representation of a node as a string."""
+            if isinstance(node, nodes.Name):
+                return node.name  # type: ignore[no-any-return]
+            if isinstance(node, nodes.Attribute):
+                return node.attrname  # type: ignore[no-any-return]
+            if isinstance(node, nodes.Const):
+                return str(node.value)
+            # this is a catch-all for nodes that are not of type Name or Attribute
+            # extremely helpful for Call or BinOp
+            return node.as_string()  # type: ignore[no-any-return]
+
         body = node.body[0]
         # Check if condition can be reduced.
         if not hasattr(body, "targets") or len(body.targets) != 1:
             return
 
         target = body.targets[0]
         if not (
             isinstance(node.test, nodes.Compare)
             and not isinstance(target, nodes.Subscript)
             and not isinstance(node.test.left, nodes.Subscript)
             and isinstance(body, nodes.Assign)
         ):
             return
-
-        # Check that the assignation is on the same variable.
-        if hasattr(node.test.left, "name"):
-            left_operand = node.test.left.name
-        elif hasattr(node.test.left, "attrname"):
-            left_operand = node.test.left.attrname
-        else:
-            return
+        # Assign body line has one requirement and that is the assign target
+        # is of type name or attribute. Attribute referring to NamedTuple.x perse.
+        # So we have to check that target is of these types
 
         if hasattr(target, "name"):
             target_assignation = target.name
         elif hasattr(target, "attrname"):
             target_assignation = target.attrname
         else:
             return
 
-        if not (left_operand == target_assignation):
-            return
-
         if len(node.test.ops) > 1:
             return
-
-        if not isinstance(body.value, (nodes.Name, nodes.Const)):
-            return
-
         operator, right_statement = node.test.ops[0]
-        if isinstance(body.value, nodes.Name):
-            body_value = body.value.name
-        else:
-            body_value = body.value.value
 
-        if isinstance(right_statement, nodes.Name):
-            right_statement_value = right_statement.name
-        elif isinstance(right_statement, nodes.Const):
-            right_statement_value = right_statement.value
+        body_value = get_node_name(body.value)
+        left_operand = get_node_name(node.test.left)
+        right_statement_value = get_node_name(right_statement)
+
+        if left_operand == target_assignation:
+            # statement is in expected form
+            pass
+        elif right_statement_value == target_assignation:
+            # statement is in reverse form
+            operator = utils.get_inverse_comparator(operator)
         else:
             return
 
-        # Verify the right part of the statement is the same.
-        if right_statement_value != body_value:
+        if body_value not in (right_statement_value, left_operand):
             return
 
         if operator in {"<", "<="}:
             reduced_to = (
                 f"{target_assignation} = max({target_assignation}, {body_value})"
             )
             self.add_message(
@@ -1102,14 +1130,35 @@
         self._check_quit_exit_call(node)
         self._check_super_with_arguments(node)
         self._check_consider_using_generator(node)
         self._check_consider_using_with(node)
         self._check_use_list_literal(node)
         self._check_use_dict_literal(node)
 
+    @utils.only_required_for_messages("use-yield-from")
+    def visit_yield(self, node: nodes.Yield) -> None:
+        if not isinstance(node.value, nodes.Name):
+            return
+
+        parent = node.parent.parent
+        if (
+            not isinstance(parent, nodes.For)
+            or isinstance(parent, nodes.AsyncFor)
+            or len(parent.body) != 1
+        ):
+            return
+
+        if parent.target.name != node.value.name:
+            return
+
+        if isinstance(node.frame(), nodes.AsyncFunctionDef):
+            return
+
+        self.add_message("use-yield-from", node=parent, confidence=HIGH)
+
     @staticmethod
     def _has_exit_in_scope(scope: nodes.LocalsDictNodeNG) -> bool:
         exit_func = scope.locals.get("exit")
         return bool(
             exit_func and isinstance(exit_func[0], (nodes.ImportFrom, nodes.Import))
         )
 
@@ -1368,18 +1417,18 @@
                     elif operator in {">", ">="}:
                         if operand is left_operand:
                             uses[value]["upper_bound"].add(comparison_node)
                         elif operand is right_operand:
                             uses[value]["lower_bound"].add(comparison_node)
                 left_operand = right_operand
 
-        uses: collections.defaultdict[
-            str, dict[str, set[nodes.Compare]]
-        ] = collections.defaultdict(
-            lambda: {"lower_bound": set(), "upper_bound": set()}
+        uses: collections.defaultdict[str, dict[str, set[nodes.Compare]]] = (
+            collections.defaultdict(
+                lambda: {"lower_bound": set(), "upper_bound": set()}
+            )
         )
         for comparison_node in node.values:
             if isinstance(comparison_node, nodes.Compare):
                 _find_lower_upper_bounds(comparison_node, uses)
 
         for bounds in uses.values():
             num_shared = len(bounds["lower_bound"].intersection(bounds["upper_bound"]))
@@ -1422,17 +1471,19 @@
         """Attempts to simplify a boolean operation.
 
         Recursively applies simplification on the operator terms,
         and keeps track of whether reductions have been made.
         """
         children = list(bool_op.get_children())
         intermediate = [
-            self._simplify_boolean_operation(child)
-            if isinstance(child, nodes.BoolOp)
-            else child
+            (
+                self._simplify_boolean_operation(child)
+                if isinstance(child, nodes.BoolOp)
+                else child
+            )
             for child in children
         ]
         result = self._apply_boolean_simplification_rules(bool_op.op, intermediate)
         if len(result) < len(children):
             self._can_simplify_bool_op = True
         if len(result) == 1:
             return result[0]
@@ -1663,27 +1714,32 @@
         for keyword in node.kwargs:
             if len(", ".join(elements)) >= 64:
                 break
             elements.append(f"**{keyword.value.as_string()}")
         suggestion = ", ".join(elements)
         return f"{{{suggestion}{', ... '  if len(suggestion) > 64 else ''}}}"
 
-    @staticmethod
-    def _name_to_concatenate(node: nodes.NodeNG) -> str | None:
+    def _name_to_concatenate(self, node: nodes.NodeNG) -> str | None:
         """Try to extract the name used in a concatenation loop."""
         if isinstance(node, nodes.Name):
             return cast("str | None", node.name)
         if not isinstance(node, nodes.JoinedStr):
             return None
 
         values = [
             value for value in node.values if isinstance(value, nodes.FormattedValue)
         ]
         if len(values) != 1 or not isinstance(values[0].value, nodes.Name):
             return None
+        # If there are more values in joined string than formatted values,
+        # they are probably separators.
+        # Allow them only if the option `suggest-join-with-non-empty-separator` is set
+        with_separators = len(node.values) > len(values)
+        if with_separators and not self._suggest_join_with_non_empty_separator:
+            return None
         return cast("str | None", values[0].value.name)
 
     def _check_consider_using_join(self, aug_assign: nodes.AugAssign) -> None:
         """We start with the augmented assignment and work our way upwards.
 
         Names of variables for nodes if match successful:
         result = ''  # assign
```

### Comparing `pylint-3.0.4/pylint/checkers/similar.py` & `pylint-3.1.0/pylint/checkers/similar.py`

 * *Files 1% similar despite different names*

```diff
@@ -389,17 +389,19 @@
             LineSet(
                 streamid,
                 lines,
                 self.namespace.ignore_comments,
                 self.namespace.ignore_docstrings,
                 self.namespace.ignore_imports,
                 self.namespace.ignore_signatures,
-                line_enabled_callback=self.linter._is_one_message_enabled
-                if hasattr(self, "linter")
-                else None,
+                line_enabled_callback=(
+                    self.linter._is_one_message_enabled
+                    if hasattr(self, "linter")
+                    else None
+                ),
             )
         )
 
     def run(self) -> None:
         """Start looking for similarities and display results on stdout."""
         if self.namespace.min_similarity_lines == 0:
             return
@@ -515,20 +517,20 @@
 
         for c_hash in sorted(common_hashes, key=operator.attrgetter("_index")):
             for indices_in_linesets in itertools.product(
                 hash_to_index_1[c_hash], hash_to_index_2[c_hash]
             ):
                 index_1 = indices_in_linesets[0]
                 index_2 = indices_in_linesets[1]
-                all_couples[
-                    LineSetStartCouple(index_1, index_2)
-                ] = CplSuccessiveLinesLimits(
-                    copy.copy(index_to_lines_1[index_1]),
-                    copy.copy(index_to_lines_2[index_2]),
-                    effective_cmn_lines_nb=self.namespace.min_similarity_lines,
+                all_couples[LineSetStartCouple(index_1, index_2)] = (
+                    CplSuccessiveLinesLimits(
+                        copy.copy(index_to_lines_1[index_1]),
+                        copy.copy(index_to_lines_2[index_2]),
+                        effective_cmn_lines_nb=self.namespace.min_similarity_lines,
+                    )
                 )
 
         remove_successive(all_couples)
 
         for cml_stripped_l, cmn_l in all_couples.items():
             start_index_1 = cml_stripped_l.fst_lineset_index
             start_index_2 = cml_stripped_l.snd_lineset_index
```

### Comparing `pylint-3.0.4/pylint/checkers/spelling.py` & `pylint-3.1.0/pylint/checkers/spelling.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,25 +122,27 @@
     r"""Filter skipping over camelCasedWords.
     This filter skips any words matching the following regular expression:
 
            ^([a-z]\w+[A-Z]+\w+)
 
     That is, any words that are camelCasedWords.
     """
+
     _pattern = re.compile(r"^([a-z]+(\d|[A-Z])(?:\w+)?)")
 
 
 class SphinxDirectives(RegExFilter):
     r"""Filter skipping over Sphinx Directives.
     This filter skips any words matching the following regular expression:
 
            ^(:([a-z]+)){1,2}:`([^`]+)(`)?
 
     That is, for example, :class:`BaseQuery`
     """
+
     # The final ` in the pattern is optional because enchant strips it out
     _pattern = re.compile(r"^(:([a-z]+)){1,2}:`([^`]+)(`)?")
 
 
 class ForwardSlashChunker(Chunker):  # type: ignore[misc]
     """This chunker allows splitting words like 'before/after' into 'before' and
     'after'.
@@ -449,18 +451,17 @@
     ) -> None:
         self._check_docstring(node)
 
     visit_asyncfunctiondef = visit_functiondef
 
     def _check_docstring(
         self,
-        node: nodes.FunctionDef
-        | nodes.AsyncFunctionDef
-        | nodes.ClassDef
-        | nodes.Module,
+        node: (
+            nodes.FunctionDef | nodes.AsyncFunctionDef | nodes.ClassDef | nodes.Module
+        ),
     ) -> None:
         """Check if the node has any spelling errors."""
         if not self.initialized:
             return
         if not node.doc_node:
             return
         start_line = node.lineno + 1
```

### Comparing `pylint-3.0.4/pylint/checkers/stdlib.py` & `pylint-3.1.0/pylint/checkers/stdlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,17 @@
         "multiprocessing.managers.SharedMemoryServer.create": (
             (None, "c"),
             (None, "typeid"),
         ),
     },
     (3, 9, 0): {"random.Random.shuffle": ((1, "random"),)},
     (3, 12, 0): {
+        "argparse.BooleanOptionalAction": ((3, "type"), (4, "choices"), (7, "metavar")),
         "coroutine.throw": ((1, "value"), (2, "traceback")),
+        "email.utils.localtime": ((1, "isdst"),),
         "shutil.rmtree": ((2, "onerror"),),
     },
 }
 
 DEPRECATED_DECORATORS: DeprecationDict = {
     (3, 8, 0): {"asyncio.coroutine"},
     (3, 3, 0): {
@@ -224,14 +226,21 @@
             "threading.Thread.isAlive",
         },
         (3, 9, 0): {
             "binascii.b2a_hqx",
             "binascii.a2b_hqx",
             "binascii.rlecode_hqx",
             "binascii.rledecode_hqx",
+            "importlib.resources.contents",
+            "importlib.resources.is_resource",
+            "importlib.resources.open_binary",
+            "importlib.resources.open_text",
+            "importlib.resources.path",
+            "importlib.resources.read_binary",
+            "importlib.resources.read_text",
         },
         (3, 10, 0): {
             "_sqlite3.enable_shared_cache",
             "importlib.abc.Finder.find_module",
             "pathlib.Path.link_to",
             "zipimport.zipimporter.load_module",
             "zipimport.zipimporter.find_module",
@@ -252,19 +261,24 @@
             "re.template",
             "unittest.findTestCases",
             "unittest.makeSuite",
             "unittest.getTestCaseNames",
             "unittest.TestLoader.loadTestsFromModule",
             "unittest.TestLoader.loadTestsFromTestCase",
             "unittest.TestLoader.getTestCaseNames",
+            "unittest.TestProgram.usageExit",
         },
         (3, 12, 0): {
             "builtins.bool.__invert__",
             "datetime.datetime.utcfromtimestamp",
             "datetime.datetime.utcnow",
+            "pkgutil.find_loader",
+            "pkgutil.get_loader",
+            "pty.master_open",
+            "pty.slave_open",
             "xml.etree.ElementTree.Element.__bool__",
         },
     },
 }
 
 
 DEPRECATED_CLASSES: dict[tuple[int, int, int], dict[str, set[str]]] = {
@@ -320,22 +334,58 @@
             "Text",
         },
         "webbrowser": {
             "MacOSX",
         },
     },
     (3, 12, 0): {
+        "ast": {
+            "Bytes",
+            "Ellipsis",
+            "NameConstant",
+            "Num",
+            "Str",
+        },
+        "asyncio": {
+            "AbstractChildWatcher",
+            "MultiLoopChildWatcher",
+            "FastChildWatcher",
+            "SafeChildWatcher",
+        },
+        "collections.abc": {
+            "ByteString",
+        },
+        "importlib.abc": {
+            "ResourceReader",
+            "Traversable",
+            "TraversableResources",
+        },
         "typing": {
+            "ByteString",
             "Hashable",
             "Sized",
         },
     },
 }
 
 
+DEPRECATED_ATTRIBUTES: DeprecationDict = {
+    (3, 2, 0): {
+        "configparser.ParsingError.filename",
+    },
+    (3, 12, 0): {
+        "calendar.January",
+        "calendar.February",
+        "sys.last_traceback",
+        "sys.last_type",
+        "sys.last_value",
+    },
+}
+
+
 def _check_mode_str(mode: Any) -> bool:
     # check type
     if not isinstance(mode, str):
         return False
     # check syntax
     modes = set(mode)
     _mode = "rwatb+Ux"
@@ -366,14 +416,15 @@
     name = "stdlib"
 
     msgs: dict[str, MessageDefinitionTuple] = {
         **DeprecatedMixin.DEPRECATED_METHOD_MESSAGE,
         **DeprecatedMixin.DEPRECATED_ARGUMENT_MESSAGE,
         **DeprecatedMixin.DEPRECATED_CLASS_MESSAGE,
         **DeprecatedMixin.DEPRECATED_DECORATOR_MESSAGE,
+        **DeprecatedMixin.DEPRECATED_ATTRIBUTE_MESSAGE,
         "W1501": (
             '"%s" is not a valid mode for open.',
             "bad-open-mode",
             "Python supports: r, w, a[, x] modes with b, +, "
             "and U (only with r) options. "
             "See https://docs.python.org/3/library/functions.html#open",
         ),
@@ -485,27 +536,31 @@
 
     def __init__(self, linter: PyLinter) -> None:
         BaseChecker.__init__(self, linter)
         self._deprecated_methods: set[str] = set()
         self._deprecated_arguments: dict[str, tuple[tuple[int | None, str], ...]] = {}
         self._deprecated_classes: dict[str, set[str]] = {}
         self._deprecated_decorators: set[str] = set()
+        self._deprecated_attributes: set[str] = set()
 
         for since_vers, func_list in DEPRECATED_METHODS[sys.version_info[0]].items():
             if since_vers <= sys.version_info:
                 self._deprecated_methods.update(func_list)
         for since_vers, args_list in DEPRECATED_ARGUMENTS.items():
             if since_vers <= sys.version_info:
                 self._deprecated_arguments.update(args_list)
         for since_vers, class_list in DEPRECATED_CLASSES.items():
             if since_vers <= sys.version_info:
                 self._deprecated_classes.update(class_list)
         for since_vers, decorator_list in DEPRECATED_DECORATORS.items():
             if since_vers <= sys.version_info:
                 self._deprecated_decorators.update(decorator_list)
+        for since_vers, attribute_list in DEPRECATED_ATTRIBUTES.items():
+            if since_vers <= sys.version_info:
+                self._deprecated_attributes.update(attribute_list)
         # Modules are checked by the ImportsChecker, because the list is
         # synced with the config argument deprecated-modules
 
     def _check_bad_thread_instantiation(self, node: nodes.Call) -> None:
         func_kwargs = {key.arg for key in node.keywords}
         if "target" in func_kwargs:
             return
@@ -864,10 +919,13 @@
 
     def deprecated_classes(self, module: str) -> Iterable[str]:
         return self._deprecated_classes.get(module, ())
 
     def deprecated_decorators(self) -> Iterable[str]:
         return self._deprecated_decorators
 
+    def deprecated_attributes(self) -> Iterable[str]:
+        return self._deprecated_attributes
+
 
 def register(linter: PyLinter) -> None:
     linter.register_checker(StdlibChecker(linter))
```

### Comparing `pylint-3.0.4/pylint/checkers/strings.py` & `pylint-3.1.0/pylint/checkers/strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,144 +61,144 @@
     tokenize.NL,
     tokenize.COMMENT,
 )
 SINGLE_QUOTED_REGEX = re.compile(f"({'|'.join(_PREFIXES)})?'''")
 DOUBLE_QUOTED_REGEX = re.compile(f"({'|'.join(_PREFIXES)})?\"\"\"")
 QUOTE_DELIMITER_REGEX = re.compile(f"({'|'.join(_PREFIXES)})?(\"|')", re.DOTALL)
 
-MSGS: dict[
-    str, MessageDefinitionTuple
-] = {  # pylint: disable=consider-using-namedtuple-or-dataclass
-    "E1300": (
-        "Unsupported format character %r (%#02x) at index %d",
-        "bad-format-character",
-        "Used when an unsupported format character is used in a format string.",
-    ),
-    "E1301": (
-        "Format string ends in middle of conversion specifier",
-        "truncated-format-string",
-        "Used when a format string terminates before the end of a "
-        "conversion specifier.",
-    ),
-    "E1302": (
-        "Mixing named and unnamed conversion specifiers in format string",
-        "mixed-format-string",
-        "Used when a format string contains both named (e.g. '%(foo)d') "
-        "and unnamed (e.g. '%d') conversion specifiers.  This is also "
-        "used when a named conversion specifier contains * for the "
-        "minimum field width and/or precision.",
-    ),
-    "E1303": (
-        "Expected mapping for format string, not %s",
-        "format-needs-mapping",
-        "Used when a format string that uses named conversion specifiers "
-        "is used with an argument that is not a mapping.",
-    ),
-    "W1300": (
-        "Format string dictionary key should be a string, not %s",
-        "bad-format-string-key",
-        "Used when a format string that uses named conversion specifiers "
-        "is used with a dictionary whose keys are not all strings.",
-    ),
-    "W1301": (
-        "Unused key %r in format string dictionary",
-        "unused-format-string-key",
-        "Used when a format string that uses named conversion specifiers "
-        "is used with a dictionary that contains keys not required by the "
-        "format string.",
-    ),
-    "E1304": (
-        "Missing key %r in format string dictionary",
-        "missing-format-string-key",
-        "Used when a format string that uses named conversion specifiers "
-        "is used with a dictionary that doesn't contain all the keys "
-        "required by the format string.",
-    ),
-    "E1305": (
-        "Too many arguments for format string",
-        "too-many-format-args",
-        "Used when a format string that uses unnamed conversion "
-        "specifiers is given too many arguments.",
-    ),
-    "E1306": (
-        "Not enough arguments for format string",
-        "too-few-format-args",
-        "Used when a format string that uses unnamed conversion "
-        "specifiers is given too few arguments",
-    ),
-    "E1307": (
-        "Argument %r does not match format type %r",
-        "bad-string-format-type",
-        "Used when a type required by format string "
-        "is not suitable for actual argument type",
-    ),
-    "E1310": (
-        "Suspicious argument in %s.%s call",
-        "bad-str-strip-call",
-        "The argument to a str.{l,r,}strip call contains a duplicate character,",
-    ),
-    "W1302": (
-        "Invalid format string",
-        "bad-format-string",
-        "Used when a PEP 3101 format string is invalid.",
-    ),
-    "W1303": (
-        "Missing keyword argument %r for format string",
-        "missing-format-argument-key",
-        "Used when a PEP 3101 format string that uses named fields "
-        "doesn't receive one or more required keywords.",
-    ),
-    "W1304": (
-        "Unused format argument %r",
-        "unused-format-string-argument",
-        "Used when a PEP 3101 format string that uses named "
-        "fields is used with an argument that "
-        "is not required by the format string.",
-    ),
-    "W1305": (
-        "Format string contains both automatic field numbering "
-        "and manual field specification",
-        "format-combined-specification",
-        "Used when a PEP 3101 format string contains both automatic "
-        "field numbering (e.g. '{}') and manual field "
-        "specification (e.g. '{0}').",
-    ),
-    "W1306": (
-        "Missing format attribute %r in format specifier %r",
-        "missing-format-attribute",
-        "Used when a PEP 3101 format string uses an "
-        "attribute specifier ({0.length}), but the argument "
-        "passed for formatting doesn't have that attribute.",
-    ),
-    "W1307": (
-        "Using invalid lookup key %r in format specifier %r",
-        "invalid-format-index",
-        "Used when a PEP 3101 format string uses a lookup specifier "
-        "({a[1]}), but the argument passed for formatting "
-        "doesn't contain or doesn't have that key as an attribute.",
-    ),
-    "W1308": (
-        "Duplicate string formatting argument %r, consider passing as named argument",
-        "duplicate-string-formatting-argument",
-        "Used when we detect that a string formatting is "
-        "repeating an argument instead of using named string arguments",
-    ),
-    "W1309": (
-        "Using an f-string that does not have any interpolated variables",
-        "f-string-without-interpolation",
-        "Used when we detect an f-string that does not use any interpolation variables, "
-        "in which case it can be either a normal string or a bug in the code.",
-    ),
-    "W1310": (
-        "Using formatting for a string that does not have any interpolated variables",
-        "format-string-without-interpolation",
-        "Used when we detect a string that does not have any interpolation variables, "
-        "in which case it can be either a normal string without formatting or a bug in the code.",
-    ),
-}
+MSGS: dict[str, MessageDefinitionTuple] = (
+    {  # pylint: disable=consider-using-namedtuple-or-dataclass
+        "E1300": (
+            "Unsupported format character %r (%#02x) at index %d",
+            "bad-format-character",
+            "Used when an unsupported format character is used in a format string.",
+        ),
+        "E1301": (
+            "Format string ends in middle of conversion specifier",
+            "truncated-format-string",
+            "Used when a format string terminates before the end of a "
+            "conversion specifier.",
+        ),
+        "E1302": (
+            "Mixing named and unnamed conversion specifiers in format string",
+            "mixed-format-string",
+            "Used when a format string contains both named (e.g. '%(foo)d') "
+            "and unnamed (e.g. '%d') conversion specifiers.  This is also "
+            "used when a named conversion specifier contains * for the "
+            "minimum field width and/or precision.",
+        ),
+        "E1303": (
+            "Expected mapping for format string, not %s",
+            "format-needs-mapping",
+            "Used when a format string that uses named conversion specifiers "
+            "is used with an argument that is not a mapping.",
+        ),
+        "W1300": (
+            "Format string dictionary key should be a string, not %s",
+            "bad-format-string-key",
+            "Used when a format string that uses named conversion specifiers "
+            "is used with a dictionary whose keys are not all strings.",
+        ),
+        "W1301": (
+            "Unused key %r in format string dictionary",
+            "unused-format-string-key",
+            "Used when a format string that uses named conversion specifiers "
+            "is used with a dictionary that contains keys not required by the "
+            "format string.",
+        ),
+        "E1304": (
+            "Missing key %r in format string dictionary",
+            "missing-format-string-key",
+            "Used when a format string that uses named conversion specifiers "
+            "is used with a dictionary that doesn't contain all the keys "
+            "required by the format string.",
+        ),
+        "E1305": (
+            "Too many arguments for format string",
+            "too-many-format-args",
+            "Used when a format string that uses unnamed conversion "
+            "specifiers is given too many arguments.",
+        ),
+        "E1306": (
+            "Not enough arguments for format string",
+            "too-few-format-args",
+            "Used when a format string that uses unnamed conversion "
+            "specifiers is given too few arguments",
+        ),
+        "E1307": (
+            "Argument %r does not match format type %r",
+            "bad-string-format-type",
+            "Used when a type required by format string "
+            "is not suitable for actual argument type",
+        ),
+        "E1310": (
+            "Suspicious argument in %s.%s call",
+            "bad-str-strip-call",
+            "The argument to a str.{l,r,}strip call contains a duplicate character,",
+        ),
+        "W1302": (
+            "Invalid format string",
+            "bad-format-string",
+            "Used when a PEP 3101 format string is invalid.",
+        ),
+        "W1303": (
+            "Missing keyword argument %r for format string",
+            "missing-format-argument-key",
+            "Used when a PEP 3101 format string that uses named fields "
+            "doesn't receive one or more required keywords.",
+        ),
+        "W1304": (
+            "Unused format argument %r",
+            "unused-format-string-argument",
+            "Used when a PEP 3101 format string that uses named "
+            "fields is used with an argument that "
+            "is not required by the format string.",
+        ),
+        "W1305": (
+            "Format string contains both automatic field numbering "
+            "and manual field specification",
+            "format-combined-specification",
+            "Used when a PEP 3101 format string contains both automatic "
+            "field numbering (e.g. '{}') and manual field "
+            "specification (e.g. '{0}').",
+        ),
+        "W1306": (
+            "Missing format attribute %r in format specifier %r",
+            "missing-format-attribute",
+            "Used when a PEP 3101 format string uses an "
+            "attribute specifier ({0.length}), but the argument "
+            "passed for formatting doesn't have that attribute.",
+        ),
+        "W1307": (
+            "Using invalid lookup key %r in format specifier %r",
+            "invalid-format-index",
+            "Used when a PEP 3101 format string uses a lookup specifier "
+            "({a[1]}), but the argument passed for formatting "
+            "doesn't contain or doesn't have that key as an attribute.",
+        ),
+        "W1308": (
+            "Duplicate string formatting argument %r, consider passing as named argument",
+            "duplicate-string-formatting-argument",
+            "Used when we detect that a string formatting is "
+            "repeating an argument instead of using named string arguments",
+        ),
+        "W1309": (
+            "Using an f-string that does not have any interpolated variables",
+            "f-string-without-interpolation",
+            "Used when we detect an f-string that does not use any interpolation variables, "
+            "in which case it can be either a normal string or a bug in the code.",
+        ),
+        "W1310": (
+            "Using formatting for a string that does not have any interpolated variables",
+            "format-string-without-interpolation",
+            "Used when we detect a string that does not have any interpolation variables, "
+            "in which case it can be either a normal string without formatting or a bug in the code.",
+        ),
+    }
+)
 
 OTHER_NODES = (
     nodes.Const,
     nodes.List,
     nodes.Lambda,
     nodes.FunctionDef,
     nodes.ListComp,
```

### Comparing `pylint-3.0.4/pylint/checkers/threading_checker.py` & `pylint-3.1.0/pylint/checkers/threading_checker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/typecheck.py` & `pylint-3.1.0/pylint/checkers/typecheck.py`

 * *Files 0% similar despite different names*

```diff
@@ -1490,17 +1490,17 @@
             has_no_context_positional_variadic = _no_context_variadic_positional(
                 node, node_scope
             )
             has_no_context_keywords_variadic = _no_context_variadic_keywords(
                 node, node_scope
             )
         else:
-            has_no_context_positional_variadic = (
-                has_no_context_keywords_variadic
-            ) = False
+            has_no_context_positional_variadic = has_no_context_keywords_variadic = (
+                False
+            )
 
         # These are coming from the functools.partial implementation in astroid
         already_filled_positionals = getattr(called, "filled_positionals", 0)
         already_filled_keywords = getattr(called, "filled_keywords", {})
 
         keyword_args += list(already_filled_keywords)
         num_positional_args += implicit_args + already_filled_positionals
```

### Comparing `pylint-3.0.4/pylint/checkers/unicode.py` & `pylint-3.1.0/pylint/checkers/unicode.py`

 * *Files 0% similar despite different names*

```diff
@@ -402,17 +402,17 @@
             # If we can't decode properly, we simply use bytes, even so the column offsets
             # might be wrong a bit, but it is still better then nothing
             line_search_byte = line
             search_dict_byte: dict[bytes, _BadChar] = {}
             for char in BAD_CHARS:
                 # Some characters might not exist in all encodings
                 with contextlib.suppress(UnicodeDecodeError):
-                    search_dict_byte[
-                        _cached_encode_search(char.unescaped, codec)
-                    ] = char
+                    search_dict_byte[_cached_encode_search(char.unescaped, codec)] = (
+                        char
+                    )
 
             return _map_positions_to_result(
                 line_search_byte,
                 search_dict_byte,
                 _cached_encode_search("\n", codec),
                 byte_str_length=_byte_to_str_length(codec),
             )
```

### Comparing `pylint-3.0.4/pylint/checkers/unsupported_version.py` & `pylint-3.1.0/pylint/checkers/unsupported_version.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/utils.py` & `pylint-3.1.0/pylint/checkers/utils.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/checkers/variables.py` & `pylint-3.1.0/pylint/checkers/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from collections import defaultdict
 from collections.abc import Generator, Iterable, Iterator
 from enum import Enum
 from functools import cached_property
 from typing import TYPE_CHECKING, Any, NamedTuple
 
 import astroid
+import astroid.exceptions
 from astroid import bases, extract_node, nodes, util
 from astroid.nodes import _base_nodes
 from astroid.typing import InferenceResult
 
 from pylint.checkers import BaseChecker, utils
 from pylint.checkers.utils import (
     in_type_checking_block,
@@ -136,15 +137,15 @@
     RETURN = 1
 
 
 def _is_from_future_import(stmt: nodes.ImportFrom, name: str) -> bool | None:
     """Check if the name is a future import from another module."""
     try:
         module = stmt.do_import_module(stmt.modname)
-    except astroid.AstroidBuildingException:
+    except astroid.AstroidBuildingError:
         return None
 
     for local_node in module.locals.get(name, []):
         if isinstance(local_node, nodes.ImportFrom) and local_node.modname == FUTURE:
             return True
     return None
 
@@ -1017,17 +1018,17 @@
             else:
                 break
         else:
             print(name)
         """
         if not other_node_try_except.orelse:
             return False
-        closest_loop: None | (
-            nodes.For | nodes.While
-        ) = utils.get_node_first_ancestor_of_type(node, (nodes.For, nodes.While))
+        closest_loop: None | (nodes.For | nodes.While) = (
+            utils.get_node_first_ancestor_of_type(node, (nodes.For, nodes.While))
+        )
         if closest_loop is None:
             return False
         if not any(
             else_statement is node or else_statement.parent_of(node)
             for else_statement in closest_loop.orelse
         ):
             # `node` not guarded by `else`
@@ -2062,15 +2063,15 @@
             return
         if isinstance(node.parent, nodes.If) and is_sys_guard(node.parent):
             return
 
         name_parts = node.modname.split(".")
         try:
             module = node.do_import_module(name_parts[0])
-        except astroid.AstroidBuildingException:
+        except astroid.AstroidBuildingError:
             return
         module = self._check_module_attrs(node, module, name_parts[1:])
         if not module:
             return
         for name, _ in node.names:
             if name == "*":
                 continue
@@ -2527,15 +2528,15 @@
             frame_locals = frame.locals
         return not (
             (isinstance(frame, nodes.ClassDef) or in_annotation_or_default_or_decorator)
             and not self._in_lambda_or_comprehension_body(node, frame)
             and name in frame_locals
         )
 
-    # pylint: disable = too-many-branches
+    # pylint: disable-next=too-many-branches,too-many-statements
     def _loopvar_name(self, node: astroid.Name) -> None:
         # filter variables according to node's scope
         astmts = [s for s in node.lookup(node.name)[1] if hasattr(s, "assign_type")]
         # If this variable usage exists inside a function definition
         # that exists in the same loop,
         # the usage is safe because the function will not be defined either if
         # the variable is not defined.
@@ -2563,16 +2564,20 @@
                 and astmts[0].statement().parent_of(node)
             )
         ):
             _astmts = []
         else:
             _astmts = astmts[:1]
         for i, stmt in enumerate(astmts[1:]):
-            if astmts[i].statement().parent_of(stmt) and not utils.in_for_else_branch(
-                astmts[i].statement(), stmt
+            try:
+                astmt_statement = astmts[i].statement()
+            except astroid.exceptions.ParentMissingError:
+                continue
+            if astmt_statement.parent_of(stmt) and not utils.in_for_else_branch(
+                astmt_statement, stmt
             ):
                 continue
             _astmts.append(stmt)
         astmts = _astmts
         if len(astmts) != 1:
             return
 
@@ -3079,17 +3084,19 @@
         """
         while module_names:
             name = module_names.pop(0)
             if name == "__dict__":
                 module = None
                 break
             try:
-                module = next(module.getattr(name)[0].infer())
+                module = module.getattr(name)[0]
                 if not isinstance(module, nodes.Module):
-                    return None
+                    module = next(module.infer())
+                    if not isinstance(module, nodes.Module):
+                        return None
             except astroid.NotFoundError:
                 # Unable to import `name` from `module`. Since `name` may itself be a
                 # module, we first check if it matches the ignored modules.
                 if is_module_ignored(f"{module.qname()}.{name}", self._ignored_modules):
                     return None
                 self.add_message(
                     "no-name-in-module", args=(name, module.name), node=node
```

### Comparing `pylint-3.0.4/pylint/config/_pylint_config/__init__.py` & `pylint-3.1.0/pylint/config/_pylint_config/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/_pylint_config/generate_command.py` & `pylint-3.1.0/pylint/config/_pylint_config/generate_command.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/_pylint_config/help_message.py` & `pylint-3.1.0/pylint/config/_pylint_config/help_message.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/_pylint_config/main.py` & `pylint-3.1.0/pylint/config/_pylint_config/main.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/_pylint_config/setup.py` & `pylint-3.1.0/pylint/config/_pylint_config/setup.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/_pylint_config/utils.py` & `pylint-3.1.0/pylint/config/_pylint_config/utils.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/argument.py` & `pylint-3.1.0/pylint/config/argument.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/arguments_manager.py` & `pylint-3.1.0/pylint/config/arguments_manager.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/arguments_provider.py` & `pylint-3.1.0/pylint/config/arguments_provider.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/callback_actions.py` & `pylint-3.1.0/pylint/config/callback_actions.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/config_file_parser.py` & `pylint-3.1.0/pylint/config/config_file_parser.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/config_initialization.py` & `pylint-3.1.0/pylint/config/config_initialization.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/deprecation_actions.py` & `pylint-3.1.0/pylint/config/deprecation_actions.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/exceptions.py` & `pylint-3.1.0/pylint/config/exceptions.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/find_default_config_files.py` & `pylint-3.1.0/pylint/config/find_default_config_files.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,20 @@
 from pathlib import Path
 
 if sys.version_info >= (3, 11):
     import tomllib
 else:
     import tomli as tomllib
 
-RC_NAMES = (Path("pylintrc"), Path(".pylintrc"))
+RC_NAMES = (
+    Path("pylintrc"),
+    Path("pylintrc.toml"),
+    Path(".pylintrc"),
+    Path(".pylintrc.toml"),
+)
 PYPROJECT_NAME = Path("pyproject.toml")
 CONFIG_NAMES = (*RC_NAMES, PYPROJECT_NAME, Path("setup.cfg"))
 
 
 def _find_pyproject() -> Path:
     """Search for file pyproject.toml in the parent directories recursively.
```

### Comparing `pylint-3.0.4/pylint/config/help_formatter.py` & `pylint-3.1.0/pylint/config/help_formatter.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/config/utils.py` & `pylint-3.1.0/pylint/config/utils.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/constants.py` & `pylint-3.1.0/pylint/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,7 +270,9 @@
     "__ipow__",
     "__ilshift__",
     "__irshift__",
     "__iand__",
     "__ixor__",
     "__ior__",
 ]
+
+MAX_NUMBER_OF_IMPORT_SHOWN = 6
```

### Comparing `pylint-3.0.4/pylint/exceptions.py` & `pylint-3.1.0/pylint/exceptions.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/__init__.py` & `pylint-3.1.0/pylint/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/_check_docs_utils.py` & `pylint-3.1.0/pylint/extensions/_check_docs_utils.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/bad_builtin.py` & `pylint-3.1.0/pylint/extensions/bad_builtin.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/broad_try_clause.py` & `pylint-3.1.0/pylint/extensions/broad_try_clause.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/check_elif.py` & `pylint-3.1.0/pylint/extensions/check_elif.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/code_style.py` & `pylint-3.1.0/pylint/extensions/code_style.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/comparison_placement.py` & `pylint-3.1.0/pylint/extensions/comparison_placement.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/confusing_elif.py` & `pylint-3.1.0/pylint/extensions/confusing_elif.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/consider_refactoring_into_while_condition.py` & `pylint-3.1.0/pylint/extensions/consider_refactoring_into_while_condition.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/consider_ternary_expression.py` & `pylint-3.1.0/pylint/extensions/consider_ternary_expression.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/dict_init_mutate.py` & `pylint-3.1.0/pylint/extensions/dict_init_mutate.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/docparams.py` & `pylint-3.1.0/pylint/extensions/docparams.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/docstyle.py` & `pylint-3.1.0/pylint/extensions/docstyle.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/dunder.py` & `pylint-3.1.0/pylint/extensions/dunder.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
     from pylint.lint import PyLinter
 
 
 class DunderChecker(BaseChecker):
     """Checks related to dunder methods."""
 
     name = "dunder"
-    priority = -1
     msgs = {
         "W3201": (
             "Bad or misspelled dunder method name %s.",
             "bad-dunder-name",
             "Used when a dunder method is misspelled or defined with a name "
             "not within the predefined list of dunder names.",
         ),
```

### Comparing `pylint-3.0.4/pylint/extensions/empty_comment.py` & `pylint-3.1.0/pylint/extensions/empty_comment.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/eq_without_hash.py` & `pylint-3.1.0/pylint/extensions/eq_without_hash.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/for_any_all.py` & `pylint-3.1.0/pylint/extensions/for_any_all.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/magic_value.py` & `pylint-3.1.0/pylint/extensions/magic_value.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/mccabe.py` & `pylint-3.1.0/pylint/extensions/mccabe.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,35 +90,17 @@
             self.reset()
 
     visitAsyncFunctionDef = visitFunctionDef
 
     def visitSimpleStatement(self, node: _StatementNodes) -> None:
         self._append_node(node)
 
-    visitAssert = (
-        visitAssign
-    ) = (
-        visitAugAssign
-    ) = (
-        visitDelete
-    ) = (
-        visitRaise
-    ) = (
+    visitAssert = visitAssign = visitAugAssign = visitDelete = visitRaise = (
         visitYield
-    ) = (
-        visitImport
-    ) = (
-        visitCall
-    ) = (
-        visitSubscript
-    ) = (
-        visitPass
-    ) = (
-        visitContinue
-    ) = (
+    ) = visitImport = visitCall = visitSubscript = visitPass = visitContinue = (
         visitBreak
     ) = visitGlobal = visitReturn = visitExpr = visitAwait = visitSimpleStatement
 
     def visitWith(self, node: nodes.With) -> None:
         self._append_node(node)
         self.dispatch_list(node.body)
```

### Comparing `pylint-3.0.4/pylint/extensions/no_self_use.py` & `pylint-3.1.0/pylint/extensions/no_self_use.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/overlapping_exceptions.py` & `pylint-3.1.0/pylint/extensions/overlapping_exceptions.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/private_import.py` & `pylint-3.1.0/pylint/extensions/private_import.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,17 +162,17 @@
                     )
                 if isinstance(usage_node, nodes.LocalsDictNodeNG):
                     self._populate_type_annotations(
                         usage_node, all_used_type_annotations
                     )
             if private_name is not None:
                 # Found a new private annotation, make sure we are not accessing it elsewhere
-                all_used_type_annotations[
-                    private_name
-                ] = self._assignments_call_private_name(name_assignments, private_name)
+                all_used_type_annotations[private_name] = (
+                    self._assignments_call_private_name(name_assignments, private_name)
+                )
 
     def _populate_type_annotations_function(
         self, node: nodes.FunctionDef, all_used_type_annotations: dict[str, bool]
     ) -> None:
         """Adds all names used as type annotation in the arguments and return type of
         the function node into the dict `all_used_type_annotations`.
         """
```

### Comparing `pylint-3.0.4/pylint/extensions/redefined_loop_name.py` & `pylint-3.1.0/pylint/extensions/redefined_loop_name.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/redefined_variable_type.py` & `pylint-3.1.0/pylint/extensions/redefined_variable_type.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/set_membership.py` & `pylint-3.1.0/pylint/extensions/set_membership.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/typing.py` & `pylint-3.1.0/pylint/extensions/typing.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/extensions/while_used.py` & `pylint-3.1.0/pylint/extensions/while_used.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/graph.py` & `pylint-3.1.0/pylint/graph.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/interfaces.py` & `pylint-3.1.0/pylint/interfaces.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/lint/__init__.py` & `pylint-3.1.0/pylint/lint/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/lint/base_options.py` & `pylint-3.1.0/pylint/lint/base_options.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/lint/caching.py` & `pylint-3.1.0/pylint/lint/caching.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/lint/expand_modules.py` & `pylint-3.1.0/pylint/lint/expand_modules.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/lint/message_state_handler.py` & `pylint-3.1.0/pylint/lint/message_state_handler.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/lint/parallel.py` & `pylint-3.1.0/pylint/lint/parallel.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,17 +139,17 @@
         _worker_initialize, extra_packages_paths=extra_packages_paths
     )
     with ProcessPoolExecutor(
         max_workers=jobs, initializer=initializer, initargs=(dill.dumps(linter),)
     ) as executor:
         linter.open()
         all_stats = []
-        all_mapreduce_data: defaultdict[
-            int, list[defaultdict[str, list[Any]]]
-        ] = defaultdict(list)
+        all_mapreduce_data: defaultdict[int, list[defaultdict[str, list[Any]]]] = (
+            defaultdict(list)
+        )
 
         # Maps each file to be worked on by a single _worker_check_single_file() call,
         # collecting any map/reduce data by checker module so that we can 'reduce' it
         # later.
         for (
             worker_idx,  # used to merge map/reduce data across workers
             module,
```

### Comparing `pylint-3.0.4/pylint/lint/pylinter.py` & `pylint-3.1.0/pylint/lint/pylinter.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,15 @@
 
 MANAGER = astroid.MANAGER
 
 
 class GetAstProtocol(Protocol):
     def __call__(
         self, filepath: str, modname: str, data: str | None = None
-    ) -> nodes.Module:
-        ...
+    ) -> nodes.Module: ...
 
 
 def _read_stdin() -> str:
     # See https://github.com/python/typeshed/pull/5623 for rationale behind assertion
     assert isinstance(sys.stdin, TextIOWrapper)
     sys.stdin = TextIOWrapper(sys.stdin.detach(), encoding="utf-8")
     return sys.stdin.read()
@@ -305,17 +304,17 @@
             self.set_reporter(reporter)
         else:
             self.set_reporter(TextReporter())
         self._reporters: dict[str, type[reporters.BaseReporter]] = {}
         """Dictionary of possible but non-initialized reporters."""
 
         # Attributes for checkers and plugins
-        self._checkers: defaultdict[
-            str, list[checkers.BaseChecker]
-        ] = collections.defaultdict(list)
+        self._checkers: defaultdict[str, list[checkers.BaseChecker]] = (
+            collections.defaultdict(list)
+        )
         """Dictionary of registered and initialized checkers."""
         self._dynamic_plugins: dict[str, ModuleType | ModuleNotFoundError | bool] = {}
         """Set of loaded plugin names."""
 
         # Attributes related to stats
         self.stats = LinterStats()
 
@@ -581,30 +580,30 @@
         return needed_checkers
 
     # pylint: disable=unused-argument
     @staticmethod
     def should_analyze_file(modname: str, path: str, is_argument: bool = False) -> bool:
         """Returns whether a module should be checked.
 
-        This implementation returns True for all python source file, indicating
-        that all files should be linted.
+        This implementation returns True for all python source files (.py and .pyi),
+        indicating that all files should be linted.
 
         Subclasses may override this method to indicate that modules satisfying
         certain conditions should not be linted.
 
         :param str modname: The name of the module to be checked.
         :param str path: The full path to the source code of the module.
         :param bool is_argument: Whether the file is an argument to pylint or not.
                                  Files which respect this property are always
                                  checked, since the user requested it explicitly.
         :returns: True if the module should be checked.
         """
         if is_argument:
             return True
-        return path.endswith(".py")
+        return path.endswith((".py", ".pyi"))
 
     # pylint: enable=unused-argument
 
     def initialize(self) -> None:
         """Initialize linter for linting.
 
         This method is called before any linting is done.
@@ -643,15 +642,15 @@
                     if "__init__.py" in files:
                         skip_subtrees.append(root)
                         yield root
                     else:
                         yield from (
                             os.path.join(root, file)
                             for file in files
-                            if file.endswith(".py")
+                            if file.endswith((".py", ".pyi"))
                         )
             else:
                 yield something
 
     def check(self, files_or_modules: Sequence[str]) -> None:
         """Main checking entry: check a list of files or modules from their name.
 
@@ -1076,15 +1075,15 @@
         MANAGER.extension_package_whitelist.update(self.config.extension_pkg_allow_list)
         if self.config.extension_pkg_whitelist:
             MANAGER.extension_package_whitelist.update(
                 self.config.extension_pkg_whitelist
             )
         self.stats.reset_message_count()
 
-    def generate_reports(self) -> int | None:
+    def generate_reports(self, verbose: bool = False) -> int | None:
         """Close the whole package /module, it's time to make reports !
 
         if persistent run, pickle results for later comparison
         """
         # Display whatever messages are left on the reporter.
         self.reporter.display_messages(report_nodes.Section())
         if not self.file_state._is_base_filestate:
@@ -1094,24 +1093,24 @@
             if self.config.reports:
                 sect = self.make_reports(self.stats, previous_stats)
             else:
                 sect = report_nodes.Section()
 
             if self.config.reports:
                 self.reporter.display_reports(sect)
-            score_value = self._report_evaluation()
+            score_value = self._report_evaluation(verbose)
             # save results if persistent run
             if self.config.persistent:
                 save_results(self.stats, self.file_state.base_name)
         else:
             self.reporter.on_close(self.stats, LinterStats())
             score_value = None
         return score_value
 
-    def _report_evaluation(self) -> int | None:
+    def _report_evaluation(self, verbose: bool = False) -> int | None:
         """Make the global evaluation report."""
         # check with at least a statement (usually 0 when there is a
         # syntax error preventing pylint from further processing)
         note = None
         previous_stats = load_results(self.file_state.base_name)
         if self.stats.statement == 0:
             return note
@@ -1135,14 +1134,19 @@
             self.stats.global_note = note
             msg = f"Your code has been rated at {note:.2f}/10"
             if previous_stats:
                 pnote = previous_stats.global_note
                 if pnote is not None:
                     msg += f" (previous run: {pnote:.2f}/10, {note - pnote:+.2f})"
 
+            if verbose:
+                checked_files_count = self.stats.node_count["module"]
+                unchecked_files_count = self.stats.undocumented["module"]
+                msg += f"\nChecked {checked_files_count} files, skipped {unchecked_files_count} files"
+
         if self.config.score:
             sect = report_nodes.EvaluationSection(msg)
             self.reporter.display_reports(sect)
         return note
 
     def _add_one_message(
         self,
```

### Comparing `pylint-3.0.4/pylint/lint/report_functions.py` & `pylint-3.1.0/pylint/lint/report_functions.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/lint/run.py` & `pylint-3.1.0/pylint/lint/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -199,21 +199,21 @@
                 linter.config.jobs = _cpu_count()
 
         if self._output:
             try:
                 with open(self._output, "w", encoding="utf-8") as output:
                     linter.reporter.out = output
                     linter.check(args)
-                    score_value = linter.generate_reports()
+                    score_value = linter.generate_reports(verbose=self.verbose)
             except OSError as ex:
                 print(ex, file=sys.stderr)
                 sys.exit(32)
         else:
             linter.check(args)
-            score_value = linter.generate_reports()
+            score_value = linter.generate_reports(verbose=self.verbose)
         if linter.config.clear_cache_post_run:
             clear_lru_caches()
             MANAGER.clear_cache()
 
         if exit:
             if linter.config.exit_zero:
                 sys.exit(0)
```

### Comparing `pylint-3.0.4/pylint/lint/utils.py` & `pylint-3.1.0/pylint/lint/utils.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/message/__init__.py` & `pylint-3.1.0/pylint/message/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/message/_deleted_message_ids.py` & `pylint-3.1.0/pylint/message/_deleted_message_ids.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/message/message.py` & `pylint-3.1.0/pylint/message/message.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/message/message_definition.py` & `pylint-3.1.0/pylint/message/message_definition.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/message/message_definition_store.py` & `pylint-3.1.0/pylint/message/message_definition_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from pylint.message.message_id_store import MessageIdStore
 
 if TYPE_CHECKING:
     from pylint.checkers import BaseChecker
 
 
 class MessageDefinitionStore:
-
     """The messages store knows information about every possible message definition but
     has no particular state during analysis.
     """
 
     def __init__(
         self, py_version: tuple[int, ...] | sys._version_info = sys.version_info
     ) -> None:
```

### Comparing `pylint-3.0.4/pylint/message/message_id_store.py` & `pylint-3.1.0/pylint/message/message_id_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
     is_deleted_symbol,
     is_moved_msgid,
     is_moved_symbol,
 )
 
 
 class MessageIdStore:
-
     """The MessageIdStore store MessageId and make sure that there is a 1-1 relation
     between msgid and symbol.
     """
 
     def __init__(self) -> None:
         self.__msgid_to_symbol: dict[str, str] = {}
         self.__symbol_to_msgid: dict[str, str] = {}
```

### Comparing `pylint-3.0.4/pylint/pyreverse/diadefslib.py` & `pylint-3.1.0/pylint/pyreverse/diadefslib.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/pyreverse/diagrams.py` & `pylint-3.1.0/pylint/pyreverse/diagrams.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/pyreverse/dot_printer.py` & `pylint-3.1.0/pylint/pyreverse/dot_printer.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/pyreverse/inspector.py` & `pylint-3.1.0/pylint/pyreverse/inspector.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     modname: str,
     verbose: bool = False,
 ) -> nodes.Module | None:
     if verbose:
         print(f"parsing {modname}...")
     try:
         return func(modname)
-    except astroid.exceptions.AstroidBuildingException as exc:
+    except astroid.exceptions.AstroidBuildingError as exc:
         print(exc)
     except Exception:  # pylint: disable=broad-except
         traceback.print_exc()
     return None
 
 
 class IdGeneratorMixIn:
```

### Comparing `pylint-3.0.4/pylint/pyreverse/main.py` & `pylint-3.1.0/pylint/pyreverse/main.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/pyreverse/mermaidjs_printer.py` & `pylint-3.1.0/pylint/pyreverse/mermaidjs_printer.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/pyreverse/plantuml_printer.py` & `pylint-3.1.0/pylint/pyreverse/plantuml_printer.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/pyreverse/printer.py` & `pylint-3.1.0/pylint/pyreverse/printer.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/pyreverse/printer_factory.py` & `pylint-3.1.0/pylint/pyreverse/printer_factory.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/pyreverse/utils.py` & `pylint-3.1.0/pylint/pyreverse/utils.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/pyreverse/writer.py` & `pylint-3.1.0/pylint/pyreverse/writer.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/reporters/__init__.py` & `pylint-3.1.0/pylint/reporters/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/reporters/base_reporter.py` & `pylint-3.1.0/pylint/reporters/base_reporter.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/reporters/collecting_reporter.py` & `pylint-3.1.0/pylint/reporters/collecting_reporter.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/reporters/json_reporter.py` & `pylint-3.1.0/pylint/reporters/json_reporter.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/reporters/multi_reporter.py` & `pylint-3.1.0/pylint/reporters/multi_reporter.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/reporters/reports_handler_mix_in.py` & `pylint-3.1.0/pylint/reporters/reports_handler_mix_in.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/reporters/text.py` & `pylint-3.1.0/pylint/reporters/text.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/reporters/ureports/base_writer.py` & `pylint-3.1.0/pylint/reporters/ureports/base_writer.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/reporters/ureports/nodes.py` & `pylint-3.1.0/pylint/reporters/ureports/nodes.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/reporters/ureports/text_writer.py` & `pylint-3.1.0/pylint/reporters/ureports/text_writer.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/__init__.py` & `pylint-3.1.0/pylint/testutils/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/_primer/package_to_lint.py` & `pylint-3.1.0/pylint/testutils/_primer/package_to_lint.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/_primer/primer.py` & `pylint-3.1.0/pylint/testutils/_primer/primer.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/_primer/primer_command.py` & `pylint-3.1.0/pylint/testutils/_primer/primer_command.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/_primer/primer_compare_command.py` & `pylint-3.1.0/pylint/testutils/_primer/primer_compare_command.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/_primer/primer_prepare_command.py` & `pylint-3.1.0/pylint/testutils/_primer/primer_prepare_command.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/_primer/primer_run_command.py` & `pylint-3.1.0/pylint/testutils/_primer/primer_run_command.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         )
         for package, data in package_data_iter:
             messages, p_fatal_msgs = self._lint_package(package, data)
             fatal_msgs += p_fatal_msgs
             local_commit = Repo(data.clone_directory).head.object.hexsha
             packages[package] = PackageData(commit=local_commit, messages=messages)
         path = self.primer_directory / (
-            f"output_{'.'.join(str(i) for i in sys.version_info[:3])}_{self.config.type}"
+            f"output_{'.'.join(str(i) for i in sys.version_info[:2])}_{self.config.type}"
             + (f"_batch{self.config.batchIdx}.txt" if self.config.batches else "")
         )
         print(f"Writing result in {path}")
         with open(path, "w", encoding="utf-8") as f:
             json.dump(packages, f)
         # Assert that a PR run does not introduce new fatal errors
         if self.config.type == "pr":
```

### Comparing `pylint-3.0.4/pylint/testutils/_run.py` & `pylint-3.1.0/pylint/testutils/_run.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     """Add a default pylintrc with the rcfile option in a list of pylint args."""
     if not any("--rcfile" in arg for arg in args):
         args.insert(0, f"--rcfile={PYLINTRC}")
     return args
 
 
 class _Run(LintRun):
-
     """Like Run, but we're using an explicitly set empty pylintrc.
 
     We don't want to use the project's pylintrc during tests, because
     it means that a change in our config could break tests.
     But we want to see if the changes to the default break tests.
     """
```

### Comparing `pylint-3.0.4/pylint/testutils/checker_test_case.py` & `pylint-3.1.0/pylint/testutils/checker_test_case.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/configuration_test.py` & `pylint-3.1.0/pylint/testutils/configuration_test.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/constants.py` & `pylint-3.1.0/pylint/testutils/constants.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/decorator.py` & `pylint-3.1.0/pylint/testutils/decorator.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/functional/__init__.py` & `pylint-3.1.0/pylint/testutils/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/functional/find_functional_tests.py` & `pylint-3.1.0/pylint/testutils/functional/find_functional_tests.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/functional/lint_module_output_update.py` & `pylint-3.1.0/pylint/testutils/functional/lint_module_output_update.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/functional/test_file.py` & `pylint-3.1.0/pylint/testutils/functional/test_file.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/get_test_info.py` & `pylint-3.1.0/pylint/testutils/get_test_info.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/global_test_linter.py` & `pylint-3.1.0/pylint/testutils/global_test_linter.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/lint_module_test.py` & `pylint-3.1.0/pylint/testutils/lint_module_test.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/output_line.py` & `pylint-3.1.0/pylint/testutils/output_line.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/pyreverse.py` & `pylint-3.1.0/pylint/testutils/pyreverse.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/reporter_for_tests.py` & `pylint-3.1.0/pylint/testutils/reporter_for_tests.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/unittest_linter.py` & `pylint-3.1.0/pylint/testutils/unittest_linter.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/testutils/utils.py` & `pylint-3.1.0/pylint/testutils/utils.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/typing.py` & `pylint-3.1.0/pylint/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,9 +129,10 @@
     Tuple[str, str, str],
     Tuple[str, str, str, ExtraMessageOptions],
 ]
 DirectoryNamespaceDict = Dict[Path, Tuple[argparse.Namespace, "DirectoryNamespaceDict"]]
 
 
 class GetProjectCallable(Protocol):
-    def __call__(self, module: str, name: str | None = "No Name") -> Project:
-        ...  # pragma: no cover
+    def __call__(
+        self, module: str, name: str | None = "No Name"
+    ) -> Project: ...  # pragma: no cover
```

### Comparing `pylint-3.0.4/pylint/utils/__init__.py` & `pylint-3.1.0/pylint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/utils/ast_walker.py` & `pylint-3.1.0/pylint/utils/ast_walker.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/utils/docs.py` & `pylint-3.1.0/pylint/utils/docs.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/utils/file_state.py` & `pylint-3.1.0/pylint/utils/file_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         node: nodes.Module | None = None,
         *,
         is_base_filestate: bool = False,
     ) -> None:
         self.base_name = modname
         self._module_msgs_state: MessageStateDict = {}
         self._raw_module_msgs_state: MessageStateDict = {}
-        self._ignored_msgs: defaultdict[
-            tuple[str, int], set[int]
-        ] = collections.defaultdict(set)
+        self._ignored_msgs: defaultdict[tuple[str, int], set[int]] = (
+            collections.defaultdict(set)
+        )
         self._suppression_mapping: dict[tuple[str, int], int] = {}
         self._module = node
         if node:
             self._effective_max_line_number = node.tolineno
         else:
             self._effective_max_line_number = None
         self._msgs_store = msg_store
```

### Comparing `pylint-3.0.4/pylint/utils/linterstats.py` & `pylint-3.1.0/pylint/utils/linterstats.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/utils/pragma_parser.py` & `pylint-3.1.0/pylint/utils/pragma_parser.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint/utils/utils.py` & `pylint-3.1.0/pylint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/pylint.egg-info/PKG-INFO` & `pylint-3.1.0/pylint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pylint
-Version: 3.0.4
+Version: 3.1.0
 Summary: python code static checker
 Author-email: Python Code Quality Authority <code-quality@python.org>
 License: GPL-2.0-or-later
 Project-URL: Docs: User Guide, https://pylint.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/pylint
 Project-URL: homepage, https://github.com/pylint-dev/pylint
-Project-URL: What's New, https://pylint.readthedocs.io/en/latest/whatsnew/2/
+Project-URL: What's New, https://pylint.readthedocs.io/en/latest/whatsnew/3/
 Project-URL: Bug Tracker, https://github.com/pylint-dev/pylint/issues
 Project-URL: Discord Server, https://discord.com/invite/Egy6P8AMB5
 Project-URL: Docs: Contributor Guide, https://pylint.readthedocs.io/en/latest/development_guide/contributor_guide/index.html
 Keywords: static code analysis,linter,python,lint
 Classifier: Development Status :: 6 - Mature
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -35,15 +35,15 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: CONTRIBUTORS.txt
 Requires-Dist: dill>=0.2; python_version < "3.11"
 Requires-Dist: dill>=0.3.6; python_version >= "3.11"
 Requires-Dist: dill>=0.3.7; python_version >= "3.12"
 Requires-Dist: platformdirs>=2.2.0
-Requires-Dist: astroid<=3.1.0-dev0,>=3.0.1
+Requires-Dist: astroid<=3.2.0-dev0,>=3.1.0
 Requires-Dist: isort!=5.13.0,<6,>=4.2.5
 Requires-Dist: mccabe<0.8,>=0.6
 Requires-Dist: tomli>=1.1.0; python_version < "3.11"
 Requires-Dist: tomlkit>=0.10.1
 Requires-Dist: colorama>=0.4.5; sys_platform == "win32"
 Requires-Dist: typing-extensions>=3.10.0; python_version < "3.10"
 Provides-Extra: testutils
```

### Comparing `pylint-3.0.4/pyproject.toml` & `pylint-3.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "dill>=0.2;python_version<'3.11'",
     "dill>=0.3.6;python_version>='3.11'",
     "dill>=0.3.7;python_version>='3.12'",
     "platformdirs>=2.2.0",
     # Also upgrade requirements_test_min.txt.
     # Pinned to dev of second minor update to allow editable installs and fix primer issues,
     # see https://github.com/pylint-dev/astroid/issues/1341
-    "astroid>=3.0.1,<=3.1.0-dev0",
+    "astroid>=3.1.0,<=3.2.0-dev0",
     "isort>=4.2.5,<6,!=5.13.0",
     "mccabe>=0.6,<0.8",
     "tomli>=1.1.0;python_version<'3.11'",
     "tomlkit>=0.10.1",
     "colorama>=0.4.5;sys_platform=='win32'",
     "typing-extensions>=3.10.0;python_version<'3.10'",
 ]
@@ -55,15 +55,15 @@
 testutils = ["gitpython>3"]
 spelling = ["pyenchant~=3.2"]
 
 [project.urls]
 "Docs: User Guide"  = "https://pylint.readthedocs.io/en/latest/"
 "Source Code"       = "https://github.com/pylint-dev/pylint"
 "homepage"          = "https://github.com/pylint-dev/pylint"
-"What's New"        = "https://pylint.readthedocs.io/en/latest/whatsnew/2/"
+"What's New"        = "https://pylint.readthedocs.io/en/latest/whatsnew/3/"
 "Bug Tracker"       = "https://github.com/pylint-dev/pylint/issues"
 "Discord Server"    = "https://discord.com/invite/Egy6P8AMB5"
 "Docs: Contributor Guide" = "https://pylint.readthedocs.io/en/latest/development_guide/contributor_guide/index.html"
 
 [project.scripts]
 pylint        = "pylint:run_pylint"
 pylint-config = "pylint:_run_pylint_config"
```

### Comparing `pylint-3.0.4/tests/test_check_parallel.py` & `pylint-3.1.0/tests/test_check_parallel.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/tests/test_func.py` & `pylint-3.1.0/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/tests/test_functional.py` & `pylint-3.1.0/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/tests/test_functional_directories.py` & `pylint-3.1.0/tests/test_functional_directories.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/tests/test_import_graph.py` & `pylint-3.1.0/tests/test_import_graph.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/tests/test_numversion.py` & `pylint-3.1.0/tests/test_numversion.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/tests/test_pragma_parser.py` & `pylint-3.1.0/tests/test_pragma_parser.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/tests/test_pylint_runners.py` & `pylint-3.1.0/tests/test_pylint_runners.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,27 @@
 import contextlib
 import os
 import pathlib
 import shlex
 import sys
 from collections.abc import Sequence
 from io import BufferedReader
-from typing import Any, NoReturn, Protocol
+from typing import Any, Protocol
 from unittest.mock import MagicMock, mock_open, patch
 
 import pytest
 
 from pylint import run_pylint, run_pyreverse, run_symilar
 from pylint.testutils import GenericTestReporter as Reporter
 from pylint.testutils._run import _Run as Run
 from pylint.testutils.utils import _test_cwd
 
 
 class _RunCallable(Protocol):  # pylint: disable=too-few-public-methods
-    def __call__(self, argv: Sequence[str] | None = None) -> NoReturn | None:
-        ...
+    def __call__(self, argv: Sequence[str] | None = None) -> None: ...
 
 
 @pytest.mark.parametrize("runner", [run_pylint, run_pyreverse, run_symilar])
 def test_runner(runner: _RunCallable, tmp_path: pathlib.Path) -> None:
     filepath = os.path.abspath(__file__)
     testargs = ["", filepath]
     with _test_cwd(tmp_path):
```

### Comparing `pylint-3.0.4/tests/test_regr.py` & `pylint-3.1.0/tests/test_regr.py`

 * *Files identical despite different names*

### Comparing `pylint-3.0.4/tests/test_self.py` & `pylint-3.1.0/tests/test_self.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,19 @@
         self._runtest([], code=32)
 
     def test_disable_all(self) -> None:
         out = StringIO()
         self._runtest([UNNECESSARY_LAMBDA, "--disable=all"], out=out, code=32)
         assert "No files to lint: exiting." in out.getvalue().strip()
 
+    def test_output_with_verbose(self) -> None:
+        out = StringIO()
+        self._runtest([UNNECESSARY_LAMBDA, "--verbose"], out=out, code=4)
+        assert "Checked 1 files, skipped 0 files" in out.getvalue().strip()
+
     def test_no_out_encoding(self) -> None:
         """Test redirection of stdout with non ascii characters."""
         # This test reproduces bug #48066 ; it happens when stdout is redirected
         # through '>' : the sys.stdout.encoding becomes then None, and if the
         # output contains non ascii, pylint will crash
         strio = StringIO()
         assert strio.encoding is None
@@ -363,15 +368,15 @@
         }
         message = output[0]
         for key, value in expected.items():
             assert key in message
             assert message[key] == value
         msg = message["message"].lower()
         assert any(x in msg for x in ("expected ':'", "invalid syntax"))
-        assert "<unknown>" in msg
+        assert "syntax_error" in msg
         assert "line 1" in msg
 
     def test_json_report_when_file_is_missing(self) -> None:
         out = StringIO()
         module = join(HERE, "regrtest_data", "totally_missing.py")
         self._runtest([module], code=1, reporter=JSON2Reporter(out))
         output = json.loads(out.getvalue())["messages"]
@@ -601,15 +606,15 @@
                         "--enable=import-error",
                     ],
                     expected_output=expected,
                 )
 
     def test_stdin_syntax_error(self) -> None:
         expected_output = """************* Module a
-a.py:1:4: E0001: Parsing failed: 'invalid syntax (<unknown>, line 1)' (syntax-error)"""
+a.py:1:4: E0001: Parsing failed: 'invalid syntax (a, line 1)' (syntax-error)"""
         with mock.patch(
             "pylint.lint.pylinter._read_stdin", return_value="for\n"
         ) as mock_stdin:
             self._test_output(
                 ["--from-stdin", "a.py", "--disable=all", "--enable=syntax-error"],
                 expected_output=expected_output,
             )
```

### Comparing `pylint-3.0.4/tests/test_similar.py` & `pylint-3.1.0/tests/test_similar.py`

 * *Files identical despite different names*

