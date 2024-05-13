# Comparing `tmp/pyccel-1.9.1.tar.gz` & `tmp/pyccel-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyccel-1.9.1.tar", last modified: Thu Aug 31 08:46:42 2023, max compression
+gzip compressed data, was "pyccel-1.9.2.tar", last modified: Fri Oct 13 17:49:39 2023, max compression
```

## Comparing `pyccel-1.9.1.tar` & `pyccel-1.9.2.tar`

### file list

```diff
@@ -1,761 +1,765 @@
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.786675 pyccel-1.9.1/
--rw-r--r--   0 yaman      (501) staff       (20)      556 2023-08-31 08:45:22.000000 pyccel-1.9.1/AUTHORS
--rw-r--r--   0 yaman      (501) staff       (20)     1081 2023-08-31 08:45:22.000000 pyccel-1.9.1/LICENSE
--rw-r--r--   0 yaman      (501) staff       (20)      289 2023-08-31 08:45:22.000000 pyccel-1.9.1/MANIFEST.in
--rw-r--r--   0 yaman      (501) staff       (20)     5435 2023-08-31 08:46:42.786919 pyccel-1.9.1/PKG-INFO
--rw-r--r--   0 yaman      (501) staff       (20)     5111 2023-08-31 08:45:22.000000 pyccel-1.9.1/README.md
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.494798 pyccel-1.9.1/ci_tools/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     5567 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/annotation_helpers.py
--rw-r--r--   0 yaman      (501) staff       (20)      963 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/basic_json_check_output.py
--rw-r--r--   0 yaman      (501) staff       (20)     4546 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/bot_clean_up.py
--rw-r--r--   0 yaman      (501) staff       (20)     2933 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/bot_comment_react.py
--rw-r--r--   0 yaman      (501) staff       (20)     2777 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/bot_hello.py
--rw-r--r--   0 yaman      (501) staff       (20)      957 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/bot_ready_for_review.py
--rw-r--r--   0 yaman      (501) staff       (20)     1169 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/bot_review_react.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.496140 pyccel-1.9.1/ci_tools/bot_tools/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/bot_tools/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    37766 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/bot_tools/bot_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)    26418 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/bot_tools/github_api_interactions.py
--rw-r--r--   0 yaman      (501) staff       (20)     2007 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/check_new_coverage.py
--rw-r--r--   0 yaman      (501) staff       (20)    10153 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/check_pylint_commands.py
--rw-r--r--   0 yaman      (501) staff       (20)     2903 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/check_python_capitalisation.py
--rw-r--r--   0 yaman      (501) staff       (20)     7863 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/check_slots.py
--rw-r--r--   0 yaman      (501) staff       (20)     1002 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/complete_check_run.py
--rw-r--r--   0 yaman      (501) staff       (20)    12642 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/coverage_analysis_tools.py
--rw-r--r--   0 yaman      (501) staff       (20)      737 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/devel_branch_tests.py
--rw-r--r--   0 yaman      (501) staff       (20)      662 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/fetch_artifacts.py
--rw-r--r--   0 yaman      (501) staff       (20)    12234 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/git_evaluation_tools.py
--rw-r--r--   0 yaman      (501) staff       (20)     3468 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/json_pytest_output.py
--rw-r--r--   0 yaman      (501) staff       (20)     3896 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/list_docs_tovalidate.py
--rw-r--r--   0 yaman      (501) staff       (20)     2348 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/parse_pylint_output.py
--rw-r--r--   0 yaman      (501) staff       (20)     6462 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/process_results.py
--rw-r--r--   0 yaman      (501) staff       (20)     1590 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/setup_check_run.py
--rw-r--r--   0 yaman      (501) staff       (20)     6278 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/summarise_doccoverage.py
--rw-r--r--   0 yaman      (501) staff       (20)     4720 2023-08-31 08:45:22.000000 pyccel-1.9.1/ci_tools/summarise_pyspelling.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.503460 pyccel-1.9.1/docs/
--rw-r--r--   0 yaman      (501) staff       (20)     2722 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/CONTRIBUTING.md
--rw-r--r--   0 yaman      (501) staff       (20)     1667 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/builtin-functions.md
--rw-r--r--   0 yaman      (501) staff       (20)     3835 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/compiler.md
--rw-r--r--   0 yaman      (501) staff       (20)     1779 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/const_keyword.md
--rw-r--r--   0 yaman      (501) staff       (20)    15361 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/decorators.md
--rw-r--r--   0 yaman      (501) staff       (20)    10405 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/function-pointers-as-arguments.md
--rw-r--r--   0 yaman      (501) staff       (20)     3264 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/header-files.md
--rw-r--r--   0 yaman      (501) staff       (20)     9696 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/installation.md
--rw-r--r--   0 yaman      (501) staff       (20)     8825 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/ndarrays.md
--rw-r--r--   0 yaman      (501) staff       (20)    16311 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/numpy-functions.md
--rw-r--r--   0 yaman      (501) staff       (20)    18414 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/openmp.md
--rw-r--r--   0 yaman      (501) staff       (20)    17685 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/quickstart.md
--rw-r--r--   0 yaman      (501) staff       (20)     1486 2023-08-31 08:45:22.000000 pyccel-1.9.1/docs/templates.md
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.505218 pyccel-1.9.1/pyccel/
--rw-r--r--   0 yaman      (501) staff       (20)       33 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.521638 pyccel-1.9.1/pyccel/ast/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    16911 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)    21553 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/bind_c.py
--rw-r--r--   0 yaman      (501) staff       (20)     7686 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/bitwise_operators.py
--rw-r--r--   0 yaman      (501) staff       (20)     3400 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/builtin_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)    29883 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/builtins.py
--rw-r--r--   0 yaman      (501) staff       (20)     6502 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/c_concepts.py
--rw-r--r--   0 yaman      (501) staff       (20)     8278 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/class_defs.py
--rw-r--r--   0 yaman      (501) staff       (20)   130916 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/core.py
--rw-r--r--   0 yaman      (501) staff       (20)    21543 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/cwrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)    10766 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/datatypes.py
--rw-r--r--   0 yaman      (501) staff       (20)     3715 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/functionalexpr.py
--rw-r--r--   0 yaman      (501) staff       (20)    29329 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/headers.py
--rw-r--r--   0 yaman      (501) staff       (20)    11790 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/internals.py
--rw-r--r--   0 yaman      (501) staff       (20)     2062 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/itertoolsext.py
--rw-r--r--   0 yaman      (501) staff       (20)    10766 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/literals.py
--rw-r--r--   0 yaman      (501) staff       (20)     3564 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/macros.py
--rw-r--r--   0 yaman      (501) staff       (20)    10805 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/mathext.py
--rw-r--r--   0 yaman      (501) staff       (20)    15051 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/numpy_wrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)    70960 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/numpyext.py
--rw-r--r--   0 yaman      (501) staff       (20)     7113 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/omp.py
--rw-r--r--   0 yaman      (501) staff       (20)    35482 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/operators.py
--rw-r--r--   0 yaman      (501) staff       (20)      869 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/scipyext.py
--rw-r--r--   0 yaman      (501) staff       (20)     7475 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/sympy_helper.py
--rw-r--r--   0 yaman      (501) staff       (20)     1630 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/sysext.py
--rw-r--r--   0 yaman      (501) staff       (20)    30831 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/utilities.py
--rw-r--r--   0 yaman      (501) staff       (20)    30023 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/ast/variable.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.523911 pyccel-1.9.1/pyccel/codegen/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     6587 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.525181 pyccel-1.9.1/pyccel/codegen/compiling/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/compiling/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    11130 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/compiling/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)    18371 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/compiling/compilers.py
--rw-r--r--   0 yaman      (501) staff       (20)    16668 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/pipeline.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.528977 pyccel-1.9.1/pyccel/codegen/printing/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/printing/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    89886 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/printing/ccode.py
--rw-r--r--   0 yaman      (501) staff       (20)     4722 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/printing/codeprinter.py
--rw-r--r--   0 yaman      (501) staff       (20)    15370 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/printing/cwrappercode.py
--rw-r--r--   0 yaman      (501) staff       (20)   121029 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/printing/fcode.py
--rw-r--r--   0 yaman      (501) staff       (20)    20480 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/printing/luacode.py
--rw-r--r--   0 yaman      (501) staff       (20)    41186 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/printing/pycode.py
--rw-r--r--   0 yaman      (501) staff       (20)     8281 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/python_wrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)     8226 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/utilities.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.532514 pyccel-1.9.1/pyccel/codegen/wrapper/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/wrapper/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    48490 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/wrapper/c_to_python_wrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)    20519 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/wrapper/fortran_to_c_wrapper.py
--rw-r--r--   0 yaman      (501) staff       (20)     3341 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/codegen/wrapper/wrapper.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.534379 pyccel-1.9.1/pyccel/commands/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/commands/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    12405 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/commands/console.py
--rw-r--r--   0 yaman      (501) staff       (20)     3659 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/commands/pyccel_clean.py
--rw-r--r--   0 yaman      (501) staff       (20)     1144 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/commands/pyccel_init.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.535212 pyccel-1.9.1/pyccel/compilers/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/compilers/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    10802 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/compilers/default_compilers.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.537018 pyccel-1.9.1/pyccel/complexity/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/complexity/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2780 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/complexity/arithmetic.py
--rw-r--r--   0 yaman      (501) staff       (20)     1145 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/complexity/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)     7188 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/complexity/memory.py
--rw-r--r--   0 yaman      (501) staff       (20)     3138 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/decorators.py
--rw-r--r--   0 yaman      (501) staff       (20)    13846 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/epyccel.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.538422 pyccel-1.9.1/pyccel/errors/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/errors/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    12564 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/errors/errors.py
--rw-r--r--   0 yaman      (501) staff       (20)    11926 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/errors/messages.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.540654 pyccel-1.9.1/pyccel/naming/
--rw-r--r--   0 yaman      (501) staff       (20)      791 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/naming/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     3369 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/naming/cnameclashchecker.py
--rw-r--r--   0 yaman      (501) staff       (20)     4048 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/naming/fortrannameclashchecker.py
--rw-r--r--   0 yaman      (501) staff       (20)     1879 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/naming/languagenameclashchecker.py
--rw-r--r--   0 yaman      (501) staff       (20)     1810 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/naming/pythonnameclashchecker.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.545080 pyccel-1.9.1/pyccel/parser/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    16321 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/base.py
--rw-r--r--   0 yaman      (501) staff       (20)     9547 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/extend_tree.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.547463 pyccel-1.9.1/pyccel/parser/grammar/
--rw-r--r--   0 yaman      (501) staff       (20)     2221 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/grammar/headers.tx
--rw-r--r--   0 yaman      (501) staff       (20)      391 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/grammar/himi.tx
--rw-r--r--   0 yaman      (501) staff       (20)     6361 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/grammar/openacc.tx
--rw-r--r--   0 yaman      (501) staff       (20)     7307 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/grammar/openmp.tx
--rw-r--r--   0 yaman      (501) staff       (20)     6539 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/grammar/pyccel.tx
--rw-r--r--   0 yaman      (501) staff       (20)     7460 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/parser.py
--rw-r--r--   0 yaman      (501) staff       (20)    22192 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/scope.py
--rw-r--r--   0 yaman      (501) staff       (20)   162460 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/semantic.py
--rw-r--r--   0 yaman      (501) staff       (20)    39799 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/syntactic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.549677 pyccel-1.9.1/pyccel/parser/syntax/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/syntax/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2236 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/syntax/basic.py
--rw-r--r--   0 yaman      (501) staff       (20)    19189 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/syntax/headers.py
--rw-r--r--   0 yaman      (501) staff       (20)    36464 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/syntax/openacc.py
--rw-r--r--   0 yaman      (501) staff       (20)    27508 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/syntax/openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)     4079 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/parser/utilities.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.550147 pyccel-1.9.1/pyccel/stdlib/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.550840 pyccel-1.9.1/pyccel/stdlib/cwrapper/
--rw-r--r--   0 yaman      (501) staff       (20)     4529 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/cwrapper/cwrapper.c
--rw-r--r--   0 yaman      (501) staff       (20)     6528 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/cwrapper/cwrapper.h
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.551726 pyccel-1.9.1/pyccel/stdlib/cwrapper_ndarrays/
--rw-r--r--   0 yaman      (501) staff       (20)    13082 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c
--rw-r--r--   0 yaman      (501) staff       (20)     1923 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.553663 pyccel-1.9.1/pyccel/stdlib/external/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/external/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     1749 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/external/dfftpack.py
--rw-r--r--   0 yaman      (501) staff       (20)     1112 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/external/fitpack.py
--rw-r--r--   0 yaman      (501) staff       (20)     1266 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/external/lapack.py
--rw-r--r--   0 yaman      (501) staff       (20)     9467 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/external/mpi4py.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.564381 pyccel-1.9.1/pyccel/stdlib/internal/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)    35250 2023-08-31 08:46:38.000000 pyccel-1.9.1/pyccel/stdlib/internal/blas.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     7825 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/blas.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     5974 2023-08-31 08:46:38.000000 pyccel-1.9.1/pyccel/stdlib/internal/dfftpack.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     1144 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/dfftpack.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     2841 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/fftw.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     2901 2023-08-31 08:46:38.000000 pyccel-1.9.1/pyccel/stdlib/internal/fitpack.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)      343 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/fitpack.pyh
--rw-r--r--   0 yaman      (501) staff       (20)    18250 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/hdf5.pyh
--rw-r--r--   0 yaman      (501) staff       (20)   354681 2023-08-31 08:46:39.000000 pyccel-1.9.1/pyccel/stdlib/internal/lapack.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)    58149 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/lapack.pyh
--rw-r--r--   0 yaman      (501) staff       (20)    25284 2023-08-31 08:46:40.000000 pyccel-1.9.1/pyccel/stdlib/internal/mpi.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     5911 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/mpi.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     1226 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/mpiext.py
--rw-r--r--   0 yaman      (501) staff       (20)    11051 2023-08-31 08:46:40.000000 pyccel-1.9.1/pyccel/stdlib/internal/openacc.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     2675 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/openacc.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     8715 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)    10087 2023-08-31 08:46:40.000000 pyccel-1.9.1/pyccel/stdlib/internal/openmp.pyccel
--rw-r--r--   0 yaman      (501) staff       (20)     2645 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/internal/openmp.pyh
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.565704 pyccel-1.9.1/pyccel/stdlib/math/
--rw-r--r--   0 yaman      (501) staff       (20)     1766 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/math/pyc_math_c.c
--rw-r--r--   0 yaman      (501) staff       (20)     1331 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/math/pyc_math_c.h
--rw-r--r--   0 yaman      (501) staff       (20)     3479 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/math/pyc_math_f90.f90
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.566714 pyccel-1.9.1/pyccel/stdlib/ndarrays/
--rw-r--r--   0 yaman      (501) staff       (20)    15769 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/ndarrays/ndarrays.c
--rw-r--r--   0 yaman      (501) staff       (20)     7481 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/ndarrays/ndarrays.h
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.567771 pyccel-1.9.1/pyccel/stdlib/numpy/
--rw-r--r--   0 yaman      (501) staff       (20)      755 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/numpy/numpy_c.c
--rw-r--r--   0 yaman      (501) staff       (20)      650 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/numpy/numpy_c.h
--rw-r--r--   0 yaman      (501) staff       (20)     4629 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/numpy/numpy_f90.f90
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.568575 pyccel-1.9.1/pyccel/stdlib/parallel/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/parallel/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     7487 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/stdlib/parallel/mpi.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.569229 pyccel-1.9.1/pyccel/symbolic/
--rw-r--r--   0 yaman      (501) staff       (20)       48 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/symbolic/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     4472 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/symbolic/lambdify.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.570692 pyccel-1.9.1/pyccel/utilities/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/utilities/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     1350 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/utilities/metaclasses.py
--rw-r--r--   0 yaman      (501) staff       (20)     1592 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/utilities/stage.py
--rw-r--r--   0 yaman      (501) staff       (20)     2185 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/utilities/strings.py
--rw-r--r--   0 yaman      (501) staff       (20)       86 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyccel/version.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.508236 pyccel-1.9.1/pyccel.egg-info/
--rw-r--r--   0 yaman      (501) staff       (20)     5435 2023-08-31 08:46:41.000000 pyccel-1.9.1/pyccel.egg-info/PKG-INFO
--rw-r--r--   0 yaman      (501) staff       (20)    25745 2023-08-31 08:46:42.000000 pyccel-1.9.1/pyccel.egg-info/SOURCES.txt
--rw-r--r--   0 yaman      (501) staff       (20)        1 2023-08-31 08:46:41.000000 pyccel-1.9.1/pyccel.egg-info/dependency_links.txt
--rw-r--r--   0 yaman      (501) staff       (20)      185 2023-08-31 08:46:42.000000 pyccel-1.9.1/pyccel.egg-info/entry_points.txt
--rw-r--r--   0 yaman      (501) staff       (20)        1 2023-08-31 08:46:40.000000 pyccel-1.9.1/pyccel.egg-info/not-zip-safe
--rw-r--r--   0 yaman      (501) staff       (20)      178 2023-08-31 08:46:42.000000 pyccel-1.9.1/pyccel.egg-info/requires.txt
--rw-r--r--   0 yaman      (501) staff       (20)       16 2023-08-31 08:46:42.000000 pyccel-1.9.1/pyccel.egg-info/top_level.txt
--rw-r--r--   0 yaman      (501) staff       (20)      225 2023-08-31 08:45:22.000000 pyccel-1.9.1/pyproject.toml
--rw-r--r--   0 yaman      (501) staff       (20)      950 2023-08-31 08:46:42.788071 pyccel-1.9.1/setup.cfg
--rw-r--r--   0 yaman      (501) staff       (20)      628 2023-08-31 08:45:22.000000 pyccel-1.9.1/setup.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.571733 pyccel-1.9.1/tests/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.572044 pyccel-1.9.1/tests/ast/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.572842 pyccel-1.9.1/tests/ast/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      257 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/ast/scripts/cyclic_dependence.py
--rw-r--r--   0 yaman      (501) staff       (20)      184 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/ast/scripts/math.py
--rw-r--r--   0 yaman      (501) staff       (20)     5580 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/ast/test_basic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.464404 pyccel-1.9.1/tests/codegen/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.573243 pyccel-1.9.1/tests/codegen/ccode/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.576295 pyccel-1.9.1/tests/codegen/ccode/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      714 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/ccode/scripts/arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)     1558 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/ccode/scripts/arrays_create.py
--rw-r--r--   0 yaman      (501) staff       (20)      754 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/ccode/scripts/arrays_indexing.py
--rw-r--r--   0 yaman      (501) staff       (20)      616 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/ccode/scripts/arrays_pointers.py
--rw-r--r--   0 yaman      (501) staff       (20)     1320 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/ccode/scripts/arrays_slicing.py
--rw-r--r--   0 yaman      (501) staff       (20)      876 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/ccode/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      925 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/ccode/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)     1184 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/ccode/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)      378 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/ccode/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)     1734 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/ccode/test_ccode_codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.576697 pyccel-1.9.1/tests/codegen/fcode/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.591295 pyccel-1.9.1/tests/codegen/fcode/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)     1280 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/CommentBlock.py
--rw-r--r--   0 yaman      (501) staff       (20)      851 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/Functional_Stmts.py
--rw-r--r--   0 yaman      (501) staff       (20)      401 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/ListComprehension.py
--rw-r--r--   0 yaman      (501) staff       (20)      145 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/USELESS_EXPRESSION.py
--rw-r--r--   0 yaman      (501) staff       (20)      229 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)      101 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/calls.py
--rw-r--r--   0 yaman      (501) staff       (20)      646 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)      734 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/classes_2.py
--rw-r--r--   0 yaman      (501) staff       (20)      735 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/classes_3.py
--rw-r--r--   0 yaman      (501) staff       (20)     1388 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/classes_4.py
--rw-r--r--   0 yaman      (501) staff       (20)      295 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/complex_numbers.py
--rw-r--r--   0 yaman      (501) staff       (20)     1272 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/decorators.py
--rw-r--r--   0 yaman      (501) staff       (20)      288 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/decorators_elemental.py
--rw-r--r--   0 yaman      (501) staff       (20)      157 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/decorators_pure.py
--rw-r--r--   0 yaman      (501) staff       (20)     1020 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/decorators_types.py
--rw-r--r--   0 yaman      (501) staff       (20)      232 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)      574 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/functions_inout.py
--rw-r--r--   0 yaman      (501) staff       (20)      480 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/generic_methods.py
--rw-r--r--   0 yaman      (501) staff       (20)      425 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/headers.py
--rw-r--r--   0 yaman      (501) staff       (20)      980 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)      264 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      485 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/issue_177.py
--rw-r--r--   0 yaman      (501) staff       (20)      190 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/lists.py
--rw-r--r--   0 yaman      (501) staff       (20)      838 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     2002 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/macros.py
--rw-r--r--   0 yaman      (501) staff       (20)      802 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/matrix_assembly.py
--rw-r--r--   0 yaman      (501) staff       (20)      681 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/matrix_mul.py
--rw-r--r--   0 yaman      (501) staff       (20)      257 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/multiple_assign.py
--rw-r--r--   0 yaman      (501) staff       (20)     1231 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/numpyext.py
--rw-r--r--   0 yaman      (501) staff       (20)      782 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/precision.py
--rw-r--r--   0 yaman      (501) staff       (20)      705 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/recursive_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      236 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/returns.py
--rw-r--r--   0 yaman      (501) staff       (20)      359 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      381 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)     1711 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/fcode/test_fcode_codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.591748 pyccel-1.9.1/tests/codegen/pycode/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.592140 pyccel-1.9.1/tests/codegen/pycode/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)     1330 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/pycode/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     1351 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/codegen/pycode/test_pycode_codegen.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.592560 pyccel-1.9.1/tests/complexity/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.592934 pyccel-1.9.1/tests/complexity/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/complexity/scripts/ex.py
--rw-r--r--   0 yaman      (501) staff       (20)     1053 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/complexity/test_complexity.py
--rw-r--r--   0 yaman      (501) staff       (20)     2423 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/conftest.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.613632 pyccel-1.9.1/tests/epyccel/
--rw-r--r--   0 yaman      (501) staff       (20)      189 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/Module_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      238 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/README.rst
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.628506 pyccel-1.9.1/tests/epyccel/modules/
--rw-r--r--   0 yaman      (501) staff       (20)      189 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/Module_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      271 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/Module_2.py
--rw-r--r--   0 yaman      (501) staff       (20)      201 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/Module_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      285 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/Module_4.py
--rw-r--r--   0 yaman      (501) staff       (20)     1225 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/Module_5.py
--rw-r--r--   0 yaman      (501) staff       (20)      698 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/Module_6.py
--rw-r--r--   0 yaman      (501) staff       (20)      771 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/Module_7.py
--rw-r--r--   0 yaman      (501) staff       (20)      234 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/Module_8.py
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      728 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/array_consts.py
--rw-r--r--   0 yaman      (501) staff       (20)    51842 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)     2507 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/augassign.py
--rw-r--r--   0 yaman      (501) staff       (20)      234 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/awkward_names.py
--rw-r--r--   0 yaman      (501) staff       (20)     3347 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/base.py
--rw-r--r--   0 yaman      (501) staff       (20)     1362 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/bitwise.py
--rw-r--r--   0 yaman      (501) staff       (20)      788 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/call_user_defined_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)     1909 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/complex_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      222 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/consts.py
--rw-r--r--   0 yaman      (501) staff       (20)     2284 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/external_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     2031 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/functionals.py
--rw-r--r--   0 yaman      (501) staff       (20)     2153 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/generic_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     4085 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/generic_functions_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     4081 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/highorder_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     4482 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     1008 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/mpi_collective.py
--rw-r--r--   0 yaman      (501) staff       (20)      489 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/mpi_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)     2823 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/multi_rank.py
--rw-r--r--   0 yaman      (501) staff       (20)     5023 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/numpy_sign.py
--rw-r--r--   0 yaman      (501) staff       (20)    14714 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)     1198 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/pointers.py
--rw-r--r--   0 yaman      (501) staff       (20)     1101 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/python_annotations.py
--rw-r--r--   0 yaman      (501) staff       (20)      681 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/strings.py
--rw-r--r--   0 yaman      (501) staff       (20)     9800 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      632 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/modules/types.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.630327 pyccel-1.9.1/tests/epyccel/recognised_functions/
--rw-r--r--   0 yaman      (501) staff       (20)     2664 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py
--rw-r--r--   0 yaman      (501) staff       (20)    37082 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/recognised_functions/test_math_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)   250560 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/recognised_functions/test_numpy_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)    42294 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/recognised_functions/test_numpy_types.py
--rw-r--r--   0 yaman      (501) staff       (20)     4693 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_array_as_func_args.py
--rw-r--r--   0 yaman      (501) staff       (20)   108229 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)    10425 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_arrays_multiple_assignments.py
--rw-r--r--   0 yaman      (501) staff       (20)     6170 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_base.py
--rw-r--r--   0 yaman      (501) staff       (20)     5120 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_bitwise.py
--rw-r--r--   0 yaman      (501) staff       (20)     9482 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_builtins.py
--rw-r--r--   0 yaman      (501) staff       (20)     4087 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_class_expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1422 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_compare_expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)      831 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_default_precision_template.py
--rw-r--r--   0 yaman      (501) staff       (20)     1191 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_docstrings.py
--rw-r--r--   0 yaman      (501) staff       (20)     7438 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_IfTernaryOperator.py
--rw-r--r--   0 yaman      (501) staff       (20)     9168 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_augassign.py
--rw-r--r--   0 yaman      (501) staff       (20)     3817 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_complex_func.py
--rw-r--r--   0 yaman      (501) staff       (20)     3136 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_decorators.py
--rw-r--r--   0 yaman      (501) staff       (20)     2309 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_default_args.py
--rw-r--r--   0 yaman      (501) staff       (20)     8182 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_division.py
--rw-r--r--   0 yaman      (501) staff       (20)     9152 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     4662 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_generators.py
--rw-r--r--   0 yaman      (501) staff       (20)     2747 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_mod.py
--rw-r--r--   0 yaman      (501) staff       (20)     4652 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_modules.py
--rw-r--r--   0 yaman      (501) staff       (20)     5519 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_multi_rank.py
--rw-r--r--   0 yaman      (501) staff       (20)    19588 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_openmp.py
--rw-r--r--   0 yaman      (501) staff       (20)     5593 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_optional_args.py
--rw-r--r--   0 yaman      (501) staff       (20)     6588 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_pow.py
--rw-r--r--   0 yaman      (501) staff       (20)     3265 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_python_annotations.py
--rw-r--r--   0 yaman      (501) staff       (20)    38124 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_return_arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)    13388 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_sign.py
--rw-r--r--   0 yaman      (501) staff       (20)     5823 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_transpose.py
--rw-r--r--   0 yaman      (501) staff       (20)     3471 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_epyccel_types.py
--rw-r--r--   0 yaman      (501) staff       (20)     3306 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_external_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     2149 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_functionals.py
--rw-r--r--   0 yaman      (501) staff       (20)    14648 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_generic_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1922 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_higherorder_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1755 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)     2115 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_kind.py
--rw-r--r--   0 yaman      (501) staff       (20)     6036 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_loops.py
--rw-r--r--   0 yaman      (501) staff       (20)     4164 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_mpi_collective.py
--rw-r--r--   0 yaman      (501) staff       (20)     2114 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_mpi_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)     1023 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_multiple_results.py
--rw-r--r--   0 yaman      (501) staff       (20)     1735 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_parallel_epyccel.py
--rw-r--r--   0 yaman      (501) staff       (20)     1258 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_pointers.py
--rw-r--r--   0 yaman      (501) staff       (20)     7496 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_return.py
--rw-r--r--   0 yaman      (501) staff       (20)     1333 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_strings.py
--rw-r--r--   0 yaman      (501) staff       (20)     3200 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/test_tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      704 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/epyccel/utilities.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.630747 pyccel-1.9.1/tests/errors/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.466556 pyccel-1.9.1/tests/errors/codegen/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.631492 pyccel-1.9.1/tests/errors/codegen/fortran/
--rw-r--r--   0 yaman      (501) staff       (20)      108 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/codegen/fortran/FORTRAN_ALLOCATABLE_IN_EXPRESSION.py
--rw-r--r--   0 yaman      (501) staff       (20)      131 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/codegen/fortran/randint.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.634104 pyccel-1.9.1/tests/errors/known_bugs/
--rw-r--r--   0 yaman      (501) staff       (20)     1160 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/known_bugs/context.py
--rw-r--r--   0 yaman      (501) staff       (20)      236 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/known_bugs/cross.py
--rw-r--r--   0 yaman      (501) staff       (20)      143 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/known_bugs/dicts.py
--rw-r--r--   0 yaman      (501) staff       (20)      495 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/known_bugs/ex3.py
--rw-r--r--   0 yaman      (501) staff       (20)      796 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/known_bugs/ex4.py
--rw-r--r--   0 yaman      (501) staff       (20)      579 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/known_bugs/header_interface.py
--rw-r--r--   0 yaman      (501) staff       (20)      928 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/known_bugs/inheritance.py
--rw-r--r--   0 yaman      (501) staff       (20)      180 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/known_bugs/lambdas.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.467424 pyccel-1.9.1/tests/errors/semantic/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.648085 pyccel-1.9.1/tests/errors/semantic/blocking/
--rw-r--r--   0 yaman      (501) staff       (20)      128 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_0.py
--rw-r--r--   0 yaman      (501) staff       (20)      166 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      174 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/COMPLEX_TYPE.py
--rw-r--r--   0 yaman      (501) staff       (20)      159 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT.py
--rw-r--r--   0 yaman      (501) staff       (20)      193 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT2.py
--rw-r--r--   0 yaman      (501) staff       (20)      155 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/DECORATOR_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      132 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      296 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
--rw-r--r--   0 yaman      (501) staff       (20)      114 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED.py
--rw-r--r--   0 yaman      (501) staff       (20)      145 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED2.py
--rw-r--r--   0 yaman      (501) staff       (20)      315 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED3.py
--rw-r--r--   0 yaman      (501) staff       (20)       94 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/INHOMOG_LIST.py
--rw-r--r--   0 yaman      (501) staff       (20)      124 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/INIT_NDARRAY_WITH_INHOMOG_LIST.py
--rw-r--r--   0 yaman      (501) staff       (20)      396 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/INTERFACE_WRONG_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      182 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/LIST_OF_TUPLES.py
--rw-r--r--   0 yaman      (501) staff       (20)      129 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/OPENMP_loop_check.py
--rw-r--r--   0 yaman      (501) staff       (20)      102 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/OPENMP_parallel_for_check.py
--rw-r--r--   0 yaman      (501) staff       (20)      131 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/OPENMP_simd_check.py
--rw-r--r--   0 yaman      (501) staff       (20)      221 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_decorator.py
--rw-r--r--   0 yaman      (501) staff       (20)      241 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_header.py
--rw-r--r--   0 yaman      (501) staff       (20)      448 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/TEMPLATE_WRONG_TYPE_CALL.py
--rw-r--r--   0 yaman      (501) staff       (20)      110 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/TOO_MANY_ARGS.py
--rw-r--r--   0 yaman      (501) staff       (20)       92 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_FUNCTION.py
--rw-r--r--   0 yaman      (501) staff       (20)       89 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_VARIABLE.py
--rw-r--r--   0 yaman      (501) staff       (20)      108 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/UNRECOGNISED_FUNCTION_CALL.py
--rw-r--r--   0 yaman      (501) staff       (20)      186 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)       95 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/ex2.py
--rw-r--r--   0 yaman      (501) staff       (20)       97 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/ex3.py
--rw-r--r--   0 yaman      (501) staff       (20)       88 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/ex4.py
--rw-r--r--   0 yaman      (501) staff       (20)       92 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/ex5.py
--rw-r--r--   0 yaman      (501) staff       (20)      100 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/str_join.py
--rw-r--r--   0 yaman      (501) staff       (20)      106 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/str_join2.py
--rw-r--r--   0 yaman      (501) staff       (20)      727 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/blocking/unknown_method.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.658261 pyccel-1.9.1/tests/errors/semantic/non_blocking/
--rw-r--r--   0 yaman      (501) staff       (20)      136 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT.py
--rw-r--r--   0 yaman      (501) staff       (20)      150 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT2.py
--rw-r--r--   0 yaman      (501) staff       (20)      152 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      118 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_2.py
--rw-r--r--   0 yaman      (501) staff       (20)       87 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      150 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_complex.py
--rw-r--r--   0 yaman      (501) staff       (20)      144 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_float.py
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_integer.py
--rw-r--r--   0 yaman      (501) staff       (20)      163 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_string.py
--rw-r--r--   0 yaman      (501) staff       (20)      143 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_complex.py
--rw-r--r--   0 yaman      (501) staff       (20)      137 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_float.py
--rw-r--r--   0 yaman      (501) staff       (20)      135 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_integer.py
--rw-r--r--   0 yaman      (501) staff       (20)      156 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_string.py
--rw-r--r--   0 yaman      (501) staff       (20)      220 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/PYCCEL_RESTRICTION_LIST_COMPREHENSION_LIMITS.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/TOO_FEW_ARGS.py
--rw-r--r--   0 yaman      (501) staff       (20)      118 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT.py
--rw-r--r--   0 yaman      (501) staff       (20)       97 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT2.py
--rw-r--r--   0 yaman      (501) staff       (20)      270 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/class_inheritance.py
--rw-r--r--   0 yaman      (501) staff       (20)      201 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/ex6.py
--rw-r--r--   0 yaman      (501) staff       (20)      143 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/is.py
--rw-r--r--   0 yaman      (501) staff       (20)      153 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/semantic/non_blocking/var_is_none.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.659217 pyccel-1.9.1/tests/errors/syntax_blockers/
--rw-r--r--   0 yaman      (501) staff       (20)      286 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_blockers/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      412 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_blockers/imports.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.667245 pyccel-1.9.1/tests/errors/syntax_errors/
--rw-r--r--   0 yaman      (501) staff       (20)      330 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/TEMPLATE_WRONG_KEY.py
--rw-r--r--   0 yaman      (501) staff       (20)      341 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/TEMPLATE_WRONG_NUMBER_ARGS.py
--rw-r--r--   0 yaman      (501) staff       (20)       91 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/dict_str_keys.py
--rw-r--r--   0 yaman      (501) staff       (20)      122 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/empty_class.py
--rw-r--r--   0 yaman      (501) staff       (20)      206 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/functions_in_template.py
--rw-r--r--   0 yaman      (501) staff       (20)      157 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/functions_in_uniontype.py
--rw-r--r--   0 yaman      (501) staff       (20)      109 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/import_star.py
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/list_comprehension_no_assign.py
--rw-r--r--   0 yaman      (501) staff       (20)       95 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/nargs.py
--rw-r--r--   0 yaman      (501) staff       (20)      125 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/not_implemented.py
--rw-r--r--   0 yaman      (501) staff       (20)      114 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/raise.py
--rw-r--r--   0 yaman      (501) staff       (20)      125 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/try.py
--rw-r--r--   0 yaman      (501) staff       (20)      156 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/types_arg.py
--rw-r--r--   0 yaman      (501) staff       (20)      137 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/types_arg_type.py
--rw-r--r--   0 yaman      (501) staff       (20)       99 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/syntax_errors/yield.py
--rw-r--r--   0 yaman      (501) staff       (20)     5505 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/errors/test_errors.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.667718 pyccel-1.9.1/tests/external/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.468820 pyccel-1.9.1/tests/external/scripts/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.668185 pyccel-1.9.1/tests/external/scripts/lapack/
--rw-r--r--   0 yaman      (501) staff       (20)     2401 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/lapack/ex1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.676486 pyccel-1.9.1/tests/external/scripts/mpi4py/
--rw-r--r--   0 yaman      (501) staff       (20)      334 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      684 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/bcast.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.677522 pyccel-1.9.1/tests/external/scripts/mpi4py/bugs/
--rw-r--r--   0 yaman      (501) staff       (20)      943 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/bugs/ex6.py
--rw-r--r--   0 yaman      (501) staff       (20)      662 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/bugs/ex8.py
--rw-r--r--   0 yaman      (501) staff       (20)      550 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/gather.py
--rw-r--r--   0 yaman      (501) staff       (20)      468 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/np_Allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      765 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/np_Bcast.py
--rw-r--r--   0 yaman      (501) staff       (20)      720 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/np_Gather.py
--rw-r--r--   0 yaman      (501) staff       (20)      435 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/np_Reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      524 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/np_Sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      636 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/np_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      402 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/np_point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1559 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/np_point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      274 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      367 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1559 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      339 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      364 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      240 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/scripts/mpi4py/who_am_i.py
--rw-r--r--   0 yaman      (501) staff       (20)     1362 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/external/test_external.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.678019 pyccel-1.9.1/tests/internal/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.470628 pyccel-1.9.1/tests/internal/scripts/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.680384 pyccel-1.9.1/tests/internal/scripts/blas/
--rw-r--r--   0 yaman      (501) staff       (20)      559 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/blas/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      890 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/blas/ex2.py
--rw-r--r--   0 yaman      (501) staff       (20)      584 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/blas/ex3.py
--rw-r--r--   0 yaman      (501) staff       (20)      920 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/blas/ex4.py
--rw-r--r--   0 yaman      (501) staff       (20)      761 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/blas/ex5.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.680860 pyccel-1.9.1/tests/internal/scripts/lapack/
--rw-r--r--   0 yaman      (501) staff       (20)     2779 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/lapack/ex1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.689077 pyccel-1.9.1/tests/internal/scripts/mpi/
--rw-r--r--   0 yaman      (501) staff       (20)     1401 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/allgather.py
--rw-r--r--   0 yaman      (501) staff       (20)     1205 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)     1391 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/alltoall.py
--rw-r--r--   0 yaman      (501) staff       (20)     1129 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/bcast.py
--rw-r--r--   0 yaman      (501) staff       (20)     2057 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/column.py
--rw-r--r--   0 yaman      (501) staff       (20)     1477 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/gather.py
--rw-r--r--   0 yaman      (501) staff       (20)     2089 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/line.py
--rw-r--r--   0 yaman      (501) staff       (20)     1771 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/nonblocking.py
--rw-r--r--   0 yaman      (501) staff       (20)     1266 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/point_to_point_1.py
--rw-r--r--   0 yaman      (501) staff       (20)     3048 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1237 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)     1431 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/scatter.py
--rw-r--r--   0 yaman      (501) staff       (20)     1372 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)     1321 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/sendrecv_replace.py
--rw-r--r--   0 yaman      (501) staff       (20)     1740 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/split.py
--rw-r--r--   0 yaman      (501) staff       (20)      772 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/mpi/who_am_i.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.690463 pyccel-1.9.1/tests/internal/scripts/openacc/
--rw-r--r--   0 yaman      (501) staff       (20)      448 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/openacc/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      619 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/openacc/sum.py
--rw-r--r--   0 yaman      (501) staff       (20)      581 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/openacc/sum_kernels.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.691379 pyccel-1.9.1/tests/internal/scripts/openmp/
--rw-r--r--   0 yaman      (501) staff       (20)      606 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/openmp/ex1.py
--rw-r--r--   0 yaman      (501) staff       (20)      412 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/scripts/openmp/ex2.py
--rw-r--r--   0 yaman      (501) staff       (20)     3608 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/internal/test_internal.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.691846 pyccel-1.9.1/tests/macro/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.472376 pyccel-1.9.1/tests/macro/scripts/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.700760 pyccel-1.9.1/tests/macro/scripts/MPI/
--rw-r--r--   0 yaman      (501) staff       (20)      447 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      864 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/bcast.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.701771 pyccel-1.9.1/tests/macro/scripts/MPI/bug/
--rw-r--r--   0 yaman      (501) staff       (20)     1586 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/bug/ex6.py
--rw-r--r--   0 yaman      (501) staff       (20)      662 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/bug/ex8.py
--rw-r--r--   0 yaman      (501) staff       (20)      788 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/gather.py
--rw-r--r--   0 yaman      (501) staff       (20)     7929 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/mpi4py.py
--rw-r--r--   0 yaman      (501) staff       (20)      548 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/np_Allreduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      898 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/np_Bcast.py
--rw-r--r--   0 yaman      (501) staff       (20)      831 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/np_Gather.py
--rw-r--r--   0 yaman      (501) staff       (20)      551 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/np_Reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      567 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/np_Sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      749 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/np_point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      602 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/np_point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1942 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/np_point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      379 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/point_to_point.py
--rw-r--r--   0 yaman      (501) staff       (20)      567 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/point_to_point_2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1952 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/point_to_point_3.py
--rw-r--r--   0 yaman      (501) staff       (20)      471 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/reduce.py
--rw-r--r--   0 yaman      (501) staff       (20)      478 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/sendrecv.py
--rw-r--r--   0 yaman      (501) staff       (20)      403 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/MPI/who_am_i.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.704990 pyccel-1.9.1/tests/macro/scripts/blas/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.705438 pyccel-1.9.1/tests/macro/scripts/blas/bugs/
--rw-r--r--   0 yaman      (501) staff       (20)      363 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/blas/bugs/dnrm2.py
--rw-r--r--   0 yaman      (501) staff       (20)      681 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/blas/runtest_daxpy.py
--rw-r--r--   0 yaman      (501) staff       (20)      467 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/blas/runtest_dcopy.py
--rw-r--r--   0 yaman      (501) staff       (20)     1148 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/blas/runtest_dgemm.py
--rw-r--r--   0 yaman      (501) staff       (20)     1186 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/blas/runtest_dgemv.py
--rw-r--r--   0 yaman      (501) staff       (20)      756 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/blas/runtest_dger.py
--rw-r--r--   0 yaman      (501) staff       (20)      482 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/blas/runtest_dscal.py
--rw-r--r--   0 yaman      (501) staff       (20)      636 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/blas/runtest_dswap.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.705906 pyccel-1.9.1/tests/macro/scripts/lapack/
--rw-r--r--   0 yaman      (501) staff       (20)      670 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/scripts/lapack/runtest_dgbtrf.py
--rw-r--r--   0 yaman      (501) staff       (20)     3214 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/macro/test_macro.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.707401 pyccel-1.9.1/tests/ndarrays/
--rw-r--r--   0 yaman      (501) staff       (20)     4723 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/ndarrays/conftest.py
--rw-r--r--   0 yaman      (501) staff       (20)     1714 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/ndarrays/leaks_check.py
--rw-r--r--   0 yaman      (501) staff       (20)    47975 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/ndarrays/test_ndarrays.c
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.709439 pyccel-1.9.1/tests/parser/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.709922 pyccel-1.9.1/tests/parser/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)     1074 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/parser/scripts/comments.py
--rw-r--r--   0 yaman      (501) staff       (20)     3490 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/parser/test_comments.py
--rw-r--r--   0 yaman      (501) staff       (20)     1468 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/parser/test_headers.py
--rw-r--r--   0 yaman      (501) staff       (20)      358 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/parser/test_openacc.py
--rw-r--r--   0 yaman      (501) staff       (20)      279 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/parser/test_openmp.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.710398 pyccel-1.9.1/tests/preprocess/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.710821 pyccel-1.9.1/tests/preprocess/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      943 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/preprocess/scripts/omp.py
--rw-r--r--   0 yaman      (501) staff       (20)     1017 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/preprocess/test_preprocess.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.711769 pyccel-1.9.1/tests/pyccel/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.712410 pyccel-1.9.1/tests/pyccel/project_abs_imports/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.712897 pyccel-1.9.1/tests/pyccel/project_abs_imports/project/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_abs_imports/project/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.713740 pyccel-1.9.1/tests/pyccel/project_abs_imports/project/folder1/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_abs_imports/project/folder1/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      288 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_abs_imports/project/folder1/mod1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.715009 pyccel-1.9.1/tests/pyccel/project_abs_imports/project/folder2/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_abs_imports/project/folder2/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      214 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_abs_imports/project/folder2/mod2.py
--rw-r--r--   0 yaman      (501) staff       (20)      293 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_abs_imports/project/folder2/mod3.py
--rw-r--r--   0 yaman      (501) staff       (20)      214 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_abs_imports/runtest.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.716894 pyccel-1.9.1/tests/pyccel/project_multi_imports/
--rw-r--r--   0 yaman      (501) staff       (20)      116 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_multi_imports/file1.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_multi_imports/file2.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_multi_imports/file3.py
--rw-r--r--   0 yaman      (501) staff       (20)      179 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_multi_imports/file4.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.717370 pyccel-1.9.1/tests/pyccel/project_rel_imports/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.717890 pyccel-1.9.1/tests/pyccel/project_rel_imports/project/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_rel_imports/project/__init__.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.718591 pyccel-1.9.1/tests/pyccel/project_rel_imports/project/folder1/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_rel_imports/project/folder1/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      288 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_rel_imports/project/folder1/mod1.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.719981 pyccel-1.9.1/tests/pyccel/project_rel_imports/project/folder2/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_rel_imports/project/folder2/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      208 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_rel_imports/project/folder2/mod2.py
--rw-r--r--   0 yaman      (501) staff       (20)      272 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_rel_imports/project/folder2/mod3.py
--rw-r--r--   0 yaman      (501) staff       (20)      214 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/project_rel_imports/runtest.py
--rw-r--r--   0 yaman      (501) staff       (20)      199 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/run_import_function.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.737203 pyccel-1.9.1/tests/pyccel/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)     2928 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/array_binary_operation.py
--rw-r--r--   0 yaman      (501) staff       (20)     4109 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/arrays_view.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.738947 pyccel-1.9.1/tests/pyccel/scripts/asserts/
--rw-r--r--   0 yaman      (501) staff       (20)      117 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/asserts/unvalid_assert1.py
--rw-r--r--   0 yaman      (501) staff       (20)      138 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/asserts/unvalid_assert2.py
--rw-r--r--   0 yaman      (501) staff       (20)      162 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/asserts/unvalid_assert3.py
--rw-r--r--   0 yaman      (501) staff       (20)      217 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/asserts/valid_assert.py
--rw-r--r--   0 yaman      (501) staff       (20)       68 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/basic_header.pyh
--rw-r--r--   0 yaman      (501) staff       (20)     1327 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/bool_comp.py
--rw-r--r--   0 yaman      (501) staff       (20)     2132 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/c_arrays.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.741284 pyccel-1.9.1/tests/pyccel/scripts/classes/
--rw-r--r--   0 yaman      (501) staff       (20)      726 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/classes/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)      590 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/classes/classes_1.py
--rw-r--r--   0 yaman      (501) staff       (20)      719 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/classes/classes_2_C.py
--rw-r--r--   0 yaman      (501) staff       (20)      492 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/classes/classes_5.py
--rw-r--r--   0 yaman      (501) staff       (20)      733 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/classes/generic_methods.py
--rw-r--r--   0 yaman      (501) staff       (20)      251 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/concatenation.py
--rw-r--r--   0 yaman      (501) staff       (20)      359 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/decorators_elemental.py
--rw-r--r--   0 yaman      (501) staff       (20)      821 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/decorators_inline.py
--rw-r--r--   0 yaman      (501) staff       (20)      872 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/default_args_mod.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.744833 pyccel-1.9.1/tests/pyccel/scripts/exits/
--rw-r--r--   0 yaman      (501) staff       (20)      126 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/exits/empty_exit.py
--rw-r--r--   0 yaman      (501) staff       (20)      150 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/exits/negative_exit1.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/exits/negative_exit2.py
--rw-r--r--   0 yaman      (501) staff       (20)      127 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/exits/positive_exit1.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/exits/positive_exit2.py
--rw-r--r--   0 yaman      (501) staff       (20)      184 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/exits/positive_exit3.py
--rw-r--r--   0 yaman      (501) staff       (20)      127 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/exits/zero_exit.py
--rw-r--r--   0 yaman      (501) staff       (20)     2236 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/expressions.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.745662 pyccel-1.9.1/tests/pyccel/scripts/folder1/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/folder1/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      283 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/folder1/folder1_funcs.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.747468 pyccel-1.9.1/tests/pyccel/scripts/folder2/
--rw-r--r--   0 yaman      (501) staff       (20)        0 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/folder2/__init__.py
--rw-r--r--   0 yaman      (501) staff       (20)      283 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/folder2/folder2_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)      198 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/folder2/runtest_imports2.py
--rw-r--r--   0 yaman      (501) staff       (20)      189 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/folder2/runtest_rel_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      283 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)      950 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)     3567 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/generic_functions.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.751124 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/
--rw-r--r--   0 yaman      (501) staff       (20)      285 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/hope_fib.py
--rw-r--r--   0 yaman      (501) staff       (20)      591 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py
--rw-r--r--   0 yaman      (501) staff       (20)      814 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py
--rw-r--r--   0 yaman      (501) staff       (20)      265 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/hope_pisum.py
--rw-r--r--   0 yaman      (501) staff       (20)     1188 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      807 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/quicksort.py
--rw-r--r--   0 yaman      (501) staff       (20)      280 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/simplify.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.753935 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/
--rw-r--r--   0 yaman      (501) staff       (20)      256 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/fib.py
--rw-r--r--   0 yaman      (501) staff       (20)      535 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py
--rw-r--r--   0 yaman      (501) staff       (20)      786 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py
--rw-r--r--   0 yaman      (501) staff       (20)     1192 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      782 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py
--rw-r--r--   0 yaman      (501) staff       (20)      264 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/simplify.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.764613 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/
--rw-r--r--   0 yaman      (501) staff       (20)      182 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/collisions2.py
--rw-r--r--   0 yaman      (501) staff       (20)      201 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/collisions3.py
--rw-r--r--   0 yaman      (501) staff       (20)      218 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/collisions4.py
--rw-r--r--   0 yaman      (501) staff       (20)      187 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/collisions5.py
--rw-r--r--   0 yaman      (501) staff       (20)      922 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import.py
--rw-r--r--   0 yaman      (501) staff       (20)      993 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import_as.py
--rw-r--r--   0 yaman      (501) staff       (20)     1002 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      249 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import_as_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      253 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import_as_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      943 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      252 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      257 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      934 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod.py
--rw-r--r--   0 yaman      (501) staff       (20)      925 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod_as.py
--rw-r--r--   0 yaman      (501) staff       (20)     1019 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod_as_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      244 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod_as_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      249 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod_as_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)     1001 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      246 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod_user.py
--rw-r--r--   0 yaman      (501) staff       (20)      250 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod_user_func.py
--rw-r--r--   0 yaman      (501) staff       (20)      152 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/user_mod.py
--rw-r--r--   0 yaman      (501) staff       (20)      134 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/import_syntax/user_mod2.py
--rw-r--r--   0 yaman      (501) staff       (20)      882 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/lapack_subroutine.py
--rw-r--r--   0 yaman      (501) staff       (20)      175 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/module_init.py
--rw-r--r--   0 yaman      (501) staff       (20)      116 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/module_init2.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.765574 pyccel-1.9.1/tests/pyccel/scripts/numpy/
--rw-r--r--   0 yaman      (501) staff       (20)     1551 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/numpy/numpy_kernels.py
--rw-r--r--   0 yaman      (501) staff       (20)     2812 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/numpy/numpy_sign.py
--rw-r--r--   0 yaman      (501) staff       (20)      812 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/print_integers.py
--rw-r--r--   0 yaman      (501) staff       (20)      885 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/print_sp_and_end.py
--rw-r--r--   0 yaman      (501) staff       (20)     2056 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/print_strings.py
--rw-r--r--   0 yaman      (501) staff       (20)      381 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/print_tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      704 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/return_numpy_arrays.py
--rw-r--r--   0 yaman      (501) staff       (20)      418 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_decorators_inline.py
--rw-r--r--   0 yaman      (501) staff       (20)      736 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_default_args.py
--rw-r--r--   0 yaman      (501) staff       (20)      673 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_degree_in.py
--rw-r--r--   0 yaman      (501) staff       (20)      166 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_folder_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      333 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_funcs.py
--rw-r--r--   0 yaman      (501) staff       (20)      324 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_function_alias.py
--rw-r--r--   0 yaman      (501) staff       (20)      659 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_generic_functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      150 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      411 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_inoutfunc.py
--rw-r--r--   0 yaman      (501) staff       (20)      167 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_module_init.py
--rw-r--r--   0 yaman      (501) staff       (20)      305 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_module_init2.py
--rw-r--r--   0 yaman      (501) staff       (20)     1499 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_multiple_results.py
--rw-r--r--   0 yaman      (501) staff       (20)      412 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/scripts/runtest_type_print.py
--rw-r--r--   0 yaman      (501) staff       (20)    46938 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/pyccel/test_pyccel.py
--rw-r--r--   0 yaman      (501) staff       (20)      844 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/run_tests.bat
--rwxr-xr-x   0 yaman      (501) staff       (20)      899 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/run_tests_py3.sh
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.766025 pyccel-1.9.1/tests/semantic/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.770959 pyccel-1.9.1/tests/semantic/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      135 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/calls.py
--rw-r--r--   0 yaman      (501) staff       (20)      506 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)      825 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)     1171 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      128 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)      197 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      141 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/lists.py
--rw-r--r--   0 yaman      (501) staff       (20)      111 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)      307 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)      163 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)      311 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/scripts/zeros.py
--rw-r--r--   0 yaman      (501) staff       (20)     1030 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/semantic/test_semantic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.771420 pyccel-1.9.1/tests/symbolic/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.772800 pyccel-1.9.1/tests/symbolic/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      958 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/symbolic/scripts/decorator.py
--rw-r--r--   0 yaman      (501) staff       (20)      283 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/symbolic/scripts/lambdas.py
--rw-r--r--   0 yaman      (501) staff       (20)      711 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/symbolic/scripts/neural_net.py
--rw-r--r--   0 yaman      (501) staff       (20)     1263 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/symbolic/test_symbolic.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.773241 pyccel-1.9.1/tests/syntax/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.782909 pyccel-1.9.1/tests/syntax/scripts/
--rw-r--r--   0 yaman      (501) staff       (20)      851 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/Functional_Stmts.py
--rw-r--r--   0 yaman      (501) staff       (20)      157 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/annotated_comments.py
--rw-r--r--   0 yaman      (501) staff       (20)       86 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/asserts.py
--rw-r--r--   0 yaman      (501) staff       (20)       77 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/breaks.py
--rw-r--r--   0 yaman      (501) staff       (20)      110 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/calls.py
--rw-r--r--   0 yaman      (501) staff       (20)      796 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/class_member_index.py
--rw-r--r--   0 yaman      (501) staff       (20)      369 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/classes.py
--rw-r--r--   0 yaman      (501) staff       (20)       86 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/dels.py
--rw-r--r--   0 yaman      (501) staff       (20)      190 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/dots.py
--rw-r--r--   0 yaman      (501) staff       (20)      964 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/expressions.py
--rw-r--r--   0 yaman      (501) staff       (20)      193 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/functions.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/ifs.py
--rw-r--r--   0 yaman      (501) staff       (20)      288 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/imports.py
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/lists.py
--rw-r--r--   0 yaman      (501) staff       (20)      110 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/loops.py
--rw-r--r--   0 yaman      (501) staff       (20)       80 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/prints.py
--rw-r--r--   0 yaman      (501) staff       (20)      196 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/slice.py
--rw-r--r--   0 yaman      (501) staff       (20)      142 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/tuples.py
--rw-r--r--   0 yaman      (501) staff       (20)       92 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/whiles.py
--rw-r--r--   0 yaman      (501) staff       (20)      311 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/scripts/zeros.py
--rw-r--r--   0 yaman      (501) staff       (20)     1059 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/syntax/test_syntax.py
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.783373 pyccel-1.9.1/tests/warnings/
-drwxr-xr-x   0 yaman      (501) staff       (20)        0 2023-08-31 08:46:42.786255 pyccel-1.9.1/tests/warnings/semantic/
--rw-r--r--   0 yaman      (501) staff       (20)      155 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/warnings/semantic/DECORATOR_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      145 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/warnings/semantic/FOUND_DUPLICATED_IMPORT.py
--rw-r--r--   0 yaman      (501) staff       (20)      130 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES.py
--rw-r--r--   0 yaman      (501) staff       (20)      318 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
--rw-r--r--   0 yaman      (501) staff       (20)      133 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/warnings/semantic/UNDEFINED_DECORATOR.py
--rw-r--r--   0 yaman      (501) staff       (20)      141 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/warnings/semantic/UNDEFINED_DECORATORS.py
--rw-r--r--   0 yaman      (501) staff       (20)     3007 2023-08-31 08:45:22.000000 pyccel-1.9.1/tests/warnings/test_warnings.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.552615 pyccel-1.9.2/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      556 2023-10-13 17:46:43.000000 pyccel-1.9.2/AUTHORS
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1081 2023-10-13 17:46:43.000000 pyccel-1.9.2/LICENSE
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      289 2023-10-13 17:46:43.000000 pyccel-1.9.2/MANIFEST.in
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6510 2023-10-13 17:49:39.552615 pyccel-1.9.2/PKG-INFO
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6186 2023-10-13 17:46:43.000000 pyccel-1.9.2/README.md
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.392612 pyccel-1.9.2/ci_tools/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     5567 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/annotation_helpers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      963 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/basic_json_check_output.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4644 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/bot_clean_up.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3103 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/bot_comment_react.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2740 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/bot_hello.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      957 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/bot_ready_for_review.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1169 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/bot_review_react.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.392612 pyccel-1.9.2/ci_tools/bot_tools/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/bot_tools/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    39132 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/bot_tools/bot_funcs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    26982 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/bot_tools/github_api_interactions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2007 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/check_new_coverage.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    10153 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/check_pylint_commands.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2903 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/check_python_capitalisation.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7863 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/check_slots.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1002 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/complete_check_run.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    12642 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/coverage_analysis_tools.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      791 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/devel_branch_tests.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      662 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/fetch_artifacts.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    12344 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/git_evaluation_tools.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3468 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/json_pytest_output.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3896 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/list_docs_tovalidate.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2348 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/parse_pylint_output.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6462 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/process_results.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1392 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/setup_check_run.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6278 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/summarise_doccoverage.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4720 2023-10-13 17:46:43.000000 pyccel-1.9.2/ci_tools/summarise_pyspelling.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.396612 pyccel-1.9.2/docs/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2722 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/CONTRIBUTING.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1667 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/builtin-functions.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3957 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/compiler.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1779 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/const_keyword.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    15361 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/decorators.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    10405 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/function-pointers-as-arguments.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3264 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/header-files.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     9696 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/installation.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     8825 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/ndarrays.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    16311 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/numpy-functions.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    18414 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/openmp.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    17685 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/quickstart.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      581 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/supported-libraries.md
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1486 2023-10-13 17:46:43.000000 pyccel-1.9.2/docs/templates.md
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.396612 pyccel-1.9.2/pyccel/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       33 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/__init__.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.472614 pyccel-1.9.2/pyccel/ast/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    16911 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/basic.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    21553 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/bind_c.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7686 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/bitwise_operators.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3400 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/builtin_imports.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    30321 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/builtins.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6502 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/c_concepts.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     8278 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/class_defs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    13961 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/cmathext.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)   132914 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/core.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    21553 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/cwrapper.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    10909 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/datatypes.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3715 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/functionalexpr.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    27316 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/headers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    13830 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/internals.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2062 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/itertoolsext.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    10766 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/literals.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3564 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/macros.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    19651 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/mathext.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    15051 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/numpy_wrapper.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    73780 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/numpyext.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7113 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/omp.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    35482 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/operators.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      869 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/scipyext.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7475 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/sympy_helper.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1630 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/sysext.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     8312 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/type_annotations.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    30908 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/utilities.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    30986 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/ast/variable.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.472614 pyccel-1.9.2/pyccel/codegen/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6587 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/codegen.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.476614 pyccel-1.9.2/pyccel/codegen/compiling/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/compiling/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    11130 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/compiling/basic.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    18371 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/compiling/compilers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    16711 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/pipeline.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.476614 pyccel-1.9.2/pyccel/codegen/printing/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/printing/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    93274 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/printing/ccode.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4722 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/printing/codeprinter.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    14138 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/printing/cwrappercode.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)   121049 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/printing/fcode.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    20480 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/printing/luacode.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    42263 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/printing/pycode.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     8281 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/python_wrapper.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     8226 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/utilities.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.480614 pyccel-1.9.2/pyccel/codegen/wrapper/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/wrapper/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    48490 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/wrapper/c_to_python_wrapper.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    20519 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/wrapper/fortran_to_c_wrapper.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3341 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/codegen/wrapper/wrapper.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.480614 pyccel-1.9.2/pyccel/commands/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/commands/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    12405 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/commands/console.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3659 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/commands/pyccel_clean.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1144 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/commands/pyccel_init.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.480614 pyccel-1.9.2/pyccel/compilers/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/compilers/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    10804 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/compilers/default_compilers.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.480614 pyccel-1.9.2/pyccel/complexity/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/complexity/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2780 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/complexity/arithmetic.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1145 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/complexity/basic.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7188 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/complexity/memory.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3138 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/decorators.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    13846 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/epyccel.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.484614 pyccel-1.9.2/pyccel/errors/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/errors/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    12564 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/errors/errors.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    11870 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/errors/messages.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.484614 pyccel-1.9.2/pyccel/naming/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      791 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/naming/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3369 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/naming/cnameclashchecker.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4048 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/naming/fortrannameclashchecker.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1879 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/naming/languagenameclashchecker.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1810 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/naming/pythonnameclashchecker.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.484614 pyccel-1.9.2/pyccel/parser/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    16321 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/base.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     9547 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/extend_tree.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.484614 pyccel-1.9.2/pyccel/parser/grammar/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1999 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/grammar/headers.tx
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      391 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/grammar/himi.tx
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6361 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/grammar/openacc.tx
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7307 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/grammar/openmp.tx
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6539 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/grammar/pyccel.tx
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7460 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/parser.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    22469 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/scope.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)   170410 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/semantic.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    41427 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/syntactic.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.484614 pyccel-1.9.2/pyccel/parser/syntax/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/syntax/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2236 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/syntax/basic.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    19833 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/syntax/headers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    36464 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/syntax/openacc.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    27508 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/syntax/openmp.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4079 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/parser/utilities.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.484614 pyccel-1.9.2/pyccel/stdlib/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/__init__.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.484614 pyccel-1.9.2/pyccel/stdlib/cwrapper/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4529 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/cwrapper/cwrapper.c
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6528 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/cwrapper/cwrapper.h
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.484614 pyccel-1.9.2/pyccel/stdlib/cwrapper_ndarrays/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    13082 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1923 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.488614 pyccel-1.9.2/pyccel/stdlib/external/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/external/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1749 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/external/dfftpack.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1112 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/external/fitpack.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1266 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/external/lapack.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     9467 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/external/mpi4py.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.488614 pyccel-1.9.2/pyccel/stdlib/internal/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    35935 2023-10-13 17:49:35.000000 pyccel-1.9.2/pyccel/stdlib/internal/blas.pyccel
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7825 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/blas.pyh
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6036 2023-10-13 17:49:35.000000 pyccel-1.9.2/pyccel/stdlib/internal/dfftpack.pyccel
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1144 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/dfftpack.pyh
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2841 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/fftw.pyh
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2950 2023-10-13 17:49:35.000000 pyccel-1.9.2/pyccel/stdlib/internal/fitpack.pyccel
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      343 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/fitpack.pyh
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    18250 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/hdf5.pyh
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)   354283 2023-10-13 17:49:36.000000 pyccel-1.9.2/pyccel/stdlib/internal/lapack.pyccel
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    58149 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/lapack.pyh
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    36995 2023-10-13 17:49:38.000000 pyccel-1.9.2/pyccel/stdlib/internal/mpi.pyccel
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     5911 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/mpi.pyh
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1226 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/mpiext.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    11119 2023-10-13 17:49:36.000000 pyccel-1.9.2/pyccel/stdlib/internal/openacc.pyccel
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2675 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/openacc.pyh
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     8715 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/openmp.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    10136 2023-10-13 17:49:36.000000 pyccel-1.9.2/pyccel/stdlib/internal/openmp.pyccel
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2645 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/internal/openmp.pyh
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.488614 pyccel-1.9.2/pyccel/stdlib/math/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1766 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/math/pyc_math_c.c
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1331 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/math/pyc_math_c.h
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3479 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/math/pyc_math_f90.f90
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.488614 pyccel-1.9.2/pyccel/stdlib/ndarrays/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    15769 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/ndarrays/ndarrays.c
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7481 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/ndarrays/ndarrays.h
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.492614 pyccel-1.9.2/pyccel/stdlib/numpy/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      755 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/numpy/numpy_c.c
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      650 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/numpy/numpy_c.h
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4629 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/numpy/numpy_f90.f90
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.492614 pyccel-1.9.2/pyccel/stdlib/parallel/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/parallel/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7487 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/stdlib/parallel/mpi.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.492614 pyccel-1.9.2/pyccel/symbolic/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       48 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/symbolic/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4472 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/symbolic/lambdify.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.492614 pyccel-1.9.2/pyccel/utilities/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/utilities/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1350 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/utilities/metaclasses.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1592 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/utilities/stage.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2185 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/utilities/strings.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       86 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyccel/version.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.396612 pyccel-1.9.2/pyccel.egg-info/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6510 2023-10-13 17:49:38.000000 pyccel-1.9.2/pyccel.egg-info/PKG-INFO
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    25888 2023-10-13 17:49:39.000000 pyccel-1.9.2/pyccel.egg-info/SOURCES.txt
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        1 2023-10-13 17:49:38.000000 pyccel-1.9.2/pyccel.egg-info/dependency_links.txt
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      185 2023-10-13 17:49:38.000000 pyccel-1.9.2/pyccel.egg-info/entry_points.txt
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        1 2023-10-13 17:49:36.000000 pyccel-1.9.2/pyccel.egg-info/not-zip-safe
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      178 2023-10-13 17:49:39.000000 pyccel-1.9.2/pyccel.egg-info/requires.txt
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       16 2023-10-13 17:49:39.000000 pyccel-1.9.2/pyccel.egg-info/top_level.txt
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      225 2023-10-13 17:46:43.000000 pyccel-1.9.2/pyproject.toml
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      950 2023-10-13 17:49:39.552615 pyccel-1.9.2/setup.cfg
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      628 2023-10-13 17:46:43.000000 pyccel-1.9.2/setup.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.492614 pyccel-1.9.2/tests/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.492614 pyccel-1.9.2/tests/ast/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.492614 pyccel-1.9.2/tests/ast/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      257 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/ast/scripts/cyclic_dependence.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      184 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/ast/scripts/math.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     5580 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/ast/test_basic.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.384612 pyccel-1.9.2/tests/codegen/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.492614 pyccel-1.9.2/tests/codegen/ccode/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.492614 pyccel-1.9.2/tests/codegen/ccode/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      714 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/ccode/scripts/arrays.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1558 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/ccode/scripts/arrays_create.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      754 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/ccode/scripts/arrays_indexing.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      616 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/ccode/scripts/arrays_pointers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1320 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/ccode/scripts/arrays_slicing.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      876 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/ccode/scripts/functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      925 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/ccode/scripts/ifs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1184 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/ccode/scripts/loops.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      378 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/ccode/scripts/whiles.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1734 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/ccode/test_ccode_codegen.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.492614 pyccel-1.9.2/tests/codegen/fcode/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.496614 pyccel-1.9.2/tests/codegen/fcode/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1280 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/CommentBlock.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      851 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/Functional_Stmts.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      401 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/ListComprehension.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      145 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/USELESS_EXPRESSION.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      229 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/arrays.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      561 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/classes_2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      566 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/classes_3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1210 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/classes_4.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      295 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/complex_numbers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1094 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/decorators.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      288 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/decorators_elemental.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      157 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/decorators_pure.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1020 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/decorators_types.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      232 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/expressions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      574 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/functions_inout.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      425 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/headers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      980 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/ifs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      261 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/imports.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      431 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/issue_177.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      190 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/lists.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      838 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/loops.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2002 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/macros.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      802 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/matrix_assembly.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      681 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/matrix_mul.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      257 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/multiple_assign.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1231 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/numpyext.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      782 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/precision.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      705 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/recursive_functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      236 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/returns.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      359 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/tuples.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      381 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/scripts/whiles.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1711 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/fcode/test_fcode_codegen.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.496614 pyccel-1.9.2/tests/codegen/pycode/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.496614 pyccel-1.9.2/tests/codegen/pycode/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1330 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/pycode/scripts/loops.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1351 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/codegen/pycode/test_pycode_codegen.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.496614 pyccel-1.9.2/tests/complexity/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.496614 pyccel-1.9.2/tests/complexity/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      142 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/complexity/scripts/ex.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1053 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/complexity/test_complexity.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2423 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/conftest.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.504614 pyccel-1.9.2/tests/epyccel/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      189 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/Module_1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      238 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/README.rst
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.508614 pyccel-1.9.2/tests/epyccel/modules/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      189 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/Module_1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      271 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/Module_2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      201 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/Module_3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      285 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/Module_4.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1225 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/Module_5.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      698 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/Module_6.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      771 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/Module_7.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      234 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/Module_8.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      728 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/array_consts.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    51842 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/arrays.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2507 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/augassign.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      234 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/awkward_names.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3347 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/base.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1362 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/bitwise.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      788 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/call_user_defined_funcs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1909 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/complex_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      222 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/consts.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2284 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/external_functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2031 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/functionals.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2153 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/generic_functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4085 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/generic_functions_2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4081 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/highorder_functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4482 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/loops.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1008 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/mpi_collective.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      489 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/mpi_point_to_point.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2823 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/multi_rank.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     5023 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/numpy_sign.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    14714 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/openmp.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1198 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/pointers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1101 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/python_annotations.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      681 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/strings.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     9800 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/tuples.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      632 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/modules/types.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.508614 pyccel-1.9.2/tests/epyccel/recognised_functions/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    15142 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/recognised_functions/test_cmath_funcs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2664 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    37112 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/recognised_functions/test_math_funcs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)   250560 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/recognised_functions/test_numpy_funcs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    42294 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/recognised_functions/test_numpy_types.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4693 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_array_as_func_args.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)   108381 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_arrays.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    10425 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_arrays_multiple_assignments.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6170 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_base.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     5120 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_bitwise.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     9482 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_builtins.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4087 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_class_expressions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1422 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_compare_expressions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      831 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_default_precision_template.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1191 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_docstrings.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7438 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_IfTernaryOperator.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     9168 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_augassign.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3817 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_complex_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3136 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_decorators.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2309 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_default_args.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     8182 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_division.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     9152 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4662 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_generators.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2632 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_headers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2747 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_mod.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4652 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_modules.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     5519 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_multi_rank.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    19683 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_openmp.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     5593 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_optional_args.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6588 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_pow.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3265 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_python_annotations.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    38124 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_return_arrays.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    13388 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_sign.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     5823 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_transpose.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3471 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_epyccel_types.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3306 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_external_functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2149 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_functionals.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    14648 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_generic_functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1922 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_higherorder_functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1755 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_imports.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2115 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_kind.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     6036 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_loops.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4164 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_mpi_collective.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2114 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_mpi_point_to_point.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1023 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_multiple_results.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1735 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_parallel_epyccel.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1258 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_pointers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7496 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_return.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1333 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_strings.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3200 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/test_tuples.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      704 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/epyccel/utilities.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.508614 pyccel-1.9.2/tests/errors/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.384612 pyccel-1.9.2/tests/errors/codegen/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.508614 pyccel-1.9.2/tests/errors/codegen/fortran/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      108 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/codegen/fortran/FORTRAN_ALLOCATABLE_IN_EXPRESSION.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      131 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/codegen/fortran/randint.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.512614 pyccel-1.9.2/tests/errors/known_bugs/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      101 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/known_bugs/calls.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      236 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/known_bugs/cross.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      143 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/known_bugs/dicts.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      423 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/known_bugs/ex3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      725 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/known_bugs/ex4.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      579 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/known_bugs/header_interface.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      769 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/known_bugs/inheritance.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      180 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/known_bugs/lambdas.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.384612 pyccel-1.9.2/tests/errors/semantic/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.516614 pyccel-1.9.2/tests/errors/semantic/blocking/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      128 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_0.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      166 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/ADD_ARRAYS_INCOMPATIBLE_SHAPES_1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      174 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/COMPLEX_TYPE.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      159 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      193 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/CONST_ASSIGNED_ARGUMENT2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      155 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/DECORATOR_WRONG_NUMBER_TYPES.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      132 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      221 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      114 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      145 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      315 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/IMPORTING_EXISTING_IDENTIFIED3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       94 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/INHOMOG_LIST.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      124 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/INIT_NDARRAY_WITH_INHOMOG_LIST.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      396 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/INTERFACE_WRONG_TYPES.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      182 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/LIST_OF_TUPLES.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      129 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/OPENMP_loop_check.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      102 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/OPENMP_parallel_for_check.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      131 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/OPENMP_simd_check.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      221 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_decorator.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      241 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_header.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      448 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/TEMPLATE_WRONG_TYPE_CALL.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      110 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/TOO_MANY_ARGS.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      121 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/TUPLE_WITH_INCOHERENT_RANKS.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       92 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_FUNCTION.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       89 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/UNDEFINED_LAMBDA_VARIABLE.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      108 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/UNRECOGNISED_FUNCTION_CALL.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      186 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/ex1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       95 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/ex2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       97 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/ex3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       88 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/ex4.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       92 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/ex5.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      100 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/str_join.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      106 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/str_join2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      628 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/blocking/unknown_method.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.516614 pyccel-1.9.2/tests/errors/semantic/non_blocking/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      136 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      150 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/INCOMPATIBLE_ARGUMENT2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      152 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      118 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       87 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/INCOMPATIBLE_TYPES_IN_ASSIGNMENT_3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      150 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_complex.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      144 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_float.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      142 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_integer.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      163 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_ISNOT_string.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      143 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_complex.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      137 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_float.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      135 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_integer.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      156 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/PRIMITIVE_IMMUTABLE_RESTRICTION_IS_string.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      220 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/PYCCEL_RESTRICTION_LIST_COMPREHENSION_LIMITS.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      130 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/TOO_FEW_ARGS.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      118 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       97 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/UNKNOWN_IMPORT2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      217 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/class_inheritance.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      201 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/ex6.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      143 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/is.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      153 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/semantic/non_blocking/var_is_none.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.516614 pyccel-1.9.2/tests/errors/syntax_blockers/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      286 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_blockers/ex1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      412 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_blockers/imports.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.520614 pyccel-1.9.2/tests/errors/syntax_errors/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      330 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/TEMPLATE_WRONG_KEY.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      341 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/TEMPLATE_WRONG_NUMBER_ARGS.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       91 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/dict_str_keys.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      122 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/empty_class.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      206 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/functions_in_template.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      157 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/functions_in_uniontype.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      109 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/import_star.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      142 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/list_comprehension_no_assign.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       95 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/nargs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      125 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/not_implemented.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      114 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/raise.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      125 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/try.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      156 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/types_arg.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      137 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/types_arg_type.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       99 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/syntax_errors/yield.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     5505 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/errors/test_errors.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.520614 pyccel-1.9.2/tests/external/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.388612 pyccel-1.9.2/tests/external/scripts/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.520614 pyccel-1.9.2/tests/external/scripts/lapack/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2401 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/lapack/ex1.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.520614 pyccel-1.9.2/tests/external/scripts/mpi4py/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      334 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/allreduce.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      684 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/bcast.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.524614 pyccel-1.9.2/tests/external/scripts/mpi4py/bugs/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      943 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/bugs/ex6.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      662 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/bugs/ex8.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      550 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/gather.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      468 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/np_Allreduce.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      765 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/np_Bcast.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      720 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/np_Gather.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      435 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/np_Reduce.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      524 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/np_Sendrecv.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      636 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/np_point_to_point.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      402 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/np_point_to_point_2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1559 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/np_point_to_point_3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      274 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/point_to_point.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      367 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/point_to_point_2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1559 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/point_to_point_3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      339 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/reduce.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      364 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/sendrecv.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      240 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/scripts/mpi4py/who_am_i.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1362 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/external/test_external.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.524614 pyccel-1.9.2/tests/internal/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.388612 pyccel-1.9.2/tests/internal/scripts/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.524614 pyccel-1.9.2/tests/internal/scripts/blas/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      559 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/blas/ex1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      890 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/blas/ex2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      584 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/blas/ex3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      920 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/blas/ex4.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      761 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/blas/ex5.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.524614 pyccel-1.9.2/tests/internal/scripts/lapack/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2779 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/lapack/ex1.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.524614 pyccel-1.9.2/tests/internal/scripts/mpi/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1401 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/allgather.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1205 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/allreduce.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1391 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/alltoall.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1129 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/bcast.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2057 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/column.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1477 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/gather.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2089 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/line.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1771 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/nonblocking.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1266 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/point_to_point_1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3048 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/point_to_point_2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1237 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/reduce.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1431 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/scatter.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1372 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/sendrecv.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1321 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/sendrecv_replace.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1740 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/split.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      772 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/mpi/who_am_i.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.524614 pyccel-1.9.2/tests/internal/scripts/openacc/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      448 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/openacc/ex1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      619 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/openacc/sum.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      581 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/openacc/sum_kernels.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.524614 pyccel-1.9.2/tests/internal/scripts/openmp/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      606 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/openmp/ex1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      412 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/scripts/openmp/ex2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3608 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/internal/test_internal.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.524614 pyccel-1.9.2/tests/macro/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.388612 pyccel-1.9.2/tests/macro/scripts/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.528615 pyccel-1.9.2/tests/macro/scripts/MPI/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      447 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/allreduce.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      864 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/bcast.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.528615 pyccel-1.9.2/tests/macro/scripts/MPI/bug/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1586 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/bug/ex6.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      662 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/bug/ex8.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      788 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/gather.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     7929 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/mpi4py.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      548 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/np_Allreduce.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      898 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/np_Bcast.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      831 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/np_Gather.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      551 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/np_Reduce.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      567 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/np_Sendrecv.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      749 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/np_point_to_point.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      602 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/np_point_to_point_2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1942 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/np_point_to_point_3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      379 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/point_to_point.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      567 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/point_to_point_2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1952 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/point_to_point_3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      471 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/reduce.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      478 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/sendrecv.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      403 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/MPI/who_am_i.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.528615 pyccel-1.9.2/tests/macro/scripts/blas/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.528615 pyccel-1.9.2/tests/macro/scripts/blas/bugs/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      363 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/blas/bugs/dnrm2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      681 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/blas/runtest_daxpy.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      467 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/blas/runtest_dcopy.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1148 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/blas/runtest_dgemm.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1186 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/blas/runtest_dgemv.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      756 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/blas/runtest_dger.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      482 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/blas/runtest_dscal.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      636 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/blas/runtest_dswap.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.528615 pyccel-1.9.2/tests/macro/scripts/lapack/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      670 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/scripts/lapack/runtest_dgbtrf.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3214 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/macro/test_macro.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.528615 pyccel-1.9.2/tests/ndarrays/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4723 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/ndarrays/conftest.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1714 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/ndarrays/leaks_check.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    47975 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/ndarrays/test_ndarrays.c
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/parser/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/parser/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1074 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/parser/scripts/comments.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3490 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/parser/test_comments.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1374 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/parser/test_headers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      358 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/parser/test_openacc.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      279 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/parser/test_openmp.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/preprocess/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/preprocess/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      943 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/preprocess/scripts/omp.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1017 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/preprocess/test_preprocess.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/pyccel/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/pyccel/project_abs_imports/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/pyccel/project_abs_imports/project/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_abs_imports/project/__init__.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/pyccel/project_abs_imports/project/folder1/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_abs_imports/project/folder1/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      288 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_abs_imports/project/folder1/mod1.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/pyccel/project_abs_imports/project/folder2/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_abs_imports/project/folder2/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      214 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_abs_imports/project/folder2/mod2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      293 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_abs_imports/project/folder2/mod3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      214 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_abs_imports/runtest.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/pyccel/project_multi_imports/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      116 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_multi_imports/file1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      130 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_multi_imports/file2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      130 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_multi_imports/file3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      179 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_multi_imports/file4.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/pyccel/project_rel_imports/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/pyccel/project_rel_imports/project/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_rel_imports/project/__init__.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/pyccel/project_rel_imports/project/folder1/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_rel_imports/project/folder1/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      288 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_rel_imports/project/folder1/mod1.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.532615 pyccel-1.9.2/tests/pyccel/project_rel_imports/project/folder2/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_rel_imports/project/folder2/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      208 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_rel_imports/project/folder2/mod2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      272 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_rel_imports/project/folder2/mod3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      214 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/project_rel_imports/runtest.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      199 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/run_import_function.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.540615 pyccel-1.9.2/tests/pyccel/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2928 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/array_binary_operation.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     4109 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/arrays_view.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.540615 pyccel-1.9.2/tests/pyccel/scripts/asserts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      117 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/asserts/unvalid_assert1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      138 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/asserts/unvalid_assert2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      162 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/asserts/unvalid_assert3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      217 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/asserts/valid_assert.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       68 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/basic_header.pyh
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1327 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/bool_comp.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2132 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/c_arrays.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.540615 pyccel-1.9.2/tests/pyccel/scripts/classes/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      627 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/classes/classes.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      729 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/classes/classes_1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      624 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/classes/classes_2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      421 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/classes/classes_3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      354 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/classes/classes_4.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      406 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/classes/classes_5.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      626 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/classes/classes_6.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      683 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/classes/generic_methods.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      251 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/concatenation.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      359 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/decorators_elemental.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      821 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/decorators_inline.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      872 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/default_args_mod.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.540615 pyccel-1.9.2/tests/pyccel/scripts/exits/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      126 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/exits/empty_exit.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      150 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/exits/negative_exit1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      130 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/exits/negative_exit2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      127 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/exits/positive_exit1.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      130 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/exits/positive_exit2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      184 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/exits/positive_exit3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      127 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/exits/zero_exit.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2236 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/expressions.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.540615 pyccel-1.9.2/tests/pyccel/scripts/folder1/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/folder1/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      283 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/folder1/folder1_funcs.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.540615 pyccel-1.9.2/tests/pyccel/scripts/folder2/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/folder2/__init__.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      283 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/folder2/folder2_funcs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      198 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/folder2/runtest_imports2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      189 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/folder2/runtest_rel_imports.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      283 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/funcs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      950 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3567 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/generic_functions.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.544615 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      285 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/hope_fib.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      591 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      814 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      265 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/hope_pisum.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1188 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      807 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/quicksort.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      280 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/simplify.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.544615 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      256 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/fib.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      535 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      786 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1192 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      782 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      264 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/simplify.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.548615 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      182 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/collisions2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      201 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/collisions3.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      218 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/collisions4.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      187 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/collisions5.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      922 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      993 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import_as.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1002 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      249 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import_as_user.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      253 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import_as_user_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      943 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      252 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import_user.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      257 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import_user_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      934 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      925 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod_as.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1019 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod_as_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      244 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod_as_user.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      249 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod_as_user_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1001 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      246 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod_user.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      250 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod_user_func.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      152 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/user_mod.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      134 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/import_syntax/user_mod2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      882 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/lapack_subroutine.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      175 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/module_init.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      116 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/module_init2.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.548615 pyccel-1.9.2/tests/pyccel/scripts/numpy/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1551 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/numpy/numpy_kernels.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2812 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/numpy/numpy_sign.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      812 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/print_integers.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      885 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/print_sp_and_end.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     2056 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/print_strings.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      381 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/print_tuples.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      704 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/return_numpy_arrays.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      418 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_decorators_inline.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      736 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_default_args.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      673 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_degree_in.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      166 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_folder_imports.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      333 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_funcs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      324 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_function_alias.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      659 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_generic_functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      150 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_imports.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      411 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_inoutfunc.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      167 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_module_init.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      305 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_module_init2.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1499 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_multiple_results.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      412 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/scripts/runtest_type_print.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)    46641 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/pyccel/test_pyccel.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      844 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/run_tests.bat
+-rwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)      899 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/run_tests_py3.sh
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.548615 pyccel-1.9.2/tests/semantic/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.548615 pyccel-1.9.2/tests/semantic/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      407 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/scripts/classes.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      825 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/scripts/expressions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1171 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/scripts/functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      128 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/scripts/ifs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      197 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/scripts/imports.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      141 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/scripts/lists.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      111 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/scripts/loops.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      307 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/scripts/tuples.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      163 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/scripts/whiles.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      311 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/scripts/zeros.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1030 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/semantic/test_semantic.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.548615 pyccel-1.9.2/tests/symbolic/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.548615 pyccel-1.9.2/tests/symbolic/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      958 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/symbolic/scripts/decorator.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      283 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/symbolic/scripts/lambdas.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      711 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/symbolic/scripts/neural_net.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1263 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/symbolic/test_symbolic.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.548615 pyccel-1.9.2/tests/syntax/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.552615 pyccel-1.9.2/tests/syntax/scripts/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      851 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/Functional_Stmts.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      157 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/annotated_comments.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       86 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/asserts.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       77 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/breaks.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      110 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/calls.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      725 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/class_member_index.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      369 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/classes.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       86 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/dels.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      190 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/dots.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      964 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/expressions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      193 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/functions.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      130 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/ifs.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      288 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/imports.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      142 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/lists.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      110 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/loops.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       80 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/prints.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      196 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/slice.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      142 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/tuples.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)       92 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/whiles.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      311 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/scripts/zeros.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     1059 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/syntax/test_syntax.py
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.552615 pyccel-1.9.2/tests/warnings/
+drwxrwxr-x   0 yamanguc  (1000) yamanguc  (1000)        0 2023-10-13 17:49:39.552615 pyccel-1.9.2/tests/warnings/semantic/
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      155 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/warnings/semantic/DECORATOR_WRONG_NUMBER_TYPES.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      145 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/warnings/semantic/FOUND_DUPLICATED_IMPORT.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      130 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      133 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/warnings/semantic/UNDEFINED_DECORATOR.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)      141 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/warnings/semantic/UNDEFINED_DECORATORS.py
+-rw-rw-r--   0 yamanguc  (1000) yamanguc  (1000)     3007 2023-10-13 17:46:43.000000 pyccel-1.9.2/tests/warnings/test_warnings.py
```

### Comparing `pyccel-1.9.1/AUTHORS` & `pyccel-1.9.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/LICENSE` & `pyccel-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/PKG-INFO` & `pyccel-1.9.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyccel
-Version: 1.9.1
+Version: 1.9.2
 Summary: UNKNOWN
 Home-page: https://github.com/pyccel/pyccel
 Author: Pyccel development team
 License: LICENSE
 Keywords: math
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
 
 # Pyccel : write Python code,  get Fortran speed
 
- [![devel_tests](https://github.com/pyccel/pyccel/actions/workflows/devel.yml/badge.svg)](https://github.com/pyccel/pyccel/actions/workflows/devel.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade) [![DOI](https://joss.theoj.org/papers/10.21105/joss.04991/status.svg)](https://doi.org/10.21105/joss.04991)
+ [![Linux unit tests](https://github.com/pyccel/pyccel/actions/workflows/linux.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/linux.yml) [![MacOSX unit tests](https://github.com/pyccel/pyccel/actions/workflows/macosx.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/macosx.yml) [![Windows unit tests](https://github.com/pyccel/pyccel/actions/workflows/windows.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/windows.yml) [![Anaconda-Linux](https://github.com/pyccel/pyccel/actions/workflows/anaconda_linux.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/anaconda_linux.yml) [![Anaconda-Windows](https://github.com/pyccel/pyccel/actions/workflows/anaconda_windows.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/anaconda_windows.yml) [![Intel unit tests](https://github.com/pyccel/pyccel/actions/workflows/intel.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/intel.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade) [![DOI](https://joss.theoj.org/papers/10.21105/joss.04991/status.svg)](https://doi.org/10.21105/joss.04991)
 
 **Pyccel** stands for Python extension language using accelerators.
 
 The aim of **Pyccel** is to provide a simple way to generate automatically, parallel low level code. The main uses would be:
 
 1.  Convert a _Python_ code (or project) into a Fortran or C code.
 2.  Accelerate _Python_ functions by converting them to _Fortran_ or _C_ functions.
@@ -100,10 +100,11 @@
 
 -   [Overview](https://github.com/pyccel/pyccel/blob/devel/developer_docs/overview.md)
 -   [How to solve an issue](https://github.com/pyccel/pyccel/blob/devel/developer_docs/how_to_solve_an_issue.md)
 -   [Review Process](https://github.com/pyccel/pyccel/blob/devel/developer_docs/review_process.md)
 -   [Development Conventions](https://github.com/pyccel/pyccel/blob/devel/developer_docs/development_conventions.md)
 -   [Tips and Tricks](https://github.com/pyccel/pyccel/blob/devel/developer_docs/tips_and_tricks.md)
 -   [Scope](https://github.com/pyccel/pyccel/blob/devel/developer_docs/scope.md)
+-   [Type Inference](https://github.com/pyccel/pyccel/blob/devel/developer_docs/type_inference.md)
 -   [Array Ordering](https://github.com/pyccel/pyccel/blob/devel/developer_docs/order_docs.md)
```

### Comparing `pyccel-1.9.1/README.md` & `pyccel-1.9.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Pyccel : write Python code,  get Fortran speed
 
- [![devel_tests](https://github.com/pyccel/pyccel/actions/workflows/devel.yml/badge.svg)](https://github.com/pyccel/pyccel/actions/workflows/devel.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade) [![DOI](https://joss.theoj.org/papers/10.21105/joss.04991/status.svg)](https://doi.org/10.21105/joss.04991)
+ [![Linux unit tests](https://github.com/pyccel/pyccel/actions/workflows/linux.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/linux.yml) [![MacOSX unit tests](https://github.com/pyccel/pyccel/actions/workflows/macosx.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/macosx.yml) [![Windows unit tests](https://github.com/pyccel/pyccel/actions/workflows/windows.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/windows.yml) [![Anaconda-Linux](https://github.com/pyccel/pyccel/actions/workflows/anaconda_linux.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/anaconda_linux.yml) [![Anaconda-Windows](https://github.com/pyccel/pyccel/actions/workflows/anaconda_windows.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/anaconda_windows.yml) [![Intel unit tests](https://github.com/pyccel/pyccel/actions/workflows/intel.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/intel.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade) [![DOI](https://joss.theoj.org/papers/10.21105/joss.04991/status.svg)](https://doi.org/10.21105/joss.04991)
 
 **Pyccel** stands for Python extension language using accelerators.
 
 The aim of **Pyccel** is to provide a simple way to generate automatically, parallel low level code. The main uses would be:
 
 1.  Convert a _Python_ code (or project) into a Fortran or C code.
 2.  Accelerate _Python_ functions by converting them to _Fortran_ or _C_ functions.
@@ -85,8 +85,9 @@
 
 -   [Overview](https://github.com/pyccel/pyccel/blob/devel/developer_docs/overview.md)
 -   [How to solve an issue](https://github.com/pyccel/pyccel/blob/devel/developer_docs/how_to_solve_an_issue.md)
 -   [Review Process](https://github.com/pyccel/pyccel/blob/devel/developer_docs/review_process.md)
 -   [Development Conventions](https://github.com/pyccel/pyccel/blob/devel/developer_docs/development_conventions.md)
 -   [Tips and Tricks](https://github.com/pyccel/pyccel/blob/devel/developer_docs/tips_and_tricks.md)
 -   [Scope](https://github.com/pyccel/pyccel/blob/devel/developer_docs/scope.md)
+-   [Type Inference](https://github.com/pyccel/pyccel/blob/devel/developer_docs/type_inference.md)
 -   [Array Ordering](https://github.com/pyccel/pyccel/blob/devel/developer_docs/order_docs.md)
```

### Comparing `pyccel-1.9.1/ci_tools/annotation_helpers.py` & `pyccel-1.9.2/ci_tools/annotation_helpers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/basic_json_check_output.py` & `pyccel-1.9.2/ci_tools/basic_json_check_output.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/bot_clean_up.py` & `pyccel-1.9.2/ci_tools/bot_clean_up.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """ Script run after a check run to trigger coverage tests if necessary, and change the draft status if necessary.
 """
 import json
 import os
+import sys
 from bot_tools.bot_funcs import Bot, test_dependencies, pr_test_keys as bot_pr_test_keys
 
 pr_test_keys = list(bot_pr_test_keys) + ['Codacy']
 
 if __name__ == '__main__':
     # Parse event payload from $GITHUB_EVENT_PATH variable
     # (documented here : https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables)
@@ -59,14 +60,17 @@
         draft = bot.is_pr_draft()
 
         if not draft:
 
             events = bot.GAI.get_events(pr_id)
 
             shas = [e.get('sha', None) for e in events]
+            if events[-1].get('event', None) == 'closed':
+                sys.exit(0)
+
             print(shas)
             print([e.get('event', None) for e in events])
             page = 1
             start_idx = -1
             while start_idx == -1:
                 try:
                     start_idx = next(i for i,s in enumerate(shas) if s == event['check_run']['head_sha'])
```

### Comparing `pyccel-1.9.1/ci_tools/bot_comment_react.py` & `pyccel-1.9.2/ci_tools/bot_comment_react.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Script run as a reaction to a comment left on a pull request.
 """
 import json
 import os
-from bot_tools.bot_funcs import Bot, pr_test_keys
+from bot_tools.bot_funcs import Bot, pr_test_keys, trust_givers
 
 def get_unique_test_list(keys):
     """
     Get a list of unique tests which should be run.
 
     Get a list of all the tests which should be run. The treatments to
     obtain this list remove duplicate tests. It also expands the `pr_tests`
@@ -55,17 +55,20 @@
     command_words = command.split()
 
     bot = Bot(pr_id = pr_id)
 
     if command_words[:2] == ['show', 'tests']:
         bot.show_tests()
 
+    elif command_words[0] == 'checklist':
+        bot.fill_checklist(event['comment']['url'], event['comment']['user']['login'])
+
     elif command_words[0] == 'run':
         if bot.is_user_trusted(event['comment']['user']['login']):
-            bot.run_tests(get_unique_test_list(command_words[1:]))
+            bot.run_tests(get_unique_test_list(command_words[1:]), force_run = bot.is_pr_fork())
         else:
             bot.warn_untrusted()
 
     elif command_words[0] == 'try':
         if bot.is_user_trusted(event['comment']['user']['login']):
             print(command_words, get_unique_test_list(command_words[2:]), command_words[1])
             bot.run_tests(get_unique_test_list(command_words[2:]), command_words[1])
@@ -74,13 +77,13 @@
 
     elif command_words[:3] == ['mark', 'as', 'ready']:
         if bot.is_user_trusted(event['comment']['user']['login']):
             bot.request_mark_as_ready()
         else:
             bot.warn_untrusted()
 
-    elif command_words[:2] == ['trust', 'user'] and len(command_words)==3 and event['comment']['user']['login'] in Bot.trust_givers:
+    elif command_words[:2] == ['trust', 'user'] and len(command_words)==3 and event['comment']['user']['login'] in trust_givers:
 
         bot.indicate_trust(command_words[2])
 
     else:
         bot.show_commands()
```

### Comparing `pyccel-1.9.1/ci_tools/bot_hello.py` & `pyccel-1.9.2/ci_tools/bot_hello.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         new_user = not has_merged_pr
     else:
         new_user = True
 
     # Choose appropriate message to welcome author
     file = 'welcome_newcomer.txt' if new_user else 'welcome_friend.txt'
 
-    bot.leave_comment(message_from_file(file) + message_from_file('checklist.txt'))
+    bot.leave_comment(message_from_file(file))
 
     # Ensure PR is draft
     if not event['pull_request']['draft']:
         bot.mark_as_draft()
 
     # If unknown user ask for trust approval
     if not trusted_user:
```

### Comparing `pyccel-1.9.1/ci_tools/bot_ready_for_review.py` & `pyccel-1.9.2/ci_tools/bot_ready_for_review.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/bot_review_react.py` & `pyccel-1.9.2/ci_tools/bot_review_react.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/bot_tools/bot_funcs.py` & `pyccel-1.9.2/ci_tools/bot_tools/bot_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .github_api_interactions import GitHubAPIInteractions
 
 default_python_versions = {
         'anaconda_linux': '3.10',
         'anaconda_windows': '3.10',
         'coverage': '3.7',
         'docs': '3.8',
+        'intel': '3.9',
         'linux': '3.7',
         'macosx': '3.10',
         'pickle_wheel': '3.7',
         'pickle': '3.8',
         'editable_pickle': '3.8',
         'pyccel_lint': '3.8',
         'pylint': '3.8',
@@ -26,14 +27,15 @@
         }
 
 test_names = {
         'anaconda_linux': "Unit tests on Linux with anaconda",
         'anaconda_windows': "Unit tests on Windows with anaconda",
         'coverage': "Coverage verification",
         'docs': "Check documentation",
+        'intel': "Unit tests on Linux with Intel compiler",
         'linux': "Unit tests on Linux",
         'macosx': "Unit tests on MacOSX",
         'pickle_wheel': "Test pickling during wheel installation",
         'pickle': "Test pickling during source installation",
         'editable_pickle': "Test pickling during editable source installation",
         'pyccel_lint': "Pyccel best practices",
         'pylint': "Python linting",
@@ -411,28 +413,28 @@
 
         Returns
         -------
         bool
             True if the test should be run, False otherwise.
         """
         print("Checking : ", name)
-        if key in ('linux', 'windows', 'macosx', 'anaconda_linux', 'anaconda_windows', 'coverage'):
+        if key in ('linux', 'windows', 'macosx', 'anaconda_linux', 'anaconda_windows', 'coverage', 'intel'):
             has_relevant_change = lambda diff: any((f.startswith('pyccel/') or f.startswith('tests/')) \
                                                     and f.endswith('.py') and f != 'pyccel/version.py' \
                                                     for f in diff) #pylint: disable=unnecessary-lambda-assignment
         elif key in ('pyccel_lint'):
             has_relevant_change = lambda diff: any(f.startswith('pyccel/') and f.endswith('.py') \
                                                     and f != 'pyccel/version.py' for f in diff) #pylint: disable=unnecessary-lambda-assignment
         elif key in ('pylint'):
             has_relevant_change = lambda diff: any(f == 'pyccel/parser/semantic.py' for f in diff) #pylint: disable=unnecessary-lambda-assignment
         elif key in ('docs'):
             has_relevant_change = lambda diff: any(f.endswith('.py') and f != 'pyccel/version.py' \
                                                     for f in diff) #pylint: disable=unnecessary-lambda-assignment
         elif key in ('spelling'):
-            has_relevant_change = lambda diff: any(f.endswith('.md') for f in diff) #pylint: disable=unnecessary-lambda-assignment
+            has_relevant_change = lambda diff: any(f.endswith('.md') or f == '.dict_custom.txt' for f in diff) #pylint: disable=unnecessary-lambda-assignment
         elif key in ('pickle', 'pickle_wheel', 'editable_pickle'):
             has_relevant_change = lambda diff: any(f.startswith('pyccel/') and f.endswith('.py') \
                                                     and f != 'pyccel/version.py' for f in diff) #pylint: disable=unnecessary-lambda-assignment
         else:
             raise NotImplementedError(f"Please update for new has_relevant_change : {key}")
 
         for c in commit_log:
@@ -519,15 +521,21 @@
             words = []
 
         if len(words) < 3:
             self._GAI.create_comment(self._pr_id, message_from_file('set_draft_no_description.txt'))
             self.mark_as_draft()
             return False
 
-        welcome_comment = next(c for c in self._GAI.get_comments(self._pr_id) if c['user']['type'] == 'Bot' and c['body'].startswith('Hello'))
+        try:
+            welcome_comment = next(c for c in self._GAI.get_comments(self._pr_id) if c['body'].startswith('Here is your checklist.'))
+        except StopIteration:
+            self._GAI.create_comment(self._pr_id, message_from_file('missing_checklist.txt'))
+            self.mark_as_draft()
+            return False
+
         if '- [ ]' in welcome_comment['body']:
             self._GAI.create_comment(self._pr_id, message_from_file('set_draft_checklist_incomplete.txt').format(url = welcome_comment['html_url']))
             self.mark_as_draft()
             return False
 
         states = self.run_tests(pr_test_keys)
 
@@ -650,16 +658,16 @@
         Returns
         -------
         bool
             True if the user is trusted, false otherwise.
         """
         print("Trusted?")
         in_team = self._GAI.check_for_user_in_team(user, 'pyccel-dev')
-        if in_team["message"] != "Not found":
-            print("In team")
+        if "message" not in in_team:
+            print("In team: ", in_team)
             return True
         print("User not in team")
         merged_prs = self._GAI.get_prs('all')
         print(merged_prs, user)
         has_merged_pr = any(pr for pr in merged_prs if pr['user']['login'] == user and pr['merged_at'])
         if has_merged_pr:
             print("Merged PR")
@@ -892,27 +900,61 @@
         target = comment_thread[0]
         comment_id = target.get('in_reply_to_id', target['id'])
         print("id: ", comment_id)
         reply = self._GAI.create_comment(self._pr_id, message,
                                  reply_to = comment_id)
         print(reply.text)
 
+    def fill_checklist(self, comment_url, user):
+        """
+        Create the PR checklist for the user.
+
+        Create the PR checklist for the user.
+
+        Parameters
+        ----------
+        comment_url : str
+            The url where the comment was left.
+
+        user : str
+            The username of the person who left the comment.
+        """
+        body = message_from_file('checklist.txt')
+        merged_prs = self._GAI.get_prs('all')
+        has_merged_pr = any(pr for pr in merged_prs if pr['user']['login'] == user and pr['merged_at'])
+        if not has_merged_pr:
+            body += message_from_file('first_checklist.txt')
+        self._GAI.modify_comment(comment_url, body)
+
     def is_pr_draft(self):
         """
         Indicate whether the pull request is a draft.
 
         Indicate whether the pull request is a draft.
 
         Returns
         -------
         bool
             True if draft, False otherwise.
         """
         return self._pr_details['draft']
 
+    def is_pr_fork(self):
+        """
+        Indicate whether the pull request is created from a fork.
+
+        Indicate whether the pull request is created from a fork.
+
+        Returns
+        -------
+        bool
+            True if fork, False otherwise.
+        """
+        return self._pr_details['head']['repo']['full_name'] != 'pyccel/pyccel'
+
     def leave_comment(self, comment):
         """
         Leave a comment on the pull request.
 
         Leave the specified comment on the pull request.
 
         Parameters
```

### Comparing `pyccel-1.9.1/ci_tools/bot_tools/github_api_interactions.py` & `pyccel-1.9.2/ci_tools/bot_tools/github_api_interactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -445,14 +445,34 @@
         else:
             issue_type = 'issues'
             suffix = ''
         url = f"https://api.github.com/repos/{self._org}/{self._repo}/{issue_type}/{pr_id}/comments{suffix}"
         print(url)
         return self._post_request("POST", url, json={"body":comment})
 
+    def modify_comment(self, comment_url, new_body):
+        """
+        Modify an existing comment.
+
+        Modify an existing comment by replacing the body with the new text.
+
+        Parameters
+        ----------
+        comment_url : str
+            The url of the comment to be modified.
+        new_body : str
+            The new body of the comment.
+
+        Returns
+        -------
+        requests.Response
+            The response collected from the request.
+        """
+        return self._post_request("PATCH", comment_url, json={"body":new_body})
+
     def create_review(self, pr_id, commit, comment, status, comments = ()):
         """
         Create a review on the specified pull request.
 
         Create a review on the specified pull request using the API as
         described here:
         https://docs.github.com/en/rest/pulls/reviews?apiVersion=2022-11-28#create-a-review-for-a-pull-request
@@ -509,15 +529,15 @@
             The team which we are checking.
 
         Returns
         -------
         dict
             A dictionary describing the result.
         """
-        url = f'https://api.github.com/orgs/{self._org}/teams/{team}/membersips/{user}'
+        url = f'https://api.github.com/orgs/{self._org}/teams/{team}/memberships/{user}'
         return self._post_request("GET", url).json()
 
     def get_prs(self, state='open'):
         """
         Get a list of all pull requests in the repository.
 
         Use the API to get a list of all pull requests in the repository which have
```

### Comparing `pyccel-1.9.1/ci_tools/check_new_coverage.py` & `pyccel-1.9.2/ci_tools/check_new_coverage.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/check_pylint_commands.py` & `pyccel-1.9.2/ci_tools/check_pylint_commands.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/check_python_capitalisation.py` & `pyccel-1.9.2/ci_tools/check_python_capitalisation.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/check_slots.py` & `pyccel-1.9.2/ci_tools/check_slots.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/complete_check_run.py` & `pyccel-1.9.2/ci_tools/complete_check_run.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/coverage_analysis_tools.py` & `pyccel-1.9.2/ci_tools/coverage_analysis_tools.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/devel_branch_tests.py` & `pyccel-1.9.2/ci_tools/devel_branch_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,7 +10,8 @@
     bot.run_tests(['windows'], '3.7', force_run = True)
     bot.run_tests(['macosx'], '3.9', force_run = True)
     bot.run_tests(['pickle'], '3.8', force_run = True)
     bot.run_tests(['editable_pickle'], '3.8', force_run = True)
     bot.run_tests(['pickle_wheel'], '3.7', force_run = True)
     bot.run_tests(['anaconda_linux'], '3.10', force_run = True)
     bot.run_tests(['anaconda_windows'], '3.10', force_run = True)
+    bot.run_tests(['intel'], '3.9', force_run = True)
```

### Comparing `pyccel-1.9.1/ci_tools/fetch_artifacts.py` & `pyccel-1.9.2/ci_tools/fetch_artifacts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/git_evaluation_tools.py` & `pyccel-1.9.2/ci_tools/git_evaluation_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,17 @@
                 changes[current_file_name] = {}
                 changes[current_file_name]['addition'] = current_file_additions
                 changes[current_file_name]['deletion'] = current_file_deletions
                 current_file_additions = []
                 current_file_deletions = []
             current_file_name = l.split(' ')[3][2:]
             i+=1
+        elif l.startswith('++') and '/dev/null' in l:
+            current_file_name = None
+            i += 1
         elif l.startswith('@@'):
             line_info = l.split('@@')[1].split()
             for info in line_info:
                 key = info[0]
                 info = info[1:]
                 if ',' in info:
                     line_num, n_lines = [int(li) for li in info.split(',')]
```

### Comparing `pyccel-1.9.1/ci_tools/json_pytest_output.py` & `pyccel-1.9.2/ci_tools/json_pytest_output.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/list_docs_tovalidate.py` & `pyccel-1.9.2/ci_tools/list_docs_tovalidate.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/parse_pylint_output.py` & `pyccel-1.9.2/ci_tools/parse_pylint_output.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/process_results.py` & `pyccel-1.9.2/ci_tools/process_results.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/setup_check_run.py` & `pyccel-1.9.2/ci_tools/setup_check_run.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """ Script called to create a check run for a job in a workflow dispatch.
 """
 import json
 import os
+import sys
 from bot_tools.bot_funcs import Bot
 
 if __name__ == '__main__':
     input_check_run_id = os.environ["GITHUB_CHECK_RUN_ID"]
 
     bot = Bot(pr_id = os.environ.get('PR_ID', 0), check_run_id = input_check_run_id, commit = os.environ["COMMIT"])
 
     if input_check_run_id == "":
         # Parse event payload from $GITHUB_EVENT_PATH variable
         # (documented here : https://docs.github.com/en/actions/learn-github-actions/variables#default-environment-variables)
         # The contents of this json file depend on the triggering event and are
         # described here :  https://docs.github.com/en/webhooks-and-events/webhooks/webhook-events-and-payloads
-        with open(os.environ["GITHUB_EVENT_PATH"], encoding="utf-8") as event_file:
-            event = json.load(event_file)
-        workflow_file = event["workflow"]
-        test_key = os.path.splitext(os.path.basename(workflow_file))[0]
+        test_key = sys.argv[1]
         posted = bot.create_in_progress_check_run(test_key)
     else:
         posted = bot.post_in_progress(int(os.environ['GITHUB_RUN_ATTEMPT']) > 1)
 
     run_id = posted['id']
     try:
         pr_id = bot.get_pr_id()
```

### Comparing `pyccel-1.9.1/ci_tools/summarise_doccoverage.py` & `pyccel-1.9.2/ci_tools/summarise_doccoverage.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/ci_tools/summarise_pyspelling.py` & `pyccel-1.9.2/ci_tools/summarise_pyspelling.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/CONTRIBUTING.md` & `pyccel-1.9.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/builtin-functions.md` & `pyccel-1.9.2/docs/builtin-functions.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/compiler.md` & `pyccel-1.9.2/docs/compiler.md`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 pyccel example.py --compiler=intel
 ```
 or
 ```python
 epyccel(my_func, compiler='intel')
 ```
 
+It is also possible to change the default compiler family by setting the environment variable `PYCCEL_DEFAULT_COMPILER`.
+
 ## User-defined compiler
 
 The user can also define their own compiler in a JSON file. To use this definition, the location of the JSON file must be passed to the _compiler_ argument. The JSON file must define the following:
 
 -   `exec` : The name of the executable
 -   `mpi_exec` : The name of the MPI executable
 -   `language` : The language handled by this compiler
```

### Comparing `pyccel-1.9.1/docs/const_keyword.md` & `pyccel-1.9.2/docs/const_keyword.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/decorators.md` & `pyccel-1.9.2/docs/decorators.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/function-pointers-as-arguments.md` & `pyccel-1.9.2/docs/function-pointers-as-arguments.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/header-files.md` & `pyccel-1.9.2/docs/header-files.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/installation.md` & `pyccel-1.9.2/docs/installation.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/ndarrays.md` & `pyccel-1.9.2/docs/ndarrays.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/numpy-functions.md` & `pyccel-1.9.2/docs/numpy-functions.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/openmp.md` & `pyccel-1.9.2/docs/openmp.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/quickstart.md` & `pyccel-1.9.2/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/docs/templates.md` & `pyccel-1.9.2/docs/templates.md`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/basic.py` & `pyccel-1.9.2/pyccel/ast/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/bind_c.py` & `pyccel-1.9.2/pyccel/ast/bind_c.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/bitwise_operators.py` & `pyccel-1.9.2/pyccel/ast/bitwise_operators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/builtin_imports.py` & `pyccel-1.9.2/pyccel/ast/builtin_imports.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/builtins.py` & `pyccel-1.9.2/pyccel/ast/builtins.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from pyccel.errors.errors import PyccelError
 
 from pyccel.utilities.stage import PyccelStage
 
 from .basic     import Basic, PyccelAstNode
 from .datatypes import (NativeInteger, NativeBool, NativeFloat,
                         NativeComplex, NativeString, str_dtype,
-                        NativeGeneric, default_precision)
+                        NativeGeneric)
 from .internals import PyccelInternalFunction, max_precision, Slice
 from .literals  import LiteralInteger, LiteralFloat, LiteralComplex, Nil
 from .literals  import Literal, LiteralImaginaryUnit, get_default_literal_value
 from .literals  import LiteralString
 from .operators import PyccelAdd, PyccelAnd, PyccelMul, PyccelIsNot
 from .operators import PyccelMinus, PyccelUnarySub, PyccelNot
 from .variable  import IndexedElement
@@ -402,15 +402,25 @@
 
     @property
     def arg(self):
         return self._arg
 
 #==============================================================================
 class PythonTuple(PyccelAstNode):
-    """ Represents a call to Python's native tuple() function.
+    """
+    Class representing a call to Python's native tuple() function.
+
+    Class representing a call to Python's native tuple() function
+    which either converts an object to a tuple or initialises a
+    literal tuple.
+
+    Parameters
+    ----------
+    *args : tuple of PyccelAstNode
+        The arguments passed to the tuple function.
     """
     __slots__ = ('_args','_inconsistent_shape','_is_homogeneous',
             '_dtype','_precision','_rank','_shape','_order')
     _iterable        = True
     _attribute_nodes = ('_args',)
 
     def __init__(self, *args):
@@ -464,19 +474,22 @@
 
                 inner_shape = [() if a.rank == 0 else a.shape for a in args]
                 self._rank = max(a.rank for a in args) + 1
                 self._shape = (LiteralInteger(len(args)), ) + inner_shape[0]
                 self._rank  = len(self._shape)
 
         else:
-            self._rank      = max(a.rank for a in args) + 1
+            max_rank = max(a.rank for a in args)
+            self._rank      = max_rank + 1
             self._dtype     = NativeGeneric()
             self._precision = 0
             if self._rank == 1:
                 self._shape     = (LiteralInteger(len(args)), )
+            elif any(a.rank != max_rank for a in args):
+                self._shape     = (LiteralInteger(len(args)), ) + (None,)*(self._rank-1)
             else:
                 self._shape     = (LiteralInteger(len(args)), ) + args[0].shape
 
         self._order = None if self._rank < 2 else 'C'
 
     def __getitem__(self,i):
         def is_int(a):
```

### Comparing `pyccel-1.9.1/pyccel/ast/c_concepts.py` & `pyccel-1.9.2/pyccel/ast/c_concepts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/class_defs.py` & `pyccel-1.9.2/pyccel/ast/class_defs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/core.py` & `pyccel-1.9.2/pyccel/ast/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2562,17 +2562,31 @@
     @property
     def results(self):
         """ List of variables which are the function results """
         return self._results
 
     @property
     def body(self):
-        """ CodeBlock containing all the statements in the function """
+        """
+        CodeBlock containing all the statements in the function.
+
+        Return a CodeBlock containing all the statements in the function.
+        """
         return self._body
 
+    @body.setter
+    def body(self, body):
+        if iterable(body):
+            body = CodeBlock(body)
+        elif not isinstance(body, CodeBlock):
+            raise TypeError('body must be an iterable or a CodeBlock')
+        self._body.remove_user_node(self)
+        self._body = body
+        self._body.set_current_user_node(self)
+
     @property
     def local_vars(self):
         """
         List of variables defined in the function.
 
         A list of all variables which are local to the function. This
         includes arguments, results, and variables defined inside the
@@ -3319,14 +3333,20 @@
 
     @property
     def name(self):
         return self._name
 
     @property
     def attributes(self):
+        """
+        The attributes of a class.
+
+        Returns a tuple containing the attributes of a ClassDef.
+        Each element within the tuple is of type Variable.
+        """
         return self._attributes
 
     @property
     def methods(self):
         return self._methods
 
     @property
@@ -3367,16 +3387,64 @@
         attribute's name."""
 
         d_attributes = {}
         for i in self.attributes:
             d_attributes[i.name] = i
         return d_attributes
 
-    # TODO add other attributes?
+    def add_new_attribute(self, attr):
+        """
+        Add a new attribute to the current class.
+
+        Add a new attribute to the current ClassDef.
+
+        Parameters
+        ----------
+        attr : Variable
+            The Variable that will be added.
+        """
+
+        if not isinstance(attr, Variable):
+            raise TypeError("Attributes must be Variables")
+        attr.set_current_user_node(self)
+        self._attributes += (attr,)
+
+    def add_new_method(self, method):
+        """
+        Add a new method to the current class.
+
+        Add a new method to the current ClassDef.
+
+        Parameters
+        ----------
+        method : FunctionDef
+            The Method that will be added.
+        """
+
+        if not isinstance(method, FunctionDef):
+            raise TypeError("Method must be FunctionDef")
+        method.set_current_user_node(self)
+        self._methods += (method,)
+
+    def add_new_interface(self, interface):
+        """
+        Add a new interface to the current class.
+
+        Add a new interface to the current ClassDef.
+
+        Parameters
+        ----------
+        interface : FunctionDef
+            The interface that will be added.
+        """
 
+        if not isinstance(interface, Interface):
+            raise TypeError("Argument 'interface' must be of type Interface")
+        interface.set_current_user_node(self)
+        self._interfaces += (interface,)
 
     def get_attribute(self, O, attr):
         """Returns the attribute attr of the class O of instance self."""
 
         if not isinstance(attr, str):
             raise TypeError('Expecting attribute to be a string')
```

### Comparing `pyccel-1.9.1/pyccel/ast/cwrapper.py` & `pyccel-1.9.2/pyccel/ast/cwrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -571,15 +571,15 @@
                        results   = [FunctionDefResult(Variable(dtype=PyccelPyObject(), name = 'o', memory_handling='alias'))])
 
     return cast_func
 
 # Functions definitions are defined in pyccel/stdlib/cwrapper/cwrapper.c
 c_to_py_registry = {
     (NativeBool(), -1)     : 'Bool_to_PyBool',
-    (NativeInteger(), -1)  : 'Int'+str(default_precision['int']*8)+'_to_PyLong',
+    (NativeInteger(), -1)  : 'Int'+str(default_precision[NativeInteger()]*8)+'_to_PyLong',
     (NativeInteger(), 1)   : 'Int8_to_NumpyLong',
     (NativeInteger(), 2)   : 'Int16_to_NumpyLong',
     (NativeInteger(), 4)   : 'Int32_to_NumpyLong',
     (NativeInteger(), 8)   : 'Int64_to_NumpyLong',
     (NativeFloat(), 4)     : 'Float_to_NumpyDouble',
     (NativeFloat(), 8)     : 'Double_to_NumpyDouble',
     (NativeFloat(), -1)    : 'Double_to_PyDouble',
```

### Comparing `pyccel-1.9.1/pyccel/ast/datatypes.py` & `pyccel-1.9.2/pyccel/ast/datatypes.py`

 * *Files 11% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     'Float',
     'String',
     'Void',
 	'NativeNumeric',
 #    '_Symbol',
     'default_precision',
     'dtype_and_precision_registry',
-    'dtype_registry'
 )
 
 #==============================================================================
 iso_c_binding = {
     "integer" : {
         1  : 'C_INT8_T',
         2  : 'C_INT16_T',
@@ -89,64 +88,57 @@
     'C_DOUBLE'              : 'f64',
     'C_LONG_DOUBLE'         : 'f128',
     'C_FLOAT_COMPLEX'       : 'c32',
     'C_DOUBLE_COMPLEX'      : 'c64',
     'C_LONG_DOUBLE_COMPLEX' : 'c128',
     'C_BOOL'                : 'b1'
 }
-default_precision = {'float': 8,
-                    'int': numpy.dtype(int).alignment,
-                    'integer': numpy.dtype(int).alignment,
-                    'complex': 8,
-                    'bool':-1}
-dtype_and_precision_registry = { 'float':('float', -1),
-                                 'double':('float', -1),
-                                 'real':('float', -1),
-                                 'pythonfloat':('float', -1), # built-in float
-                                 'float32':('float',4),
-                                 'float64':('float',8),
-                                 'f4':('float',4),
-                                 'f8':('float',8),
-                                 'pythoncomplex':('complex', -1),
-                                 'complex':('complex', -1),  # to create numpy array with dtype='complex'
-                                 'complex64':('complex',4),
-                                 'complex128':('complex',8),
-                                 'c8':('complex',4),
-                                 'c16':('complex',8),
-                                 'int8' :('int',1),
-                                 'int16':('int',2),
-                                 'int32':('int',4),
-                                 'int64':('int',8),
-                                 'i1' :('int',1),
-                                 'i2':('int',2),
-                                 'i4':('int',4),
-                                 'i8':('int',8),
-                                 'int'  :('int', -1),
-                                 'pythonint'  :('int', -1),
-                                 'integer':('int',-1),
-                                 'bool' :('bool',-1),
-                                 'b1' :('bool',-1),
-                                 'pythonbool' :('bool',-1)}
 
+#==============================================================================
 
 class DataType(metaclass=Singleton):
-    """Base class representing native datatypes"""
+    """
+    Base class representing native datatypes.
+
+    The base class from which all data types must inherit.
+    """
     __slots__ = ()
     _name = '__UNDEFINED__'
 
     @property
     def name(self):
+        """
+        Get the name of the datatype.
+
+        Get the name of the datatype.
+        """
         return self._name
 
     def __str__(self):
         return str(self.name).lower()
 
     def __repr__(self):
         return str(self.__class__.__name__)+'()'
 
+    def __reduce__(self):
+        """
+        Function called during pickling.
+
+        For more details see : https://docs.python.org/3/library/pickle.html#object.__reduce__.
+        This function is necessary to ensure that DataTypes remain singletons.
+
+        Returns
+        -------
+        callable
+            A callable to create the object.
+        args
+            A tuple containing any arguments to be passed to the callable.
+        """
+        return (self.__class__, ())
+
 class NativeBool(DataType):
     """Class representing boolean datatype"""
     __slots__ = ()
     _name = 'Bool'
 
 class NativeInteger(DataType):
     """Class representing integer datatype"""
@@ -214,25 +206,49 @@
 Cmplx          = NativeComplex()
 Void           = NativeVoid()
 Nil            = NativeNil()
 String         = NativeString()
 _Symbol        = NativeSymbol()
 Generic        = NativeGeneric()
 
-dtype_registry = {'bool': Bool,
-                  'int': Int,
-                  'integer': Int,
-                  'float'   : Float,
-                  'complex': Cmplx,
-                  'void': Void,
-                  'nil': Nil,
-                  'symbol': _Symbol,
-                  '*': Generic,
-                  'str': String}
-
+dtype_and_precision_registry = { 'float' : (Float, -1),
+                                 'double' : (Float, -1),
+                                 'real' : (Float, -1),
+                                 'float32' : (Float,4),
+                                 'float64' : (Float,8),
+                                 'f4' : (Float,4),
+                                 'f8' : (Float,8),
+                                 'complex' : (Cmplx, -1),
+                                 'complex64' : (Cmplx,4),
+                                 'complex128' : (Cmplx,8),
+                                 'c8' : (Cmplx,4),
+                                 'c16' : (Cmplx,8),
+                                 'int8' :(Int,1),
+                                 'int16' : (Int,2),
+                                 'int32' : (Int,4),
+                                 'int64' : (Int,8),
+                                 'i1' :(Int,1),
+                                 'i2' : (Int,2),
+                                 'i4' : (Int,4),
+                                 'i8' : (Int,8),
+                                 'int'  :(Int, -1),
+                                 'integer' : (Int,-1),
+                                 'bool' :(Bool,-1),
+                                 'b1' :(Bool,-1),
+                                 'void' : (Void, 0),
+                                 'nil' : (Nil, 0),
+                                 'symbol' : (_Symbol, 0),
+                                 '*' : (Generic, 0),
+                                 'str' : (String, 0),
+                                 }
+
+default_precision = {Float : 8,
+                     Int : numpy.dtype(int).alignment,
+                     Cmplx : 8,
+                     Bool : -1}
 
 class UnionType:
     """ Class representing multiple different possible
     datatypes for a function argument. If multiple
     arguments have union types then the result is a
     cross product of types
     """
@@ -291,14 +307,16 @@
         prefix = 'Pyccel{0}'.format(prefix)
 
     newclass = type(prefix + name, (BaseClass,),
                     {"__init__": __init__,
                      "_name": name,
                      "prefix": prefix,
                      "alias": name})
+
+    dtype_and_precision_registry[name] = (newclass(), 0)
     return newclass
 
 def is_pyccel_datatype(expr):
     return isinstance(expr, CustomDataType)
 
 def is_iterable_datatype(dtype):
     """Returns True if dtype is an iterable class."""
@@ -314,36 +332,35 @@
 def is_with_construct_datatype(dtype):
     """Returns True if dtype is an with_construct class."""
     if is_pyccel_datatype(dtype):
         return dtype.is_with_construct
     else:
         return False
 
-# TODO check the use of Floats
 def datatype(arg):
-    """Returns the datatype singleton for the given dtype.
+    """
+    Get the datatype indicated by a string.
 
-    arg : str or pyccel expression
-        If a str ('bool', 'int', 'float','complex', or 'void'), return the
-        singleton for the corresponding dtype. If a pyccel expression, return
-        the datatype that best fits the expression. This is determined from the
-        assumption system. For more control, use the `DataType` class directly.
+    Return the datatype singleton for the dtype described
+    by the argument.
 
-    Returns:
-        DataType
+    Parameters
+    ----------
+    arg : str
+        Return the singleton for the corresponding dtype.
 
+    Returns
+    -------
+    DataType
+        The data type described by the string.
     """
-
-
     if isinstance(arg, str):
-        if arg.lower() not in dtype_registry:
+        if arg not in dtype_and_precision_registry:
             raise ValueError("Unrecognized datatype " + arg)
-        return dtype_registry[arg]
-    if isinstance(arg, DataType):
-        return dtype_registry[arg.name.lower()]
+        return dtype_and_precision_registry[arg][0]
     else:
         raise TypeError('Expecting a DataType')
 
 def str_dtype(dtype):
 
     """
     Get a string describing a datatype.
```

### Comparing `pyccel-1.9.1/pyccel/ast/functionalexpr.py` & `pyccel-1.9.2/pyccel/ast/functionalexpr.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/headers.py` & `pyccel-1.9.2/pyccel/ast/headers.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,24 +14,22 @@
 from .datatypes         import datatype, DataTypeFactory, UnionType, default_precision
 from .internals         import PyccelSymbol, Slice
 from .macros            import Macro, MacroShape, construct_macro
 from .variable          import DottedName, DottedVariable
 from .variable          import Variable
 
 __all__ = (
-    'ClassHeader',
     'FunctionHeader',
     'Header',
     'InterfaceHeader',
     'MacroFunction',
     'MacroVariable',
     'MetaVariable',
     'MethodHeader',
     'Template',
-    'VariableHeader',
 )
 
 #==============================================================================
 errors = Errors()
 
 #==============================================================================
 class Header(Basic):
@@ -78,67 +76,14 @@
            a callable that can be called
            to create the initial version of the object
            and its arguments
         """
         return (self.__class__, (self.name, self.value))
 
 #==============================================================================
-# TODO rename dtypes to arguments
-class VariableHeader(Header):
-    """Represents a variable header in the code.
-
-    name: str
-        variable name
-
-    dtypes: dict
-        a dictionary for typing
-
-    Examples
-
-    """
-    __slots__ = ('_name','_dtypes')
-
-    def __init__(self, name, dtypes):
-        if not(isinstance(dtypes, dict)):
-            raise TypeError("Expecting dtypes to be a dict.")
-
-        self._name   = name
-        self._dtypes = dtypes
-
-        super().__init__()
-
-    @property
-    def name(self):
-        return self._name
-
-    @property
-    def dtypes(self):
-        return self._dtypes
-
-    def __reduce_ex__(self, i):
-        """ Used by pickle to create an object of this class.
-
-          Parameters
-          ----------
-
-          i : int
-           protocol
-
-          Results
-          -------
-
-          out : tuple
-           A tuple of two elements
-           a callable that can be called
-           to create the initial version of the object
-           and its arguments
-        """
-        return (self.__class__, (self.name, self.dtypes))
-
-#==============================================================================
 class Template(Header):
     """Represents a template.
 
     Parameters
     ----------
     name: str
         The name of the template.
@@ -332,26 +277,27 @@
             rank = dc['rank']
             is_const = dc['is_const']
 
             order = None
             shape = None
             annotation = None
 
-            if rank and precision == -1:
-                precision = default_precision[dtype]
-
-            if rank >1:
-                order = dc['order']
-
             if isinstance(dtype, str):
                 annotation = dtype
                 try:
                     dtype = datatype(dtype)
                 except ValueError:
                     dtype = DataTypeFactory(str(dtype), ("_name"))()
+
+            if rank and precision == -1:
+                precision = default_precision[dtype]
+
+            if rank >1:
+                order = dc['order']
+
             var = Variable(dtype, var_name,
                            memory_handling=memory_handling, is_const=is_const,
                            rank=rank, shape=shape ,order=order, precision=precision,
                            is_temp=True)
 
             return var, annotation
 
@@ -561,49 +507,14 @@
         args = (self.name.split('.'),
                 self.dtypes,
                 self.results,
                 self.is_static,)
         return (self.__class__, args)
 
 #==============================================================================
-class ClassHeader(Header):
-    """Represents class header in the code.
-
-    name: str
-        class name
-
-    options: str, list, tuple
-        a list of options
-
-    Examples
-
-    >>> from pyccel.ast.headers import ClassHeader
-    >>> ClassHeader('Matrix', ('abstract', 'public'))
-    ClassHeader(Matrix, (abstract, public))
-    """
-    __slots__ = ('_name','_options')
-
-    def __init__(self, name, options):
-        if not(iterable(options)):
-            raise TypeError("Expecting options to be iterable.")
-
-        self._name    = name
-        self._options = options
-
-        super().__init__()
-
-    @property
-    def name(self):
-        return self._name
-
-    @property
-    def options(self):
-        return self._options
-
-#==============================================================================
 class InterfaceHeader(Header):
     """Represents an interface header in the code.
 
     Parameters
     ----------
     name: str
         the name used to call the functions
```

### Comparing `pyccel-1.9.1/pyccel/ast/internals.py` & `pyccel-1.9.2/pyccel/ast/internals.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 from .basic     import Basic, PyccelAstNode, Immutable
 from .datatypes import NativeInteger, default_precision
 from .literals  import LiteralInteger
 
 pyccel_stage = PyccelStage()
 
 __all__ = (
+    'AnnotatedPyccelSymbol',
     'PrecomputedCode',
-    'PyccelArraySize',
     'PyccelArrayShapeElement',
+    'PyccelArraySize',
     'PyccelInternalFunction',
     'PyccelSymbol',
     'Slice',
     'get_final_precision',
     'max_precision',
 )
 
@@ -279,21 +280,30 @@
             stop = ''
         else:
             stop = str(self.stop)
         return '{0} : {1}'.format(start, stop)
 
 
 class PyccelSymbol(str, Immutable):
-    """Symbolic placeholder for a Python variable, which has a name but no type yet.
+    """
+    Class representing a symbol in the code.
+
+    Symbolic placeholder for a Python variable, which has a name but no type yet.
     This is very generic, and it can also represent a function or a module.
 
     Parameters
     ----------
-    name : String
-        name of the symbol
+    name : str
+        Name of the symbol.
+
+    is_temp : bool
+        Indicates if the symbol is a temporary object. This either means that the
+        symbol represents an object originally named `_` in the code, or that the
+        symbol represents an object created by Pyccel in order to assign a
+        temporary object. This is sometimes necessary to facilitate the translation.
 
     Examples
     --------
     >>> from pyccel.ast.internals import PyccelSymbol
     >>> x = PyccelSymbol('x')
     x
     """
@@ -310,14 +320,60 @@
     def is_temp(self):
         """
         Indicates if this symbol represents a temporary variable created by Pyccel,
         and was not present in the original Python code [default value : False].
         """
         return self._is_temp
 
+class AnnotatedPyccelSymbol(Basic):
+    """
+    Class representing a symbol in the code which has an annotation.
+
+    Symbolic placeholder for a Python variable, which has a name but no type yet.
+    This is very generic, and it can also represent a function or a module.
+
+    Parameters
+    ----------
+    name : str
+        Name of the symbol.
+
+    annotation : SyntacticTypeAnnotation
+        The annotation describing the type that the object will have.
+
+    is_temp : bool
+        Indicates if the symbol is a temporary object. This either means that the
+        symbol represents an object originally named `_` in the code, or that the
+        symbol represents an object created by Pyccel in order to assign a
+        temporary object. This is sometimes necessary to facilitate the translation.
+    """
+    __slots__ = ('_name', '_annotation')
+    _attribute_nodes = ()
+
+    def __init__(self, name, annotation, is_temp = False):
+        self._name = PyccelSymbol(name, is_temp)
+        self._annotation = annotation
+        super().__init__()
+
+    @property
+    def name(self):
+        """
+        Get the PyccelSymbol describing the name.
+
+        Get the PyccelSymbol describing the name of the symbol in the code.
+        """
+        return self._name
+
+    @property
+    def annotation(self):
+        """
+        Get the annotation.
+
+        Get the annotation left on the symbol. This should be a type annotation.
+        """
+        return self._annotation
 
 class PrecomputedCode(Basic):
     """
     Internal helper class for storing code which must be defined by the printer
     before it is needed chronologically (e.g. for inline functions as arguments
     to the same function).
     This class should be avoided if at all possible as it may break code which
@@ -370,42 +426,56 @@
     (x, y, z)
     """
     names = names.split(',')
     symbols = [PyccelSymbol(name.strip()) for name in names]
     return tuple(symbols)
 
 
-def max_precision(objs : list, dtype = None, allow_native = True):
+def max_precision(objs : list, allow_native : bool = True):
     """
-    Returns the largest precision of an object in the list
+    Return the largest precision amongst the objects in the list.
+
+    Return the largest precision amongst the objects in the list.
 
     Parameters
     ----------
     objs : list
-           A list of PyccelAstNodes
-    dtype : Dtype class
-            If this argument is provided then only the
-            precision of objects with this dtype are
-            considered
+       A list of PyccelAstNodes.
+
+    allow_native : bool, default=True
+        Allow the final result to be a native precision (i.e. -1).
+
+    Returns
+    -------
+    int
+        The largest precision found.
     """
     if allow_native and all(o.precision == -1 for o in objs):
         return -1
-    elif dtype:
-        def_prec = default_precision[str(dtype)]
-        return max(def_prec if o.precision == -1 \
-                else o.precision for o in objs if o.dtype is dtype)
     else:
         ndarray_list = [o for o in objs if getattr(o, 'is_ndarray', False)]
         if ndarray_list:
             return get_final_precision(max(ndarray_list, key=attrgetter('precision')))
         return max(get_final_precision(o) for o in objs)
 
 
 def get_final_precision(obj):
     """
-    Get the the usable precision of an object. Ie. the precision that you
-    can use to print, eg 8 instead of -1 for a default precision float
+    Get the usable precision of an object.
+
+    Get the usable precision of an object. I.e. the precision that you
+    can use to print, e.g. 8 instead of -1 for a default precision float.
 
     If the precision is set to the default then the value of the default
-    precision is returned, otherwise the provided precision is returned
+    precision is returned, otherwise the provided precision is returned.
+
+    Parameters
+    ----------
+    obj : PyccelAstNode
+        The object whose precision we want to investigate.
+
+    Returns
+    -------
+    int
+        The precision of the object to be used in the code.
     """
-    return default_precision[str(obj.dtype)] if obj.precision == -1 else obj.precision
+    return default_precision[obj.dtype] if obj.precision == -1 else obj.precision
```

### Comparing `pyccel-1.9.1/pyccel/ast/itertoolsext.py` & `pyccel-1.9.2/pyccel/ast/itertoolsext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/literals.py` & `pyccel-1.9.2/pyccel/ast/literals.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/macros.py` & `pyccel-1.9.2/pyccel/ast/macros.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/numpy_wrapper.py` & `pyccel-1.9.2/pyccel/ast/numpy_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/numpyext.py` & `pyccel-1.9.2/pyccel/ast/numpyext.py`

 * *Files 4% similar despite different names*

```diff
@@ -386,15 +386,15 @@
         # Arrays and NumPy datatype objects have priority
         dtype_array_precisions = [p for a,d,p in zip(arrays_and_dtypes, dtypes, precisions) \
                                   if (getattr(a,'rank', 0) != 0 or isinstance(a,PyccelFunctionDef))]
         if dtype_array_precisions:
             self._precision = max(dtype_array_precisions)
         else:
             if -1 in precisions:
-                precisions.append(default_precision[str(self.dtype)])
+                precisions.append(default_precision[self.dtype])
             self._precision = max(precisions)
 
         super().__init__(*arrays_and_dtypes)
 
 #==============================================================================
 
 def process_dtype(dtype):
@@ -449,15 +449,14 @@
         if dtype not in dtype_registry:
             raise TypeError(f'Unknown type of {dtype}.')
     else:
         raise TypeError(f'Unknown type of {dtype}.')
     dtype, precision = dtype_registry[dtype]
     if precision == -1:
         precision = default_precision[dtype]
-    dtype = datatype(dtype)
 
     return dtype, precision
 
 #==============================================================================
 class NumpyNewArray(PyccelInternalFunction):
     """
     Superclass for nodes representing NumPy array allocation functions.
@@ -662,17 +661,23 @@
 
     def __getitem__(self, index):
         step = PyccelMul(index, self.step, simplify=True)
         return PyccelAdd(self.start, step, simplify=True)
 
 #==============================================================================
 class NumpySum(PyccelInternalFunction):
-    """Represents a call to  numpy.sum for code generation.
+    """
+    Represents a call to  numpy.sum for code generation.
+
+    Represents a call to  numpy.sum for code generation.
 
+    Parameters
+    ----------
     arg : list , tuple , PythonTuple, PythonList, Variable
+        The argument passed to the sum function.
     """
     __slots__ = ('_dtype','_precision')
     name = 'sum'
     _rank  = 0
     _shape = None
     _order = None
 
@@ -680,39 +685,45 @@
         if not isinstance(arg, PyccelAstNode):
             raise TypeError('Unknown type of  %s.' % type(arg))
         super().__init__(arg)
         if isinstance(arg.dtype, NativeBool):
             self._dtype = NativeInteger()
         else:
             self._dtype = arg.dtype
-        self._precision = max(arg.precision, default_precision[str(self._dtype)])
+        self._precision = max(arg.precision, default_precision[self._dtype])
 
     @property
     def arg(self):
         return self._args[0]
 
 #==============================================================================
 class NumpyProduct(PyccelInternalFunction):
-    """Represents a call to  numpy.prod for code generation.
+    """
+    Represents a call to numpy.prod for code generation.
+
+    Represents a call to numpy.prod for code generation.
 
+    Parameters
+    ----------
     arg : list , tuple , PythonTuple, PythonList, Variable
+        The argument passed to the prod function.
     """
     __slots__ = ('_arg','_dtype','_precision')
     name = 'product'
     _rank  = 0
     _shape = None
     _order = None
 
     def __init__(self, arg):
         if not isinstance(arg, PyccelAstNode):
             raise TypeError('Unknown type of  %s.' % type(arg))
         super().__init__(arg)
         self._arg = PythonList(arg) if arg.rank == 0 else self._args[0]
         self._arg = NumpyInt(self._arg) if (isinstance(arg.dtype, NativeBool) or \
-                    (isinstance(arg.dtype, NativeInteger) and get_final_precision(self._arg) < default_precision['int']))\
+                    (isinstance(arg.dtype, NativeInteger) and get_final_precision(self._arg) < default_precision[NativeInteger()]))\
                     else self._arg
         self._dtype = self._arg.dtype
         self._precision = get_final_precision(self._arg)
 
     @property
     def arg(self):
         return self._arg
@@ -860,15 +871,15 @@
         if dtype:
             self._dtype, self._precision = process_dtype(dtype)
         else:
             args      = (start, stop)
             type_info = NumpyResultType(*args)
             if type_info.dtype is NativeInteger():
                 self._dtype     = NativeFloat()
-                self._precision = default_precision['float']
+                self._precision = default_precision[self._dtype]
             else:
                 self._dtype = type_info.dtype
                 self._precision = type_info.precision
 
         self._index = Variable('int', 'linspace_index')
         self._start = start
         self._stop  = stop
@@ -1023,23 +1034,28 @@
         """ Indicates whether the function should be
         called elementwise for an array argument
         """
         return True
 
 #==============================================================================
 class NumpyRand(PyccelInternalFunction):
-
     """
-      Represents a call to  numpy.random.random or numpy.random.rand for code generation.
+    Represents a call to  numpy.random.random or numpy.random.rand for code generation.
+
+    Represents a call to  numpy.random.random or numpy.random.rand for code generation.
 
+    Parameters
+    ----------
+    *args : tuple of PyccelAstNode
+        The arguments passed to the function.
     """
     __slots__ = ('_shape','_rank','_order')
     name = 'rand'
     _dtype = NativeFloat()
-    _precision = default_precision['float']
+    _precision = default_precision[NativeFloat()]
 
     def __init__(self, *args):
         super().__init__(*args)
         self._rank  = len(args)
         self._shape = None if self._rank == 0 else args
         self._order = None if self._rank < 2 else 'C'
 
@@ -1156,22 +1172,36 @@
     def __init__(self, shape, dtype='float', order='C'):
         if not dtype:
             raise TypeError("Data type must be provided")
         super().__init__(shape, Nil(), dtype, order)
 
 #==============================================================================
 class NumpyEmpty(NumpyAutoFill):
-    """ Represents a call to numpy.empty for code generation.
+    """
+    Represents a call to numpy.empty for code generation.
+
+    Represents a call to numpy.empty for code generation.
+
+    Parameters
+    ----------
+    shape : PyccelAstNode
+        The shape of the array to be created.
+
+    dtype : PythonType, PyccelFunctionDef, LiteralString, str
+        The actual dtype passed to the NumPy function.
+
+    order : str, LiteralString
+        The order passed to the function.
     """
     __slots__ = ()
     name = 'empty'
 
     def __init__(self, shape, dtype='float', order='C'):
         if dtype in NativeNumeric:
-            precision = default_precision[str_dtype(dtype)]
+            precision = default_precision[dtype]
             dtype = DtypePrecisionToCastFunction[dtype.name][precision]
         super().__init__(shape, dtype, order)
     @property
     def fill_value(self):
         return None
 
 #==============================================================================
@@ -1453,53 +1483,104 @@
     __slots__ = ('_dtype','_precision','_shape','_rank','_order')
     @property
     def is_elemental(self):
         return True
 
 #------------------------------------------------------------------------------
 class NumpyUfuncUnary(NumpyUfuncBase):
-    """Numpy's universal function with one argument.
+    """
+    Class representing Numpy's universal function with one argument.
+
+    Class representing Numpy's universal function. All classes which
+    inherit from this class have one argument and operate on it
+    elementally. In other words it should be equivalent to write:
+    >>> for i in iterable: NumpyUfuncUnary(i)
+
+    or
+    >>> NumpyUfuncUnary(iterable)
+
+    Parameters
+    ----------
+    x : PyccelAstNode
+        The argument passed to the function.
     """
     __slots__ = ()
     def __init__(self, x):
         self._set_dtype_precision(x)
         self._set_shape_rank(x)
         self._set_order(x)
         super().__init__(x)
 
     def _set_shape_rank(self, x):
         self._shape      = x.shape
         self._rank       = x.rank
 
     def _set_dtype_precision(self, x):
+        """
+        Use the argument to calculate the dtype and precision of the result.
+
+        Use the argument to calculate the dtype and precision of the result.
+
+        Parameters
+        ----------
+        x : PyccelAstNode
+            The argument passed to the function.
+        """
         self._dtype      = x.dtype if x.dtype is NativeComplex() else NativeFloat()
-        self._precision  = default_precision[str_dtype(self._dtype)]
+        self._precision  = default_precision[self._dtype]
 
     def _set_order(self, x):
         self._order      = x.order
 
 #------------------------------------------------------------------------------
 class NumpyUfuncBinary(NumpyUfuncBase):
-    """Numpy's universal function with two arguments.
+    """
+    Class representing Numpy's universal function with two arguments.
+
+    Class representing Numpy's universal function. All classes which
+    inherit from this class have two arguments and operate on them
+    in lockstep. In other words it should be equivalent to write:
+    >>> for i,_ in enumerate(iterable1): NumpyUfuncUnary(iterable1(i), iterable2(i))
+
+    or
+    >>> NumpyUfuncUnary(iterable1, iterable2)
+
+    Parameters
+    ----------
+    x1 : PyccelAstNode
+        The first argument passed to the function.
+    x2 : PyccelAstNode
+        The second argument passed to the function.
     """
     __slots__ = ()
-    # TODO: apply Numpy's broadcasting rules to get shape/rank of output
     def __init__(self, x1, x2):
         super().__init__(x1, x2)
         self._set_dtype_precision(x1, x2)
         self._set_shape_rank(x1, x2)
         self._set_order(x1, x2)
 
     def _set_shape_rank(self, x1, x2):
         self._shape = broadcast(x1.shape, x2.shape)
         self._rank  = 0 if self._shape is None else len(self._shape)
 
     def _set_dtype_precision(self, x1, x2):
+        """
+        Use the argument to calculate the dtype and precision of the result.
+
+        Use the argument to calculate the dtype and precision of the result.
+
+        Parameters
+        ----------
+        x1 : PyccelAstNode
+            The first argument passed to the function.
+        x2 : PyccelAstNode
+            The second argument passed to the function.
+        """
         self._dtype     = NativeFloat()
-        self._precision = default_precision['float']
+        self._precision = default_precision[self._dtype]
 
     def _set_order(self, x1, x2):
         if x1.order == x2.order:
             self._order = x1.order
         else:
             self._order = None if self._rank < 2 else 'C'
 
@@ -1608,20 +1689,40 @@
     __slots__ = ()
     name = 'abs'
     def _set_dtype_precision(self, x):
         self._dtype     = NativeInteger() if x.dtype is NativeInteger() else NativeFloat()
         self._precision = get_final_precision(x)
 
 class NumpyFloor(NumpyUfuncUnary):
-    """Represent a call to the floor function in the Numpy library"""
+    """
+    Represent a call to the floor function in the Numpy library.
+
+    Represent a call to the floor function in the Numpy library.
+
+    Parameters
+    ----------
+    x : PyccelAstNode
+        The argument passed to the function.
+    """
     __slots__ = ()
     name = 'floor'
+
     def _set_dtype_precision(self, x):
+        """
+        Use the argument to calculate the dtype and precision of the result.
+
+        Use the argument to calculate the dtype and precision of the result.
+
+        Parameters
+        ----------
+        x : PyccelAstNode
+            The argument passed to the function.
+        """
         self._dtype     = NativeFloat()
-        self._precision = default_precision[str_dtype(self._dtype)]
+        self._precision = default_precision[self._dtype]
 
 class NumpyMod(NumpyUfuncBinary):
     """
     Represent a call to the `numpy.mod` function.
 
     Represent a call to the mod function in the Numpy library.
```

### Comparing `pyccel-1.9.1/pyccel/ast/omp.py` & `pyccel-1.9.2/pyccel/ast/omp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/operators.py` & `pyccel-1.9.2/pyccel/ast/operators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/scipyext.py` & `pyccel-1.9.2/pyccel/ast/scipyext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/sympy_helper.py` & `pyccel-1.9.2/pyccel/ast/sympy_helper.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/sysext.py` & `pyccel-1.9.2/pyccel/ast/sysext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/ast/utilities.py` & `pyccel-1.9.2/pyccel/ast/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 from .core          import (AsName, Import, FunctionDef, FunctionCall,
                             Allocate, Duplicate, Assign, For, CodeBlock,
                             Concatenate, Decorator, Module, PyccelFunctionDef)
 
 from .builtins      import (builtin_functions_dict,
                             PythonRange, PythonList, PythonTuple)
+from .cmathext      import cmath_mod
 from .internals     import PyccelInternalFunction, Slice
 from .itertoolsext  import itertools_mod
 from .literals      import LiteralInteger, Nil
 from .mathext       import math_mod
 from .sysext        import sys_mod
 
 from .numpyext      import (NumpyEmpty, NumpyArray, numpy_mod,
@@ -83,14 +84,15 @@
 # TODO add documentation
 builtin_import_registry = Module('__main__',
         (),(),
         imports = [
             Import('numpy', numpy_mod),
             Import('scipy', scipy_mod),
             Import('itertools', itertools_mod),
+            Import('cmath', cmath_mod),
             Import('math', math_mod),
             Import('pyccel', pyccel_mod),
             Import('sys', sys_mod),
             ])
 if sys.version_info < (3, 10):
     from .builtin_imports import python_builtin_libs
 else:
```

### Comparing `pyccel-1.9.1/pyccel/ast/variable.py` & `pyccel-1.9.2/pyccel/ast/variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,15 +179,15 @@
         self._order          = order
         self._is_argument    = is_argument
         self._is_temp        = is_temp
 
         # ------------ PyccelAstNode Properties ---------------
         if isinstance(dtype, str) or str(dtype) == '*':
 
-            dtype = datatype(str(dtype))
+            dtype = datatype(dtype)
         elif not isinstance(dtype, DataType):
             raise TypeError('datatype must be an instance of DataType.')
 
         if not isinstance(rank, int):
             raise TypeError('rank must be an instance of int.')
 
         if rank == 0:
@@ -283,14 +283,31 @@
         Indicate that the Variable's shape is unknown at compilation time.
 
         Indicate that the exact shape is unknown, e.g. if the allocate is done in
         an If block.
         """
         self._shape = [PyccelArrayShapeElement(self, LiteralInteger(i)) for i in range(self.rank)]
 
+    def set_init_shape(self, shape):
+        """
+        Set the shape that was passed to the variable upon creation.
+
+        Set the shape that was passed to the variable upon creation. Normally this can be
+        deduced when the variable was created, however this may not be the case if the
+        variable was predeclared via a header or an annotation.
+
+        Parameters
+        ----------
+        shape : tuple
+            The shape of the array. A tuple whose elements indicate the number of elements along
+            each of the dimensions of an array. The elements of the tuple should be None or PyccelAstNodes.
+        """
+        self._alloc_shape = shape
+        self._shape = self.process_shape(shape)
+
     @property
     def name(self):
         """ Name of the variable
         """
         return self._name
 
     @property
@@ -468,40 +485,49 @@
         equivalent numpy precision
         """
         if not self._is_argument:
             self._precision = get_final_precision(self)
 
     def clone(self, name, new_class = None, **kwargs):
         """
+        Create a clone of the current variable.
+
         Create a new Variable object of the chosen class
-        with the provided name and options
+        with the provided name and options. All non-specified
+        options will match the current instance.
 
         Parameters
-        ==========
-        name      : str
-                    The name of the new Variable
-        new_class : type
-                    The class of the new Variable
-                    The default is the same class
-        kwargs    : dict
-                    Dictionary containing any keyword-value
-                    pairs which are valid constructor keywords
+        ----------
+        name : str
+            The name of the new Variable.
+        new_class : type, optional
+            The class type of the new Variable (e.g. DottedVariable).
+            The default is the same class type.
+        **kwargs : dict
+            Dictionary containing any keyword-value
+            pairs which are valid constructor keywords.
+
+        Returns
+        -------
+        Variable
+            The cloned variable.
         """
 
         if (new_class is None):
             cls = self.__class__
         else:
             cls = new_class
 
         args = inspect.signature(Variable.__init__)
         new_kwargs = {k:getattr(self, '_'+k) \
                             for k in args.parameters.keys() \
                             if '_'+k in dir(self)}
         new_kwargs.update(kwargs)
         new_kwargs['name'] = name
+        new_kwargs['shape'] = self.alloc_shape
 
         return cls(**new_kwargs)
 
     def rename(self, newname):
         """ Forbidden method for renaming the variable
         """
         # The name is part of the hash so it must never change
```

### Comparing `pyccel-1.9.1/pyccel/codegen/codegen.py` & `pyccel-1.9.2/pyccel/codegen/codegen.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/codegen/compiling/basic.py` & `pyccel-1.9.2/pyccel/codegen/compiling/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/codegen/compiling/compilers.py` & `pyccel-1.9.2/pyccel/codegen/compiling/compilers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/codegen/pipeline.py` & `pyccel-1.9.2/pyccel/codegen/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         raise ValueError("conda warnings accept {off, basic,verbose}")
 
     if language is None:
         language = 'fortran'
 
     # Choose Fortran compiler
     if compiler is None:
-        compiler = 'GNU'
+        compiler = os.environ.get('PYCCEL_DEFAULT_COMPILER', 'GNU')
 
     fflags = [] if fflags is None else fflags.split()
     wrapper_flags = [] if wrapper_flags is None else wrapper_flags.split()
 
     # Get compiler object
     Compiler.acceptable_bin_paths = get_condaless_search_path(conda_warnings)
     src_compiler = Compiler(compiler, language, debug)
```

### Comparing `pyccel-1.9.1/pyccel/codegen/printing/ccode.py` & `pyccel-1.9.2/pyccel/codegen/printing/ccode.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,28 @@
 from pyccel.ast.basic     import ScopedNode
 
 from pyccel.ast.builtins  import PythonRange, PythonComplex
 from pyccel.ast.builtins  import PythonPrint, PythonType
 from pyccel.ast.builtins  import PythonList, PythonTuple
 
 from pyccel.ast.core      import Declare, For, CodeBlock
-from pyccel.ast.core      import FuncAddressDeclare, FunctionCall, FunctionCallArgument, FunctionDef
+from pyccel.ast.core      import FuncAddressDeclare, FunctionCall, FunctionCallArgument
 from pyccel.ast.core      import Allocate, Deallocate
 from pyccel.ast.core      import FunctionAddress, FunctionDefArgument
 from pyccel.ast.core      import Assign, Import, AugAssign, AliasAssign
 from pyccel.ast.core      import SeparatorComment
 from pyccel.ast.core      import Module, AsName
 
 from pyccel.ast.operators import PyccelAdd, PyccelMul, PyccelMinus, PyccelLt, PyccelGt
 from pyccel.ast.operators import PyccelAssociativeParenthesis, PyccelMod
 from pyccel.ast.operators import PyccelUnarySub, IfTernaryOperator
 
 from pyccel.ast.datatypes import NativeInteger, NativeBool, NativeComplex, NativeVoid
 from pyccel.ast.datatypes import NativeFloat, NativeTuple, datatype, default_precision
-from pyccel.ast.datatypes import CustomDataType
+from pyccel.ast.datatypes import CustomDataType, NativeString
 
 from pyccel.ast.internals import Slice, PrecomputedCode, get_final_precision, PyccelArrayShapeElement
 
 from pyccel.ast.literals  import LiteralTrue, LiteralFalse, LiteralImaginaryUnit, LiteralFloat
 from pyccel.ast.literals  import LiteralString, LiteralInteger, Literal
 from pyccel.ast.literals  import Nil
 
@@ -181,14 +181,29 @@
 
     # --------------------------- internal functions --------------------------
     'MathFactorial' : 'pyc_factorial',
     'MathGcd'       : 'pyc_gcd',
     'MathDegrees'   : 'pyc_degrees',
     'MathRadians'   : 'pyc_radians',
     'MathLcm'       : 'pyc_lcm',
+    # --------------------------- cmath functions --------------------------
+    'CmathAcos'  : 'cacos',
+    'CmathAcosh' : 'cacosh',
+    'CmathAsin'  : 'casin',
+    'CmathAsinh' : 'casinh',
+    'CmathAtan'  : 'catan',
+    'CmathAtanh' : 'catanh',
+    'CmathCos'   : 'ccos',
+    'CmathCosh'  : 'ccosh',
+    'CmathExp'   : 'cexp',
+    'CmathSin'   : 'csin',
+    'CmathSinh'  : 'csinh',
+    'CmathSqrt'  : 'csqrt',
+    'CmathTan'   : 'ctan',
+    'CmathTanh'  : 'ctanh',
 }
 
 c_library_headers = (
     "complex",
     "ctype",
     "float",
     "math",
@@ -199,54 +214,21 @@
     "stdio",
     "stdlib",
     "string",
     "tgmath",
     "inttypes",
 )
 
-dtype_registry = {('float',8)   : 'double',
-                  ('float',4)   : 'float',
-                  ('complex',8) : 'double complex',
-                  ('complex',4) : 'float complex',
-                  ('int',4)     : 'int32_t',
-                  ('int',8)     : 'int64_t',
-                  ('int',2)     : 'int16_t',
-                  ('int',1)     : 'int8_t',
-                  ('bool',-1)   : 'bool'}
-
-ndarray_type_registry = {
-                  ('float',8)   : 'nd_double',
-                  ('float',4)   : 'nd_float',
-                  ('complex',8) : 'nd_cdouble',
-                  ('complex',4) : 'nd_cfloat',
-                  ('int',8)     : 'nd_int64',
-                  ('int',4)     : 'nd_int32',
-                  ('int',2)     : 'nd_int16',
-                  ('int',1)     : 'nd_int8',
-                  ('bool',-1)   : 'nd_bool'}
-
-type_to_format = {('float',8)   : '%.12lf',
-                  ('float',4)   : '%.12f',
-                  ('complex',8) : '(%.12lf + %.12lfj)',
-                  ('complex',4) : '(%.12f + %.12fj)',
-                  ('int',4)     : '%d',
-                  ('int',8)     : LiteralString("%") + CMacro('PRId64'),
-                  ('int',2)     : LiteralString("%") + CMacro('PRId16'),
-                  ('int',1)     : LiteralString("%") + CMacro('PRId8'),
-                  ('bool',-1)   : '%s',
-                  ('string', 0) : '%s'}
-
 import_dict = {'omp_lib' : 'omp' }
 
 c_imports = {n : Import(n, Module(n, (), ())) for n in
                 ['stdlib',
                  'math',
                  'string',
                  'ndarrays',
-                 'math',
                  'complex',
                  'stdint',
                  'pyc_math_c',
                  'stdio',
                  "inttypes",
                  'stdbool',
                  'assert',
@@ -270,14 +252,48 @@
     printmethod = "_ccode"
     language = "C"
 
     _default_settings = {
         'tabwidth': 4,
     }
 
+    dtype_registry = {(NativeFloat(),8)   : 'double',
+                      (NativeFloat(),4)   : 'float',
+                      (NativeComplex(),8) : 'double complex',
+                      (NativeComplex(),4) : 'float complex',
+                      (NativeInteger(),4)     : 'int32_t',
+                      (NativeInteger(),8)     : 'int64_t',
+                      (NativeInteger(),2)     : 'int16_t',
+                      (NativeInteger(),1)     : 'int8_t',
+                      (NativeBool(),-1) : 'bool',
+                      (NativeVoid(), 0) : 'void',
+                      }
+
+    ndarray_type_registry = {
+                      (NativeFloat(),8)   : 'nd_double',
+                      (NativeFloat(),4)   : 'nd_float',
+                      (NativeComplex(),8) : 'nd_cdouble',
+                      (NativeComplex(),4) : 'nd_cfloat',
+                      (NativeInteger(),8)     : 'nd_int64',
+                      (NativeInteger(),4)     : 'nd_int32',
+                      (NativeInteger(),2)     : 'nd_int16',
+                      (NativeInteger(),1)     : 'nd_int8',
+                      (NativeBool(),-1)   : 'nd_bool'}
+
+    type_to_format = {(NativeFloat(),8)   : '%.12lf',
+                      (NativeFloat(),4)   : '%.12f',
+                      (NativeComplex(),8) : '(%.12lf + %.12lfj)',
+                      (NativeComplex(),4) : '(%.12f + %.12fj)',
+                      (NativeInteger(),4)     : '%d',
+                      (NativeInteger(),8)     : LiteralString("%") + CMacro('PRId64'),
+                      (NativeInteger(),2)     : LiteralString("%") + CMacro('PRId16'),
+                      (NativeInteger(),1)     : LiteralString("%") + CMacro('PRId8'),
+                      (NativeBool(),-1)   : '%s',
+                      (NativeString(), 0) : '%s'}
+
     def __init__(self, filename, prefix_module = None):
 
         errors.set_target(filename, 'file')
 
         super().__init__()
         self.prefix_module = prefix_module
         self._additional_imports = {'stdlib':c_imports['stdlib']}
@@ -382,15 +398,15 @@
 
         # If the data is copied from a Variable rather than a list or tuple
         # use the function array_copy_data directly
         if isinstance(arg, Variable):
             return f"array_copy_data({lhs_address}, {self._print(arg)}, 0);\n"
 
         order = lhs.order
-        rhs_dtype = self._print(rhs.dtype)
+        rhs_dtype = rhs.dtype
         declare_dtype = self.find_in_dtype_registry(rhs_dtype, rhs.precision)
         dtype = self.find_in_ndarray_type_registry(rhs_dtype, rhs.precision)
 
         flattened_list = self._flatten_list(arg)
         operations = ""
 
         # Get the variable where the data will be copied
@@ -447,59 +463,66 @@
                     operations += self._print(AugAssign(offset_var, '+', LiteralInteger(lenSubset)))
 
         if order == "F":
             operations += f"array_copy_data({lhs_address}, {self._print(copy_to)}, 0);\n" + self._print(Deallocate(copy_to))
         return operations
 
     def arrayFill(self, expr):
-        """ print the assignment of a NdArray
+        """
+        Print the assignment of a NdArray.
+
+        Print the code necessary to create and fill an ndarray.
 
-        parameters
+        Parameters
         ----------
-            expr : PyccelAstNode
-                The Assign Node used to get the lhs and rhs
-        Return
-        ------
-            String
-                Return a str that contains a call to the C function array_fill,
+        expr : PyccelAstNode
+            The Assign Node used to get the lhs and rhs.
+
+        Returns
+        -------
+        str
+            Return a str that contains a call to the C function array_fill.
         """
         rhs = expr.rhs
         lhs = expr.lhs
         code_init = ''
-        declare_dtype = self.find_in_dtype_registry(self._print(rhs.dtype), rhs.precision)
+        declare_dtype = self.find_in_dtype_registry(rhs.dtype, rhs.precision)
 
         if rhs.fill_value is not None:
             if isinstance(rhs.fill_value, Literal):
                 code_init += 'array_fill(({0}){1}, {2});\n'.format(declare_dtype, self._print(rhs.fill_value), self._print(lhs))
             else:
                 code_init += 'array_fill({0}, {1});\n'.format(self._print(rhs.fill_value), self._print(lhs))
         return code_init
 
     def _init_stack_array(self, expr):
-        """ return a string which handles the assignment of a stack ndarray
+        """
+        Return a string which handles the assignment of a stack ndarray.
+
+        Print the code necessary to initialise a ndarray on the stack.
 
         Parameters
         ----------
-            expr : PyccelAstNode
-                The Assign Node used to get the lhs and rhs
+        expr : PyccelAstNode
+            The Assign Node used to get the lhs and rhs.
+
         Returns
         -------
-            buffer_array : str
-                String initialising the stack (C) array which stores the data
-            array_init   : str
-                String containing the rhs of the initialization of a stack array
+        buffer_array : str
+            String initialising the stack (C) array which stores the data.
+        array_init   : str
+            String containing the rhs of the initialization of a stack array.
         """
         var = expr
-        dtype_str = self._print(var.dtype)
-        dtype = self.find_in_dtype_registry(dtype_str, var.precision)
-        np_dtype = self.find_in_ndarray_type_registry(dtype_str, var.precision)
+        dtype = self.find_in_dtype_registry(var.dtype, var.precision)
+        np_dtype = self.find_in_ndarray_type_registry(var.dtype, var.precision)
         shape = ", ".join(self._print(i) for i in var.alloc_shape)
         tot_shape = self._print(functools.reduce(
             lambda x,y: PyccelMul(x,y,simplify=True), var.alloc_shape))
-        declare_dtype = self.find_in_dtype_registry('int', 8)
+        declare_dtype = self.find_in_dtype_registry(NativeInteger(), 8)
 
         dummy_array_name = self.scope.get_new_name('array_dummy')
         buffer_array = "{dtype} {name}[{size}];\n".format(
                 dtype = dtype,
                 name  = dummy_array_name,
                 size  = tot_shape)
         shape_init = "({declare_dtype}[]){{{shape}}}".format(declare_dtype=declare_dtype, shape=shape)
@@ -662,21 +685,21 @@
             arg = "1"
         else:
             arg = self._print(expr.status)
         return f"{code}exit({arg});\n"
 
     def _print_PythonFloat(self, expr):
         value = self._print(expr.arg)
-        type_name = self.find_in_dtype_registry('float', expr.precision)
+        type_name = self.find_in_dtype_registry(NativeFloat(), expr.precision)
         return '({0})({1})'.format(type_name, value)
 
     def _print_PythonInt(self, expr):
         self.add_import(c_imports['stdint'])
         value = self._print(expr.arg)
-        type_name = self.find_in_dtype_registry('int', expr.precision)
+        type_name = self.find_in_dtype_registry(NativeInteger(), expr.precision)
         return '({0})({1})'.format(type_name, value)
 
     def _print_PythonBool(self, expr):
         value = self._print(expr.arg)
         return '({} != 0)'.format(value)
 
     def _print_Literal(self, expr):
@@ -702,15 +725,15 @@
 
     def _print_PythonComplex(self, expr):
         if expr.is_cast:
             value = self._print(expr.internal_var)
         else:
             value = self._print(PyccelAssociativeParenthesis(PyccelAdd(expr.real,
                             PyccelMul(expr.imag, LiteralImaginaryUnit()))))
-        type_name = self.find_in_dtype_registry('complex', expr.precision)
+        type_name = self.find_in_dtype_registry(NativeComplex(), expr.precision)
         return '({0})({1})'.format(type_name, value)
 
     def _print_LiteralImaginaryUnit(self, expr):
         self.add_import(c_imports['complex'])
         return '_Complex_I'
 
     def _print_PythonLen(self, expr):
@@ -732,17 +755,22 @@
         if isinstance(name, AsName):
             name = name.name
         # TODO: Add interfaces
         classes = ""
         funcs = ""
         for classDef in expr.module.classes:
             classes += f"struct {classDef.name} {{\n"
+            classes += ''.join(self._print(Declare(var.dtype,var)) for var in classDef.attributes)
             for method in classDef.methods:
                 method.rename(classDef.name + ("__" + method.name if not method.name.startswith("__") else method.name))
                 funcs += f"{self.function_signature(method)};\n"
+            for interface in classDef.interfaces:
+                for func in interface.functions:
+                    func.rename(classDef.name + ("__" + func.name if not func.name.startswith("__") else func.name))
+                    funcs += f"{self.function_signature(func)};\n"
             classes += "};\n"
         funcs += '\n'.join(f"{self.function_signature(f)};" for f in expr.module.funcs)
 
         global_variables = ''.join(['extern '+self._print(d) for d in expr.module.declarations if not d.variable.is_private])
 
         # Print imports last to be sure that all additional_imports have been collected
         imports = [*expr.module.imports, *self._additional_imports.values()]
@@ -886,17 +914,16 @@
             return 'cpow({}, {})'.format(b, e)
 
         self.add_import(c_imports['math'])
         b = self._print(b if b.dtype is NativeFloat() else NumpyFloat(b))
         e = self._print(e if e.dtype is NativeFloat() else NumpyFloat(e))
         code = 'pow({}, {})'.format(b, e)
         if expr.dtype is NativeInteger():
-            dtype = self._print(expr.dtype)
             prec  = expr.precision
-            cast_type = self.find_in_dtype_registry(dtype, prec)
+            cast_type = self.find_in_dtype_registry(expr.dtype, prec)
             return '({}){}'.format(cast_type, code)
         return code
 
     def _print_Import(self, expr):
         if expr.ignore:
             return ''
         if isinstance(expr.source, AsName):
@@ -932,16 +959,36 @@
                                .replace('\t', '\\t')\
                                .replace('\v', '\\v')\
                                .replace('"', '\\"')\
                                .replace("'", "\\'")
         return '"{}"'.format(format_str)
 
     def get_print_format_and_arg(self, var):
+        """
+        Get the C print format string for the object var.
+
+        Get the C print format string which will allow the generated code
+        to print the variable passed as argument.
+
+        Parameters
+        ----------
+        var : PyccelAstNode
+            The object which will be printed.
+
+        Returns
+        -------
+        arg_format : str
+            The format which should be printed in the format string of the
+            generated print expression.
+        arg : str
+            The code which should be printed in the arguments of the generated
+            print expression to print the object.
+        """
         try:
-            arg_format = type_to_format[(self._print(var.dtype), get_final_precision(var))]
+            arg_format = self.type_to_format[(var.dtype, get_final_precision(var))]
         except KeyError:
             errors.report("{} type is not supported currently".format(var.dtype), severity='fatal')
         if var.dtype is NativeComplex():
             arg = '{}, {}'.format(self._print(NumpyReal(var)), self._print(NumpyImag(var)))
         elif var.dtype is NativeBool():
             arg = '{} ? "True" : "False"'.format(self._print(var))
         else:
@@ -1048,28 +1095,76 @@
                 args_format.append(arg_format)
                 args.append(arg)
         if args_format:
             code += formatted_args_to_printf(args_format, args, end)
         return code
 
     def find_in_dtype_registry(self, dtype, prec):
+        """
+        Find the corresponding C dtype in the dtype_registry.
+
+        Find the corresponding C dtype in the dtype_registry.
+        Raise PYCCEL_RESTRICTION_TODO if not found.
+
+        Parameters
+        ----------
+        dtype : DataType
+            The data type of the expression.
+
+        prec : int
+            The precision of the expression.
+
+        Returns
+        -------
+        str
+            The code which declares the datatype in C.
+        """
         if prec == -1:
             prec = default_precision[dtype]
+
+        if dtype is NativeBool():
+            self.add_import(c_imports['stdbool'])
+        elif dtype is NativeInteger():
+            self.add_import(c_imports['stdint'])
+        elif dtype is NativeComplex():
+            self.add_import(c_imports['complex'])
+
         try :
-            return dtype_registry[(dtype, prec)]
+            return self.dtype_registry[(dtype, prec)]
         except KeyError:
             errors.report(PYCCEL_RESTRICTION_TODO,
                     symbol = "{}[kind = {}]".format(dtype, prec),
                     severity='fatal')
 
     def find_in_ndarray_type_registry(self, dtype, prec):
+        """
+        Find the descriptor for the datatype in the ndarray_type_registry.
+
+        Find the tag which allows the user to access data of the specified
+        type and precision within a ndarray.
+        Raise PYCCEL_RESTRICTION_TODO if not found.
+
+        Parameters
+        ----------
+        dtype : DataType
+            The data type of the expression.
+
+        prec : int
+            The precision of the expression.
+
+        Returns
+        -------
+        str
+            The code which declares the datatype in C.
+        """
         if prec == -1:
             prec = default_precision[dtype]
+
         try :
-            return ndarray_type_registry[(dtype, prec)]
+            return self.ndarray_type_registry[(dtype, prec)]
         except KeyError:
             errors.report(PYCCEL_RESTRICTION_TODO,
                     symbol = "{}[kind = {}]".format(dtype, prec),
                     severity='fatal')
 
     def get_declare_type(self, expr):
         """
@@ -1103,29 +1198,30 @@
         'int64_t'
 
         For an object accessed via a pointer:
         >>> v = Variable('int', 'x', is_optional=True, rank=1)
         >>> self.get_declare_type(v)
         't_ndarray*'
         """
-        dtype = self._print(expr.dtype)
+        dtype = expr.dtype
         prec  = expr.precision
         rank  = expr.rank
-        if isinstance(expr.dtype, NativeInteger):
-            self.add_import(c_imports['stdint'])
-        if not dtype.startswith("struct"):
-            dtype = self.find_in_dtype_registry(dtype, prec)
+
         if rank > 0:
             if expr.is_ndarray or isinstance(expr, HomogeneousTupleVariable):
                 if expr.rank > 15:
                     errors.report(UNSUPPORTED_ARRAY_RANK, symbol=expr, severity='fatal')
                 self.add_import(c_imports['ndarrays'])
                 dtype = 't_ndarray'
             else:
                 errors.report(PYCCEL_RESTRICTION_TODO+' (rank>0)', symbol=expr, severity='fatal')
+        elif not isinstance(dtype, CustomDataType):
+            dtype = self.find_in_dtype_registry(dtype, prec)
+        else:
+            dtype = self._print(expr.dtype)
 
         if self.is_c_pointer(expr):
             return f'{dtype}*'
         else:
             return dtype
 
     def _print_FuncAddressDeclare(self, expr):
@@ -1165,33 +1261,14 @@
 
         external = 'extern ' if expr.external else ''
 
         declaration = f'{external}{declaration_type} {variable}{init};\n'
 
         return preface + declaration
 
-    def _print_NativeBool(self, expr):
-        self.add_import(c_imports['stdbool'])
-        return 'bool'
-
-    def _print_NativeInteger(self, expr):
-        return 'int'
-
-    def _print_NativeFloat(self, expr):
-        return 'float'
-
-    def _print_NativeVoid(self, expr):
-        return 'void'
-
-    def _print_NativeComplex(self, expr):
-        self.add_import(c_imports['complex'])
-        return 'complex'
-    def _print_NativeString(self, expr):
-        return 'string'
-
     def function_signature(self, expr, print_arg_names = True):
         """
         Get the C representation of the function signature.
 
         Extract from the function definition `expr` all the
         information (name, input, output) needed to create the
         function signature and return a string describing the
@@ -1217,19 +1294,19 @@
         result_vars = [r.var for r in expr.results if not r.is_argument]
 
         n_results = len(result_vars)
 
         if n_results == 1:
             ret_type = self.get_declare_type(result_vars[0])
         elif n_results > 1:
-            ret_type = self._print(datatype('int'))
+            ret_type = self.find_in_dtype_registry(NativeInteger(), -1)
             arg_vars.extend(result_vars)
             self._additional_args.append(result_vars) # Ensure correct result for is_c_pointer
         else:
-            ret_type = self._print(datatype('void'))
+            ret_type = self.find_in_dtype_registry(NativeVoid(), 0)
 
         name = expr.name
         if not arg_vars:
             arg_code = 'void'
         else:
             def get_arg_declaration(var):
                 """ Get the code which declares the argument variable.
@@ -1265,16 +1342,15 @@
                 if isinstance(ind, tuple) and len(ind) == 1:
                     inds[i].args = ind[0]
                 if allow_negative_indexes and \
                         not isinstance(ind, LiteralInteger) and not isinstance(ind, Slice):
                     inds[i] = IfTernaryOperator(PyccelLt(ind, LiteralInteger(0)),
                         PyccelAdd(base_shape[i], ind, simplify = True), ind)
         #set dtype to the C struct types
-        dtype = self._print(expr.dtype)
-        dtype = self.find_in_ndarray_type_registry(dtype, expr.precision)
+        dtype = self.find_in_ndarray_type_registry(expr.dtype, expr.precision)
         base_name = self._print(base)
         if getattr(base, 'is_ndarray', False) or isinstance(base, HomogeneousTupleVariable):
             if expr.rank > 0:
                 #managing the Slice input
                 for i , ind in enumerate(inds):
                     if isinstance(ind, Slice):
                         inds[i] = self._new_slice_with_processed_arguments(ind, PyccelArrayShapeElement(base, i),
@@ -1287,32 +1363,39 @@
             inds = [self._cast_to(i, NativeInteger(), 8).format(self._print(i)) for i in inds]
         else:
             raise NotImplementedError(expr)
         return "GET_ELEMENT(%s, %s, %s)" % (base_name, dtype, ", ".join(inds))
 
 
     def _cast_to(self, expr, dtype, precision):
-        """ add cast to an expression when needed
-        parameters
+        """
+        Add a cast to an expression when needed.
+
+        Get a format string which provides the code to cast the object `expr`
+        to the specified dtype and precision. If the dtype and precision already
+        match then the format string will simply print the expression.
+
+        Parameters
         ----------
-            expr      : PyccelAstNode
-                the expression to be cast
-            dtype     : Datatype
-                base type of the cast
-            precision : integer
-                precision of the base type of the cast
+        expr : PyccelAstNode
+            The expression to be cast.
+        dtype : Datatype
+            The target type of the cast.
+        precision : int
+            The target precision of the cast.
 
-        Return
-        ------
-            String
-                Return format string that contains the desired cast type
-                NB: You should insert the expression to be cast in the string after using this function.
+        Returns
+        -------
+        str
+            A format string that contains the desired cast type.
+            NB: You should insert the expression to be cast in the string
+            after using this function.
         """
         if (expr.dtype != dtype or expr.precision != precision):
-            cast=self.find_in_dtype_registry(self._print(dtype), precision)
+            cast=self.find_in_dtype_registry(dtype, precision)
             return '({}){{}}'.format(cast)
         return '{}'
 
     def _print_DottedVariable(self, expr):
         """convert dotted Variable to their C equivalent"""
 
         name_code = self._print(expr.name)
@@ -1406,29 +1489,31 @@
             shape_var = DottedVariable(NativeVoid(), 'shape', lhs = variable)
             free_code = f'if ({self._print(shape_var)} != NULL)\n'
             free_code += "{{\n{}}}\n".format(self._print(Deallocate(variable)))
         elif (expr.status == 'allocated'):
             free_code += self._print(Deallocate(variable))
         self.add_import(c_imports['ndarrays'])
         shape = ", ".join(self._print(i) for i in expr.shape)
-        dtype = self._print(variable.dtype)
-        dtype = self.find_in_ndarray_type_registry(dtype, variable.precision)
-        shape_dtype = self.find_in_dtype_registry('int', 8)
+        dtype = self.find_in_ndarray_type_registry(variable.dtype, variable.precision)
+        shape_dtype = self.find_in_dtype_registry(NativeInteger(), 8)
         shape_Assign = "("+ shape_dtype +"[]){" + shape + "}"
         is_view = 'false' if variable.on_heap else 'true'
         order = "order_f" if expr.order == "F" else "order_c"
         alloc_code = f"{self._print(variable)} = array_create({variable.rank}, {shape_Assign}, {dtype}, {is_view}, {order});\n"
         return '{}{}'.format(free_code, alloc_code)
 
     def _print_Deallocate(self, expr):
         if isinstance(expr.variable, InhomogeneousTupleVariable):
             return ''.join(self._print(Deallocate(v)) for v in expr.variable)
         variable_address = self._print(ObjectAddress(expr.variable))
         if expr.variable.is_alias:
             return f'free_pointer({variable_address});\n'
+        if isinstance(expr.variable.dtype, CustomDataType):
+            Pyccel__del = expr.variable.cls_base.scope.find('__del__').name
+            return f"{Pyccel__del}({variable_address});\n"
         return f'free_array({variable_address});\n'
 
     def _print_Slice(self, expr):
         start = self._print(expr.start)
         stop = self._print(expr.stop)
         step = self._print(expr.step)
         slice_type = 'RANGE' if expr.slice_type == Slice.Range else 'ELEMENT'
@@ -1537,26 +1622,29 @@
         except KeyError:
             errors.report(PYCCEL_RESTRICTION_TODO, severity='fatal')
 
         if func_name.startswith("pyc"):
             self.add_import(c_imports['pyc_math_c'])
         else:
             if expr.dtype is NativeComplex():
-                self.add_import(c_imports['cmath'])
+                self.add_import(c_imports['complex'])
             else:
                 self.add_import(c_imports['math'])
-        args = []
-        for arg in expr.args:
-            if arg.dtype != NativeFloat() and not func_name.startswith("pyc"):
-                args.append(self._print(NumpyFloat(arg)))
-            else:
-                args.append(self._print(arg))
+        if expr.dtype is NativeComplex():
+            args = [self._print(a) for a in expr.args]
+        else:
+            args = []
+            for arg in expr.args:
+                if arg.dtype is not NativeFloat() and not func_name.startswith("pyc"):
+                    args.append(self._print(NumpyFloat(arg)))
+                else:
+                    args.append(self._print(arg))
         code_args = ', '.join(args)
-        if expr.dtype == NativeInteger():
-            cast_type = self.find_in_dtype_registry('int', expr.precision)
+        if expr.dtype is NativeInteger():
+            cast_type = self.find_in_dtype_registry(NativeInteger(), expr.precision)
             return '({0}){1}({2})'.format(cast_type, func_name, code_args)
         return '{0}({1})'.format(func_name, code_args)
 
     def _print_MathIsfinite(self, expr):
         """Convert a Python expression with a math isfinite function call to C
         function call"""
         # add necessary include
@@ -1630,15 +1718,15 @@
         '''
         if not isinstance(expr.arg, (NumpyArray, Variable, IndexedElement)):
             raise TypeError(f'Expecting a NumpyArray, given {type(expr.arg)}')
         dtype, prec, name = (expr.arg.dtype,
                              expr.arg.precision,
                              self._print(expr.arg))
         if prec == -1:
-            prec = default_precision[self._print(dtype)]
+            prec = default_precision[dtype]
 
         if isinstance(dtype, NativeInteger):
             return f'numpy_sum_int{prec * 8}({name})'
         elif isinstance(dtype, NativeFloat):
             return f'numpy_sum_float{prec * 8}({name})'
         elif isinstance(dtype, NativeComplex):
             return f'numpy_sum_complex{prec * 16}({name})'
@@ -1655,16 +1743,15 @@
             lhs = self._print(lhs_source)
 
             if isinstance(expr.endpoint, LiteralTrue):
                 cond_template = lhs + ' = {stop}'
             else:
                 cond_template = lhs + ' = {cond} ? {stop} : ' + lhs
 
-        dtype = self._print(expr.dtype)
-        v = self._cast_to(expr.stop, dtype, expr.precision).format(self._print(expr.stop))
+        v = self._cast_to(expr.stop, expr.dtype, expr.precision).format(self._print(expr.stop))
 
         init_value = template.format(
             start = self._print(expr.start),
             step  = self._print(expr.step),
             index = self._print(expr.ind),
         )
         if isinstance(expr.endpoint, LiteralFalse):
@@ -1852,15 +1939,15 @@
         self.add_import(c_imports['math'])
         # the result type of the floor division is dependent on the arguments
         # type, if all arguments are integers the result is integer otherwise
         # the result type is float
         need_to_cast = all(a.dtype is NativeInteger() for a in expr.args)
         code = ' / '.join(self._print(a if a.dtype is NativeFloat() else NumpyFloat(a)) for a in expr.args)
         if (need_to_cast):
-            cast_type = self.find_in_dtype_registry('int', expr.precision)
+            cast_type = self.find_in_dtype_registry(NativeInteger(), expr.precision)
             return "({})floor({})".format(cast_type, code)
         return "floor({})".format(code)
 
     def _print_PyccelRShift(self, expr):
         return ' >> '.join(self._print(a) for a in expr.args)
 
     def _print_PyccelLShift(self, expr):
@@ -2246,18 +2333,22 @@
                                     body=body)
 
     #================== CLASSES ==================
 
     def _print_CustomDataType(self, expr):
         return "struct " + expr.name
 
+    def _print_Del(self, expr):
+        return ''.join(self._print(var) for var in expr.variables)
+
     def _print_ClassDef(self, expr):
         methods = ''.join(self._print(method) for method in expr.methods)
-        return methods
+        interfaces = ''.join(self._print(function) for interface in expr.interfaces for function in interface.functions)
 
+        return methods + interfaces
     #=================== MACROS ==================
 
     def _print_MacroShape(self, expr):
         var = expr.argument
         if not isinstance(var, (Variable, IndexedElement)):
             raise TypeError('Expecting a variable, given {}'.format(type(var)))
         shape = var.shape
```

### Comparing `pyccel-1.9.1/pyccel/codegen/printing/codeprinter.py` & `pyccel-1.9.2/pyccel/codegen/printing/codeprinter.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/codegen/printing/cwrappercode.py` & `pyccel-1.9.2/pyccel/codegen/printing/cwrappercode.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,45 +2,37 @@
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 
 from pyccel.codegen.printing.ccode import CCodePrinter
 
-from pyccel.ast.bind_c   import BindCPointer
-from pyccel.ast.bind_c   import BindCModule, BindCFunctionDef
-
-from pyccel.ast.core import FunctionAddress, SeparatorComment
-from pyccel.ast.core import Import, Module
-
-from pyccel.ast.cwrapper    import PyBuildValueNode
-from pyccel.ast.cwrapper    import Py_None
-from pyccel.ast.cwrapper    import PyccelPyObject
-
-from pyccel.ast.literals  import LiteralString, Nil
-
+from pyccel.ast.bind_c     import BindCPointer
+from pyccel.ast.bind_c     import BindCModule, BindCFunctionDef
+from pyccel.ast.core       import FunctionAddress, SeparatorComment
+from pyccel.ast.core       import Import, Module
+from pyccel.ast.cwrapper   import PyBuildValueNode
+from pyccel.ast.cwrapper   import Py_None
+from pyccel.ast.cwrapper   import PyccelPyObject
+from pyccel.ast.literals   import LiteralString, Nil
 from pyccel.ast.c_concepts import ObjectAddress
 
-from pyccel.errors.errors   import Errors
-
-errors = Errors()
+from pyccel.errors.errors  import Errors
 
-__all__ = ["CWrapperCodePrinter", "cwrappercode"]
+__all__ = ("CWrapperCodePrinter", "cwrappercode")
 
-dtype_registry = {('pyobject'     , 0) : 'PyObject',
-                  ('pyarrayobject', 0) : 'PyArrayObject',
-                  ('void'         , 0) : 'void',
-                  ('bind_c_ptr'   , 0) : 'void'}
+errors = Errors()
 
-module_imports  = [Import('numpy_version', Module('numpy_version',(),())),
+module_imports = [Import('numpy_version', Module('numpy_version',(),())),
             Import('numpy/arrayobject', Module('numpy/arrayobject',(),())),
             Import('cwrapper', Module('cwrapper',(),()))]
 
 cwrapper_ndarray_import = Import('cwrapper_ndarrays', Module('cwrapper_ndarrays', (), ()))
 
+
 class CWrapperCodePrinter(CCodePrinter):
     """
     A printer for printing the C-Python interface.
 
     A printer to convert Pyccel's AST describing a translated module,
     to strings of C code which provide an interface between the module
     and Python code.
@@ -52,22 +44,25 @@
     filename : str
             The name of the file being pyccelised.
     target_language : str
             The language which the code was translated to [fortran/c].
     **settings : dict
             Any additional arguments which are necessary for CCodePrinter.
     """
+    dtype_registry = {**CCodePrinter.dtype_registry,
+                      (PyccelPyObject() , 0) : 'PyObject',
+                      (BindCPointer()   , 0) : 'void'}
+
     def __init__(self, filename, target_language, **settings):
         CCodePrinter.__init__(self, filename, **settings)
         self._target_language = target_language
         self._to_free_PyObject_list = []
         self._function_wrapper_names = dict()
         self._module_name = None
 
-
     # --------------------------------------------------------------------
     #                       Helper functions
     # --------------------------------------------------------------------
 
     def is_c_pointer(self, a):
         """
         Indicate whether the object is a pointer in C code.
@@ -157,47 +152,15 @@
 
         See Also
         --------
         CCodePrinter.get_declare_type : The extended function.
         """
         if expr.dtype is BindCPointer():
             return 'void*'
-        dtype = self._print(expr.dtype)
-        prec  = expr.precision
-        if dtype != "pyarrayobject":
-            return CCodePrinter.get_declare_type(self, expr)
-        else :
-            dtype = self.find_in_dtype_registry(dtype, prec)
-
-        if self.is_c_pointer(expr):
-            return f'{dtype}*'
-        else:
-            return dtype
-
-    def find_in_dtype_registry(self, dtype, prec):
-        """
-        Find the corresponding C dtype in the dtype_registry
-        raise PYCCEL_RESTRICTION_TODO if not found
-
-        Parameters
-        -----------
-        dtype : String
-            expression data type
-
-        prec  : Integer
-            expression precision
-
-        Returns
-        -------
-        dtype : String
-        """
-        try :
-            return dtype_registry[(dtype, prec)]
-        except KeyError:
-            return CCodePrinter.find_in_dtype_registry(self, dtype, prec)
+        return CCodePrinter.get_declare_type(self, expr)
 
     def _handle_is_operator(self, Op, expr):
         """
         Get the code to print an `is` or `is not` expression.
 
         Get the code to print an `is` or `is not` expression. These two operators
         function similarly so this helper function reduces code duplication.
@@ -226,36 +189,26 @@
             rhs = ObjectAddress(expr.rhs)
             lhs = self._print(lhs)
             rhs = self._print(rhs)
             return f'{lhs} {Op} {rhs}'
         else:
             return super()._handle_is_operator(Op, expr)
 
-    # -------------------------------------------------------------------
-    # Functions managing the creation of wrapper body
-    # -------------------------------------------------------------------
-
-    def _print_BindCPointer(self, expr):
-        return 'bind_c_ptr'
-
     #--------------------------------------------------------------------
     #                 _print_ClassName functions
     #--------------------------------------------------------------------
 
     def _print_DottedName(self, expr):
         names = expr.name
         return '.'.join(self._print(n) for n in names)
 
     def _print_PyInterface(self, expr):
         funcs_to_print = (*expr.functions, expr.type_check_func, expr.interface_func)
         return '\n'.join(self._print(f) for f in funcs_to_print)
 
-    def _print_PyccelPyObject(self, expr):
-        return 'pyobject'
-
     def _print_PyArg_ParseTupleNode(self, expr):
         name    = 'PyArg_ParseTupleAndKeywords'
         pyarg   = expr.pyarg
         pykwarg = expr.pykwarg
         flags   = expr.flags
         # All args are modified so even pointers are passed by address
         args    = ', '.join(f'&{a.name}' for a in expr.args)
```

### Comparing `pyccel-1.9.1/pyccel/codegen/printing/fcode.py` & `pyccel-1.9.2/pyccel/codegen/printing/fcode.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,55 +11,47 @@
 import re
 from itertools import chain
 from collections import OrderedDict
 
 import functools
 
 from pyccel.ast.basic import PyccelAstNode
+
 from pyccel.ast.bind_c import BindCPointer, BindCFunctionDef, BindCFunctionDefArgument, BindCModule
+
+from pyccel.ast.builtins import PythonInt, PythonType,PythonPrint, PythonRange
+from pyccel.ast.builtins import PythonFloat, PythonTuple
+from pyccel.ast.builtins import PythonComplex, PythonBool, PythonAbs
+from pyccel.ast.builtins import python_builtin_datatypes_dict as python_builtin_datatypes
+
 from pyccel.ast.core import get_iterable_ranges
 from pyccel.ast.core import FunctionDef, InlineFunctionDef
 from pyccel.ast.core import SeparatorComment, Comment
 from pyccel.ast.core import ConstructorCall
 from pyccel.ast.core import FunctionCallArgument
 from pyccel.ast.core import ErrorExit, FunctionAddress
-from pyccel.ast.core import Return, Module
-from pyccel.ast.core import Import
-from pyccel.ast.itertoolsext import Product
-from pyccel.ast.core import (Assign, AliasAssign, Declare,
-                             CodeBlock, AsName, EmptyNode,
-                             If, IfSection, For, Deallocate)
-
-from pyccel.ast.variable  import (Variable,
-                             IndexedElement,
-                             InhomogeneousTupleVariable,
-                             DottedName, )
-
-from pyccel.ast.operators      import PyccelAdd, PyccelMul, PyccelMinus
-from pyccel.ast.operators      import PyccelMod
-from pyccel.ast.operators      import PyccelUnarySub, PyccelLt, PyccelGt, IfTernaryOperator
-
-from pyccel.ast.core      import FunctionCall, DottedFunctionCall, PyccelFunctionDef
-
-from pyccel.ast.builtins  import (PythonInt, PythonType,
-                                  PythonPrint, PythonRange,
-                                  PythonFloat, PythonTuple)
-from pyccel.ast.builtins  import PythonComplex, PythonBool, PythonAbs
+from pyccel.ast.core import Return, Module, If, IfSection, For
+from pyccel.ast.core import Import, CodeBlock, AsName, EmptyNode
+from pyccel.ast.core import Assign, AliasAssign, Declare, Deallocate
+from pyccel.ast.core import FunctionCall, DottedFunctionCall, PyccelFunctionDef
+
 from pyccel.ast.datatypes import is_pyccel_datatype
 from pyccel.ast.datatypes import is_iterable_datatype, is_with_construct_datatype
 from pyccel.ast.datatypes import NativeSymbol, NativeString, str_dtype
 from pyccel.ast.datatypes import NativeInteger, NativeBool, NativeFloat, NativeComplex
 from pyccel.ast.datatypes import iso_c_binding
 from pyccel.ast.datatypes import iso_c_binding_shortcut_mapping
 from pyccel.ast.datatypes import NativeRange, NativeNumeric
 from pyccel.ast.datatypes import CustomDataType
 
 from pyccel.ast.internals import Slice, PrecomputedCode, PyccelArrayShapeElement
 from pyccel.ast.internals import PyccelInternalFunction, get_final_precision
 
+from pyccel.ast.itertoolsext import Product
+
 from pyccel.ast.literals  import LiteralInteger, LiteralFloat, Literal
 from pyccel.ast.literals  import LiteralTrue, LiteralFalse, LiteralString
 from pyccel.ast.literals  import Nil
 
 from pyccel.ast.mathext  import math_constants
 
 from pyccel.ast.numpyext import NumpyEmpty, NumpyInt32
@@ -67,17 +59,23 @@
 from pyccel.ast.numpyext import NumpyReal, NumpyImag
 from pyccel.ast.numpyext import NumpyRand
 from pyccel.ast.numpyext import NumpyNewArray
 from pyccel.ast.numpyext import NumpyNonZero
 from pyccel.ast.numpyext import NumpySign
 from pyccel.ast.numpyext import DtypePrecisionToCastFunction
 
+from pyccel.ast.operators import PyccelAdd, PyccelMul, PyccelMinus
+from pyccel.ast.operators import PyccelMod
+from pyccel.ast.operators import PyccelUnarySub, PyccelLt, PyccelGt, IfTernaryOperator
+
 from pyccel.ast.utilities import builtin_import_registry as pyccel_builtin_import_registry
 from pyccel.ast.utilities import expand_to_loops
 
+from pyccel.ast.variable import Variable, IndexedElement, InhomogeneousTupleVariable, DottedName
+
 from pyccel.errors.errors import Errors
 from pyccel.errors.messages import *
 from pyccel.codegen.printing.codeprinter import CodePrinter
 
 
 # TODO: add examples
 # TODO: use _get_statement when returning a string
@@ -151,30 +149,38 @@
     # 'MathIsinf'   : '???', # TODO
     # --------------------------- internal functions --------------------------
     'MathFactorial' : 'pyc_factorial',
     'MathGcd'       : 'pyc_gcd',
     'MathDegrees'   : 'pyc_degrees',
     'MathRadians'   : 'pyc_radians',
     'MathLcm'       : 'pyc_lcm',
+    # --------------------------- cmath functions --------------------------
+    'CmathAcos'  : 'acos',
+    'CmathAcosh' : 'acosh',
+    'CmathAsin'  : 'asin',
+    'CmathAsinh' : 'asinh',
+    'CmathAtan'  : 'atan',
+    'CmathAtanh' : 'atanh',
+    'CmathCos'   : 'cos',
+    'CmathCosh'  : 'cosh',
+    'CmathExp'   : 'exp',
+    'CmathSin'   : 'sin',
+    'CmathSinh'  : 'sinh',
+    'CmathSqrt'  : 'sqrt',
+    'CmathTan'   : 'tan',
+    'CmathTanh'  : 'tanh',
 }
 
 INF = math_constants['inf']
 
 _default_methods = {
     '__init__': 'create',
     '__del__' : 'free',
 }
 
-python_builtin_datatypes = {
-    'integer' : PythonInt,
-    'float'   : PythonFloat,
-    'bool'    : PythonBool,
-    'complex' : PythonComplex
-}
-
 type_to_print_format = {
         ('float'): 'F0.12',
         ('complex'): '"(",F0.12," + ",F0.12,")"',
         ('int'): 'I0',
         ('bool'): 'A',
         ('string'): 'A',
         ('tuple'):  '*'
@@ -1662,14 +1668,19 @@
 
 #-----------------------------------------------------------------------------
     def _print_Deallocate(self, expr):
         var = expr.variable
         if isinstance(var, InhomogeneousTupleVariable):
             return ''.join(self._print(Deallocate(v)) for v in var)
 
+        if isinstance(var.dtype, CustomDataType):
+            Pyccel__del = expr.variable.cls_base.scope.find('__del__')
+            Pyccel_del_args = [FunctionCallArgument(arg) for arg in Pyccel__del.arguments]
+            return self._print(DottedFunctionCall(Pyccel__del, Pyccel_del_args, var))
+
         if var.is_alias:
             return ''
         else:
             var_code = self._print(var)
             code  = 'if (allocated({})) then\n'.format(var_code)
             code += '  deallocate({})\n'     .format(var_code)
             code += 'end if\n'
@@ -1963,27 +1974,15 @@
         code = ''
         if expr.stmt:
             code += self._print(expr.stmt)
         code +='return\n'
         return code
 
     def _print_Del(self, expr):
-        # TODO: treate class case
-        code = ''
-        for var in expr.variables:
-            if isinstance(var, Variable):
-                dtype = var.dtype
-                if is_pyccel_datatype(dtype):
-                    code = 'call {0} % free()'.format(self._print(var))
-                else:
-                    code = 'deallocate({0}){1}'.format(self._print(var), code)
-            else:
-                errors.report(PYCCEL_RESTRICTION_TODO, symbol=expr,
-                    severity='fatal')
-        return code + '\n'
+        return ''.join(self._print(var) for var in expr.variables)
 
     def _print_ClassDef(self, expr):
         # ... we don't print 'hidden' classes
         if expr.hide:
             return '', ''
         # ...
         self.set_scope(expr.scope)
```

### Comparing `pyccel-1.9.1/pyccel/codegen/printing/luacode.py` & `pyccel-1.9.2/pyccel/codegen/printing/luacode.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/codegen/printing/pycode.py` & `pyccel-1.9.2/pyccel/codegen/printing/pycode.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import warnings
 
 from pyccel.decorators import __all__ as pyccel_decorators
 
 from pyccel.ast.builtins   import PythonMin, PythonMax, PythonType
 from pyccel.ast.core       import CodeBlock, Import, Assign, FunctionCall, For, AsName, FunctionAddress
 from pyccel.ast.core       import IfSection, FunctionDef, Module, DottedFunctionCall, PyccelFunctionDef
-from pyccel.ast.datatypes  import default_precision, datatype
+from pyccel.ast.datatypes  import datatype
 from pyccel.ast.functionalexpr import FunctionalFor
 from pyccel.ast.literals   import LiteralTrue, LiteralString
 from pyccel.ast.literals   import LiteralInteger, LiteralFloat, LiteralComplex
 from pyccel.ast.numpyext   import NumpyShape, NumpySize, numpy_target_swap
 from pyccel.ast.numpyext   import NumpyArray, NumpyNonZero, NumpyResultType
 from pyccel.ast.numpyext   import DtypePrecisionToCastFunction
 from pyccel.ast.variable   import DottedName, HomogeneousTupleVariable, Variable
@@ -211,15 +211,15 @@
         if isinstance(init_dtype, (PythonType, NumpyResultType)):
             dtype = self._print(init_dtype)
         elif isinstance(init_dtype, PyccelFunctionDef):
             dtype = self._get_numpy_name(init_dtype.cls_name)
         else:
             dtype = self._print(expr.dtype)
             if expr.precision != -1:
-                dtype = self._get_numpy_name(DtypePrecisionToCastFunction[datatype(dtype).name][expr.precision])
+                dtype = self._get_numpy_name(DtypePrecisionToCastFunction[expr.dtype.name][expr.precision])
         return f"dtype = {dtype}"
 
     def _print_Header(self, expr):
         return ''
 
     def _print_tuple(self, expr):
         fs = ', '.join(self._print(f) for f in expr)
@@ -243,27 +243,40 @@
     def _print_DottedVariable(self, expr):
         rhs_code = self._print_Variable(expr)
         lhs_code = self._print(expr.lhs)
         return f"{lhs_code}.{rhs_code}"
 
     def _print_FunctionDefArgument(self, expr):
         name = self._print(expr.name)
-        type_annotation = ''
         default = ''
 
         if expr.annotation:
-            type_annotation = f' : {expr.annotation}'
+            type_annotation = self._print(expr.annotation)
+        else:
+            var = expr.var
+            def get_type_annotation(var):
+                if isinstance(var, Variable):
+                    type_annotation = str(var.dtype)
+                    if var.rank:
+                        type_annotation += '[' + ','.join(':' for _ in range(var.rank)) + ']'
+                    return f"'{type_annotation}'"
+                elif isinstance(var, FunctionAddress):
+                    results = ', '.join(get_type_annotation(r.var) for r in var.results)
+                    arguments = ', '.join(get_type_annotation(a.var) for a in var.arguments)
+                    return f'"({results})({arguments})"'
+
+            type_annotation = get_type_annotation(var)
 
         if expr.has_default:
             if isinstance(expr.value, FunctionDef):
                 default = f' = {self._print(expr.value.name)}'
             else:
                 default = f' = {self._print(expr.value)}'
 
-        return f'{name}{type_annotation}{default}'
+        return f'{name} : {type_annotation}{default}'
 
     def _print_FunctionCallArgument(self, expr):
         if expr.keyword:
             return '{} = {}'.format(expr.keyword, self._print(expr.value))
         else:
             return self._print(expr.value)
 
@@ -349,15 +362,15 @@
                 for func in f:
                     if isinstance(func, FunctionCall):
                         args = func.args
                     elif func == n:
                         args = []
                     else:
                         args = [LiteralString(a) for a in func]
-                    if n == 'types' and len(args)==0:
+                    if n == 'types':
                         continue
                     if args:
                         args = ', '.join(self._print(i) for i in args)
                         dec += '@{name}({args})\n'.format(name=n, args=args)
 
                     else:
                         dec += '@{name}\n'.format(name=n)
@@ -480,21 +493,30 @@
 
     def _print_PythonMap(self, expr):
         return 'map({func}, {args})'.format(
                 func = self._print(expr.func.name),
                 args = self._print(expr.func_args))
 
     def _print_PythonReal(self, expr):
-        return '({}).real'.format(self._print(expr.internal_var))
+        if isinstance(expr.internal_var, Variable):
+            return '{}.real'.format(self._print(expr.internal_var))
+        else:
+            return '({}).real'.format(self._print(expr.internal_var))
 
     def _print_PythonImag(self, expr):
-        return '({}).imag'.format(self._print(expr.internal_var))
+        if isinstance(expr.internal_var, Variable):
+            return '{}.imag'.format(self._print(expr.internal_var))
+        else:
+            return '({}).imag'.format(self._print(expr.internal_var))
 
     def _print_PythonConjugate(self, expr):
-        return '({}).conjugate()'.format(self._print(expr.internal_var))
+        if isinstance(expr.internal_var, Variable):
+            return '{}.conjugate()'.format(self._print(expr.internal_var))
+        else:
+            return '({}).conjugate()'.format(self._print(expr.internal_var))
 
     def _print_PythonPrint(self, expr):
         return 'print({})\n'.format(', '.join(self._print(a) for a in expr.expr))
 
     def _print_PyccelArrayShapeElement(self, expr):
         arg = self._print(expr.arg)
         index = self._print(expr.index)
@@ -1066,15 +1088,15 @@
     def _print_ConstructorCall(self, expr):
         cls_name = expr.funcdef.cls_name
         cls_variable = expr.cls_variable
         args = ', '.join(self._print(arg) for arg in expr.args[1:])
         return f"{cls_variable} = {cls_name}({args})\n"
 
     def _print_Del(self, expr):
-        return ''.join(f'del {var}\n' for var in expr.variables)
+        return ''.join(f'del {var.variable}\n' for var in expr.variables)
 
     #------------------OmpAnnotatedComment Printer------------------
 
     def _print_OmpAnnotatedComment(self, expr):
         clauses = ''
         if expr.combined:
             clauses = ' ' + expr.combined
```

### Comparing `pyccel-1.9.1/pyccel/codegen/python_wrapper.py` & `pyccel-1.9.2/pyccel/codegen/python_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/codegen/utilities.py` & `pyccel-1.9.2/pyccel/codegen/utilities.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/codegen/wrapper/c_to_python_wrapper.py` & `pyccel-1.9.2/pyccel/codegen/wrapper/c_to_python_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/codegen/wrapper/fortran_to_c_wrapper.py` & `pyccel-1.9.2/pyccel/codegen/wrapper/fortran_to_c_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/codegen/wrapper/wrapper.py` & `pyccel-1.9.2/pyccel/codegen/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/commands/console.py` & `pyccel-1.9.2/pyccel/commands/console.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/commands/pyccel_clean.py` & `pyccel-1.9.2/pyccel/commands/pyccel_clean.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/commands/pyccel_init.py` & `pyccel-1.9.2/pyccel/commands/pyccel_init.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/compilers/default_compilers.py` & `pyccel-1.9.2/pyccel/compilers/default_compilers.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
                   'flags' : ("-acc"),
                   },
               'family': 'PGI',
               }
 
 #------------------------------------------------------------
 nvfort_info = {'exec' : 'nvfort',
-              'mpi_exec' : 'nvfort',
+              'mpi_exec' : 'mpifort',
               'language': 'fortran',
               'module_output_flag': '-module',
               'debug_flags': ("-Mbounds","-g","-O0"),
               'release_flags': ("-O3","-Munroll",),
               'general_flags' : ('-fPIC',),
               'standard_flags' : ('-Mstandard',),
               'openmp': {
@@ -119,16 +119,16 @@
     gcc_info['mpi_exec'] = 'gcc'
     gcc_info['mpi']['flags']    = ('-D','USE_MPI_MODULE')
     gcc_info['mpi']['libs']     = ('msmpi',)
     gcc_info['mpi']['includes'] = (os.environ["MSMPI_INC"].rstrip('\\'),)
     gcc_info['mpi']['libdirs']  = (os.environ["MSMPI_LIB64"].rstrip('\\'),)
 
 #------------------------------------------------------------
-icc_info = {'exec' : 'icc',
-            'mpi_exec' : 'mpiicc',
+icc_info = {'exec' : 'icx',
+            'mpi_exec' : 'mpicc',
             'language': 'c',
             'debug_flags': ("-g","-O0"),
             'release_flags': ("-O3","-funroll-loops",),
             'general_flags' : ('-fPIC',),
             'standard_flags' : ('-std=c99',),
             'openmp': {
                 'flags' : ('-fopenmp',),
@@ -154,15 +154,15 @@
                 'flags' : ("-acc"),
                 },
             'family': 'PGI',
             }
 
 #------------------------------------------------------------
 nvc_info = {'exec' : 'nvc',
-            'mpi_exec' : 'nvc',
+            'mpi_exec' : 'mpicc',
             'language': 'c',
             'debug_flags': ("-g","-O0"),
             'release_flags': ("-O3","-Munroll",),
             'general_flags' : ('-fPIC',),
             'standard_flags' : ('-std=c99',),
             'openmp': {
                 'flags' : ('-mp',),
```

### Comparing `pyccel-1.9.1/pyccel/complexity/arithmetic.py` & `pyccel-1.9.2/pyccel/complexity/arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/complexity/basic.py` & `pyccel-1.9.2/pyccel/complexity/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/complexity/memory.py` & `pyccel-1.9.2/pyccel/complexity/memory.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/decorators.py` & `pyccel-1.9.2/pyccel/decorators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/epyccel.py` & `pyccel-1.9.2/pyccel/epyccel.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/errors/errors.py` & `pyccel-1.9.2/pyccel/errors/errors.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/errors/messages.py` & `pyccel-1.9.2/pyccel/errors/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,15 +114,14 @@
 # Fortran limitation
 FORTRAN_ALLOCATABLE_IN_EXPRESSION = 'An allocatable function cannot be used in an expression'
 FORTRAN_RANDINT_ALLOCATABLE_IN_EXPRESSION = "Numpy's randint function does not have a fortran equivalent. It can be expressed as '(high-low)*rand(size)+low' using numpy's rand, however allocatable function cannot be used in an expression"
 FORTRAN_ELEMENTAL_SINGLE_ARGUMENT = 'Elemental functions are defined as scalar operators, with a single dummy argument'
 
 # other Pyccel messages
 PYCCEL_INVALID_HEADER = 'Annotated comments must start with omp, acc or header'
-PYCCEL_MISSING_HEADER = 'Cannot find associated header'
 MACRO_MISSING_HEADER_OR_FUNC = 'Cannot find associated header/FunctionDef to macro'
 PYCCEL_UNFOUND_IMPORTED_MODULE = 'Unable to import'
 FOUND_DUPLICATED_IMPORT = 'Duplicated import '
 PYCCEL_UNEXPECTED_IMPORT = 'Pyccel has not correctly handled "import module" statement. Try again with "from module import function" syntax'
 
 IMPORTING_EXISTING_IDENTIFIED = \
         'Trying to import an identifier that already exists in the namespace. Hint: use import as'
```

### Comparing `pyccel-1.9.1/pyccel/naming/__init__.py` & `pyccel-1.9.2/pyccel/naming/__init__.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/naming/cnameclashchecker.py` & `pyccel-1.9.2/pyccel/naming/cnameclashchecker.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/naming/fortrannameclashchecker.py` & `pyccel-1.9.2/pyccel/naming/fortrannameclashchecker.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/naming/languagenameclashchecker.py` & `pyccel-1.9.2/pyccel/naming/languagenameclashchecker.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/naming/pythonnameclashchecker.py` & `pyccel-1.9.2/pyccel/naming/pythonnameclashchecker.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/parser/base.py` & `pyccel-1.9.2/pyccel/parser/base.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/parser/extend_tree.py` & `pyccel-1.9.2/pyccel/parser/extend_tree.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/parser/grammar/headers.tx` & `pyccel-1.9.2/pyccel/parser/grammar/headers.tx`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 ;
 
 HeaderStmt: '#$' 'header' stmt=Statement;
 
 Statement:
     FunctionMacroStmt 
   | VariableHeaderStmt
-  | FunctionHeaderStmt 
-  | ClassHeaderStmt
+  | FunctionHeaderStmt
   | MetavarHeaderStmt
   | TemplateStmt
   | InterfaceStmt
 ;
 
 TrailerSubscriptList: '[' args*=':' [','] ']'  ( '(' 'order' '=' order = ID ')' )?;
 
@@ -35,27 +34,14 @@
 
 TemplateStmt: 'template' name = ID '(' dtypes+=TypeHeader['|'] ')';
 
 FunctionKind: 'function' | 'method';
 Static: 'static';
 HeaderResults: 'results' '(' decs+=TypeHeader[','] ')'; 
 
-ClassHeaderStmt: 'class'  name=ID '(' options+=ClassOptions[','] ')';
-
-ClassOptions: 
-    'abstract' 
-  | 'private' 
-  | 'public' 
-  | 'iterable' 
-  | 'with' 
-  | 'hide' 
-  | 'openmp'
-  | 'openacc'
-;
-
 MetavarHeaderStmt: 'metavar'  name=ID '=' value=MetavarValues;
 MetavarValues: BOOL|STRING;
 
 InterfaceStmt: 'interface' name=ID '=' args+=ID['|'];
 
 // **** macros ****
```

### Comparing `pyccel-1.9.1/pyccel/parser/grammar/openacc.tx` & `pyccel-1.9.2/pyccel/parser/grammar/openacc.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/parser/grammar/openmp.tx` & `pyccel-1.9.2/pyccel/parser/grammar/openmp.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/parser/grammar/pyccel.tx` & `pyccel-1.9.2/pyccel/parser/grammar/pyccel.tx`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/parser/parser.py` & `pyccel-1.9.2/pyccel/parser/parser.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/parser/scope.py` & `pyccel-1.9.2/pyccel/parser/scope.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 """ Module containing the Scope class
 """
 
 from pyccel.ast.core      import ClassDef
-from pyccel.ast.datatypes import DataTypeFactory
 from pyccel.ast.headers   import MacroFunction, MacroVariable
-from pyccel.ast.headers   import FunctionHeader, ClassHeader, MethodHeader
+from pyccel.ast.headers   import FunctionHeader, MethodHeader
 from pyccel.ast.internals import PyccelSymbol
 from pyccel.ast.variable  import Variable, DottedName
 
 from pyccel.errors.errors import Errors
 
 from pyccel.naming.pythonnameclashchecker import PythonNameClashChecker
 
@@ -194,36 +193,50 @@
 
     @property
     def symbolic_functions(self):
         """ A dictionary of symbolic functions defined in this scope
         """
         return self._locals['symbolic_functions']
 
-    def find(self, name, category = None):
-        """ Find and return the specified object in the scope.
-        If the object cannot be found then None is returned
+    def find(self, name, category = None, local_only = False):
+        """
+        Find and return the specified object in the scope.
+
+        Find a specified object in the scope and return it.
+        The object is identified by a string contianing its name.
+        If the object cannot be found then None is returned.
 
         Parameters
         ----------
         name : str
-            The name of the object we are searching for
-        category : str
+            The name of the object we are searching for.
+        category : str, optional
             The type of object we are searching for.
-            This must be one of the strings in Scope.categories
+            This must be one of the strings in Scope.categories.
+            If no value is provided then we look in all categories.
+        local_only : bool, default=False
+            Indicates whether we should look for variables in the
+            entire scope or whether we should limit ourselves to the
+            local scope.
+
+        Returns
+        -------
+        pyccel.ast.basic.Basic
+            The object stored in the scope.
         """
         for l in ([category] if category else self._locals.keys()):
             if name in self._locals[l]:
                 return self._locals[l][name]
 
             if name in self.imports[l]:
                 return self.imports[l][name]
 
         # Walk up the tree of Scope objects, until the root if needed
-        if self.parent_scope:
-            return self.parent_scope.find(name, category)
+        if self.parent_scope and (self.is_loop or not local_only):
+            return self.parent_scope.find(name, category, local_only)
         else:
             return None
 
     def find_all(self, category):
         """ Find and return all objects from the specified category
         in the scope.
 
@@ -409,21 +422,14 @@
             Raised if the header type is unknown.
         """
         if isinstance(expr, (FunctionHeader, MethodHeader)):
             if expr.name in self.headers:
                 self.headers[expr.name].append(expr)
             else:
                 self.headers[expr.name] = [expr]
-        elif isinstance(expr, ClassHeader):
-            self.headers[expr.name] = expr
-
-            #  create a new Datatype for the current class
-
-            dtype = DataTypeFactory(expr.name, '_name')
-            self.cls_constructs[expr.name] = dtype
         else:
             msg = 'header of type{0} is not supported'
             msg = msg.format(str(type(expr)))
             raise TypeError(msg)
 
     def insert_symbol(self, symbol):
         """ Add a new symbol to the scope
```

### Comparing `pyccel-1.9.1/pyccel/parser/semantic.py` & `pyccel-1.9.2/pyccel/parser/semantic.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 
 #==============================================================================
 
 from pyccel.ast.basic import Basic, PyccelAstNode, ScopedNode
 
 from pyccel.ast.builtins import PythonPrint
 from pyccel.ast.builtins import PythonInt, PythonBool, PythonFloat, PythonComplex
-from pyccel.ast.builtins import python_builtin_datatype
+from pyccel.ast.builtins import python_builtin_datatype, PythonImag, PythonReal
 from pyccel.ast.builtins import PythonList, PythonConjugate
 from pyccel.ast.builtins import (PythonRange, PythonZip, PythonEnumerate,
-                                 PythonTuple, Lambda)
+                                 PythonTuple, Lambda, PythonMap)
 
 from pyccel.ast.core import Comment, CommentBlock, Pass
 from pyccel.ast.core import If, IfSection
 from pyccel.ast.core import Allocate, Deallocate
 from pyccel.ast.core import Assign, AliasAssign, SymbolicAssign
 from pyccel.ast.core import AugAssign, CodeBlock
 from pyccel.ast.core import Return, FunctionDefArgument, FunctionDefResult
@@ -57,16 +57,16 @@
 from pyccel.ast.core import Decorator
 from pyccel.ast.core import PyccelFunctionDef
 from pyccel.ast.core import Assert
 
 from pyccel.ast.class_defs import NumpyArrayClass, TupleClass, get_cls_base
 
 from pyccel.ast.datatypes import NativeRange, str_dtype
-from pyccel.ast.datatypes import NativeSymbol
-from pyccel.ast.datatypes import default_precision
+from pyccel.ast.datatypes import NativeSymbol, DataTypeFactory, CustomDataType
+from pyccel.ast.datatypes import default_precision, dtype_and_precision_registry
 from pyccel.ast.datatypes import (NativeInteger, NativeBool,
                                   NativeFloat, NativeString,
                                   NativeGeneric, NativeComplex,
                                   NativeVoid)
 
 from pyccel.ast.functionalexpr import FunctionalSum, FunctionalMax, FunctionalMin, GeneratorComprehension, FunctionalFor
 
@@ -74,18 +74,18 @@
 from pyccel.ast.headers import MacroFunction, MacroVariable
 
 from pyccel.ast.internals import PyccelInternalFunction, Slice, PyccelSymbol, get_final_precision
 from pyccel.ast.itertoolsext import Product
 
 from pyccel.ast.literals import LiteralTrue, LiteralFalse
 from pyccel.ast.literals import LiteralInteger, LiteralFloat
-from pyccel.ast.literals import Nil, LiteralString
+from pyccel.ast.literals import Nil, LiteralString, LiteralImaginaryUnit
 from pyccel.ast.literals import Literal, convert_to_literal
 
-from pyccel.ast.mathext  import math_constants
+from pyccel.ast.mathext  import math_constants, MathSqrt, MathAtan2, MathSin, MathCos
 
 from pyccel.ast.numpyext import NumpyMatmul
 from pyccel.ast.numpyext import NumpyBool
 from pyccel.ast.numpyext import NumpyWhere, NumpyArray
 from pyccel.ast.numpyext import NumpyInt, NumpyInt8, NumpyInt16, NumpyInt32, NumpyInt64
 from pyccel.ast.numpyext import NumpyFloat, NumpyFloat32, NumpyFloat64
 from pyccel.ast.numpyext import NumpyComplex, NumpyComplex64, NumpyComplex128
@@ -99,14 +99,16 @@
 
 from pyccel.ast.operators import PyccelArithmeticOperator, PyccelIs, PyccelIsNot, IfTernaryOperator, PyccelUnarySub
 from pyccel.ast.operators import PyccelNot, PyccelEq, PyccelAdd, PyccelMul, PyccelPow
 from pyccel.ast.operators import PyccelAssociativeParenthesis, PyccelDiv
 
 from pyccel.ast.sympy_helper import sympy_to_pyccel, pyccel_to_sympy
 
+from pyccel.ast.type_annotations import VariableTypeAnnotation, UnionTypeAnnotation
+
 from pyccel.ast.utilities import builtin_function as pyccel_builtin_function
 from pyccel.ast.utilities import builtin_import as pyccel_builtin_import
 from pyccel.ast.utilities import builtin_import_registry as pyccel_builtin_import_registry
 from pyccel.ast.utilities import split_positional_keyword_arguments
 from pyccel.ast.utilities import recognised_source
 
 from pyccel.ast.variable import Constant
@@ -127,15 +129,15 @@
         INVALID_POINTER_REASSIGN, INCOMPATIBLE_REDEFINITION, ARRAY_IS_ARG,
         INCOMPATIBLE_REDEFINITION_STACK_ARRAY, ARRAY_REALLOCATION, RECURSIVE_RESULTS_REQUIRED,
         PYCCEL_RESTRICTION_INHOMOG_LIST, UNDEFINED_IMPORT_OBJECT, UNDEFINED_LAMBDA_VARIABLE,
         UNDEFINED_LAMBDA_FUNCTION, UNDEFINED_INIT_METHOD, UNDEFINED_FUNCTION,
         INVALID_MACRO_COMPOSITION, WRONG_NUMBER_OUTPUT_ARGS, INVALID_FOR_ITERABLE,
         PYCCEL_RESTRICTION_LIST_COMPREHENSION_LIMITS, PYCCEL_RESTRICTION_LIST_COMPREHENSION_SIZE,
         UNUSED_DECORATORS, DUPLICATED_SIGNATURE, FUNCTION_TYPE_EXPECTED,
-        UNSUPPORTED_POINTER_RETURN_VALUE, PYCCEL_MISSING_HEADER, PYCCEL_RESTRICTION_OPTIONAL_NONE,
+        UNSUPPORTED_POINTER_RETURN_VALUE, PYCCEL_RESTRICTION_OPTIONAL_NONE,
         PYCCEL_RESTRICTION_PRIMITIVE_IMMUTABLE, PYCCEL_RESTRICTION_IS_ISNOT,
         FOUND_DUPLICATED_IMPORT, UNDEFINED_WITH_ACCESS, MACRO_MISSING_HEADER_OR_FUNC,)
 
 from pyccel.parser.base      import BasicParser
 from pyccel.parser.syntactic import SyntaxParser
 
 from pyccel.utilities.stage import PyccelStage
@@ -340,26 +342,42 @@
         current namespace is the program namespace.
         """
         self._program_namespace = self.scope
         self.scope = self._module_namespace
 
     def check_for_variable(self, name):
         """
+        Search for a Variable object with the given name in the current scope.
+
         Search for a Variable object with the given name in the current scope,
         defined by the local and global Python scopes. Return None if not found.
+
+        Parameters
+        ----------
+        name : str
+            The object describing the variable.
+
+        Returns
+        -------
+        Variable
+            Returns the variable if found or None.
         """
 
-        if self.current_class:
-            for i in self._current_class.attributes:
-                if i.name == name:
-                    var = i
-                    return var
-            return None
-        else:
-            return self.scope.find(name, 'variables')
+        if isinstance(name, DottedName):
+            prefix_parts = name.name[:-1]
+            syntactic_prefix = prefix_parts[0] if len(prefix_parts) == 1 else DottedName(*prefix_parts)
+            prefix = self._visit(syntactic_prefix)
+            class_def = self.scope.find(prefix.dtype.name, 'classes')
+            attr_name = name.name[-1]
+            attribute = class_def.scope.find(attr_name, 'variables') if class_def else None
+            if attribute:
+                return attribute.clone(attribute.name, new_class = DottedVariable, lhs = prefix)
+            else:
+                return None
+        return self.scope.find(name, 'variables')
 
     def get_variable(self, name):
         """ Like 'check_for_variable', but raise Pyccel error if Variable is not found.
         """
         var = self.check_for_variable(name)
         if var is None:
             if name == '_':
@@ -466,19 +484,37 @@
     #=======================================================
     #              Utility functions
     #=======================================================
 
     def _garbage_collector(self, expr):
         """
         Search in a CodeBlock if no trailing Return Node is present add the needed frees.
+
+        The primary purpose of _garbage_collector is to search within a CodeBlock
+        instance for cases where no trailing Return node is present, and when such
+        situations occur, it adds the necessary deallocate operations to free up resources.
+
+        Parameters
+        ----------
+        expr : CodeBlock
+            The body where the method searches for the absence of trailing `Return` nodes.
+
+        Returns
+        -------
+        List
+            A list of instances of the `Deallocate` type.
         """
+
+        deallocs = []
         if len(expr.body)>0 and not isinstance(expr.body[-1], Return):
-            deallocs = [Deallocate(i) for i in self._allocs[-1]]
-        else:
-            deallocs = []
+            for i in self._allocs[-1]:
+                if isinstance(i, DottedVariable):
+                    if isinstance(i.lhs.dtype, CustomDataType) and self._current_function != '__del__':
+                        continue
+                deallocs.append(Deallocate(i))
         self._allocs.pop()
         return deallocs
 
     def _infer_type(self, expr):
         """
         Infer all relevant type information for the expression.
 
@@ -523,15 +559,15 @@
             return d_var
 
         elif isinstance(expr, Variable):
             d_var['datatype'       ] = expr.dtype
             d_var['memory_handling'] = expr.memory_handling
             d_var['shape'          ] = expr.shape
             d_var['rank'           ] = expr.rank
-            d_var['cls_base'       ] = expr.cls_base or self.scope.find(expr.dtype, 'classes')
+            d_var['cls_base'       ] = expr.cls_base or self.scope.find(expr.dtype.name, 'classes')
             d_var['is_target'      ] = expr.is_target
             d_var['order'          ] = expr.order
             d_var['precision'      ] = expr.precision
             return d_var
 
         elif isinstance(expr, PythonTuple):
             d_var['datatype'       ] = expr.dtype
@@ -1100,31 +1136,57 @@
         -------
         pyccel.ast.variable.Variable
             The representation of the lhs provided by the SemanticParser.
         """
 
         if isinstance(lhs, IndexedElement):
             lhs = self._visit(lhs)
-        elif isinstance(lhs, PyccelSymbol):
+        elif isinstance(lhs, (PyccelSymbol, DottedName)):
 
-            name = lhs
+            name = str(lhs)
             if lhs == '_':
                 name = self.scope.get_new_name()
             dtype = d_var.pop('datatype')
 
             d_lhs = d_var.copy()
             # ISSUES #177: lhs must be a pointer when rhs is heap array
             if not arr_in_multirets:
                 self._ensure_target(rhs, d_lhs)
 
-            var = self.check_for_variable(name)
+            var = self.check_for_variable(lhs)
 
             # Variable not yet declared (hence array not yet allocated)
             if var is None:
 
+                if isinstance(lhs, DottedName):
+                    prefix_parts = lhs.name[:-1]
+                    syntactic_prefix = prefix_parts[0] if len(prefix_parts) == 1 else DottedName(*prefix_parts)
+                    prefix = self._visit(syntactic_prefix)
+                    class_def = prefix.cls_base
+                    if prefix.name == 'self':
+                        var = self.get_variable('self')
+
+                        # Collect the name that should be used in the generated code
+                        attribute_name = lhs.name[-1]
+                        new_name = class_def.scope.get_expected_name(attribute_name)
+                        # Create the attribute
+                        member = self._create_variable(new_name, dtype, rhs, d_lhs)
+
+                        # Insert the attribute to the class scope
+                        # Passing the original name ensures that the attribute can be found under this name
+                        class_def.scope.insert_variable(member, attribute_name)
+
+                        # Create the local DottedVariable
+                        lhs = member.clone(member.name, new_class = DottedVariable, lhs = var)
+
+                        # update the attributes of the class and push it to the scope
+                        class_def.add_new_attribute(lhs)
+
+                    else:
+                        errors.report(f"{lhs.name[0]} should be named : self", symbol=lhs, severity='fatal')
                 # Update variable's dictionary with information from function decorators
                 decorators = self.scope.decorators
                 if decorators:
                     if 'stack_array' in decorators:
                         if name in decorators['stack_array']:
                             d_lhs.update(memory_handling='stack')
                     if 'allow_negative_index' in decorators:
@@ -1144,21 +1206,21 @@
                         if (isinstance(a, Variable) and not a.is_argument) \
                                 or not all(b.is_argument for b in a.get_attribute_nodes(Variable)):
                             errors.report(STACK_ARRAY_UNKNOWN_SHAPE, symbol=name,
                             severity='error',
                             bounding_box=(self._current_fst_node.lineno,
                                 self._current_fst_node.col_offset))
 
-                new_name = self.scope.get_expected_name(name)
+                if not isinstance(lhs, DottedVariable):
+                    new_name = self.scope.get_expected_name(name)
+                    # Create new variable
+                    lhs = self._create_variable(new_name, dtype, rhs, d_lhs, arr_in_multirets=arr_in_multirets)
 
-                # Create new variable
-                lhs = self._create_variable(new_name, dtype, rhs, d_lhs, arr_in_multirets=arr_in_multirets)
-
-                # Add variable to scope
-                self.scope.insert_variable(lhs, name)
+                    # Add variable to scope
+                    self.scope.insert_variable(lhs, name)
 
                 # ...
                 # Add memory allocation if needed
                 array_declared_in_function = (isinstance(rhs, FunctionCall) and not isinstance(rhs.funcdef, PyccelFunctionDef) \
                                             and not getattr(rhs.funcdef, 'is_elemental', False) and not isinstance(lhs, HomogeneousTupleVariable)) or arr_in_multirets
                 if lhs.on_heap and not array_declared_in_function:
                     if self.scope.is_loop:
@@ -1220,82 +1282,52 @@
                 self._ensure_inferred_type_matches_existing(dtype, d_var, var, is_augassign, new_expressions, rhs)
 
                 # in the case of elemental, lhs is not of the same dtype as
                 # var.
                 # TODO d_lhs must be consistent with var!
                 # the following is a small fix, since lhs must be already
                 # declared
-                lhs = var
-
-        elif isinstance(lhs, DottedName):
-
-            dtype = d_var.pop('datatype')
-            name = self.scope.get_expected_name(lhs.name[-1])
-            if self._current_function == '__init__':
-
-                cls      = self.get_variable('self')
-                cls_name = str(cls.cls_base.name)
-                cls      = self.scope.find(cls_name, 'classes')
-
-                attributes = cls.attributes
-                parent     = cls.superclasses
-                attributes = list(attributes)
-                n_name     = str(lhs.name[-1])
-
-                # update the self variable with the new attributes
-
-                var      = self.get_variable('self')
-                d_lhs    = d_var.copy()
-
-
-                # ISSUES #177: lhs must be a pointer when rhs is heap array
-                if not arr_in_multirets:
-                    self._ensure_target(rhs, d_lhs)
-
-                member = self._create_variable(n_name, dtype, rhs, d_lhs)
-                lhs    = member.clone(member.name, new_class = DottedVariable, lhs = var)
-
-                # update the attributes of the class and push it to the scope
-                attributes += [member]
-                new_cls = ClassDef(cls_name, attributes, [], superclasses=parent)
-                self.scope.parent_scope.update_class(new_cls)
-            else:
-                lhs = self._visit(lhs)
+                if isinstance(lhs, DottedName):
+                    lhs = var.clone(var.name, new_class = DottedVariable, lhs = self._visit(lhs.name[0]))
+                else:
+                    lhs = var
         else:
             lhs_type = str(type(lhs))
             raise NotImplementedError(f"_assign_lhs_variable does not handle {lhs_type}")
 
         return lhs
 
     def _ensure_inferred_type_matches_existing(self, dtype, d_var, var, is_augassign, new_expressions, rhs):
         """
+        Ensure that the inferred type matches the existing variable.
+
         Ensure that the inferred type of the new variable, matches the existing variable (which has the
         same name). If this is not the case then errors are raised preventing pyccel reaching the codegen
         stage.
         This function also handles any reallocations caused by differing shapes between the two objects.
         These allocations/deallocations are saved in the list new_expressions
 
         Parameters
         ----------
         dtype : DataType
-                The inferred DataType
+            The inferred DataType.
         d_var : dict
-                The inferred information about the variable. Usually created by the _infer_type function
-        var   : Variable
-                The existing variable
+            The inferred information about the variable. Usually created by the _infer_type function.
+        var : Variable
+            The existing variable.
         is_augassign : bool
-                A boolean indicating if the assign statement is an augassign (tests are less strict)
+            A boolean indicating if the assign statement is an augassign (tests are less strict).
         new_expressions : list
-                A list to which any new expressions created are appended
-        rhs   : PyccelAstNode
-                The right hand side of the expression : lhs=rhs
-                If is_augassign is False, this value is not used
+            A list to which any new expressions created are appended.
+        rhs : PyccelAstNode
+            The right hand side of the expression : lhs=rhs.
+            If is_augassign is False, this value is not used.
         """
         precision = d_var.get('precision',None)
-        internal_precision = default_precision[str(dtype)] if precision == -1 else precision
+        internal_precision = default_precision[dtype] if precision == -1 else precision
 
         # TODO improve check type compatibility
         if not hasattr(var, 'dtype'):
             name = var.name
             errors.report(INCOMPATIBLE_TYPES_IN_ASSIGNMENT.format('<module>', dtype),
                     symbol=f'{name}={dtype}',
                     bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
@@ -1356,14 +1388,20 @@
 
         elif not is_augassign:
 
             rank  = getattr(var, 'rank' , 'None')
             order = getattr(var, 'order', 'None')
             shape = getattr(var, 'shape', 'None')
 
+            # Get previous allocation calls
+            previous_allocations = var.get_direct_user_nodes(lambda p: isinstance(p, Allocate))
+
+            if len(previous_allocations) == 0:
+                var.set_init_shape(d_var['shape'])
+
             if (d_var['rank'] != rank) or (rank > 1 and d_var['order'] != order):
 
                 txt = '|{name}| {dtype}{old} <-> {dtype}{new}'
                 def format_shape(s):
                     return "" if s is None else s
                 txt = txt.format(name=var.name, dtype=dtype, old=format_shape(var.shape),
                     new=format_shape(d_var['shape']))
@@ -1376,66 +1414,62 @@
                 if var.is_argument:
                     errors.report(ARRAY_IS_ARG, symbol=var,
                         severity='error',
                         bounding_box=(self._current_fst_node.lineno,
                             self._current_fst_node.col_offset))
 
                 elif var.is_stack_array:
-                    errors.report(INCOMPATIBLE_REDEFINITION_STACK_ARRAY, symbol=var.name,
-                        severity='error',
-                        bounding_box=(self._current_fst_node.lineno,
-                            self._current_fst_node.col_offset))
+                    if var.get_direct_user_nodes(lambda a: isinstance(a, Assign) and a.lhs is var):
+                        errors.report(INCOMPATIBLE_REDEFINITION_STACK_ARRAY, symbol=var.name,
+                            severity='error',
+                            bounding_box=(self._current_fst_node.lineno,
+                                self._current_fst_node.col_offset))
 
                 else:
-                    var.set_changeable_shape()
-                    previous_allocations = var.get_direct_user_nodes(lambda p: isinstance(p, Allocate))
-                    if not previous_allocations:
-                        errors.report("PYCCEL INTERNAL ERROR : Variable exists already, but it has never been allocated",
-                                symbol=var, severity='fatal')
-
-                    last_allocation = previous_allocations[-1]
-
-                    # Find outermost IfSection of last allocation
-                    last_alloc_ifsection = last_allocation.get_user_nodes(IfSection)
-                    alloc_ifsection = last_alloc_ifsection[-1] if last_alloc_ifsection else None
-                    while len(last_alloc_ifsection)>0:
-                        alloc_ifsection = last_alloc_ifsection[-1]
-                        last_alloc_ifsection = alloc_ifsection.get_user_nodes(IfSection)
-
-                    ifsection_has_if = len(alloc_ifsection.get_direct_user_nodes(
-                                                        lambda x: isinstance(x,If))) == 1 \
-                                    if alloc_ifsection else False
-
-                    if alloc_ifsection and not ifsection_has_if:
-                        status = last_allocation.status
-                    elif last_allocation.get_user_nodes((If, For, While)):
-                        status='unknown'
+                    if previous_allocations:
+                        var.set_changeable_shape()
+                        last_allocation = previous_allocations[-1]
+
+                        # Find outermost IfSection of last allocation
+                        last_alloc_ifsection = last_allocation.get_user_nodes(IfSection)
+                        alloc_ifsection = last_alloc_ifsection[-1] if last_alloc_ifsection else None
+                        while len(last_alloc_ifsection)>0:
+                            alloc_ifsection = last_alloc_ifsection[-1]
+                            last_alloc_ifsection = alloc_ifsection.get_user_nodes(IfSection)
+
+                        ifsection_has_if = len(alloc_ifsection.get_direct_user_nodes(
+                                                            lambda x: isinstance(x,If))) == 1 \
+                                        if alloc_ifsection else False
+
+                        if alloc_ifsection and not ifsection_has_if:
+                            status = last_allocation.status
+                        elif last_allocation.get_user_nodes((If, For, While)):
+                            status='unknown'
+                        else:
+                            status='allocated'
                     else:
-                        status='allocated'
+                        status = 'unallocated'
+
                     new_expressions.append(Allocate(var,
                         shape=d_var['shape'], order=d_var['order'],
                         status=status))
 
                     if status != 'unallocated':
                         errors.report(ARRAY_REALLOCATION, symbol=var.name,
                             severity='warning',
                             bounding_box=(self._current_fst_node.lineno,
                                 self._current_fst_node.col_offset))
-            else:
-                # Same shape as before
-                previous_allocations = var.get_direct_user_nodes(lambda p: isinstance(p, Allocate))
-
-                if previous_allocations and previous_allocations[-1].get_user_nodes(IfSection) \
+            elif previous_allocations and previous_allocations[-1].get_user_nodes(IfSection) \
                         and not previous_allocations[-1].get_user_nodes((If)):
-                    # If previously allocated in If still under construction
-                    status = previous_allocations[-1].status
+                # If previously allocated in If still under construction
+                status = previous_allocations[-1].status
 
-                    new_expressions.append(Allocate(var,
-                        shape=d_var['shape'], order=d_var['order'],
-                        status=status))
+                new_expressions.append(Allocate(var,
+                    shape=d_var['shape'], order=d_var['order'],
+                    status=status))
 
         if var.precision == -1 and precision != var.precision:
             var.use_exact_precision()
 
     def _assign_GeneratorComprehension(self, lhs_name, expr):
         """
         Visit the GeneratorComprehension node.
@@ -1848,14 +1882,21 @@
 
             # Save parsed code
             line = self._visit(b)
             ls.extend(self._additional_exprs[-1])
             self._additional_exprs[-1] = []
             if isinstance(line, CodeBlock):
                 ls.extend(line.body)
+            # ----- If block to handle VariableHeader. To be removed when headers are deprecated. ---
+            elif isinstance(line, list) and isinstance(line[0], Variable):
+                self.scope.insert_variable(line[0])
+                if len(line) != 1:
+                    errors.report(f"Variable {line[0]} cannot have multiple types",
+                            severity='error', symbol=line[0])
+            # ---------------------------- End of if block ------------------------------------------
             else:
                 ls.append(line)
         self._additional_exprs.pop()
 
         return CodeBlock(ls)
 
     def _visit_Nil(self, expr):
@@ -1998,14 +2039,96 @@
                     severity='fatal')
             else:
                 errors.report(UNDEFINED_VARIABLE, symbol=name,
                     bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                     severity='fatal')
         return var
 
+    def _visit_AnnotatedPyccelSymbol(self, expr):
+        # Check if the variable already exists
+        var = self.scope.find(expr, 'variables', local_only = True)
+        if var is not None:
+            errors.report("Variable has been declared multiple times",
+                    symbol=expr, severity='error')
+
+        # Get the semantic type annotation (should be UnionTypeAnnotation)
+        types = self._visit(expr.annotation)
+
+        # Get the collisionless name from the scope
+        name = self.scope.get_expected_name(expr.name)
+
+        # Use the local decorators to define the memory and index handling
+        allows_negative_indexes = False
+        array_memory_handling = 'heap'
+        decorators = self.scope.decorators
+        if decorators:
+            if 'stack_array' in decorators:
+                if expr.name in decorators['stack_array']:
+                    array_memory_handling = 'stack'
+            if 'allow_negative_index' in decorators:
+                if expr.name in decorators['allow_negative_index']:
+                    allows_negative_indexes = True
+
+        # For each possible data type create the necessary variables
+        possible_args = []
+        for t in types.type_list:
+            if isinstance(t, VariableTypeAnnotation):
+                dtype = t.datatype
+                prec  = t.precision
+                rank  = t.rank
+                v = Variable(dtype, name, precision = prec,
+                        shape = None, rank = rank, order = t.order, cls_base = t.cls_base,
+                        is_const = t.is_const, is_optional = False,
+                        memory_handling = array_memory_handling if rank > 0 else 'stack',
+                        allows_negative_indexes = allows_negative_indexes)
+                possible_args.append(v)
+            else:
+                errors.report(PYCCEL_RESTRICTION_TODO + '\nUnrecoginsed type annotation',
+                        severity='fatal', symbol=expr)
+
+        # An annotated variable must have a type
+        assert len(possible_args) != 0
+
+        return possible_args
+
+    def _visit_SyntacticTypeAnnotation(self, expr):
+        is_const = expr.is_const is True
+        types = []
+
+        for dtype_name, rank, order in zip(expr.dtypes, expr.ranks, expr.orders):
+            # Find the DataType instance and the associated precision
+            prec = -1
+            try:
+                dtype, prec = dtype_and_precision_registry[dtype_name]
+            except KeyError:
+                errors.report(f'Could not identify type : {dtype_name}',
+                        severity='fatal', symbol=expr)
+
+            try:
+                cls_base = get_cls_base(dtype, prec, rank)
+            except KeyError:
+                cls_base = self.scope.find(dtype_name, 'classes')
+
+            if rank > 1 and order is None:
+                order = 'C'
+            elif order is not None and rank < 2:
+                errors.report(f"Ordering is not applicable to objects with rank {rank}",
+                        symbol=expr.fst, severity='warning')
+                order = None
+
+            # NumPy objects cannot have default precision
+            if prec == -1 and cls_base is NumpyArrayClass:
+                prec = default_precision[dtype]
+
+            # Save the potential type
+            types.append(VariableTypeAnnotation(dtype, cls_base, prec, rank, order, is_const))
+
+        # Collect all possible types into a UnionTypeAnnotation
+        return UnionTypeAnnotation(*types)
+
 
     def _visit_DottedName(self, expr):
 
         var = self.check_for_variable(_get_name(expr))
         if var:
             return var
 
@@ -2020,15 +2143,14 @@
             if len(results) != 1:
                 errors.report("Cannot get attribute of function call with multiple returns",
                         symbol=expr,
                         bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                         severity='fatal')
             first = results[0].var
         rhs_name = _get_name(rhs)
-        attr_name = []
 
         # Handle case of imported module
         if isinstance(first, Module):
 
             if rhs_name in first:
                 imp = self.scope.find(_get_name(lhs), 'imports')
 
@@ -2077,17 +2199,14 @@
         if d_var.get('cls_base', None) is None:
             errors.report(f'Attribute {rhs_name} not found',
                 bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                 severity='fatal')
 
         cls_base = d_var['cls_base']
 
-        if cls_base:
-            attr_name = [i.name for i in cls_base.attributes]
-
         # look for a class method
         if isinstance(rhs, FunctionCall):
             macro = self.scope.find(rhs_name, 'macros')
             if macro is not None:
                 master = macro.master
                 args = rhs.args
                 args = [lhs] + list(args)
@@ -2101,19 +2220,17 @@
                 numpy_class = method.cls_name
                 self.insert_import('numpy', AsName(numpy_class, numpy_class.name))
             return self._handle_function(expr, method, args, is_method = True)
 
         # look for a class attribute / property
         elif isinstance(rhs, PyccelSymbol) and cls_base:
             # standard class attribute
-            if rhs in attr_name:
-                self._current_class = cls_base
-                second = self._visit(rhs)
-                self._current_class = None
-                return second.clone(second.name, new_class = DottedVariable, lhs = visited_lhs)
+            second = self.check_for_variable(expr)
+            if second:
+                return second
 
             # class property?
             else:
                 method = cls_base.get_method(rhs_name)
                 assert 'property' in method.decorators
                 if cls_base.name == 'numpy.ndarray':
                     numpy_class = method.cls_name
@@ -2264,14 +2381,48 @@
 
                 pyccel_stage.set_stage('semantic')
 
                 return self._visit(new_call)
 
         return self._handle_function(expr, func, (arg,))
 
+    def _visit_CmathPolar(self, expr):
+        arg, = self._handle_function_args(expr.args) #pylint: disable=unbalanced-tuple-unpacking
+        z = arg.value
+        x = PythonReal(z)
+        y = PythonImag(z)
+        x_var = self.scope.get_temporary_variable(z, dtype=NativeFloat())
+        y_var = self.scope.get_temporary_variable(z, dtype=NativeFloat())
+        self._additional_exprs[-1].append(Assign(x_var, x))
+        self._additional_exprs[-1].append(Assign(y_var, y))
+        r = MathSqrt(PyccelAdd(PyccelMul(x_var,x_var), PyccelMul(y_var,y_var)))
+        t = MathAtan2(y_var, x_var)
+        self.insert_import('math', AsName(MathSqrt, 'sqrt'))
+        self.insert_import('math', AsName(MathAtan2, 'atan2'))
+        return PythonTuple(r,t)
+
+    def _visit_CmathRect(self, expr):
+        arg_r, arg_phi = self._handle_function_args(expr.args) #pylint: disable=unbalanced-tuple-unpacking
+        r = arg_r.value
+        phi = arg_phi.value
+        x = PyccelMul(r, MathCos(phi))
+        y = PyccelMul(r, MathSin(phi))
+        self.insert_import('math', AsName(MathCos, 'cos'))
+        self.insert_import('math', AsName(MathSin, 'sin'))
+        return PyccelAdd(x, PyccelMul(y, LiteralImaginaryUnit()))
+
+    def _visit_CmathPhase(self, expr):
+        arg, = self._handle_function_args(expr.args) #pylint: disable=unbalanced-tuple-unpacking
+        var = arg.value
+        if var.dtype is not NativeComplex():
+            return LiteralFloat(0.0)
+        else:
+            self.insert_import('math', AsName(MathAtan2, 'atan2'))
+            return MathAtan2(PythonImag(var), PythonReal(var))
+
     def _visit_Lambda(self, expr):
         expr_names = set(str(a) for a in expr.expr.get_attribute_nodes(PyccelSymbol))
         var_names = map(str, expr.variables)
         missing_vars = expr_names.difference(var_names)
         if len(missing_vars) > 0:
             errors.report(UNDEFINED_LAMBDA_VARIABLE, symbol = missing_vars,
                 bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
@@ -2347,14 +2498,15 @@
                     'cls_base' : self.scope.find(method.cls_name, 'classes')}
             cls_variable = self._assign_lhs_variable(expr.current_user_node.lhs, d_var, expr, [], True)
             args = (FunctionCallArgument(cls_variable), *args)
             # TODO check compatibility
             # TODO treat parametrized arguments.
 
             expr = ConstructorCall(method, args, cls_variable)
+            self._allocs[-1].append(cls_variable)
             #if len(stmts) > 0:
             #    stmts.append(expr)
             #    return CodeBlock(stmts)
             return expr
         else:
 
             # first we check if it is a macro, in this case, we will create
@@ -2417,14 +2569,16 @@
 
         # Visit object
         if isinstance(rhs, FunctionCall):
             name = rhs.funcdef
             macro = self.scope.find(name, 'macros')
             if macro is None:
                 rhs = self._visit(rhs)
+                if isinstance(rhs, (PythonMap, PythonZip, PythonEnumerate, PythonRange)):
+                    errors.report(f"{type(rhs)} cannot be saved to variables", symbol=expr, severity='fatal')
             else:
 
                 # TODO check types from FunctionDef
                 master = macro.master
                 results = []
                 args = [self._visit(i) for i in rhs.args]
                 args_names = [arg.value.name for arg in args if isinstance(arg.value, Variable)]
@@ -3079,33 +3233,14 @@
 
             return self._visit(lhs)
         else:
             cond        = self._visit(expr.cond)
             value_false = self._visit(expr.value_false)
             return IfTernaryOperator(cond, value_true, value_false)
 
-    def _visit_VariableHeader(self, expr):
-        warnings.warn("Support for specifying types via headers will be removed in " +
-                      "a future version of Pyccel. This annotation may be unnecessary " +
-                      "in your code. If you find it is necessary please open a discussion " +
-                      "at https://github.com/pyccel/pyccel/discussions so we do not " +
-                      "remove support until an alternative is in place.", FutureWarning)
-
-        # TODO improve
-        #      move it to the ast like create_definition for FunctionHeader?
-
-        name  = expr.name
-        d_var = expr.dtypes.copy()
-        dtype = d_var.pop('datatype')
-        d_var.pop('is_func')
-
-        var = Variable(dtype, name, **d_var)
-        self.scope.insert_variable(var)
-        return expr
-
     def _visit_FunctionHeader(self, expr):
         warnings.warn("Support for specifying types via headers will be removed in a " +
                       "future version of Pyccel. Please use type hints. The @template " +
                       "decorator can be used to specify multiple types. See the " +
                       "documentation at " +
                       "https://github.com/pyccel/pyccel/blob/devel/docs/quickstart.md#type-annotations " +
                       "for examples.", FutureWarning)
@@ -3122,21 +3257,14 @@
                       "https://github.com/pyccel/pyccel/blob/devel/docs/templates.md " +
                       "for examples.", FutureWarning)
         expr.clear_syntactic_user_nodes()
         expr.update_pyccel_staging()
         self.scope.insert_template(expr)
         return expr
 
-    def _visit_ClassHeader(self, expr):
-        # TODO should we return it and keep it in the AST?
-        expr.clear_syntactic_user_nodes()
-        expr.update_pyccel_staging()
-        self.scope.insert_header(expr)
-        return expr
-
     def _visit_Return(self, expr):
 
         results     = expr.expr
         f_name      = self._current_function
         if isinstance(f_name, DottedName):
             f_name = f_name.name[-1]
 
@@ -3270,15 +3398,16 @@
                     original_symbols = expr.scope.python_names.copy())
 
             if cls_name and str(arguments[0].name) == 'self':
                 arg       = arguments[0]
                 arguments = arguments[1:]
                 dt        = self.get_class_construct(cls_name)()
                 cls_base  = self.scope.find(cls_name, 'classes')
-                var       = Variable(dt, 'self', cls_base=cls_base)
+                cls_base.scope.insert_symbols(expr.scope.local_used_symbols.copy())
+                var       = Variable(dt, 'self', cls_base=cls_base, is_argument=True)
                 self.scope.insert_variable(var)
 
             if arguments:
                 for (a, ah) in zip(arguments, m.arguments):
                     ahv = ah.var
                     if isinstance(ahv, FunctionAddress):
                         d_var = {}
@@ -3456,20 +3585,18 @@
                     body,
                     **func_kwargs)
             if not is_recursive:
                 recursive_func_obj.invalidate_node()
 
             if cls_name:
                 cls = self.scope.find(cls_name, 'classes')
-                methods = list(cls.methods) + [func]
 
                 # update the class methods
-                superclasses = self._find_superclasses(cls)
-                self.scope.update_class(ClassDef(cls_name, cls.attributes,
-                        methods, superclasses=superclasses))
+                if expr.name == func.name:
+                    cls.add_new_method(func)
 
             funcs += [func]
 
             #clear the sympy cache
             #TODO clear all variable except the global ones
             cache.clear_cache()
         if len(funcs) == 1:
@@ -3477,14 +3604,17 @@
             self.insert_function(funcs)
 
         else:
             for f in funcs:
                 self.insert_function(f)
 
             funcs = Interface(interface_name, funcs)
+            if cls_name:
+                cls = self.scope.find(cls_name, 'classes')
+                cls.add_new_interface(funcs)
             self.insert_function(funcs)
 #        TODO move this to codegen
 #        if vec_func:
 #           self._visit_FunctionDef(vec_func)
 #           vec_func = self.scope.functions.pop(vec_name)
 #           if isinstance(funcs, Interface):
 #               funcs = list(funcs.funcs)+[vec_func]
@@ -3535,77 +3665,84 @@
 
     def _visit_ClassDef(self, expr):
 
         # TODO - improve the use and def of interfaces
         #      - wouldn't be better if it is done inside ClassDef?
 
         name = expr.name
-        # remove quotes for str representation
-        name = name.replace("'", '')
 
-        parent = self._find_superclasses(expr)
+        #  create a new Datatype for the current class
+        dtype = DataTypeFactory(name, '_name')
+        self.scope.cls_constructs[name] = dtype
 
-        cls = ClassDef(name, [], [], superclasses=parent)
-        self.scope.insert_class(cls)
+        parent = self._find_superclasses(expr)
 
         scope = self.create_new_class_scope(name, used_symbols=expr.scope.local_used_symbols,
                     original_symbols = expr.scope.python_names.copy())
+
+        cls = ClassDef(name, [], [], superclasses=parent, scope=scope)
+        self.scope.parent_scope.insert_class(cls)
+
         methods = list(expr.methods)
-        interfaces = []
-        const = None
+        init_func = None
 
         for (i, method) in enumerate(methods):
-            m_name = method.name.replace("'", '')
-
+            m_name = method.name
             if m_name == '__init__':
                 self._visit_FunctionDef(method)
                 methods.pop(i)
-                const = self.scope.functions.pop(m_name)
-                break
-
+                init_func = self.scope.functions.pop(m_name)
 
+                # create a new attribute to check allocation
+                deallocater_rhs = Variable(NativeBool(), self.scope.get_new_name('is_freed'))
+                deallocater_lhs = Variable(cls.name, 'self', cls_base = cls, is_argument=True)
+                deallocater = DottedVariable(*deallocater_rhs, lhs = deallocater_lhs, name = deallocater_rhs.name, dtype = deallocater_rhs.dtype)
+                cls.add_new_attribute(deallocater)
+                deallocater_assign = Assign(deallocater, LiteralFalse())
+                cls.methods[i].body.insert2body(deallocater_assign, back=False)
+                break
 
-        if not const:
+        if not init_func:
             errors.report(UNDEFINED_INIT_METHOD, symbol=name,
                    bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
                    severity='error')
 
-        ms = []
         for i in methods:
             self._visit_FunctionDef(i)
-            m_name = i.name.replace("'", '')
-            m = self.scope.functions.pop(m_name)
-            ms.append(m)
-
-        methods = [const] + ms
-        header = self.get_headers(name)
 
-        if not header:
-            errors.report(PYCCEL_MISSING_HEADER, symbol=name,
-                   bounding_box=(self._current_fst_node.lineno, self._current_fst_node.col_offset),
-                   severity='fatal')
-
-        attributes = self.scope.find(name, 'classes').attributes
+        if not any(method.name == '__del__' for method in methods):
+            argument = FunctionDefArgument(Variable(cls.name, 'self', cls_base = cls))
+            scope = self.create_new_function_scope('__del__')
+            del_method = FunctionDef('__del__', [argument], (), [Pass()], cls_name=cls.name, scope=scope)
+            self.exit_function_scope()
+            self.insert_function(del_method)
+            cls.add_new_method(del_method)
 
-        for i in methods.copy():
-            if isinstance(i, Interface):
-                methods.remove(i)
-                interfaces += [i]
+        for method in cls.methods:
+            if method.name == '__del__':
+                self._current_function = method.name
+                attribute = [attr for attr in cls.attributes if not attr.on_stack]
+                if attribute:
+                    # Create a new list that store local attributes
+                    self._allocs.append([])
+                    self._allocs[-1].extend(attribute)
+                    method.body.insert2body(*self._garbage_collector(method.body))
+                condition = If(IfSection(PyccelNot(deallocater),
+                                [method.body]+[Assign(deallocater, LiteralTrue())]))
+                method.body = [condition]
+                self._current_function = None
+                break
 
         self.exit_class_scope()
 
-        cls = ClassDef(name, attributes, methods,
-              interfaces=interfaces, superclasses=parent, scope=scope)
-        self.scope.update_class(cls)
-
         return EmptyNode()
 
     def _visit_Del(self, expr):
 
-        ls = [self._visit(i) for i in expr.variables]
+        ls = [Deallocate(self._visit(i)) for i in expr.variables]
         return Del(ls)
 
     def _visit_PyccelIs(self, expr):
         # Handles PyccelIs and PyccelIsNot
         IsClass = type(expr)
 
         # TODO ERROR wrong position ??
@@ -3724,16 +3861,21 @@
 
             p       = self.d_parsers[source_target]
             import_init = p.semantic_parser.ast.init_func if source_target not in container['imports'] else None
             import_free = p.semantic_parser.ast.free_func if source_target not in container['imports'] else None
             if expr.target:
                 targets = {i.target if isinstance(i,AsName) else i:None for i in expr.target}
                 names = [i.name if isinstance(i,AsName) else i for i in expr.target]
-                for entry in ['variables', 'classes', 'functions']:
-                    d_son = getattr(p.scope, entry)
+
+                p_scope = p.scope
+                p_imports = p_scope.imports
+                entries = ['variables', 'classes', 'functions']
+                direct_sons = ((e,getattr(p.scope, e)) for e in entries)
+                import_sons = ((e,p_imports[e]) for e in entries)
+                for entry, d_son in chain(direct_sons, import_sons):
                     for t,n in zip(targets.keys(),names):
                         if n in d_son:
                             e = d_son[n]
                             if t == n:
                                 container[entry][t] = e
                             else:
                                 container[entry][t] = e.clone(t)
```

### Comparing `pyccel-1.9.1/pyccel/parser/syntactic.py` & `pyccel-1.9.2/pyccel/parser/syntactic.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 
 import os
 import re
 
 import ast
 import warnings
 
+from textx.exceptions import TextXSyntaxError
+
 #==============================================================================
 
 from sympy.core import cache
 
 #==============================================================================
 
 from pyccel.ast.basic import Basic
@@ -58,15 +60,15 @@
 from pyccel.ast.headers  import MetaVariable
 from pyccel.ast.literals import LiteralInteger, LiteralFloat, LiteralComplex
 from pyccel.ast.literals import LiteralFalse, LiteralTrue, LiteralString
 from pyccel.ast.literals import Nil
 from pyccel.ast.functionalexpr import FunctionalSum, FunctionalMax, FunctionalMin, GeneratorComprehension, FunctionalFor
 from pyccel.ast.variable  import DottedName
 
-from pyccel.ast.internals import Slice, PyccelSymbol, PyccelInternalFunction
+from pyccel.ast.internals import Slice, PyccelSymbol, PyccelInternalFunction, AnnotatedPyccelSymbol
 
 from pyccel.parser.base        import BasicParser
 from pyccel.parser.extend_tree import extend_tree
 from pyccel.parser.utilities   import read_file
 from pyccel.parser.utilities   import get_default_path
 
 from pyccel.parser.syntax.headers import parse as hdr_parse
@@ -177,22 +179,59 @@
 
         return ast
 
     def _treat_iterable(self, stmt):
         return (self._visit(i) for i in stmt)
 
     def _treat_comment_line(self, line, stmt):
+        """
+        Parse a comment line.
+
+        Parse a comment which fits in a single line. If the comment
+        begins with `#$` then it should contain a header recognised
+        by Pyccel and should be parsed using textx.
+
+        Parameters
+        ----------
+        line : str
+            The comment line.
+        stmt : ast.Ast
+            The comment object in the code. This is useful for raising
+            neat errors.
+
+        Returns
+        -------
+        pyccel.ast.basic.Basic
+            The treated object as a Pyccel ast node.
+        """
         if line.startswith('#$'):
             env = line[2:].lstrip()
             if env.startswith('omp'):
-                expr = omp_parse(stmts=line)
+                try:
+                    expr = omp_parse(stmts=line)
+                except TextXSyntaxError as e:
+                    errors.report(f"Invalid OpenMP header. {e.message}",
+                            symbol = stmt, column = e.col,
+                              severity='fatal')
             elif env.startswith('acc'):
-                expr = acc_parse(stmts=line)
+                try:
+                    expr = acc_parse(stmts=line)
+                except TextXSyntaxError as e:
+                    errors.report(f"Invalid OpenACC header. {e.message}",
+                            symbol = stmt, column = e.col,
+                              severity='fatal')
             elif env.startswith('header'):
-                expr = hdr_parse(stmts=line)
+                try:
+                    expr = hdr_parse(stmts=line)
+                except TextXSyntaxError as e:
+                    errors.report(f"Invalid header. {e.message}",
+                            symbol = stmt, column = e.col,
+                              severity='fatal')
+                if isinstance(expr, AnnotatedPyccelSymbol):
+                    self.scope.insert_symbol(expr.name)
                 if isinstance(expr, MetaVariable):
 
                     # a metavar will not appear in the semantic stage.
                     # but can be used to modify the ast
 
                     self._metavars[str(expr.name)] = expr.value
                     expr = EmptyNode()
@@ -746,16 +785,18 @@
                         container = ls[-1].value
                         container = container if isinstance(container, PythonTuple) else [container]
                         results = fill_types(container)
                     types = fill_types(ls[:-1])
                 else:
                     types = fill_types(ls)
 
-                txt  = '#$ header ' + name
-                txt += '(' + ','.join(types) + ')'
+                txt  = '#$ header '
+                if len(self._context) > 1 and isinstance(self._context[-2], ast.ClassDef):
+                    txt += 'method '
+                txt += name + '(' + ','.join(types) + ')'
 
                 if results:
                     txt += ' results(' + ','.join(results) + ')'
 
                 header = hdr_parse(stmts=txt)
                 headers += [header]
```

### Comparing `pyccel-1.9.1/pyccel/parser/syntax/basic.py` & `pyccel-1.9.2/pyccel/parser/syntax/basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/parser/syntax/headers.py` & `pyccel-1.9.2/pyccel/parser/syntax/headers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # coding: utf-8
 #------------------------------------------------------------------------------------------#
 # This file is part of Pyccel which is released under MIT License. See the LICENSE file or #
 # go to https://github.com/pyccel/pyccel/blob/master/LICENSE for full license details.     #
 #------------------------------------------------------------------------------------------#
 """
 """
+import warnings
 from os.path import join, dirname
 
 from textx.metamodel import metamodel_from_file
 
 from pyccel.parser.syntax.basic import BasicStmt
-from pyccel.ast.headers   import FunctionHeader, ClassHeader, MethodHeader, VariableHeader, Template
+from pyccel.ast.headers   import FunctionHeader, MethodHeader, Template
 from pyccel.ast.headers   import MetaVariable , UnionType, InterfaceHeader
 from pyccel.ast.headers   import construct_macro, MacroFunction, MacroVariable
 from pyccel.ast.core      import FunctionDefArgument, EmptyNode
 from pyccel.ast.variable  import DottedName
 from pyccel.ast.datatypes import dtype_and_precision_registry as dtype_registry, default_precision
+from pyccel.ast.datatypes import NativeNumeric
 from pyccel.ast.literals  import LiteralString, LiteralInteger, LiteralFloat
 from pyccel.ast.literals  import LiteralTrue, LiteralFalse
-from pyccel.ast.internals import PyccelSymbol
+from pyccel.ast.internals import PyccelSymbol, AnnotatedPyccelSymbol
+from pyccel.ast.type_annotations import SyntacticTypeAnnotation
 from pyccel.errors.errors import Errors
 from pyccel.utilities.stage import PyccelStage
 
 DEBUG = False
 errors = Errors()
 pyccel_stage = PyccelStage()
 
@@ -109,31 +112,50 @@
         d_var['is_const'] = False
         if not(d_var['precision']):
             if d_var['datatype'] in ['double','float','complex','int']:
                 d_var['precision'] = default_precision[d_var['datatype']]
         return d_var
 
 class Type(BasicStmt):
-    """Base class representing a header type in the grammar."""
+    """
+    Base class representing a header type in the grammar.
 
-    def __init__(self, **kwargs):
-        """
-        Constructor for a Type.
+    Base class representing a header type in the grammar.
 
-        dtype: str
-            variable type
-        """
-        self.dtype   = kwargs.pop('dtype')
-        self.prec    = kwargs.pop('prec')
-        self.trailer = kwargs.pop('trailer', [])
+    Parameters
+    ----------
+    dtype : str
+        The variable type.
+
+    prec : int
+        The precision of the object.
+
+    trailer : iterable, TrailerSubscriptsList
+        An object created by textx describing the trailing decorators of the
+        type. The number of elements is equal to the rank. The order is also
+        described when the iterable is non-empty.
+
+    **kwargs : dict
+        The textx arguments.
+    """
+
+    def __init__(self, dtype, prec, trailer = (), **kwargs):
+        self.dtype   = dtype
+        self.prec    = prec
+        self.trailer = trailer
 
         super(Type, self).__init__(**kwargs)
 
     @property
     def expr(self):
+        """
+        Get the dictionary describing the type.
+
+        Get the dictionary describing the type.
+        """
         dtype = self.dtype
         precision = self.prec
         if dtype in dtype_registry.keys():
             dtype,precision = dtype_registry[dtype]
         trailer = self.trailer
         order = 'C'
 
@@ -147,15 +169,15 @@
         d_var['datatype']=dtype
         d_var['rank'] = len(trailer)
         d_var['memory_handling'] = 'heap' if len(trailer) > 0 else 'stack'
         d_var['precision']  = precision
         d_var['is_func'] = False
         d_var['is_const'] = False
         if not(precision):
-            if dtype in ['double' ,'float','complex', 'int']:
+            if dtype in NativeNumeric:
                 d_var['precision'] = default_precision[dtype]
 
         if d_var['rank']>1:
             d_var['order'] = order
         return d_var
 
 class ShapedID(BasicStmt):
@@ -241,36 +263,51 @@
     @property
     def expr(self):
         decs = [i.expr for i in self.decs]
         return decs
 
 
 class VariableHeaderStmt(BasicStmt):
-    """Base class representing a header statement in the grammar."""
+    """
+    Base class representing a header statement in the grammar.
 
-    def __init__(self, **kwargs):
-        """
-        Constructor for a VariableHeader statement.
-        In the case of builtin datatypes, we export a Variable
+    Base class representing a header statement in the grammar.
+    To be removed when header support is deprecated.
 
-        name: str
-            variable name
-        dec: list, tuple
-            list of argument types
-        """
-        self.name = kwargs.pop('name')
-        self.dec  = kwargs.pop('dec')
+    Parameters
+    ----------
+    name : str
+        Variable name.
+    dec : list, tuple
+        List of argument types.
+    **kwargs : dict
+        TextX keyword arguments.
+    """
+
+    def __init__(self, name, dec, **kwargs):
+        self.name = name
+        self.dec  = dec
 
         super(VariableHeaderStmt, self).__init__(**kwargs)
 
     @property
     def expr(self):
-        dtype = self.dec.expr
+        """
+        Convert a VariableHeaderStmt generated by TextX to a Pyccel AST object.
+
+        Convert a VariableHeaderStmt generated by TextX to a Pyccel AST object.
+        """
+        warnings.warn("Support for specifying types via headers will be removed in " +
+                      "a future version of Pyccel. This annotation may be unnecessary " +
+                      "in your code. If you find it is necessary please open a discussion " +
+                      "at https://github.com/pyccel/pyccel/discussions so we do not " +
+                      "remove support until an alternative is in place.", FutureWarning)
+        dtype = SyntacticTypeAnnotation.build_from_textx(self.dec)
 
-        return VariableHeader(self.name, dtype)
+        return AnnotatedPyccelSymbol(self.name, annotation=dtype)
 
 class FunctionHeaderStmt(BasicStmt):
     """Base class representing a function header statement in the grammar."""
 
     def __init__(self, **kwargs):
         """
         Constructor for a FunctionHeader statement
@@ -323,36 +360,14 @@
             return MethodHeader((cls_instance, self.name), dtypes, [] )
         else:
             return FunctionHeader(self.name,
                                   dtypes,
                                   results=results,
                                   is_static=is_static)
 
-class ClassHeaderStmt(BasicStmt):
-    """Base class representing a class header statement in the grammar."""
-
-    def __init__(self, **kwargs):
-        """
-        Constructor for a Header statement
-
-        name: str
-            class name
-        options: list, tuple
-            list of class options
-        """
-        self.name    = kwargs.pop('name')
-        self.options = kwargs.pop('options')
-
-        super(ClassHeaderStmt, self).__init__(**kwargs)
-
-    @property
-    def expr(self):
-        options = [str(i) for i in self.options]
-        return ClassHeader(self.name, options)
-
 
 class MetavarHeaderStmt(BasicStmt):
     """Base class representing a metavar header statement in the grammar."""
 
     def __init__(self, **kwargs):
         """
         Constructor for a MetavarHeader statement.
@@ -543,15 +558,14 @@
 # lists.
 hdr_classes = [Header, TypeHeader,
                Type, ListType, UnionTypeStmt, FuncType,
                ShapedID,
                HeaderResults,
                FunctionHeaderStmt,
                TemplateStmt,
-               ClassHeaderStmt,
                VariableHeaderStmt,
                MetavarHeaderStmt,
                InterfaceStmt,
                MacroStmt,
                MacroArg,
                MacroList,
                FunctionMacroStmt,StringStmt]
@@ -603,15 +617,14 @@
 #=========================================================================================================
 #=========================================================================================================
 if __name__ == '__main__':
     print(parse(stmts='#$ header variable x :: int'))
     print(parse(stmts='#$ header variable x float [:, :]'))
     print(parse(stmts='#$ header function f(float [:], int [:]) results(int)'))
     print(parse(stmts='#$ header function f(float|int, int [:]) results(int)'))
-    print(parse(stmts='#$ header class Square(public)'))
     print(parse(stmts='#$ header method translate(Point, [double], [int], int[:,:], double[:])'))
     print(parse(stmts="#$ header metavar module_name='mpi'"))
     print(parse(stmts='#$ header interface funcs=fun1|fun2|fun3'))
     print(parse(stmts='#$ header function _f(int, int [:])'))
     print(parse(stmts='#$ header macro _f(x) := f(x, x.shape)'))
     print(parse(stmts='#$ header macro _g(x) := g(x, x.shape[0], x.shape[1])'))
     print(parse(stmts='#$ header macro (a, b), _f(x) := f(x.shape, x, a, b)'))
```

### Comparing `pyccel-1.9.1/pyccel/parser/syntax/openacc.py` & `pyccel-1.9.2/pyccel/parser/syntax/openacc.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/parser/syntax/openmp.py` & `pyccel-1.9.2/pyccel/parser/syntax/openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/parser/utilities.py` & `pyccel-1.9.2/pyccel/parser/utilities.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/cwrapper/cwrapper.c` & `pyccel-1.9.2/pyccel/stdlib/cwrapper/cwrapper.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/cwrapper/cwrapper.h` & `pyccel-1.9.2/pyccel/stdlib/cwrapper/cwrapper.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c` & `pyccel-1.9.2/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h` & `pyccel-1.9.2/pyccel/stdlib/cwrapper_ndarrays/cwrapper_ndarrays.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/external/dfftpack.py` & `pyccel-1.9.2/pyccel/stdlib/external/dfftpack.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/external/fitpack.py` & `pyccel-1.9.2/pyccel/stdlib/external/fitpack.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/external/lapack.py` & `pyccel-1.9.2/pyccel/stdlib/external/lapack.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/external/mpi4py.py` & `pyccel-1.9.2/pyccel/stdlib/external/mpi4py.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/blas.pyh` & `pyccel-1.9.2/pyccel/stdlib/internal/blas.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/dfftpack.pyccel` & `pyccel-1.9.2/pyccel/stdlib/internal/dfftpack.pyccel`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-00000000: 8004 954b 1700 0000 0000 008c 2031 3362  ...K........ 13b
+00000000: 8004 9589 1700 0000 0000 008c 2031 3362  ............ 13b
 00000010: 6133 3830 6537 3438 3037 6630 3830 3266  a380e74807f0802f
 00000020: 6366 3030 3564 6138 3432 6366 3894 8c05  cf005da842cf8...
-00000030: 312e 392e 3194 8c17 7079 6363 656c 2e70  1.9.1...pyccel.p
+00000030: 312e 392e 3294 8c17 7079 6363 656c 2e70  1.9.2...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 7804 0000 2320 7079 6363 656c 2068 6561  x...# pyccel hea
 00000080: 6465 7220 666f 7220 4446 5454 5041 434b  der for DFTTPACK
 00000090: 2e0a 0a23 2420 6865 6164 6572 206d 6574  ...#$ header met
 000000a0: 6176 6172 2069 676e 6f72 655f 6174 5f69  avar ignore_at_i
@@ -73,302 +73,306 @@
 00000480: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
 00000490: 207a 6666 7466 2869 6e74 2c20 636f 6d70   zfftf(int, comp
 000004a0: 6c65 7820 5b3a 5d2c 2064 6f75 626c 6520  lex [:], double 
 000004b0: 5b3a 5d29 0a23 2420 6865 6164 6572 2066  [:]).#$ header f
 000004c0: 756e 6374 696f 6e20 7a66 6674 6228 696e  unction zfftb(in
 000004d0: 742c 2063 6f6d 706c 6578 205b 3a5d 2c20  t, complex [:], 
 000004e0: 646f 7562 6c65 205b 3a5d 290a 948c 045f  double [:])...._
-000004f0: 6673 7494 8c03 6173 7494 8c06 4d6f 6475  fst...ast...Modu
-00000500: 6c65 9493 9429 5294 7d94 288c 0462 6f64  le...)R.}.(..bod
-00000510: 7994 5d94 288c 1970 7963 6365 6c2e 7061  y.].(..pyccel.pa
-00000520: 7273 6572 2e65 7874 656e 645f 7472 6565  rser.extend_tree
-00000530: 948c 0b43 6f6d 6d65 6e74 4c69 6e65 9493  ...CommentLine..
-00000540: 948c 1d23 2070 7963 6365 6c20 6865 6164  ...# pyccel head
-00000550: 6572 2066 6f72 2044 4654 5450 4143 4b2e  er for DFTTPACK.
-00000560: 944b 014b 0087 9452 9468 118c 1043 6f6d  .K.K...R.h...Com
-00000570: 6d65 6e74 4d75 6c74 694c 696e 6594 9394  mentMultiLine...
-00000580: 8c8a 2324 2068 6561 6465 7220 6d65 7461  ..#$ header meta
-00000590: 7661 7220 6967 6e6f 7265 5f61 745f 696d  var ignore_at_im
-000005a0: 706f 7274 3d54 7275 650a 2324 2068 6561  port=True.#$ hea
-000005b0: 6465 7220 6d65 7461 7661 7220 6d6f 6475  der metavar modu
-000005c0: 6c65 5f76 6572 7369 6f6e 3d27 312e 3027  le_version='1.0'
-000005d0: 0a23 2420 6865 6164 6572 206d 6574 6176  .#$ header metav
-000005e0: 6172 2073 6176 653d 5472 7565 0a23 2420  ar save=True.#$ 
-000005f0: 6865 6164 6572 206d 6574 6176 6172 2065  header metavar e
-00000600: 7874 6572 6e61 6c3d 5472 7565 944b 034b  xternal=True.K.K
-00000610: 0087 9452 9468 188c 9523 2420 6865 6164  ...R.h...#$ head
-00000620: 6572 2066 756e 6374 696f 6e20 6466 6674  er function dfft
-00000630: 6928 696e 742c 2064 6f75 626c 6520 5b3a  i(int, double [:
-00000640: 5d29 0a23 2420 6865 6164 6572 2066 756e  ]).#$ header fun
-00000650: 6374 696f 6e20 6466 6674 6628 696e 742c  ction dfftf(int,
-00000660: 2064 6f75 626c 6520 5b3a 5d2c 2064 6f75   double [:], dou
-00000670: 626c 6520 5b3a 5d29 0a23 2420 6865 6164  ble [:]).#$ head
-00000680: 6572 2066 756e 6374 696f 6e20 6466 6674  er function dfft
-00000690: 6228 696e 742c 2064 6f75 626c 6520 5b3a  b(int, double [:
-000006a0: 5d2c 2064 6f75 626c 6520 5b3a 5d29 944b  ], double [:]).K
-000006b0: 0a4b 0087 9452 9468 188c 9823 2420 6865  .K...R.h...#$ he
-000006c0: 6164 6572 2066 756e 6374 696f 6e20 647a  ader function dz
-000006d0: 6666 7469 2869 6e74 2c20 646f 7562 6c65  ffti(int, double
-000006e0: 205b 3a5d 290a 2324 2068 6561 6465 7220   [:]).#$ header 
-000006f0: 6675 6e63 7469 6f6e 2064 7a66 6674 6628  function dzfftf(
-00000700: 696e 742c 2064 6f75 626c 6520 5b3a 5d2c  int, double [:],
-00000710: 2064 6f75 626c 6520 5b3a 5d29 0a23 2420   double [:]).#$ 
-00000720: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
-00000730: 647a 6666 7462 2869 6e74 2c20 646f 7562  dzfftb(int, doub
-00000740: 6c65 205b 3a5d 2c20 646f 7562 6c65 205b  le [:], double [
-00000750: 3a5d 2994 4b0e 4b00 8794 5294 6818 8c9b  :]).K.K...R.h...
-00000760: 2324 2068 6561 6465 7220 6675 6e63 7469  #$ header functi
-00000770: 6f6e 2064 636f 7371 6928 696e 7420 2c20  on dcosqi(int , 
-00000780: 646f 7562 6c65 205b 3a5d 290a 2324 2068  double [:]).#$ h
-00000790: 6561 6465 7220 6675 6e63 7469 6f6e 2064  eader function d
-000007a0: 636f 7371 6628 696e 7420 2c20 646f 7562  cosqf(int , doub
-000007b0: 6c65 205b 3a5d 2c20 646f 7562 6c65 205b  le [:], double [
-000007c0: 3a5d 290a 2324 2068 6561 6465 7220 6675  :]).#$ header fu
-000007d0: 6e63 7469 6f6e 2064 636f 7371 6228 696e  nction dcosqb(in
-000007e0: 7420 2c20 646f 7562 6c65 205b 3a5d 2c20  t , double [:], 
-000007f0: 646f 7562 6c65 205b 3a5d 2994 4b12 4b00  double [:]).K.K.
-00000800: 8794 5294 6818 8c63 2324 2068 6561 6465  ..R.h..c#$ heade
-00000810: 7220 6675 6e63 7469 6f6e 2064 636f 7374  r function dcost
-00000820: 6928 696e 7420 2c20 646f 7562 6c65 205b  i(int , double [
-00000830: 3a5d 290a 2324 2068 6561 6465 7220 6675  :]).#$ header fu
-00000840: 6e63 7469 6f6e 2064 636f 7374 2028 696e  nction dcost (in
-00000850: 7420 2c20 646f 7562 6c65 205b 3a5d 2c20  t , double [:], 
-00000860: 646f 7562 6c65 205b 3a5d 2994 4b16 4b00  double [:]).K.K.
-00000870: 8794 5294 6818 8c9b 2324 2068 6561 6465  ..R.h...#$ heade
-00000880: 7220 6675 6e63 7469 6f6e 2064 7369 6e71  r function dsinq
-00000890: 6928 696e 7420 2c20 646f 7562 6c65 205b  i(int , double [
-000008a0: 3a5d 290a 2324 2068 6561 6465 7220 6675  :]).#$ header fu
-000008b0: 6e63 7469 6f6e 2064 7369 6e71 6628 696e  nction dsinqf(in
-000008c0: 7420 2c20 646f 7562 6c65 205b 3a5d 2c20  t , double [:], 
-000008d0: 646f 7562 6c65 205b 3a5d 290a 2324 2068  double [:]).#$ h
-000008e0: 6561 6465 7220 6675 6e63 7469 6f6e 2064  eader function d
-000008f0: 7369 6e71 6228 696e 7420 2c20 646f 7562  sinqb(int , doub
-00000900: 6c65 205b 3a5d 2c20 646f 7562 6c65 205b  le [:], double [
-00000910: 3a5d 2994 4b19 4b00 8794 5294 6818 8c61  :]).K.K...R.h..a
-00000920: 2324 2068 6561 6465 7220 6675 6e63 7469  #$ header functi
-00000930: 6f6e 2064 7369 6e74 6928 696e 742c 2064  on dsinti(int, d
-00000940: 6f75 626c 6520 5b3a 5d29 0a23 2420 6865  ouble [:]).#$ he
-00000950: 6164 6572 2066 756e 6374 696f 6e20 6473  ader function ds
-00000960: 696e 7420 2869 6e74 2c20 646f 7562 6c65  int (int, double
-00000970: 205b 3a5d 2c20 646f 7562 6c65 205b 3a5d   [:], double [:]
-00000980: 2994 4b1d 4b00 8794 5294 6818 8c97 2324  ).K.K...R.h...#$
-00000990: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
-000009a0: 207a 6666 7469 2869 6e74 2c20 646f 7562   zffti(int, doub
-000009b0: 6c65 205b 3a5d 290a 2324 2068 6561 6465  le [:]).#$ heade
-000009c0: 7220 6675 6e63 7469 6f6e 207a 6666 7466  r function zfftf
-000009d0: 2869 6e74 2c20 636f 6d70 6c65 7820 5b3a  (int, complex [:
-000009e0: 5d2c 2064 6f75 626c 6520 5b3a 5d29 0a23  ], double [:]).#
-000009f0: 2420 6865 6164 6572 2066 756e 6374 696f  $ header functio
-00000a00: 6e20 7a66 6674 6228 696e 742c 2063 6f6d  n zfftb(int, com
-00000a10: 706c 6578 205b 3a5d 2c20 646f 7562 6c65  plex [:], double
-00000a20: 205b 3a5d 2994 4b20 4b00 8794 5294 658c   [:]).K K...R.e.
-00000a30: 0c74 7970 655f 6967 6e6f 7265 7394 5d94  .type_ignores.].
-00000a40: 8c06 6c69 6e65 6e6f 944b 018c 0a63 6f6c  ..lineno.K...col
-00000a50: 5f6f 6666 7365 7494 4b01 7562 8c04 5f61  _offset.K.ub.._a
-00000a60: 7374 948c 0f70 7963 6365 6c2e 6173 742e  st...pyccel.ast.
-00000a70: 636f 7265 948c 064d 6f64 756c 6594 9394  core...Module...
-00000a80: 2981 944e 7d94 288c 055f 6e61 6d65 9468  )..N}.(.._name.h
-00000a90: 368c 0641 734e 616d 6594 9394 2981 944e  6..AsName...)..N
-00000aa0: 7d94 288c 045f 6f62 6a94 8c08 6466 6674  }.(.._obj...dfft
-00000ab0: 7061 636b 948c 075f 7461 7267 6574 948c  pack..._target..
-00000ac0: 1470 7963 6365 6c2e 6173 742e 696e 7465  .pyccel.ast.inte
-00000ad0: 726e 616c 7394 8c0c 5079 6363 656c 5379  rnals...PyccelSy
-00000ae0: 6d62 6f6c 9493 948c 0864 6666 7470 6163  mbol.....dfftpac
-00000af0: 6b94 8594 8194 4e7d 948c 085f 6973 5f74  k.....N}..._is_t
-00000b00: 656d 7094 8973 8694 628c 0b5f 7573 6572  emp..s..b.._user
-00000b10: 5f6e 6f64 6573 945d 9468 095d 948c 165f  _nodes.].h.]..._
-00000b20: 7265 6375 7273 696f 6e5f 696e 5f70 726f  recursion_in_pro
-00000b30: 6772 6573 7394 898c 0f5f 7079 6363 656c  gress...._pyccel
-00000b40: 5f73 7461 6769 6e67 948c 0973 796e 7461  _staging...synta
-00000b50: 6374 6963 9475 8694 628c 0a5f 7661 7269  ctic.u..b.._vari
-00000b60: 6162 6c65 7394 298c 065f 6675 6e63 7394  ables.).._funcs.
-00000b70: 298c 0b5f 696e 7465 7266 6163 6573 9429  ).._interfaces.)
-00000b80: 8c08 5f63 6c61 7373 6573 9429 8c08 5f69  .._classes.).._i
-00000b90: 6d70 6f72 7473 9429 8c0a 5f69 6e69 745f  mports.).._init_
-00000ba0: 6675 6e63 944e 8c0a 5f66 7265 655f 6675  func.N.._free_fu
-00000bb0: 6e63 944e 8c08 5f70 726f 6772 616d 9468  nc.N.._program.h
-00000bc0: 368c 0561 7070 6c79 9493 9468 368c 0943  6..apply...h6..C
-00000bd0: 6f64 6542 6c6f 636b 9493 9429 7d94 680f  odeBlock...)}.h.
-00000be0: 2868 5c68 368c 0743 6f6d 6d65 6e74 9493  (h\h6..Comment..
-00000bf0: 9429 7d94 8c04 7465 7874 948c 1b70 7963  .)}...text...pyc
-00000c00: 6365 6c20 6865 6164 6572 2066 6f72 2044  cel header for D
-00000c10: 4654 5450 4143 4b2e 9473 8794 5294 8c12  FTTPACK..s..R...
-00000c20: 7079 6363 656c 2e61 7374 2e68 6561 6465  pyccel.ast.heade
-00000c30: 7273 948c 0e46 756e 6374 696f 6e48 6561  rs...FunctionHea
-00000c40: 6465 7294 9394 288c 0564 6666 7469 945d  der...(..dffti.]
-00000c50: 9428 7d94 288c 0864 6174 6174 7970 6594  .(}.(..datatype.
-00000c60: 8c03 696e 7494 8c04 7261 6e6b 944b 008c  ..int...rank.K..
-00000c70: 0f6d 656d 6f72 795f 6861 6e64 6c69 6e67  .memory_handling
-00000c80: 948c 0573 7461 636b 948c 0970 7265 6369  ...stack...preci
-00000c90: 7369 6f6e 944a ffff ffff 8c07 6973 5f66  sion.J......is_f
-00000ca0: 756e 6394 898c 0869 735f 636f 6e73 7494  unc....is_const.
-00000cb0: 8975 7d94 2868 6d8c 0566 6c6f 6174 9468  .u}.(hm..float.h
-00000cc0: 6f4b 0168 708c 0468 6561 7094 6872 4aff  oK.hp..heap.hrJ.
-00000cd0: ffff ff68 7389 6874 8975 655d 9489 7494  ...hs.ht.ue]..t.
-00000ce0: 5294 6869 288c 0564 6666 7466 945d 9428  R.hi(..dfftf.].(
-00000cf0: 7d94 2868 6d68 6e68 6f4b 0068 7068 7168  }.(hmhnhoK.hphqh
-00000d00: 724a ffff ffff 6873 8968 7489 757d 9428  rJ....hs.ht.u}.(
-00000d10: 686d 6876 686f 4b01 6870 6877 6872 4aff  hmhvhoK.hphwhrJ.
-00000d20: ffff ff68 7389 6874 8975 7d94 2868 6d68  ...hs.ht.u}.(hmh
-00000d30: 7668 6f4b 0168 7068 7768 724a ffff ffff  vhoK.hphwhrJ....
-00000d40: 6873 8968 7489 7565 5d94 8974 9452 9468  hs.ht.ue]..t.R.h
-00000d50: 6928 8c05 6466 6674 6294 5d94 287d 9428  i(..dfftb.].(}.(
-00000d60: 686d 686e 686f 4b00 6870 6871 6872 4aff  hmhnhoK.hphqhrJ.
-00000d70: ffff ff68 7389 6874 8975 7d94 2868 6d68  ...hs.ht.u}.(hmh
-00000d80: 7668 6f4b 0168 7068 7768 724a ffff ffff  vhoK.hphwhrJ....
-00000d90: 6873 8968 7489 757d 9428 686d 6876 686f  hs.ht.u}.(hmhvho
-00000da0: 4b01 6870 6877 6872 4aff ffff ff68 7389  K.hphwhrJ....hs.
-00000db0: 6874 8975 655d 9489 7494 5294 6869 288c  ht.ue]..t.R.hi(.
-00000dc0: 0664 7a66 6674 6994 5d94 287d 9428 686d  .dzffti.].(}.(hm
-00000dd0: 686e 686f 4b00 6870 6871 6872 4aff ffff  hnhoK.hphqhrJ...
-00000de0: ff68 7389 6874 8975 7d94 2868 6d68 7668  .hs.ht.u}.(hmhvh
-00000df0: 6f4b 0168 7068 7768 724a ffff ffff 6873  oK.hphwhrJ....hs
-00000e00: 8968 7489 7565 5d94 8974 9452 9468 6928  .ht.ue]..t.R.hi(
-00000e10: 8c06 647a 6666 7466 945d 9428 7d94 2868  ..dzfftf.].(}.(h
-00000e20: 6d68 6e68 6f4b 0068 7068 7168 724a ffff  mhnhoK.hphqhrJ..
-00000e30: ffff 6873 8968 7489 757d 9428 686d 6876  ..hs.ht.u}.(hmhv
-00000e40: 686f 4b01 6870 6877 6872 4aff ffff ff68  hoK.hphwhrJ....h
-00000e50: 7389 6874 8975 7d94 2868 6d68 7668 6f4b  s.ht.u}.(hmhvhoK
-00000e60: 0168 7068 7768 724a ffff ffff 6873 8968  .hphwhrJ....hs.h
-00000e70: 7489 7565 5d94 8974 9452 9468 6928 8c06  t.ue]..t.R.hi(..
-00000e80: 647a 6666 7462 945d 9428 7d94 2868 6d68  dzfftb.].(}.(hmh
-00000e90: 6e68 6f4b 0068 7068 7168 724a ffff ffff  nhoK.hphqhrJ....
-00000ea0: 6873 8968 7489 757d 9428 686d 6876 686f  hs.ht.u}.(hmhvho
-00000eb0: 4b01 6870 6877 6872 4aff ffff ff68 7389  K.hphwhrJ....hs.
-00000ec0: 6874 8975 7d94 2868 6d68 7668 6f4b 0168  ht.u}.(hmhvhoK.h
-00000ed0: 7068 7768 724a ffff ffff 6873 8968 7489  phwhrJ....hs.ht.
-00000ee0: 7565 5d94 8974 9452 9468 6928 8c06 6463  ue]..t.R.hi(..dc
-00000ef0: 6f73 7169 945d 9428 7d94 2868 6d68 6e68  osqi.].(}.(hmhnh
-00000f00: 6f4b 0068 7068 7168 724a ffff ffff 6873  oK.hphqhrJ....hs
-00000f10: 8968 7489 757d 9428 686d 6876 686f 4b01  .ht.u}.(hmhvhoK.
-00000f20: 6870 6877 6872 4aff ffff ff68 7389 6874  hphwhrJ....hs.ht
-00000f30: 8975 655d 9489 7494 5294 6869 288c 0664  .ue]..t.R.hi(..d
-00000f40: 636f 7371 6694 5d94 287d 9428 686d 686e  cosqf.].(}.(hmhn
-00000f50: 686f 4b00 6870 6871 6872 4aff ffff ff68  hoK.hphqhrJ....h
-00000f60: 7389 6874 8975 7d94 2868 6d68 7668 6f4b  s.ht.u}.(hmhvhoK
-00000f70: 0168 7068 7768 724a ffff ffff 6873 8968  .hphwhrJ....hs.h
-00000f80: 7489 757d 9428 686d 6876 686f 4b01 6870  t.u}.(hmhvhoK.hp
-00000f90: 6877 6872 4aff ffff ff68 7389 6874 8975  hwhrJ....hs.ht.u
-00000fa0: 655d 9489 7494 5294 6869 288c 0664 636f  e]..t.R.hi(..dco
-00000fb0: 7371 6294 5d94 287d 9428 686d 686e 686f  sqb.].(}.(hmhnho
-00000fc0: 4b00 6870 6871 6872 4aff ffff ff68 7389  K.hphqhrJ....hs.
-00000fd0: 6874 8975 7d94 2868 6d68 7668 6f4b 0168  ht.u}.(hmhvhoK.h
-00000fe0: 7068 7768 724a ffff ffff 6873 8968 7489  phwhrJ....hs.ht.
-00000ff0: 757d 9428 686d 6876 686f 4b01 6870 6877  u}.(hmhvhoK.hphw
-00001000: 6872 4aff ffff ff68 7389 6874 8975 655d  hrJ....hs.ht.ue]
-00001010: 9489 7494 5294 6869 288c 0664 636f 7374  ..t.R.hi(..dcost
-00001020: 6994 5d94 287d 9428 686d 686e 686f 4b00  i.].(}.(hmhnhoK.
-00001030: 6870 6871 6872 4aff ffff ff68 7389 6874  hphqhrJ....hs.ht
-00001040: 8975 7d94 2868 6d68 7668 6f4b 0168 7068  .u}.(hmhvhoK.hph
-00001050: 7768 724a ffff ffff 6873 8968 7489 7565  whrJ....hs.ht.ue
-00001060: 5d94 8974 9452 9468 6928 8c05 6463 6f73  ]..t.R.hi(..dcos
-00001070: 7494 5d94 287d 9428 686d 686e 686f 4b00  t.].(}.(hmhnhoK.
-00001080: 6870 6871 6872 4aff ffff ff68 7389 6874  hphqhrJ....hs.ht
-00001090: 8975 7d94 2868 6d68 7668 6f4b 0168 7068  .u}.(hmhvhoK.hph
-000010a0: 7768 724a ffff ffff 6873 8968 7489 757d  whrJ....hs.ht.u}
-000010b0: 9428 686d 6876 686f 4b01 6870 6877 6872  .(hmhvhoK.hphwhr
-000010c0: 4aff ffff ff68 7389 6874 8975 655d 9489  J....hs.ht.ue]..
-000010d0: 7494 5294 6869 288c 0664 7369 6e71 6994  t.R.hi(..dsinqi.
-000010e0: 5d94 287d 9428 686d 686e 686f 4b00 6870  ].(}.(hmhnhoK.hp
-000010f0: 6871 6872 4aff ffff ff68 7389 6874 8975  hqhrJ....hs.ht.u
-00001100: 7d94 2868 6d68 7668 6f4b 0168 7068 7768  }.(hmhvhoK.hphwh
-00001110: 724a ffff ffff 6873 8968 7489 7565 5d94  rJ....hs.ht.ue].
-00001120: 8974 9452 9468 6928 8c06 6473 696e 7166  .t.R.hi(..dsinqf
-00001130: 945d 9428 7d94 2868 6d68 6e68 6f4b 0068  .].(}.(hmhnhoK.h
-00001140: 7068 7168 724a ffff ffff 6873 8968 7489  phqhrJ....hs.ht.
-00001150: 757d 9428 686d 6876 686f 4b01 6870 6877  u}.(hmhvhoK.hphw
-00001160: 6872 4aff ffff ff68 7389 6874 8975 7d94  hrJ....hs.ht.u}.
-00001170: 2868 6d68 7668 6f4b 0168 7068 7768 724a  (hmhvhoK.hphwhrJ
-00001180: ffff ffff 6873 8968 7489 7565 5d94 8974  ....hs.ht.ue]..t
-00001190: 9452 9468 6928 8c06 6473 696e 7162 945d  .R.hi(..dsinqb.]
-000011a0: 9428 7d94 2868 6d68 6e68 6f4b 0068 7068  .(}.(hmhnhoK.hph
-000011b0: 7168 724a ffff ffff 6873 8968 7489 757d  qhrJ....hs.ht.u}
-000011c0: 9428 686d 6876 686f 4b01 6870 6877 6872  .(hmhvhoK.hphwhr
-000011d0: 4aff ffff ff68 7389 6874 8975 7d94 2868  J....hs.ht.u}.(h
-000011e0: 6d68 7668 6f4b 0168 7068 7768 724a ffff  mhvhoK.hphwhrJ..
-000011f0: ffff 6873 8968 7489 7565 5d94 8974 9452  ..hs.ht.ue]..t.R
-00001200: 9468 6928 8c06 6473 696e 7469 945d 9428  .hi(..dsinti.].(
-00001210: 7d94 2868 6d68 6e68 6f4b 0068 7068 7168  }.(hmhnhoK.hphqh
-00001220: 724a ffff ffff 6873 8968 7489 757d 9428  rJ....hs.ht.u}.(
-00001230: 686d 6876 686f 4b01 6870 6877 6872 4aff  hmhvhoK.hphwhrJ.
-00001240: ffff ff68 7389 6874 8975 655d 9489 7494  ...hs.ht.ue]..t.
-00001250: 5294 6869 288c 0564 7369 6e74 945d 9428  R.hi(..dsint.].(
-00001260: 7d94 2868 6d68 6e68 6f4b 0068 7068 7168  }.(hmhnhoK.hphqh
-00001270: 724a ffff ffff 6873 8968 7489 757d 9428  rJ....hs.ht.u}.(
-00001280: 686d 6876 686f 4b01 6870 6877 6872 4aff  hmhvhoK.hphwhrJ.
-00001290: ffff ff68 7389 6874 8975 7d94 2868 6d68  ...hs.ht.u}.(hmh
-000012a0: 7668 6f4b 0168 7068 7768 724a ffff ffff  vhoK.hphwhrJ....
-000012b0: 6873 8968 7489 7565 5d94 8974 9452 9468  hs.ht.ue]..t.R.h
-000012c0: 6928 8c05 7a66 6674 6994 5d94 287d 9428  i(..zffti.].(}.(
-000012d0: 686d 686e 686f 4b00 6870 6871 6872 4aff  hmhnhoK.hphqhrJ.
-000012e0: ffff ff68 7389 6874 8975 7d94 2868 6d68  ...hs.ht.u}.(hmh
-000012f0: 7668 6f4b 0168 7068 7768 724a ffff ffff  vhoK.hphwhrJ....
-00001300: 6873 8968 7489 7565 5d94 8974 9452 9468  hs.ht.ue]..t.R.h
-00001310: 6928 8c05 7a66 6674 6694 5d94 287d 9428  i(..zfftf.].(}.(
-00001320: 686d 686e 686f 4b00 6870 6871 6872 4aff  hmhnhoK.hphqhrJ.
-00001330: ffff ff68 7389 6874 8975 7d94 2868 6d8c  ...hs.ht.u}.(hm.
-00001340: 0763 6f6d 706c 6578 9468 6f4b 0168 7068  .complex.hoK.hph
-00001350: 7768 724a ffff ffff 6873 8968 7489 757d  whrJ....hs.ht.u}
-00001360: 9428 686d 6876 686f 4b01 6870 6877 6872  .(hmhvhoK.hphwhr
-00001370: 4aff ffff ff68 7389 6874 8975 655d 9489  J....hs.ht.ue]..
-00001380: 7494 5294 6869 288c 057a 6666 7462 945d  t.R.hi(..zfftb.]
-00001390: 9428 7d94 2868 6d68 6e68 6f4b 0068 7068  .(}.(hmhnhoK.hph
-000013a0: 7168 724a ffff ffff 6873 8968 7489 757d  qhrJ....hs.ht.u}
-000013b0: 9428 686d 68f9 686f 4b01 6870 6877 6872  .(hmh.hoK.hphwhr
-000013c0: 4aff ffff ff68 7389 6874 8975 7d94 2868  J....hs.ht.u}.(h
-000013d0: 6d68 7668 6f4b 0168 7068 7768 724a ffff  mhvhoK.hphwhrJ..
-000013e0: ffff 6873 8968 7489 7565 5d94 8974 9452  ..hs.ht.ue]..t.R
-000013f0: 9474 9473 8794 5294 8c0f 5f76 6172 6961  .t.s..R..._varia
-00001400: 626c 655f 696e 6974 7394 298c 145f 696e  ble_inits.).._in
-00001410: 7465 726e 616c 5f64 6963 7469 6f6e 6172  ternal_dictionar
-00001420: 7994 7d94 8c06 5f73 636f 7065 948c 1370  y.}..._scope...p
-00001430: 7963 6365 6c2e 7061 7273 6572 2e73 636f  yccel.parser.sco
-00001440: 7065 948c 0553 636f 7065 9493 9429 8194  pe...Scope...)..
-00001450: 4e7d 9428 6857 7d94 288c 0966 756e 6374  N}.(hW}.(..funct
-00001460: 696f 6e73 947d 948c 0976 6172 6961 626c  ions.}...variabl
-00001470: 6573 947d 948c 0763 6c61 7373 6573 947d  es.}...classes.}
-00001480: 948c 0769 6d70 6f72 7473 947d 948c 1273  ...imports.}...s
-00001490: 796d 626f 6c69 635f 6675 6e63 7469 6f6e  ymbolic_function
-000014a0: 7394 7d94 8c06 6d61 6372 6f73 947d 948c  s.}...macros.}..
-000014b0: 0974 656d 706c 6174 6573 947d 948c 0768  .templates.}...h
-000014c0: 6561 6465 7273 947d 948c 0a64 6563 6f72  eaders.}...decor
-000014d0: 6174 6f72 7394 7d94 8c0e 636c 735f 636f  ators.}...cls_co
-000014e0: 6e73 7472 7563 7473 947d 9475 8c07 5f6c  nstructs.}.u.._l
-000014f0: 6f63 616c 7394 7d94 286a 1301 0000 7d94  ocals.}.(j....}.
-00001500: 6a15 0100 007d 946a 1701 0000 7d94 6a19  j....}.j....}.j.
-00001510: 0100 007d 946a 1b01 0000 7d94 6a1d 0100  ...}.j....}.j...
-00001520: 007d 946a 1f01 0000 7d94 6a21 0100 007d  .}.j....}.j!...}
-00001530: 946a 2301 0000 7d94 6a25 0100 007d 9475  .j#...}.j%...}.u
-00001540: 8c0d 5f70 6172 656e 745f 7363 6f70 6594  .._parent_scope.
-00001550: 4e8c 0c5f 736f 6e73 5f73 636f 7065 7394  N.._sons_scopes.
-00001560: 7d94 8c08 5f69 735f 6c6f 6f70 9489 8c06  }..._is_loop....
-00001570: 5f6c 6f6f 7073 945d 948c 145f 7465 6d70  _loops.]..._temp
-00001580: 6f72 6172 795f 7661 7269 6162 6c65 7394  orary_variables.
-00001590: 5d94 8c0d 5f75 7365 645f 7379 6d62 6f6c  ]..._used_symbol
-000015a0: 7394 7d94 6848 6845 8c08 6466 6674 7061  s.}.hHhE..dfftpa
-000015b0: 636b 9485 9481 944e 7d94 684a 8973 8694  ck.....N}.hJ.s..
-000015c0: 6273 8c0e 5f64 756d 6d79 5f63 6f75 6e74  bs.._dummy_count
-000015d0: 6572 944b 008c 105f 6f72 6967 696e 616c  er.K..._original
-000015e0: 5f73 796d 626f 6c94 7d94 6a3f 0100 0068  _symbol.}.j?...h
-000015f0: 4873 7586 9462 684c 5d94 6809 5d94 680d  Hsu..bhL].h.].h.
-00001600: 6168 4f89 6850 6851 7586 9462 8c09 5f66  ahO.hPhQu..b.._f
-00001610: 696c 656e 616d 6594 8c3b 2f55 7365 7273  ilename..;/Users
-00001620: 2f79 616d 616e 2f74 6d70 2f70 7963 6365  /yaman/tmp/pycce
-00001630: 6c2f 7079 6363 656c 2f73 7464 6c69 622f  l/pyccel/stdlib/
-00001640: 696e 7465 726e 616c 2f64 6666 7470 6163  internal/dfftpac
-00001650: 6b2e 7079 6894 8c09 5f6d 6574 6176 6172  k.pyh..._metavar
-00001660: 7394 7d94 288c 1069 676e 6f72 655f 6174  s.}.(..ignore_at
-00001670: 5f69 6d70 6f72 7494 888c 0e6d 6f64 756c  _import....modul
-00001680: 655f 7665 7273 696f 6e94 8c03 312e 3094  e_version...1.0.
-00001690: 8c04 7361 7665 9488 8c08 6578 7465 726e  ..save....extern
-000016a0: 616c 9488 756a 0c01 0000 6a10 0100 008c  al..uj....j.....
-000016b0: 0e5f 6375 7272 656e 745f 636c 6173 7394  ._current_class.
-000016c0: 4e8c 115f 6375 7272 656e 745f 6675 6e63  N.._current_func
-000016d0: 7469 6f6e 944e 8c0c 5f73 796e 7461 785f  tion.N.._syntax_
-000016e0: 646f 6e65 9488 8c0e 5f73 656d 616e 7469  done...._semanti
-000016f0: 635f 646f 6e65 9489 8c11 5f63 7572 7265  c_done...._curre
-00001700: 6e74 5f66 7374 5f6e 6f64 6594 4e8c 095f  nt_fst_node.N.._
-00001710: 626c 6f63 6b69 6e67 9489 8c14 5f63 7265  blocking...._cre
-00001720: 6174 6564 5f66 726f 6d5f 7069 636b 6c65  ated_from_pickle
-00001730: 9489 8c08 5f63 6f6e 7465 7874 945d 948c  ...._context.]..
-00001740: 0e5f 696e 5f6c 6873 5f61 7373 6967 6e94  ._in_lhs_assign.
-00001750: 8975 6287 942e                           .ub...
+000004f0: 6673 7494 8c04 5f61 7374 948c 064d 6f64  fst..._ast...Mod
+00000500: 756c 6594 9394 2952 947d 9428 8c04 626f  ule...)R.}.(..bo
+00000510: 6479 945d 9428 8c19 7079 6363 656c 2e70  dy.].(..pyccel.p
+00000520: 6172 7365 722e 6578 7465 6e64 5f74 7265  arser.extend_tre
+00000530: 6594 8c0b 436f 6d6d 656e 744c 696e 6594  e...CommentLine.
+00000540: 9394 8c1d 2320 7079 6363 656c 2068 6561  ....# pyccel hea
+00000550: 6465 7220 666f 7220 4446 5454 5041 434b  der for DFTTPACK
+00000560: 2e94 4b01 4b00 8794 5294 6811 8c10 436f  ..K.K...R.h...Co
+00000570: 6d6d 656e 744d 756c 7469 4c69 6e65 9493  mmentMultiLine..
+00000580: 948c 8a23 2420 6865 6164 6572 206d 6574  ...#$ header met
+00000590: 6176 6172 2069 676e 6f72 655f 6174 5f69  avar ignore_at_i
+000005a0: 6d70 6f72 743d 5472 7565 0a23 2420 6865  mport=True.#$ he
+000005b0: 6164 6572 206d 6574 6176 6172 206d 6f64  ader metavar mod
+000005c0: 756c 655f 7665 7273 696f 6e3d 2731 2e30  ule_version='1.0
+000005d0: 270a 2324 2068 6561 6465 7220 6d65 7461  '.#$ header meta
+000005e0: 7661 7220 7361 7665 3d54 7275 650a 2324  var save=True.#$
+000005f0: 2068 6561 6465 7220 6d65 7461 7661 7220   header metavar 
+00000600: 6578 7465 726e 616c 3d54 7275 6594 4b03  external=True.K.
+00000610: 4b00 8794 5294 6818 8c95 2324 2068 6561  K...R.h...#$ hea
+00000620: 6465 7220 6675 6e63 7469 6f6e 2064 6666  der function dff
+00000630: 7469 2869 6e74 2c20 646f 7562 6c65 205b  ti(int, double [
+00000640: 3a5d 290a 2324 2068 6561 6465 7220 6675  :]).#$ header fu
+00000650: 6e63 7469 6f6e 2064 6666 7466 2869 6e74  nction dfftf(int
+00000660: 2c20 646f 7562 6c65 205b 3a5d 2c20 646f  , double [:], do
+00000670: 7562 6c65 205b 3a5d 290a 2324 2068 6561  uble [:]).#$ hea
+00000680: 6465 7220 6675 6e63 7469 6f6e 2064 6666  der function dff
+00000690: 7462 2869 6e74 2c20 646f 7562 6c65 205b  tb(int, double [
+000006a0: 3a5d 2c20 646f 7562 6c65 205b 3a5d 2994  :], double [:]).
+000006b0: 4b0a 4b00 8794 5294 6818 8c98 2324 2068  K.K...R.h...#$ h
+000006c0: 6561 6465 7220 6675 6e63 7469 6f6e 2064  eader function d
+000006d0: 7a66 6674 6928 696e 742c 2064 6f75 626c  zffti(int, doubl
+000006e0: 6520 5b3a 5d29 0a23 2420 6865 6164 6572  e [:]).#$ header
+000006f0: 2066 756e 6374 696f 6e20 647a 6666 7466   function dzfftf
+00000700: 2869 6e74 2c20 646f 7562 6c65 205b 3a5d  (int, double [:]
+00000710: 2c20 646f 7562 6c65 205b 3a5d 290a 2324  , double [:]).#$
+00000720: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
+00000730: 2064 7a66 6674 6228 696e 742c 2064 6f75   dzfftb(int, dou
+00000740: 626c 6520 5b3a 5d2c 2064 6f75 626c 6520  ble [:], double 
+00000750: 5b3a 5d29 944b 0e4b 0087 9452 9468 188c  [:]).K.K...R.h..
+00000760: 9b23 2420 6865 6164 6572 2066 756e 6374  .#$ header funct
+00000770: 696f 6e20 6463 6f73 7169 2869 6e74 202c  ion dcosqi(int ,
+00000780: 2064 6f75 626c 6520 5b3a 5d29 0a23 2420   double [:]).#$ 
+00000790: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+000007a0: 6463 6f73 7166 2869 6e74 202c 2064 6f75  dcosqf(int , dou
+000007b0: 626c 6520 5b3a 5d2c 2064 6f75 626c 6520  ble [:], double 
+000007c0: 5b3a 5d29 0a23 2420 6865 6164 6572 2066  [:]).#$ header f
+000007d0: 756e 6374 696f 6e20 6463 6f73 7162 2869  unction dcosqb(i
+000007e0: 6e74 202c 2064 6f75 626c 6520 5b3a 5d2c  nt , double [:],
+000007f0: 2064 6f75 626c 6520 5b3a 5d29 944b 124b   double [:]).K.K
+00000800: 0087 9452 9468 188c 6323 2420 6865 6164  ...R.h..c#$ head
+00000810: 6572 2066 756e 6374 696f 6e20 6463 6f73  er function dcos
+00000820: 7469 2869 6e74 202c 2064 6f75 626c 6520  ti(int , double 
+00000830: 5b3a 5d29 0a23 2420 6865 6164 6572 2066  [:]).#$ header f
+00000840: 756e 6374 696f 6e20 6463 6f73 7420 2869  unction dcost (i
+00000850: 6e74 202c 2064 6f75 626c 6520 5b3a 5d2c  nt , double [:],
+00000860: 2064 6f75 626c 6520 5b3a 5d29 944b 164b   double [:]).K.K
+00000870: 0087 9452 9468 188c 9b23 2420 6865 6164  ...R.h...#$ head
+00000880: 6572 2066 756e 6374 696f 6e20 6473 696e  er function dsin
+00000890: 7169 2869 6e74 202c 2064 6f75 626c 6520  qi(int , double 
+000008a0: 5b3a 5d29 0a23 2420 6865 6164 6572 2066  [:]).#$ header f
+000008b0: 756e 6374 696f 6e20 6473 696e 7166 2869  unction dsinqf(i
+000008c0: 6e74 202c 2064 6f75 626c 6520 5b3a 5d2c  nt , double [:],
+000008d0: 2064 6f75 626c 6520 5b3a 5d29 0a23 2420   double [:]).#$ 
+000008e0: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+000008f0: 6473 696e 7162 2869 6e74 202c 2064 6f75  dsinqb(int , dou
+00000900: 626c 6520 5b3a 5d2c 2064 6f75 626c 6520  ble [:], double 
+00000910: 5b3a 5d29 944b 194b 0087 9452 9468 188c  [:]).K.K...R.h..
+00000920: 6123 2420 6865 6164 6572 2066 756e 6374  a#$ header funct
+00000930: 696f 6e20 6473 696e 7469 2869 6e74 2c20  ion dsinti(int, 
+00000940: 646f 7562 6c65 205b 3a5d 290a 2324 2068  double [:]).#$ h
+00000950: 6561 6465 7220 6675 6e63 7469 6f6e 2064  eader function d
+00000960: 7369 6e74 2028 696e 742c 2064 6f75 626c  sint (int, doubl
+00000970: 6520 5b3a 5d2c 2064 6f75 626c 6520 5b3a  e [:], double [:
+00000980: 5d29 944b 1d4b 0087 9452 9468 188c 9723  ]).K.K...R.h...#
+00000990: 2420 6865 6164 6572 2066 756e 6374 696f  $ header functio
+000009a0: 6e20 7a66 6674 6928 696e 742c 2064 6f75  n zffti(int, dou
+000009b0: 626c 6520 5b3a 5d29 0a23 2420 6865 6164  ble [:]).#$ head
+000009c0: 6572 2066 756e 6374 696f 6e20 7a66 6674  er function zfft
+000009d0: 6628 696e 742c 2063 6f6d 706c 6578 205b  f(int, complex [
+000009e0: 3a5d 2c20 646f 7562 6c65 205b 3a5d 290a  :], double [:]).
+000009f0: 2324 2068 6561 6465 7220 6675 6e63 7469  #$ header functi
+00000a00: 6f6e 207a 6666 7462 2869 6e74 2c20 636f  on zfftb(int, co
+00000a10: 6d70 6c65 7820 5b3a 5d2c 2064 6f75 626c  mplex [:], doubl
+00000a20: 6520 5b3a 5d29 944b 204b 0087 9452 9465  e [:]).K K...R.e
+00000a30: 8c0c 7479 7065 5f69 676e 6f72 6573 945d  ..type_ignores.]
+00000a40: 948c 066c 696e 656e 6f94 4b01 8c0a 636f  ...lineno.K...co
+00000a50: 6c5f 6f66 6673 6574 944b 0175 6268 0a8c  l_offset.K.ubh..
+00000a60: 0f70 7963 6365 6c2e 6173 742e 636f 7265  .pyccel.ast.core
+00000a70: 948c 064d 6f64 756c 6594 9394 2981 944e  ...Module...)..N
+00000a80: 7d94 288c 055f 6e61 6d65 9468 358c 0641  }.(.._name.h5..A
+00000a90: 734e 616d 6594 9394 2981 944e 7d94 288c  sName...)..N}.(.
+00000aa0: 045f 6f62 6a94 8c08 6466 6674 7061 636b  ._obj...dfftpack
+00000ab0: 948c 075f 7461 7267 6574 948c 1470 7963  ..._target...pyc
+00000ac0: 6365 6c2e 6173 742e 696e 7465 726e 616c  cel.ast.internal
+00000ad0: 7394 8c0c 5079 6363 656c 5379 6d62 6f6c  s...PyccelSymbol
+00000ae0: 9493 948c 0864 6666 7470 6163 6b94 8594  .....dfftpack...
+00000af0: 8194 4e7d 948c 085f 6973 5f74 656d 7094  ..N}..._is_temp.
+00000b00: 8973 8694 628c 0b5f 7573 6572 5f6e 6f64  .s..b.._user_nod
+00000b10: 6573 945d 9468 095d 948c 165f 7265 6375  es.].h.]..._recu
+00000b20: 7273 696f 6e5f 696e 5f70 726f 6772 6573  rsion_in_progres
+00000b30: 7394 898c 0f5f 7079 6363 656c 5f73 7461  s...._pyccel_sta
+00000b40: 6769 6e67 948c 0973 796e 7461 6374 6963  ging...syntactic
+00000b50: 9475 8694 628c 0a5f 7661 7269 6162 6c65  .u..b.._variable
+00000b60: 7394 298c 065f 6675 6e63 7394 298c 0b5f  s.).._funcs.).._
+00000b70: 696e 7465 7266 6163 6573 9429 8c08 5f63  interfaces.).._c
+00000b80: 6c61 7373 6573 9429 8c08 5f69 6d70 6f72  lasses.).._impor
+00000b90: 7473 9429 8c0a 5f69 6e69 745f 6675 6e63  ts.).._init_func
+00000ba0: 944e 8c0a 5f66 7265 655f 6675 6e63 944e  .N.._free_func.N
+00000bb0: 8c08 5f70 726f 6772 616d 9468 358c 0561  .._program.h5..a
+00000bc0: 7070 6c79 9493 9468 358c 0943 6f64 6542  pply...h5..CodeB
+00000bd0: 6c6f 636b 9493 9429 7d94 680f 2868 5b68  lock...)}.h.(h[h
+00000be0: 358c 0743 6f6d 6d65 6e74 9493 9429 7d94  5..Comment...)}.
+00000bf0: 8c04 7465 7874 948c 1b70 7963 6365 6c20  ..text...pyccel 
+00000c00: 6865 6164 6572 2066 6f72 2044 4654 5450  header for DFTTP
+00000c10: 4143 4b2e 9473 8794 5294 8c12 7079 6363  ACK..s..R...pycc
+00000c20: 656c 2e61 7374 2e68 6561 6465 7273 948c  el.ast.headers..
+00000c30: 0e46 756e 6374 696f 6e48 6561 6465 7294  .FunctionHeader.
+00000c40: 9394 288c 0564 6666 7469 945d 9428 7d94  ..(..dffti.].(}.
+00000c50: 288c 0864 6174 6174 7970 6594 8c14 7079  (..datatype...py
+00000c60: 6363 656c 2e61 7374 2e64 6174 6174 7970  ccel.ast.datatyp
+00000c70: 6573 948c 0d4e 6174 6976 6549 6e74 6567  es...NativeInteg
+00000c80: 6572 9493 9429 5294 8c04 7261 6e6b 944b  er...)R...rank.K
+00000c90: 008c 0f6d 656d 6f72 795f 6861 6e64 6c69  ...memory_handli
+00000ca0: 6e67 948c 0573 7461 636b 948c 0970 7265  ng...stack...pre
+00000cb0: 6369 7369 6f6e 944a ffff ffff 8c07 6973  cision.J......is
+00000cc0: 5f66 756e 6394 898c 0869 735f 636f 6e73  _func....is_cons
+00000cd0: 7494 8975 7d94 2868 6c68 6d8c 0b4e 6174  t..u}.(hlhm..Nat
+00000ce0: 6976 6546 6c6f 6174 9493 9429 5294 6871  iveFloat...)R.hq
+00000cf0: 4b01 6872 8c04 6865 6170 9468 744a ffff  K.hr..heap.htJ..
+00000d00: ffff 6875 8968 7689 7565 5d94 8974 9452  ..hu.hv.ue]..t.R
+00000d10: 9468 6828 8c05 6466 6674 6694 5d94 287d  .hh(..dfftf.].(}
+00000d20: 9428 686c 6870 6871 4b00 6872 6873 6874  .(hlhphqK.hrhsht
+00000d30: 4aff ffff ff68 7589 6876 8975 7d94 2868  J....hu.hv.u}.(h
+00000d40: 6c68 7a68 714b 0168 7268 7b68 744a ffff  lhzhqK.hrh{htJ..
+00000d50: ffff 6875 8968 7689 757d 9428 686c 687a  ..hu.hv.u}.(hlhz
+00000d60: 6871 4b01 6872 687b 6874 4aff ffff ff68  hqK.hrh{htJ....h
+00000d70: 7589 6876 8975 655d 9489 7494 5294 6868  u.hv.ue]..t.R.hh
+00000d80: 288c 0564 6666 7462 945d 9428 7d94 2868  (..dfftb.].(}.(h
+00000d90: 6c68 7068 714b 0068 7268 7368 744a ffff  lhphqK.hrhshtJ..
+00000da0: ffff 6875 8968 7689 757d 9428 686c 687a  ..hu.hv.u}.(hlhz
+00000db0: 6871 4b01 6872 687b 6874 4aff ffff ff68  hqK.hrh{htJ....h
+00000dc0: 7589 6876 8975 7d94 2868 6c68 7a68 714b  u.hv.u}.(hlhzhqK
+00000dd0: 0168 7268 7b68 744a ffff ffff 6875 8968  .hrh{htJ....hu.h
+00000de0: 7689 7565 5d94 8974 9452 9468 6828 8c06  v.ue]..t.R.hh(..
+00000df0: 647a 6666 7469 945d 9428 7d94 2868 6c68  dzffti.].(}.(hlh
+00000e00: 7068 714b 0068 7268 7368 744a ffff ffff  phqK.hrhshtJ....
+00000e10: 6875 8968 7689 757d 9428 686c 687a 6871  hu.hv.u}.(hlhzhq
+00000e20: 4b01 6872 687b 6874 4aff ffff ff68 7589  K.hrh{htJ....hu.
+00000e30: 6876 8975 655d 9489 7494 5294 6868 288c  hv.ue]..t.R.hh(.
+00000e40: 0664 7a66 6674 6694 5d94 287d 9428 686c  .dzfftf.].(}.(hl
+00000e50: 6870 6871 4b00 6872 6873 6874 4aff ffff  hphqK.hrhshtJ...
+00000e60: ff68 7589 6876 8975 7d94 2868 6c68 7a68  .hu.hv.u}.(hlhzh
+00000e70: 714b 0168 7268 7b68 744a ffff ffff 6875  qK.hrh{htJ....hu
+00000e80: 8968 7689 757d 9428 686c 687a 6871 4b01  .hv.u}.(hlhzhqK.
+00000e90: 6872 687b 6874 4aff ffff ff68 7589 6876  hrh{htJ....hu.hv
+00000ea0: 8975 655d 9489 7494 5294 6868 288c 0664  .ue]..t.R.hh(..d
+00000eb0: 7a66 6674 6294 5d94 287d 9428 686c 6870  zfftb.].(}.(hlhp
+00000ec0: 6871 4b00 6872 6873 6874 4aff ffff ff68  hqK.hrhshtJ....h
+00000ed0: 7589 6876 8975 7d94 2868 6c68 7a68 714b  u.hv.u}.(hlhzhqK
+00000ee0: 0168 7268 7b68 744a ffff ffff 6875 8968  .hrh{htJ....hu.h
+00000ef0: 7689 757d 9428 686c 687a 6871 4b01 6872  v.u}.(hlhzhqK.hr
+00000f00: 687b 6874 4aff ffff ff68 7589 6876 8975  h{htJ....hu.hv.u
+00000f10: 655d 9489 7494 5294 6868 288c 0664 636f  e]..t.R.hh(..dco
+00000f20: 7371 6994 5d94 287d 9428 686c 6870 6871  sqi.].(}.(hlhphq
+00000f30: 4b00 6872 6873 6874 4aff ffff ff68 7589  K.hrhshtJ....hu.
+00000f40: 6876 8975 7d94 2868 6c68 7a68 714b 0168  hv.u}.(hlhzhqK.h
+00000f50: 7268 7b68 744a ffff ffff 6875 8968 7689  rh{htJ....hu.hv.
+00000f60: 7565 5d94 8974 9452 9468 6828 8c06 6463  ue]..t.R.hh(..dc
+00000f70: 6f73 7166 945d 9428 7d94 2868 6c68 7068  osqf.].(}.(hlhph
+00000f80: 714b 0068 7268 7368 744a ffff ffff 6875  qK.hrhshtJ....hu
+00000f90: 8968 7689 757d 9428 686c 687a 6871 4b01  .hv.u}.(hlhzhqK.
+00000fa0: 6872 687b 6874 4aff ffff ff68 7589 6876  hrh{htJ....hu.hv
+00000fb0: 8975 7d94 2868 6c68 7a68 714b 0168 7268  .u}.(hlhzhqK.hrh
+00000fc0: 7b68 744a ffff ffff 6875 8968 7689 7565  {htJ....hu.hv.ue
+00000fd0: 5d94 8974 9452 9468 6828 8c06 6463 6f73  ]..t.R.hh(..dcos
+00000fe0: 7162 945d 9428 7d94 2868 6c68 7068 714b  qb.].(}.(hlhphqK
+00000ff0: 0068 7268 7368 744a ffff ffff 6875 8968  .hrhshtJ....hu.h
+00001000: 7689 757d 9428 686c 687a 6871 4b01 6872  v.u}.(hlhzhqK.hr
+00001010: 687b 6874 4aff ffff ff68 7589 6876 8975  h{htJ....hu.hv.u
+00001020: 7d94 2868 6c68 7a68 714b 0168 7268 7b68  }.(hlhzhqK.hrh{h
+00001030: 744a ffff ffff 6875 8968 7689 7565 5d94  tJ....hu.hv.ue].
+00001040: 8974 9452 9468 6828 8c06 6463 6f73 7469  .t.R.hh(..dcosti
+00001050: 945d 9428 7d94 2868 6c68 7068 714b 0068  .].(}.(hlhphqK.h
+00001060: 7268 7368 744a ffff ffff 6875 8968 7689  rhshtJ....hu.hv.
+00001070: 757d 9428 686c 687a 6871 4b01 6872 687b  u}.(hlhzhqK.hrh{
+00001080: 6874 4aff ffff ff68 7589 6876 8975 655d  htJ....hu.hv.ue]
+00001090: 9489 7494 5294 6868 288c 0564 636f 7374  ..t.R.hh(..dcost
+000010a0: 945d 9428 7d94 2868 6c68 7068 714b 0068  .].(}.(hlhphqK.h
+000010b0: 7268 7368 744a ffff ffff 6875 8968 7689  rhshtJ....hu.hv.
+000010c0: 757d 9428 686c 687a 6871 4b01 6872 687b  u}.(hlhzhqK.hrh{
+000010d0: 6874 4aff ffff ff68 7589 6876 8975 7d94  htJ....hu.hv.u}.
+000010e0: 2868 6c68 7a68 714b 0168 7268 7b68 744a  (hlhzhqK.hrh{htJ
+000010f0: ffff ffff 6875 8968 7689 7565 5d94 8974  ....hu.hv.ue]..t
+00001100: 9452 9468 6828 8c06 6473 696e 7169 945d  .R.hh(..dsinqi.]
+00001110: 9428 7d94 2868 6c68 7068 714b 0068 7268  .(}.(hlhphqK.hrh
+00001120: 7368 744a ffff ffff 6875 8968 7689 757d  shtJ....hu.hv.u}
+00001130: 9428 686c 687a 6871 4b01 6872 687b 6874  .(hlhzhqK.hrh{ht
+00001140: 4aff ffff ff68 7589 6876 8975 655d 9489  J....hu.hv.ue]..
+00001150: 7494 5294 6868 288c 0664 7369 6e71 6694  t.R.hh(..dsinqf.
+00001160: 5d94 287d 9428 686c 6870 6871 4b00 6872  ].(}.(hlhphqK.hr
+00001170: 6873 6874 4aff ffff ff68 7589 6876 8975  hshtJ....hu.hv.u
+00001180: 7d94 2868 6c68 7a68 714b 0168 7268 7b68  }.(hlhzhqK.hrh{h
+00001190: 744a ffff ffff 6875 8968 7689 757d 9428  tJ....hu.hv.u}.(
+000011a0: 686c 687a 6871 4b01 6872 687b 6874 4aff  hlhzhqK.hrh{htJ.
+000011b0: ffff ff68 7589 6876 8975 655d 9489 7494  ...hu.hv.ue]..t.
+000011c0: 5294 6868 288c 0664 7369 6e71 6294 5d94  R.hh(..dsinqb.].
+000011d0: 287d 9428 686c 6870 6871 4b00 6872 6873  (}.(hlhphqK.hrhs
+000011e0: 6874 4aff ffff ff68 7589 6876 8975 7d94  htJ....hu.hv.u}.
+000011f0: 2868 6c68 7a68 714b 0168 7268 7b68 744a  (hlhzhqK.hrh{htJ
+00001200: ffff ffff 6875 8968 7689 757d 9428 686c  ....hu.hv.u}.(hl
+00001210: 687a 6871 4b01 6872 687b 6874 4aff ffff  hzhqK.hrh{htJ...
+00001220: ff68 7589 6876 8975 655d 9489 7494 5294  .hu.hv.ue]..t.R.
+00001230: 6868 288c 0664 7369 6e74 6994 5d94 287d  hh(..dsinti.].(}
+00001240: 9428 686c 6870 6871 4b00 6872 6873 6874  .(hlhphqK.hrhsht
+00001250: 4aff ffff ff68 7589 6876 8975 7d94 2868  J....hu.hv.u}.(h
+00001260: 6c68 7a68 714b 0168 7268 7b68 744a ffff  lhzhqK.hrh{htJ..
+00001270: ffff 6875 8968 7689 7565 5d94 8974 9452  ..hu.hv.ue]..t.R
+00001280: 9468 6828 8c05 6473 696e 7494 5d94 287d  .hh(..dsint.].(}
+00001290: 9428 686c 6870 6871 4b00 6872 6873 6874  .(hlhphqK.hrhsht
+000012a0: 4aff ffff ff68 7589 6876 8975 7d94 2868  J....hu.hv.u}.(h
+000012b0: 6c68 7a68 714b 0168 7268 7b68 744a ffff  lhzhqK.hrh{htJ..
+000012c0: ffff 6875 8968 7689 757d 9428 686c 687a  ..hu.hv.u}.(hlhz
+000012d0: 6871 4b01 6872 687b 6874 4aff ffff ff68  hqK.hrh{htJ....h
+000012e0: 7589 6876 8975 655d 9489 7494 5294 6868  u.hv.ue]..t.R.hh
+000012f0: 288c 057a 6666 7469 945d 9428 7d94 2868  (..zffti.].(}.(h
+00001300: 6c68 7068 714b 0068 7268 7368 744a ffff  lhphqK.hrhshtJ..
+00001310: ffff 6875 8968 7689 757d 9428 686c 687a  ..hu.hv.u}.(hlhz
+00001320: 6871 4b01 6872 687b 6874 4aff ffff ff68  hqK.hrh{htJ....h
+00001330: 7589 6876 8975 655d 9489 7494 5294 6868  u.hv.ue]..t.R.hh
+00001340: 288c 057a 6666 7466 945d 9428 7d94 2868  (..zfftf.].(}.(h
+00001350: 6c68 7068 714b 0068 7268 7368 744a ffff  lhphqK.hrhshtJ..
+00001360: ffff 6875 8968 7689 757d 9428 686c 686d  ..hu.hv.u}.(hlhm
+00001370: 8c0d 4e61 7469 7665 436f 6d70 6c65 7894  ..NativeComplex.
+00001380: 9394 2952 9468 714b 0168 7268 7b68 744a  ..)R.hqK.hrh{htJ
+00001390: ffff ffff 6875 8968 7689 757d 9428 686c  ....hu.hv.u}.(hl
+000013a0: 687a 6871 4b01 6872 687b 6874 4aff ffff  hzhqK.hrh{htJ...
+000013b0: ff68 7589 6876 8975 655d 9489 7494 5294  .hu.hv.ue]..t.R.
+000013c0: 6868 288c 057a 6666 7462 945d 9428 7d94  hh(..zfftb.].(}.
+000013d0: 2868 6c68 7068 714b 0068 7268 7368 744a  (hlhphqK.hrhshtJ
+000013e0: ffff ffff 6875 8968 7689 757d 9428 686c  ....hu.hv.u}.(hl
+000013f0: 68ff 6871 4b01 6872 687b 6874 4aff ffff  h.hqK.hrh{htJ...
+00001400: ff68 7589 6876 8975 7d94 2868 6c68 7a68  .hu.hv.u}.(hlhzh
+00001410: 714b 0168 7268 7b68 744a ffff ffff 6875  qK.hrh{htJ....hu
+00001420: 8968 7689 7565 5d94 8974 9452 9474 9473  .hv.ue]..t.R.t.s
+00001430: 8794 5294 8c0f 5f76 6172 6961 626c 655f  ..R..._variable_
+00001440: 696e 6974 7394 298c 145f 696e 7465 726e  inits.).._intern
+00001450: 616c 5f64 6963 7469 6f6e 6172 7994 7d94  al_dictionary.}.
+00001460: 8c06 5f73 636f 7065 948c 1370 7963 6365  .._scope...pycce
+00001470: 6c2e 7061 7273 6572 2e73 636f 7065 948c  l.parser.scope..
+00001480: 0553 636f 7065 9493 9429 8194 4e7d 9428  .Scope...)..N}.(
+00001490: 6856 7d94 288c 0966 756e 6374 696f 6e73  hV}.(..functions
+000014a0: 947d 948c 0976 6172 6961 626c 6573 947d  .}...variables.}
+000014b0: 948c 0763 6c61 7373 6573 947d 948c 0769  ...classes.}...i
+000014c0: 6d70 6f72 7473 947d 948c 1273 796d 626f  mports.}...symbo
+000014d0: 6c69 635f 6675 6e63 7469 6f6e 7394 7d94  lic_functions.}.
+000014e0: 8c06 6d61 6372 6f73 947d 948c 0974 656d  ..macros.}...tem
+000014f0: 706c 6174 6573 947d 948c 0768 6561 6465  plates.}...heade
+00001500: 7273 947d 948c 0a64 6563 6f72 6174 6f72  rs.}...decorator
+00001510: 7394 7d94 8c0e 636c 735f 636f 6e73 7472  s.}...cls_constr
+00001520: 7563 7473 947d 9475 8c07 5f6c 6f63 616c  ucts.}.u.._local
+00001530: 7394 7d94 286a 1901 0000 7d94 6a1b 0100  s.}.(j....}.j...
+00001540: 007d 946a 1d01 0000 7d94 6a1f 0100 007d  .}.j....}.j....}
+00001550: 946a 2101 0000 7d94 6a23 0100 007d 946a  .j!...}.j#...}.j
+00001560: 2501 0000 7d94 6a27 0100 007d 946a 2901  %...}.j'...}.j).
+00001570: 0000 7d94 6a2b 0100 007d 9475 8c0d 5f70  ..}.j+...}.u.._p
+00001580: 6172 656e 745f 7363 6f70 6594 4e8c 0c5f  arent_scope.N.._
+00001590: 736f 6e73 5f73 636f 7065 7394 7d94 8c08  sons_scopes.}...
+000015a0: 5f69 735f 6c6f 6f70 9489 8c06 5f6c 6f6f  _is_loop...._loo
+000015b0: 7073 945d 948c 145f 7465 6d70 6f72 6172  ps.]..._temporar
+000015c0: 795f 7661 7269 6162 6c65 7394 5d94 8c0d  y_variables.]...
+000015d0: 5f75 7365 645f 7379 6d62 6f6c 7394 7d94  _used_symbols.}.
+000015e0: 6847 6844 8c08 6466 6674 7061 636b 9485  hGhD..dfftpack..
+000015f0: 9481 944e 7d94 6849 8973 8694 6273 8c0e  ...N}.hI.s..bs..
+00001600: 5f64 756d 6d79 5f63 6f75 6e74 6572 944b  _dummy_counter.K
+00001610: 008c 105f 6f72 6967 696e 616c 5f73 796d  ..._original_sym
+00001620: 626f 6c94 7d94 6a45 0100 0068 4773 7586  bol.}.jE...hGsu.
+00001630: 9462 684b 5d94 6809 5d94 680d 6168 4e89  .bhK].h.].h.ahN.
+00001640: 684f 6850 7586 9462 8c09 5f66 696c 656e  hOhPu..b.._filen
+00001650: 616d 6594 8c3d 2f68 6f6d 652f 7961 6d61  ame..=/home/yama
+00001660: 6e67 7563 2f74 6d70 2f70 7963 6365 6c2f  nguc/tmp/pyccel/
+00001670: 7079 6363 656c 2f73 7464 6c69 622f 696e  pyccel/stdlib/in
+00001680: 7465 726e 616c 2f64 6666 7470 6163 6b2e  ternal/dfftpack.
+00001690: 7079 6894 8c09 5f6d 6574 6176 6172 7394  pyh..._metavars.
+000016a0: 7d94 288c 1069 676e 6f72 655f 6174 5f69  }.(..ignore_at_i
+000016b0: 6d70 6f72 7494 888c 0e6d 6f64 756c 655f  mport....module_
+000016c0: 7665 7273 696f 6e94 8c03 312e 3094 8c04  version...1.0...
+000016d0: 7361 7665 9488 8c08 6578 7465 726e 616c  save....external
+000016e0: 9488 756a 1201 0000 6a16 0100 008c 0e5f  ..uj....j......_
+000016f0: 6375 7272 656e 745f 636c 6173 7394 4e8c  current_class.N.
+00001700: 115f 6375 7272 656e 745f 6675 6e63 7469  ._current_functi
+00001710: 6f6e 944e 8c0c 5f73 796e 7461 785f 646f  on.N.._syntax_do
+00001720: 6e65 9488 8c0e 5f73 656d 616e 7469 635f  ne...._semantic_
+00001730: 646f 6e65 9489 8c11 5f63 7572 7265 6e74  done...._current
+00001740: 5f66 7374 5f6e 6f64 6594 4e8c 095f 626c  _fst_node.N.._bl
+00001750: 6f63 6b69 6e67 9489 8c14 5f63 7265 6174  ocking...._creat
+00001760: 6564 5f66 726f 6d5f 7069 636b 6c65 9489  ed_from_pickle..
+00001770: 8c08 5f63 6f6e 7465 7874 945d 948c 0e5f  .._context.]..._
+00001780: 696e 5f6c 6873 5f61 7373 6967 6e94 8975  in_lhs_assign..u
+00001790: 6287 942e                                b...
```

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/dfftpack.pyh` & `pyccel-1.9.2/pyccel/stdlib/internal/dfftpack.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/fftw.pyh` & `pyccel-1.9.2/pyccel/stdlib/internal/fftw.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/fitpack.pyccel` & `pyccel-1.9.2/pyccel/stdlib/internal/fitpack.pyccel`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-00000000: 8004 954a 0b00 0000 0000 008c 2062 6362  ...J........ bcb
+00000000: 8004 957b 0b00 0000 0000 008c 2062 6362  ...{........ bcb
 00000010: 3932 6461 3730 6233 3364 3836 3939 3234  92da70b33d869924
 00000020: 6537 3333 3034 3531 3564 3365 3494 8c05  e73304515d3e4...
-00000030: 312e 392e 3194 8c17 7079 6363 656c 2e70  1.9.1...pyccel.p
+00000030: 312e 392e 3294 8c17 7079 6363 656c 2e70  1.9.2...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 5701 0000 2320 7079 6363 656c 2068 6561  W...# pyccel hea
 00000080: 6465 7220 666f 7220 4649 5450 4143 4b2e  der for FITPACK.
 00000090: 0a0a 0a23 2420 6865 6164 6572 206d 6574  ...#$ header met
 000000a0: 6176 6172 2069 676e 6f72 655f 6174 5f69  avar ignore_at_i
@@ -23,160 +23,163 @@
 00000160: 2c20 696e 742c 2064 6f75 626c 655b 3a5d  , int, double[:]
 00000170: 2c20 696e 742c 2069 6e74 2c20 646f 7562  , int, int, doub
 00000180: 6c65 5b3a 5d2c 2069 6e74 2c20 646f 7562  le[:], int, doub
 00000190: 6c65 5b3a 5d2c 2069 6e74 2c20 646f 7562  le[:], int, doub
 000001a0: 6c65 5b3a 5d2c 2064 6f75 626c 655b 3a5d  le[:], double[:]
 000001b0: 2c20 696e 742c 2069 6e74 5b3a 5d2c 2069  , int, int[:], i
 000001c0: 6e74 202c 2069 6e74 290a 0a94 8c04 5f66  nt , int)....._f
-000001d0: 7374 948c 0361 7374 948c 064d 6f64 756c  st...ast...Modul
-000001e0: 6594 9394 2952 947d 9428 8c04 626f 6479  e...)R.}.(..body
-000001f0: 945d 9428 8c19 7079 6363 656c 2e70 6172  .].(..pyccel.par
-00000200: 7365 722e 6578 7465 6e64 5f74 7265 6594  ser.extend_tree.
-00000210: 8c0b 436f 6d6d 656e 744c 696e 6594 9394  ..CommentLine...
-00000220: 8c1c 2320 7079 6363 656c 2068 6561 6465  ..# pyccel heade
-00000230: 7220 666f 7220 4649 5450 4143 4b2e 944b  r for FITPACK..K
-00000240: 014b 0087 9452 9468 118c 1043 6f6d 6d65  .K...R.h...Comme
-00000250: 6e74 4d75 6c74 694c 696e 6594 9394 8c96  ntMultiLine.....
-00000260: 2324 2068 6561 6465 7220 6d65 7461 7661  #$ header metava
-00000270: 7220 6967 6e6f 7265 5f61 745f 696d 706f  r ignore_at_impo
-00000280: 7274 3d54 7275 650a 2324 2068 6561 6465  rt=True.#$ heade
-00000290: 7220 6d65 7461 7661 7220 6c69 6272 6172  r metavar librar
-000002a0: 6965 733d 2724 7b46 4954 5041 434b 5f4c  ies='${FITPACK_L
-000002b0: 4942 5241 5249 4553 7d27 0a23 2420 6865  IBRARIES}'.#$ he
-000002c0: 6164 6572 206d 6574 6176 6172 2073 6176  ader metavar sav
-000002d0: 653d 5472 7565 0a23 2420 6865 6164 6572  e=True.#$ header
-000002e0: 206d 6574 6176 6172 2065 7874 6572 6e61   metavar externa
-000002f0: 6c3d 5472 7565 944b 044b 0087 9452 9468  l=True.K.K...R.h
-00000300: 138c 9d23 2420 6865 6164 6572 2066 756e  ...#$ header fun
-00000310: 6374 696f 6e20 6269 7370 6576 2864 6f75  ction bispev(dou
-00000320: 626c 655b 3a5d 202c 2069 6e74 2c20 646f  ble[:] , int, do
-00000330: 7562 6c65 5b3a 5d2c 2069 6e74 2c20 646f  uble[:], int, do
-00000340: 7562 6c65 5b3a 5d2c 2069 6e74 2c20 696e  uble[:], int, in
-00000350: 742c 2064 6f75 626c 655b 3a5d 2c20 696e  t, double[:], in
-00000360: 742c 2064 6f75 626c 655b 3a5d 2c20 696e  t, double[:], in
-00000370: 742c 2064 6f75 626c 655b 3a5d 2c20 646f  t, double[:], do
-00000380: 7562 6c65 5b3a 5d2c 2069 6e74 2c20 696e  uble[:], int, in
-00000390: 745b 3a5d 2c20 696e 7420 2c20 696e 7429  t[:], int , int)
-000003a0: 944b 0a4b 0087 9452 9465 8c0c 7479 7065  .K.K...R.e..type
-000003b0: 5f69 676e 6f72 6573 945d 948c 066c 696e  _ignores.]...lin
-000003c0: 656e 6f94 4b01 8c0a 636f 6c5f 6f66 6673  eno.K...col_offs
-000003d0: 6574 944b 0175 628c 045f 6173 7494 8c0f  et.K.ub.._ast...
-000003e0: 7079 6363 656c 2e61 7374 2e63 6f72 6594  pyccel.ast.core.
-000003f0: 8c06 4d6f 6475 6c65 9493 9429 8194 4e7d  ..Module...)..N}
-00000400: 9428 8c05 5f6e 616d 6594 6824 8c06 4173  .(.._name.h$..As
-00000410: 4e61 6d65 9493 9429 8194 4e7d 9428 8c04  Name...)..N}.(..
-00000420: 5f6f 626a 948c 0766 6974 7061 636b 948c  _obj...fitpack..
-00000430: 075f 7461 7267 6574 948c 1470 7963 6365  ._target...pycce
-00000440: 6c2e 6173 742e 696e 7465 726e 616c 7394  l.ast.internals.
-00000450: 8c0c 5079 6363 656c 5379 6d62 6f6c 9493  ..PyccelSymbol..
-00000460: 948c 0766 6974 7061 636b 9485 9481 944e  ...fitpack.....N
-00000470: 7d94 8c08 5f69 735f 7465 6d70 9489 7386  }..._is_temp..s.
-00000480: 9462 8c0b 5f75 7365 725f 6e6f 6465 7394  .b.._user_nodes.
-00000490: 5d94 6809 5d94 8c16 5f72 6563 7572 7369  ].h.]..._recursi
-000004a0: 6f6e 5f69 6e5f 7072 6f67 7265 7373 9489  on_in_progress..
-000004b0: 8c0f 5f70 7963 6365 6c5f 7374 6167 696e  .._pyccel_stagin
-000004c0: 6794 8c09 7379 6e74 6163 7469 6394 7586  g...syntactic.u.
-000004d0: 9462 8c0a 5f76 6172 6961 626c 6573 9429  .b.._variables.)
-000004e0: 8c06 5f66 756e 6373 9429 8c0b 5f69 6e74  .._funcs.).._int
-000004f0: 6572 6661 6365 7394 298c 085f 636c 6173  erfaces.).._clas
-00000500: 7365 7394 298c 085f 696d 706f 7274 7394  ses.).._imports.
-00000510: 298c 0a5f 696e 6974 5f66 756e 6394 4e8c  ).._init_func.N.
-00000520: 0a5f 6672 6565 5f66 756e 6394 4e8c 085f  ._free_func.N.._
-00000530: 7072 6f67 7261 6d94 6824 8c05 6170 706c  program.h$..appl
-00000540: 7994 9394 6824 8c09 436f 6465 426c 6f63  y...h$..CodeBloc
-00000550: 6b94 9394 297d 9468 0f68 4a68 248c 0743  k...)}.h.hJh$..C
-00000560: 6f6d 6d65 6e74 9493 9429 7d94 8c04 7465  omment...)}...te
-00000570: 7874 948c 1a70 7963 6365 6c20 6865 6164  xt...pyccel head
-00000580: 6572 2066 6f72 2046 4954 5041 434b 2e94  er for FITPACK..
-00000590: 7387 9452 948c 1270 7963 6365 6c2e 6173  s..R...pyccel.as
-000005a0: 742e 6865 6164 6572 7394 8c0e 4675 6e63  t.headers...Func
-000005b0: 7469 6f6e 4865 6164 6572 9493 9428 8c06  tionHeader...(..
-000005c0: 6269 7370 6576 945d 9428 7d94 288c 0864  bispev.].(}.(..d
-000005d0: 6174 6174 7970 6594 8c05 666c 6f61 7494  atatype...float.
-000005e0: 8c04 7261 6e6b 944b 018c 0f6d 656d 6f72  ..rank.K...memor
-000005f0: 795f 6861 6e64 6c69 6e67 948c 0468 6561  y_handling...hea
-00000600: 7094 8c09 7072 6563 6973 696f 6e94 4aff  p...precision.J.
-00000610: ffff ff8c 0769 735f 6675 6e63 9489 8c08  .....is_func....
-00000620: 6973 5f63 6f6e 7374 9489 757d 9428 685b  is_const..u}.(h[
-00000630: 8c03 696e 7494 685d 4b00 685e 8c05 7374  ..int.h]K.h^..st
-00000640: 6163 6b94 6860 4aff ffff ff68 6189 6862  ack.h`J....ha.hb
-00000650: 8975 7d94 2868 5b68 5c68 5d4b 0168 5e68  .u}.(h[h\h]K.h^h
-00000660: 5f68 604a ffff ffff 6861 8968 6289 757d  _h`J....ha.hb.u}
-00000670: 9428 685b 6864 685d 4b00 685e 6865 6860  .(h[hdh]K.h^heh`
-00000680: 4aff ffff ff68 6189 6862 8975 7d94 2868  J....ha.hb.u}.(h
-00000690: 5b68 5c68 5d4b 0168 5e68 5f68 604a ffff  [h\h]K.h^h_h`J..
-000006a0: ffff 6861 8968 6289 757d 9428 685b 6864  ..ha.hb.u}.(h[hd
-000006b0: 685d 4b00 685e 6865 6860 4aff ffff ff68  h]K.h^heh`J....h
-000006c0: 6189 6862 8975 7d94 2868 5b68 6468 5d4b  a.hb.u}.(h[hdh]K
-000006d0: 0068 5e68 6568 604a ffff ffff 6861 8968  .h^heh`J....ha.h
-000006e0: 6289 757d 9428 685b 685c 685d 4b01 685e  b.u}.(h[h\h]K.h^
-000006f0: 685f 6860 4aff ffff ff68 6189 6862 8975  h_h`J....ha.hb.u
-00000700: 7d94 2868 5b68 6468 5d4b 0068 5e68 6568  }.(h[hdh]K.h^heh
-00000710: 604a ffff ffff 6861 8968 6289 757d 9428  `J....ha.hb.u}.(
-00000720: 685b 685c 685d 4b01 685e 685f 6860 4aff  h[h\h]K.h^h_h`J.
-00000730: ffff ff68 6189 6862 8975 7d94 2868 5b68  ...ha.hb.u}.(h[h
-00000740: 6468 5d4b 0068 5e68 6568 604a ffff ffff  dh]K.h^heh`J....
-00000750: 6861 8968 6289 757d 9428 685b 685c 685d  ha.hb.u}.(h[h\h]
-00000760: 4b01 685e 685f 6860 4aff ffff ff68 6189  K.h^h_h`J....ha.
-00000770: 6862 8975 7d94 2868 5b68 5c68 5d4b 0168  hb.u}.(h[h\h]K.h
-00000780: 5e68 5f68 604a ffff ffff 6861 8968 6289  ^h_h`J....ha.hb.
-00000790: 757d 9428 685b 6864 685d 4b00 685e 6865  u}.(h[hdh]K.h^he
-000007a0: 6860 4aff ffff ff68 6189 6862 8975 7d94  h`J....ha.hb.u}.
-000007b0: 2868 5b68 6468 5d4b 0168 5e68 5f68 604a  (h[hdh]K.h^h_h`J
-000007c0: ffff ffff 6861 8968 6289 757d 9428 685b  ....ha.hb.u}.(h[
-000007d0: 6864 685d 4b00 685e 6865 6860 4aff ffff  hdh]K.h^heh`J...
-000007e0: ff68 6189 6862 8975 7d94 2868 5b68 6468  .ha.hb.u}.(h[hdh
-000007f0: 5d4b 0068 5e68 6568 604a ffff ffff 6861  ]K.h^heh`J....ha
-00000800: 8968 6289 7565 5d94 8974 9452 9486 9473  .hb.ue]..t.R...s
-00000810: 8794 5294 8c0f 5f76 6172 6961 626c 655f  ..R..._variable_
-00000820: 696e 6974 7394 298c 145f 696e 7465 726e  inits.).._intern
-00000830: 616c 5f64 6963 7469 6f6e 6172 7994 7d94  al_dictionary.}.
-00000840: 8c06 5f73 636f 7065 948c 1370 7963 6365  .._scope...pycce
-00000850: 6c2e 7061 7273 6572 2e73 636f 7065 948c  l.parser.scope..
-00000860: 0553 636f 7065 9493 9429 8194 4e7d 9428  .Scope...)..N}.(
-00000870: 6845 7d94 288c 0966 756e 6374 696f 6e73  hE}.(..functions
-00000880: 947d 948c 0976 6172 6961 626c 6573 947d  .}...variables.}
-00000890: 948c 0763 6c61 7373 6573 947d 948c 0769  ...classes.}...i
-000008a0: 6d70 6f72 7473 947d 948c 1273 796d 626f  mports.}...symbo
-000008b0: 6c69 635f 6675 6e63 7469 6f6e 7394 7d94  lic_functions.}.
-000008c0: 8c06 6d61 6372 6f73 947d 948c 0974 656d  ..macros.}...tem
-000008d0: 706c 6174 6573 947d 948c 0768 6561 6465  plates.}...heade
-000008e0: 7273 947d 948c 0a64 6563 6f72 6174 6f72  rs.}...decorator
-000008f0: 7394 7d94 8c0e 636c 735f 636f 6e73 7472  s.}...cls_constr
-00000900: 7563 7473 947d 9475 8c07 5f6c 6f63 616c  ucts.}.u.._local
-00000910: 7394 7d94 2868 857d 9468 877d 9468 897d  s.}.(h.}.h.}.h.}
-00000920: 9468 8b7d 9468 8d7d 9468 8f7d 9468 917d  .h.}.h.}.h.}.h.}
-00000930: 9468 937d 9468 957d 9468 977d 9475 8c0d  .h.}.h.}.h.}.u..
-00000940: 5f70 6172 656e 745f 7363 6f70 6594 4e8c  _parent_scope.N.
-00000950: 0c5f 736f 6e73 5f73 636f 7065 7394 7d94  ._sons_scopes.}.
-00000960: 8c08 5f69 735f 6c6f 6f70 9489 8c06 5f6c  .._is_loop...._l
-00000970: 6f6f 7073 945d 948c 145f 7465 6d70 6f72  oops.]..._tempor
-00000980: 6172 795f 7661 7269 6162 6c65 7394 5d94  ary_variables.].
-00000990: 8c0d 5f75 7365 645f 7379 6d62 6f6c 7394  .._used_symbols.
-000009a0: 7d94 6836 6833 8c07 6669 7470 6163 6b94  }.h6h3..fitpack.
-000009b0: 8594 8194 4e7d 9468 3889 7386 9462 738c  ....N}.h8.s..bs.
-000009c0: 0e5f 6475 6d6d 795f 636f 756e 7465 7294  ._dummy_counter.
-000009d0: 4b00 8c10 5f6f 7269 6769 6e61 6c5f 7379  K..._original_sy
-000009e0: 6d62 6f6c 947d 9468 b168 3673 7586 9462  mbol.}.h.h6su..b
-000009f0: 683a 5d94 6809 5d94 680d 6168 3d89 683e  h:].h.].h.ah=.h>
-00000a00: 683f 7586 9462 8c09 5f66 696c 656e 616d  h?u..b.._filenam
-00000a10: 6594 8c3a 2f55 7365 7273 2f79 616d 616e  e..:/Users/yaman
-00000a20: 2f74 6d70 2f70 7963 6365 6c2f 7079 6363  /tmp/pyccel/pycc
-00000a30: 656c 2f73 7464 6c69 622f 696e 7465 726e  el/stdlib/intern
-00000a40: 616c 2f66 6974 7061 636b 2e70 7968 948c  al/fitpack.pyh..
-00000a50: 095f 6d65 7461 7661 7273 947d 9428 8c10  ._metavars.}.(..
-00000a60: 6967 6e6f 7265 5f61 745f 696d 706f 7274  ignore_at_import
-00000a70: 9488 8c09 6c69 6272 6172 6965 7394 8c14  ....libraries...
-00000a80: 247b 4649 5450 4143 4b5f 4c49 4252 4152  ${FITPACK_LIBRAR
-00000a90: 4945 537d 948c 0473 6176 6594 888c 0865  IES}...save....e
-00000aa0: 7874 6572 6e61 6c94 8875 687e 6882 8c0e  xternal..uh~h...
-00000ab0: 5f63 7572 7265 6e74 5f63 6c61 7373 944e  _current_class.N
-00000ac0: 8c11 5f63 7572 7265 6e74 5f66 756e 6374  .._current_funct
-00000ad0: 696f 6e94 4e8c 0c5f 7379 6e74 6178 5f64  ion.N.._syntax_d
-00000ae0: 6f6e 6594 888c 0e5f 7365 6d61 6e74 6963  one...._semantic
-00000af0: 5f64 6f6e 6594 898c 115f 6375 7272 656e  _done...._curren
-00000b00: 745f 6673 745f 6e6f 6465 944e 8c09 5f62  t_fst_node.N.._b
-00000b10: 6c6f 636b 696e 6794 898c 145f 6372 6561  locking...._crea
-00000b20: 7465 645f 6672 6f6d 5f70 6963 6b6c 6594  ted_from_pickle.
-00000b30: 898c 085f 636f 6e74 6578 7494 5d94 8c0e  ..._context.]...
-00000b40: 5f69 6e5f 6c68 735f 6173 7369 676e 9489  _in_lhs_assign..
-00000b50: 7562 8794 2e                             ub...
+000001d0: 7374 948c 045f 6173 7494 8c06 4d6f 6475  st..._ast...Modu
+000001e0: 6c65 9493 9429 5294 7d94 288c 0462 6f64  le...)R.}.(..bod
+000001f0: 7994 5d94 288c 1970 7963 6365 6c2e 7061  y.].(..pyccel.pa
+00000200: 7273 6572 2e65 7874 656e 645f 7472 6565  rser.extend_tree
+00000210: 948c 0b43 6f6d 6d65 6e74 4c69 6e65 9493  ...CommentLine..
+00000220: 948c 1c23 2070 7963 6365 6c20 6865 6164  ...# pyccel head
+00000230: 6572 2066 6f72 2046 4954 5041 434b 2e94  er for FITPACK..
+00000240: 4b01 4b00 8794 5294 6811 8c10 436f 6d6d  K.K...R.h...Comm
+00000250: 656e 744d 756c 7469 4c69 6e65 9493 948c  entMultiLine....
+00000260: 9623 2420 6865 6164 6572 206d 6574 6176  .#$ header metav
+00000270: 6172 2069 676e 6f72 655f 6174 5f69 6d70  ar ignore_at_imp
+00000280: 6f72 743d 5472 7565 0a23 2420 6865 6164  ort=True.#$ head
+00000290: 6572 206d 6574 6176 6172 206c 6962 7261  er metavar libra
+000002a0: 7269 6573 3d27 247b 4649 5450 4143 4b5f  ries='${FITPACK_
+000002b0: 4c49 4252 4152 4945 537d 270a 2324 2068  LIBRARIES}'.#$ h
+000002c0: 6561 6465 7220 6d65 7461 7661 7220 7361  eader metavar sa
+000002d0: 7665 3d54 7275 650a 2324 2068 6561 6465  ve=True.#$ heade
+000002e0: 7220 6d65 7461 7661 7220 6578 7465 726e  r metavar extern
+000002f0: 616c 3d54 7275 6594 4b04 4b00 8794 5294  al=True.K.K...R.
+00000300: 6813 8c9d 2324 2068 6561 6465 7220 6675  h...#$ header fu
+00000310: 6e63 7469 6f6e 2062 6973 7065 7628 646f  nction bispev(do
+00000320: 7562 6c65 5b3a 5d20 2c20 696e 742c 2064  uble[:] , int, d
+00000330: 6f75 626c 655b 3a5d 2c20 696e 742c 2064  ouble[:], int, d
+00000340: 6f75 626c 655b 3a5d 2c20 696e 742c 2069  ouble[:], int, i
+00000350: 6e74 2c20 646f 7562 6c65 5b3a 5d2c 2069  nt, double[:], i
+00000360: 6e74 2c20 646f 7562 6c65 5b3a 5d2c 2069  nt, double[:], i
+00000370: 6e74 2c20 646f 7562 6c65 5b3a 5d2c 2064  nt, double[:], d
+00000380: 6f75 626c 655b 3a5d 2c20 696e 742c 2069  ouble[:], int, i
+00000390: 6e74 5b3a 5d2c 2069 6e74 202c 2069 6e74  nt[:], int , int
+000003a0: 2994 4b0a 4b00 8794 5294 658c 0c74 7970  ).K.K...R.e..typ
+000003b0: 655f 6967 6e6f 7265 7394 5d94 8c06 6c69  e_ignores.]...li
+000003c0: 6e65 6e6f 944b 018c 0a63 6f6c 5f6f 6666  neno.K...col_off
+000003d0: 7365 7494 4b01 7562 680a 8c0f 7079 6363  set.K.ubh...pycc
+000003e0: 656c 2e61 7374 2e63 6f72 6594 8c06 4d6f  el.ast.core...Mo
+000003f0: 6475 6c65 9493 9429 8194 4e7d 9428 8c05  dule...)..N}.(..
+00000400: 5f6e 616d 6594 6823 8c06 4173 4e61 6d65  _name.h#..AsName
+00000410: 9493 9429 8194 4e7d 9428 8c04 5f6f 626a  ...)..N}.(.._obj
+00000420: 948c 0766 6974 7061 636b 948c 075f 7461  ...fitpack..._ta
+00000430: 7267 6574 948c 1470 7963 6365 6c2e 6173  rget...pyccel.as
+00000440: 742e 696e 7465 726e 616c 7394 8c0c 5079  t.internals...Py
+00000450: 6363 656c 5379 6d62 6f6c 9493 948c 0766  ccelSymbol.....f
+00000460: 6974 7061 636b 9485 9481 944e 7d94 8c08  itpack.....N}...
+00000470: 5f69 735f 7465 6d70 9489 7386 9462 8c0b  _is_temp..s..b..
+00000480: 5f75 7365 725f 6e6f 6465 7394 5d94 6809  _user_nodes.].h.
+00000490: 5d94 8c16 5f72 6563 7572 7369 6f6e 5f69  ]..._recursion_i
+000004a0: 6e5f 7072 6f67 7265 7373 9489 8c0f 5f70  n_progress...._p
+000004b0: 7963 6365 6c5f 7374 6167 696e 6794 8c09  yccel_staging...
+000004c0: 7379 6e74 6163 7469 6394 7586 9462 8c0a  syntactic.u..b..
+000004d0: 5f76 6172 6961 626c 6573 9429 8c06 5f66  _variables.).._f
+000004e0: 756e 6373 9429 8c0b 5f69 6e74 6572 6661  uncs.).._interfa
+000004f0: 6365 7394 298c 085f 636c 6173 7365 7394  ces.).._classes.
+00000500: 298c 085f 696d 706f 7274 7394 298c 0a5f  ).._imports.).._
+00000510: 696e 6974 5f66 756e 6394 4e8c 0a5f 6672  init_func.N.._fr
+00000520: 6565 5f66 756e 6394 4e8c 085f 7072 6f67  ee_func.N.._prog
+00000530: 7261 6d94 6823 8c05 6170 706c 7994 9394  ram.h#..apply...
+00000540: 6823 8c09 436f 6465 426c 6f63 6b94 9394  h#..CodeBlock...
+00000550: 297d 9468 0f68 4968 238c 0743 6f6d 6d65  )}.h.hIh#..Comme
+00000560: 6e74 9493 9429 7d94 8c04 7465 7874 948c  nt...)}...text..
+00000570: 1a70 7963 6365 6c20 6865 6164 6572 2066  .pyccel header f
+00000580: 6f72 2046 4954 5041 434b 2e94 7387 9452  or FITPACK..s..R
+00000590: 948c 1270 7963 6365 6c2e 6173 742e 6865  ...pyccel.ast.he
+000005a0: 6164 6572 7394 8c0e 4675 6e63 7469 6f6e  aders...Function
+000005b0: 4865 6164 6572 9493 9428 8c06 6269 7370  Header...(..bisp
+000005c0: 6576 945d 9428 7d94 288c 0864 6174 6174  ev.].(}.(..datat
+000005d0: 7970 6594 8c14 7079 6363 656c 2e61 7374  ype...pyccel.ast
+000005e0: 2e64 6174 6174 7970 6573 948c 0b4e 6174  .datatypes...Nat
+000005f0: 6976 6546 6c6f 6174 9493 9429 5294 8c04  iveFloat...)R...
+00000600: 7261 6e6b 944b 018c 0f6d 656d 6f72 795f  rank.K...memory_
+00000610: 6861 6e64 6c69 6e67 948c 0468 6561 7094  handling...heap.
+00000620: 8c09 7072 6563 6973 696f 6e94 4aff ffff  ..precision.J...
+00000630: ff8c 0769 735f 6675 6e63 9489 8c08 6973  ...is_func....is
+00000640: 5f63 6f6e 7374 9489 757d 9428 685a 685b  _const..u}.(hZh[
+00000650: 8c0d 4e61 7469 7665 496e 7465 6765 7294  ..NativeInteger.
+00000660: 9394 2952 9468 5f4b 0068 608c 0573 7461  ..)R.h_K.h`..sta
+00000670: 636b 9468 624a ffff ffff 6863 8968 6489  ck.hbJ....hc.hd.
+00000680: 757d 9428 685a 685e 685f 4b01 6860 6861  u}.(hZh^h_K.h`ha
+00000690: 6862 4aff ffff ff68 6389 6864 8975 7d94  hbJ....hc.hd.u}.
+000006a0: 2868 5a68 6868 5f4b 0068 6068 6968 624a  (hZhhh_K.h`hihbJ
+000006b0: ffff ffff 6863 8968 6489 757d 9428 685a  ....hc.hd.u}.(hZ
+000006c0: 685e 685f 4b01 6860 6861 6862 4aff ffff  h^h_K.h`hahbJ...
+000006d0: ff68 6389 6864 8975 7d94 2868 5a68 6868  .hc.hd.u}.(hZhhh
+000006e0: 5f4b 0068 6068 6968 624a ffff ffff 6863  _K.h`hihbJ....hc
+000006f0: 8968 6489 757d 9428 685a 6868 685f 4b00  .hd.u}.(hZhhh_K.
+00000700: 6860 6869 6862 4aff ffff ff68 6389 6864  h`hihbJ....hc.hd
+00000710: 8975 7d94 2868 5a68 5e68 5f4b 0168 6068  .u}.(hZh^h_K.h`h
+00000720: 6168 624a ffff ffff 6863 8968 6489 757d  ahbJ....hc.hd.u}
+00000730: 9428 685a 6868 685f 4b00 6860 6869 6862  .(hZhhh_K.h`hihb
+00000740: 4aff ffff ff68 6389 6864 8975 7d94 2868  J....hc.hd.u}.(h
+00000750: 5a68 5e68 5f4b 0168 6068 6168 624a ffff  Zh^h_K.h`hahbJ..
+00000760: ffff 6863 8968 6489 757d 9428 685a 6868  ..hc.hd.u}.(hZhh
+00000770: 685f 4b00 6860 6869 6862 4aff ffff ff68  h_K.h`hihbJ....h
+00000780: 6389 6864 8975 7d94 2868 5a68 5e68 5f4b  c.hd.u}.(hZh^h_K
+00000790: 0168 6068 6168 624a ffff ffff 6863 8968  .h`hahbJ....hc.h
+000007a0: 6489 757d 9428 685a 685e 685f 4b01 6860  d.u}.(hZh^h_K.h`
+000007b0: 6861 6862 4aff ffff ff68 6389 6864 8975  hahbJ....hc.hd.u
+000007c0: 7d94 2868 5a68 6868 5f4b 0068 6068 6968  }.(hZhhh_K.h`hih
+000007d0: 624a ffff ffff 6863 8968 6489 757d 9428  bJ....hc.hd.u}.(
+000007e0: 685a 6868 685f 4b01 6860 6861 6862 4aff  hZhhh_K.h`hahbJ.
+000007f0: ffff ff68 6389 6864 8975 7d94 2868 5a68  ...hc.hd.u}.(hZh
+00000800: 6868 5f4b 0068 6068 6968 624a ffff ffff  hh_K.h`hihbJ....
+00000810: 6863 8968 6489 757d 9428 685a 6868 685f  hc.hd.u}.(hZhhh_
+00000820: 4b00 6860 6869 6862 4aff ffff ff68 6389  K.h`hihbJ....hc.
+00000830: 6864 8975 655d 9489 7494 5294 8694 7387  hd.ue]..t.R...s.
+00000840: 9452 948c 0f5f 7661 7269 6162 6c65 5f69  .R..._variable_i
+00000850: 6e69 7473 9429 8c14 5f69 6e74 6572 6e61  nits.).._interna
+00000860: 6c5f 6469 6374 696f 6e61 7279 947d 948c  l_dictionary.}..
+00000870: 065f 7363 6f70 6594 8c13 7079 6363 656c  ._scope...pyccel
+00000880: 2e70 6172 7365 722e 7363 6f70 6594 8c05  .parser.scope...
+00000890: 5363 6f70 6594 9394 2981 944e 7d94 2868  Scope...)..N}.(h
+000008a0: 447d 9428 8c09 6675 6e63 7469 6f6e 7394  D}.(..functions.
+000008b0: 7d94 8c09 7661 7269 6162 6c65 7394 7d94  }...variables.}.
+000008c0: 8c07 636c 6173 7365 7394 7d94 8c07 696d  ..classes.}...im
+000008d0: 706f 7274 7394 7d94 8c12 7379 6d62 6f6c  ports.}...symbol
+000008e0: 6963 5f66 756e 6374 696f 6e73 947d 948c  ic_functions.}..
+000008f0: 066d 6163 726f 7394 7d94 8c09 7465 6d70  .macros.}...temp
+00000900: 6c61 7465 7394 7d94 8c07 6865 6164 6572  lates.}...header
+00000910: 7394 7d94 8c0a 6465 636f 7261 746f 7273  s.}...decorators
+00000920: 947d 948c 0e63 6c73 5f63 6f6e 7374 7275  .}...cls_constru
+00000930: 6374 7394 7d94 758c 075f 6c6f 6361 6c73  cts.}.u.._locals
+00000940: 947d 9428 6889 7d94 688b 7d94 688d 7d94  .}.(h.}.h.}.h.}.
+00000950: 688f 7d94 6891 7d94 6893 7d94 6895 7d94  h.}.h.}.h.}.h.}.
+00000960: 6897 7d94 6899 7d94 689b 7d94 758c 0d5f  h.}.h.}.h.}.u.._
+00000970: 7061 7265 6e74 5f73 636f 7065 944e 8c0c  parent_scope.N..
+00000980: 5f73 6f6e 735f 7363 6f70 6573 947d 948c  _sons_scopes.}..
+00000990: 085f 6973 5f6c 6f6f 7094 898c 065f 6c6f  ._is_loop...._lo
+000009a0: 6f70 7394 5d94 8c14 5f74 656d 706f 7261  ops.]..._tempora
+000009b0: 7279 5f76 6172 6961 626c 6573 945d 948c  ry_variables.]..
+000009c0: 0d5f 7573 6564 5f73 796d 626f 6c73 947d  ._used_symbols.}
+000009d0: 9468 3568 328c 0766 6974 7061 636b 9485  .h5h2..fitpack..
+000009e0: 9481 944e 7d94 6837 8973 8694 6273 8c0e  ...N}.h7.s..bs..
+000009f0: 5f64 756d 6d79 5f63 6f75 6e74 6572 944b  _dummy_counter.K
+00000a00: 008c 105f 6f72 6967 696e 616c 5f73 796d  ..._original_sym
+00000a10: 626f 6c94 7d94 68b5 6835 7375 8694 6268  bol.}.h.h5su..bh
+00000a20: 395d 9468 095d 9468 0d61 683c 8968 3d68  9].h.].h.ah<.h=h
+00000a30: 3e75 8694 628c 095f 6669 6c65 6e61 6d65  >u..b.._filename
+00000a40: 948c 3c2f 686f 6d65 2f79 616d 616e 6775  ..</home/yamangu
+00000a50: 632f 746d 702f 7079 6363 656c 2f70 7963  c/tmp/pyccel/pyc
+00000a60: 6365 6c2f 7374 646c 6962 2f69 6e74 6572  cel/stdlib/inter
+00000a70: 6e61 6c2f 6669 7470 6163 6b2e 7079 6894  nal/fitpack.pyh.
+00000a80: 8c09 5f6d 6574 6176 6172 7394 7d94 288c  .._metavars.}.(.
+00000a90: 1069 676e 6f72 655f 6174 5f69 6d70 6f72  .ignore_at_impor
+00000aa0: 7494 888c 096c 6962 7261 7269 6573 948c  t....libraries..
+00000ab0: 1424 7b46 4954 5041 434b 5f4c 4942 5241  .${FITPACK_LIBRA
+00000ac0: 5249 4553 7d94 8c04 7361 7665 9488 8c08  RIES}...save....
+00000ad0: 6578 7465 726e 616c 9488 7568 8268 868c  external..uh.h..
+00000ae0: 0e5f 6375 7272 656e 745f 636c 6173 7394  ._current_class.
+00000af0: 4e8c 115f 6375 7272 656e 745f 6675 6e63  N.._current_func
+00000b00: 7469 6f6e 944e 8c0c 5f73 796e 7461 785f  tion.N.._syntax_
+00000b10: 646f 6e65 9488 8c0e 5f73 656d 616e 7469  done...._semanti
+00000b20: 635f 646f 6e65 9489 8c11 5f63 7572 7265  c_done...._curre
+00000b30: 6e74 5f66 7374 5f6e 6f64 6594 4e8c 095f  nt_fst_node.N.._
+00000b40: 626c 6f63 6b69 6e67 9489 8c14 5f63 7265  blocking...._cre
+00000b50: 6174 6564 5f66 726f 6d5f 7069 636b 6c65  ated_from_pickle
+00000b60: 9489 8c08 5f63 6f6e 7465 7874 945d 948c  ...._context.]..
+00000b70: 0e5f 696e 5f6c 6873 5f61 7373 6967 6e94  ._in_lhs_assign.
+00000b80: 8975 6287 942e                           .ub...
```

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/hdf5.pyh` & `pyccel-1.9.2/pyccel/stdlib/internal/hdf5.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/lapack.pyh` & `pyccel-1.9.2/pyccel/stdlib/internal/lapack.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/mpi.pyh` & `pyccel-1.9.2/pyccel/stdlib/internal/mpi.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/mpiext.py` & `pyccel-1.9.2/pyccel/stdlib/internal/mpiext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/openacc.pyccel` & `pyccel-1.9.2/pyccel/stdlib/internal/openacc.pyccel`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-00000000: 8004 9520 2b00 0000 0000 008c 2039 3265  ... +....... 92e
+00000000: 8004 9564 2b00 0000 0000 008c 2039 3265  ...d+....... 92e
 00000010: 3531 6230 3535 3231 6330 3337 3164 3037  51b05521c0371d07
 00000020: 3034 6535 3738 3737 3135 3361 6294 8c05  04e57877153ab...
-00000030: 312e 392e 3194 8c17 7079 6363 656c 2e70  1.9.1...pyccel.p
+00000030: 312e 392e 3294 8c17 7079 6363 656c 2e70  1.9.2...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 730a 0000 2320 7079 6363 656c 2068 6561  s...# pyccel hea
 00000080: 6465 7220 666f 7220 4f70 656e 4143 432e  der for OpenACC.
 00000090: 0a23 204f 7065 6e41 4343 2064 6972 6563  .# OpenACC direc
 000000a0: 7469 7665 7320 616e 6420 436f 6e73 7472  tives and Constr
@@ -169,523 +169,527 @@
 00000a80: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000a90: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000aa0: 2e2e 2e2e 2e2e 0a0a 2320 2e2e 2e2e 2e2e  ........# ......
 00000ab0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000ac0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000ad0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000ae0: 2e2e 2e2e 2e2e 0a94 8c04 5f66 7374 948c  .........._fst..
-00000af0: 0361 7374 948c 064d 6f64 756c 6594 9394  .ast...Module...
-00000b00: 2952 947d 9428 8c04 626f 6479 945d 9428  )R.}.(..body.].(
-00000b10: 8c19 7079 6363 656c 2e70 6172 7365 722e  ..pyccel.parser.
-00000b20: 6578 7465 6e64 5f74 7265 6594 8c10 436f  extend_tree...Co
-00000b30: 6d6d 656e 744d 756c 7469 4c69 6e65 9493  mmentMultiLine..
-00000b40: 9458 d202 0000 2320 7079 6363 656c 2068  .X....# pyccel h
-00000b50: 6561 6465 7220 666f 7220 4f70 656e 4143  eader for OpenAC
-00000b60: 432e 0a23 204f 7065 6e41 4343 2064 6972  C..# OpenACC dir
-00000b70: 6563 7469 7665 7320 616e 6420 436f 6e73  ectives and Cons
-00000b80: 7472 7563 7473 2061 7265 2068 616e 646c  tructs are handl
-00000b90: 6564 2062 7920 7468 6520 7061 7273 6572  ed by the parser
-00000ba0: 2028 7365 6520 6f70 656e 6163 632e 7478   (see openacc.tx
-00000bb0: 2920 616e 6420 6172 6520 7061 7274 7320  ) and are parts 
-00000bc0: 6f66 2074 6865 2050 7963 6365 6c20 6c61  of the Pyccel la
-00000bd0: 6e67 7561 6765 2e0a 2320 5765 206f 6e6c  nguage..# We onl
-00000be0: 7920 6c69 7374 2068 6572 6520 7768 6174  y list here what
-00000bf0: 2063 616e 206e 6f74 2062 6520 6465 7363   can not be desc
-00000c00: 7269 6265 6420 696e 2074 6865 206f 7065  ribed in the ope
-00000c10: 6e61 6363 2067 7261 6d6d 6172 2e0a 230a  nacc grammar..#.
-00000c20: 2320 544f 444f 202d 2064 6576 6963 6574  # TODO - devicet
-00000c30: 7970 6520 6973 2066 6f72 2074 6865 206d  ype is for the m
-00000c40: 6f6d 656e 7420 616e 2069 6e74 6567 6572  oment an integer
-00000c50: 2e20 3d3e 206e 6565 6420 746f 2061 6464  . => need to add
-00000c60: 2070 7265 6369 7369 6f6e 0a23 2020 2020   precision.#    
-00000c70: 2020 2d20 6368 616e 6765 202a 2074 6f20    - change * to 
-00000c80: 685f 766f 6964 2a20 616e 6420 645f 766f  h_void* and d_vo
-00000c90: 6964 2a20 696e 0a23 2020 2020 2020 2020  id* in.#        
-00000ca0: 202b 2061 6363 5f6d 6170 5f64 6174 610a   + acc_map_data.
-00000cb0: 2320 2020 2020 2020 2020 2b20 6163 635f  #         + acc_
-00000cc0: 756e 6d61 705f 6461 7461 0a23 2020 2020  unmap_data.#    
-00000cd0: 2020 2020 202b 2061 6363 5f64 6576 6963       + acc_devic
-00000ce0: 6570 7472 0a23 2020 2020 2020 2020 202b  eptr.#         +
-00000cf0: 2061 6363 5f68 6f73 7470 7472 0a23 2020   acc_hostptr.#  
-00000d00: 2020 2020 2020 202b 2061 6363 5f6d 656d         + acc_mem
-00000d10: 6370 795f 746f 5f64 6576 6963 650a 2320  cpy_to_device.# 
-00000d20: 2020 2020 2020 2020 2b20 6163 635f 6d65          + acc_me
-00000d30: 6d63 7079 5f74 6f5f 6465 7669 6365 5f61  mcpy_to_device_a
-00000d40: 7379 6e63 0a23 2020 2020 2020 2020 202b  sync.#         +
-00000d50: 2061 6363 5f6d 656d 6370 795f 6672 6f6d   acc_memcpy_from
-00000d60: 5f64 6576 6963 650a 2320 2020 2020 2020  _device.#       
-00000d70: 2020 2b20 6163 635f 6d65 6d63 7079 5f66    + acc_memcpy_f
-00000d80: 726f 6d5f 6465 7669 6365 5f61 7379 6e63  rom_device_async
-00000d90: 0a23 2020 2020 2020 2020 202b 2061 6363  .#         + acc
-00000da0: 5f6d 656d 6370 795f 6465 7669 6365 0a23  _memcpy_device.#
-00000db0: 2020 2020 2020 2020 202b 2061 6363 5f6d           + acc_m
-00000dc0: 656d 6370 795f 6465 7669 6365 5f61 7379  emcpy_device_asy
-00000dd0: 6e63 0a23 2020 2020 2020 2020 202b 0a23  nc.#         +.#
-00000de0: 2020 2020 2020 2d20 6461 7461 206d 6f76        - data mov
-00000df0: 656d 656e 7420 726f 7574 696e 6573 2028  ement routines (
-00000e00: 646f 2077 6520 7265 616c 6c79 206e 6565  do we really nee
-00000e10: 6420 7468 656d 3f29 944b 014b 0087 9452  d them?).K.K...R
-00000e20: 9468 138c 8b23 2420 6865 6164 6572 206d  .h...#$ header m
-00000e30: 6574 6176 6172 206d 6f64 756c 655f 6e61  etavar module_na
-00000e40: 6d65 3d27 6f70 656e 6163 6327 0a23 2420  me='openacc'.#$ 
-00000e50: 6865 6164 6572 206d 6574 6176 6172 206d  header metavar m
-00000e60: 6f64 756c 655f 7665 7273 696f 6e3d 2732  odule_version='2
-00000e70: 2e35 270a 2324 2068 6561 6465 7220 6d65  .5'.#$ header me
-00000e80: 7461 7661 7220 7361 7665 3d54 7275 650a  tavar save=True.
-00000e90: 2324 2068 6561 6465 7220 6d65 7461 7661  #$ header metava
-00000ea0: 7220 6578 7465 726e 616c 3d46 616c 7365  r external=False
-00000eb0: 944b 154b 0087 9452 9468 138c af23 202e  .K.K...R.h...# .
+00000af0: 045f 6173 7494 8c06 4d6f 6475 6c65 9493  ._ast...Module..
+00000b00: 9429 5294 7d94 288c 0462 6f64 7994 5d94  .)R.}.(..body.].
+00000b10: 288c 1970 7963 6365 6c2e 7061 7273 6572  (..pyccel.parser
+00000b20: 2e65 7874 656e 645f 7472 6565 948c 1043  .extend_tree...C
+00000b30: 6f6d 6d65 6e74 4d75 6c74 694c 696e 6594  ommentMultiLine.
+00000b40: 9394 58d2 0200 0023 2070 7963 6365 6c20  ..X....# pyccel 
+00000b50: 6865 6164 6572 2066 6f72 204f 7065 6e41  header for OpenA
+00000b60: 4343 2e0a 2320 4f70 656e 4143 4320 6469  CC..# OpenACC di
+00000b70: 7265 6374 6976 6573 2061 6e64 2043 6f6e  rectives and Con
+00000b80: 7374 7275 6374 7320 6172 6520 6861 6e64  structs are hand
+00000b90: 6c65 6420 6279 2074 6865 2070 6172 7365  led by the parse
+00000ba0: 7220 2873 6565 206f 7065 6e61 6363 2e74  r (see openacc.t
+00000bb0: 7829 2061 6e64 2061 7265 2070 6172 7473  x) and are parts
+00000bc0: 206f 6620 7468 6520 5079 6363 656c 206c   of the Pyccel l
+00000bd0: 616e 6775 6167 652e 0a23 2057 6520 6f6e  anguage..# We on
+00000be0: 6c79 206c 6973 7420 6865 7265 2077 6861  ly list here wha
+00000bf0: 7420 6361 6e20 6e6f 7420 6265 2064 6573  t can not be des
+00000c00: 6372 6962 6564 2069 6e20 7468 6520 6f70  cribed in the op
+00000c10: 656e 6163 6320 6772 616d 6d61 722e 0a23  enacc grammar..#
+00000c20: 0a23 2054 4f44 4f20 2d20 6465 7669 6365  .# TODO - device
+00000c30: 7479 7065 2069 7320 666f 7220 7468 6520  type is for the 
+00000c40: 6d6f 6d65 6e74 2061 6e20 696e 7465 6765  moment an intege
+00000c50: 722e 203d 3e20 6e65 6564 2074 6f20 6164  r. => need to ad
+00000c60: 6420 7072 6563 6973 696f 6e0a 2320 2020  d precision.#   
+00000c70: 2020 202d 2063 6861 6e67 6520 2a20 746f     - change * to
+00000c80: 2068 5f76 6f69 642a 2061 6e64 2064 5f76   h_void* and d_v
+00000c90: 6f69 642a 2069 6e0a 2320 2020 2020 2020  oid* in.#       
+00000ca0: 2020 2b20 6163 635f 6d61 705f 6461 7461    + acc_map_data
+00000cb0: 0a23 2020 2020 2020 2020 202b 2061 6363  .#         + acc
+00000cc0: 5f75 6e6d 6170 5f64 6174 610a 2320 2020  _unmap_data.#   
+00000cd0: 2020 2020 2020 2b20 6163 635f 6465 7669        + acc_devi
+00000ce0: 6365 7074 720a 2320 2020 2020 2020 2020  ceptr.#         
+00000cf0: 2b20 6163 635f 686f 7374 7074 720a 2320  + acc_hostptr.# 
+00000d00: 2020 2020 2020 2020 2b20 6163 635f 6d65          + acc_me
+00000d10: 6d63 7079 5f74 6f5f 6465 7669 6365 0a23  mcpy_to_device.#
+00000d20: 2020 2020 2020 2020 202b 2061 6363 5f6d           + acc_m
+00000d30: 656d 6370 795f 746f 5f64 6576 6963 655f  emcpy_to_device_
+00000d40: 6173 796e 630a 2320 2020 2020 2020 2020  async.#         
+00000d50: 2b20 6163 635f 6d65 6d63 7079 5f66 726f  + acc_memcpy_fro
+00000d60: 6d5f 6465 7669 6365 0a23 2020 2020 2020  m_device.#      
+00000d70: 2020 202b 2061 6363 5f6d 656d 6370 795f     + acc_memcpy_
+00000d80: 6672 6f6d 5f64 6576 6963 655f 6173 796e  from_device_asyn
+00000d90: 630a 2320 2020 2020 2020 2020 2b20 6163  c.#         + ac
+00000da0: 635f 6d65 6d63 7079 5f64 6576 6963 650a  c_memcpy_device.
+00000db0: 2320 2020 2020 2020 2020 2b20 6163 635f  #         + acc_
+00000dc0: 6d65 6d63 7079 5f64 6576 6963 655f 6173  memcpy_device_as
+00000dd0: 796e 630a 2320 2020 2020 2020 2020 2b0a  ync.#         +.
+00000de0: 2320 2020 2020 202d 2064 6174 6120 6d6f  #      - data mo
+00000df0: 7665 6d65 6e74 2072 6f75 7469 6e65 7320  vement routines 
+00000e00: 2864 6f20 7765 2072 6561 6c6c 7920 6e65  (do we really ne
+00000e10: 6564 2074 6865 6d3f 2994 4b01 4b00 8794  ed them?).K.K...
+00000e20: 5294 6813 8c8b 2324 2068 6561 6465 7220  R.h...#$ header 
+00000e30: 6d65 7461 7661 7220 6d6f 6475 6c65 5f6e  metavar module_n
+00000e40: 616d 653d 276f 7065 6e61 6363 270a 2324  ame='openacc'.#$
+00000e50: 2068 6561 6465 7220 6d65 7461 7661 7220   header metavar 
+00000e60: 6d6f 6475 6c65 5f76 6572 7369 6f6e 3d27  module_version='
+00000e70: 322e 3527 0a23 2420 6865 6164 6572 206d  2.5'.#$ header m
+00000e80: 6574 6176 6172 2073 6176 653d 5472 7565  etavar save=True
+00000e90: 0a23 2420 6865 6164 6572 206d 6574 6176  .#$ header metav
+00000ea0: 6172 2065 7874 6572 6e61 6c3d 4661 6c73  ar external=Fals
+00000eb0: 6594 4b15 4b00 8794 5294 6813 8caf 2320  e.K.K...R.h...# 
 00000ec0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000ed0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000ee0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000ef0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e0a 2320 2020  ............#   
-00000f00: 2020 2020 2020 2020 2052 756e 7469 6d65           Runtime
-00000f10: 204c 6962 7261 7279 2052 6f75 7469 6e65   Library Routine
-00000f20: 7320 666f 7220 466f 7274 7261 6e0a 2320  s for Fortran.# 
-00000f30: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00000ef0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 0a23 2020  .............#  
+00000f00: 2020 2020 2020 2020 2020 5275 6e74 696d            Runtim
+00000f10: 6520 4c69 6272 6172 7920 526f 7574 696e  e Library Routin
+00000f20: 6573 2066 6f72 2046 6f72 7472 616e 0a23  es for Fortran.#
+00000f30: 202e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e   ...............
 00000f40: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000f50: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000f60: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 944b 1a4b  .............K.K
-00000f70: 0087 9452 9468 118c 0b43 6f6d 6d65 6e74  ...R.h...Comment
-00000f80: 4c69 6e65 9493 948c 3823 2420 6865 6164  Line....8#$ head
-00000f90: 6572 2066 756e 6374 696f 6e20 6163 635f  er function acc_
-00000fa0: 6765 745f 6e75 6d5f 6465 7669 6365 7328  get_num_devices(
-00000fb0: 696e 7429 2072 6573 756c 7473 2869 6e74  int) results(int
-00000fc0: 2994 4b1e 4b00 8794 5294 6813 8c61 2324  ).K.K...R.h..a#$
-00000fd0: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
-00000fe0: 2061 6363 5f73 6574 5f64 6576 6963 655f   acc_set_device_
-00000ff0: 7479 7065 2869 6e74 290a 2324 2068 6561  type(int).#$ hea
-00001000: 6465 7220 6675 6e63 7469 6f6e 2061 6363  der function acc
-00001010: 5f67 6574 5f64 6576 6963 655f 7479 7065  _get_device_type
-00001020: 2829 2072 6573 756c 7473 2869 6e74 2994  () results(int).
-00001030: 4b20 4b00 8794 5294 6813 8c67 2324 2068  K K...R.h..g#$ h
-00001040: 6561 6465 7220 6675 6e63 7469 6f6e 2061  eader function a
-00001050: 6363 5f73 6574 5f64 6576 6963 655f 6e75  cc_set_device_nu
-00001060: 6d28 696e 742c 2069 6e74 290a 2324 2068  m(int, int).#$ h
-00001070: 6561 6465 7220 6675 6e63 7469 6f6e 2061  eader function a
-00001080: 6363 5f67 6574 5f64 6576 6963 655f 6e75  cc_get_device_nu
-00001090: 6d28 696e 7429 2072 6573 756c 7473 2869  m(int) results(i
-000010a0: 6e74 2994 4b23 4b00 8794 5294 6813 8c45  nt).K#K...R.h..E
-000010b0: 2324 2068 6561 6465 7220 6675 6e63 7469  #$ header functi
-000010c0: 6f6e 2061 6363 5f69 6e69 7428 696e 7429  on acc_init(int)
-000010d0: 0a23 2420 6865 6164 6572 2066 756e 6374  .#$ header funct
-000010e0: 696f 6e20 6163 635f 7368 7574 646f 776e  ion acc_shutdown
-000010f0: 2869 6e74 2994 4b26 4b00 8794 5294 6813  (int).K&K...R.h.
-00001100: 8c6b 2324 2068 6561 6465 7220 6675 6e63  .k#$ header func
-00001110: 7469 6f6e 2061 6363 5f61 7379 6e63 5f74  tion acc_async_t
-00001120: 6573 7428 626f 6f6c 2920 7265 7375 6c74  est(bool) result
-00001130: 7328 626f 6f6c 290a 2324 2068 6561 6465  s(bool).#$ heade
-00001140: 7220 6675 6e63 7469 6f6e 2061 6363 5f61  r function acc_a
-00001150: 7379 6e63 5f74 6573 745f 616c 6c28 2920  sync_test_all() 
-00001160: 7265 7375 6c74 7328 626f 6f6c 2994 4b29  results(bool).K)
-00001170: 4b00 8794 5294 6813 8c9d 2324 2068 6561  K...R.h...#$ hea
-00001180: 6465 7220 6675 6e63 7469 6f6e 2061 6363  der function acc
-00001190: 5f77 6169 7428 626f 6f6c 290a 2324 2068  _wait(bool).#$ h
-000011a0: 6561 6465 7220 6675 6e63 7469 6f6e 2061  eader function a
-000011b0: 6363 5f77 6169 745f 616c 6c28 626f 6f6c  cc_wait_all(bool
-000011c0: 290a 2324 2068 6561 6465 7220 6675 6e63  ).#$ header func
-000011d0: 7469 6f6e 2061 6363 5f77 6169 745f 6173  tion acc_wait_as
-000011e0: 796e 6328 626f 6f6c 2c20 626f 6f6c 290a  ync(bool, bool).
-000011f0: 2324 2068 6561 6465 7220 6675 6e63 7469  #$ header functi
-00001200: 6f6e 2061 6363 5f77 6169 745f 616c 6c5f  on acc_wait_all_
-00001210: 6173 796e 6328 2994 4b2c 4b00 8794 5294  async().K,K...R.
-00001220: 6813 8c62 2324 2068 6561 6465 7220 6675  h..b#$ header fu
-00001230: 6e63 7469 6f6e 2061 6363 5f67 6574 5f64  nction acc_get_d
-00001240: 6566 6175 6c74 5f61 7379 6e63 2829 2072  efault_async() r
-00001250: 6573 756c 7473 2869 6e74 290a 2324 2068  esults(int).#$ h
-00001260: 6561 6465 7220 6675 6e63 7469 6f6e 2061  eader function a
-00001270: 6363 5f73 6574 5f64 6566 6175 6c74 5f61  cc_set_default_a
-00001280: 7379 6e63 2829 944b 314b 0087 9452 9468  sync().K1K...R.h
-00001290: 138c 7823 2420 6865 6164 6572 2066 756e  ..x#$ header fun
-000012a0: 6374 696f 6e20 6163 635f 6f6e 5f64 6576  ction acc_on_dev
-000012b0: 6963 6528 696e 7429 0a23 0a23 2420 6865  ice(int).#.#$ he
-000012c0: 6164 6572 2066 756e 6374 696f 6e20 6163  ader function ac
-000012d0: 635f 6d61 6c6c 6f63 2869 6e74 2920 7265  c_malloc(int) re
-000012e0: 7375 6c74 7328 696e 7429 0a23 2420 6865  sults(int).#$ he
-000012f0: 6164 6572 2066 756e 6374 696f 6e20 6163  ader function ac
-00001300: 635f 6672 6565 2869 6e74 2994 4b34 4b00  c_free(int).K4K.
-00001310: 8794 5294 6813 8c4f 2324 2068 6561 6465  ..R.h..O#$ heade
-00001320: 7220 6675 6e63 7469 6f6e 2061 6363 5f6d  r function acc_m
-00001330: 6170 5f64 6174 6128 2a2c 202a 2c20 696e  ap_data(*, *, in
-00001340: 7429 0a23 2420 6865 6164 6572 2066 756e  t).#$ header fun
-00001350: 6374 696f 6e20 6163 635f 756e 6d61 705f  ction acc_unmap_
-00001360: 6461 7461 282a 2994 4b39 4b00 8794 5294  data(*).K9K...R.
-00001370: 6813 8c5f 2324 2068 6561 6465 7220 6675  h.._#$ header fu
-00001380: 6e63 7469 6f6e 2061 6363 5f64 6576 6963  nction acc_devic
-00001390: 6570 7472 282a 2920 7265 7375 6c74 7328  eptr(*) results(
-000013a0: 696e 7429 0a23 2420 6865 6164 6572 2066  int).#$ header f
-000013b0: 756e 6374 696f 6e20 6163 635f 686f 7374  unction acc_host
-000013c0: 7074 7228 2a29 2072 6573 756c 7473 2869  ptr(*) results(i
-000013d0: 6e74 2994 4b3c 4b00 8794 5294 6813 5850  nt).K<K...R.h.XP
-000013e0: 0100 0023 2420 6865 6164 6572 2066 756e  ...#$ header fun
-000013f0: 6374 696f 6e20 6163 635f 6d65 6d63 7079  ction acc_memcpy
-00001400: 5f74 6f5f 6465 7669 6365 282a 2c20 2a2c  _to_device(*, *,
-00001410: 2069 6e74 290a 2324 2068 6561 6465 7220   int).#$ header 
-00001420: 6675 6e63 7469 6f6e 2061 6363 5f6d 656d  function acc_mem
-00001430: 6370 795f 746f 5f64 6576 6963 655f 6173  cpy_to_device_as
-00001440: 796e 6328 2a2c 202a 2c20 696e 742c 2069  ync(*, *, int, i
-00001450: 6e74 290a 2324 2068 6561 6465 7220 6675  nt).#$ header fu
-00001460: 6e63 7469 6f6e 2061 6363 5f6d 656d 6370  nction acc_memcp
-00001470: 795f 6672 6f6d 5f64 6576 6963 6528 2a2c  y_from_device(*,
-00001480: 202a 2c20 696e 7429 0a23 2420 6865 6164   *, int).#$ head
-00001490: 6572 2066 756e 6374 696f 6e20 6163 635f  er function acc_
-000014a0: 6d65 6d63 7079 5f66 726f 6d5f 6465 7669  memcpy_from_devi
-000014b0: 6365 5f61 7379 6e63 282a 2c20 2a2c 2069  ce_async(*, *, i
-000014c0: 6e74 2c20 696e 7429 0a23 2420 6865 6164  nt, int).#$ head
-000014d0: 6572 2066 756e 6374 696f 6e20 6163 635f  er function acc_
-000014e0: 6d65 6d63 7079 5f64 6576 6963 6528 2a2c  memcpy_device(*,
-000014f0: 202a 2c20 696e 7429 0a23 2420 6865 6164   *, int).#$ head
-00001500: 6572 2066 756e 6374 696f 6e20 6163 635f  er function acc_
-00001510: 6d65 6d63 7079 5f64 6576 6963 655f 6173  memcpy_device_as
-00001520: 796e 6328 2a2c 202a 2c20 696e 742c 2069  ync(*, *, int, i
-00001530: 6e74 2994 4b3f 4b00 8794 5294 681e 8c3e  nt).K?K...R.h..>
-00001540: 2320 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  # ..............
+00000f60: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e94 4b1a  ..............K.
+00000f70: 4b00 8794 5294 6811 8c0b 436f 6d6d 656e  K...R.h...Commen
+00000f80: 744c 696e 6594 9394 8c38 2324 2068 6561  tLine....8#$ hea
+00000f90: 6465 7220 6675 6e63 7469 6f6e 2061 6363  der function acc
+00000fa0: 5f67 6574 5f6e 756d 5f64 6576 6963 6573  _get_num_devices
+00000fb0: 2869 6e74 2920 7265 7375 6c74 7328 696e  (int) results(in
+00000fc0: 7429 944b 1e4b 0087 9452 9468 138c 6123  t).K.K...R.h..a#
+00000fd0: 2420 6865 6164 6572 2066 756e 6374 696f  $ header functio
+00000fe0: 6e20 6163 635f 7365 745f 6465 7669 6365  n acc_set_device
+00000ff0: 5f74 7970 6528 696e 7429 0a23 2420 6865  _type(int).#$ he
+00001000: 6164 6572 2066 756e 6374 696f 6e20 6163  ader function ac
+00001010: 635f 6765 745f 6465 7669 6365 5f74 7970  c_get_device_typ
+00001020: 6528 2920 7265 7375 6c74 7328 696e 7429  e() results(int)
+00001030: 944b 204b 0087 9452 9468 138c 6723 2420  .K K...R.h..g#$ 
+00001040: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+00001050: 6163 635f 7365 745f 6465 7669 6365 5f6e  acc_set_device_n
+00001060: 756d 2869 6e74 2c20 696e 7429 0a23 2420  um(int, int).#$ 
+00001070: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+00001080: 6163 635f 6765 745f 6465 7669 6365 5f6e  acc_get_device_n
+00001090: 756d 2869 6e74 2920 7265 7375 6c74 7328  um(int) results(
+000010a0: 696e 7429 944b 234b 0087 9452 9468 138c  int).K#K...R.h..
+000010b0: 4523 2420 6865 6164 6572 2066 756e 6374  E#$ header funct
+000010c0: 696f 6e20 6163 635f 696e 6974 2869 6e74  ion acc_init(int
+000010d0: 290a 2324 2068 6561 6465 7220 6675 6e63  ).#$ header func
+000010e0: 7469 6f6e 2061 6363 5f73 6875 7464 6f77  tion acc_shutdow
+000010f0: 6e28 696e 7429 944b 264b 0087 9452 9468  n(int).K&K...R.h
+00001100: 138c 6b23 2420 6865 6164 6572 2066 756e  ..k#$ header fun
+00001110: 6374 696f 6e20 6163 635f 6173 796e 635f  ction acc_async_
+00001120: 7465 7374 2862 6f6f 6c29 2072 6573 756c  test(bool) resul
+00001130: 7473 2862 6f6f 6c29 0a23 2420 6865 6164  ts(bool).#$ head
+00001140: 6572 2066 756e 6374 696f 6e20 6163 635f  er function acc_
+00001150: 6173 796e 635f 7465 7374 5f61 6c6c 2829  async_test_all()
+00001160: 2072 6573 756c 7473 2862 6f6f 6c29 944b   results(bool).K
+00001170: 294b 0087 9452 9468 138c 9d23 2420 6865  )K...R.h...#$ he
+00001180: 6164 6572 2066 756e 6374 696f 6e20 6163  ader function ac
+00001190: 635f 7761 6974 2862 6f6f 6c29 0a23 2420  c_wait(bool).#$ 
+000011a0: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+000011b0: 6163 635f 7761 6974 5f61 6c6c 2862 6f6f  acc_wait_all(boo
+000011c0: 6c29 0a23 2420 6865 6164 6572 2066 756e  l).#$ header fun
+000011d0: 6374 696f 6e20 6163 635f 7761 6974 5f61  ction acc_wait_a
+000011e0: 7379 6e63 2862 6f6f 6c2c 2062 6f6f 6c29  sync(bool, bool)
+000011f0: 0a23 2420 6865 6164 6572 2066 756e 6374  .#$ header funct
+00001200: 696f 6e20 6163 635f 7761 6974 5f61 6c6c  ion acc_wait_all
+00001210: 5f61 7379 6e63 2829 944b 2c4b 0087 9452  _async().K,K...R
+00001220: 9468 138c 6223 2420 6865 6164 6572 2066  .h..b#$ header f
+00001230: 756e 6374 696f 6e20 6163 635f 6765 745f  unction acc_get_
+00001240: 6465 6661 756c 745f 6173 796e 6328 2920  default_async() 
+00001250: 7265 7375 6c74 7328 696e 7429 0a23 2420  results(int).#$ 
+00001260: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+00001270: 6163 635f 7365 745f 6465 6661 756c 745f  acc_set_default_
+00001280: 6173 796e 6328 2994 4b31 4b00 8794 5294  async().K1K...R.
+00001290: 6813 8c78 2324 2068 6561 6465 7220 6675  h..x#$ header fu
+000012a0: 6e63 7469 6f6e 2061 6363 5f6f 6e5f 6465  nction acc_on_de
+000012b0: 7669 6365 2869 6e74 290a 230a 2324 2068  vice(int).#.#$ h
+000012c0: 6561 6465 7220 6675 6e63 7469 6f6e 2061  eader function a
+000012d0: 6363 5f6d 616c 6c6f 6328 696e 7429 2072  cc_malloc(int) r
+000012e0: 6573 756c 7473 2869 6e74 290a 2324 2068  esults(int).#$ h
+000012f0: 6561 6465 7220 6675 6e63 7469 6f6e 2061  eader function a
+00001300: 6363 5f66 7265 6528 696e 7429 944b 344b  cc_free(int).K4K
+00001310: 0087 9452 9468 138c 4f23 2420 6865 6164  ...R.h..O#$ head
+00001320: 6572 2066 756e 6374 696f 6e20 6163 635f  er function acc_
+00001330: 6d61 705f 6461 7461 282a 2c20 2a2c 2069  map_data(*, *, i
+00001340: 6e74 290a 2324 2068 6561 6465 7220 6675  nt).#$ header fu
+00001350: 6e63 7469 6f6e 2061 6363 5f75 6e6d 6170  nction acc_unmap
+00001360: 5f64 6174 6128 2a29 944b 394b 0087 9452  _data(*).K9K...R
+00001370: 9468 138c 5f23 2420 6865 6164 6572 2066  .h.._#$ header f
+00001380: 756e 6374 696f 6e20 6163 635f 6465 7669  unction acc_devi
+00001390: 6365 7074 7228 2a29 2072 6573 756c 7473  ceptr(*) results
+000013a0: 2869 6e74 290a 2324 2068 6561 6465 7220  (int).#$ header 
+000013b0: 6675 6e63 7469 6f6e 2061 6363 5f68 6f73  function acc_hos
+000013c0: 7470 7472 282a 2920 7265 7375 6c74 7328  tptr(*) results(
+000013d0: 696e 7429 944b 3c4b 0087 9452 9468 1358  int).K<K...R.h.X
+000013e0: 5001 0000 2324 2068 6561 6465 7220 6675  P...#$ header fu
+000013f0: 6e63 7469 6f6e 2061 6363 5f6d 656d 6370  nction acc_memcp
+00001400: 795f 746f 5f64 6576 6963 6528 2a2c 202a  y_to_device(*, *
+00001410: 2c20 696e 7429 0a23 2420 6865 6164 6572  , int).#$ header
+00001420: 2066 756e 6374 696f 6e20 6163 635f 6d65   function acc_me
+00001430: 6d63 7079 5f74 6f5f 6465 7669 6365 5f61  mcpy_to_device_a
+00001440: 7379 6e63 282a 2c20 2a2c 2069 6e74 2c20  sync(*, *, int, 
+00001450: 696e 7429 0a23 2420 6865 6164 6572 2066  int).#$ header f
+00001460: 756e 6374 696f 6e20 6163 635f 6d65 6d63  unction acc_memc
+00001470: 7079 5f66 726f 6d5f 6465 7669 6365 282a  py_from_device(*
+00001480: 2c20 2a2c 2069 6e74 290a 2324 2068 6561  , *, int).#$ hea
+00001490: 6465 7220 6675 6e63 7469 6f6e 2061 6363  der function acc
+000014a0: 5f6d 656d 6370 795f 6672 6f6d 5f64 6576  _memcpy_from_dev
+000014b0: 6963 655f 6173 796e 6328 2a2c 202a 2c20  ice_async(*, *, 
+000014c0: 696e 742c 2069 6e74 290a 2324 2068 6561  int, int).#$ hea
+000014d0: 6465 7220 6675 6e63 7469 6f6e 2061 6363  der function acc
+000014e0: 5f6d 656d 6370 795f 6465 7669 6365 282a  _memcpy_device(*
+000014f0: 2c20 2a2c 2069 6e74 290a 2324 2068 6561  , *, int).#$ hea
+00001500: 6465 7220 6675 6e63 7469 6f6e 2061 6363  der function acc
+00001510: 5f6d 656d 6370 795f 6465 7669 6365 5f61  _memcpy_device_a
+00001520: 7379 6e63 282a 2c20 2a2c 2069 6e74 2c20  sync(*, *, int, 
+00001530: 696e 7429 944b 3f4b 0087 9452 9468 1e8c  int).K?K...R.h..
+00001540: 3e23 202e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ># .............
 00001550: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001560: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00001570: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 944b  ...............K
-00001580: 464b 0087 9452 9468 138c a023 202e 2e2e  FK...R.h...# ...
+00001570: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e94  ................
+00001580: 4b46 4b00 8794 5294 6813 8ca0 2320 2e2e  KFK...R.h...# ..
 00001590: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 000015a0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 000015b0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-000015c0: 2e2e 2e2e 2e2e 2e2e 2e0a 2320 2020 2020  ..........#     
-000015d0: 2020 2020 2020 4461 7461 204d 6f76 656d        Data Movem
-000015e0: 656e 7420 726f 7574 696e 6573 0a23 202e  ent routines.# .
+000015c0: 2e2e 2e2e 2e2e 2e2e 2e2e 0a23 2020 2020  ...........#    
+000015d0: 2020 2020 2020 2044 6174 6120 4d6f 7665         Data Move
+000015e0: 6d65 6e74 2072 6f75 7469 6e65 730a 2320  ment routines.# 
 000015f0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001600: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001610: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00001620: 2e2e 2e2e 2e2e 2e2e 2e2e 2e94 4b48 4b00  ............KHK.
-00001630: 8794 5294 681e 8c3e 2320 2e2e 2e2e 2e2e  ..R.h..># ......
+00001620: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 944b 484b  .............KHK
+00001630: 0087 9452 9468 1e8c 3e23 202e 2e2e 2e2e  ...R.h..># .....
 00001640: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001650: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001660: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00001670: 2e2e 2e2e 2e2e 944b 4c4b 0087 9452 9465  .......KLK...R.e
-00001680: 8c0c 7479 7065 5f69 676e 6f72 6573 945d  ..type_ignores.]
-00001690: 948c 066c 696e 656e 6f94 4b01 8c0a 636f  ...lineno.K...co
-000016a0: 6c5f 6f66 6673 6574 944b 0175 628c 045f  l_offset.K.ub.._
-000016b0: 6173 7494 8c0f 7079 6363 656c 2e61 7374  ast...pyccel.ast
-000016c0: 2e63 6f72 6594 8c06 4d6f 6475 6c65 9493  .core...Module..
-000016d0: 9429 8194 4e7d 9428 8c05 5f6e 616d 6594  .)..N}.(.._name.
-000016e0: 684e 8c06 4173 4e61 6d65 9493 9429 8194  hN..AsName...)..
-000016f0: 4e7d 9428 8c04 5f6f 626a 948c 076f 7065  N}.(.._obj...ope
-00001700: 6e61 6363 948c 075f 7461 7267 6574 948c  nacc..._target..
-00001710: 1470 7963 6365 6c2e 6173 742e 696e 7465  .pyccel.ast.inte
-00001720: 726e 616c 7394 8c0c 5079 6363 656c 5379  rnals...PyccelSy
-00001730: 6d62 6f6c 9493 948c 076f 7065 6e61 6363  mbol.....openacc
-00001740: 9485 9481 944e 7d94 8c08 5f69 735f 7465  .....N}..._is_te
-00001750: 6d70 9489 7386 9462 8c0b 5f75 7365 725f  mp..s..b.._user_
-00001760: 6e6f 6465 7394 5d94 6809 5d94 8c16 5f72  nodes.].h.]..._r
-00001770: 6563 7572 7369 6f6e 5f69 6e5f 7072 6f67  ecursion_in_prog
-00001780: 7265 7373 9489 8c0f 5f70 7963 6365 6c5f  ress...._pyccel_
-00001790: 7374 6167 696e 6794 8c09 7379 6e74 6163  staging...syntac
-000017a0: 7469 6394 7586 9462 8c0a 5f76 6172 6961  tic.u..b.._varia
-000017b0: 626c 6573 9429 8c06 5f66 756e 6373 9429  bles.).._funcs.)
-000017c0: 8c0b 5f69 6e74 6572 6661 6365 7394 298c  .._interfaces.).
-000017d0: 085f 636c 6173 7365 7394 298c 085f 696d  ._classes.).._im
-000017e0: 706f 7274 7394 298c 0a5f 696e 6974 5f66  ports.).._init_f
-000017f0: 756e 6394 4e8c 0a5f 6672 6565 5f66 756e  unc.N.._free_fun
-00001800: 6394 4e8c 085f 7072 6f67 7261 6d94 684e  c.N.._program.hN
-00001810: 8c05 6170 706c 7994 9394 684e 8c09 436f  ..apply...hN..Co
-00001820: 6465 426c 6f63 6b94 9394 297d 9468 0f28  deBlock...)}.h.(
-00001830: 6874 684e 8c07 436f 6d6d 656e 7494 9394  hthN..Comment...
-00001840: 297d 948c 0474 6578 7494 8c1a 7079 6363  )}...text...pycc
-00001850: 656c 2068 6561 6465 7220 666f 7220 4f70  el header for Op
-00001860: 656e 4143 432e 9473 8794 5294 6874 6879  enACC..s..R.hthy
-00001870: 297d 9468 7b8c 724f 7065 6e41 4343 2064  )}.h{.rOpenACC d
-00001880: 6972 6563 7469 7665 7320 616e 6420 436f  irectives and Co
-00001890: 6e73 7472 7563 7473 2061 7265 2068 616e  nstructs are han
-000018a0: 646c 6564 2062 7920 7468 6520 7061 7273  dled by the pars
-000018b0: 6572 2028 7365 6520 6f70 656e 6163 632e  er (see openacc.
-000018c0: 7478 2920 616e 6420 6172 6520 7061 7274  tx) and are part
-000018d0: 7320 6f66 2074 6865 2050 7963 6365 6c20  s of the Pyccel 
-000018e0: 6c61 6e67 7561 6765 2e94 7387 9452 9468  language..s..R.h
-000018f0: 7468 7929 7d94 687b 8c43 5765 206f 6e6c  thy)}.h{.CWe onl
-00001900: 7920 6c69 7374 2068 6572 6520 7768 6174  y list here what
-00001910: 2063 616e 206e 6f74 2062 6520 6465 7363   can not be desc
-00001920: 7269 6265 6420 696e 2074 6865 206f 7065  ribed in the ope
-00001930: 6e61 6363 2067 7261 6d6d 6172 2e94 7387  nacc grammar..s.
-00001940: 9452 9468 7468 7929 7d94 687b 8c00 9473  .R.hthy)}.h{...s
-00001950: 8794 5294 6874 6879 297d 9468 7b8c 4854  ..R.hthy)}.h{.HT
-00001960: 4f44 4f20 2d20 6465 7669 6365 7479 7065  ODO - devicetype
-00001970: 2069 7320 666f 7220 7468 6520 6d6f 6d65   is for the mome
-00001980: 6e74 2061 6e20 696e 7465 6765 722e 203d  nt an integer. =
-00001990: 3e20 6e65 6564 2074 6f20 6164 6420 7072  > need to add pr
-000019a0: 6563 6973 696f 6e94 7387 9452 9468 7468  ecision.s..R.hth
-000019b0: 7929 7d94 687b 8c24 2d20 6368 616e 6765  y)}.h{.$- change
-000019c0: 202a 2074 6f20 685f 766f 6964 2a20 616e   * to h_void* an
-000019d0: 6420 645f 766f 6964 2a20 696e 9473 8794  d d_void* in.s..
-000019e0: 5294 6874 6879 297d 9468 7b8c 0e2b 2061  R.hthy)}.h{..+ a
-000019f0: 6363 5f6d 6170 5f64 6174 6194 7387 9452  cc_map_data.s..R
-00001a00: 9468 7468 7929 7d94 687b 8c10 2b20 6163  .hthy)}.h{..+ ac
-00001a10: 635f 756e 6d61 705f 6461 7461 9473 8794  c_unmap_data.s..
-00001a20: 5294 6874 6879 297d 9468 7b8c 0f2b 2061  R.hthy)}.h{..+ a
-00001a30: 6363 5f64 6576 6963 6570 7472 9473 8794  cc_deviceptr.s..
-00001a40: 5294 6874 6879 297d 9468 7b8c 0d2b 2061  R.hthy)}.h{..+ a
-00001a50: 6363 5f68 6f73 7470 7472 9473 8794 5294  cc_hostptr.s..R.
-00001a60: 6874 6879 297d 9468 7b8c 162b 2061 6363  hthy)}.h{..+ acc
-00001a70: 5f6d 656d 6370 795f 746f 5f64 6576 6963  _memcpy_to_devic
-00001a80: 6594 7387 9452 9468 7468 7929 7d94 687b  e.s..R.hthy)}.h{
-00001a90: 8c1c 2b20 6163 635f 6d65 6d63 7079 5f74  ..+ acc_memcpy_t
-00001aa0: 6f5f 6465 7669 6365 5f61 7379 6e63 9473  o_device_async.s
-00001ab0: 8794 5294 6874 6879 297d 9468 7b8c 182b  ..R.hthy)}.h{..+
-00001ac0: 2061 6363 5f6d 656d 6370 795f 6672 6f6d   acc_memcpy_from
-00001ad0: 5f64 6576 6963 6594 7387 9452 9468 7468  _device.s..R.hth
-00001ae0: 7929 7d94 687b 8c1e 2b20 6163 635f 6d65  y)}.h{..+ acc_me
-00001af0: 6d63 7079 5f66 726f 6d5f 6465 7669 6365  mcpy_from_device
-00001b00: 5f61 7379 6e63 9473 8794 5294 6874 6879  _async.s..R.hthy
-00001b10: 297d 9468 7b8c 132b 2061 6363 5f6d 656d  )}.h{..+ acc_mem
-00001b20: 6370 795f 6465 7669 6365 9473 8794 5294  cpy_device.s..R.
-00001b30: 6874 6879 297d 9468 7b8c 192b 2061 6363  hthy)}.h{..+ acc
-00001b40: 5f6d 656d 6370 795f 6465 7669 6365 5f61  _memcpy_device_a
-00001b50: 7379 6e63 9473 8794 5294 6874 6879 297d  sync.s..R.hthy)}
-00001b60: 9468 7b8c 012b 9473 8794 5294 6874 6879  .h{..+.s..R.hthy
-00001b70: 297d 9468 7b8c 322d 2064 6174 6120 6d6f  )}.h{.2- data mo
-00001b80: 7665 6d65 6e74 2072 6f75 7469 6e65 7320  vement routines 
-00001b90: 2864 6f20 7765 2072 6561 6c6c 7920 6e65  (do we really ne
-00001ba0: 6564 2074 6865 6d3f 2994 7387 9452 9468  ed them?).s..R.h
-00001bb0: 7468 7929 7d94 687b 8c3c 2e2e 2e2e 2e2e  thy)}.h{.<......
+00001670: 2e2e 2e2e 2e2e 2e94 4b4c 4b00 8794 5294  ........KLK...R.
+00001680: 658c 0c74 7970 655f 6967 6e6f 7265 7394  e..type_ignores.
+00001690: 5d94 8c06 6c69 6e65 6e6f 944b 018c 0a63  ]...lineno.K...c
+000016a0: 6f6c 5f6f 6666 7365 7494 4b01 7562 680a  ol_offset.K.ubh.
+000016b0: 8c0f 7079 6363 656c 2e61 7374 2e63 6f72  ..pyccel.ast.cor
+000016c0: 6594 8c06 4d6f 6475 6c65 9493 9429 8194  e...Module...)..
+000016d0: 4e7d 9428 8c05 5f6e 616d 6594 684d 8c06  N}.(.._name.hM..
+000016e0: 4173 4e61 6d65 9493 9429 8194 4e7d 9428  AsName...)..N}.(
+000016f0: 8c04 5f6f 626a 948c 076f 7065 6e61 6363  .._obj...openacc
+00001700: 948c 075f 7461 7267 6574 948c 1470 7963  ..._target...pyc
+00001710: 6365 6c2e 6173 742e 696e 7465 726e 616c  cel.ast.internal
+00001720: 7394 8c0c 5079 6363 656c 5379 6d62 6f6c  s...PyccelSymbol
+00001730: 9493 948c 076f 7065 6e61 6363 9485 9481  .....openacc....
+00001740: 944e 7d94 8c08 5f69 735f 7465 6d70 9489  .N}..._is_temp..
+00001750: 7386 9462 8c0b 5f75 7365 725f 6e6f 6465  s..b.._user_node
+00001760: 7394 5d94 6809 5d94 8c16 5f72 6563 7572  s.].h.]..._recur
+00001770: 7369 6f6e 5f69 6e5f 7072 6f67 7265 7373  sion_in_progress
+00001780: 9489 8c0f 5f70 7963 6365 6c5f 7374 6167  ...._pyccel_stag
+00001790: 696e 6794 8c09 7379 6e74 6163 7469 6394  ing...syntactic.
+000017a0: 7586 9462 8c0a 5f76 6172 6961 626c 6573  u..b.._variables
+000017b0: 9429 8c06 5f66 756e 6373 9429 8c0b 5f69  .).._funcs.).._i
+000017c0: 6e74 6572 6661 6365 7394 298c 085f 636c  nterfaces.).._cl
+000017d0: 6173 7365 7394 298c 085f 696d 706f 7274  asses.).._import
+000017e0: 7394 298c 0a5f 696e 6974 5f66 756e 6394  s.).._init_func.
+000017f0: 4e8c 0a5f 6672 6565 5f66 756e 6394 4e8c  N.._free_func.N.
+00001800: 085f 7072 6f67 7261 6d94 684d 8c05 6170  ._program.hM..ap
+00001810: 706c 7994 9394 684d 8c09 436f 6465 426c  ply...hM..CodeBl
+00001820: 6f63 6b94 9394 297d 9468 0f28 6873 684d  ock...)}.h.(hshM
+00001830: 8c07 436f 6d6d 656e 7494 9394 297d 948c  ..Comment...)}..
+00001840: 0474 6578 7494 8c1a 7079 6363 656c 2068  .text...pyccel h
+00001850: 6561 6465 7220 666f 7220 4f70 656e 4143  eader for OpenAC
+00001860: 432e 9473 8794 5294 6873 6878 297d 9468  C..s..R.hshx)}.h
+00001870: 7a8c 724f 7065 6e41 4343 2064 6972 6563  z.rOpenACC direc
+00001880: 7469 7665 7320 616e 6420 436f 6e73 7472  tives and Constr
+00001890: 7563 7473 2061 7265 2068 616e 646c 6564  ucts are handled
+000018a0: 2062 7920 7468 6520 7061 7273 6572 2028   by the parser (
+000018b0: 7365 6520 6f70 656e 6163 632e 7478 2920  see openacc.tx) 
+000018c0: 616e 6420 6172 6520 7061 7274 7320 6f66  and are parts of
+000018d0: 2074 6865 2050 7963 6365 6c20 6c61 6e67   the Pyccel lang
+000018e0: 7561 6765 2e94 7387 9452 9468 7368 7829  uage..s..R.hshx)
+000018f0: 7d94 687a 8c43 5765 206f 6e6c 7920 6c69  }.hz.CWe only li
+00001900: 7374 2068 6572 6520 7768 6174 2063 616e  st here what can
+00001910: 206e 6f74 2062 6520 6465 7363 7269 6265   not be describe
+00001920: 6420 696e 2074 6865 206f 7065 6e61 6363  d in the openacc
+00001930: 2067 7261 6d6d 6172 2e94 7387 9452 9468   grammar..s..R.h
+00001940: 7368 7829 7d94 687a 8c00 9473 8794 5294  shx)}.hz...s..R.
+00001950: 6873 6878 297d 9468 7a8c 4854 4f44 4f20  hshx)}.hz.HTODO 
+00001960: 2d20 6465 7669 6365 7479 7065 2069 7320  - devicetype is 
+00001970: 666f 7220 7468 6520 6d6f 6d65 6e74 2061  for the moment a
+00001980: 6e20 696e 7465 6765 722e 203d 3e20 6e65  n integer. => ne
+00001990: 6564 2074 6f20 6164 6420 7072 6563 6973  ed to add precis
+000019a0: 696f 6e94 7387 9452 9468 7368 7829 7d94  ion.s..R.hshx)}.
+000019b0: 687a 8c24 2d20 6368 616e 6765 202a 2074  hz.$- change * t
+000019c0: 6f20 685f 766f 6964 2a20 616e 6420 645f  o h_void* and d_
+000019d0: 766f 6964 2a20 696e 9473 8794 5294 6873  void* in.s..R.hs
+000019e0: 6878 297d 9468 7a8c 0e2b 2061 6363 5f6d  hx)}.hz..+ acc_m
+000019f0: 6170 5f64 6174 6194 7387 9452 9468 7368  ap_data.s..R.hsh
+00001a00: 7829 7d94 687a 8c10 2b20 6163 635f 756e  x)}.hz..+ acc_un
+00001a10: 6d61 705f 6461 7461 9473 8794 5294 6873  map_data.s..R.hs
+00001a20: 6878 297d 9468 7a8c 0f2b 2061 6363 5f64  hx)}.hz..+ acc_d
+00001a30: 6576 6963 6570 7472 9473 8794 5294 6873  eviceptr.s..R.hs
+00001a40: 6878 297d 9468 7a8c 0d2b 2061 6363 5f68  hx)}.hz..+ acc_h
+00001a50: 6f73 7470 7472 9473 8794 5294 6873 6878  ostptr.s..R.hshx
+00001a60: 297d 9468 7a8c 162b 2061 6363 5f6d 656d  )}.hz..+ acc_mem
+00001a70: 6370 795f 746f 5f64 6576 6963 6594 7387  cpy_to_device.s.
+00001a80: 9452 9468 7368 7829 7d94 687a 8c1c 2b20  .R.hshx)}.hz..+ 
+00001a90: 6163 635f 6d65 6d63 7079 5f74 6f5f 6465  acc_memcpy_to_de
+00001aa0: 7669 6365 5f61 7379 6e63 9473 8794 5294  vice_async.s..R.
+00001ab0: 6873 6878 297d 9468 7a8c 182b 2061 6363  hshx)}.hz..+ acc
+00001ac0: 5f6d 656d 6370 795f 6672 6f6d 5f64 6576  _memcpy_from_dev
+00001ad0: 6963 6594 7387 9452 9468 7368 7829 7d94  ice.s..R.hshx)}.
+00001ae0: 687a 8c1e 2b20 6163 635f 6d65 6d63 7079  hz..+ acc_memcpy
+00001af0: 5f66 726f 6d5f 6465 7669 6365 5f61 7379  _from_device_asy
+00001b00: 6e63 9473 8794 5294 6873 6878 297d 9468  nc.s..R.hshx)}.h
+00001b10: 7a8c 132b 2061 6363 5f6d 656d 6370 795f  z..+ acc_memcpy_
+00001b20: 6465 7669 6365 9473 8794 5294 6873 6878  device.s..R.hshx
+00001b30: 297d 9468 7a8c 192b 2061 6363 5f6d 656d  )}.hz..+ acc_mem
+00001b40: 6370 795f 6465 7669 6365 5f61 7379 6e63  cpy_device_async
+00001b50: 9473 8794 5294 6873 6878 297d 9468 7a8c  .s..R.hshx)}.hz.
+00001b60: 012b 9473 8794 5294 6873 6878 297d 9468  .+.s..R.hshx)}.h
+00001b70: 7a8c 322d 2064 6174 6120 6d6f 7665 6d65  z.2- data moveme
+00001b80: 6e74 2072 6f75 7469 6e65 7320 2864 6f20  nt routines (do 
+00001b90: 7765 2072 6561 6c6c 7920 6e65 6564 2074  we really need t
+00001ba0: 6865 6d3f 2994 7387 9452 9468 7368 7829  hem?).s..R.hshx)
+00001bb0: 7d94 687a 8c3c 2e2e 2e2e 2e2e 2e2e 2e2e  }.hz.<..........
 00001bc0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001bd0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001be0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00001bf0: 2e2e 2e2e 2e2e 9473 8794 5294 6874 6879  .......s..R.hthy
-00001c00: 297d 9468 7b8c 2452 756e 7469 6d65 204c  )}.h{.$Runtime L
-00001c10: 6962 7261 7279 2052 6f75 7469 6e65 7320  ibrary Routines 
-00001c20: 666f 7220 466f 7274 7261 6e94 7387 9452  for Fortran.s..R
-00001c30: 9468 7468 7929 7d94 687b 8c3c 2e2e 2e2e  .hthy)}.h{.<....
+00001bf0: 2e2e 9473 8794 5294 6873 6878 297d 9468  ...s..R.hshx)}.h
+00001c00: 7a8c 2452 756e 7469 6d65 204c 6962 7261  z.$Runtime Libra
+00001c10: 7279 2052 6f75 7469 6e65 7320 666f 7220  ry Routines for 
+00001c20: 466f 7274 7261 6e94 7387 9452 9468 7368  Fortran.s..R.hsh
+00001c30: 7829 7d94 687a 8c3c 2e2e 2e2e 2e2e 2e2e  x)}.hz.<........
 00001c40: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001c50: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001c60: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00001c70: 2e2e 2e2e 2e2e 2e2e 9473 8794 5294 8c12  .........s..R...
-00001c80: 7079 6363 656c 2e61 7374 2e68 6561 6465  pyccel.ast.heade
-00001c90: 7273 948c 0e46 756e 6374 696f 6e48 6561  rs...FunctionHea
-00001ca0: 6465 7294 9394 288c 1361 6363 5f67 6574  der...(..acc_get
-00001cb0: 5f6e 756d 5f64 6576 6963 6573 945d 947d  _num_devices.].}
-00001cc0: 9428 8c08 6461 7461 7479 7065 948c 0369  .(..datatype...i
-00001cd0: 6e74 948c 0472 616e 6b94 4b00 8c0f 6d65  nt...rank.K...me
-00001ce0: 6d6f 7279 5f68 616e 646c 696e 6794 8c05  mory_handling...
-00001cf0: 7374 6163 6b94 8c09 7072 6563 6973 696f  stack...precisio
-00001d00: 6e94 4aff ffff ff8c 0769 735f 6675 6e63  n.J......is_func
-00001d10: 9489 8c08 6973 5f63 6f6e 7374 9489 7561  ....is_const..ua
-00001d20: 5d94 7d94 2868 d568 d668 d74b 0068 d868  ].}.(h.h.h.K.h.h
-00001d30: d968 da4a ffff ffff 68db 8968 dc89 7561  .h.J....h..h..ua
-00001d40: 8974 9452 9468 d128 8c13 6163 635f 7365  .t.R.h.(..acc_se
-00001d50: 745f 6465 7669 6365 5f74 7970 6594 5d94  t_device_type.].
-00001d60: 7d94 2868 d568 d668 d74b 0068 d868 d968  }.(h.h.h.K.h.h.h
-00001d70: da4a ffff ffff 68db 8968 dc89 7561 5d94  .J....h..h..ua].
-00001d80: 8974 9452 9468 d128 8c13 6163 635f 6765  .t.R.h.(..acc_ge
-00001d90: 745f 6465 7669 6365 5f74 7970 6594 5d94  t_device_type.].
-00001da0: 5d94 7d94 2868 d568 d668 d74b 0068 d868  ].}.(h.h.h.K.h.h
-00001db0: d968 da4a ffff ffff 68db 8968 dc89 7561  .h.J....h..h..ua
-00001dc0: 8974 9452 9468 d128 8c12 6163 635f 7365  .t.R.h.(..acc_se
-00001dd0: 745f 6465 7669 6365 5f6e 756d 945d 9428  t_device_num.].(
-00001de0: 7d94 2868 d568 d668 d74b 0068 d868 d968  }.(h.h.h.K.h.h.h
-00001df0: da4a ffff ffff 68db 8968 dc89 757d 9428  .J....h..h..u}.(
-00001e00: 68d5 68d6 68d7 4b00 68d8 68d9 68da 4aff  h.h.h.K.h.h.h.J.
-00001e10: ffff ff68 db89 68dc 8975 655d 9489 7494  ...h..h..ue]..t.
-00001e20: 5294 68d1 288c 1261 6363 5f67 6574 5f64  R.h.(..acc_get_d
-00001e30: 6576 6963 655f 6e75 6d94 5d94 7d94 2868  evice_num.].}.(h
-00001e40: d568 d668 d74b 0068 d868 d968 da4a ffff  .h.h.K.h.h.h.J..
-00001e50: ffff 68db 8968 dc89 7561 5d94 7d94 2868  ..h..h..ua].}.(h
-00001e60: d568 d668 d74b 0068 d868 d968 da4a ffff  .h.h.K.h.h.h.J..
-00001e70: ffff 68db 8968 dc89 7561 8974 9452 9468  ..h..h..ua.t.R.h
-00001e80: d128 8c08 6163 635f 696e 6974 945d 947d  .(..acc_init.].}
-00001e90: 9428 68d5 68d6 68d7 4b00 68d8 68d9 68da  .(h.h.h.K.h.h.h.
-00001ea0: 4aff ffff ff68 db89 68dc 8975 615d 9489  J....h..h..ua]..
-00001eb0: 7494 5294 68d1 288c 0c61 6363 5f73 6875  t.R.h.(..acc_shu
-00001ec0: 7464 6f77 6e94 5d94 7d94 2868 d568 d668  tdown.].}.(h.h.h
-00001ed0: d74b 0068 d868 d968 da4a ffff ffff 68db  .K.h.h.h.J....h.
-00001ee0: 8968 dc89 7561 5d94 8974 9452 9468 d128  .h..ua]..t.R.h.(
-00001ef0: 8c0e 6163 635f 6173 796e 635f 7465 7374  ..acc_async_test
-00001f00: 945d 947d 9428 68d5 8c04 626f 6f6c 9468  .].}.(h...bool.h
-00001f10: d74b 0068 d868 d968 da4a ffff ffff 68db  .K.h.h.h.J....h.
-00001f20: 8968 dc89 7561 5d94 7d94 2868 d56a 0a01  .h..ua].}.(h.j..
-00001f30: 0000 68d7 4b00 68d8 68d9 68da 4aff ffff  ..h.K.h.h.h.J...
-00001f40: ff68 db89 68dc 8975 6189 7494 5294 68d1  .h..h..ua.t.R.h.
-00001f50: 288c 1261 6363 5f61 7379 6e63 5f74 6573  (..acc_async_tes
-00001f60: 745f 616c 6c94 5d94 5d94 7d94 2868 d56a  t_all.].].}.(h.j
-00001f70: 0a01 0000 68d7 4b00 68d8 68d9 68da 4aff  ....h.K.h.h.h.J.
-00001f80: ffff ff68 db89 68dc 8975 6189 7494 5294  ...h..h..ua.t.R.
-00001f90: 68d1 288c 0861 6363 5f77 6169 7494 5d94  h.(..acc_wait.].
-00001fa0: 7d94 2868 d56a 0a01 0000 68d7 4b00 68d8  }.(h.j....h.K.h.
-00001fb0: 68d9 68da 4aff ffff ff68 db89 68dc 8975  h.h.J....h..h..u
-00001fc0: 615d 9489 7494 5294 68d1 288c 0c61 6363  a]..t.R.h.(..acc
-00001fd0: 5f77 6169 745f 616c 6c94 5d94 7d94 2868  _wait_all.].}.(h
-00001fe0: d56a 0a01 0000 68d7 4b00 68d8 68d9 68da  .j....h.K.h.h.h.
-00001ff0: 4aff ffff ff68 db89 68dc 8975 615d 9489  J....h..h..ua]..
-00002000: 7494 5294 68d1 288c 0e61 6363 5f77 6169  t.R.h.(..acc_wai
-00002010: 745f 6173 796e 6394 5d94 287d 9428 68d5  t_async.].(}.(h.
-00002020: 6a0a 0100 0068 d74b 0068 d868 d968 da4a  j....h.K.h.h.h.J
-00002030: ffff ffff 68db 8968 dc89 757d 9428 68d5  ....h..h..u}.(h.
-00002040: 6a0a 0100 0068 d74b 0068 d868 d968 da4a  j....h.K.h.h.h.J
-00002050: ffff ffff 68db 8968 dc89 7565 5d94 8974  ....h..h..ue]..t
-00002060: 9452 9468 d128 8c12 6163 635f 7761 6974  .R.h.(..acc_wait
-00002070: 5f61 6c6c 5f61 7379 6e63 945d 945d 9489  _all_async.].]..
-00002080: 7494 5294 68d1 288c 1561 6363 5f67 6574  t.R.h.(..acc_get
-00002090: 5f64 6566 6175 6c74 5f61 7379 6e63 945d  _default_async.]
-000020a0: 945d 947d 9428 68d5 68d6 68d7 4b00 68d8  .].}.(h.h.h.K.h.
-000020b0: 68d9 68da 4aff ffff ff68 db89 68dc 8975  h.h.J....h..h..u
-000020c0: 6189 7494 5294 68d1 288c 1561 6363 5f73  a.t.R.h.(..acc_s
-000020d0: 6574 5f64 6566 6175 6c74 5f61 7379 6e63  et_default_async
-000020e0: 945d 945d 9489 7494 5294 68d1 288c 0d61  .].]..t.R.h.(..a
-000020f0: 6363 5f6f 6e5f 6465 7669 6365 945d 947d  cc_on_device.].}
-00002100: 9428 68d5 68d6 68d7 4b00 68d8 68d9 68da  .(h.h.h.K.h.h.h.
-00002110: 4aff ffff ff68 db89 68dc 8975 615d 9489  J....h..h..ua]..
-00002120: 7494 5294 6874 6879 297d 9468 7b68 8873  t.R.hthy)}.h{h.s
-00002130: 8794 5294 68d1 288c 0a61 6363 5f6d 616c  ..R.h.(..acc_mal
-00002140: 6c6f 6394 5d94 7d94 2868 d568 d668 d74b  loc.].}.(h.h.h.K
-00002150: 0068 d868 d968 da4a ffff ffff 68db 8968  .h.h.h.J....h..h
-00002160: dc89 7561 5d94 7d94 2868 d568 d668 d74b  ..ua].}.(h.h.h.K
-00002170: 0068 d868 d968 da4a ffff ffff 68db 8968  .h.h.h.J....h..h
-00002180: dc89 7561 8974 9452 9468 d128 8c08 6163  ..ua.t.R.h.(..ac
-00002190: 635f 6672 6565 945d 947d 9428 68d5 68d6  c_free.].}.(h.h.
-000021a0: 68d7 4b00 68d8 68d9 68da 4aff ffff ff68  h.K.h.h.h.J....h
-000021b0: db89 68dc 8975 615d 9489 7494 5294 68d1  ..h..ua]..t.R.h.
-000021c0: 288c 0c61 6363 5f6d 6170 5f64 6174 6194  (..acc_map_data.
-000021d0: 5d94 287d 9428 68d5 8c01 2a94 68d7 4b00  ].(}.(h...*.h.K.
-000021e0: 68d8 68d9 68da 4b00 68db 8968 dc89 757d  h.h.h.K.h..h..u}
-000021f0: 9428 68d5 6a51 0100 0068 d74b 0068 d868  .(h.jQ...h.K.h.h
-00002200: d968 da4b 0068 db89 68dc 8975 7d94 2868  .h.K.h..h..u}.(h
-00002210: d568 d668 d74b 0068 d868 d968 da4a ffff  .h.h.K.h.h.h.J..
-00002220: ffff 68db 8968 dc89 7565 5d94 8974 9452  ..h..h..ue]..t.R
-00002230: 9468 d128 8c0e 6163 635f 756e 6d61 705f  .h.(..acc_unmap_
-00002240: 6461 7461 945d 947d 9428 68d5 6a51 0100  data.].}.(h.jQ..
-00002250: 0068 d74b 0068 d868 d968 da4b 0068 db89  .h.K.h.h.h.K.h..
-00002260: 68dc 8975 615d 9489 7494 5294 68d1 288c  h..ua]..t.R.h.(.
-00002270: 0d61 6363 5f64 6576 6963 6570 7472 945d  .acc_deviceptr.]
-00002280: 947d 9428 68d5 6a51 0100 0068 d74b 0068  .}.(h.jQ...h.K.h
-00002290: d868 d968 da4b 0068 db89 68dc 8975 615d  .h.h.K.h..h..ua]
-000022a0: 947d 9428 68d5 68d6 68d7 4b00 68d8 68d9  .}.(h.h.h.K.h.h.
-000022b0: 68da 4aff ffff ff68 db89 68dc 8975 6189  h.J....h..h..ua.
-000022c0: 7494 5294 68d1 288c 0b61 6363 5f68 6f73  t.R.h.(..acc_hos
-000022d0: 7470 7472 945d 947d 9428 68d5 6a51 0100  tptr.].}.(h.jQ..
-000022e0: 0068 d74b 0068 d868 d968 da4b 0068 db89  .h.K.h.h.h.K.h..
-000022f0: 68dc 8975 615d 947d 9428 68d5 68d6 68d7  h..ua].}.(h.h.h.
-00002300: 4b00 68d8 68d9 68da 4aff ffff ff68 db89  K.h.h.h.J....h..
-00002310: 68dc 8975 6189 7494 5294 68d1 288c 1461  h..ua.t.R.h.(..a
-00002320: 6363 5f6d 656d 6370 795f 746f 5f64 6576  cc_memcpy_to_dev
-00002330: 6963 6594 5d94 287d 9428 68d5 6a51 0100  ice.].(}.(h.jQ..
-00002340: 0068 d74b 0068 d868 d968 da4b 0068 db89  .h.K.h.h.h.K.h..
-00002350: 68dc 8975 7d94 2868 d56a 5101 0000 68d7  h..u}.(h.jQ...h.
-00002360: 4b00 68d8 68d9 68da 4b00 68db 8968 dc89  K.h.h.h.K.h..h..
-00002370: 757d 9428 68d5 68d6 68d7 4b00 68d8 68d9  u}.(h.h.h.K.h.h.
-00002380: 68da 4aff ffff ff68 db89 68dc 8975 655d  h.J....h..h..ue]
-00002390: 9489 7494 5294 68d1 288c 1a61 6363 5f6d  ..t.R.h.(..acc_m
-000023a0: 656d 6370 795f 746f 5f64 6576 6963 655f  emcpy_to_device_
-000023b0: 6173 796e 6394 5d94 287d 9428 68d5 6a51  async.].(}.(h.jQ
-000023c0: 0100 0068 d74b 0068 d868 d968 da4b 0068  ...h.K.h.h.h.K.h
-000023d0: db89 68dc 8975 7d94 2868 d56a 5101 0000  ..h..u}.(h.jQ...
-000023e0: 68d7 4b00 68d8 68d9 68da 4b00 68db 8968  h.K.h.h.h.K.h..h
-000023f0: dc89 757d 9428 68d5 68d6 68d7 4b00 68d8  ..u}.(h.h.h.K.h.
-00002400: 68d9 68da 4aff ffff ff68 db89 68dc 8975  h.h.J....h..h..u
-00002410: 7d94 2868 d568 d668 d74b 0068 d868 d968  }.(h.h.h.K.h.h.h
-00002420: da4a ffff ffff 68db 8968 dc89 7565 5d94  .J....h..h..ue].
-00002430: 8974 9452 9468 d128 8c16 6163 635f 6d65  .t.R.h.(..acc_me
-00002440: 6d63 7079 5f66 726f 6d5f 6465 7669 6365  mcpy_from_device
-00002450: 945d 9428 7d94 2868 d56a 5101 0000 68d7  .].(}.(h.jQ...h.
-00002460: 4b00 68d8 68d9 68da 4b00 68db 8968 dc89  K.h.h.h.K.h..h..
-00002470: 757d 9428 68d5 6a51 0100 0068 d74b 0068  u}.(h.jQ...h.K.h
-00002480: d868 d968 da4b 0068 db89 68dc 8975 7d94  .h.h.K.h..h..u}.
-00002490: 2868 d568 d668 d74b 0068 d868 d968 da4a  (h.h.h.K.h.h.h.J
-000024a0: ffff ffff 68db 8968 dc89 7565 5d94 8974  ....h..h..ue]..t
-000024b0: 9452 9468 d128 8c1c 6163 635f 6d65 6d63  .R.h.(..acc_memc
-000024c0: 7079 5f66 726f 6d5f 6465 7669 6365 5f61  py_from_device_a
-000024d0: 7379 6e63 945d 9428 7d94 2868 d56a 5101  sync.].(}.(h.jQ.
-000024e0: 0000 68d7 4b00 68d8 68d9 68da 4b00 68db  ..h.K.h.h.h.K.h.
-000024f0: 8968 dc89 757d 9428 68d5 6a51 0100 0068  .h..u}.(h.jQ...h
-00002500: d74b 0068 d868 d968 da4b 0068 db89 68dc  .K.h.h.h.K.h..h.
-00002510: 8975 7d94 2868 d568 d668 d74b 0068 d868  .u}.(h.h.h.K.h.h
-00002520: d968 da4a ffff ffff 68db 8968 dc89 757d  .h.J....h..h..u}
-00002530: 9428 68d5 68d6 68d7 4b00 68d8 68d9 68da  .(h.h.h.K.h.h.h.
-00002540: 4aff ffff ff68 db89 68dc 8975 655d 9489  J....h..h..ue]..
-00002550: 7494 5294 68d1 288c 1161 6363 5f6d 656d  t.R.h.(..acc_mem
-00002560: 6370 795f 6465 7669 6365 945d 9428 7d94  cpy_device.].(}.
-00002570: 2868 d56a 5101 0000 68d7 4b00 68d8 68d9  (h.jQ...h.K.h.h.
-00002580: 68da 4b00 68db 8968 dc89 757d 9428 68d5  h.K.h..h..u}.(h.
-00002590: 6a51 0100 0068 d74b 0068 d868 d968 da4b  jQ...h.K.h.h.h.K
-000025a0: 0068 db89 68dc 8975 7d94 2868 d568 d668  .h..h..u}.(h.h.h
-000025b0: d74b 0068 d868 d968 da4a ffff ffff 68db  .K.h.h.h.J....h.
-000025c0: 8968 dc89 7565 5d94 8974 9452 9468 d128  .h..ue]..t.R.h.(
-000025d0: 8c17 6163 635f 6d65 6d63 7079 5f64 6576  ..acc_memcpy_dev
-000025e0: 6963 655f 6173 796e 6394 5d94 287d 9428  ice_async.].(}.(
-000025f0: 68d5 6a51 0100 0068 d74b 0068 d868 d968  h.jQ...h.K.h.h.h
-00002600: da4b 0068 db89 68dc 8975 7d94 2868 d56a  .K.h..h..u}.(h.j
-00002610: 5101 0000 68d7 4b00 68d8 68d9 68da 4b00  Q...h.K.h.h.h.K.
-00002620: 68db 8968 dc89 757d 9428 68d5 68d6 68d7  h..h..u}.(h.h.h.
-00002630: 4b00 68d8 68d9 68da 4aff ffff ff68 db89  K.h.h.h.J....h..
-00002640: 68dc 8975 7d94 2868 d568 d668 d74b 0068  h..u}.(h.h.h.K.h
-00002650: d868 d968 da4a ffff ffff 68db 8968 dc89  .h.h.J....h..h..
-00002660: 7565 5d94 8974 9452 9468 7468 7929 7d94  ue]..t.R.hthy)}.
-00002670: 687b 8c3c 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  h{.<............
-00002680: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00002690: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-000026a0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-000026b0: 9473 8794 5294 6874 6879 297d 9468 7b8c  .s..R.hthy)}.h{.
-000026c0: 3c2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  <...............
+00001c70: 2e2e 2e2e 9473 8794 5294 8c12 7079 6363  .....s..R...pycc
+00001c80: 656c 2e61 7374 2e68 6561 6465 7273 948c  el.ast.headers..
+00001c90: 0e46 756e 6374 696f 6e48 6561 6465 7294  .FunctionHeader.
+00001ca0: 9394 288c 1361 6363 5f67 6574 5f6e 756d  ..(..acc_get_num
+00001cb0: 5f64 6576 6963 6573 945d 947d 9428 8c08  _devices.].}.(..
+00001cc0: 6461 7461 7479 7065 948c 1470 7963 6365  datatype...pycce
+00001cd0: 6c2e 6173 742e 6461 7461 7479 7065 7394  l.ast.datatypes.
+00001ce0: 8c0d 4e61 7469 7665 496e 7465 6765 7294  ..NativeInteger.
+00001cf0: 9394 2952 948c 0472 616e 6b94 4b00 8c0f  ..)R...rank.K...
+00001d00: 6d65 6d6f 7279 5f68 616e 646c 696e 6794  memory_handling.
+00001d10: 8c05 7374 6163 6b94 8c09 7072 6563 6973  ..stack...precis
+00001d20: 696f 6e94 4aff ffff ff8c 0769 735f 6675  ion.J......is_fu
+00001d30: 6e63 9489 8c08 6973 5f63 6f6e 7374 9489  nc....is_const..
+00001d40: 7561 5d94 7d94 2868 d468 d868 d94b 0068  ua].}.(h.h.h.K.h
+00001d50: da68 db68 dc4a ffff ffff 68dd 8968 de89  .h.h.J....h..h..
+00001d60: 7561 8974 9452 9468 d028 8c13 6163 635f  ua.t.R.h.(..acc_
+00001d70: 7365 745f 6465 7669 6365 5f74 7970 6594  set_device_type.
+00001d80: 5d94 7d94 2868 d468 d868 d94b 0068 da68  ].}.(h.h.h.K.h.h
+00001d90: db68 dc4a ffff ffff 68dd 8968 de89 7561  .h.J....h..h..ua
+00001da0: 5d94 8974 9452 9468 d028 8c13 6163 635f  ]..t.R.h.(..acc_
+00001db0: 6765 745f 6465 7669 6365 5f74 7970 6594  get_device_type.
+00001dc0: 5d94 5d94 7d94 2868 d468 d868 d94b 0068  ].].}.(h.h.h.K.h
+00001dd0: da68 db68 dc4a ffff ffff 68dd 8968 de89  .h.h.J....h..h..
+00001de0: 7561 8974 9452 9468 d028 8c12 6163 635f  ua.t.R.h.(..acc_
+00001df0: 7365 745f 6465 7669 6365 5f6e 756d 945d  set_device_num.]
+00001e00: 9428 7d94 2868 d468 d868 d94b 0068 da68  .(}.(h.h.h.K.h.h
+00001e10: db68 dc4a ffff ffff 68dd 8968 de89 757d  .h.J....h..h..u}
+00001e20: 9428 68d4 68d8 68d9 4b00 68da 68db 68dc  .(h.h.h.K.h.h.h.
+00001e30: 4aff ffff ff68 dd89 68de 8975 655d 9489  J....h..h..ue]..
+00001e40: 7494 5294 68d0 288c 1261 6363 5f67 6574  t.R.h.(..acc_get
+00001e50: 5f64 6576 6963 655f 6e75 6d94 5d94 7d94  _device_num.].}.
+00001e60: 2868 d468 d868 d94b 0068 da68 db68 dc4a  (h.h.h.K.h.h.h.J
+00001e70: ffff ffff 68dd 8968 de89 7561 5d94 7d94  ....h..h..ua].}.
+00001e80: 2868 d468 d868 d94b 0068 da68 db68 dc4a  (h.h.h.K.h.h.h.J
+00001e90: ffff ffff 68dd 8968 de89 7561 8974 9452  ....h..h..ua.t.R
+00001ea0: 9468 d028 8c08 6163 635f 696e 6974 945d  .h.(..acc_init.]
+00001eb0: 947d 9428 68d4 68d8 68d9 4b00 68da 68db  .}.(h.h.h.K.h.h.
+00001ec0: 68dc 4aff ffff ff68 dd89 68de 8975 615d  h.J....h..h..ua]
+00001ed0: 9489 7494 5294 68d0 288c 0c61 6363 5f73  ..t.R.h.(..acc_s
+00001ee0: 6875 7464 6f77 6e94 5d94 7d94 2868 d468  hutdown.].}.(h.h
+00001ef0: d868 d94b 0068 da68 db68 dc4a ffff ffff  .h.K.h.h.h.J....
+00001f00: 68dd 8968 de89 7561 5d94 8974 9452 9468  h..h..ua]..t.R.h
+00001f10: d028 8c0e 6163 635f 6173 796e 635f 7465  .(..acc_async_te
+00001f20: 7374 945d 947d 9428 68d4 68d5 8c0a 4e61  st.].}.(h.h...Na
+00001f30: 7469 7665 426f 6f6c 9493 9429 5294 68d9  tiveBool...)R.h.
+00001f40: 4b00 68da 68db 68dc 4aff ffff ff68 dd89  K.h.h.h.J....h..
+00001f50: 68de 8975 615d 947d 9428 68d4 6a0e 0100  h..ua].}.(h.j...
+00001f60: 0068 d94b 0068 da68 db68 dc4a ffff ffff  .h.K.h.h.h.J....
+00001f70: 68dd 8968 de89 7561 8974 9452 9468 d028  h..h..ua.t.R.h.(
+00001f80: 8c12 6163 635f 6173 796e 635f 7465 7374  ..acc_async_test
+00001f90: 5f61 6c6c 945d 945d 947d 9428 68d4 6a0e  _all.].].}.(h.j.
+00001fa0: 0100 0068 d94b 0068 da68 db68 dc4a ffff  ...h.K.h.h.h.J..
+00001fb0: ffff 68dd 8968 de89 7561 8974 9452 9468  ..h..h..ua.t.R.h
+00001fc0: d028 8c08 6163 635f 7761 6974 945d 947d  .(..acc_wait.].}
+00001fd0: 9428 68d4 6a0e 0100 0068 d94b 0068 da68  .(h.j....h.K.h.h
+00001fe0: db68 dc4a ffff ffff 68dd 8968 de89 7561  .h.J....h..h..ua
+00001ff0: 5d94 8974 9452 9468 d028 8c0c 6163 635f  ]..t.R.h.(..acc_
+00002000: 7761 6974 5f61 6c6c 945d 947d 9428 68d4  wait_all.].}.(h.
+00002010: 6a0e 0100 0068 d94b 0068 da68 db68 dc4a  j....h.K.h.h.h.J
+00002020: ffff ffff 68dd 8968 de89 7561 5d94 8974  ....h..h..ua]..t
+00002030: 9452 9468 d028 8c0e 6163 635f 7761 6974  .R.h.(..acc_wait
+00002040: 5f61 7379 6e63 945d 9428 7d94 2868 d46a  _async.].(}.(h.j
+00002050: 0e01 0000 68d9 4b00 68da 68db 68dc 4aff  ....h.K.h.h.h.J.
+00002060: ffff ff68 dd89 68de 8975 7d94 2868 d46a  ...h..h..u}.(h.j
+00002070: 0e01 0000 68d9 4b00 68da 68db 68dc 4aff  ....h.K.h.h.h.J.
+00002080: ffff ff68 dd89 68de 8975 655d 9489 7494  ...h..h..ue]..t.
+00002090: 5294 68d0 288c 1261 6363 5f77 6169 745f  R.h.(..acc_wait_
+000020a0: 616c 6c5f 6173 796e 6394 5d94 5d94 8974  all_async.].]..t
+000020b0: 9452 9468 d028 8c15 6163 635f 6765 745f  .R.h.(..acc_get_
+000020c0: 6465 6661 756c 745f 6173 796e 6394 5d94  default_async.].
+000020d0: 5d94 7d94 2868 d468 d868 d94b 0068 da68  ].}.(h.h.h.K.h.h
+000020e0: db68 dc4a ffff ffff 68dd 8968 de89 7561  .h.J....h..h..ua
+000020f0: 8974 9452 9468 d028 8c15 6163 635f 7365  .t.R.h.(..acc_se
+00002100: 745f 6465 6661 756c 745f 6173 796e 6394  t_default_async.
+00002110: 5d94 5d94 8974 9452 9468 d028 8c0d 6163  ].]..t.R.h.(..ac
+00002120: 635f 6f6e 5f64 6576 6963 6594 5d94 7d94  c_on_device.].}.
+00002130: 2868 d468 d868 d94b 0068 da68 db68 dc4a  (h.h.h.K.h.h.h.J
+00002140: ffff ffff 68dd 8968 de89 7561 5d94 8974  ....h..h..ua]..t
+00002150: 9452 9468 7368 7829 7d94 687a 6887 7387  .R.hshx)}.hzh.s.
+00002160: 9452 9468 d028 8c0a 6163 635f 6d61 6c6c  .R.h.(..acc_mall
+00002170: 6f63 945d 947d 9428 68d4 68d8 68d9 4b00  oc.].}.(h.h.h.K.
+00002180: 68da 68db 68dc 4aff ffff ff68 dd89 68de  h.h.h.J....h..h.
+00002190: 8975 615d 947d 9428 68d4 68d8 68d9 4b00  .ua].}.(h.h.h.K.
+000021a0: 68da 68db 68dc 4aff ffff ff68 dd89 68de  h.h.h.J....h..h.
+000021b0: 8975 6189 7494 5294 68d0 288c 0861 6363  .ua.t.R.h.(..acc
+000021c0: 5f66 7265 6594 5d94 7d94 2868 d468 d868  _free.].}.(h.h.h
+000021d0: d94b 0068 da68 db68 dc4a ffff ffff 68dd  .K.h.h.h.J....h.
+000021e0: 8968 de89 7561 5d94 8974 9452 9468 d028  .h..ua]..t.R.h.(
+000021f0: 8c0c 6163 635f 6d61 705f 6461 7461 945d  ..acc_map_data.]
+00002200: 9428 7d94 2868 d468 d58c 0d4e 6174 6976  .(}.(h.h...Nativ
+00002210: 6547 656e 6572 6963 9493 9429 5294 68d9  eGeneric...)R.h.
+00002220: 4b00 68da 68db 68dc 4b00 68dd 8968 de89  K.h.h.h.K.h..h..
+00002230: 757d 9428 68d4 6a57 0100 0068 d94b 0068  u}.(h.jW...h.K.h
+00002240: da68 db68 dc4b 0068 dd89 68de 8975 7d94  .h.h.K.h..h..u}.
+00002250: 2868 d468 d868 d94b 0068 da68 db68 dc4a  (h.h.h.K.h.h.h.J
+00002260: ffff ffff 68dd 8968 de89 7565 5d94 8974  ....h..h..ue]..t
+00002270: 9452 9468 d028 8c0e 6163 635f 756e 6d61  .R.h.(..acc_unma
+00002280: 705f 6461 7461 945d 947d 9428 68d4 6a57  p_data.].}.(h.jW
+00002290: 0100 0068 d94b 0068 da68 db68 dc4b 0068  ...h.K.h.h.h.K.h
+000022a0: dd89 68de 8975 615d 9489 7494 5294 68d0  ..h..ua]..t.R.h.
+000022b0: 288c 0d61 6363 5f64 6576 6963 6570 7472  (..acc_deviceptr
+000022c0: 945d 947d 9428 68d4 6a57 0100 0068 d94b  .].}.(h.jW...h.K
+000022d0: 0068 da68 db68 dc4b 0068 dd89 68de 8975  .h.h.h.K.h..h..u
+000022e0: 615d 947d 9428 68d4 68d8 68d9 4b00 68da  a].}.(h.h.h.K.h.
+000022f0: 68db 68dc 4aff ffff ff68 dd89 68de 8975  h.h.J....h..h..u
+00002300: 6189 7494 5294 68d0 288c 0b61 6363 5f68  a.t.R.h.(..acc_h
+00002310: 6f73 7470 7472 945d 947d 9428 68d4 6a57  ostptr.].}.(h.jW
+00002320: 0100 0068 d94b 0068 da68 db68 dc4b 0068  ...h.K.h.h.h.K.h
+00002330: dd89 68de 8975 615d 947d 9428 68d4 68d8  ..h..ua].}.(h.h.
+00002340: 68d9 4b00 68da 68db 68dc 4aff ffff ff68  h.K.h.h.h.J....h
+00002350: dd89 68de 8975 6189 7494 5294 68d0 288c  ..h..ua.t.R.h.(.
+00002360: 1461 6363 5f6d 656d 6370 795f 746f 5f64  .acc_memcpy_to_d
+00002370: 6576 6963 6594 5d94 287d 9428 68d4 6a57  evice.].(}.(h.jW
+00002380: 0100 0068 d94b 0068 da68 db68 dc4b 0068  ...h.K.h.h.h.K.h
+00002390: dd89 68de 8975 7d94 2868 d46a 5701 0000  ..h..u}.(h.jW...
+000023a0: 68d9 4b00 68da 68db 68dc 4b00 68dd 8968  h.K.h.h.h.K.h..h
+000023b0: de89 757d 9428 68d4 68d8 68d9 4b00 68da  ..u}.(h.h.h.K.h.
+000023c0: 68db 68dc 4aff ffff ff68 dd89 68de 8975  h.h.J....h..h..u
+000023d0: 655d 9489 7494 5294 68d0 288c 1a61 6363  e]..t.R.h.(..acc
+000023e0: 5f6d 656d 6370 795f 746f 5f64 6576 6963  _memcpy_to_devic
+000023f0: 655f 6173 796e 6394 5d94 287d 9428 68d4  e_async.].(}.(h.
+00002400: 6a57 0100 0068 d94b 0068 da68 db68 dc4b  jW...h.K.h.h.h.K
+00002410: 0068 dd89 68de 8975 7d94 2868 d46a 5701  .h..h..u}.(h.jW.
+00002420: 0000 68d9 4b00 68da 68db 68dc 4b00 68dd  ..h.K.h.h.h.K.h.
+00002430: 8968 de89 757d 9428 68d4 68d8 68d9 4b00  .h..u}.(h.h.h.K.
+00002440: 68da 68db 68dc 4aff ffff ff68 dd89 68de  h.h.h.J....h..h.
+00002450: 8975 7d94 2868 d468 d868 d94b 0068 da68  .u}.(h.h.h.K.h.h
+00002460: db68 dc4a ffff ffff 68dd 8968 de89 7565  .h.J....h..h..ue
+00002470: 5d94 8974 9452 9468 d028 8c16 6163 635f  ]..t.R.h.(..acc_
+00002480: 6d65 6d63 7079 5f66 726f 6d5f 6465 7669  memcpy_from_devi
+00002490: 6365 945d 9428 7d94 2868 d46a 5701 0000  ce.].(}.(h.jW...
+000024a0: 68d9 4b00 68da 68db 68dc 4b00 68dd 8968  h.K.h.h.h.K.h..h
+000024b0: de89 757d 9428 68d4 6a57 0100 0068 d94b  ..u}.(h.jW...h.K
+000024c0: 0068 da68 db68 dc4b 0068 dd89 68de 8975  .h.h.h.K.h..h..u
+000024d0: 7d94 2868 d468 d868 d94b 0068 da68 db68  }.(h.h.h.K.h.h.h
+000024e0: dc4a ffff ffff 68dd 8968 de89 7565 5d94  .J....h..h..ue].
+000024f0: 8974 9452 9468 d028 8c1c 6163 635f 6d65  .t.R.h.(..acc_me
+00002500: 6d63 7079 5f66 726f 6d5f 6465 7669 6365  mcpy_from_device
+00002510: 5f61 7379 6e63 945d 9428 7d94 2868 d46a  _async.].(}.(h.j
+00002520: 5701 0000 68d9 4b00 68da 68db 68dc 4b00  W...h.K.h.h.h.K.
+00002530: 68dd 8968 de89 757d 9428 68d4 6a57 0100  h..h..u}.(h.jW..
+00002540: 0068 d94b 0068 da68 db68 dc4b 0068 dd89  .h.K.h.h.h.K.h..
+00002550: 68de 8975 7d94 2868 d468 d868 d94b 0068  h..u}.(h.h.h.K.h
+00002560: da68 db68 dc4a ffff ffff 68dd 8968 de89  .h.h.J....h..h..
+00002570: 757d 9428 68d4 68d8 68d9 4b00 68da 68db  u}.(h.h.h.K.h.h.
+00002580: 68dc 4aff ffff ff68 dd89 68de 8975 655d  h.J....h..h..ue]
+00002590: 9489 7494 5294 68d0 288c 1161 6363 5f6d  ..t.R.h.(..acc_m
+000025a0: 656d 6370 795f 6465 7669 6365 945d 9428  emcpy_device.].(
+000025b0: 7d94 2868 d46a 5701 0000 68d9 4b00 68da  }.(h.jW...h.K.h.
+000025c0: 68db 68dc 4b00 68dd 8968 de89 757d 9428  h.h.K.h..h..u}.(
+000025d0: 68d4 6a57 0100 0068 d94b 0068 da68 db68  h.jW...h.K.h.h.h
+000025e0: dc4b 0068 dd89 68de 8975 7d94 2868 d468  .K.h..h..u}.(h.h
+000025f0: d868 d94b 0068 da68 db68 dc4a ffff ffff  .h.K.h.h.h.J....
+00002600: 68dd 8968 de89 7565 5d94 8974 9452 9468  h..h..ue]..t.R.h
+00002610: d028 8c17 6163 635f 6d65 6d63 7079 5f64  .(..acc_memcpy_d
+00002620: 6576 6963 655f 6173 796e 6394 5d94 287d  evice_async.].(}
+00002630: 9428 68d4 6a57 0100 0068 d94b 0068 da68  .(h.jW...h.K.h.h
+00002640: db68 dc4b 0068 dd89 68de 8975 7d94 2868  .h.K.h..h..u}.(h
+00002650: d46a 5701 0000 68d9 4b00 68da 68db 68dc  .jW...h.K.h.h.h.
+00002660: 4b00 68dd 8968 de89 757d 9428 68d4 68d8  K.h..h..u}.(h.h.
+00002670: 68d9 4b00 68da 68db 68dc 4aff ffff ff68  h.K.h.h.h.J....h
+00002680: dd89 68de 8975 7d94 2868 d468 d868 d94b  ..h..u}.(h.h.h.K
+00002690: 0068 da68 db68 dc4a ffff ffff 68dd 8968  .h.h.h.J....h..h
+000026a0: de89 7565 5d94 8974 9452 9468 7368 7829  ..ue]..t.R.hshx)
+000026b0: 7d94 687a 8c3c 2e2e 2e2e 2e2e 2e2e 2e2e  }.hz.<..........
+000026c0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 000026d0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 000026e0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-000026f0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e94 7387  ..............s.
-00002700: 9452 9468 7468 7929 7d94 687b 8c16 4461  .R.hthy)}.h{..Da
-00002710: 7461 204d 6f76 656d 656e 7420 726f 7574  ta Movement rout
-00002720: 696e 6573 9473 8794 5294 6874 6879 297d  ines.s..R.hthy)}
-00002730: 9468 7b8c 3c2e 2e2e 2e2e 2e2e 2e2e 2e2e  .h{.<...........
-00002740: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00002750: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00002760: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00002770: 2e94 7387 9452 9468 7468 7929 7d94 687b  ..s..R.hthy)}.h{
-00002780: 8c3c 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  .<..............
+000026f0: 2e2e 9473 8794 5294 6873 6878 297d 9468  ...s..R.hshx)}.h
+00002700: 7a8c 3c2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  z.<.............
+00002710: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00002720: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00002730: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e94  ................
+00002740: 7387 9452 9468 7368 7829 7d94 687a 8c16  s..R.hshx)}.hz..
+00002750: 4461 7461 204d 6f76 656d 656e 7420 726f  Data Movement ro
+00002760: 7574 696e 6573 9473 8794 5294 6873 6878  utines.s..R.hshx
+00002770: 297d 9468 7a8c 3c2e 2e2e 2e2e 2e2e 2e2e  )}.hz.<.........
+00002780: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00002790: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 000027a0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-000027b0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 9473  ...............s
-000027c0: 8794 5294 7494 7387 9452 948c 0f5f 7661  ..R.t.s..R..._va
-000027d0: 7269 6162 6c65 5f69 6e69 7473 9429 8c14  riable_inits.)..
-000027e0: 5f69 6e74 6572 6e61 6c5f 6469 6374 696f  _internal_dictio
-000027f0: 6e61 7279 947d 948c 065f 7363 6f70 6594  nary.}..._scope.
-00002800: 8c13 7079 6363 656c 2e70 6172 7365 722e  ..pyccel.parser.
-00002810: 7363 6f70 6594 8c05 5363 6f70 6594 9394  scope...Scope...
-00002820: 2981 944e 7d94 2868 6f7d 9428 8c09 6675  )..N}.(ho}.(..fu
-00002830: 6e63 7469 6f6e 7394 7d94 8c09 7661 7269  nctions.}...vari
-00002840: 6162 6c65 7394 7d94 8c07 636c 6173 7365  ables.}...classe
-00002850: 7394 7d94 8c07 696d 706f 7274 7394 7d94  s.}...imports.}.
-00002860: 8c12 7379 6d62 6f6c 6963 5f66 756e 6374  ..symbolic_funct
-00002870: 696f 6e73 947d 948c 066d 6163 726f 7394  ions.}...macros.
-00002880: 7d94 8c09 7465 6d70 6c61 7465 7394 7d94  }...templates.}.
-00002890: 8c07 6865 6164 6572 7394 7d94 8c0a 6465  ..headers.}...de
-000028a0: 636f 7261 746f 7273 947d 948c 0e63 6c73  corators.}...cls
-000028b0: 5f63 6f6e 7374 7275 6374 7394 7d94 758c  _constructs.}.u.
-000028c0: 075f 6c6f 6361 6c73 947d 9428 6abf 0100  ._locals.}.(j...
-000028d0: 007d 946a c101 0000 7d94 6ac3 0100 007d  .}.j....}.j....}
-000028e0: 946a c501 0000 7d94 6ac7 0100 007d 946a  .j....}.j....}.j
-000028f0: c901 0000 7d94 6acb 0100 007d 946a cd01  ....}.j....}.j..
-00002900: 0000 7d94 6acf 0100 007d 946a d101 0000  ..}.j....}.j....
-00002910: 7d94 758c 0d5f 7061 7265 6e74 5f73 636f  }.u.._parent_sco
-00002920: 7065 944e 8c0c 5f73 6f6e 735f 7363 6f70  pe.N.._sons_scop
-00002930: 6573 947d 948c 085f 6973 5f6c 6f6f 7094  es.}..._is_loop.
-00002940: 898c 065f 6c6f 6f70 7394 5d94 8c14 5f74  ..._loops.]..._t
-00002950: 656d 706f 7261 7279 5f76 6172 6961 626c  emporary_variabl
-00002960: 6573 945d 948c 0d5f 7573 6564 5f73 796d  es.]..._used_sym
-00002970: 626f 6c73 947d 9468 6068 5d8c 076f 7065  bols.}.h`h]..ope
-00002980: 6e61 6363 9485 9481 944e 7d94 6862 8973  nacc.....N}.hb.s
-00002990: 8694 6273 8c0e 5f64 756d 6d79 5f63 6f75  ..bs.._dummy_cou
-000029a0: 6e74 6572 944b 008c 105f 6f72 6967 696e  nter.K..._origin
-000029b0: 616c 5f73 796d 626f 6c94 7d94 6aeb 0100  al_symbol.}.j...
-000029c0: 0068 6073 7586 9462 6864 5d94 6809 5d94  .h`su..bhd].h.].
-000029d0: 680d 6168 6789 6868 6869 7586 9462 8c09  h.ahg.hhhiu..b..
-000029e0: 5f66 696c 656e 616d 6594 8c3a 2f55 7365  _filename..:/Use
-000029f0: 7273 2f79 616d 616e 2f74 6d70 2f70 7963  rs/yaman/tmp/pyc
-00002a00: 6365 6c2f 7079 6363 656c 2f73 7464 6c69  cel/pyccel/stdli
-00002a10: 622f 696e 7465 726e 616c 2f6f 7065 6e61  b/internal/opena
-00002a20: 6363 2e70 7968 948c 095f 6d65 7461 7661  cc.pyh..._metava
-00002a30: 7273 947d 9428 8c0b 6d6f 6475 6c65 5f6e  rs.}.(..module_n
-00002a40: 616d 6594 8c07 6f70 656e 6163 6394 8c0e  ame...openacc...
-00002a50: 6d6f 6475 6c65 5f76 6572 7369 6f6e 948c  module_version..
-00002a60: 0332 2e35 948c 0473 6176 6594 888c 0865  .2.5...save....e
-00002a70: 7874 6572 6e61 6c94 8975 6ab8 0100 006a  xternal..uj....j
-00002a80: bc01 0000 8c0e 5f63 7572 7265 6e74 5f63  ......_current_c
-00002a90: 6c61 7373 944e 8c11 5f63 7572 7265 6e74  lass.N.._current
-00002aa0: 5f66 756e 6374 696f 6e94 4e8c 0c5f 7379  _function.N.._sy
-00002ab0: 6e74 6178 5f64 6f6e 6594 888c 0e5f 7365  ntax_done...._se
-00002ac0: 6d61 6e74 6963 5f64 6f6e 6594 898c 115f  mantic_done...._
-00002ad0: 6375 7272 656e 745f 6673 745f 6e6f 6465  current_fst_node
-00002ae0: 944e 8c09 5f62 6c6f 636b 696e 6794 898c  .N.._blocking...
-00002af0: 145f 6372 6561 7465 645f 6672 6f6d 5f70  ._created_from_p
-00002b00: 6963 6b6c 6594 898c 085f 636f 6e74 6578  ickle...._contex
-00002b10: 7494 5d94 8c0e 5f69 6e5f 6c68 735f 6173  t.]..._in_lhs_as
-00002b20: 7369 676e 9489 7562 8794 2e              sign..ub...
+000027b0: 2e2e 2e94 7387 9452 9468 7368 7829 7d94  ....s..R.hshx)}.
+000027c0: 687a 8c3c 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  hz.<............
+000027d0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+000027e0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+000027f0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00002800: 9473 8794 5294 7494 7387 9452 948c 0f5f  .s..R.t.s..R..._
+00002810: 7661 7269 6162 6c65 5f69 6e69 7473 9429  variable_inits.)
+00002820: 8c14 5f69 6e74 6572 6e61 6c5f 6469 6374  .._internal_dict
+00002830: 696f 6e61 7279 947d 948c 065f 7363 6f70  ionary.}..._scop
+00002840: 6594 8c13 7079 6363 656c 2e70 6172 7365  e...pyccel.parse
+00002850: 722e 7363 6f70 6594 8c05 5363 6f70 6594  r.scope...Scope.
+00002860: 9394 2981 944e 7d94 2868 6e7d 9428 8c09  ..)..N}.(hn}.(..
+00002870: 6675 6e63 7469 6f6e 7394 7d94 8c09 7661  functions.}...va
+00002880: 7269 6162 6c65 7394 7d94 8c07 636c 6173  riables.}...clas
+00002890: 7365 7394 7d94 8c07 696d 706f 7274 7394  ses.}...imports.
+000028a0: 7d94 8c12 7379 6d62 6f6c 6963 5f66 756e  }...symbolic_fun
+000028b0: 6374 696f 6e73 947d 948c 066d 6163 726f  ctions.}...macro
+000028c0: 7394 7d94 8c09 7465 6d70 6c61 7465 7394  s.}...templates.
+000028d0: 7d94 8c07 6865 6164 6572 7394 7d94 8c0a  }...headers.}...
+000028e0: 6465 636f 7261 746f 7273 947d 948c 0e63  decorators.}...c
+000028f0: 6c73 5f63 6f6e 7374 7275 6374 7394 7d94  ls_constructs.}.
+00002900: 758c 075f 6c6f 6361 6c73 947d 9428 6ac5  u.._locals.}.(j.
+00002910: 0100 007d 946a c701 0000 7d94 6ac9 0100  ...}.j....}.j...
+00002920: 007d 946a cb01 0000 7d94 6acd 0100 007d  .}.j....}.j....}
+00002930: 946a cf01 0000 7d94 6ad1 0100 007d 946a  .j....}.j....}.j
+00002940: d301 0000 7d94 6ad5 0100 007d 946a d701  ....}.j....}.j..
+00002950: 0000 7d94 758c 0d5f 7061 7265 6e74 5f73  ..}.u.._parent_s
+00002960: 636f 7065 944e 8c0c 5f73 6f6e 735f 7363  cope.N.._sons_sc
+00002970: 6f70 6573 947d 948c 085f 6973 5f6c 6f6f  opes.}..._is_loo
+00002980: 7094 898c 065f 6c6f 6f70 7394 5d94 8c14  p...._loops.]...
+00002990: 5f74 656d 706f 7261 7279 5f76 6172 6961  _temporary_varia
+000029a0: 626c 6573 945d 948c 0d5f 7573 6564 5f73  bles.]..._used_s
+000029b0: 796d 626f 6c73 947d 9468 5f68 5c8c 076f  ymbols.}.h_h\..o
+000029c0: 7065 6e61 6363 9485 9481 944e 7d94 6861  penacc.....N}.ha
+000029d0: 8973 8694 6273 8c0e 5f64 756d 6d79 5f63  .s..bs.._dummy_c
+000029e0: 6f75 6e74 6572 944b 008c 105f 6f72 6967  ounter.K..._orig
+000029f0: 696e 616c 5f73 796d 626f 6c94 7d94 6af1  inal_symbol.}.j.
+00002a00: 0100 0068 5f73 7586 9462 6863 5d94 6809  ...h_su..bhc].h.
+00002a10: 5d94 680d 6168 6689 6867 6868 7586 9462  ].h.ahf.hghhu..b
+00002a20: 8c09 5f66 696c 656e 616d 6594 8c3c 2f68  .._filename..</h
+00002a30: 6f6d 652f 7961 6d61 6e67 7563 2f74 6d70  ome/yamanguc/tmp
+00002a40: 2f70 7963 6365 6c2f 7079 6363 656c 2f73  /pyccel/pyccel/s
+00002a50: 7464 6c69 622f 696e 7465 726e 616c 2f6f  tdlib/internal/o
+00002a60: 7065 6e61 6363 2e70 7968 948c 095f 6d65  penacc.pyh..._me
+00002a70: 7461 7661 7273 947d 9428 8c0b 6d6f 6475  tavars.}.(..modu
+00002a80: 6c65 5f6e 616d 6594 8c07 6f70 656e 6163  le_name...openac
+00002a90: 6394 8c0e 6d6f 6475 6c65 5f76 6572 7369  c...module_versi
+00002aa0: 6f6e 948c 0332 2e35 948c 0473 6176 6594  on...2.5...save.
+00002ab0: 888c 0865 7874 6572 6e61 6c94 8975 6abe  ...external..uj.
+00002ac0: 0100 006a c201 0000 8c0e 5f63 7572 7265  ...j......_curre
+00002ad0: 6e74 5f63 6c61 7373 944e 8c11 5f63 7572  nt_class.N.._cur
+00002ae0: 7265 6e74 5f66 756e 6374 696f 6e94 4e8c  rent_function.N.
+00002af0: 0c5f 7379 6e74 6178 5f64 6f6e 6594 888c  ._syntax_done...
+00002b00: 0e5f 7365 6d61 6e74 6963 5f64 6f6e 6594  ._semantic_done.
+00002b10: 898c 115f 6375 7272 656e 745f 6673 745f  ..._current_fst_
+00002b20: 6e6f 6465 944e 8c09 5f62 6c6f 636b 696e  node.N.._blockin
+00002b30: 6794 898c 145f 6372 6561 7465 645f 6672  g...._created_fr
+00002b40: 6f6d 5f70 6963 6b6c 6594 898c 085f 636f  om_pickle...._co
+00002b50: 6e74 6578 7494 5d94 8c0e 5f69 6e5f 6c68  ntext.]..._in_lh
+00002b60: 735f 6173 7369 676e 9489 7562 8794 2e    s_assign..ub...
```

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/openacc.pyh` & `pyccel-1.9.2/pyccel/stdlib/internal/openacc.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/openmp.py` & `pyccel-1.9.2/pyccel/stdlib/internal/openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/openmp.pyccel` & `pyccel-1.9.2/pyccel/stdlib/internal/openmp.pyccel`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-00000000: 8004 955c 2700 0000 0000 008c 2062 6331  ...\'....... bc1
+00000000: 8004 958d 2700 0000 0000 008c 2062 6331  ....'....... bc1
 00000010: 3734 3231 3738 6137 6338 3035 6261 3062  742178a7c805ba0b
 00000020: 3630 3738 3263 6466 3138 3933 3194 8c05  60782cdf18931...
-00000030: 312e 392e 3194 8c17 7079 6363 656c 2e70  1.9.1...pyccel.p
+00000030: 312e 392e 3294 8c17 7079 6363 656c 2e70  1.9.2...pyccel.p
 00000040: 6172 7365 722e 7379 6e74 6163 7469 6394  arser.syntactic.
 00000050: 8c0c 5379 6e74 6178 5061 7273 6572 9493  ..SyntaxParser..
 00000060: 9429 8194 7d94 288c 055f 636f 6465 9458  .)..}.(.._code.X
 00000070: 550a 0000 2320 7079 6363 656c 2068 6561  U...# pyccel hea
 00000080: 6465 7220 666f 7220 4f70 656e 4d50 2e0a  der for OpenMP..
 00000090: 2320 4f70 656e 4d50 2064 6972 6563 7469  # OpenMP directi
 000000a0: 7665 7320 616e 6420 436f 6e73 7472 7563  ves and Construc
@@ -167,465 +167,468 @@
 00000a60: 5f67 6574 5f6d 6178 5f74 6173 6b5f 7072  _get_max_task_pr
 00000a70: 696f 7269 7479 2829 2072 6573 756c 7473  iority() results
 00000a80: 2869 6e74 3332 2920 0a0a 2320 2e2e 2e2e  (int32) ..# ....
 00000a90: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000aa0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000ab0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000ac0: 2e2e 2e2e 2e2e 2e2e 0a94 8c04 5f66 7374  ............_fst
-00000ad0: 948c 0361 7374 948c 064d 6f64 756c 6594  ...ast...Module.
-00000ae0: 9394 2952 947d 9428 8c04 626f 6479 945d  ..)R.}.(..body.]
-00000af0: 9428 8c19 7079 6363 656c 2e70 6172 7365  .(..pyccel.parse
-00000b00: 722e 6578 7465 6e64 5f74 7265 6594 8c10  r.extend_tree...
-00000b10: 436f 6d6d 656e 744d 756c 7469 4c69 6e65  CommentMultiLine
-00000b20: 9493 948c d323 2070 7963 6365 6c20 6865  .....# pyccel he
-00000b30: 6164 6572 2066 6f72 204f 7065 6e4d 502e  ader for OpenMP.
-00000b40: 0a23 204f 7065 6e4d 5020 6469 7265 6374  .# OpenMP direct
-00000b50: 6976 6573 2061 6e64 2043 6f6e 7374 7275  ives and Constru
-00000b60: 6374 7320 6172 6520 6861 6e64 6c65 6420  cts are handled 
-00000b70: 6279 2074 6865 2070 6172 7365 7220 2873  by the parser (s
-00000b80: 6565 206f 7065 6e6d 702e 7478 2920 616e  ee openmp.tx) an
-00000b90: 6420 6172 6520 7061 7274 7320 6f66 2074  d are parts of t
-00000ba0: 6865 2050 7963 6365 6c20 6c61 6e67 7561  he Pyccel langua
-00000bb0: 6765 2e0a 2320 5765 206f 6e6c 7920 6c69  ge..# We only li
-00000bc0: 7374 2068 6572 6520 7768 6174 2063 616e  st here what can
-00000bd0: 206e 6f74 2062 6520 6465 7363 7269 6265   not be describe
-00000be0: 6420 696e 2074 6865 206f 7065 6e6d 7020  d in the openmp 
-00000bf0: 6772 616d 6d61 722e 944b 014b 0087 9452  grammar..K.K...R
-00000c00: 9468 138c b023 2420 6865 6164 6572 206d  .h...#$ header m
-00000c10: 6574 6176 6172 206d 6f64 756c 655f 6e61  etavar module_na
-00000c20: 6d65 203d 2027 6f6d 705f 6c69 6227 0a23  me = 'omp_lib'.#
-00000c30: 2420 6865 6164 6572 206d 6574 6176 6172  $ header metavar
-00000c40: 206d 6f64 756c 655f 7665 7273 696f 6e20   module_version 
-00000c50: 3d20 2734 2e35 270a 2324 2068 6561 6465  = '4.5'.#$ heade
-00000c60: 7220 6d65 7461 7661 7220 7361 7665 3d54  r metavar save=T
-00000c70: 7275 650a 2324 2068 6561 6465 7220 6d65  rue.#$ header me
-00000c80: 7461 7661 7220 6e6f 5f74 6172 6765 743d  tavar no_target=
-00000c90: 5472 7565 0a23 2420 6865 6164 6572 206d  True.#$ header m
-00000ca0: 6574 6176 6172 2065 7874 6572 6e61 6c3d  etavar external=
-00000cb0: 4661 6c73 6594 4b05 4b00 8794 5294 6813  False.K.K...R.h.
-00000cc0: 8caf 2320 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ..# ............
+00000ad0: 948c 045f 6173 7494 8c06 4d6f 6475 6c65  ..._ast...Module
+00000ae0: 9493 9429 5294 7d94 288c 0462 6f64 7994  ...)R.}.(..body.
+00000af0: 5d94 288c 1970 7963 6365 6c2e 7061 7273  ].(..pyccel.pars
+00000b00: 6572 2e65 7874 656e 645f 7472 6565 948c  er.extend_tree..
+00000b10: 1043 6f6d 6d65 6e74 4d75 6c74 694c 696e  .CommentMultiLin
+00000b20: 6594 9394 8cd3 2320 7079 6363 656c 2068  e.....# pyccel h
+00000b30: 6561 6465 7220 666f 7220 4f70 656e 4d50  eader for OpenMP
+00000b40: 2e0a 2320 4f70 656e 4d50 2064 6972 6563  ..# OpenMP direc
+00000b50: 7469 7665 7320 616e 6420 436f 6e73 7472  tives and Constr
+00000b60: 7563 7473 2061 7265 2068 616e 646c 6564  ucts are handled
+00000b70: 2062 7920 7468 6520 7061 7273 6572 2028   by the parser (
+00000b80: 7365 6520 6f70 656e 6d70 2e74 7829 2061  see openmp.tx) a
+00000b90: 6e64 2061 7265 2070 6172 7473 206f 6620  nd are parts of 
+00000ba0: 7468 6520 5079 6363 656c 206c 616e 6775  the Pyccel langu
+00000bb0: 6167 652e 0a23 2057 6520 6f6e 6c79 206c  age..# We only l
+00000bc0: 6973 7420 6865 7265 2077 6861 7420 6361  ist here what ca
+00000bd0: 6e20 6e6f 7420 6265 2064 6573 6372 6962  n not be describ
+00000be0: 6564 2069 6e20 7468 6520 6f70 656e 6d70  ed in the openmp
+00000bf0: 2067 7261 6d6d 6172 2e94 4b01 4b00 8794   grammar..K.K...
+00000c00: 5294 6813 8cb0 2324 2068 6561 6465 7220  R.h...#$ header 
+00000c10: 6d65 7461 7661 7220 6d6f 6475 6c65 5f6e  metavar module_n
+00000c20: 616d 6520 3d20 276f 6d70 5f6c 6962 270a  ame = 'omp_lib'.
+00000c30: 2324 2068 6561 6465 7220 6d65 7461 7661  #$ header metava
+00000c40: 7220 6d6f 6475 6c65 5f76 6572 7369 6f6e  r module_version
+00000c50: 203d 2027 342e 3527 0a23 2420 6865 6164   = '4.5'.#$ head
+00000c60: 6572 206d 6574 6176 6172 2073 6176 653d  er metavar save=
+00000c70: 5472 7565 0a23 2420 6865 6164 6572 206d  True.#$ header m
+00000c80: 6574 6176 6172 206e 6f5f 7461 7267 6574  etavar no_target
+00000c90: 3d54 7275 650a 2324 2068 6561 6465 7220  =True.#$ header 
+00000ca0: 6d65 7461 7661 7220 6578 7465 726e 616c  metavar external
+00000cb0: 3d46 616c 7365 944b 054b 0087 9452 9468  =False.K.K...R.h
+00000cc0: 138c af23 202e 2e2e 2e2e 2e2e 2e2e 2e2e  ...# ...........
 00000cd0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000ce0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000cf0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000d00: 0a23 2020 2020 2020 2020 2020 2020 5275  .#            Ru
-00000d10: 6e74 696d 6520 4c69 6272 6172 7920 526f  ntime Library Ro
-00000d20: 7574 696e 6573 2066 6f72 2046 6f72 7472  utines for Fortr
-00000d30: 616e 0a23 202e 2e2e 2e2e 2e2e 2e2e 2e2e  an.# ...........
+00000d00: 2e0a 2320 2020 2020 2020 2020 2020 2052  ..#            R
+00000d10: 756e 7469 6d65 204c 6962 7261 7279 2052  untime Library R
+00000d20: 6f75 7469 6e65 7320 666f 7220 466f 7274  outines for Fort
+00000d30: 7261 6e0a 2320 2e2e 2e2e 2e2e 2e2e 2e2e  ran.# ..........
 00000d40: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000d50: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00000d60: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00000d70: 2e94 4b0b 4b00 8794 5294 6813 8c65 2324  ..K.K...R.h..e#$
-00000d80: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
-00000d90: 206f 6d70 5f73 6574 5f6e 756d 5f74 6872   omp_set_num_thr
-00000da0: 6561 6473 2869 6e74 3332 290a 2324 2068  eads(int32).#$ h
-00000db0: 6561 6465 7220 6675 6e63 7469 6f6e 206f  eader function o
-00000dc0: 6d70 5f67 6574 5f6e 756d 5f74 6872 6561  mp_get_num_threa
-00000dd0: 6473 2829 2072 6573 756c 7473 2869 6e74  ds() results(int
-00000de0: 3332 2994 4b0f 4b00 8794 5294 6813 8cd7  32).K.K...R.h...
-00000df0: 2324 2068 6561 6465 7220 6675 6e63 7469  #$ header functi
-00000e00: 6f6e 206f 6d70 5f67 6574 5f6d 6178 5f74  on omp_get_max_t
-00000e10: 6872 6561 6473 2829 2072 6573 756c 7473  hreads() results
-00000e20: 2869 6e74 3332 290a 2324 2068 6561 6465  (int32).#$ heade
-00000e30: 7220 6675 6e63 7469 6f6e 206f 6d70 5f67  r function omp_g
-00000e40: 6574 5f74 6872 6561 645f 6e75 6d28 2920  et_thread_num() 
-00000e50: 7265 7375 6c74 7328 696e 7433 3229 0a23  results(int32).#
-00000e60: 2420 6865 6164 6572 2066 756e 6374 696f  $ header functio
-00000e70: 6e20 6f6d 705f 6765 745f 6e75 6d5f 7072  n omp_get_num_pr
-00000e80: 6f63 7328 2920 7265 7375 6c74 7328 696e  ocs() results(in
-00000e90: 7433 3229 0a23 2420 6865 6164 6572 2066  t32).#$ header f
-00000ea0: 756e 6374 696f 6e20 6f6d 705f 696e 5f70  unction omp_in_p
-00000eb0: 6172 616c 6c65 6c28 2920 7265 7375 6c74  arallel() result
-00000ec0: 7328 626f 6f6c 2994 4b12 4b00 8794 5294  s(bool).K.K...R.
-00000ed0: 6813 8c5f 2324 2068 6561 6465 7220 6675  h.._#$ header fu
-00000ee0: 6e63 7469 6f6e 206f 6d70 5f73 6574 5f64  nction omp_set_d
-00000ef0: 796e 616d 6963 2862 6f6f 6c29 0a23 2420  ynamic(bool).#$ 
-00000f00: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
-00000f10: 6f6d 705f 6765 745f 6479 6e61 6d69 6328  omp_get_dynamic(
-00000f20: 2920 2020 2020 7265 7375 6c74 7328 626f  )     results(bo
-00000f30: 6f6c 2994 4b17 4b00 8794 5294 6811 8c0b  ol).K.K...R.h...
-00000f40: 436f 6d6d 656e 744c 696e 6594 9394 8c37  CommentLine....7
-00000f50: 2324 2068 6561 6465 7220 6675 6e63 7469  #$ header functi
-00000f60: 6f6e 206f 6d70 5f67 6574 5f63 616e 6365  on omp_get_cance
-00000f70: 6c6c 6174 696f 6e28 2920 7265 7375 6c74  llation() result
-00000f80: 7328 626f 6f6c 2994 4b1a 4b00 8794 5294  s(bool).K.K...R.
-00000f90: 6813 8c59 2324 2068 6561 6465 7220 6675  h..Y#$ header fu
-00000fa0: 6e63 7469 6f6e 206f 6d70 5f73 6574 5f6e  nction omp_set_n
-00000fb0: 6573 7465 6428 626f 6f6c 290a 2324 2068  ested(bool).#$ h
-00000fc0: 6561 6465 7220 6675 6e63 7469 6f6e 206f  eader function o
-00000fd0: 6d70 5f67 6574 5f6e 6573 7465 6428 2920  mp_get_nested() 
-00000fe0: 7265 7375 6c74 7328 626f 6f6c 2994 4b1c  results(bool).K.
-00000ff0: 4b00 8794 5294 6813 8c6d 2324 2068 6561  K...R.h..m#$ hea
-00001000: 6465 7220 6675 6e63 7469 6f6e 206f 6d70  der function omp
-00001010: 5f73 6574 5f73 6368 6564 756c 6528 696e  _set_schedule(in
-00001020: 7433 322c 2069 6e74 3332 290a 2324 2068  t32, int32).#$ h
-00001030: 6561 6465 7220 6675 6e63 7469 6f6e 206f  eader function o
-00001040: 6d70 5f67 6574 5f73 6368 6564 756c 6528  mp_get_schedule(
-00001050: 2920 7265 7375 6c74 7328 696e 7433 322c  ) results(int32,
-00001060: 2069 6e74 3332 2994 4b1f 4b00 8794 5294   int32).K.K...R.
-00001070: 6813 8cdc 2324 2068 6561 6465 7220 6675  h...#$ header fu
-00001080: 6e63 7469 6f6e 206f 6d70 5f67 6574 5f74  nction omp_get_t
-00001090: 6872 6561 645f 6c69 6d69 7428 2920 7265  hread_limit() re
-000010a0: 7375 6c74 7328 696e 7433 3229 0a23 2420  sults(int32).#$ 
-000010b0: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
-000010c0: 6f6d 705f 7365 745f 6d61 785f 6163 7469  omp_set_max_acti
-000010d0: 7665 5f6c 6576 656c 7328 696e 7433 3229  ve_levels(int32)
-000010e0: 0a23 2420 6865 6164 6572 2066 756e 6374  .#$ header funct
-000010f0: 696f 6e20 6f6d 705f 6765 745f 6d61 785f  ion omp_get_max_
-00001100: 6163 7469 7665 5f6c 6576 656c 7328 2920  active_levels() 
-00001110: 7265 7375 6c74 7328 696e 7433 3229 0a23  results(int32).#
-00001120: 2420 6865 6164 6572 2066 756e 6374 696f  $ header functio
-00001130: 6e20 6f6d 705f 6765 745f 6c65 7665 6c28  n omp_get_level(
-00001140: 2920 7265 7375 6c74 7328 696e 7433 3229  ) results(int32)
-00001150: 944b 224b 0087 9452 9468 278c 4423 2420  .K"K...R.h'.D#$ 
-00001160: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
-00001170: 6f6d 705f 6765 745f 616e 6365 7374 6f72  omp_get_ancestor
-00001180: 5f74 6872 6561 645f 6e75 6d28 696e 7433  _thread_num(int3
-00001190: 3229 2072 6573 756c 7473 2869 6e74 3332  2) results(int32
-000011a0: 2994 4b27 4b00 8794 5294 6813 8cd9 2324  ).K'K...R.h...#$
-000011b0: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
-000011c0: 206f 6d70 5f67 6574 5f74 6561 6d5f 7369   omp_get_team_si
-000011d0: 7a65 2869 6e74 3332 2920 7265 7375 6c74  ze(int32) result
-000011e0: 7328 696e 7433 3229 0a23 2420 6865 6164  s(int32).#$ head
-000011f0: 6572 2066 756e 6374 696f 6e20 6f6d 705f  er function omp_
-00001200: 6765 745f 6163 7469 7665 5f6c 6576 656c  get_active_level
-00001210: 2829 2072 6573 756c 7473 2869 6e74 3332  () results(int32
-00001220: 290a 2324 2068 6561 6465 7220 6675 6e63  ).#$ header func
-00001230: 7469 6f6e 206f 6d70 5f69 6e5f 6669 6e61  tion omp_in_fina
-00001240: 6c28 2920 7265 7375 6c74 7328 626f 6f6c  l() results(bool
-00001250: 290a 2324 2068 6561 6465 7220 6675 6e63  ).#$ header func
-00001260: 7469 6f6e 206f 6d70 5f67 6574 5f70 726f  tion omp_get_pro
-00001270: 635f 6269 6e64 2829 2072 6573 756c 7473  c_bind() results
-00001280: 2869 6e74 3332 2994 4b29 4b00 8794 5294  (int32).K)K...R.
-00001290: 6813 5866 0100 0023 2420 6865 6164 6572  h.Xf...#$ header
-000012a0: 2066 756e 6374 696f 6e20 6f6d 705f 6765   function omp_ge
-000012b0: 745f 6e75 6d5f 706c 6163 6573 2829 2072  t_num_places() r
-000012c0: 6573 756c 7473 2869 6e74 3332 290a 2324  esults(int32).#$
-000012d0: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
-000012e0: 206f 6d70 5f67 6574 5f70 6c61 6365 5f6e   omp_get_place_n
-000012f0: 756d 5f70 726f 6373 2869 6e74 3332 2920  um_procs(int32) 
-00001300: 2072 6573 756c 7473 2869 6e74 3332 290a   results(int32).
-00001310: 2324 2068 6561 6465 7220 6675 6e63 7469  #$ header functi
-00001320: 6f6e 206f 6d70 5f67 6574 5f70 6c61 6365  on omp_get_place
-00001330: 5f70 726f 635f 6964 7328 696e 7433 322c  _proc_ids(int32,
-00001340: 2069 6e74 3332 205b 3a5d 290a 2324 2068   int32 [:]).#$ h
-00001350: 6561 6465 7220 6675 6e63 7469 6f6e 206f  eader function o
-00001360: 6d70 5f67 6574 5f70 6c61 6365 5f6e 756d  mp_get_place_num
-00001370: 2829 2072 6573 756c 7473 2869 6e74 3332  () results(int32
-00001380: 290a 2324 2068 6561 6465 7220 6675 6e63  ).#$ header func
-00001390: 7469 6f6e 206f 6d70 5f67 6574 5f70 6172  tion omp_get_par
-000013a0: 7469 7469 6f6e 5f6e 756d 5f70 6c61 6365  tition_num_place
-000013b0: 7328 2920 7265 7375 6c74 7328 696e 7433  s() results(int3
-000013c0: 3229 0a23 2420 6865 6164 6572 2066 756e  2).#$ header fun
-000013d0: 6374 696f 6e20 6f6d 705f 6765 745f 7061  ction omp_get_pa
-000013e0: 7274 6974 696f 6e5f 706c 6163 655f 6e75  rtition_place_nu
-000013f0: 6d73 2869 6e74 3332 205b 3a5d 2994 4b2e  ms(int32 [:]).K.
-00001400: 4b00 8794 5294 6813 8c6b 2324 2068 6561  K...R.h..k#$ hea
-00001410: 6465 7220 6675 6e63 7469 6f6e 206f 6d70  der function omp
-00001420: 5f73 6574 5f64 6566 6175 6c74 5f64 6576  _set_default_dev
-00001430: 6963 6528 696e 7433 3229 0a23 2420 6865  ice(int32).#$ he
-00001440: 6164 6572 2066 756e 6374 696f 6e20 6f6d  ader function om
-00001450: 705f 6765 745f 6465 6661 756c 745f 6465  p_get_default_de
-00001460: 7669 6365 2829 2072 6573 756c 7473 2869  vice() results(i
-00001470: 6e74 3332 2994 4b35 4b00 8794 5294 6827  nt32).K5K...R.h'
-00001480: 8c37 2324 2068 6561 6465 7220 6675 6e63  .7#$ header func
-00001490: 7469 6f6e 206f 6d70 5f67 6574 5f6e 756d  tion omp_get_num
-000014a0: 5f64 6576 6963 6573 2829 2072 6573 756c  _devices() resul
-000014b0: 7473 2869 6e74 3332 2994 4b38 4b00 8794  ts(int32).K8K...
-000014c0: 5294 6813 8c6a 2324 2068 6561 6465 7220  R.h..j#$ header 
-000014d0: 6675 6e63 7469 6f6e 206f 6d70 5f67 6574  function omp_get
-000014e0: 5f6e 756d 5f74 6561 6d73 2829 2072 6573  _num_teams() res
-000014f0: 756c 7473 2869 6e74 3332 290a 2324 2068  ults(int32).#$ h
-00001500: 6561 6465 7220 6675 6e63 7469 6f6e 206f  eader function o
-00001510: 6d70 5f67 6574 5f74 6561 6d5f 6e75 6d28  mp_get_team_num(
-00001520: 2920 7265 7375 6c74 7328 696e 7433 3229  ) results(int32)
-00001530: 944b 3a4b 0087 9452 9468 138c 7323 2420  .K:K...R.h..s#$ 
-00001540: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
-00001550: 6f6d 705f 6973 5f69 6e69 7469 616c 5f64  omp_is_initial_d
-00001560: 6576 6963 6528 2920 7265 7375 6c74 7328  evice() results(
-00001570: 626f 6f6c 290a 2324 2068 6561 6465 7220  bool).#$ header 
-00001580: 6675 6e63 7469 6f6e 206f 6d70 5f67 6574  function omp_get
-00001590: 5f69 6e69 7469 616c 5f64 6576 6963 6528  _initial_device(
-000015a0: 2920 7265 7375 6c74 7328 696e 7433 3229  ) results(int32)
-000015b0: 944b 3d4b 0087 9452 9468 278c 3d23 2420  .K=K...R.h'.=#$ 
-000015c0: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
-000015d0: 6f6d 705f 6765 745f 6d61 785f 7461 736b  omp_get_max_task
-000015e0: 5f70 7269 6f72 6974 7928 2920 7265 7375  _priority() resu
-000015f0: 6c74 7328 696e 7433 3229 944b 404b 0087  lts(int32).K@K..
-00001600: 9452 9468 278c 3e23 202e 2e2e 2e2e 2e2e  .R.h'.># .......
+00000d70: 2e2e 944b 0b4b 0087 9452 9468 138c 6523  ...K.K...R.h..e#
+00000d80: 2420 6865 6164 6572 2066 756e 6374 696f  $ header functio
+00000d90: 6e20 6f6d 705f 7365 745f 6e75 6d5f 7468  n omp_set_num_th
+00000da0: 7265 6164 7328 696e 7433 3229 0a23 2420  reads(int32).#$ 
+00000db0: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+00000dc0: 6f6d 705f 6765 745f 6e75 6d5f 7468 7265  omp_get_num_thre
+00000dd0: 6164 7328 2920 7265 7375 6c74 7328 696e  ads() results(in
+00000de0: 7433 3229 944b 0f4b 0087 9452 9468 138c  t32).K.K...R.h..
+00000df0: d723 2420 6865 6164 6572 2066 756e 6374  .#$ header funct
+00000e00: 696f 6e20 6f6d 705f 6765 745f 6d61 785f  ion omp_get_max_
+00000e10: 7468 7265 6164 7328 2920 7265 7375 6c74  threads() result
+00000e20: 7328 696e 7433 3229 0a23 2420 6865 6164  s(int32).#$ head
+00000e30: 6572 2066 756e 6374 696f 6e20 6f6d 705f  er function omp_
+00000e40: 6765 745f 7468 7265 6164 5f6e 756d 2829  get_thread_num()
+00000e50: 2072 6573 756c 7473 2869 6e74 3332 290a   results(int32).
+00000e60: 2324 2068 6561 6465 7220 6675 6e63 7469  #$ header functi
+00000e70: 6f6e 206f 6d70 5f67 6574 5f6e 756d 5f70  on omp_get_num_p
+00000e80: 726f 6373 2829 2072 6573 756c 7473 2869  rocs() results(i
+00000e90: 6e74 3332 290a 2324 2068 6561 6465 7220  nt32).#$ header 
+00000ea0: 6675 6e63 7469 6f6e 206f 6d70 5f69 6e5f  function omp_in_
+00000eb0: 7061 7261 6c6c 656c 2829 2072 6573 756c  parallel() resul
+00000ec0: 7473 2862 6f6f 6c29 944b 124b 0087 9452  ts(bool).K.K...R
+00000ed0: 9468 138c 5f23 2420 6865 6164 6572 2066  .h.._#$ header f
+00000ee0: 756e 6374 696f 6e20 6f6d 705f 7365 745f  unction omp_set_
+00000ef0: 6479 6e61 6d69 6328 626f 6f6c 290a 2324  dynamic(bool).#$
+00000f00: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
+00000f10: 206f 6d70 5f67 6574 5f64 796e 616d 6963   omp_get_dynamic
+00000f20: 2829 2020 2020 2072 6573 756c 7473 2862  ()     results(b
+00000f30: 6f6f 6c29 944b 174b 0087 9452 9468 118c  ool).K.K...R.h..
+00000f40: 0b43 6f6d 6d65 6e74 4c69 6e65 9493 948c  .CommentLine....
+00000f50: 3723 2420 6865 6164 6572 2066 756e 6374  7#$ header funct
+00000f60: 696f 6e20 6f6d 705f 6765 745f 6361 6e63  ion omp_get_canc
+00000f70: 656c 6c61 7469 6f6e 2829 2072 6573 756c  ellation() resul
+00000f80: 7473 2862 6f6f 6c29 944b 1a4b 0087 9452  ts(bool).K.K...R
+00000f90: 9468 138c 5923 2420 6865 6164 6572 2066  .h..Y#$ header f
+00000fa0: 756e 6374 696f 6e20 6f6d 705f 7365 745f  unction omp_set_
+00000fb0: 6e65 7374 6564 2862 6f6f 6c29 0a23 2420  nested(bool).#$ 
+00000fc0: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+00000fd0: 6f6d 705f 6765 745f 6e65 7374 6564 2829  omp_get_nested()
+00000fe0: 2072 6573 756c 7473 2862 6f6f 6c29 944b   results(bool).K
+00000ff0: 1c4b 0087 9452 9468 138c 6d23 2420 6865  .K...R.h..m#$ he
+00001000: 6164 6572 2066 756e 6374 696f 6e20 6f6d  ader function om
+00001010: 705f 7365 745f 7363 6865 6475 6c65 2869  p_set_schedule(i
+00001020: 6e74 3332 2c20 696e 7433 3229 0a23 2420  nt32, int32).#$ 
+00001030: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+00001040: 6f6d 705f 6765 745f 7363 6865 6475 6c65  omp_get_schedule
+00001050: 2829 2072 6573 756c 7473 2869 6e74 3332  () results(int32
+00001060: 2c20 696e 7433 3229 944b 1f4b 0087 9452  , int32).K.K...R
+00001070: 9468 138c dc23 2420 6865 6164 6572 2066  .h...#$ header f
+00001080: 756e 6374 696f 6e20 6f6d 705f 6765 745f  unction omp_get_
+00001090: 7468 7265 6164 5f6c 696d 6974 2829 2072  thread_limit() r
+000010a0: 6573 756c 7473 2869 6e74 3332 290a 2324  esults(int32).#$
+000010b0: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
+000010c0: 206f 6d70 5f73 6574 5f6d 6178 5f61 6374   omp_set_max_act
+000010d0: 6976 655f 6c65 7665 6c73 2869 6e74 3332  ive_levels(int32
+000010e0: 290a 2324 2068 6561 6465 7220 6675 6e63  ).#$ header func
+000010f0: 7469 6f6e 206f 6d70 5f67 6574 5f6d 6178  tion omp_get_max
+00001100: 5f61 6374 6976 655f 6c65 7665 6c73 2829  _active_levels()
+00001110: 2072 6573 756c 7473 2869 6e74 3332 290a   results(int32).
+00001120: 2324 2068 6561 6465 7220 6675 6e63 7469  #$ header functi
+00001130: 6f6e 206f 6d70 5f67 6574 5f6c 6576 656c  on omp_get_level
+00001140: 2829 2072 6573 756c 7473 2869 6e74 3332  () results(int32
+00001150: 2994 4b22 4b00 8794 5294 6827 8c44 2324  ).K"K...R.h'.D#$
+00001160: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
+00001170: 206f 6d70 5f67 6574 5f61 6e63 6573 746f   omp_get_ancesto
+00001180: 725f 7468 7265 6164 5f6e 756d 2869 6e74  r_thread_num(int
+00001190: 3332 2920 7265 7375 6c74 7328 696e 7433  32) results(int3
+000011a0: 3229 944b 274b 0087 9452 9468 138c d923  2).K'K...R.h...#
+000011b0: 2420 6865 6164 6572 2066 756e 6374 696f  $ header functio
+000011c0: 6e20 6f6d 705f 6765 745f 7465 616d 5f73  n omp_get_team_s
+000011d0: 697a 6528 696e 7433 3229 2072 6573 756c  ize(int32) resul
+000011e0: 7473 2869 6e74 3332 290a 2324 2068 6561  ts(int32).#$ hea
+000011f0: 6465 7220 6675 6e63 7469 6f6e 206f 6d70  der function omp
+00001200: 5f67 6574 5f61 6374 6976 655f 6c65 7665  _get_active_leve
+00001210: 6c28 2920 7265 7375 6c74 7328 696e 7433  l() results(int3
+00001220: 3229 0a23 2420 6865 6164 6572 2066 756e  2).#$ header fun
+00001230: 6374 696f 6e20 6f6d 705f 696e 5f66 696e  ction omp_in_fin
+00001240: 616c 2829 2072 6573 756c 7473 2862 6f6f  al() results(boo
+00001250: 6c29 0a23 2420 6865 6164 6572 2066 756e  l).#$ header fun
+00001260: 6374 696f 6e20 6f6d 705f 6765 745f 7072  ction omp_get_pr
+00001270: 6f63 5f62 696e 6428 2920 7265 7375 6c74  oc_bind() result
+00001280: 7328 696e 7433 3229 944b 294b 0087 9452  s(int32).K)K...R
+00001290: 9468 1358 6601 0000 2324 2068 6561 6465  .h.Xf...#$ heade
+000012a0: 7220 6675 6e63 7469 6f6e 206f 6d70 5f67  r function omp_g
+000012b0: 6574 5f6e 756d 5f70 6c61 6365 7328 2920  et_num_places() 
+000012c0: 7265 7375 6c74 7328 696e 7433 3229 0a23  results(int32).#
+000012d0: 2420 6865 6164 6572 2066 756e 6374 696f  $ header functio
+000012e0: 6e20 6f6d 705f 6765 745f 706c 6163 655f  n omp_get_place_
+000012f0: 6e75 6d5f 7072 6f63 7328 696e 7433 3229  num_procs(int32)
+00001300: 2020 7265 7375 6c74 7328 696e 7433 3229    results(int32)
+00001310: 0a23 2420 6865 6164 6572 2066 756e 6374  .#$ header funct
+00001320: 696f 6e20 6f6d 705f 6765 745f 706c 6163  ion omp_get_plac
+00001330: 655f 7072 6f63 5f69 6473 2869 6e74 3332  e_proc_ids(int32
+00001340: 2c20 696e 7433 3220 5b3a 5d29 0a23 2420  , int32 [:]).#$ 
+00001350: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+00001360: 6f6d 705f 6765 745f 706c 6163 655f 6e75  omp_get_place_nu
+00001370: 6d28 2920 7265 7375 6c74 7328 696e 7433  m() results(int3
+00001380: 3229 0a23 2420 6865 6164 6572 2066 756e  2).#$ header fun
+00001390: 6374 696f 6e20 6f6d 705f 6765 745f 7061  ction omp_get_pa
+000013a0: 7274 6974 696f 6e5f 6e75 6d5f 706c 6163  rtition_num_plac
+000013b0: 6573 2829 2072 6573 756c 7473 2869 6e74  es() results(int
+000013c0: 3332 290a 2324 2068 6561 6465 7220 6675  32).#$ header fu
+000013d0: 6e63 7469 6f6e 206f 6d70 5f67 6574 5f70  nction omp_get_p
+000013e0: 6172 7469 7469 6f6e 5f70 6c61 6365 5f6e  artition_place_n
+000013f0: 756d 7328 696e 7433 3220 5b3a 5d29 944b  ums(int32 [:]).K
+00001400: 2e4b 0087 9452 9468 138c 6b23 2420 6865  .K...R.h..k#$ he
+00001410: 6164 6572 2066 756e 6374 696f 6e20 6f6d  ader function om
+00001420: 705f 7365 745f 6465 6661 756c 745f 6465  p_set_default_de
+00001430: 7669 6365 2869 6e74 3332 290a 2324 2068  vice(int32).#$ h
+00001440: 6561 6465 7220 6675 6e63 7469 6f6e 206f  eader function o
+00001450: 6d70 5f67 6574 5f64 6566 6175 6c74 5f64  mp_get_default_d
+00001460: 6576 6963 6528 2920 7265 7375 6c74 7328  evice() results(
+00001470: 696e 7433 3229 944b 354b 0087 9452 9468  int32).K5K...R.h
+00001480: 278c 3723 2420 6865 6164 6572 2066 756e  '.7#$ header fun
+00001490: 6374 696f 6e20 6f6d 705f 6765 745f 6e75  ction omp_get_nu
+000014a0: 6d5f 6465 7669 6365 7328 2920 7265 7375  m_devices() resu
+000014b0: 6c74 7328 696e 7433 3229 944b 384b 0087  lts(int32).K8K..
+000014c0: 9452 9468 138c 6a23 2420 6865 6164 6572  .R.h..j#$ header
+000014d0: 2066 756e 6374 696f 6e20 6f6d 705f 6765   function omp_ge
+000014e0: 745f 6e75 6d5f 7465 616d 7328 2920 7265  t_num_teams() re
+000014f0: 7375 6c74 7328 696e 7433 3229 0a23 2420  sults(int32).#$ 
+00001500: 6865 6164 6572 2066 756e 6374 696f 6e20  header function 
+00001510: 6f6d 705f 6765 745f 7465 616d 5f6e 756d  omp_get_team_num
+00001520: 2829 2072 6573 756c 7473 2869 6e74 3332  () results(int32
+00001530: 2994 4b3a 4b00 8794 5294 6813 8c73 2324  ).K:K...R.h..s#$
+00001540: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
+00001550: 206f 6d70 5f69 735f 696e 6974 6961 6c5f   omp_is_initial_
+00001560: 6465 7669 6365 2829 2072 6573 756c 7473  device() results
+00001570: 2862 6f6f 6c29 0a23 2420 6865 6164 6572  (bool).#$ header
+00001580: 2066 756e 6374 696f 6e20 6f6d 705f 6765   function omp_ge
+00001590: 745f 696e 6974 6961 6c5f 6465 7669 6365  t_initial_device
+000015a0: 2829 2072 6573 756c 7473 2869 6e74 3332  () results(int32
+000015b0: 2994 4b3d 4b00 8794 5294 6827 8c3d 2324  ).K=K...R.h'.=#$
+000015c0: 2068 6561 6465 7220 6675 6e63 7469 6f6e   header function
+000015d0: 206f 6d70 5f67 6574 5f6d 6178 5f74 6173   omp_get_max_tas
+000015e0: 6b5f 7072 696f 7269 7479 2829 2072 6573  k_priority() res
+000015f0: 756c 7473 2869 6e74 3332 2994 4b40 4b00  ults(int32).K@K.
+00001600: 8794 5294 6827 8c3e 2320 2e2e 2e2e 2e2e  ..R.h'.># ......
 00001610: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001620: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001630: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00001640: 2e2e 2e2e 2e94 4b42 4b00 8794 5294 658c  ......KBK...R.e.
-00001650: 0c74 7970 655f 6967 6e6f 7265 7394 5d94  .type_ignores.].
-00001660: 8c06 6c69 6e65 6e6f 944b 018c 0a63 6f6c  ..lineno.K...col
-00001670: 5f6f 6666 7365 7494 4b01 7562 8c04 5f61  _offset.K.ub.._a
-00001680: 7374 948c 0f70 7963 6365 6c2e 6173 742e  st...pyccel.ast.
-00001690: 636f 7265 948c 064d 6f64 756c 6594 9394  core...Module...
-000016a0: 2981 944e 7d94 288c 055f 6e61 6d65 9468  )..N}.(.._name.h
-000016b0: 548c 0641 734e 616d 6594 9394 2981 944e  T..AsName...)..N
-000016c0: 7d94 288c 045f 6f62 6a94 8c06 6f70 656e  }.(.._obj...open
-000016d0: 6d70 948c 075f 7461 7267 6574 948c 1470  mp..._target...p
-000016e0: 7963 6365 6c2e 6173 742e 696e 7465 726e  yccel.ast.intern
-000016f0: 616c 7394 8c0c 5079 6363 656c 5379 6d62  als...PyccelSymb
-00001700: 6f6c 9493 948c 066f 7065 6e6d 7094 8594  ol.....openmp...
-00001710: 8194 4e7d 948c 085f 6973 5f74 656d 7094  ..N}..._is_temp.
-00001720: 8973 8694 628c 0b5f 7573 6572 5f6e 6f64  .s..b.._user_nod
-00001730: 6573 945d 9468 095d 948c 165f 7265 6375  es.].h.]..._recu
-00001740: 7273 696f 6e5f 696e 5f70 726f 6772 6573  rsion_in_progres
-00001750: 7394 898c 0f5f 7079 6363 656c 5f73 7461  s...._pyccel_sta
-00001760: 6769 6e67 948c 0973 796e 7461 6374 6963  ging...syntactic
-00001770: 9475 8694 628c 0a5f 7661 7269 6162 6c65  .u..b.._variable
-00001780: 7394 298c 065f 6675 6e63 7394 298c 0b5f  s.).._funcs.).._
-00001790: 696e 7465 7266 6163 6573 9429 8c08 5f63  interfaces.).._c
-000017a0: 6c61 7373 6573 9429 8c08 5f69 6d70 6f72  lasses.).._impor
-000017b0: 7473 9429 8c0a 5f69 6e69 745f 6675 6e63  ts.).._init_func
-000017c0: 944e 8c0a 5f66 7265 655f 6675 6e63 944e  .N.._free_func.N
-000017d0: 8c08 5f70 726f 6772 616d 9468 548c 0561  .._program.hT..a
-000017e0: 7070 6c79 9493 9468 548c 0943 6f64 6542  pply...hT..CodeB
-000017f0: 6c6f 636b 9493 9429 7d94 680f 2868 7a68  lock...)}.h.(hzh
-00001800: 548c 0743 6f6d 6d65 6e74 9493 9429 7d94  T..Comment...)}.
-00001810: 8c04 7465 7874 948c 1970 7963 6365 6c20  ..text...pyccel 
-00001820: 6865 6164 6572 2066 6f72 204f 7065 6e4d  header for OpenM
-00001830: 502e 9473 8794 5294 687a 687f 297d 9468  P..s..R.hzh.)}.h
-00001840: 818c 704f 7065 6e4d 5020 6469 7265 6374  ..pOpenMP direct
-00001850: 6976 6573 2061 6e64 2043 6f6e 7374 7275  ives and Constru
-00001860: 6374 7320 6172 6520 6861 6e64 6c65 6420  cts are handled 
-00001870: 6279 2074 6865 2070 6172 7365 7220 2873  by the parser (s
-00001880: 6565 206f 7065 6e6d 702e 7478 2920 616e  ee openmp.tx) an
-00001890: 6420 6172 6520 7061 7274 7320 6f66 2074  d are parts of t
-000018a0: 6865 2050 7963 6365 6c20 6c61 6e67 7561  he Pyccel langua
-000018b0: 6765 2e94 7387 9452 9468 7a68 7f29 7d94  ge..s..R.hzh.)}.
-000018c0: 6881 8c42 5765 206f 6e6c 7920 6c69 7374  h..BWe only list
-000018d0: 2068 6572 6520 7768 6174 2063 616e 206e   here what can n
-000018e0: 6f74 2062 6520 6465 7363 7269 6265 6420  ot be described 
-000018f0: 696e 2074 6865 206f 7065 6e6d 7020 6772  in the openmp gr
-00001900: 616d 6d61 722e 9473 8794 5294 687a 687f  ammar..s..R.hzh.
-00001910: 297d 9468 818c 3c2e 2e2e 2e2e 2e2e 2e2e  )}.h..<.........
+00001640: 2e2e 2e2e 2e2e 944b 424b 0087 9452 9465  .......KBK...R.e
+00001650: 8c0c 7479 7065 5f69 676e 6f72 6573 945d  ..type_ignores.]
+00001660: 948c 066c 696e 656e 6f94 4b01 8c0a 636f  ...lineno.K...co
+00001670: 6c5f 6f66 6673 6574 944b 0175 6268 0a8c  l_offset.K.ubh..
+00001680: 0f70 7963 6365 6c2e 6173 742e 636f 7265  .pyccel.ast.core
+00001690: 948c 064d 6f64 756c 6594 9394 2981 944e  ...Module...)..N
+000016a0: 7d94 288c 055f 6e61 6d65 9468 538c 0641  }.(.._name.hS..A
+000016b0: 734e 616d 6594 9394 2981 944e 7d94 288c  sName...)..N}.(.
+000016c0: 045f 6f62 6a94 8c06 6f70 656e 6d70 948c  ._obj...openmp..
+000016d0: 075f 7461 7267 6574 948c 1470 7963 6365  ._target...pycce
+000016e0: 6c2e 6173 742e 696e 7465 726e 616c 7394  l.ast.internals.
+000016f0: 8c0c 5079 6363 656c 5379 6d62 6f6c 9493  ..PyccelSymbol..
+00001700: 948c 066f 7065 6e6d 7094 8594 8194 4e7d  ...openmp.....N}
+00001710: 948c 085f 6973 5f74 656d 7094 8973 8694  ..._is_temp..s..
+00001720: 628c 0b5f 7573 6572 5f6e 6f64 6573 945d  b.._user_nodes.]
+00001730: 9468 095d 948c 165f 7265 6375 7273 696f  .h.]..._recursio
+00001740: 6e5f 696e 5f70 726f 6772 6573 7394 898c  n_in_progress...
+00001750: 0f5f 7079 6363 656c 5f73 7461 6769 6e67  ._pyccel_staging
+00001760: 948c 0973 796e 7461 6374 6963 9475 8694  ...syntactic.u..
+00001770: 628c 0a5f 7661 7269 6162 6c65 7394 298c  b.._variables.).
+00001780: 065f 6675 6e63 7394 298c 0b5f 696e 7465  ._funcs.).._inte
+00001790: 7266 6163 6573 9429 8c08 5f63 6c61 7373  rfaces.).._class
+000017a0: 6573 9429 8c08 5f69 6d70 6f72 7473 9429  es.).._imports.)
+000017b0: 8c0a 5f69 6e69 745f 6675 6e63 944e 8c0a  .._init_func.N..
+000017c0: 5f66 7265 655f 6675 6e63 944e 8c08 5f70  _free_func.N.._p
+000017d0: 726f 6772 616d 9468 538c 0561 7070 6c79  rogram.hS..apply
+000017e0: 9493 9468 538c 0943 6f64 6542 6c6f 636b  ...hS..CodeBlock
+000017f0: 9493 9429 7d94 680f 2868 7968 538c 0743  ...)}.h.(hyhS..C
+00001800: 6f6d 6d65 6e74 9493 9429 7d94 8c04 7465  omment...)}...te
+00001810: 7874 948c 1970 7963 6365 6c20 6865 6164  xt...pyccel head
+00001820: 6572 2066 6f72 204f 7065 6e4d 502e 9473  er for OpenMP..s
+00001830: 8794 5294 6879 687e 297d 9468 808c 704f  ..R.hyh~)}.h..pO
+00001840: 7065 6e4d 5020 6469 7265 6374 6976 6573  penMP directives
+00001850: 2061 6e64 2043 6f6e 7374 7275 6374 7320   and Constructs 
+00001860: 6172 6520 6861 6e64 6c65 6420 6279 2074  are handled by t
+00001870: 6865 2070 6172 7365 7220 2873 6565 206f  he parser (see o
+00001880: 7065 6e6d 702e 7478 2920 616e 6420 6172  penmp.tx) and ar
+00001890: 6520 7061 7274 7320 6f66 2074 6865 2050  e parts of the P
+000018a0: 7963 6365 6c20 6c61 6e67 7561 6765 2e94  yccel language..
+000018b0: 7387 9452 9468 7968 7e29 7d94 6880 8c42  s..R.hyh~)}.h..B
+000018c0: 5765 206f 6e6c 7920 6c69 7374 2068 6572  We only list her
+000018d0: 6520 7768 6174 2063 616e 206e 6f74 2062  e what can not b
+000018e0: 6520 6465 7363 7269 6265 6420 696e 2074  e described in t
+000018f0: 6865 206f 7065 6e6d 7020 6772 616d 6d61  he openmp gramma
+00001900: 722e 9473 8794 5294 6879 687e 297d 9468  r..s..R.hyh~)}.h
+00001910: 808c 3c2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ..<.............
 00001920: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00001930: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00001940: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00001950: 2e2e 2e94 7387 9452 9468 7a68 7f29 7d94  ....s..R.hzh.)}.
-00001960: 6881 8c24 5275 6e74 696d 6520 4c69 6272  h..$Runtime Libr
-00001970: 6172 7920 526f 7574 696e 6573 2066 6f72  ary Routines for
-00001980: 2046 6f72 7472 616e 9473 8794 5294 687a   Fortran.s..R.hz
-00001990: 687f 297d 9468 818c 3c2e 2e2e 2e2e 2e2e  h.)}.h..<.......
+00001940: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e94  ................
+00001950: 7387 9452 9468 7968 7e29 7d94 6880 8c24  s..R.hyh~)}.h..$
+00001960: 5275 6e74 696d 6520 4c69 6272 6172 7920  Runtime Library 
+00001970: 526f 7574 696e 6573 2066 6f72 2046 6f72  Routines for For
+00001980: 7472 616e 9473 8794 5294 6879 687e 297d  tran.s..R.hyh~)}
+00001990: 9468 808c 3c2e 2e2e 2e2e 2e2e 2e2e 2e2e  .h..<...........
 000019a0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 000019b0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 000019c0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-000019d0: 2e2e 2e2e 2e94 7387 9452 948c 1270 7963  ......s..R...pyc
-000019e0: 6365 6c2e 6173 742e 6865 6164 6572 7394  cel.ast.headers.
-000019f0: 8c0e 4675 6e63 7469 6f6e 4865 6164 6572  ..FunctionHeader
-00001a00: 9493 9428 8c13 6f6d 705f 7365 745f 6e75  ...(..omp_set_nu
-00001a10: 6d5f 7468 7265 6164 7394 5d94 7d94 288c  m_threads.].}.(.
-00001a20: 0864 6174 6174 7970 6594 8c03 696e 7494  .datatype...int.
-00001a30: 8c04 7261 6e6b 944b 008c 0f6d 656d 6f72  ..rank.K...memor
-00001a40: 795f 6861 6e64 6c69 6e67 948c 0573 7461  y_handling...sta
-00001a50: 636b 948c 0970 7265 6369 7369 6f6e 944b  ck...precision.K
-00001a60: 048c 0769 735f 6675 6e63 9489 8c08 6973  ...is_func....is
-00001a70: 5f63 6f6e 7374 9489 7561 5d94 8974 9452  _const..ua]..t.R
-00001a80: 9468 9b28 8c13 6f6d 705f 6765 745f 6e75  .h.(..omp_get_nu
-00001a90: 6d5f 7468 7265 6164 7394 5d94 5d94 7d94  m_threads.].].}.
-00001aa0: 2868 9f68 a068 a14b 0068 a268 a368 a44b  (h.h.h.K.h.h.h.K
-00001ab0: 0468 a589 68a6 8975 6189 7494 5294 689b  .h..h..ua.t.R.h.
-00001ac0: 288c 136f 6d70 5f67 6574 5f6d 6178 5f74  (..omp_get_max_t
-00001ad0: 6872 6561 6473 945d 945d 947d 9428 689f  hreads.].].}.(h.
-00001ae0: 68a0 68a1 4b00 68a2 68a3 68a4 4b04 68a5  h.h.K.h.h.h.K.h.
-00001af0: 8968 a689 7561 8974 9452 9468 9b28 8c12  .h..ua.t.R.h.(..
-00001b00: 6f6d 705f 6765 745f 7468 7265 6164 5f6e  omp_get_thread_n
-00001b10: 756d 945d 945d 947d 9428 689f 68a0 68a1  um.].].}.(h.h.h.
-00001b20: 4b00 68a2 68a3 68a4 4b04 68a5 8968 a689  K.h.h.h.K.h..h..
-00001b30: 7561 8974 9452 9468 9b28 8c11 6f6d 705f  ua.t.R.h.(..omp_
-00001b40: 6765 745f 6e75 6d5f 7072 6f63 7394 5d94  get_num_procs.].
-00001b50: 5d94 7d94 2868 9f68 a068 a14b 0068 a268  ].}.(h.h.h.K.h.h
-00001b60: a368 a44b 0468 a589 68a6 8975 6189 7494  .h.K.h..h..ua.t.
-00001b70: 5294 689b 288c 0f6f 6d70 5f69 6e5f 7061  R.h.(..omp_in_pa
-00001b80: 7261 6c6c 656c 945d 945d 947d 9428 689f  rallel.].].}.(h.
-00001b90: 8c04 626f 6f6c 9468 a14b 0068 a268 a368  ..bool.h.K.h.h.h
-00001ba0: a44a ffff ffff 68a5 8968 a689 7561 8974  .J....h..h..ua.t
-00001bb0: 9452 9468 9b28 8c0f 6f6d 705f 7365 745f  .R.h.(..omp_set_
-00001bc0: 6479 6e61 6d69 6394 5d94 7d94 2868 9f68  dynamic.].}.(h.h
-00001bd0: c668 a14b 0068 a268 a368 a44a ffff ffff  .h.K.h.h.h.J....
-00001be0: 68a5 8968 a689 7561 5d94 8974 9452 9468  h..h..ua]..t.R.h
-00001bf0: 9b28 8c0f 6f6d 705f 6765 745f 6479 6e61  .(..omp_get_dyna
-00001c00: 6d69 6394 5d94 5d94 7d94 2868 9f68 c668  mic.].].}.(h.h.h
-00001c10: a14b 0068 a268 a368 a44a ffff ffff 68a5  .K.h.h.h.J....h.
-00001c20: 8968 a689 7561 8974 9452 9468 9b28 8c14  .h..ua.t.R.h.(..
-00001c30: 6f6d 705f 6765 745f 6361 6e63 656c 6c61  omp_get_cancella
-00001c40: 7469 6f6e 945d 945d 947d 9428 689f 68c6  tion.].].}.(h.h.
-00001c50: 68a1 4b00 68a2 68a3 68a4 4aff ffff ff68  h.K.h.h.h.J....h
-00001c60: a589 68a6 8975 6189 7494 5294 689b 288c  ..h..ua.t.R.h.(.
-00001c70: 0e6f 6d70 5f73 6574 5f6e 6573 7465 6494  .omp_set_nested.
-00001c80: 5d94 7d94 2868 9f68 c668 a14b 0068 a268  ].}.(h.h.h.K.h.h
-00001c90: a368 a44a ffff ffff 68a5 8968 a689 7561  .h.J....h..h..ua
-00001ca0: 5d94 8974 9452 9468 9b28 8c0e 6f6d 705f  ]..t.R.h.(..omp_
-00001cb0: 6765 745f 6e65 7374 6564 945d 945d 947d  get_nested.].].}
-00001cc0: 9428 689f 68c6 68a1 4b00 68a2 68a3 68a4  .(h.h.h.K.h.h.h.
-00001cd0: 4aff ffff ff68 a589 68a6 8975 6189 7494  J....h..h..ua.t.
-00001ce0: 5294 689b 288c 106f 6d70 5f73 6574 5f73  R.h.(..omp_set_s
-00001cf0: 6368 6564 756c 6594 5d94 287d 9428 689f  chedule.].(}.(h.
-00001d00: 68a0 68a1 4b00 68a2 68a3 68a4 4b04 68a5  h.h.K.h.h.h.K.h.
-00001d10: 8968 a689 757d 9428 689f 68a0 68a1 4b00  .h..u}.(h.h.h.K.
-00001d20: 68a2 68a3 68a4 4b04 68a5 8968 a689 7565  h.h.h.K.h..h..ue
-00001d30: 5d94 8974 9452 9468 9b28 8c10 6f6d 705f  ]..t.R.h.(..omp_
-00001d40: 6765 745f 7363 6865 6475 6c65 945d 945d  get_schedule.].]
-00001d50: 9428 7d94 2868 9f68 a068 a14b 0068 a268  .(}.(h.h.h.K.h.h
-00001d60: a368 a44b 0468 a589 68a6 8975 7d94 2868  .h.K.h..h..u}.(h
-00001d70: 9f68 a068 a14b 0068 a268 a368 a44b 0468  .h.h.K.h.h.h.K.h
-00001d80: a589 68a6 8975 6589 7494 5294 689b 288c  ..h..ue.t.R.h.(.
-00001d90: 146f 6d70 5f67 6574 5f74 6872 6561 645f  .omp_get_thread_
-00001da0: 6c69 6d69 7494 5d94 5d94 7d94 2868 9f68  limit.].].}.(h.h
-00001db0: a068 a14b 0068 a268 a368 a44b 0468 a589  .h.K.h.h.h.K.h..
-00001dc0: 68a6 8975 6189 7494 5294 689b 288c 196f  h..ua.t.R.h.(..o
-00001dd0: 6d70 5f73 6574 5f6d 6178 5f61 6374 6976  mp_set_max_activ
-00001de0: 655f 6c65 7665 6c73 945d 947d 9428 689f  e_levels.].}.(h.
-00001df0: 68a0 68a1 4b00 68a2 68a3 68a4 4b04 68a5  h.h.K.h.h.h.K.h.
-00001e00: 8968 a689 7561 5d94 8974 9452 9468 9b28  .h..ua]..t.R.h.(
-00001e10: 8c19 6f6d 705f 6765 745f 6d61 785f 6163  ..omp_get_max_ac
-00001e20: 7469 7665 5f6c 6576 656c 7394 5d94 5d94  tive_levels.].].
-00001e30: 7d94 2868 9f68 a068 a14b 0068 a268 a368  }.(h.h.h.K.h.h.h
-00001e40: a44b 0468 a589 68a6 8975 6189 7494 5294  .K.h..h..ua.t.R.
-00001e50: 689b 288c 0d6f 6d70 5f67 6574 5f6c 6576  h.(..omp_get_lev
-00001e60: 656c 945d 945d 947d 9428 689f 68a0 68a1  el.].].}.(h.h.h.
-00001e70: 4b00 68a2 68a3 68a4 4b04 68a5 8968 a689  K.h.h.h.K.h..h..
-00001e80: 7561 8974 9452 9468 9b28 8c1b 6f6d 705f  ua.t.R.h.(..omp_
-00001e90: 6765 745f 616e 6365 7374 6f72 5f74 6872  get_ancestor_thr
-00001ea0: 6561 645f 6e75 6d94 5d94 7d94 2868 9f68  ead_num.].}.(h.h
-00001eb0: a068 a14b 0068 a268 a368 a44b 0468 a589  .h.K.h.h.h.K.h..
-00001ec0: 68a6 8975 615d 947d 9428 689f 68a0 68a1  h..ua].}.(h.h.h.
-00001ed0: 4b00 68a2 68a3 68a4 4b04 68a5 8968 a689  K.h.h.h.K.h..h..
-00001ee0: 7561 8974 9452 9468 9b28 8c11 6f6d 705f  ua.t.R.h.(..omp_
-00001ef0: 6765 745f 7465 616d 5f73 697a 6594 5d94  get_team_size.].
-00001f00: 7d94 2868 9f68 a068 a14b 0068 a268 a368  }.(h.h.h.K.h.h.h
-00001f10: a44b 0468 a589 68a6 8975 615d 947d 9428  .K.h..h..ua].}.(
-00001f20: 689f 68a0 68a1 4b00 68a2 68a3 68a4 4b04  h.h.h.K.h.h.h.K.
-00001f30: 68a5 8968 a689 7561 8974 9452 9468 9b28  h..h..ua.t.R.h.(
-00001f40: 8c14 6f6d 705f 6765 745f 6163 7469 7665  ..omp_get_active
-00001f50: 5f6c 6576 656c 945d 945d 947d 9428 689f  _level.].].}.(h.
-00001f60: 68a0 68a1 4b00 68a2 68a3 68a4 4b04 68a5  h.h.K.h.h.h.K.h.
-00001f70: 8968 a689 7561 8974 9452 9468 9b28 8c0c  .h..ua.t.R.h.(..
-00001f80: 6f6d 705f 696e 5f66 696e 616c 945d 945d  omp_in_final.].]
-00001f90: 947d 9428 689f 68c6 68a1 4b00 68a2 68a3  .}.(h.h.h.K.h.h.
-00001fa0: 68a4 4aff ffff ff68 a589 68a6 8975 6189  h.J....h..h..ua.
-00001fb0: 7494 5294 689b 288c 116f 6d70 5f67 6574  t.R.h.(..omp_get
-00001fc0: 5f70 726f 635f 6269 6e64 945d 945d 947d  _proc_bind.].].}
-00001fd0: 9428 689f 68a0 68a1 4b00 68a2 68a3 68a4  .(h.h.h.K.h.h.h.
-00001fe0: 4b04 68a5 8968 a689 7561 8974 9452 9468  K.h..h..ua.t.R.h
-00001ff0: 9b28 8c12 6f6d 705f 6765 745f 6e75 6d5f  .(..omp_get_num_
-00002000: 706c 6163 6573 945d 945d 947d 9428 689f  places.].].}.(h.
-00002010: 68a0 68a1 4b00 68a2 68a3 68a4 4b04 68a5  h.h.K.h.h.h.K.h.
-00002020: 8968 a689 7561 8974 9452 9468 9b28 8c17  .h..ua.t.R.h.(..
-00002030: 6f6d 705f 6765 745f 706c 6163 655f 6e75  omp_get_place_nu
-00002040: 6d5f 7072 6f63 7394 5d94 7d94 2868 9f68  m_procs.].}.(h.h
-00002050: a068 a14b 0068 a268 a368 a44b 0468 a589  .h.K.h.h.h.K.h..
-00002060: 68a6 8975 615d 947d 9428 689f 68a0 68a1  h..ua].}.(h.h.h.
-00002070: 4b00 68a2 68a3 68a4 4b04 68a5 8968 a689  K.h.h.h.K.h..h..
-00002080: 7561 8974 9452 9468 9b28 8c16 6f6d 705f  ua.t.R.h.(..omp_
-00002090: 6765 745f 706c 6163 655f 7072 6f63 5f69  get_place_proc_i
-000020a0: 6473 945d 9428 7d94 2868 9f68 a068 a14b  ds.].(}.(h.h.h.K
-000020b0: 0068 a268 a368 a44b 0468 a589 68a6 8975  .h.h.h.K.h..h..u
-000020c0: 7d94 2868 9f68 a068 a14b 0168 a28c 0468  }.(h.h.h.K.h...h
-000020d0: 6561 7094 68a4 4b04 68a5 8968 a689 7565  eap.h.K.h..h..ue
-000020e0: 5d94 8974 9452 9468 9b28 8c11 6f6d 705f  ]..t.R.h.(..omp_
-000020f0: 6765 745f 706c 6163 655f 6e75 6d94 5d94  get_place_num.].
-00002100: 5d94 7d94 2868 9f68 a068 a14b 0068 a268  ].}.(h.h.h.K.h.h
-00002110: a368 a44b 0468 a589 68a6 8975 6189 7494  .h.K.h..h..ua.t.
-00002120: 5294 689b 288c 1c6f 6d70 5f67 6574 5f70  R.h.(..omp_get_p
-00002130: 6172 7469 7469 6f6e 5f6e 756d 5f70 6c61  artition_num_pla
-00002140: 6365 7394 5d94 5d94 7d94 2868 9f68 a068  ces.].].}.(h.h.h
-00002150: a14b 0068 a268 a368 a44b 0468 a589 68a6  .K.h.h.h.K.h..h.
-00002160: 8975 6189 7494 5294 689b 288c 1c6f 6d70  .ua.t.R.h.(..omp
-00002170: 5f67 6574 5f70 6172 7469 7469 6f6e 5f70  _get_partition_p
-00002180: 6c61 6365 5f6e 756d 7394 5d94 7d94 2868  lace_nums.].}.(h
-00002190: 9f68 a068 a14b 0168 a26a 3e01 0000 68a4  .h.h.K.h.j>...h.
-000021a0: 4b04 68a5 8968 a689 7561 5d94 8974 9452  K.h..h..ua]..t.R
-000021b0: 9468 9b28 8c16 6f6d 705f 7365 745f 6465  .h.(..omp_set_de
-000021c0: 6661 756c 745f 6465 7669 6365 945d 947d  fault_device.].}
-000021d0: 9428 689f 68a0 68a1 4b00 68a2 68a3 68a4  .(h.h.h.K.h.h.h.
-000021e0: 4b04 68a5 8968 a689 7561 5d94 8974 9452  K.h..h..ua]..t.R
-000021f0: 9468 9b28 8c16 6f6d 705f 6765 745f 6465  .h.(..omp_get_de
-00002200: 6661 756c 745f 6465 7669 6365 945d 945d  fault_device.].]
-00002210: 947d 9428 689f 68a0 68a1 4b00 68a2 68a3  .}.(h.h.h.K.h.h.
-00002220: 68a4 4b04 68a5 8968 a689 7561 8974 9452  h.K.h..h..ua.t.R
-00002230: 9468 9b28 8c13 6f6d 705f 6765 745f 6e75  .h.(..omp_get_nu
-00002240: 6d5f 6465 7669 6365 7394 5d94 5d94 7d94  m_devices.].].}.
-00002250: 2868 9f68 a068 a14b 0068 a268 a368 a44b  (h.h.h.K.h.h.h.K
-00002260: 0468 a589 68a6 8975 6189 7494 5294 689b  .h..h..ua.t.R.h.
-00002270: 288c 116f 6d70 5f67 6574 5f6e 756d 5f74  (..omp_get_num_t
-00002280: 6561 6d73 945d 945d 947d 9428 689f 68a0  eams.].].}.(h.h.
-00002290: 68a1 4b00 68a2 68a3 68a4 4b04 68a5 8968  h.K.h.h.h.K.h..h
-000022a0: a689 7561 8974 9452 9468 9b28 8c10 6f6d  ..ua.t.R.h.(..om
-000022b0: 705f 6765 745f 7465 616d 5f6e 756d 945d  p_get_team_num.]
-000022c0: 945d 947d 9428 689f 68a0 68a1 4b00 68a2  .].}.(h.h.h.K.h.
-000022d0: 68a3 68a4 4b04 68a5 8968 a689 7561 8974  h.h.K.h..h..ua.t
-000022e0: 9452 9468 9b28 8c15 6f6d 705f 6973 5f69  .R.h.(..omp_is_i
-000022f0: 6e69 7469 616c 5f64 6576 6963 6594 5d94  nitial_device.].
-00002300: 5d94 7d94 2868 9f68 c668 a14b 0068 a268  ].}.(h.h.h.K.h.h
-00002310: a368 a44a ffff ffff 68a5 8968 a689 7561  .h.J....h..h..ua
-00002320: 8974 9452 9468 9b28 8c16 6f6d 705f 6765  .t.R.h.(..omp_ge
-00002330: 745f 696e 6974 6961 6c5f 6465 7669 6365  t_initial_device
-00002340: 945d 945d 947d 9428 689f 68a0 68a1 4b00  .].].}.(h.h.h.K.
-00002350: 68a2 68a3 68a4 4b04 68a5 8968 a689 7561  h.h.h.K.h..h..ua
-00002360: 8974 9452 9468 9b28 8c19 6f6d 705f 6765  .t.R.h.(..omp_ge
-00002370: 745f 6d61 785f 7461 736b 5f70 7269 6f72  t_max_task_prior
-00002380: 6974 7994 5d94 5d94 7d94 2868 9f68 a068  ity.].].}.(h.h.h
-00002390: a14b 0068 a268 a368 a44b 0468 a589 68a6  .K.h.h.h.K.h..h.
-000023a0: 8975 6189 7494 5294 687a 687f 297d 9468  .ua.t.R.hzh.)}.h
-000023b0: 818c 3c2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ..<.............
-000023c0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-000023d0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-000023e0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e94  ................
-000023f0: 7387 9452 9474 9473 8794 5294 8c0f 5f76  s..R.t.s..R..._v
-00002400: 6172 6961 626c 655f 696e 6974 7394 298c  ariable_inits.).
-00002410: 145f 696e 7465 726e 616c 5f64 6963 7469  ._internal_dicti
-00002420: 6f6e 6172 7994 7d94 8c06 5f73 636f 7065  onary.}..._scope
-00002430: 948c 1370 7963 6365 6c2e 7061 7273 6572  ...pyccel.parser
-00002440: 2e73 636f 7065 948c 0553 636f 7065 9493  .scope...Scope..
-00002450: 9429 8194 4e7d 9428 6875 7d94 288c 0966  .)..N}.(hu}.(..f
-00002460: 756e 6374 696f 6e73 947d 948c 0976 6172  unctions.}...var
-00002470: 6961 626c 6573 947d 948c 0763 6c61 7373  iables.}...class
-00002480: 6573 947d 948c 0769 6d70 6f72 7473 947d  es.}...imports.}
-00002490: 948c 1273 796d 626f 6c69 635f 6675 6e63  ...symbolic_func
-000024a0: 7469 6f6e 7394 7d94 8c06 6d61 6372 6f73  tions.}...macros
-000024b0: 947d 948c 0974 656d 706c 6174 6573 947d  .}...templates.}
-000024c0: 948c 0768 6561 6465 7273 947d 948c 0a64  ...headers.}...d
-000024d0: 6563 6f72 6174 6f72 7394 7d94 8c0e 636c  ecorators.}...cl
-000024e0: 735f 636f 6e73 7472 7563 7473 947d 9475  s_constructs.}.u
-000024f0: 8c07 5f6c 6f63 616c 7394 7d94 286a 9501  .._locals.}.(j..
-00002500: 0000 7d94 6a97 0100 007d 946a 9901 0000  ..}.j....}.j....
-00002510: 7d94 6a9b 0100 007d 946a 9d01 0000 7d94  }.j....}.j....}.
-00002520: 6a9f 0100 007d 946a a101 0000 7d94 6aa3  j....}.j....}.j.
-00002530: 0100 007d 946a a501 0000 7d94 6aa7 0100  ...}.j....}.j...
-00002540: 007d 9475 8c0d 5f70 6172 656e 745f 7363  .}.u.._parent_sc
-00002550: 6f70 6594 4e8c 0c5f 736f 6e73 5f73 636f  ope.N.._sons_sco
-00002560: 7065 7394 7d94 8c08 5f69 735f 6c6f 6f70  pes.}..._is_loop
-00002570: 9489 8c06 5f6c 6f6f 7073 945d 948c 145f  ...._loops.]..._
-00002580: 7465 6d70 6f72 6172 795f 7661 7269 6162  temporary_variab
-00002590: 6c65 7394 5d94 8c0d 5f75 7365 645f 7379  les.]..._used_sy
-000025a0: 6d62 6f6c 7394 7d94 6866 6863 8c06 6f70  mbols.}.hfhc..op
-000025b0: 656e 6d70 9485 9481 944e 7d94 6868 8973  enmp.....N}.hh.s
-000025c0: 8694 6273 8c0e 5f64 756d 6d79 5f63 6f75  ..bs.._dummy_cou
-000025d0: 6e74 6572 944b 008c 105f 6f72 6967 696e  nter.K..._origin
-000025e0: 616c 5f73 796d 626f 6c94 7d94 6ac1 0100  al_symbol.}.j...
-000025f0: 0068 6673 7586 9462 686a 5d94 6809 5d94  .hfsu..bhj].h.].
-00002600: 680d 6168 6d89 686e 686f 7586 9462 8c09  h.ahm.hnhou..b..
-00002610: 5f66 696c 656e 616d 6594 8c39 2f55 7365  _filename..9/Use
-00002620: 7273 2f79 616d 616e 2f74 6d70 2f70 7963  rs/yaman/tmp/pyc
-00002630: 6365 6c2f 7079 6363 656c 2f73 7464 6c69  cel/pyccel/stdli
-00002640: 622f 696e 7465 726e 616c 2f6f 7065 6e6d  b/internal/openm
-00002650: 702e 7079 6894 8c09 5f6d 6574 6176 6172  p.pyh..._metavar
-00002660: 7394 7d94 288c 0b6d 6f64 756c 655f 6e61  s.}.(..module_na
-00002670: 6d65 948c 076f 6d70 5f6c 6962 948c 0e6d  me...omp_lib...m
-00002680: 6f64 756c 655f 7665 7273 696f 6e94 8c03  odule_version...
-00002690: 342e 3594 8c04 7361 7665 9488 8c09 6e6f  4.5...save....no
-000026a0: 5f74 6172 6765 7494 888c 0865 7874 6572  _target....exter
-000026b0: 6e61 6c94 8975 6a8e 0100 006a 9201 0000  nal..uj....j....
-000026c0: 8c0e 5f63 7572 7265 6e74 5f63 6c61 7373  .._current_class
-000026d0: 944e 8c11 5f63 7572 7265 6e74 5f66 756e  .N.._current_fun
-000026e0: 6374 696f 6e94 4e8c 0c5f 7379 6e74 6178  ction.N.._syntax
-000026f0: 5f64 6f6e 6594 888c 0e5f 7365 6d61 6e74  _done...._semant
-00002700: 6963 5f64 6f6e 6594 898c 115f 6375 7272  ic_done...._curr
-00002710: 656e 745f 6673 745f 6e6f 6465 944e 8c09  ent_fst_node.N..
-00002720: 5f62 6c6f 636b 696e 6794 898c 145f 6372  _blocking...._cr
-00002730: 6561 7465 645f 6672 6f6d 5f70 6963 6b6c  eated_from_pickl
-00002740: 6594 898c 085f 636f 6e74 6578 7494 5d94  e...._context.].
-00002750: 8c0e 5f69 6e5f 6c68 735f 6173 7369 676e  .._in_lhs_assign
-00002760: 9489 7562 8794 2e                        ..ub...
+000019d0: 2e94 7387 9452 948c 1270 7963 6365 6c2e  ..s..R...pyccel.
+000019e0: 6173 742e 6865 6164 6572 7394 8c0e 4675  ast.headers...Fu
+000019f0: 6e63 7469 6f6e 4865 6164 6572 9493 9428  nctionHeader...(
+00001a00: 8c13 6f6d 705f 7365 745f 6e75 6d5f 7468  ..omp_set_num_th
+00001a10: 7265 6164 7394 5d94 7d94 288c 0864 6174  reads.].}.(..dat
+00001a20: 6174 7970 6594 8c14 7079 6363 656c 2e61  atype...pyccel.a
+00001a30: 7374 2e64 6174 6174 7970 6573 948c 0d4e  st.datatypes...N
+00001a40: 6174 6976 6549 6e74 6567 6572 9493 9429  ativeInteger...)
+00001a50: 5294 8c04 7261 6e6b 944b 008c 0f6d 656d  R...rank.K...mem
+00001a60: 6f72 795f 6861 6e64 6c69 6e67 948c 0573  ory_handling...s
+00001a70: 7461 636b 948c 0970 7265 6369 7369 6f6e  tack...precision
+00001a80: 944b 048c 0769 735f 6675 6e63 9489 8c08  .K...is_func....
+00001a90: 6973 5f63 6f6e 7374 9489 7561 5d94 8974  is_const..ua]..t
+00001aa0: 9452 9468 9a28 8c13 6f6d 705f 6765 745f  .R.h.(..omp_get_
+00001ab0: 6e75 6d5f 7468 7265 6164 7394 5d94 5d94  num_threads.].].
+00001ac0: 7d94 2868 9e68 a268 a34b 0068 a468 a568  }.(h.h.h.K.h.h.h
+00001ad0: a64b 0468 a789 68a8 8975 6189 7494 5294  .K.h..h..ua.t.R.
+00001ae0: 689a 288c 136f 6d70 5f67 6574 5f6d 6178  h.(..omp_get_max
+00001af0: 5f74 6872 6561 6473 945d 945d 947d 9428  _threads.].].}.(
+00001b00: 689e 68a2 68a3 4b00 68a4 68a5 68a6 4b04  h.h.h.K.h.h.h.K.
+00001b10: 68a7 8968 a889 7561 8974 9452 9468 9a28  h..h..ua.t.R.h.(
+00001b20: 8c12 6f6d 705f 6765 745f 7468 7265 6164  ..omp_get_thread
+00001b30: 5f6e 756d 945d 945d 947d 9428 689e 68a2  _num.].].}.(h.h.
+00001b40: 68a3 4b00 68a4 68a5 68a6 4b04 68a7 8968  h.K.h.h.h.K.h..h
+00001b50: a889 7561 8974 9452 9468 9a28 8c11 6f6d  ..ua.t.R.h.(..om
+00001b60: 705f 6765 745f 6e75 6d5f 7072 6f63 7394  p_get_num_procs.
+00001b70: 5d94 5d94 7d94 2868 9e68 a268 a34b 0068  ].].}.(h.h.h.K.h
+00001b80: a468 a568 a64b 0468 a789 68a8 8975 6189  .h.h.K.h..h..ua.
+00001b90: 7494 5294 689a 288c 0f6f 6d70 5f69 6e5f  t.R.h.(..omp_in_
+00001ba0: 7061 7261 6c6c 656c 945d 945d 947d 9428  parallel.].].}.(
+00001bb0: 689e 689f 8c0a 4e61 7469 7665 426f 6f6c  h.h...NativeBool
+00001bc0: 9493 9429 5294 68a3 4b00 68a4 68a5 68a6  ...)R.h.K.h.h.h.
+00001bd0: 4aff ffff ff68 a789 68a8 8975 6189 7494  J....h..h..ua.t.
+00001be0: 5294 689a 288c 0f6f 6d70 5f73 6574 5f64  R.h.(..omp_set_d
+00001bf0: 796e 616d 6963 945d 947d 9428 689e 68ca  ynamic.].}.(h.h.
+00001c00: 68a3 4b00 68a4 68a5 68a6 4aff ffff ff68  h.K.h.h.h.J....h
+00001c10: a789 68a8 8975 615d 9489 7494 5294 689a  ..h..ua]..t.R.h.
+00001c20: 288c 0f6f 6d70 5f67 6574 5f64 796e 616d  (..omp_get_dynam
+00001c30: 6963 945d 945d 947d 9428 689e 68ca 68a3  ic.].].}.(h.h.h.
+00001c40: 4b00 68a4 68a5 68a6 4aff ffff ff68 a789  K.h.h.h.J....h..
+00001c50: 68a8 8975 6189 7494 5294 689a 288c 146f  h..ua.t.R.h.(..o
+00001c60: 6d70 5f67 6574 5f63 616e 6365 6c6c 6174  mp_get_cancellat
+00001c70: 696f 6e94 5d94 5d94 7d94 2868 9e68 ca68  ion.].].}.(h.h.h
+00001c80: a34b 0068 a468 a568 a64a ffff ffff 68a7  .K.h.h.h.J....h.
+00001c90: 8968 a889 7561 8974 9452 9468 9a28 8c0e  .h..ua.t.R.h.(..
+00001ca0: 6f6d 705f 7365 745f 6e65 7374 6564 945d  omp_set_nested.]
+00001cb0: 947d 9428 689e 68ca 68a3 4b00 68a4 68a5  .}.(h.h.h.K.h.h.
+00001cc0: 68a6 4aff ffff ff68 a789 68a8 8975 615d  h.J....h..h..ua]
+00001cd0: 9489 7494 5294 689a 288c 0e6f 6d70 5f67  ..t.R.h.(..omp_g
+00001ce0: 6574 5f6e 6573 7465 6494 5d94 5d94 7d94  et_nested.].].}.
+00001cf0: 2868 9e68 ca68 a34b 0068 a468 a568 a64a  (h.h.h.K.h.h.h.J
+00001d00: ffff ffff 68a7 8968 a889 7561 8974 9452  ....h..h..ua.t.R
+00001d10: 9468 9a28 8c10 6f6d 705f 7365 745f 7363  .h.(..omp_set_sc
+00001d20: 6865 6475 6c65 945d 9428 7d94 2868 9e68  hedule.].(}.(h.h
+00001d30: a268 a34b 0068 a468 a568 a64b 0468 a789  .h.K.h.h.h.K.h..
+00001d40: 68a8 8975 7d94 2868 9e68 a268 a34b 0068  h..u}.(h.h.h.K.h
+00001d50: a468 a568 a64b 0468 a789 68a8 8975 655d  .h.h.K.h..h..ue]
+00001d60: 9489 7494 5294 689a 288c 106f 6d70 5f67  ..t.R.h.(..omp_g
+00001d70: 6574 5f73 6368 6564 756c 6594 5d94 5d94  et_schedule.].].
+00001d80: 287d 9428 689e 68a2 68a3 4b00 68a4 68a5  (}.(h.h.h.K.h.h.
+00001d90: 68a6 4b04 68a7 8968 a889 757d 9428 689e  h.K.h..h..u}.(h.
+00001da0: 68a2 68a3 4b00 68a4 68a5 68a6 4b04 68a7  h.h.K.h.h.h.K.h.
+00001db0: 8968 a889 7565 8974 9452 9468 9a28 8c14  .h..ue.t.R.h.(..
+00001dc0: 6f6d 705f 6765 745f 7468 7265 6164 5f6c  omp_get_thread_l
+00001dd0: 696d 6974 945d 945d 947d 9428 689e 68a2  imit.].].}.(h.h.
+00001de0: 68a3 4b00 68a4 68a5 68a6 4b04 68a7 8968  h.K.h.h.h.K.h..h
+00001df0: a889 7561 8974 9452 9468 9a28 8c19 6f6d  ..ua.t.R.h.(..om
+00001e00: 705f 7365 745f 6d61 785f 6163 7469 7665  p_set_max_active
+00001e10: 5f6c 6576 656c 7394 5d94 7d94 2868 9e68  _levels.].}.(h.h
+00001e20: a268 a34b 0068 a468 a568 a64b 0468 a789  .h.K.h.h.h.K.h..
+00001e30: 68a8 8975 615d 9489 7494 5294 689a 288c  h..ua]..t.R.h.(.
+00001e40: 196f 6d70 5f67 6574 5f6d 6178 5f61 6374  .omp_get_max_act
+00001e50: 6976 655f 6c65 7665 6c73 945d 945d 947d  ive_levels.].].}
+00001e60: 9428 689e 68a2 68a3 4b00 68a4 68a5 68a6  .(h.h.h.K.h.h.h.
+00001e70: 4b04 68a7 8968 a889 7561 8974 9452 9468  K.h..h..ua.t.R.h
+00001e80: 9a28 8c0d 6f6d 705f 6765 745f 6c65 7665  .(..omp_get_leve
+00001e90: 6c94 5d94 5d94 7d94 2868 9e68 a268 a34b  l.].].}.(h.h.h.K
+00001ea0: 0068 a468 a568 a64b 0468 a789 68a8 8975  .h.h.h.K.h..h..u
+00001eb0: 6189 7494 5294 689a 288c 1b6f 6d70 5f67  a.t.R.h.(..omp_g
+00001ec0: 6574 5f61 6e63 6573 746f 725f 7468 7265  et_ancestor_thre
+00001ed0: 6164 5f6e 756d 945d 947d 9428 689e 68a2  ad_num.].}.(h.h.
+00001ee0: 68a3 4b00 68a4 68a5 68a6 4b04 68a7 8968  h.K.h.h.h.K.h..h
+00001ef0: a889 7561 5d94 7d94 2868 9e68 a268 a34b  ..ua].}.(h.h.h.K
+00001f00: 0068 a468 a568 a64b 0468 a789 68a8 8975  .h.h.h.K.h..h..u
+00001f10: 6189 7494 5294 689a 288c 116f 6d70 5f67  a.t.R.h.(..omp_g
+00001f20: 6574 5f74 6561 6d5f 7369 7a65 945d 947d  et_team_size.].}
+00001f30: 9428 689e 68a2 68a3 4b00 68a4 68a5 68a6  .(h.h.h.K.h.h.h.
+00001f40: 4b04 68a7 8968 a889 7561 5d94 7d94 2868  K.h..h..ua].}.(h
+00001f50: 9e68 a268 a34b 0068 a468 a568 a64b 0468  .h.h.K.h.h.h.K.h
+00001f60: a789 68a8 8975 6189 7494 5294 689a 288c  ..h..ua.t.R.h.(.
+00001f70: 146f 6d70 5f67 6574 5f61 6374 6976 655f  .omp_get_active_
+00001f80: 6c65 7665 6c94 5d94 5d94 7d94 2868 9e68  level.].].}.(h.h
+00001f90: a268 a34b 0068 a468 a568 a64b 0468 a789  .h.K.h.h.h.K.h..
+00001fa0: 68a8 8975 6189 7494 5294 689a 288c 0c6f  h..ua.t.R.h.(..o
+00001fb0: 6d70 5f69 6e5f 6669 6e61 6c94 5d94 5d94  mp_in_final.].].
+00001fc0: 7d94 2868 9e68 ca68 a34b 0068 a468 a568  }.(h.h.h.K.h.h.h
+00001fd0: a64a ffff ffff 68a7 8968 a889 7561 8974  .J....h..h..ua.t
+00001fe0: 9452 9468 9a28 8c11 6f6d 705f 6765 745f  .R.h.(..omp_get_
+00001ff0: 7072 6f63 5f62 696e 6494 5d94 5d94 7d94  proc_bind.].].}.
+00002000: 2868 9e68 a268 a34b 0068 a468 a568 a64b  (h.h.h.K.h.h.h.K
+00002010: 0468 a789 68a8 8975 6189 7494 5294 689a  .h..h..ua.t.R.h.
+00002020: 288c 126f 6d70 5f67 6574 5f6e 756d 5f70  (..omp_get_num_p
+00002030: 6c61 6365 7394 5d94 5d94 7d94 2868 9e68  laces.].].}.(h.h
+00002040: a268 a34b 0068 a468 a568 a64b 0468 a789  .h.K.h.h.h.K.h..
+00002050: 68a8 8975 6189 7494 5294 689a 288c 176f  h..ua.t.R.h.(..o
+00002060: 6d70 5f67 6574 5f70 6c61 6365 5f6e 756d  mp_get_place_num
+00002070: 5f70 726f 6373 945d 947d 9428 689e 68a2  _procs.].}.(h.h.
+00002080: 68a3 4b00 68a4 68a5 68a6 4b04 68a7 8968  h.K.h.h.h.K.h..h
+00002090: a889 7561 5d94 7d94 2868 9e68 a268 a34b  ..ua].}.(h.h.h.K
+000020a0: 0068 a468 a568 a64b 0468 a789 68a8 8975  .h.h.h.K.h..h..u
+000020b0: 6189 7494 5294 689a 288c 166f 6d70 5f67  a.t.R.h.(..omp_g
+000020c0: 6574 5f70 6c61 6365 5f70 726f 635f 6964  et_place_proc_id
+000020d0: 7394 5d94 287d 9428 689e 68a2 68a3 4b00  s.].(}.(h.h.h.K.
+000020e0: 68a4 68a5 68a6 4b04 68a7 8968 a889 757d  h.h.h.K.h..h..u}
+000020f0: 9428 689e 68a2 68a3 4b01 68a4 8c04 6865  .(h.h.h.K.h...he
+00002100: 6170 9468 a64b 0468 a789 68a8 8975 655d  ap.h.K.h..h..ue]
+00002110: 9489 7494 5294 689a 288c 116f 6d70 5f67  ..t.R.h.(..omp_g
+00002120: 6574 5f70 6c61 6365 5f6e 756d 945d 945d  et_place_num.].]
+00002130: 947d 9428 689e 68a2 68a3 4b00 68a4 68a5  .}.(h.h.h.K.h.h.
+00002140: 68a6 4b04 68a7 8968 a889 7561 8974 9452  h.K.h..h..ua.t.R
+00002150: 9468 9a28 8c1c 6f6d 705f 6765 745f 7061  .h.(..omp_get_pa
+00002160: 7274 6974 696f 6e5f 6e75 6d5f 706c 6163  rtition_num_plac
+00002170: 6573 945d 945d 947d 9428 689e 68a2 68a3  es.].].}.(h.h.h.
+00002180: 4b00 68a4 68a5 68a6 4b04 68a7 8968 a889  K.h.h.h.K.h..h..
+00002190: 7561 8974 9452 9468 9a28 8c1c 6f6d 705f  ua.t.R.h.(..omp_
+000021a0: 6765 745f 7061 7274 6974 696f 6e5f 706c  get_partition_pl
+000021b0: 6163 655f 6e75 6d73 945d 947d 9428 689e  ace_nums.].}.(h.
+000021c0: 68a2 68a3 4b01 68a4 6a42 0100 0068 a64b  h.h.K.h.jB...h.K
+000021d0: 0468 a789 68a8 8975 615d 9489 7494 5294  .h..h..ua]..t.R.
+000021e0: 689a 288c 166f 6d70 5f73 6574 5f64 6566  h.(..omp_set_def
+000021f0: 6175 6c74 5f64 6576 6963 6594 5d94 7d94  ault_device.].}.
+00002200: 2868 9e68 a268 a34b 0068 a468 a568 a64b  (h.h.h.K.h.h.h.K
+00002210: 0468 a789 68a8 8975 615d 9489 7494 5294  .h..h..ua]..t.R.
+00002220: 689a 288c 166f 6d70 5f67 6574 5f64 6566  h.(..omp_get_def
+00002230: 6175 6c74 5f64 6576 6963 6594 5d94 5d94  ault_device.].].
+00002240: 7d94 2868 9e68 a268 a34b 0068 a468 a568  }.(h.h.h.K.h.h.h
+00002250: a64b 0468 a789 68a8 8975 6189 7494 5294  .K.h..h..ua.t.R.
+00002260: 689a 288c 136f 6d70 5f67 6574 5f6e 756d  h.(..omp_get_num
+00002270: 5f64 6576 6963 6573 945d 945d 947d 9428  _devices.].].}.(
+00002280: 689e 68a2 68a3 4b00 68a4 68a5 68a6 4b04  h.h.h.K.h.h.h.K.
+00002290: 68a7 8968 a889 7561 8974 9452 9468 9a28  h..h..ua.t.R.h.(
+000022a0: 8c11 6f6d 705f 6765 745f 6e75 6d5f 7465  ..omp_get_num_te
+000022b0: 616d 7394 5d94 5d94 7d94 2868 9e68 a268  ams.].].}.(h.h.h
+000022c0: a34b 0068 a468 a568 a64b 0468 a789 68a8  .K.h.h.h.K.h..h.
+000022d0: 8975 6189 7494 5294 689a 288c 106f 6d70  .ua.t.R.h.(..omp
+000022e0: 5f67 6574 5f74 6561 6d5f 6e75 6d94 5d94  _get_team_num.].
+000022f0: 5d94 7d94 2868 9e68 a268 a34b 0068 a468  ].}.(h.h.h.K.h.h
+00002300: a568 a64b 0468 a789 68a8 8975 6189 7494  .h.K.h..h..ua.t.
+00002310: 5294 689a 288c 156f 6d70 5f69 735f 696e  R.h.(..omp_is_in
+00002320: 6974 6961 6c5f 6465 7669 6365 945d 945d  itial_device.].]
+00002330: 947d 9428 689e 68ca 68a3 4b00 68a4 68a5  .}.(h.h.h.K.h.h.
+00002340: 68a6 4aff ffff ff68 a789 68a8 8975 6189  h.J....h..h..ua.
+00002350: 7494 5294 689a 288c 166f 6d70 5f67 6574  t.R.h.(..omp_get
+00002360: 5f69 6e69 7469 616c 5f64 6576 6963 6594  _initial_device.
+00002370: 5d94 5d94 7d94 2868 9e68 a268 a34b 0068  ].].}.(h.h.h.K.h
+00002380: a468 a568 a64b 0468 a789 68a8 8975 6189  .h.h.K.h..h..ua.
+00002390: 7494 5294 689a 288c 196f 6d70 5f67 6574  t.R.h.(..omp_get
+000023a0: 5f6d 6178 5f74 6173 6b5f 7072 696f 7269  _max_task_priori
+000023b0: 7479 945d 945d 947d 9428 689e 68a2 68a3  ty.].].}.(h.h.h.
+000023c0: 4b00 68a4 68a5 68a6 4b04 68a7 8968 a889  K.h.h.h.K.h..h..
+000023d0: 7561 8974 9452 9468 7968 7e29 7d94 6880  ua.t.R.hyh~)}.h.
+000023e0: 8c3c 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  .<..............
+000023f0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00002400: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
+00002410: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 9473  ...............s
+00002420: 8794 5294 7494 7387 9452 948c 0f5f 7661  ..R.t.s..R..._va
+00002430: 7269 6162 6c65 5f69 6e69 7473 9429 8c14  riable_inits.)..
+00002440: 5f69 6e74 6572 6e61 6c5f 6469 6374 696f  _internal_dictio
+00002450: 6e61 7279 947d 948c 065f 7363 6f70 6594  nary.}..._scope.
+00002460: 8c13 7079 6363 656c 2e70 6172 7365 722e  ..pyccel.parser.
+00002470: 7363 6f70 6594 8c05 5363 6f70 6594 9394  scope...Scope...
+00002480: 2981 944e 7d94 2868 747d 9428 8c09 6675  )..N}.(ht}.(..fu
+00002490: 6e63 7469 6f6e 7394 7d94 8c09 7661 7269  nctions.}...vari
+000024a0: 6162 6c65 7394 7d94 8c07 636c 6173 7365  ables.}...classe
+000024b0: 7394 7d94 8c07 696d 706f 7274 7394 7d94  s.}...imports.}.
+000024c0: 8c12 7379 6d62 6f6c 6963 5f66 756e 6374  ..symbolic_funct
+000024d0: 696f 6e73 947d 948c 066d 6163 726f 7394  ions.}...macros.
+000024e0: 7d94 8c09 7465 6d70 6c61 7465 7394 7d94  }...templates.}.
+000024f0: 8c07 6865 6164 6572 7394 7d94 8c0a 6465  ..headers.}...de
+00002500: 636f 7261 746f 7273 947d 948c 0e63 6c73  corators.}...cls
+00002510: 5f63 6f6e 7374 7275 6374 7394 7d94 758c  _constructs.}.u.
+00002520: 075f 6c6f 6361 6c73 947d 9428 6a99 0100  ._locals.}.(j...
+00002530: 007d 946a 9b01 0000 7d94 6a9d 0100 007d  .}.j....}.j....}
+00002540: 946a 9f01 0000 7d94 6aa1 0100 007d 946a  .j....}.j....}.j
+00002550: a301 0000 7d94 6aa5 0100 007d 946a a701  ....}.j....}.j..
+00002560: 0000 7d94 6aa9 0100 007d 946a ab01 0000  ..}.j....}.j....
+00002570: 7d94 758c 0d5f 7061 7265 6e74 5f73 636f  }.u.._parent_sco
+00002580: 7065 944e 8c0c 5f73 6f6e 735f 7363 6f70  pe.N.._sons_scop
+00002590: 6573 947d 948c 085f 6973 5f6c 6f6f 7094  es.}..._is_loop.
+000025a0: 898c 065f 6c6f 6f70 7394 5d94 8c14 5f74  ..._loops.]..._t
+000025b0: 656d 706f 7261 7279 5f76 6172 6961 626c  emporary_variabl
+000025c0: 6573 945d 948c 0d5f 7573 6564 5f73 796d  es.]..._used_sym
+000025d0: 626f 6c73 947d 9468 6568 628c 066f 7065  bols.}.hehb..ope
+000025e0: 6e6d 7094 8594 8194 4e7d 9468 6789 7386  nmp.....N}.hg.s.
+000025f0: 9462 738c 0e5f 6475 6d6d 795f 636f 756e  .bs.._dummy_coun
+00002600: 7465 7294 4b00 8c10 5f6f 7269 6769 6e61  ter.K..._origina
+00002610: 6c5f 7379 6d62 6f6c 947d 946a c501 0000  l_symbol.}.j....
+00002620: 6865 7375 8694 6268 695d 9468 095d 9468  hesu..bhi].h.].h
+00002630: 0d61 686c 8968 6d68 6e75 8694 628c 095f  .ahl.hmhnu..b.._
+00002640: 6669 6c65 6e61 6d65 948c 3b2f 686f 6d65  filename..;/home
+00002650: 2f79 616d 616e 6775 632f 746d 702f 7079  /yamanguc/tmp/py
+00002660: 6363 656c 2f70 7963 6365 6c2f 7374 646c  ccel/pyccel/stdl
+00002670: 6962 2f69 6e74 6572 6e61 6c2f 6f70 656e  ib/internal/open
+00002680: 6d70 2e70 7968 948c 095f 6d65 7461 7661  mp.pyh..._metava
+00002690: 7273 947d 9428 8c0b 6d6f 6475 6c65 5f6e  rs.}.(..module_n
+000026a0: 616d 6594 8c07 6f6d 705f 6c69 6294 8c0e  ame...omp_lib...
+000026b0: 6d6f 6475 6c65 5f76 6572 7369 6f6e 948c  module_version..
+000026c0: 0334 2e35 948c 0473 6176 6594 888c 096e  .4.5...save....n
+000026d0: 6f5f 7461 7267 6574 9488 8c08 6578 7465  o_target....exte
+000026e0: 726e 616c 9489 756a 9201 0000 6a96 0100  rnal..uj....j...
+000026f0: 008c 0e5f 6375 7272 656e 745f 636c 6173  ..._current_clas
+00002700: 7394 4e8c 115f 6375 7272 656e 745f 6675  s.N.._current_fu
+00002710: 6e63 7469 6f6e 944e 8c0c 5f73 796e 7461  nction.N.._synta
+00002720: 785f 646f 6e65 9488 8c0e 5f73 656d 616e  x_done...._seman
+00002730: 7469 635f 646f 6e65 9489 8c11 5f63 7572  tic_done...._cur
+00002740: 7265 6e74 5f66 7374 5f6e 6f64 6594 4e8c  rent_fst_node.N.
+00002750: 095f 626c 6f63 6b69 6e67 9489 8c14 5f63  ._blocking...._c
+00002760: 7265 6174 6564 5f66 726f 6d5f 7069 636b  reated_from_pick
+00002770: 6c65 9489 8c08 5f63 6f6e 7465 7874 945d  le...._context.]
+00002780: 948c 0e5f 696e 5f6c 6873 5f61 7373 6967  ..._in_lhs_assig
+00002790: 6e94 8975 6287 942e                      n..ub...
```

### Comparing `pyccel-1.9.1/pyccel/stdlib/internal/openmp.pyh` & `pyccel-1.9.2/pyccel/stdlib/internal/openmp.pyh`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/math/pyc_math_c.c` & `pyccel-1.9.2/pyccel/stdlib/math/pyc_math_c.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/math/pyc_math_c.h` & `pyccel-1.9.2/pyccel/stdlib/math/pyc_math_c.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/math/pyc_math_f90.f90` & `pyccel-1.9.2/pyccel/stdlib/math/pyc_math_f90.f90`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/ndarrays/ndarrays.c` & `pyccel-1.9.2/pyccel/stdlib/ndarrays/ndarrays.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/ndarrays/ndarrays.h` & `pyccel-1.9.2/pyccel/stdlib/ndarrays/ndarrays.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/numpy/numpy_c.c` & `pyccel-1.9.2/pyccel/stdlib/numpy/numpy_c.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/numpy/numpy_c.h` & `pyccel-1.9.2/pyccel/stdlib/numpy/numpy_c.h`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/numpy/numpy_f90.f90` & `pyccel-1.9.2/pyccel/stdlib/numpy/numpy_f90.f90`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/stdlib/parallel/mpi.py` & `pyccel-1.9.2/pyccel/stdlib/parallel/mpi.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/symbolic/lambdify.py` & `pyccel-1.9.2/pyccel/symbolic/lambdify.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/utilities/metaclasses.py` & `pyccel-1.9.2/pyccel/utilities/metaclasses.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/utilities/stage.py` & `pyccel-1.9.2/pyccel/utilities/stage.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel/utilities/strings.py` & `pyccel-1.9.2/pyccel/utilities/strings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/pyccel.egg-info/PKG-INFO` & `pyccel-1.9.2/pyccel.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: pyccel
-Version: 1.9.1
+Version: 1.9.2
 Summary: UNKNOWN
 Home-page: https://github.com/pyccel/pyccel
 Author: Pyccel development team
 License: LICENSE
 Keywords: math
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 License-File: AUTHORS
 
 # Pyccel : write Python code,  get Fortran speed
 
- [![devel_tests](https://github.com/pyccel/pyccel/actions/workflows/devel.yml/badge.svg)](https://github.com/pyccel/pyccel/actions/workflows/devel.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade) [![DOI](https://joss.theoj.org/papers/10.21105/joss.04991/status.svg)](https://doi.org/10.21105/joss.04991)
+ [![Linux unit tests](https://github.com/pyccel/pyccel/actions/workflows/linux.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/linux.yml) [![MacOSX unit tests](https://github.com/pyccel/pyccel/actions/workflows/macosx.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/macosx.yml) [![Windows unit tests](https://github.com/pyccel/pyccel/actions/workflows/windows.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/windows.yml) [![Anaconda-Linux](https://github.com/pyccel/pyccel/actions/workflows/anaconda_linux.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/anaconda_linux.yml) [![Anaconda-Windows](https://github.com/pyccel/pyccel/actions/workflows/anaconda_windows.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/anaconda_windows.yml) [![Intel unit tests](https://github.com/pyccel/pyccel/actions/workflows/intel.yml/badge.svg?branch=devel&event=push)](https://github.com/pyccel/pyccel/actions/workflows/intel.yml) [![codacy](https://app.codacy.com/project/badge/Grade/9723f47b95db491886a0e78339bd4698)](https://www.codacy.com/gh/pyccel/pyccel?utm_source=github.com&utm_medium=referral&utm_content=pyccel/pyccel&utm_campaign=Badge_Grade) [![DOI](https://joss.theoj.org/papers/10.21105/joss.04991/status.svg)](https://doi.org/10.21105/joss.04991)
 
 **Pyccel** stands for Python extension language using accelerators.
 
 The aim of **Pyccel** is to provide a simple way to generate automatically, parallel low level code. The main uses would be:
 
 1.  Convert a _Python_ code (or project) into a Fortran or C code.
 2.  Accelerate _Python_ functions by converting them to _Fortran_ or _C_ functions.
@@ -100,10 +100,11 @@
 
 -   [Overview](https://github.com/pyccel/pyccel/blob/devel/developer_docs/overview.md)
 -   [How to solve an issue](https://github.com/pyccel/pyccel/blob/devel/developer_docs/how_to_solve_an_issue.md)
 -   [Review Process](https://github.com/pyccel/pyccel/blob/devel/developer_docs/review_process.md)
 -   [Development Conventions](https://github.com/pyccel/pyccel/blob/devel/developer_docs/development_conventions.md)
 -   [Tips and Tricks](https://github.com/pyccel/pyccel/blob/devel/developer_docs/tips_and_tricks.md)
 -   [Scope](https://github.com/pyccel/pyccel/blob/devel/developer_docs/scope.md)
+-   [Type Inference](https://github.com/pyccel/pyccel/blob/devel/developer_docs/type_inference.md)
 -   [Array Ordering](https://github.com/pyccel/pyccel/blob/devel/developer_docs/order_docs.md)
```

### Comparing `pyccel-1.9.1/pyccel.egg-info/SOURCES.txt` & `pyccel-1.9.2/pyccel.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 docs/function-pointers-as-arguments.md
 docs/header-files.md
 docs/installation.md
 docs/ndarrays.md
 docs/numpy-functions.md
 docs/openmp.md
 docs/quickstart.md
+docs/supported-libraries.md
 docs/templates.md
 pyccel/__init__.py
 pyccel/decorators.py
 pyccel/epyccel.py
 pyccel/version.py
 pyccel.egg-info/PKG-INFO
 pyccel.egg-info/SOURCES.txt
@@ -60,14 +61,15 @@
 pyccel/ast/basic.py
 pyccel/ast/bind_c.py
 pyccel/ast/bitwise_operators.py
 pyccel/ast/builtin_imports.py
 pyccel/ast/builtins.py
 pyccel/ast/c_concepts.py
 pyccel/ast/class_defs.py
+pyccel/ast/cmathext.py
 pyccel/ast/core.py
 pyccel/ast/cwrapper.py
 pyccel/ast/datatypes.py
 pyccel/ast/functionalexpr.py
 pyccel/ast/headers.py
 pyccel/ast/internals.py
 pyccel/ast/itertoolsext.py
@@ -77,14 +79,15 @@
 pyccel/ast/numpy_wrapper.py
 pyccel/ast/numpyext.py
 pyccel/ast/omp.py
 pyccel/ast/operators.py
 pyccel/ast/scipyext.py
 pyccel/ast/sympy_helper.py
 pyccel/ast/sysext.py
+pyccel/ast/type_annotations.py
 pyccel/ast/utilities.py
 pyccel/ast/variable.py
 pyccel/codegen/__init__.py
 pyccel/codegen/codegen.py
 pyccel/codegen/pipeline.py
 pyccel/codegen/python_wrapper.py
 pyccel/codegen/utilities.py
@@ -201,27 +204,24 @@
 tests/codegen/ccode/scripts/whiles.py
 tests/codegen/fcode/test_fcode_codegen.py
 tests/codegen/fcode/scripts/CommentBlock.py
 tests/codegen/fcode/scripts/Functional_Stmts.py
 tests/codegen/fcode/scripts/ListComprehension.py
 tests/codegen/fcode/scripts/USELESS_EXPRESSION.py
 tests/codegen/fcode/scripts/arrays.py
-tests/codegen/fcode/scripts/calls.py
-tests/codegen/fcode/scripts/classes.py
 tests/codegen/fcode/scripts/classes_2.py
 tests/codegen/fcode/scripts/classes_3.py
 tests/codegen/fcode/scripts/classes_4.py
 tests/codegen/fcode/scripts/complex_numbers.py
 tests/codegen/fcode/scripts/decorators.py
 tests/codegen/fcode/scripts/decorators_elemental.py
 tests/codegen/fcode/scripts/decorators_pure.py
 tests/codegen/fcode/scripts/decorators_types.py
 tests/codegen/fcode/scripts/expressions.py
 tests/codegen/fcode/scripts/functions_inout.py
-tests/codegen/fcode/scripts/generic_methods.py
 tests/codegen/fcode/scripts/headers.py
 tests/codegen/fcode/scripts/ifs.py
 tests/codegen/fcode/scripts/imports.py
 tests/codegen/fcode/scripts/issue_177.py
 tests/codegen/fcode/scripts/lists.py
 tests/codegen/fcode/scripts/loops.py
 tests/codegen/fcode/scripts/macros.py
@@ -254,14 +254,15 @@
 tests/epyccel/test_epyccel_augassign.py
 tests/epyccel/test_epyccel_complex_func.py
 tests/epyccel/test_epyccel_decorators.py
 tests/epyccel/test_epyccel_default_args.py
 tests/epyccel/test_epyccel_division.py
 tests/epyccel/test_epyccel_functions.py
 tests/epyccel/test_epyccel_generators.py
+tests/epyccel/test_epyccel_headers.py
 tests/epyccel/test_epyccel_mod.py
 tests/epyccel/test_epyccel_modules.py
 tests/epyccel/test_epyccel_multi_rank.py
 tests/epyccel/test_epyccel_openmp.py
 tests/epyccel/test_epyccel_optional_args.py
 tests/epyccel/test_epyccel_pow.py
 tests/epyccel/test_epyccel_python_annotations.py
@@ -315,22 +316,23 @@
 tests/epyccel/modules/numpy_sign.py
 tests/epyccel/modules/openmp.py
 tests/epyccel/modules/pointers.py
 tests/epyccel/modules/python_annotations.py
 tests/epyccel/modules/strings.py
 tests/epyccel/modules/tuples.py
 tests/epyccel/modules/types.py
+tests/epyccel/recognised_functions/test_cmath_funcs.py
 tests/epyccel/recognised_functions/test_epyccel_pyc_math.py
 tests/epyccel/recognised_functions/test_math_funcs.py
 tests/epyccel/recognised_functions/test_numpy_funcs.py
 tests/epyccel/recognised_functions/test_numpy_types.py
 tests/errors/test_errors.py
 tests/errors/codegen/fortran/FORTRAN_ALLOCATABLE_IN_EXPRESSION.py
 tests/errors/codegen/fortran/randint.py
-tests/errors/known_bugs/context.py
+tests/errors/known_bugs/calls.py
 tests/errors/known_bugs/cross.py
 tests/errors/known_bugs/dicts.py
 tests/errors/known_bugs/ex3.py
 tests/errors/known_bugs/ex4.py
 tests/errors/known_bugs/header_interface.py
 tests/errors/known_bugs/inheritance.py
 tests/errors/known_bugs/lambdas.py
@@ -352,14 +354,15 @@
 tests/errors/semantic/blocking/OPENMP_loop_check.py
 tests/errors/semantic/blocking/OPENMP_parallel_for_check.py
 tests/errors/semantic/blocking/OPENMP_simd_check.py
 tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_decorator.py
 tests/errors/semantic/blocking/RECURSIVE_RESULTS_REQUIRED_header.py
 tests/errors/semantic/blocking/TEMPLATE_WRONG_TYPE_CALL.py
 tests/errors/semantic/blocking/TOO_MANY_ARGS.py
+tests/errors/semantic/blocking/TUPLE_WITH_INCOHERENT_RANKS.py
 tests/errors/semantic/blocking/UNDEFINED_LAMBDA_FUNCTION.py
 tests/errors/semantic/blocking/UNDEFINED_LAMBDA_VARIABLE.py
 tests/errors/semantic/blocking/UNRECOGNISED_FUNCTION_CALL.py
 tests/errors/semantic/blocking/ex1.py
 tests/errors/semantic/blocking/ex2.py
 tests/errors/semantic/blocking/ex3.py
 tests/errors/semantic/blocking/ex4.py
@@ -551,16 +554,19 @@
 tests/pyccel/scripts/runtest_type_print.py
 tests/pyccel/scripts/asserts/unvalid_assert1.py
 tests/pyccel/scripts/asserts/unvalid_assert2.py
 tests/pyccel/scripts/asserts/unvalid_assert3.py
 tests/pyccel/scripts/asserts/valid_assert.py
 tests/pyccel/scripts/classes/classes.py
 tests/pyccel/scripts/classes/classes_1.py
-tests/pyccel/scripts/classes/classes_2_C.py
+tests/pyccel/scripts/classes/classes_2.py
+tests/pyccel/scripts/classes/classes_3.py
+tests/pyccel/scripts/classes/classes_4.py
 tests/pyccel/scripts/classes/classes_5.py
+tests/pyccel/scripts/classes/classes_6.py
 tests/pyccel/scripts/classes/generic_methods.py
 tests/pyccel/scripts/exits/empty_exit.py
 tests/pyccel/scripts/exits/negative_exit1.py
 tests/pyccel/scripts/exits/negative_exit2.py
 tests/pyccel/scripts/exits/positive_exit1.py
 tests/pyccel/scripts/exits/positive_exit2.py
 tests/pyccel/scripts/exits/positive_exit3.py
@@ -605,15 +611,14 @@
 tests/pyccel/scripts/import_syntax/import_mod_user.py
 tests/pyccel/scripts/import_syntax/import_mod_user_func.py
 tests/pyccel/scripts/import_syntax/user_mod.py
 tests/pyccel/scripts/import_syntax/user_mod2.py
 tests/pyccel/scripts/numpy/numpy_kernels.py
 tests/pyccel/scripts/numpy/numpy_sign.py
 tests/semantic/test_semantic.py
-tests/semantic/scripts/calls.py
 tests/semantic/scripts/classes.py
 tests/semantic/scripts/expressions.py
 tests/semantic/scripts/functions.py
 tests/semantic/scripts/ifs.py
 tests/semantic/scripts/imports.py
 tests/semantic/scripts/lists.py
 tests/semantic/scripts/loops.py
@@ -645,10 +650,9 @@
 tests/syntax/scripts/tuples.py
 tests/syntax/scripts/whiles.py
 tests/syntax/scripts/zeros.py
 tests/warnings/test_warnings.py
 tests/warnings/semantic/DECORATOR_WRONG_NUMBER_TYPES.py
 tests/warnings/semantic/FOUND_DUPLICATED_IMPORT.py
 tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES.py
-tests/warnings/semantic/HEADER_WRONG_NUMBER_TYPES_INCLASS.py
 tests/warnings/semantic/UNDEFINED_DECORATOR.py
 tests/warnings/semantic/UNDEFINED_DECORATORS.py
```

### Comparing `pyccel-1.9.1/setup.cfg` & `pyccel-1.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/setup.py` & `pyccel-1.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/ast/test_basic.py` & `pyccel-1.9.2/tests/ast/test_basic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/ccode/scripts/arrays.py` & `pyccel-1.9.2/tests/codegen/ccode/scripts/arrays.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/ccode/scripts/arrays_create.py` & `pyccel-1.9.2/tests/codegen/ccode/scripts/arrays_create.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/ccode/scripts/arrays_indexing.py` & `pyccel-1.9.2/tests/codegen/ccode/scripts/arrays_indexing.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/ccode/scripts/arrays_pointers.py` & `pyccel-1.9.2/tests/codegen/ccode/scripts/arrays_pointers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/ccode/scripts/arrays_slicing.py` & `pyccel-1.9.2/tests/codegen/ccode/scripts/arrays_slicing.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/ccode/scripts/functions.py` & `pyccel-1.9.2/tests/codegen/ccode/scripts/functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/ccode/scripts/ifs.py` & `pyccel-1.9.2/tests/codegen/ccode/scripts/ifs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/ccode/scripts/loops.py` & `pyccel-1.9.2/tests/codegen/ccode/scripts/loops.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/ccode/test_ccode_codegen.py` & `pyccel-1.9.2/tests/codegen/ccode/test_ccode_codegen.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/CommentBlock.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/CommentBlock.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/Functional_Stmts.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/Functional_Stmts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/classes_4.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/classes_4.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 # pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 #An example of a class
-#$ header class Shape(public)
-#$ header method __init__(Shape, double, double)
-#$ header method area(Shape) results(double)
-#$ header method perimeter(Shape) results(double)
-#$ header method describe(Shape,str)
-#$ header method authorName(Shape,str)
-#$ header method scaleSize(Shape, double)
 
 class Shape:
 
-    def __init__(self, x, y):
+    def __init__(self : 'Shape', x : float, y : float):
         self.x = x
         self.y = y
         self.description = "This shape has not been described yet"
         self.author = "Nobody has claimed to make this shape yet"
 
-    def area(self):
+    def area(self : 'Shape') -> float:
         y = self.x * self.y
         return y
 
-    def perimeter(self):
+    def perimeter(self : 'Shape') -> float:
         x = 2 * self.x + 2 * self.y
         return x
 
-    def describe(self, text):
+    def describe(self : 'Shape', text : str):
         self.description = text
 
-    def authorName(self, text):
+    def authorName(self : 'Shape', text : str):
         self.author = text
 
-    def scaleSize(self, scale):
+    def scaleSize(self : 'Shape', scale : float):
         self.x = self.x * scale
         self.y = self.y * scale
 
 rectangle = Shape(100., 45.)
 #finding the area of your rectangle:
 print(rectangle.area())
```

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/decorators.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,35 @@
 # pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 #An example of a class
-#$ header class Shape(public)
-#$ header method __init__(Shape, double, double)
-#$ header method area(Shape) results(double)
-#$ header method perimeter(Shape) results(double)
-#$ header method describe(Shape,str)
-#$ header method authorName(Shape,str)
-#$ header method scaleSize(Shape, double)
 
 class Shape:
 
-    def __init__(self, x, y):
+    def __init__(self : 'Shape', x : float, y : float):
         self.x = x
         self.y = y
         self.description = "This shape has not been described yet"
         self.author = "Nobody has claimed to make this shape yet"
 
     @property
-    def area(self):
+    def area(self : 'Shape') -> float:
         y = self.x * self.y
         return y
 
     @property
-    def perimeter(self):
+    def perimeter(self : 'Shape') -> float:
         x = 2 * self.x + 2 * self.y
         return x
 
-    def describe(self, text):
+    def describe(self : 'Shape', text : str):
         self.description = text
 
-    def authorName(self, text):
+    def authorName(self : 'Shape', text : str):
         self.author = text
 
-    def scaleSize(self, scale):
+    def scaleSize(self : 'Shape', scale : float):
         self.x = self.x * scale
         self.y = self.y * scale
 
 rectangle = Shape(100., 45.)
 #finding the area of your rectangle:
 print(rectangle.area)
```

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/decorators_types.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/decorators_types.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/functions_inout.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/functions_inout.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/ifs.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/ifs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/loops.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/loops.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/macros.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/macros.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/matrix_assembly.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/matrix_assembly.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/matrix_mul.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/matrix_mul.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/numpyext.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/numpyext.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/precision.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/precision.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/scripts/recursive_functions.py` & `pyccel-1.9.2/tests/codegen/fcode/scripts/recursive_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/fcode/test_fcode_codegen.py` & `pyccel-1.9.2/tests/codegen/fcode/test_fcode_codegen.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/pycode/scripts/loops.py` & `pyccel-1.9.2/tests/codegen/pycode/scripts/loops.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/codegen/pycode/test_pycode_codegen.py` & `pyccel-1.9.2/tests/codegen/pycode/test_pycode_codegen.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/complexity/test_complexity.py` & `pyccel-1.9.2/tests/complexity/test_complexity.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/conftest.py` & `pyccel-1.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/Module_5.py` & `pyccel-1.9.2/tests/epyccel/modules/Module_5.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/Module_6.py` & `pyccel-1.9.2/tests/epyccel/modules/Module_6.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/Module_7.py` & `pyccel-1.9.2/tests/epyccel/modules/Module_7.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/array_consts.py` & `pyccel-1.9.2/tests/epyccel/modules/array_consts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/arrays.py` & `pyccel-1.9.2/tests/epyccel/modules/arrays.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/augassign.py` & `pyccel-1.9.2/tests/epyccel/modules/augassign.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/base.py` & `pyccel-1.9.2/tests/epyccel/modules/base.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/bitwise.py` & `pyccel-1.9.2/tests/epyccel/modules/bitwise.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/call_user_defined_funcs.py` & `pyccel-1.9.2/tests/epyccel/modules/call_user_defined_funcs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/complex_func.py` & `pyccel-1.9.2/tests/epyccel/modules/complex_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/external_functions.py` & `pyccel-1.9.2/tests/epyccel/modules/external_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/functionals.py` & `pyccel-1.9.2/tests/epyccel/modules/functionals.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/generic_functions.py` & `pyccel-1.9.2/tests/epyccel/modules/generic_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/generic_functions_2.py` & `pyccel-1.9.2/tests/epyccel/modules/generic_functions_2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/highorder_functions.py` & `pyccel-1.9.2/tests/epyccel/modules/highorder_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/loops.py` & `pyccel-1.9.2/tests/epyccel/modules/loops.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/mpi_collective.py` & `pyccel-1.9.2/tests/epyccel/modules/mpi_collective.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/multi_rank.py` & `pyccel-1.9.2/tests/epyccel/modules/multi_rank.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/numpy_sign.py` & `pyccel-1.9.2/tests/epyccel/modules/numpy_sign.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/openmp.py` & `pyccel-1.9.2/tests/epyccel/modules/openmp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/pointers.py` & `pyccel-1.9.2/tests/epyccel/modules/pointers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/python_annotations.py` & `pyccel-1.9.2/tests/epyccel/modules/python_annotations.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/strings.py` & `pyccel-1.9.2/tests/epyccel/modules/strings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/tuples.py` & `pyccel-1.9.2/tests/epyccel/modules/tuples.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/modules/types.py` & `pyccel-1.9.2/tests/epyccel/modules/types.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py` & `pyccel-1.9.2/tests/epyccel/recognised_functions/test_epyccel_pyc_math.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/recognised_functions/test_math_funcs.py` & `pyccel-1.9.2/tests/epyccel/recognised_functions/test_math_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # pylint: disable=missing-function-docstring, missing-module-docstring
+from math import nan, inf, modf
+import os
+import sys
 import pytest
 from numpy.random import rand, randint, uniform
 from numpy import isclose
 
 from pyccel.epyccel import epyccel
-from pyccel.decorators import types
+from pyccel.decorators import template
 
-import sys
 
 RTOL = 1e-13
 ATOL = 1e-14
 
 max_float = 3.40282e5        # maximum positive float
 min_float = sys.float_info.min  # Minimum positive float
 
@@ -534,25 +536,25 @@
         pytest.param("c", marks = pytest.mark.c),
         pytest.param("fortran", marks = [
             pytest.mark.xfail(reason="isfinite not implemented"),
             pytest.mark.fortran]
         )
     )
 )
+@pytest.mark.skipif(os.environ.get('PYCCEL_DEFAULT_COMPILER', None) == 'intel', reason='Nan not correctly passed to intel function')
 def test_isfinite_call(language): # isfinite
     def isfinite_call(x : 'float'):
         from math import isfinite
         return isfinite(x)
 
     f1 = epyccel(isfinite_call, language = language)
     x = rand()
 
     assert(isfinite_call(x) == f1(x))
 
-    from math import nan, inf
     # Test not a number
     assert(isfinite_call(nan) == f1(nan))
     # Test infinite number
     assert(isfinite_call(inf) == f1(inf))
     # Test negative infinite number
     assert(isfinite_call(-inf) == f1(-inf))
 
@@ -571,15 +573,14 @@
         return isinf(x)
 
     f1 = epyccel(isinf_call, language = language)
     x = rand()
 
     assert(isinf_call(x) == f1(x))
 
-    from math import nan, inf
     # Test not a number
     assert(isinf_call(nan) == f1(nan))
     # Test infinite number
     assert(isinf_call(inf) == f1(inf))
     # Test negative infinite number
     assert(isinf_call(-inf) == f1(-inf))
 
@@ -591,15 +592,14 @@
         return isnan(x)
 
     f1 = epyccel(isnan_call, language = language)
     x = rand()
 
     assert(isnan_call(x) == f1(x))
 
-    from math import nan, inf
     # Test not a number
     assert(isnan_call(nan) == f1(nan))
     # Test infinite number
     assert(isnan_call(inf) == f1(inf))
     # Test negative infinite number
     assert(isnan_call(-inf) == f1(-inf))
 
@@ -929,17 +929,16 @@
     x = uniform(low=low, high=high)
     y = uniform(low=low, high=high)
     assert(isclose(f2(x,y) ,  log10_phrase(x,y), rtol=RTOL, atol=ATOL))
 
 #--------------------------------- Pow function ------------------------------#
 
 def test_pow_call(language):
-    @types('real', 'real')
-    @types('real', 'int')
-    def pow_call(x, y):
+    @template('T', [int, float])
+    def pow_call(x : float, y : 'T'):
         from math import pow as my_pow
         return my_pow(x, y)
 
     f1 = epyccel(pow_call, language = language)
     high = 10
     # case 1: x > 0
     x = uniform(low=min_float)
@@ -1121,15 +1120,14 @@
         return gamma(x)
 
     f1 = epyccel(gamma_call, language = language)
 
     # Domain ]0, +inf[ || (x < 0 and x.fraction not null)
     x = uniform(low=min_float)
     assert(isclose(f1(x) , gamma_call(x), rtol=RTOL, atol=ATOL))
-    from math import modf
     # make fractional part different from zero to test negative case
     if modf(x)[0] == 0:
         x += - 0.1
     assert(isclose(f1(-x) , gamma_call(-x), rtol=RTOL, atol=ATOL))
 
     assert isinstance(f1(x), type(gamma_call(x)))
 
@@ -1154,15 +1152,14 @@
         return lgamma(x)
 
     f1 = epyccel(lgamma_call, language = language)
 
     # Domain ]0, +inf[ || (x < 0 and x.fraction not null)
     x = uniform(low=min_float)
     assert(isclose(f1(x) , lgamma_call(x), rtol=RTOL, atol=ATOL))
-    from math import modf
     _, f = modf(x)
     # make fractional part different from zero to test negative case
     if f == 0:
         x += - 0.1
     assert(isclose(f1(-x) , lgamma_call(-x), rtol=RTOL, atol=ATOL))
     assert isinstance(f1(x), type(lgamma_call(x)))
```

### Comparing `pyccel-1.9.1/tests/epyccel/recognised_functions/test_numpy_funcs.py` & `pyccel-1.9.2/tests/epyccel/recognised_functions/test_numpy_funcs.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/recognised_functions/test_numpy_types.py` & `pyccel-1.9.2/tests/epyccel/recognised_functions/test_numpy_types.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_array_as_func_args.py` & `pyccel-1.9.2/tests/epyccel/test_array_as_func_args.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_arrays.py` & `pyccel-1.9.2/tests/epyccel/test_arrays.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import numpy as np
 from numpy import iinfo
 from numpy.random import randint
 
 from pyccel.epyccel import epyccel
 from modules        import arrays
 
+RTOL = 1e-12
+ATOL = 1e-16
+
 def check_array_equal(a, b):
     """
     Check that two arrays are equal.
 
     Check that two arrays are equal. To be equal they must have the same
     shape, dtype, and order.
     """
@@ -1098,15 +1101,15 @@
     x1 = np.array( [1.,2.,3.] )
     x2 = np.copy(x1)
     a = 5.
 
     f1(x1, a)
     f2(x2, a)
 
-    assert np.array_equal( x1, x2 )
+    assert np.allclose(x1, x2, rtol=RTOL, atol=ATOL)
 
 def test_array_float_1d_scalar_mod(language):
     f1 = arrays.array_float_1d_scalar_mod
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [1.,2.,3.] )
     x2 = np.copy(x1)
@@ -1269,15 +1272,15 @@
     x1 = np.array( [[1.,2.,3.], [4.,5.,6.]] )
     x2 = np.copy(x1)
     a = 5.
 
     f1(x1, a)
     f2(x2, a)
 
-    assert np.array_equal( x1, x2 )
+    assert np.allclose(x1, x2, rtol=RTOL, atol=ATOL)
 
 def test_array_float_2d_C_scalar_mod(language):
 
     f1 = arrays.array_float_2d_C_scalar_mod
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [[1.,2.,3.], [4.,5.,6.]] )
@@ -1472,15 +1475,15 @@
     x1 = np.array( [[1.,2.,3.], [4.,5.,6.]], order='F' )
     x2 = np.copy(x1)
     a = 5.
 
     f1(x1, a)
     f2(x2, a)
 
-    assert np.array_equal( x1, x2 )
+    assert np.allclose(x1, x2, rtol=RTOL, atol=ATOL)
 
 def test_array_float_2d_F_scalar_mod(language):
 
     f1 = arrays.array_float_2d_F_scalar_mod
     f2 = epyccel( f1 , language = language)
 
     x1 = np.array( [[1.,2.,3.], [4.,5.,6.]], order='F' )
@@ -1798,21 +1801,21 @@
     x2 = f2()
     assert np.equal( x1, x2 )
 
 def test_multiple_stack_array_1(language):
 
     f1 = arrays.multiple_stack_array_1
     f2 = epyccel(f1, language = language)
-    assert np.equal(f1(), f2())
+    assert np.allclose(f1(), f2(), rtol=RTOL, atol=ATOL)
 
 def test_multiple_stack_array_2(language):
 
     f1 = arrays.multiple_stack_array_2
     f2 = epyccel(f1, language = language)
-    assert np.equal(f1(), f2())
+    assert np.allclose(f1(), f2(), rtol=RTOL, atol=ATOL)
 
 #==============================================================================
 # TEST: 2D Stack ARRAYS OF REAL
 #==============================================================================
 
 def test_array_float_sum_2d_stack_array(language):
 
@@ -1830,21 +1833,21 @@
     x2 = f2()
     assert np.equal( x1, x2 )
 
 def test_multiple_2d_stack_array_1(language):
 
     f1 = arrays.multiple_2d_stack_array_1
     f2 = epyccel(f1, language = language)
-    assert np.equal(f1(), f2())
+    assert np.allclose(f1(), f2(), rtol=RTOL, atol=ATOL)
 
 def test_multiple_2d_stack_array_2(language):
 
     f1 = arrays.multiple_2d_stack_array_2
     f2 = epyccel(f1, language = language)
-    assert np.equal(f1(), f2())
+    assert np.allclose(f1(), f2(), rtol=RTOL, atol=ATOL)
 
 #==============================================================================
 # TEST: Product and matrix multiplication
 #==============================================================================
 @pytest.mark.parametrize( 'language', [
         pytest.param("c", marks = [
             pytest.mark.skip(reason="prod not implemented in c"),
@@ -3565,16 +3568,14 @@
     f1 = arrays.arrs_2d_negative_index
     f2 = epyccel(f1, language = language)
     assert np.allclose(f1(), f2(), rtol=RTOL, atol=ATOL)
 
 #==============================================================================
 # TEST : NUMPY ARANGE
 #==============================================================================
-RTOL = 1e-12
-ATOL = 1e-16
 
 def test_numpy_arange_one_arg(language):
     f1 = arrays.arr_arange_1
     f2 = epyccel(f1, language = language)
     assert f1() == f2()
 
 def test_numpy_arange_two_arg(language):
```

### Comparing `pyccel-1.9.1/tests/epyccel/test_arrays_multiple_assignments.py` & `pyccel-1.9.2/tests/epyccel/test_arrays_multiple_assignments.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_base.py` & `pyccel-1.9.2/tests/epyccel/test_base.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_bitwise.py` & `pyccel-1.9.2/tests/epyccel/test_bitwise.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_builtins.py` & `pyccel-1.9.2/tests/epyccel/test_builtins.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_class_expressions.py` & `pyccel-1.9.2/tests/epyccel/test_class_expressions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_compare_expressions.py` & `pyccel-1.9.2/tests/epyccel/test_compare_expressions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_default_precision_template.py` & `pyccel-1.9.2/tests/epyccel/test_default_precision_template.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_docstrings.py` & `pyccel-1.9.2/tests/epyccel/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_IfTernaryOperator.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_IfTernaryOperator.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_augassign.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_augassign.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_complex_func.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_complex_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_decorators.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_decorators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_default_args.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_default_args.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_division.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_division.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_functions.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_generators.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_generators.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_mod.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_mod.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_modules.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_modules.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_multi_rank.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_multi_rank.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_openmp.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_openmp.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,14 +376,15 @@
     set_num_threads = epyccel(openmp.set_num_threads, fflags = '-Wall', accelerators=['openmp'], language=language)
     set_num_threads(4)
     x = random.randint(20, size=(5))
 
     assert f1(x) == np.sum(x)
 
 @pytest.mark.external
+@pytest.mark.xfail(os.environ.get('PYCCEL_DEFAULT_COMPILER', None) == 'intel', reason='#1539')
 def test_omp_range_sum_critical(language):
     f1 = epyccel(openmp.omp_range_sum_critical, fflags = '-Wall', accelerators=['openmp'], language=language)
 
     for _ in range(0, 4):
         x = random.randint(10, 1000)
         assert f1(x) == openmp.omp_range_sum_critical(x)
```

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_optional_args.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_optional_args.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_pow.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_pow.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_python_annotations.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_python_annotations.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_return_arrays.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_return_arrays.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_sign.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_sign.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_transpose.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_transpose.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_epyccel_types.py` & `pyccel-1.9.2/tests/epyccel/test_epyccel_types.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_external_functions.py` & `pyccel-1.9.2/tests/epyccel/test_external_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_functionals.py` & `pyccel-1.9.2/tests/epyccel/test_functionals.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_generic_functions.py` & `pyccel-1.9.2/tests/epyccel/test_generic_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_higherorder_functions.py` & `pyccel-1.9.2/tests/epyccel/test_higherorder_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_imports.py` & `pyccel-1.9.2/tests/epyccel/test_imports.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_kind.py` & `pyccel-1.9.2/tests/epyccel/test_kind.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_loops.py` & `pyccel-1.9.2/tests/epyccel/test_loops.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_mpi_collective.py` & `pyccel-1.9.2/tests/epyccel/test_mpi_collective.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_mpi_point_to_point.py` & `pyccel-1.9.2/tests/epyccel/test_mpi_point_to_point.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_multiple_results.py` & `pyccel-1.9.2/tests/epyccel/test_multiple_results.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_parallel_epyccel.py` & `pyccel-1.9.2/tests/epyccel/test_parallel_epyccel.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_pointers.py` & `pyccel-1.9.2/tests/epyccel/test_pointers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_return.py` & `pyccel-1.9.2/tests/epyccel/test_return.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_strings.py` & `pyccel-1.9.2/tests/epyccel/test_strings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/test_tuples.py` & `pyccel-1.9.2/tests/epyccel/test_tuples.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/epyccel/utilities.py` & `pyccel-1.9.2/tests/epyccel/utilities.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/errors/known_bugs/ex4.py` & `pyccel-1.9.2/tests/errors/known_bugs/ex4.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 # coding: utf-8
 
-#$ header class Square(public)
-#$ header method __init__(Square, int [:], int [:], int [:])
-#$ header method __del__(Square)
-
 class Square(object):
-    def __init__(self, starts, stops, steps):
+    def __init__(self : 'Square', starts : 'int[:]', stops : 'int[:]', steps : 'int[:]'):
         self.starts = starts
         self.stops  = stops
         self.steps  = steps
 
         self.rx = range(self.starts[0], self.stops[0], self.steps[0])
         self.ry = range(self.starts[1], self.stops[1], self.steps[1])
 
         self.indices = tensor (self.rx, self.ry)
 
-    def __del__(self):
+    def __del__(self : 'Square'):
         pass
 
 starts = zeros(2, int)
 stops  = zeros(2, int)
 steps  = ones(2, int)
 
 stops[0] = 4
```

### Comparing `pyccel-1.9.1/tests/errors/known_bugs/header_interface.py` & `pyccel-1.9.2/tests/errors/known_bugs/header_interface.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/errors/semantic/blocking/unknown_method.py` & `pyccel-1.9.2/tests/pyccel/scripts/classes/generic_methods.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# pylint: disable=missing-class-docstring,  missing-function-docstring, missing-module-docstring
-#$ header class Point(public)
-#$ header method __init__(Point, double, double)
-#$ header method __del__(Point)
-#$ header method translate(Point, double, double)
+# pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
+from pyccel.decorators import template
 
 class Point(object):
-    def __init__(self, x, y):
+    def __init__(self : 'Point', x : float, y : float):
         self.x = x
         self.y = y
 
-    def __del__(self):
+    def __del__(self : 'Point'):
         pass
 
-    def translate(self, a, b):
+    @template('T', [int, float])
+    def translate(self : 'Point', a : 'T', b : 'T'):
         self.x = self.x + a
         self.y = self.y + b
 
 if __name__ == '__main__':
     p = Point(0.0, 0.0)
     x=p.x
     p.x=x
@@ -24,13 +22,11 @@
     a = p.x - 2
     a = 2 * p.x - 2
     a = 2 * (p.x + 6) - 2
 
     p.y = a + 5
     p.y = p.x + 5
 
-    p.translated(1.0, 2.0)
+    p.translate(1.0, 2.0)
 
     print(p.x, p.y)
     print(a)
-
-    del p
```

### Comparing `pyccel-1.9.1/tests/errors/test_errors.py` & `pyccel-1.9.2/tests/errors/test_errors.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/lapack/ex1.py` & `pyccel-1.9.2/tests/external/scripts/lapack/ex1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/mpi4py/bcast.py` & `pyccel-1.9.2/tests/external/scripts/mpi4py/bcast.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/mpi4py/bugs/ex6.py` & `pyccel-1.9.2/tests/external/scripts/mpi4py/bugs/ex6.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/mpi4py/bugs/ex8.py` & `pyccel-1.9.2/tests/external/scripts/mpi4py/bugs/ex8.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/mpi4py/gather.py` & `pyccel-1.9.2/tests/external/scripts/mpi4py/gather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/mpi4py/np_Bcast.py` & `pyccel-1.9.2/tests/external/scripts/mpi4py/np_Bcast.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/mpi4py/np_Gather.py` & `pyccel-1.9.2/tests/external/scripts/mpi4py/np_Gather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/mpi4py/np_Sendrecv.py` & `pyccel-1.9.2/tests/external/scripts/mpi4py/np_Sendrecv.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/mpi4py/np_point_to_point.py` & `pyccel-1.9.2/tests/external/scripts/mpi4py/np_point_to_point.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/mpi4py/np_point_to_point_3.py` & `pyccel-1.9.2/tests/external/scripts/mpi4py/np_point_to_point_3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/scripts/mpi4py/point_to_point_3.py` & `pyccel-1.9.2/tests/external/scripts/mpi4py/point_to_point_3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/external/test_external.py` & `pyccel-1.9.2/tests/external/test_external.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/blas/ex1.py` & `pyccel-1.9.2/tests/internal/scripts/blas/ex1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/blas/ex2.py` & `pyccel-1.9.2/tests/internal/scripts/blas/ex2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/blas/ex3.py` & `pyccel-1.9.2/tests/internal/scripts/blas/ex3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/blas/ex4.py` & `pyccel-1.9.2/tests/internal/scripts/blas/ex4.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/blas/ex5.py` & `pyccel-1.9.2/tests/internal/scripts/blas/ex5.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/lapack/ex1.py` & `pyccel-1.9.2/tests/internal/scripts/lapack/ex1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/allgather.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/allgather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/allreduce.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/allreduce.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/alltoall.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/alltoall.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/bcast.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/bcast.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/column.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/column.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/gather.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/gather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/line.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/line.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/nonblocking.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/nonblocking.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/point_to_point_1.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/point_to_point_1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/point_to_point_2.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/point_to_point_2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/reduce.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/reduce.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/scatter.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/scatter.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/sendrecv.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/sendrecv.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/sendrecv_replace.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/sendrecv_replace.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/split.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/split.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/mpi/who_am_i.py` & `pyccel-1.9.2/tests/internal/scripts/mpi/who_am_i.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/openacc/sum.py` & `pyccel-1.9.2/tests/internal/scripts/openacc/sum.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/openacc/sum_kernels.py` & `pyccel-1.9.2/tests/internal/scripts/openacc/sum_kernels.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/scripts/openmp/ex1.py` & `pyccel-1.9.2/tests/internal/scripts/openmp/ex1.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/internal/test_internal.py` & `pyccel-1.9.2/tests/internal/test_internal.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/bcast.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/bcast.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/bug/ex6.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/bug/ex6.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/bug/ex8.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/bug/ex8.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/gather.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/gather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/mpi4py.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/mpi4py.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/np_Allreduce.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/np_Allreduce.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/np_Bcast.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/np_Bcast.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/np_Gather.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/np_Gather.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/np_Reduce.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/np_Reduce.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/np_Sendrecv.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/np_Sendrecv.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/np_point_to_point.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/np_point_to_point.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/np_point_to_point_2.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/np_point_to_point_2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/np_point_to_point_3.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/np_point_to_point_3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/point_to_point_2.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/point_to_point_2.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/MPI/point_to_point_3.py` & `pyccel-1.9.2/tests/macro/scripts/MPI/point_to_point_3.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/blas/runtest_daxpy.py` & `pyccel-1.9.2/tests/macro/scripts/blas/runtest_daxpy.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/blas/runtest_dgemm.py` & `pyccel-1.9.2/tests/macro/scripts/blas/runtest_dgemm.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/blas/runtest_dgemv.py` & `pyccel-1.9.2/tests/macro/scripts/blas/runtest_dgemv.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/blas/runtest_dger.py` & `pyccel-1.9.2/tests/macro/scripts/blas/runtest_dger.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/blas/runtest_dswap.py` & `pyccel-1.9.2/tests/macro/scripts/blas/runtest_dswap.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/scripts/lapack/runtest_dgbtrf.py` & `pyccel-1.9.2/tests/macro/scripts/lapack/runtest_dgbtrf.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/macro/test_macro.py` & `pyccel-1.9.2/tests/macro/test_macro.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/ndarrays/conftest.py` & `pyccel-1.9.2/tests/ndarrays/conftest.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/ndarrays/leaks_check.py` & `pyccel-1.9.2/tests/ndarrays/leaks_check.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/ndarrays/test_ndarrays.c` & `pyccel-1.9.2/tests/ndarrays/test_ndarrays.c`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/parser/scripts/comments.py` & `pyccel-1.9.2/tests/parser/scripts/comments.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/parser/test_comments.py` & `pyccel-1.9.2/tests/parser/test_comments.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/parser/test_headers.py` & `pyccel-1.9.2/tests/parser/test_headers.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,14 @@
 
 def test_function():
     print (parse(stmts='#$ header function f(float [:], int [:]) results(int)'))
 
 def test_function_static():
     print (parse(stmts='#$ header function static f(float [:], int [:]) results(int)'))
 
-def test_class():
-    print (parse(stmts='#$ header class Square(public)'))
-
 def test_method():
     print (parse(stmts='#$ header method translate(Point, double, double)'))
 
 def test_metavar():
     print (parse(stmts="#$ header metavar module_name='mpi'"))
 
 def test_macro():
@@ -31,11 +28,10 @@
     print (parse(stmts='#$ header macro _dswap(x, y, incx=1, incy=1) := dswap(x.shape, x, incx, y, incy)'))
 
 ######################
 if __name__ == '__main__':
     test_variable()
     test_function()
     test_function_static()
-    test_class()
     test_method()
     test_metavar()
     test_macro()
```

### Comparing `pyccel-1.9.1/tests/preprocess/scripts/omp.py` & `pyccel-1.9.2/tests/preprocess/scripts/omp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/preprocess/test_preprocess.py` & `pyccel-1.9.2/tests/preprocess/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/array_binary_operation.py` & `pyccel-1.9.2/tests/pyccel/scripts/array_binary_operation.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/arrays_view.py` & `pyccel-1.9.2/tests/pyccel/scripts/arrays_view.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/bool_comp.py` & `pyccel-1.9.2/tests/pyccel/scripts/bool_comp.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/c_arrays.py` & `pyccel-1.9.2/tests/pyccel/scripts/c_arrays.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/decorators_inline.py` & `pyccel-1.9.2/tests/pyccel/scripts/decorators_inline.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/default_args_mod.py` & `pyccel-1.9.2/tests/pyccel/scripts/default_args_mod.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/expressions.py` & `pyccel-1.9.2/tests/pyccel/scripts/expressions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/functions.py` & `pyccel-1.9.2/tests/pyccel/scripts/functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/generic_functions.py` & `pyccel-1.9.2/tests/pyccel/scripts/generic_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py` & `pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/hope_ln_python.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py` & `pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/hope_pairwise_python.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py` & `pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/point_spread_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks/quicksort.py` & `pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks/quicksort.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py` & `pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/hope_ln_python.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py` & `pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/hope_pairwise_python.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py` & `pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/point_spread_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py` & `pyccel-1.9.2/tests/pyccel/scripts/hope_benchmarks_decorators/quicksort.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import.py` & `pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import_as.py` & `pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import_as.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py` & `pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import_as_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/import_syntax/from_mod_import_func.py` & `pyccel-1.9.2/tests/pyccel/scripts/import_syntax/from_mod_import_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod.py` & `pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod_as.py` & `pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod_as.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod_as_func.py` & `pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod_as_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/import_syntax/import_mod_func.py` & `pyccel-1.9.2/tests/pyccel/scripts/import_syntax/import_mod_func.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/lapack_subroutine.py` & `pyccel-1.9.2/tests/pyccel/scripts/lapack_subroutine.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/numpy/numpy_kernels.py` & `pyccel-1.9.2/tests/pyccel/scripts/numpy/numpy_kernels.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/numpy/numpy_sign.py` & `pyccel-1.9.2/tests/pyccel/scripts/numpy/numpy_sign.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/print_integers.py` & `pyccel-1.9.2/tests/pyccel/scripts/print_integers.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/print_sp_and_end.py` & `pyccel-1.9.2/tests/pyccel/scripts/print_sp_and_end.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/print_strings.py` & `pyccel-1.9.2/tests/pyccel/scripts/print_strings.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/return_numpy_arrays.py` & `pyccel-1.9.2/tests/pyccel/scripts/return_numpy_arrays.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/runtest_default_args.py` & `pyccel-1.9.2/tests/pyccel/scripts/runtest_default_args.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/runtest_degree_in.py` & `pyccel-1.9.2/tests/pyccel/scripts/runtest_degree_in.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/runtest_generic_functions.py` & `pyccel-1.9.2/tests/pyccel/scripts/runtest_generic_functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/scripts/runtest_multiple_results.py` & `pyccel-1.9.2/tests/pyccel/scripts/runtest_multiple_results.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/pyccel/test_pyccel.py` & `pyccel-1.9.2/tests/pyccel/test_pyccel.py`

 * *Files 1% similar despite different names*

```diff
@@ -858,34 +858,23 @@
 #------------------------------------------------------------------------------
 def test_basic_header():
     filename='scripts/basic_header.pyh'
     cwd = get_abs_path('.')
     compile_pyccel(cwd, filename)
 
 #------------------------------------------------------------------------------
-@pytest.mark.parametrize( "test_file", ["scripts/classes/classes.py",
+@pytest.mark.xdist_incompatible
+@pytest.mark.parametrize( "test_file", ["scripts/classes/generic_methods.py",
+                                        "scripts/classes/classes.py",
                                         "scripts/classes/classes_1.py",
+                                        "scripts/classes/classes_2.py",
+                                        "scripts/classes/classes_3.py",
+                                        "scripts/classes/classes_4.py",
                                         "scripts/classes/classes_5.py",
-                                        "scripts/classes/generic_methods.py",
-                                        ] )
-@pytest.mark.parametrize( 'language', (
-        pytest.param("python", marks = pytest.mark.python),
-        pytest.param("fortran", marks = pytest.mark.fortran)
-    )
-)
-
-def test_classes_f_only( test_file , language):
-    if language == "python":
-        pyccel_test(test_file, language=language)
-    else:
-        pyccel_test(test_file, compile_with_pyccel = False, language=language)
-
-#------------------------------------------------------------------------------
-@pytest.mark.xdist_incompatible
-@pytest.mark.parametrize( "test_file", ["scripts/classes/classes_2_C.py",
+                                        "scripts/classes/classes_6.py",
                                         ] )
 @pytest.mark.parametrize( 'language', (
         pytest.param("python", marks = pytest.mark.python),
         pytest.param("c", marks = pytest.mark.c),
         pytest.param("fortran", marks = pytest.mark.fortran)
     )
 )
```

### Comparing `pyccel-1.9.1/tests/run_tests.bat` & `pyccel-1.9.2/tests/run_tests.bat`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/run_tests_py3.sh` & `pyccel-1.9.2/tests/run_tests_py3.sh`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/semantic/scripts/expressions.py` & `pyccel-1.9.2/tests/semantic/scripts/expressions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/semantic/scripts/functions.py` & `pyccel-1.9.2/tests/semantic/scripts/functions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/semantic/test_semantic.py` & `pyccel-1.9.2/tests/semantic/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/symbolic/scripts/decorator.py` & `pyccel-1.9.2/tests/symbolic/scripts/decorator.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/symbolic/scripts/neural_net.py` & `pyccel-1.9.2/tests/symbolic/scripts/neural_net.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/symbolic/test_symbolic.py` & `pyccel-1.9.2/tests/symbolic/test_symbolic.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/syntax/scripts/Functional_Stmts.py` & `pyccel-1.9.2/tests/syntax/scripts/Functional_Stmts.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/syntax/scripts/class_member_index.py` & `pyccel-1.9.2/tests/syntax/scripts/class_member_index.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 # pylint: disable=missing-function-docstring, missing-module-docstring, missing-class-docstring
 # coding: utf-8
 
-#$ header class Square(public)
-#$ header method __init__(Square, int [:], int [:], int [:])
-#$ header method __del__(Square)
-
 class Square(object):
-    def __init__(self, starts, stops, steps):
+    def __init__(self : 'Square', starts : 'int[:]', stops : 'int[:]', steps : 'int[:]'):
         self.starts = starts
         self.stops  = stops
         self.steps  = steps
 
         self.rx = range(self.starts[0], self.stops[0], self.steps[0])
         self.ry = range(self.starts[1], self.stops[1], self.steps[1])
 
         self.indices = tensor (self.rx, self.ry)
 
-    def __del__(self):
+    def __del__(self : 'Square'):
         pass
 
 starts = zeros(2, int)
 stops  = zeros(2, int)
 steps  = ones(2, int)
 
 stops[0] = 4
```

### Comparing `pyccel-1.9.1/tests/syntax/scripts/expressions.py` & `pyccel-1.9.2/tests/syntax/scripts/expressions.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/syntax/test_syntax.py` & `pyccel-1.9.2/tests/syntax/test_syntax.py`

 * *Files identical despite different names*

### Comparing `pyccel-1.9.1/tests/warnings/test_warnings.py` & `pyccel-1.9.2/tests/warnings/test_warnings.py`

 * *Files identical despite different names*

