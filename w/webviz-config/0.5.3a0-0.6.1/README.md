# Comparing `tmp/webviz-config-0.5.3a0.tar.gz` & `tmp/webviz_config-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webviz-config-0.5.3a0.tar", last modified: Thu Aug  3 06:57:44 2023, max compression
+gzip compressed data, was "webviz_config-0.6.1.tar", last modified: Mon May 13 13:09:36 2024, max compression
```

## Comparing `webviz-config-0.5.3a0.tar` & `webviz_config-0.6.1.tar`

### file list

```diff
@@ -1,239 +1,240 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.784086 webviz-config-0.5.3a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.756086 webviz-config-0.5.3a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.756086 webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.756086 webviz-config-0.5.3a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.github/workflows/webviz-config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)    25925 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/INTRODUCTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)   326542 2023-05-27 00:10:14.000000 webviz-config-0.5.3a0/LICENSE.chromedriver
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-08-03 06:57:44.784086 webviz-config-0.5.3a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13515 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/WEBVIZ_LAYOUT_FRAMEWORK_(WLF).md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.756086 webviz-config-0.5.3a0/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    24118 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/before-after-plugin-actions.png
--rw-r--r--   0 runner    (1001) docker     (123)    16439 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/before-after-settings.png
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/before-after-tabs-views.png
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/high-level-overview.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    59175 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/implement-plugin.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    62309 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/implement-settings-group.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    60748 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/implement-view-element.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    59578 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/implement-view.svg
--rw-r--r--   0 runner    (1001) docker     (123)    70182 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/assets/webviz-layout-overview.png
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/bandit.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.760086 webviz-config-0.5.3a0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/basic_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/basic_example_advanced_menu.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/basic_example_wlf.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/demo_portable.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example-markdown.md
--rwxr-xr-x   0 runner    (1001) docker     (123)    10746 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example.pdf
--rwxr-xr-x   0 runner    (1001) docker     (123)   553912 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example_banner.png
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example_javascript.js
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/examples/example_stylesheet.css
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)    39008 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:57:44.784086 webviz-config-0.5.3a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.760086 webviz-config-0.5.3a0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.760086 webviz-config-0.5.3a0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/data/basic_example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/data/example_data.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_callback_typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_create_themed_layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_data_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_docker_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_example_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_example_wlf_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_plugin_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_plugin_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_portable.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_syntax_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/test_table_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.760086 webviz-config-0.5.3a0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/unit_tests/test_webviz_factory_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/unit_tests/test_webviz_instance_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/tests/unit_tests/test_webviz_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.764086 webviz-config-0.5.3a0/webviz_config/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4905 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_build_webviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    23853 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_config_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.768086 webviz-config-0.5.3a0/webviz_config/_deployment/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/azure_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/azure_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/github_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/interactive_terminal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10125 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/radix.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/radix_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deployment/radix_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_deprecation_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.768086 webviz-config-0.5.3a0/webviz_config/_dockerize/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_dockerize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_dockerize/_create_docker_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_dockerize/_pip_git_url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.768086 webviz-config-0.5.3a0/webviz_config/_docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/_build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/_create_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/open_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.772086 webviz-config-0.5.3a0/webviz_config/_docs/static/
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/INTRODUCTION.md
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-copy-code.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   251818 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-katex.js
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-tabs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   106239 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/docsify.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.772086 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    31136 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_AMS-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8392 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13668 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    29932 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21244 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    22076 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    32312 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21192 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Math-BoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21668 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Math-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    13300 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    11792 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Script-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size1-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size2-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size3-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size4-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16868 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Typewriter-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    22476 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/katex.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/prism-bash.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/prism-python.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/prism-yaml.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/search.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-08-03 06:52:46.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/vue.css
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/webviz-doc.css
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_docs/static/webviz-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_is_reload_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_localhost_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20691 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_plugin_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_shared_settings_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6496 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_theme_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_user_data_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_user_preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_webviz_settings_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/_write_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     9358 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/common_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/deprecation_decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_banner_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_data_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_embed_pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_data_download.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_portable.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_tour.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/_shared_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/_text_view_element.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7182 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/_view.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_markdown.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_pivot_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_syntax_highlighter.py
--rw-r--r--   0 runner    (1001) docker     (123)    20735 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/generic_plugins/_table_plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/plugins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/static/
--rwxr-xr-x   0 runner    (1001) docker     (123)       37 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/static/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.776086 webviz-config-0.5.3a0/webviz_config/static/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/static/assets/webviz_config.css
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/static/assets/webviz_layout.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.780086 webviz-config-0.5.3a0/webviz_config/templates/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2649 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/Dockerfile.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/README.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/argument_deprecations.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/copy_data_template.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/feedback.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/plugin_deprecations.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/plugin_docs.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/radixconfig.yaml.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/sidebar.md.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/webviz-doc.js.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/templates/webviz_template.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.780086 webviz-config-0.5.3a0/webviz_config/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/testing/_composite.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/testing/_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/testing/_webviz_ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.780086 webviz-config-0.5.3a0/webviz_config/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/themes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/themes/_default_theme.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.780086 webviz-config-0.5.3a0/webviz_config/themes/default_assets/
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/themes/default_assets/default_theme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.780086 webviz-config-0.5.3a0/webviz_config/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_available_port.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_callback_typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_dash_component_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_deprecate_webviz_settings_attribute_in_dash_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_localhost_open_browser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_silence_flask_startup.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/_str_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/utils/terminal_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3577 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_factory_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_instance_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.784086 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_layout_base_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_layout_unique_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_settings_group_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)    24056 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-08-03 06:52:44.000000 webviz-config-0.5.3a0/webviz_config/webviz_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 06:57:44.764086 webviz-config-0.5.3a0/webviz_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7440 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 06:53:03.000000 webviz-config-0.5.3a0/webviz_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-03 06:57:44.000000 webviz-config-0.5.3a0/webviz_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.483061 webviz_config-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.443061 webviz_config-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.443061 webviz_config-0.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-13 13:05:46.000000 webviz_config-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 13:05:46.000000 webviz_config-0.6.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-13 13:05:46.000000 webviz_config-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-13 13:05:46.000000 webviz_config-0.6.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.443061 webviz_config-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-13 13:05:46.000000 webviz_config-0.6.1/.github/workflows/webviz-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 13:05:46.000000 webviz_config-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 13:05:46.000000 webviz_config-0.6.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)    20081 2024-05-13 13:05:46.000000 webviz_config-0.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-13 13:05:46.000000 webviz_config-0.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    25925 2024-05-13 13:05:46.000000 webviz_config-0.6.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10699 2024-05-13 13:05:46.000000 webviz_config-0.6.1/INTRODUCTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-13 13:05:46.000000 webviz_config-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   326542 2023-05-27 00:10:14.000000 webviz_config-0.6.1/LICENSE.chromedriver
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-05-13 13:09:36.483061 webviz_config-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6063 2024-05-13 13:05:46.000000 webviz_config-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-13 13:05:46.000000 webviz_config-0.6.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13515 2024-05-13 13:05:46.000000 webviz_config-0.6.1/WEBVIZ_LAYOUT_FRAMEWORK_(WLF).md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.447061 webviz_config-0.6.1/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    24118 2024-05-13 13:05:46.000000 webviz_config-0.6.1/assets/before-after-plugin-actions.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16439 2024-05-13 13:05:46.000000 webviz_config-0.6.1/assets/before-after-settings.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-05-13 13:05:46.000000 webviz_config-0.6.1/assets/before-after-tabs-views.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10252 2024-05-13 13:05:46.000000 webviz_config-0.6.1/assets/high-level-overview.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59175 2024-05-13 13:05:46.000000 webviz_config-0.6.1/assets/implement-plugin.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    62309 2024-05-13 13:05:46.000000 webviz_config-0.6.1/assets/implement-settings-group.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    60748 2024-05-13 13:05:46.000000 webviz_config-0.6.1/assets/implement-view-element.svg
+-rwxr-xr-x   0 runner    (1001) docker     (127)    59578 2024-05-13 13:05:46.000000 webviz_config-0.6.1/assets/implement-view.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    70182 2024-05-13 13:05:46.000000 webviz_config-0.6.1/assets/webviz-layout-overview.png
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-13 13:05:46.000000 webviz_config-0.6.1/bandit.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.451061 webviz_config-0.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-05-13 13:05:46.000000 webviz_config-0.6.1/examples/basic_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-13 13:05:46.000000 webviz_config-0.6.1/examples/basic_example_advanced_menu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-13 13:05:46.000000 webviz_config-0.6.1/examples/basic_example_wlf.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-13 13:05:46.000000 webviz_config-0.6.1/examples/demo_portable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-13 13:05:46.000000 webviz_config-0.6.1/examples/example-markdown.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10746 2024-05-13 13:05:46.000000 webviz_config-0.6.1/examples/example.pdf
+-rwxr-xr-x   0 runner    (1001) docker     (127)   553912 2024-05-13 13:05:46.000000 webviz_config-0.6.1/examples/example_banner.png
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 13:05:46.000000 webviz_config-0.6.1/examples/example_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-13 13:05:46.000000 webviz_config-0.6.1/examples/example_javascript.js
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:05:46.000000 webviz_config-0.6.1/examples/example_stylesheet.css
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-13 13:05:46.000000 webviz_config-0.6.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)    39008 2024-05-13 13:05:46.000000 webviz_config-0.6.1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-13 13:05:46.000000 webviz_config-0.6.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 13:05:46.000000 webviz_config-0.6.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:09:36.483061 webviz_config-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4772 2024-05-13 13:05:46.000000 webviz_config-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.451061 webviz_config-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.451061 webviz_config-0.6.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/data/basic_example.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/data/example_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     6773 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_callback_typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_create_themed_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_data_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_docker_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_example_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_example_wlf_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_plugin_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_plugin_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_portable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_syntax_highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/test_table_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.455061 webviz_config-0.6.1/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/unit_tests/test_webviz_factory_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/unit_tests/test_webviz_instance_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-13 13:05:46.000000 webviz_config-0.6.1/tests/unit_tests/test_webviz_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.459061 webviz_config-0.6.1/webviz_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_build_webviz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23853 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_config_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.463061 webviz_config-0.6.1/webviz_config/_deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16538 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_deployment/azure_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_deployment/azure_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_deployment/github_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_deployment/interactive_terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_deployment/radix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_deployment/radix_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_deployment/radix_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_deprecation_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.463061 webviz_config-0.6.1/webviz_config/_dockerize/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_dockerize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_dockerize/_create_docker_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_dockerize/_pip_git_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.463061 webviz_config-0.6.1/webviz_config/_docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10623 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_docs/_build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_docs/_create_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_docs/open_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.467061 webviz_config-0.6.1/webviz_config/_docs/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    10699 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/INTRODUCTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_docs/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/docsify-copy-code.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   251818 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/docsify-katex.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/docsify-tabs.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)   106239 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/docsify.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.471061 webviz_config-0.6.1/webviz_config/_docs/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    31136 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_AMS-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     8392 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     8248 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13912 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13668 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    29932 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Main-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    21244 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Main-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    22076 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Main-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    32312 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Main-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    21192 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Math-BoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    21668 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Math-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    15296 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Bold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    14484 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Italic.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    13300 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    11792 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Script-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Size1-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Size2-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Size3-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Size4-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16868 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Typewriter-Regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_docs/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22476 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/katex.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5967 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/prism-bash.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/prism-python.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/prism-yaml.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/search.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-05-13 13:05:48.000000 webviz_config-0.6.1/webviz_config/_docs/static/vue.css
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_docs/static/webviz-doc.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9096 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_docs/static/webviz-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_is_reload_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_localhost_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8161 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20691 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_plugin_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_shared_settings_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_theme_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_user_data_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_user_preferences.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_webviz_settings_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/_write_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9358 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/common_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/deprecation_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.471061 webviz_config-0.6.1/webviz_config/generic_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_banner_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_data_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_embed_pdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_data_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_portable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_tour.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.471061 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.471061 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/_shared_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.471061 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/_text_view_element.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.475061 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_views/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.475061 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/_view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.475061 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7182 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5668 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_pivot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_syntax_highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20735 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/generic_plugins/_table_plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.475061 webviz_config-0.6.1/webviz_config/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4439 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/plugins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.475061 webviz_config-0.6.1/webviz_config/static/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       37 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/static/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.475061 webviz_config-0.6.1/webviz_config/static/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/static/assets/webviz_config.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/static/assets/webviz_layout.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.475061 webviz_config-0.6.1/webviz_config/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2649 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/Dockerfile.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/README.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/argument_deprecations.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/copy_data_template.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/feedback.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/plugin_deprecations.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/plugin_docs.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/radixconfig.yaml.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/sidebar.md.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/webviz-doc.js.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     9379 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/templates/webviz_template.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.479061 webviz_config-0.6.1/webviz_config/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/testing/_composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/testing/_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/testing/_webviz_ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.479061 webviz_config-0.6.1/webviz_config/themes/
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/themes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/themes/_default_theme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.479061 webviz_config-0.6.1/webviz_config/themes/default_assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/themes/default_assets/default_theme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.479061 webviz_config-0.6.1/webviz_config/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/utils/_available_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4842 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/utils/_callback_typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/utils/_dash_component_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/utils/_deprecate_webviz_settings_attribute_in_dash_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/utils/_localhost_open_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/utils/_silence_flask_startup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/utils/_str_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/utils/terminal_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/webviz_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/webviz_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/webviz_factory_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/webviz_instance_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.479061 webviz_config-0.6.1/webviz_config/webviz_plugin_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/webviz_plugin_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/webviz_plugin_subclasses/_layout_base_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/webviz_plugin_subclasses/_layout_unique_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/webviz_plugin_subclasses/_settings_group_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24056 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/webviz_plugin_subclasses/_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8516 2024-05-13 13:05:46.000000 webviz_config-0.6.1/webviz_config/webviz_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:09:36.479061 webviz_config-0.6.1/webviz_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-05-13 13:09:36.000000 webviz_config-0.6.1/webviz_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-05-13 13:09:36.000000 webviz_config-0.6.1/webviz_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:09:36.000000 webviz_config-0.6.1/webviz_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-13 13:09:36.000000 webviz_config-0.6.1/webviz_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:06:02.000000 webviz_config-0.6.1/webviz_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 13:09:36.000000 webviz_config-0.6.1/webviz_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 13:09:36.000000 webviz_config-0.6.1/webviz_config.egg-info/top_level.txt
```

### Comparing `webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/bug_report.md` & `webviz_config-0.6.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/.github/ISSUE_TEMPLATE/feature_request.md` & `webviz_config-0.6.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/.github/workflows/webviz-config.yml` & `webviz_config-0.6.1/.github/workflows/webviz-config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 jobs:
   webviz-config:
     runs-on: ubuntu-latest
     env:
       PYTHONWARNINGS: default # We want to see e.g. DeprecationWarnings
     strategy:
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11", "3.12"]
 
     steps:
       - name: 📖 Checkout commit locally
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Set setuptools_scm version
         if: github.event_name == 'release'
         # Need to instruct setuptools_scm to use the GitHub provided tag, despite local git changes (due to build step)
         run: echo "SETUPTOOLS_SCM_PRETEND_VERSION=${{ github.event.release.tag_name }}" >> $GITHUB_ENV
 
       - name: 🐍 Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: 📦 Install npm dependencies
         run: |
           npm ci --ignore-scripts
           npm run postinstall
```

### Comparing `webviz-config-0.5.3a0/CHANGELOG.md` & `webviz_config-0.6.1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/CODE_OF_CONDUCT.md` & `webviz_config-0.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/CONTRIBUTING.md` & `webviz_config-0.6.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/INTRODUCTION.md` & `webviz_config-0.6.1/INTRODUCTION.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/LICENSE` & `webviz_config-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/LICENSE.chromedriver` & `webviz_config-0.6.1/LICENSE.chromedriver`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/PKG-INFO` & `webviz_config-0.6.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: webviz-config
-Version: 0.5.3a0
-Summary: Configuration file support for webviz
-Home-page: https://github.com/equinor/webviz-config
-Author: R&T Equinor
-Project-URL: Documentation, https://equinor.github.io/webviz-config
-Project-URL: Download, https://pypi.org/project/webviz-config
-Project-URL: Source, https://github.com/equinor/webviz-config
-Project-URL: Tracker, https://github.com/equinor/webviz-config/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: English
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Dash
-Classifier: Framework :: Flask
-Classifier: Topic :: Multimedia :: Graphics
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: ~=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: deployment
-License-File: LICENSE
-License-File: LICENSE.chromedriver
-
 <h4>This package will be deprecated - we move instead all collaboration focus to the reusable React and Dash components in:
 <ul>
   <li>https://github.com/equinor/webviz-subsurface-components</li>
   <li>https://github.com/equinor/webviz-core-components</li>
 </ul>
 </h2>
 
@@ -43,25 +16,25 @@
 <p align="center">
 <a href="https://badge.fury.io/py/webviz-config"><img src="https://badge.fury.io/py/webviz-config.svg"></a>
 <a href="https://equinor.github.io/webviz-config"><img src="https://img.shields.io/badge/docs-passing-brightgreen"></a>
 <a href="https://github.com/equinor/webviz-config/blob/master/LICENSE"><img src="https://img.shields.io/github/license/equinor/webviz-config.svg?color=dark-green"></a>
 <a href="https://github.com/equinor/webviz-config/actions?query=branch%3Amaster"><img src="https://github.com/equinor/webviz-config/workflows/webviz-config/badge.svg"></a>
 <a href="https://lgtm.com/projects/g/equinor/webviz-config/alerts/"><img alt="Total alerts" src="https://img.shields.io/lgtm/alerts/g/equinor/webviz-config.svg?logo=lgtm&logoWidth=18"/></a>
 <a href="https://lgtm.com/projects/g/equinor/webviz-config/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/equinor/webviz-config.svg?logo=lgtm&logoWidth=18"/></a>
-<a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue.svg"></a>
+<a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-blue.svg"></a>
 <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 <br/>
 
 Writing a [Dash web application](https://github.com/plotly/dash) gives a lot of flexibility, however, it also requires :snake: Python knowledge from the person setting it up.
 
 *Webviz™* is a MIT-licensed configuration layer on top of Dash, which encourages making reusable components and dashboards, which can then be added/removed when creating an application using a short [`yaml`](https://en.wikipedia.org/wiki/YAML) configuration file.
 
 This Python package, `webviz-config`, is the core plugin framework. For a real example repository using this plugin system, see e.g. [`webviz-subsurface`](https://github.com/equinor/webviz-subsurface).
- 
+
 **These are the main user groups targeted by *Webviz™*:**
 - **You do not know Python**, and only want to add different predefined dashboards or visualizations/components in a certain order and/or on different pages in the application. Optionally with some text and mathematical equations (that you provide) inbetween the  dashboards, explaining what the user is looking at.
 - **You know [Python](https://www.python.org/)**, and want to create generic or specialized dashboards you or other users can reuse by simply asking for it in the Webviz™ configuration file. This can be done without knowing JavaScript (see also [Dash](https://plot.ly/dash/) for more information).
 - **You know [React](https://reactjs.org/)**, and want to create highly specialized visualization which Python or pure config-file users can reuse.
 
 *Webviz™* will create web applications with very :lock: strict security headers and CSP settings, giving an rating of **A+** on e.g. [Mozilla observatory](https://observatory.mozilla.org/). It also facilitates a :whale: Docker setup, where the Python code can be ran completely unpriviliged in a sandbox (both with respect to file system access and network communication).
 
@@ -111,24 +84,23 @@
 The optional arguments can be seen when running
 ```bash
 webviz --help
 ```
 
 ### Usage
 
-See [the introduction](https://github.com/equinor/webviz-config/blob/c2cbdb171372151de48f7d950b9b0637a805ce7d/./INTRODUCTION.md) page for information on how you
+See [the introduction](./INTRODUCTION.md) page for information on how you
 create a `webviz` configuration file and use it.
 
 ### Creating new plugins
 
 If you are interested in creating new plugins which can be configured through
-the configuration file, take a look at the [contribution guide](https://github.com/equinor/webviz-config/blob/c2cbdb171372151de48f7d950b9b0637a805ce7d/./CONTRIBUTING.md).
+the configuration file, take a look at the [contribution guide](./CONTRIBUTING.md).
 
 To quickly get started, we recommend using the corresponding
 [cookiecutter template](https://github.com/equinor/webviz-plugin-boilerplate).
 
 ### License
 
-`webviz-config` is, with a few exceptions listed below, [MIT](https://github.com/equinor/webviz-config/blob/c2cbdb171372151de48f7d950b9b0637a805ce7d/./LICENSE) licensed.
-
-- The [`webviz-config` logo](https://github.com/equinor/webviz-config/blob/c2cbdb171372151de48f7d950b9b0637a805ce7d/./webviz_config/_docs/static/webviz-logo.svg) is [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)
+`webviz-config` is, with a few exceptions listed below, [MIT](./LICENSE) licensed.
 
+- The [`webviz-config` logo](./webviz_config/_docs/static/webviz-logo.svg) is [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_a4h65bve_/tmpn0lg6kcy_TarContainer/0/17", line 33, column 5: Levels of opening and closing headings don't match*

```diff
@@ -1,35 +1,21 @@
-Metadata-Version: 2.1 Name: webviz-config Version: 0.5.3a0 Summary:
-Configuration file support for webviz Home-page: https://github.com/equinor/
-webviz-config Author: R&T Equinor Project-URL: Documentation, https://
-equinor.github.io/webviz-config Project-URL: Download, https://pypi.org/
-project/webviz-config Project-URL: Source, https://github.com/equinor/webviz-
-config Project-URL: Tracker, https://github.com/equinor/webviz-config/issues
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-OS Independent Classifier: Natural Language :: English Classifier: Environment
-:: Web Environment Classifier: Framework :: Dash Classifier: Framework :: Flask
-Classifier: Topic :: Multimedia :: Graphics Classifier: Topic :: Scientific/
-Engineering Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: License :: OSI Approved :: MIT License Requires-Python: ~=3.8
-Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
-deployment License-File: LICENSE License-File: LICENSE.chromedriver
 TThhiiss ppaacckkaaggee wwiillll bbee ddeepprreeccaatteedd -- wwee mmoovvee iinnsstteeaadd aallll ccoollllaabboorraattiioonn ffooccuuss ttoo
 tthhee rreeuussaabbllee RReeaacctt aanndd DDaasshh ccoommppoonneennttss iinn::
     ** hhttttppss::////ggiitthhuubb..ccoomm//eeqquuiinnoorr//wweebbvviizz--ssuubbssuurrffaaccee--ccoommppoonneennttss
     ** hhttttppss::////ggiitthhuubb..ccoomm//eeqquuiinnoorr//wweebbvviizz--ccoorree--ccoommppoonneennttss
 ===============================================================================
    [https://github.com/equinor/webviz-config/raw/master/webviz_config/_docs/
                      static/webviz-logo.svg?sanitize=true]
                ********** DDeemmooccrraattiizziinngg PPyytthhoonn wweebb aapppplliiccaattiioonnss **********
 _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_w_e_b_v_i_z_-_c_o_n_f_i_g_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_d_o_c_s_-
   _p_a_s_s_i_n_g_-_b_r_i_g_h_t_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_e_q_u_i_n_o_r_/_w_e_b_v_i_z_-
     _c_o_n_f_i_g_._s_v_g_?_c_o_l_o_r_=_d_a_r_k_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_q_u_i_n_o_r_/_w_e_b_v_i_z_-_c_o_n_f_i_g_/
 _w_o_r_k_f_l_o_w_s_/_w_e_b_v_i_z_-_c_o_n_f_i_g_/_b_a_d_g_e_._s_v_g_]_[_T_o_t_a_l_ _a_l_e_r_t_s_]_[_L_a_n_g_u_a_g_e_ _g_r_a_d_e_:_ _P_y_t_h_o_n_]_[_h_t_t_p_s_:
-   _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._8_%_2_0_|_%_2_0_3_._9_%_2_0_|_%_2_0_3_._1_0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
-              _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
+ _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._8_%_2_0_|_%_2_0_3_._9_%_2_0_|_%_2_0_3_._1_0_%_2_0_|_%_2_0_3_._1_1_%_2_0_|_%_2_0_3_._1_2_-
+     _b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 
 Writing a [Dash web application](https://github.com/plotly/dash) gives a lot of
 flexibility, however, it also requires :snake: Python knowledge from the person
 setting it up. *Webvizâ¢* is a MIT-licensed configuration layer on top of
 Dash, which encourages making reusable components and dashboards, which can
 then be added/removed when creating an application using a short [`yaml`]
 (https://en.wikipedia.org/wiki/YAML) configuration file. This Python package,
@@ -70,22 +56,17 @@
 After installation, there is a console script named `webviz` available. You can
 test the installation by using the provided example configuration file, ```bash
 webviz build ./examples/basic_example.yaml ``` Without any additional
 arguments, this will 1) create a temporary folder 2) write the Python
 application code to that folder 3) start a localhost server When stopping the
 server (press CTRL+C at any time), the temporary folder is deleted. The
 optional arguments can be seen when running ```bash webviz --help ``` ### Usage
-See [the introduction](https://github.com/equinor/webviz-config/blob/
-c2cbdb171372151de48f7d950b9b0637a805ce7d/./INTRODUCTION.md) page for
-information on how you create a `webviz` configuration file and use it. ###
-Creating new plugins If you are interested in creating new plugins which can be
-configured through the configuration file, take a look at the [contribution
-guide](https://github.com/equinor/webviz-config/blob/
-c2cbdb171372151de48f7d950b9b0637a805ce7d/./CONTRIBUTING.md). To quickly get
-started, we recommend using the corresponding [cookiecutter template](https://
-github.com/equinor/webviz-plugin-boilerplate). ### License `webviz-config` is,
-with a few exceptions listed below, [MIT](https://github.com/equinor/webviz-
-config/blob/c2cbdb171372151de48f7d950b9b0637a805ce7d/./LICENSE) licensed. - The
-[`webviz-config` logo](https://github.com/equinor/webviz-config/blob/
-c2cbdb171372151de48f7d950b9b0637a805ce7d/./webviz_config/_docs/static/webviz-
+See [the introduction](./INTRODUCTION.md) page for information on how you
+create a `webviz` configuration file and use it. ### Creating new plugins If
+you are interested in creating new plugins which can be configured through the
+configuration file, take a look at the [contribution guide](./CONTRIBUTING.md).
+To quickly get started, we recommend using the corresponding [cookiecutter
+template](https://github.com/equinor/webviz-plugin-boilerplate). ### License
+`webviz-config` is, with a few exceptions listed below, [MIT](./LICENSE)
+licensed. - The [`webviz-config` logo](./webviz_config/_docs/static/webviz-
 logo.svg) is [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/
 4.0/)
```

### Comparing `webviz-config-0.5.3a0/WEBVIZ_LAYOUT_FRAMEWORK_(WLF).md` & `webviz_config-0.6.1/WEBVIZ_LAYOUT_FRAMEWORK_(WLF).md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/assets/before-after-plugin-actions.png` & `webviz_config-0.6.1/assets/before-after-plugin-actions.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/assets/before-after-settings.png` & `webviz_config-0.6.1/assets/before-after-settings.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/assets/before-after-tabs-views.png` & `webviz_config-0.6.1/assets/before-after-tabs-views.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/assets/high-level-overview.png` & `webviz_config-0.6.1/assets/high-level-overview.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/assets/implement-plugin.svg` & `webviz_config-0.6.1/assets/implement-plugin.svg`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/assets/implement-settings-group.svg` & `webviz_config-0.6.1/assets/implement-settings-group.svg`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/assets/implement-view-element.svg` & `webviz_config-0.6.1/assets/implement-view-element.svg`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/assets/implement-view.svg` & `webviz_config-0.6.1/assets/implement-view.svg`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/assets/webviz-layout-overview.png` & `webviz_config-0.6.1/assets/webviz-layout-overview.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/examples/basic_example.yaml` & `webviz_config-0.6.1/examples/basic_example.yaml`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/examples/basic_example_advanced_menu.yaml` & `webviz_config-0.6.1/examples/basic_example_advanced_menu.yaml`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/examples/basic_example_wlf.yaml` & `webviz_config-0.6.1/examples/basic_example_wlf.yaml`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/examples/example-markdown.md` & `webviz_config-0.6.1/examples/example-markdown.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/examples/example.pdf` & `webviz_config-0.6.1/examples/example.pdf`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/examples/example_banner.png` & `webviz_config-0.6.1/examples/example_banner.png`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/mypy.ini` & `webviz_config-0.6.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/package-lock.json` & `webviz_config-0.6.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/package.json` & `webviz_config-0.6.1/package.json`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/setup.py` & `webviz_config-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/data/basic_example.yaml` & `webviz_config-0.6.1/tests/data/basic_example.yaml`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/test_callback_typecheck.py` & `webviz_config-0.6.1/tests/test_callback_typecheck.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/test_create_themed_layout.py` & `webviz_config-0.6.1/tests/test_create_themed_layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,8 +143,8 @@
             "legend": {"font": {"family": "Arial"}},
         }
         # create a new layout from specified and theme layouts
         new_layout = default_theme.create_themed_layout(specified_layout)
         # test some values
         assert new_layout["colorway"] == specified_layout["colorway"]
         assert new_layout["xaxis"]["title"]["text"] == "Title"
-        assert dash_duo.get_logs() == [], "browser console should contain no error"
+        assert not dash_duo.get_logs(), "browser console should contain no error"
```

### Comparing `webviz-config-0.5.3a0/tests/test_data_table.py` & `webviz_config-0.6.1/tests/test_data_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,36 +7,34 @@
 from webviz_config.generic_plugins import _data_table
 
 # mocked functions
 GET_DATA = "webviz_config.generic_plugins._data_table.get_data"
 
 
 def test_data_table(dash_duo):
-
     app = dash.Dash(__name__)
     app.config.suppress_callback_exceptions = True
     CACHE.init_app(app.server)
     code_file = "./tests/data/example_data.csv"
     with mock.patch(GET_DATA) as mock_path:
         mock_path.return_value = pd.read_csv(code_file)
         page = _data_table.DataTable(app, code_file)
         app.layout = page.layout
         dash_duo.start_server(app)
-        assert dash_duo.get_logs() == [], "browser console should contain no error"
+        assert not dash_duo.get_logs(), "browser console should contain no error"
 
 
 def test_data_table_with_settings(dash_duo):
-
     app = dash.Dash(__name__)
     app.css.config.serve_locally = True
     app.scripts.config.serve_locally = True
     app.config.suppress_callback_exceptions = True
     CACHE.init_app(app.server)
     code_file = "./tests/data/example_data.csv"
     with mock.patch(GET_DATA) as mock_path:
         mock_path.return_value = pd.read_csv(code_file)
         page = _data_table.DataTable(
             app, csv_file=code_file, sorting=False, filtering=False, pagination=False
         )
         app.layout = page.layout
         dash_duo.start_server(app)
-        assert dash_duo.get_logs() == [], "browser console should contain no error"
+        assert not dash_duo.get_logs(), "browser console should contain no error"
```

### Comparing `webviz-config-0.5.3a0/tests/test_docker_setup.py` & `webviz_config-0.6.1/tests/test_docker_setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+
 import pytest
 
 from webviz_config._dockerize._create_docker_setup import get_python_requirements
 
 
 @pytest.mark.parametrize(
     "distributions, requirements",
@@ -35,15 +37,16 @@
                 }
             },
             ["git+https://github.com/equinor/webviz-config@0.3.0"],
         ),
     ],
 )
 def test_derived_requirements(distributions, requirements):
-    with pytest.warns(None) as record:
+    with warnings.catch_warnings(record=True) as record:
+        warnings.simplefilter("always")
         assert set(requirements).issubset(get_python_requirements(distributions))
         assert len(record) == len(
             [
                 metadata
                 for metadata in distributions.values()
                 if metadata["download_url"] is None and metadata["source_url"] is None
             ]
```

### Comparing `webviz-config-0.5.3a0/tests/test_docstring.py` & `webviz_config-0.6.1/tests/test_docstring.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/test_example_plugin.py` & `webviz_config-0.6.1/tests/test_example_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/test_example_wlf_plugin.py` & `webviz_config-0.6.1/tests/test_example_wlf_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from webviz_config.testing import WebvizComposite
 from webviz_config.generic_plugins._example_wlf_plugin import ExampleWlfPlugin
 
 
 def test_example_wlf_plugin(
     _webviz_duo: WebvizComposite,
 ) -> None:
-
     plugin = ExampleWlfPlugin(title="hello")
 
     _webviz_duo.start_server(plugin)
 
     _webviz_duo.toggle_webviz_settings_drawer()
 
     _webviz_duo.toggle_webviz_settings_group(
@@ -19,8 +18,8 @@
     component_id = _webviz_duo.view_settings_group_unique_component_id(
         view_id="plot-view",
         settings_group_id="plot-settings",
         component_unique_id="coordinates-selector",
     )
 
     _webviz_duo.wait_for_contains_text(component_id, "x - y")
-    assert _webviz_duo.get_logs() == []
+    assert not _webviz_duo.get_logs()
```

### Comparing `webviz-config-0.5.3a0/tests/test_plugin_init.py` & `webviz_config-0.6.1/tests/test_plugin_init.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/test_plugin_metadata.py` & `webviz_config-0.6.1/tests/test_plugin_metadata.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/test_portable.py` & `webviz_config-0.6.1/tests/test_portable.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         "table-example",
         "pdf-example",
         "syntax-highlighting-example",
         "plot-a-table",
         "pivot-table",
     ]:
         dash_duo.wait_for_element(f".Menu__Page[href='/{page}']").click()
-    assert dash_duo.get_logs() == [], "browser console should contain no error"
+    assert not dash_duo.get_logs(), "browser console should contain no error"
```

### Comparing `webviz-config-0.5.3a0/tests/test_schema.py` & `webviz_config-0.6.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/test_syntax_highlighter.py` & `webviz_config-0.6.1/tests/test_syntax_highlighter.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 import dash
 
 from webviz_config.common_cache import CACHE
 from webviz_config.generic_plugins import _syntax_highlighter
 
 
 def test_syntax_highlighter(dash_duo):
-
     app = dash.Dash(__name__)
     app.config.suppress_callback_exceptions = True
     CACHE.init_app(app.server)
     code_file = Path("./tests/data/basic_example.yaml")
     with mock.patch(
         "webviz_config.generic_plugins._syntax_highlighter.get_path"
     ) as mock_path:
         mock_path.return_value = code_file
         page = _syntax_highlighter.SyntaxHighlighter(app, code_file)
         app.layout = page.layout
         dash_duo.start_server(app)
-        assert dash_duo.get_logs() == [], "browser console should contain no error"
+        assert not dash_duo.get_logs(), "browser console should contain no error"
```

### Comparing `webviz-config-0.5.3a0/tests/test_table_plotter.py` & `webviz_config-0.6.1/tests/test_table_plotter.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/unit_tests/test_webviz_factory_registry.py` & `webviz_config-0.6.1/tests/unit_tests/test_webviz_factory_registry.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/unit_tests/test_webviz_instance_info.py` & `webviz_config-0.6.1/tests/unit_tests/test_webviz_instance_info.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/tests/unit_tests/test_webviz_settings.py` & `webviz_config-0.6.1/tests/unit_tests/test_webviz_settings.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/__init__.py` & `webviz_config-0.6.1/webviz_config/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_build_webviz.py` & `webviz_config-0.6.1/webviz_config/_build_webviz.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_config_parser.py` & `webviz_config-0.6.1/webviz_config/_config_parser.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_deployment/azure_cli.py` & `webviz_config-0.6.1/webviz_config/_deployment/azure_cli.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_deployment/azure_configuration.py` & `webviz_config-0.6.1/webviz_config/_deployment/azure_configuration.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_deployment/github_cli.py` & `webviz_config-0.6.1/webviz_config/_deployment/github_cli.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_deployment/interactive_terminal.py` & `webviz_config-0.6.1/webviz_config/_deployment/interactive_terminal.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_deployment/radix.py` & `webviz_config-0.6.1/webviz_config/_deployment/radix.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_deployment/radix_cli.py` & `webviz_config-0.6.1/webviz_config/_deployment/radix_cli.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_deployment/radix_configuration.py` & `webviz_config-0.6.1/webviz_config/_deployment/radix_configuration.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_deprecation_store.py` & `webviz_config-0.6.1/webviz_config/_deprecation_store.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_dockerize/_create_docker_setup.py` & `webviz_config-0.6.1/webviz_config/_dockerize/_create_docker_setup.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_dockerize/_pip_git_url.py` & `webviz_config-0.6.1/webviz_config/_dockerize/_pip_git_url.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/_build_docs.py` & `webviz_config-0.6.1/webviz_config/_docs/_build_docs.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/_create_schema.py` & `webviz_config-0.6.1/webviz_config/_docs/_create_schema.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/open_docs.py` & `webviz_config-0.6.1/webviz_config/_docs/open_docs.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/INTRODUCTION.md` & `webviz_config-0.6.1/webviz_config/_docs/static/INTRODUCTION.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/README.md` & `webviz_config-0.6.1/webviz_config/_docs/static/README.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-copy-code.min.js` & `webviz_config-0.6.1/webviz_config/_docs/static/docsify-copy-code.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-katex.js` & `webviz_config-0.6.1/webviz_config/_docs/static/docsify-katex.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/docsify-tabs.min.js` & `webviz_config-0.6.1/webviz_config/_docs/static/docsify-tabs.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/docsify.min.js` & `webviz_config-0.6.1/webviz_config/_docs/static/docsify.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_AMS-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_AMS-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Bold.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Bold.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Caligraphic-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Bold.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Bold.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Fraktur-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Bold.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Main-Bold.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-BoldItalic.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Main-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Italic.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Main-Italic.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Main-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Main-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Math-BoldItalic.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Math-BoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Math-Italic.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Math-Italic.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Bold.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Bold.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Italic.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Italic.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_SansSerif-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Script-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Script-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size1-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Size1-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size2-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Size2-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size3-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Size3-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Size4-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Size4-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/fonts/KaTeX_Typewriter-Regular.woff2` & `webviz_config-0.6.1/webviz_config/_docs/static/fonts/KaTeX_Typewriter-Regular.woff2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/index.html` & `webviz_config-0.6.1/webviz_config/_docs/static/index.html`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/katex.min.css` & `webviz_config-0.6.1/webviz_config/_docs/static/katex.min.css`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/prism-bash.min.js` & `webviz_config-0.6.1/webviz_config/_docs/static/prism-bash.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/prism-python.min.js` & `webviz_config-0.6.1/webviz_config/_docs/static/prism-python.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/prism-yaml.min.js` & `webviz_config-0.6.1/webviz_config/_docs/static/prism-yaml.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/search.min.js` & `webviz_config-0.6.1/webviz_config/_docs/static/search.min.js`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/vue.css` & `webviz_config-0.6.1/webviz_config/_docs/static/vue.css`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_docs/static/webviz-logo.svg` & `webviz_config-0.6.1/webviz_config/_docs/static/webviz-logo.svg`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_localhost_token.py` & `webviz_config-0.6.1/webviz_config/_localhost_token.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_oauth2.py` & `webviz_config-0.6.1/webviz_config/_oauth2.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_plugin_abc.py` & `webviz_config-0.6.1/webviz_config/_plugin_abc.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_shared_settings_subscriptions.py` & `webviz_config-0.6.1/webviz_config/_shared_settings_subscriptions.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_theme_class.py` & `webviz_config-0.6.1/webviz_config/_theme_class.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_user_preferences.py` & `webviz_config-0.6.1/webviz_config/_user_preferences.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_webviz_settings_class.py` & `webviz_config-0.6.1/webviz_config/_webviz_settings_class.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/_write_script.py` & `webviz_config-0.6.1/webviz_config/_write_script.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/command_line.py` & `webviz_config-0.6.1/webviz_config/command_line.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/common_cache.py` & `webviz_config-0.6.1/webviz_config/common_cache.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/deprecation_decorators.py` & `webviz_config-0.6.1/webviz_config/deprecation_decorators.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_banner_image.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_banner_image.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_data_table.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_data_table.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_embed_pdf.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_embed_pdf.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_assets.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_example_assets.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_data_download.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_example_data_download.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_plugin.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_example_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_portable.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_example_portable.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_tour.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_example_tour.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_plugin.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/_shared_settings.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_shared_settings/_shared_settings.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/_text_view_element.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_shared_view_elements/_text_view_element.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/_view.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_views/_plot/_view.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/_view.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_example_wlf_plugin/_views/_table/_view.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_markdown.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_markdown.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_pivot_table.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_pivot_table.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_syntax_highlighter.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_syntax_highlighter.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/generic_plugins/_table_plotter.py` & `webviz_config-0.6.1/webviz_config/generic_plugins/_table_plotter.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/plugins/__init__.py` & `webviz_config-0.6.1/webviz_config/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/plugins/_utils.py` & `webviz_config-0.6.1/webviz_config/plugins/_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/static/README.md` & `webviz_config-0.6.1/webviz_config/static/README.md`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/static/assets/webviz_config.css` & `webviz_config-0.6.1/webviz_config/static/assets/webviz_config.css`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/static/assets/webviz_layout.css` & `webviz_config-0.6.1/webviz_config/static/assets/webviz_layout.css`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/templates/Dockerfile.jinja2` & `webviz_config-0.6.1/webviz_config/templates/Dockerfile.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/templates/copy_data_template.py.jinja2` & `webviz_config-0.6.1/webviz_config/templates/copy_data_template.py.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/templates/feedback.md.jinja2` & `webviz_config-0.6.1/webviz_config/templates/feedback.md.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/templates/plugin_docs.md.jinja2` & `webviz_config-0.6.1/webviz_config/templates/plugin_docs.md.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/templates/radixconfig.yaml.jinja2` & `webviz_config-0.6.1/webviz_config/templates/radixconfig.yaml.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/templates/webviz-doc.js.jinja2` & `webviz_config-0.6.1/webviz_config/templates/webviz-doc.js.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/templates/webviz_template.py.jinja2` & `webviz_config-0.6.1/webviz_config/templates/webviz_template.py.jinja2`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/testing/_composite.py` & `webviz_config-0.6.1/webviz_config/testing/_composite.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/testing/_plugin.py` & `webviz_config-0.6.1/webviz_config/testing/_plugin.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/themes/default_assets/default_theme.css` & `webviz_config-0.6.1/webviz_config/themes/default_assets/default_theme.css`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/utils/_available_port.py` & `webviz_config-0.6.1/webviz_config/utils/_available_port.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/utils/_callback_typecheck.py` & `webviz_config-0.6.1/webviz_config/utils/_callback_typecheck.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/utils/_dash_component_utils.py` & `webviz_config-0.6.1/webviz_config/utils/_dash_component_utils.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/utils/_deprecate_webviz_settings_attribute_in_dash_app.py` & `webviz_config-0.6.1/webviz_config/utils/_deprecate_webviz_settings_attribute_in_dash_app.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/utils/_localhost_open_browser.py` & `webviz_config-0.6.1/webviz_config/utils/_localhost_open_browser.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/utils/_silence_flask_startup.py` & `webviz_config-0.6.1/webviz_config/utils/_silence_flask_startup.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/webviz_assets.py` & `webviz_config-0.6.1/webviz_config/webviz_assets.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/webviz_factory.py` & `webviz_config-0.6.1/webviz_config/webviz_factory.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/webviz_factory_registry.py` & `webviz_config-0.6.1/webviz_config/webviz_factory_registry.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/webviz_instance_info.py` & `webviz_config-0.6.1/webviz_config/webviz_instance_info.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_layout_base_abc.py` & `webviz_config-0.6.1/webviz_config/webviz_plugin_subclasses/_layout_base_abc.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_layout_unique_id.py` & `webviz_config-0.6.1/webviz_config/webviz_plugin_subclasses/_layout_unique_id.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_settings_group_abc.py` & `webviz_config-0.6.1/webviz_config/webviz_plugin_subclasses/_settings_group_abc.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/webviz_plugin_subclasses/_views.py` & `webviz_config-0.6.1/webviz_config/webviz_plugin_subclasses/_views.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config/webviz_store.py` & `webviz_config-0.6.1/webviz_config/webviz_store.py`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config.egg-info/PKG-INFO` & `webviz_config-0.6.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webviz-config
-Version: 0.5.3a0
+Version: 0.6.1
 Summary: Configuration file support for webviz
 Home-page: https://github.com/equinor/webviz-config
 Author: R&T Equinor
 Project-URL: Documentation, https://equinor.github.io/webviz-config
 Project-URL: Download, https://pypi.org/project/webviz-config
 Project-URL: Source, https://github.com/equinor/webviz-config
 Project-URL: Tracker, https://github.com/equinor/webviz-config/issues
@@ -16,18 +16,55 @@
 Classifier: Framework :: Flask
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: deployment
 License-File: LICENSE
 License-File: LICENSE.chromedriver
+Requires-Dist: bleach[css]>=5
+Requires-Dist: cryptography>=2.4
+Requires-Dist: dash>=2.0
+Requires-Dist: dash-pivottable>=0.0.2
+Requires-Dist: flask>=2.0
+Requires-Dist: flask-caching>=1.4
+Requires-Dist: flask-talisman>=0.6
+Requires-Dist: jinja2>=2.10
+Requires-Dist: markdown>=3.0
+Requires-Dist: msal>=1.5.0
+Requires-Dist: orjson>=3.3
+Requires-Dist: pandas>=1.0
+Requires-Dist: pyarrow>=0.16
+Requires-Dist: pyyaml>=5.1
+Requires-Dist: requests>=2.20
+Requires-Dist: tqdm>=4.8
+Requires-Dist: webviz-core-components>=0.6
+Requires-Dist: werkzeug>=2.0
+Provides-Extra: tests
+Requires-Dist: bandit; extra == "tests"
+Requires-Dist: black<23,>=22.12; extra == "tests"
+Requires-Dist: dash[testing]; extra == "tests"
+Requires-Dist: jsonschema; extra == "tests"
+Requires-Dist: mypy; extra == "tests"
+Requires-Dist: pylint<=2.13.9; extra == "tests"
+Requires-Dist: pytest-xdist; extra == "tests"
+Requires-Dist: pytest-forked; extra == "tests"
+Requires-Dist: selenium; extra == "tests"
+Requires-Dist: types-bleach; extra == "tests"
+Requires-Dist: types-markdown; extra == "tests"
+Requires-Dist: types-pyyaml; extra == "tests"
+Requires-Dist: types-requests; extra == "tests"
+Provides-Extra: deployment
+Requires-Dist: aiohttp; extra == "deployment"
+Requires-Dist: azure-core; extra == "deployment"
+Requires-Dist: azure-identity; extra == "deployment"
+Requires-Dist: azure-mgmt-resource; extra == "deployment"
+Requires-Dist: azure-mgmt-storage; extra == "deployment"
+Requires-Dist: azure-storage-blob; extra == "deployment"
 
 <h4>This package will be deprecated - we move instead all collaboration focus to the reusable React and Dash components in:
 <ul>
   <li>https://github.com/equinor/webviz-subsurface-components</li>
   <li>https://github.com/equinor/webviz-core-components</li>
 </ul>
 </h2>
@@ -43,25 +80,25 @@
 <p align="center">
 <a href="https://badge.fury.io/py/webviz-config"><img src="https://badge.fury.io/py/webviz-config.svg"></a>
 <a href="https://equinor.github.io/webviz-config"><img src="https://img.shields.io/badge/docs-passing-brightgreen"></a>
 <a href="https://github.com/equinor/webviz-config/blob/master/LICENSE"><img src="https://img.shields.io/github/license/equinor/webviz-config.svg?color=dark-green"></a>
 <a href="https://github.com/equinor/webviz-config/actions?query=branch%3Amaster"><img src="https://github.com/equinor/webviz-config/workflows/webviz-config/badge.svg"></a>
 <a href="https://lgtm.com/projects/g/equinor/webviz-config/alerts/"><img alt="Total alerts" src="https://img.shields.io/lgtm/alerts/g/equinor/webviz-config.svg?logo=lgtm&logoWidth=18"/></a>
 <a href="https://lgtm.com/projects/g/equinor/webviz-config/context:python"><img alt="Language grade: Python" src="https://img.shields.io/lgtm/grade/python/g/equinor/webviz-config.svg?logo=lgtm&logoWidth=18"/></a>
-<a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10-blue.svg"></a>
+<a href="https://www.python.org/"><img src="https://img.shields.io/badge/python-3.8%20|%203.9%20|%203.10%20|%203.11%20|%203.12-blue.svg"></a>
 <a href="https://github.com/psf/black"><img src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 </p>
 <br/>
 
 Writing a [Dash web application](https://github.com/plotly/dash) gives a lot of flexibility, however, it also requires :snake: Python knowledge from the person setting it up.
 
 *Webviz™* is a MIT-licensed configuration layer on top of Dash, which encourages making reusable components and dashboards, which can then be added/removed when creating an application using a short [`yaml`](https://en.wikipedia.org/wiki/YAML) configuration file.
 
 This Python package, `webviz-config`, is the core plugin framework. For a real example repository using this plugin system, see e.g. [`webviz-subsurface`](https://github.com/equinor/webviz-subsurface).
- 
+
 **These are the main user groups targeted by *Webviz™*:**
 - **You do not know Python**, and only want to add different predefined dashboards or visualizations/components in a certain order and/or on different pages in the application. Optionally with some text and mathematical equations (that you provide) inbetween the  dashboards, explaining what the user is looking at.
 - **You know [Python](https://www.python.org/)**, and want to create generic or specialized dashboards you or other users can reuse by simply asking for it in the Webviz™ configuration file. This can be done without knowing JavaScript (see also [Dash](https://plot.ly/dash/) for more information).
 - **You know [React](https://reactjs.org/)**, and want to create highly specialized visualization which Python or pure config-file users can reuse.
 
 *Webviz™* will create web applications with very :lock: strict security headers and CSP settings, giving an rating of **A+** on e.g. [Mozilla observatory](https://observatory.mozilla.org/). It also facilitates a :whale: Docker setup, where the Python code can be ran completely unpriviliged in a sandbox (both with respect to file system access and network communication).
 
@@ -111,24 +148,23 @@
 The optional arguments can be seen when running
 ```bash
 webviz --help
 ```
 
 ### Usage
 
-See [the introduction](https://github.com/equinor/webviz-config/blob/c2cbdb171372151de48f7d950b9b0637a805ce7d/./INTRODUCTION.md) page for information on how you
+See [the introduction](https://github.com/equinor/webviz-config/blob/c1d884fd08bfcbcdecd89b141343826134817a21/./INTRODUCTION.md) page for information on how you
 create a `webviz` configuration file and use it.
 
 ### Creating new plugins
 
 If you are interested in creating new plugins which can be configured through
-the configuration file, take a look at the [contribution guide](https://github.com/equinor/webviz-config/blob/c2cbdb171372151de48f7d950b9b0637a805ce7d/./CONTRIBUTING.md).
+the configuration file, take a look at the [contribution guide](https://github.com/equinor/webviz-config/blob/c1d884fd08bfcbcdecd89b141343826134817a21/./CONTRIBUTING.md).
 
 To quickly get started, we recommend using the corresponding
 [cookiecutter template](https://github.com/equinor/webviz-plugin-boilerplate).
 
 ### License
 
-`webviz-config` is, with a few exceptions listed below, [MIT](https://github.com/equinor/webviz-config/blob/c2cbdb171372151de48f7d950b9b0637a805ce7d/./LICENSE) licensed.
-
-- The [`webviz-config` logo](https://github.com/equinor/webviz-config/blob/c2cbdb171372151de48f7d950b9b0637a805ce7d/./webviz_config/_docs/static/webviz-logo.svg) is [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)
+`webviz-config` is, with a few exceptions listed below, [MIT](https://github.com/equinor/webviz-config/blob/c1d884fd08bfcbcdecd89b141343826134817a21/./LICENSE) licensed.
 
+- The [`webviz-config` logo](https://github.com/equinor/webviz-config/blob/c1d884fd08bfcbcdecd89b141343826134817a21/./webviz_config/_docs/static/webviz-logo.svg) is [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_a4h65bve_/tmpn0lg6kcy_TarContainer/0/232", line 33, column 5: Levels of opening and closing headings don't match*

```diff
@@ -1,35 +1,55 @@
-Metadata-Version: 2.1 Name: webviz-config Version: 0.5.3a0 Summary:
-Configuration file support for webviz Home-page: https://github.com/equinor/
-webviz-config Author: R&T Equinor Project-URL: Documentation, https://
-equinor.github.io/webviz-config Project-URL: Download, https://pypi.org/
-project/webviz-config Project-URL: Source, https://github.com/equinor/webviz-
-config Project-URL: Tracker, https://github.com/equinor/webviz-config/issues
-Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
-OS Independent Classifier: Natural Language :: English Classifier: Environment
-:: Web Environment Classifier: Framework :: Dash Classifier: Framework :: Flask
+Metadata-Version: 2.1 Name: webviz-config Version: 0.6.1 Summary: Configuration
+file support for webviz Home-page: https://github.com/equinor/webviz-config
+Author: R&T Equinor Project-URL: Documentation, https://equinor.github.io/
+webviz-config Project-URL: Download, https://pypi.org/project/webviz-config
+Project-URL: Source, https://github.com/equinor/webviz-config Project-URL:
+Tracker, https://github.com/equinor/webviz-config/issues Classifier:
+Programming Language :: Python :: 3 Classifier: Operating System :: OS
+Independent Classifier: Natural Language :: English Classifier: Environment ::
+Web Environment Classifier: Framework :: Dash Classifier: Framework :: Flask
 Classifier: Topic :: Multimedia :: Graphics Classifier: Topic :: Scientific/
 Engineering Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License Requires-Python: ~=3.8
-Description-Content-Type: text/markdown Provides-Extra: tests Provides-Extra:
-deployment License-File: LICENSE License-File: LICENSE.chromedriver
+Description-Content-Type: text/markdown License-File: LICENSE License-File:
+LICENSE.chromedriver Requires-Dist: bleach[css]>=5 Requires-Dist:
+cryptography>=2.4 Requires-Dist: dash>=2.0 Requires-Dist: dash-
+pivottable>=0.0.2 Requires-Dist: flask>=2.0 Requires-Dist: flask-caching>=1.4
+Requires-Dist: flask-talisman>=0.6 Requires-Dist: jinja2>=2.10 Requires-Dist:
+markdown>=3.0 Requires-Dist: msal>=1.5.0 Requires-Dist: orjson>=3.3 Requires-
+Dist: pandas>=1.0 Requires-Dist: pyarrow>=0.16 Requires-Dist: pyyaml>=5.1
+Requires-Dist: requests>=2.20 Requires-Dist: tqdm>=4.8 Requires-Dist: webviz-
+core-components>=0.6 Requires-Dist: werkzeug>=2.0 Provides-Extra: tests
+Requires-Dist: bandit; extra == "tests" Requires-Dist: black<23,>=22.12; extra
+== "tests" Requires-Dist: dash[testing]; extra == "tests" Requires-Dist:
+jsonschema; extra == "tests" Requires-Dist: mypy; extra == "tests" Requires-
+Dist: pylint<=2.13.9; extra == "tests" Requires-Dist: pytest-xdist; extra ==
+"tests" Requires-Dist: pytest-forked; extra == "tests" Requires-Dist: selenium;
+extra == "tests" Requires-Dist: types-bleach; extra == "tests" Requires-Dist:
+types-markdown; extra == "tests" Requires-Dist: types-pyyaml; extra == "tests"
+Requires-Dist: types-requests; extra == "tests" Provides-Extra: deployment
+Requires-Dist: aiohttp; extra == "deployment" Requires-Dist: azure-core; extra
+== "deployment" Requires-Dist: azure-identity; extra == "deployment" Requires-
+Dist: azure-mgmt-resource; extra == "deployment" Requires-Dist: azure-mgmt-
+storage; extra == "deployment" Requires-Dist: azure-storage-blob; extra ==
+"deployment"
 TThhiiss ppaacckkaaggee wwiillll bbee ddeepprreeccaatteedd -- wwee mmoovvee iinnsstteeaadd aallll ccoollllaabboorraattiioonn ffooccuuss ttoo
 tthhee rreeuussaabbllee RReeaacctt aanndd DDaasshh ccoommppoonneennttss iinn::
     ** hhttttppss::////ggiitthhuubb..ccoomm//eeqquuiinnoorr//wweebbvviizz--ssuubbssuurrffaaccee--ccoommppoonneennttss
     ** hhttttppss::////ggiitthhuubb..ccoomm//eeqquuiinnoorr//wweebbvviizz--ccoorree--ccoommppoonneennttss
 ===============================================================================
    [https://github.com/equinor/webviz-config/raw/master/webviz_config/_docs/
                      static/webviz-logo.svg?sanitize=true]
                ********** DDeemmooccrraattiizziinngg PPyytthhoonn wweebb aapppplliiccaattiioonnss **********
 _[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_w_e_b_v_i_z_-_c_o_n_f_i_g_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_d_o_c_s_-
   _p_a_s_s_i_n_g_-_b_r_i_g_h_t_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_e_q_u_i_n_o_r_/_w_e_b_v_i_z_-
     _c_o_n_f_i_g_._s_v_g_?_c_o_l_o_r_=_d_a_r_k_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_e_q_u_i_n_o_r_/_w_e_b_v_i_z_-_c_o_n_f_i_g_/
 _w_o_r_k_f_l_o_w_s_/_w_e_b_v_i_z_-_c_o_n_f_i_g_/_b_a_d_g_e_._s_v_g_]_[_T_o_t_a_l_ _a_l_e_r_t_s_]_[_L_a_n_g_u_a_g_e_ _g_r_a_d_e_:_ _P_y_t_h_o_n_]_[_h_t_t_p_s_:
-   _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._8_%_2_0_|_%_2_0_3_._9_%_2_0_|_%_2_0_3_._1_0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
-              _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
+ _/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._8_%_2_0_|_%_2_0_3_._9_%_2_0_|_%_2_0_3_._1_0_%_2_0_|_%_2_0_3_._1_1_%_2_0_|_%_2_0_3_._1_2_-
+     _b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 
 Writing a [Dash web application](https://github.com/plotly/dash) gives a lot of
 flexibility, however, it also requires :snake: Python knowledge from the person
 setting it up. *Webvizâ¢* is a MIT-licensed configuration layer on top of
 Dash, which encourages making reusable components and dashboards, which can
 then be added/removed when creating an application using a short [`yaml`]
 (https://en.wikipedia.org/wiki/YAML) configuration file. This Python package,
@@ -71,21 +91,21 @@
 test the installation by using the provided example configuration file, ```bash
 webviz build ./examples/basic_example.yaml ``` Without any additional
 arguments, this will 1) create a temporary folder 2) write the Python
 application code to that folder 3) start a localhost server When stopping the
 server (press CTRL+C at any time), the temporary folder is deleted. The
 optional arguments can be seen when running ```bash webviz --help ``` ### Usage
 See [the introduction](https://github.com/equinor/webviz-config/blob/
-c2cbdb171372151de48f7d950b9b0637a805ce7d/./INTRODUCTION.md) page for
+c1d884fd08bfcbcdecd89b141343826134817a21/./INTRODUCTION.md) page for
 information on how you create a `webviz` configuration file and use it. ###
 Creating new plugins If you are interested in creating new plugins which can be
 configured through the configuration file, take a look at the [contribution
 guide](https://github.com/equinor/webviz-config/blob/
-c2cbdb171372151de48f7d950b9b0637a805ce7d/./CONTRIBUTING.md). To quickly get
+c1d884fd08bfcbcdecd89b141343826134817a21/./CONTRIBUTING.md). To quickly get
 started, we recommend using the corresponding [cookiecutter template](https://
 github.com/equinor/webviz-plugin-boilerplate). ### License `webviz-config` is,
 with a few exceptions listed below, [MIT](https://github.com/equinor/webviz-
-config/blob/c2cbdb171372151de48f7d950b9b0637a805ce7d/./LICENSE) licensed. - The
+config/blob/c1d884fd08bfcbcdecd89b141343826134817a21/./LICENSE) licensed. - The
 [`webviz-config` logo](https://github.com/equinor/webviz-config/blob/
-c2cbdb171372151de48f7d950b9b0637a805ce7d/./webviz_config/_docs/static/webviz-
+c1d884fd08bfcbcdecd89b141343826134817a21/./webviz_config/_docs/static/webviz-
 logo.svg) is [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/
 4.0/)
```

### Comparing `webviz-config-0.5.3a0/webviz_config.egg-info/SOURCES.txt` & `webviz_config-0.6.1/webviz_config.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 INTRODUCTION.md
 LICENSE
 LICENSE.chromedriver
 README.md
+SECURITY.md
 WEBVIZ_LAYOUT_FRAMEWORK_(WLF).md
 bandit.yml
 mypy.ini
 package-lock.json
 package.json
 pytest.ini
 setup.py
```

### Comparing `webviz-config-0.5.3a0/webviz_config.egg-info/entry_points.txt` & `webviz_config-0.6.1/webviz_config.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `webviz-config-0.5.3a0/webviz_config.egg-info/requires.txt` & `webviz_config-0.6.1/webviz_config.egg-info/requires.txt`

 * *Files identical despite different names*

