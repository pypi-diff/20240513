# Comparing `tmp/glean_parser-8.1.1.tar.gz` & `tmp/glean_parser-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/glean_parser-8.1.1.tar", last modified: Wed Aug  2 10:14:29 2023, max compression
+gzip compressed data, was "dist/glean_parser-9.0.0.tar", last modified: Wed Sep 13 12:45:36 2023, max compression
```

## Comparing `glean_parser-8.1.1.tar` & `glean_parser-9.0.0.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6784 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      292 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.editorconfig
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/.github/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.github/dependabot.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.github/pull_request_template.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      169 2023-08-02 10:14:13.000000 glean_parser-8.1.1/.swiftlint.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-08-02 10:14:13.000000 glean_parser-8.1.1/AUTHORS.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25674 2023-08-02 10:14:13.000000 glean_parser-8.1.1/CHANGELOG.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-08-02 10:14:13.000000 glean_parser-8.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-08-02 10:14:13.000000 glean_parser-8.1.1/CONTRIBUTING.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-08-02 10:14:13.000000 glean_parser-8.1.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-08-02 10:14:13.000000 glean_parser-8.1.1/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2448 2023-08-02 10:14:13.000000 glean_parser-8.1.1/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28820 2023-08-02 10:14:29.000000 glean_parser-8.1.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-08-02 10:14:13.000000 glean_parser-8.1.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/Makefile
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/docs/_static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/_static/glean.jpeg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/authors.md
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4921 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/contributing.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25674 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/history.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/installation.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/make.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/metrics-yaml.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/pings-yaml.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/readme.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-08-02 10:14:13.000000 glean_parser-8.1.1/docs/tags-yaml.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8631 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4405 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/coverage.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/data_review.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11230 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/javascript.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6004 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/javascript_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12598 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/kotlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18248 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/lint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9066 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/markdown.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12431 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15309 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2815 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/pings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6744 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/rust.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser/schemas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19566 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/schemas/metrics.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25849 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/schemas/metrics.2-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4315 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/schemas/pings.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4363 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/schemas/pings.2-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/schemas/tags.1-0-0.schema.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8379 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/swift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/tags.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/data_review.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/javascript.buildinfo.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/javascript.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5368 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/javascript_server.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/kotlin.buildinfo.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/kotlin.geckoview.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5247 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/kotlin.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3425 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/markdown.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/qmldir.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3600 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/rust.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4809 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/templates/swift.jinja2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8148 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/translate.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2037 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/translation_options.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16825 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2118 2023-08-02 10:14:13.000000 glean_parser-8.1.1/glean_parser/validate_ping.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28820 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3278 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      152 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-08-02 10:14:29.000000 glean_parser-8.1.1/glean_parser.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-08-02 10:14:13.000000 glean_parser-8.1.1/pytest.ini
--rw-r--r--   0 circleci  (1001) circleci  (1002)      479 2023-08-02 10:14:13.000000 glean_parser-8.1.1/requirements_dev.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-08-02 10:14:29.000000 glean_parser-8.1.1/setup.cfg
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2286 2023-08-02 10:14:13.000000 glean_parser-8.1.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/conftest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/tests/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/all_metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/all_pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      885 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/bad_ping.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9453 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/core.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/duplicate_labeled.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/duplicate_send_in_ping.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/empty.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      755 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/event_key_ordering.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/events_with_types.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      489 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/fxa-server-metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/fxa-server-pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3539 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/gecko.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/invalid-ping-names.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/invalid.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      481 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/jwe.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/metric-with-tags.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      768 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/mixed-expirations.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      672 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/old_event_api.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/ordering.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1451 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/pings.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/rate.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2577 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/schema-violation.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/send_if_empty_with_metrics.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/single_labeled.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/smaller.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/tags.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/telemetry_mirror.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/text.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/text_invalid.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/unknown_ping_used.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/wrong_key.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/data/yaml_nits.yamlx
--rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/detekt.yml
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     7083 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_javascript.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_javascript_server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14509 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_kotlin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13673 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_lint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7306 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_markdown.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5919 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_metrics.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32166 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_pings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8037 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_rust.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10767 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_swift.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1467 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_tags.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7318 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_translate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1295 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/test_validate_ping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1571 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tests/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 10:14:29.000000 glean_parser-8.1.1/tools/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4715 2023-08-02 10:14:13.000000 glean_parser-8.1.1/tools/extract_data_categories.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6358 2023-09-13 12:45:20.000000 glean_parser-9.0.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      292 2023-09-13 12:45:20.000000 glean_parser-9.0.0/.editorconfig
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/.github/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      323 2023-09-13 12:45:20.000000 glean_parser-9.0.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-09-13 12:45:20.000000 glean_parser-9.0.0/.github/dependabot.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2023-09-13 12:45:20.000000 glean_parser-9.0.0/.github/pull_request_template.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1242 2023-09-13 12:45:20.000000 glean_parser-9.0.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      169 2023-09-13 12:45:20.000000 glean_parser-9.0.0/.swiftlint.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-09-13 12:45:20.000000 glean_parser-9.0.0/AUTHORS.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25913 2023-09-13 12:45:20.000000 glean_parser-9.0.0/CHANGELOG.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-09-13 12:45:20.000000 glean_parser-9.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6006 2023-09-13 12:45:20.000000 glean_parser-9.0.0/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16725 2023-09-13 12:45:20.000000 glean_parser-9.0.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      350 2023-09-13 12:45:20.000000 glean_parser-9.0.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2448 2023-09-13 12:45:20.000000 glean_parser-9.0.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28967 2023-09-13 12:45:36.000000 glean_parser-9.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2282 2023-09-13 12:45:20.000000 glean_parser-9.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/Makefile
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/docs/_static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   116026 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/_static/glean.jpeg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      455 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/authors.md
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4921 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6006 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/contributing.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25913 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/history.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      484 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      929 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/installation.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      774 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/make.bat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      436 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/metrics-yaml.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/pings-yaml.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2282 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/readme.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-09-13 12:45:20.000000 glean_parser-9.0.0/docs/tags-yaml.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      533 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     8631 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4405 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/coverage.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2152 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/data_review.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11230 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/javascript.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6004 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/javascript_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12598 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/kotlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18248 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/lint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9066 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/markdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12431 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15309 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2982 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/pings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6744 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/rust.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser/schemas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19566 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/schemas/metrics.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25849 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/schemas/metrics.2-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4315 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/schemas/pings.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4705 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/schemas/pings.2-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1231 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/schemas/tags.1-0-0.schema.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8379 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/swift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1391 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/tags.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3287 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/data_review.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/javascript.buildinfo.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2669 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/javascript.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5773 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/javascript_server.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      920 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/kotlin.buildinfo.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5099 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/kotlin.geckoview.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5247 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/kotlin.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3425 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/markdown.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/qmldir.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3635 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/rust.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4874 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/templates/swift.jinja2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8148 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/translate.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2037 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/translation_options.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16004 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2118 2023-09-13 12:45:20.000000 glean_parser-9.0.0/glean_parser/validate_ping.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28967 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3278 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       82 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-09-13 12:45:36.000000 glean_parser-9.0.0/glean_parser.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-09-13 12:45:20.000000 glean_parser-9.0.0/pytest.ini
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      335 2023-09-13 12:45:20.000000 glean_parser-9.0.0/requirements_dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      155 2023-09-13 12:45:36.000000 glean_parser-9.0.0/setup.cfg
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2089 2023-09-13 12:45:20.000000 glean_parser-9.0.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/conftest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/tests/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1997 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/all_metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/all_pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      885 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/bad_ping.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9453 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/core.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      786 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/duplicate_labeled.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      518 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/duplicate_send_in_ping.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      104 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/empty.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      755 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/event_key_ordering.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      688 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/events_with_types.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      489 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/fxa-server-metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/fxa-server-pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3539 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/gecko.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      597 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/invalid-ping-names.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/invalid.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      481 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/jwe.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      714 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/metric-with-tags.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      768 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/mixed-expirations.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      672 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/old_event_api.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1232 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/ordering.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1451 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/pings.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1799 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/rate.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2577 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/schema-violation.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      548 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/send_if_empty_with_metrics.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/single_labeled.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/smaller.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      445 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/tags.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/telemetry_mirror.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/text.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1377 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/text_invalid.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      799 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/unknown_ping_used.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1535 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/wrong_key.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      551 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/data/yaml_nits.yamlx
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/detekt.yml
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     7083 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13895 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_javascript.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1869 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_javascript_server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14509 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_kotlin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13673 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_lint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7306 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_markdown.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5919 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_metrics.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32023 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2169 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_pings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8037 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_rust.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10767 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_swift.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1467 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_tags.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7318 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_translate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1108 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1295 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/test_validate_ping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1571 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tests/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-09-13 12:45:36.000000 glean_parser-9.0.0/tools/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     4715 2023-09-13 12:45:20.000000 glean_parser-9.0.0/tools/extract_data_categories.py
```

### Comparing `glean_parser-8.1.1/.circleci/config.yml` & `glean_parser-9.0.0/.circleci/config.yml`

 * *Files 3% similar despite different names*

```diff
@@ -88,29 +88,14 @@
             CC=broken_compiler pip install . --user
       - run:
           name: license-check
           command: |
             pip-licenses --fail-on 'GNU General Public License v3 (GPLv3)'
 
 jobs:
-  build-36:
-    docker:
-      - image: cimg/python:3.6
-    steps:
-      - test-start
-      - test-python-version
-
-  build-36-min:
-    docker:
-      - image: cimg/python:3.6
-    steps:
-      - test-start
-      - test-min-requirements
-      - test-python-version
-
   build-37:
     docker:
       - image: cimg/python:3.7
     steps:
       - test-start
       - test-python-version
 
@@ -218,22 +203,14 @@
           filters:
             tags:
               only: /.*/
       - license-check:
           filters:
             tags:
               only: /.*/
-      - build-36:
-          filters:
-            tags:
-              only: /.*/
-      - build-36-min:
-          filters:
-            tags:
-              only: /.*/
       - build-37:
           filters:
             tags:
               only: /.*/
       - build-38:
           filters:
             tags:
```

### Comparing `glean_parser-8.1.1/.github/pull_request_template.md` & `glean_parser-9.0.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/.gitignore` & `glean_parser-9.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/CHANGELOG.md` & `glean_parser-9.0.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Changelog
 
 ## Unreleased
 
+## 9.0.0
+
+- BREAKING CHANGE: Dropped support for Python 3.6 ([#615](https://github.com/mozilla/glean_parser/issues/615))
+- Allow metadata to configure precise timestamps in pings ([#592](https://github.com/mozilla/glean_parser/pull/592))
+
 ## 8.1.1
 
 - Small updates to the `javascript_server` tempalte to address lint warnings ([#598](https://github.com/mozilla/glean_parser/pull/598))
 
 ## 8.1.0
 
 - Increased the maximum metric name length in version 2.0.0 schema ([#596](https://github.com/mozilla/glean_parser/pull/596))
```

### Comparing `glean_parser-8.1.1/CODE_OF_CONDUCT.md` & `glean_parser-9.0.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/CONTRIBUTING.md` & `glean_parser-9.0.0/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put your
    new functionality into a function with a docstring, and describe
    public-facing features in the docs.
-3. The pull request should work for Python 3.6, 3.7, 3.8 and 3.9 (The CI system
+3. The pull request should work for Python 3.7+ (The CI system
    will take care of testing all of these Python versions).
 4. The pull request should update the changelog in `CHANGELOG.md`.
 
 ## Tips
 
 To run a subset of tests:
```

### Comparing `glean_parser-8.1.1/LICENSE` & `glean_parser-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/Makefile` & `glean_parser-9.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/PKG-INFO` & `glean_parser-9.0.0/glean_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
-Name: glean_parser
-Version: 8.1.1
+Name: glean-parser
+Version: 9.0.0
 Summary: Parser tools for Mozilla's Glean telemetry
 Home-page: https://github.com/mozilla/glean_parser
 Author: The Glean Team
 Author-email: glean-team@mozilla.com
 Keywords: glean_parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -34,30 +33,26 @@
 
 - [How to Contribute](https://github.com/mozilla/glean_parser/blob/main/CONTRIBUTING.md). Please file bugs in [bugzilla](https://bugzilla.mozilla.org/enter_bug.cgi?assigned_to=nobody%40mozilla.org&bug_ignored=0&bug_severity=normal&bug_status=NEW&cf_fission_milestone=---&cf_fx_iteration=---&cf_fx_points=---&cf_status_firefox65=---&cf_status_firefox66=---&cf_status_firefox67=---&cf_status_firefox_esr60=---&cf_status_thunderbird_esr60=---&cf_tracking_firefox65=---&cf_tracking_firefox66=---&cf_tracking_firefox67=---&cf_tracking_firefox_esr60=---&cf_tracking_firefox_relnote=---&cf_tracking_thunderbird_esr60=---&product=Data%20Platform%20and%20Tools&component=Glean%3A%20SDK&contenttypemethod=list&contenttypeselection=text%2Fplain&defined_groups=1&flag_type-203=X&flag_type-37=X&flag_type-41=X&flag_type-607=X&flag_type-721=X&flag_type-737=X&flag_type-787=X&flag_type-799=X&flag_type-800=X&flag_type-803=X&flag_type-835=X&flag_type-846=X&flag_type-855=X&flag_type-864=X&flag_type-916=X&flag_type-929=X&flag_type-930=X&flag_type-935=X&flag_type-936=X&flag_type-937=X&form_name=enter_bug&maketemplate=Remember%20values%20as%20bookmarkable%20template&op_sys=Unspecified&priority=P3&&rep_platform=Unspecified&status_whiteboard=%5Btelemetry%3Aglean-rs%3Am%3F%5D&target_milestone=---&version=unspecified).
 - [User documentation for Glean](https://mozilla.github.io/glean/).
 - [`glean_parser` developer documentation](https://mozilla.github.io/glean_parser/).
 
 ## Requirements
 
--   Python 3.6 (or later)
+-   Python 3.7 (or later)
 
 The following library requirements are installed automatically when
 `glean_parser` is installed by `pip`.
 
 -   appdirs
 -   Click
 -   diskcache
 -   Jinja2
 -   jsonschema
 -   PyYAML
 
-Additionally on Python 3.6:
-
--   iso8601
-
 ## Usage
 
 ```sh
 $ glean_parser --help
 ```
 
 Read in `metrics.yaml`, translate to Kotlin format, and
@@ -74,14 +69,19 @@
 ```
 
 
 # Changelog
 
 ## Unreleased
 
+## 9.0.0
+
+- BREAKING CHANGE: Dropped support for Python 3.6 ([#615](https://github.com/mozilla/glean_parser/issues/615))
+- Allow metadata to configure precise timestamps in pings ([#592](https://github.com/mozilla/glean_parser/pull/592))
+
 ## 8.1.1
 
 - Small updates to the `javascript_server` tempalte to address lint warnings ([#598](https://github.com/mozilla/glean_parser/pull/598))
 
 ## 8.1.0
 
 - Increased the maximum metric name length in version 2.0.0 schema ([#596](https://github.com/mozilla/glean_parser/pull/596))
```

### Comparing `glean_parser-8.1.1/README.md` & `glean_parser-9.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,26 @@
 
 - [How to Contribute](https://github.com/mozilla/glean_parser/blob/main/CONTRIBUTING.md). Please file bugs in [bugzilla](https://bugzilla.mozilla.org/enter_bug.cgi?assigned_to=nobody%40mozilla.org&bug_ignored=0&bug_severity=normal&bug_status=NEW&cf_fission_milestone=---&cf_fx_iteration=---&cf_fx_points=---&cf_status_firefox65=---&cf_status_firefox66=---&cf_status_firefox67=---&cf_status_firefox_esr60=---&cf_status_thunderbird_esr60=---&cf_tracking_firefox65=---&cf_tracking_firefox66=---&cf_tracking_firefox67=---&cf_tracking_firefox_esr60=---&cf_tracking_firefox_relnote=---&cf_tracking_thunderbird_esr60=---&product=Data%20Platform%20and%20Tools&component=Glean%3A%20SDK&contenttypemethod=list&contenttypeselection=text%2Fplain&defined_groups=1&flag_type-203=X&flag_type-37=X&flag_type-41=X&flag_type-607=X&flag_type-721=X&flag_type-737=X&flag_type-787=X&flag_type-799=X&flag_type-800=X&flag_type-803=X&flag_type-835=X&flag_type-846=X&flag_type-855=X&flag_type-864=X&flag_type-916=X&flag_type-929=X&flag_type-930=X&flag_type-935=X&flag_type-936=X&flag_type-937=X&form_name=enter_bug&maketemplate=Remember%20values%20as%20bookmarkable%20template&op_sys=Unspecified&priority=P3&&rep_platform=Unspecified&status_whiteboard=%5Btelemetry%3Aglean-rs%3Am%3F%5D&target_milestone=---&version=unspecified).
 - [User documentation for Glean](https://mozilla.github.io/glean/).
 - [`glean_parser` developer documentation](https://mozilla.github.io/glean_parser/).
 
 ## Requirements
 
--   Python 3.6 (or later)
+-   Python 3.7 (or later)
 
 The following library requirements are installed automatically when
 `glean_parser` is installed by `pip`.
 
 -   appdirs
 -   Click
 -   diskcache
 -   Jinja2
 -   jsonschema
 -   PyYAML
 
-Additionally on Python 3.6:
-
--   iso8601
-
 ## Usage
 
 ```sh
 $ glean_parser --help
 ```
 
 Read in `metrics.yaml`, translate to Kotlin format, and
```

### Comparing `glean_parser-8.1.1/docs/Makefile` & `glean_parser-9.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/docs/_static/glean.jpeg` & `glean_parser-9.0.0/docs/_static/glean.jpeg`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/docs/conf.py` & `glean_parser-9.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/docs/contributing.md` & `glean_parser-9.0.0/docs/contributing.md`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 
 Before you submit a pull request, check that it meets these guidelines:
 
 1. The pull request should include tests.
 2. If the pull request adds functionality, the docs should be updated. Put your
    new functionality into a function with a docstring, and describe
    public-facing features in the docs.
-3. The pull request should work for Python 3.6, 3.7, 3.8 and 3.9 (The CI system
+3. The pull request should work for Python 3.7+ (The CI system
    will take care of testing all of these Python versions).
 4. The pull request should update the changelog in `CHANGELOG.md`.
 
 ## Tips
 
 To run a subset of tests:
```

### Comparing `glean_parser-8.1.1/docs/history.md` & `glean_parser-9.0.0/docs/history.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 # Changelog
 
 ## Unreleased
 
+## 9.0.0
+
+- BREAKING CHANGE: Dropped support for Python 3.6 ([#615](https://github.com/mozilla/glean_parser/issues/615))
+- Allow metadata to configure precise timestamps in pings ([#592](https://github.com/mozilla/glean_parser/pull/592))
+
 ## 8.1.1
 
 - Small updates to the `javascript_server` tempalte to address lint warnings ([#598](https://github.com/mozilla/glean_parser/pull/598))
 
 ## 8.1.0
 
 - Increased the maximum metric name length in version 2.0.0 schema ([#596](https://github.com/mozilla/glean_parser/pull/596))
```

### Comparing `glean_parser-8.1.1/docs/installation.md` & `glean_parser-9.0.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/docs/make.bat` & `glean_parser-9.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/docs/readme.md` & `glean_parser-9.0.0/docs/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,26 @@
 
 - [How to Contribute](https://github.com/mozilla/glean_parser/blob/main/CONTRIBUTING.md). Please file bugs in [bugzilla](https://bugzilla.mozilla.org/enter_bug.cgi?assigned_to=nobody%40mozilla.org&bug_ignored=0&bug_severity=normal&bug_status=NEW&cf_fission_milestone=---&cf_fx_iteration=---&cf_fx_points=---&cf_status_firefox65=---&cf_status_firefox66=---&cf_status_firefox67=---&cf_status_firefox_esr60=---&cf_status_thunderbird_esr60=---&cf_tracking_firefox65=---&cf_tracking_firefox66=---&cf_tracking_firefox67=---&cf_tracking_firefox_esr60=---&cf_tracking_firefox_relnote=---&cf_tracking_thunderbird_esr60=---&product=Data%20Platform%20and%20Tools&component=Glean%3A%20SDK&contenttypemethod=list&contenttypeselection=text%2Fplain&defined_groups=1&flag_type-203=X&flag_type-37=X&flag_type-41=X&flag_type-607=X&flag_type-721=X&flag_type-737=X&flag_type-787=X&flag_type-799=X&flag_type-800=X&flag_type-803=X&flag_type-835=X&flag_type-846=X&flag_type-855=X&flag_type-864=X&flag_type-916=X&flag_type-929=X&flag_type-930=X&flag_type-935=X&flag_type-936=X&flag_type-937=X&form_name=enter_bug&maketemplate=Remember%20values%20as%20bookmarkable%20template&op_sys=Unspecified&priority=P3&&rep_platform=Unspecified&status_whiteboard=%5Btelemetry%3Aglean-rs%3Am%3F%5D&target_milestone=---&version=unspecified).
 - [User documentation for Glean](https://mozilla.github.io/glean/).
 - [`glean_parser` developer documentation](https://mozilla.github.io/glean_parser/).
 
 ## Requirements
 
--   Python 3.6 (or later)
+-   Python 3.7 (or later)
 
 The following library requirements are installed automatically when
 `glean_parser` is installed by `pip`.
 
 -   appdirs
 -   Click
 -   diskcache
 -   Jinja2
 -   jsonschema
 -   PyYAML
 
-Additionally on Python 3.6:
-
--   iso8601
-
 ## Usage
 
 ```sh
 $ glean_parser --help
 ```
 
 Read in `metrics.yaml`, translate to Kotlin format, and
```

### Comparing `glean_parser-8.1.1/glean_parser/__init__.py` & `glean_parser-9.0.0/glean_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/__main__.py` & `glean_parser-9.0.0/glean_parser/__main__.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/coverage.py` & `glean_parser-9.0.0/glean_parser/coverage.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/data_review.py` & `glean_parser-9.0.0/glean_parser/data_review.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/javascript.py` & `glean_parser-9.0.0/glean_parser/javascript.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/javascript_server.py` & `glean_parser-9.0.0/glean_parser/javascript_server.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/kotlin.py` & `glean_parser-9.0.0/glean_parser/kotlin.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/lint.py` & `glean_parser-9.0.0/glean_parser/lint.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/markdown.py` & `glean_parser-9.0.0/glean_parser/markdown.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/metrics.py` & `glean_parser-9.0.0/glean_parser/metrics.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/parser.py` & `glean_parser-9.0.0/glean_parser/parser.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/pings.py` & `glean_parser-9.0.0/glean_parser/pings.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         self.description = description
 
         self.bugs = bugs
         self.notification_emails = notification_emails
         if metadata is None:
             metadata = {}
         self.metadata = metadata
+        self.precise_timestamps = self.metadata.get("precise_timestamps", True)
         if data_reviews is None:
             data_reviews = []
         self.data_reviews = data_reviews
         self.include_client_id = include_client_id
         self.send_if_empty = send_if_empty
         if reasons is None:
             reasons = {}
@@ -84,14 +85,15 @@
         d = self.__dict__.copy()
         del d["name"]
         return d
 
     def _serialize_input(self) -> Dict[str, util.JSONType]:
         d = self.serialize()
         modified_dict = util.remove_output_params(d, "defined_in")
+        modified_dict = util.remove_output_params(modified_dict, "precise_timestamps")
         return modified_dict
 
     def identifier(self) -> str:
         """
         Used for the "generated from ..." comment in the output.
         """
         return self.name
```

### Comparing `glean_parser-8.1.1/glean_parser/rust.py` & `glean_parser-9.0.0/glean_parser/rust.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/schemas/metrics.1-0-0.schema.yaml` & `glean_parser-9.0.0/glean_parser/schemas/metrics.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/schemas/metrics.2-0-0.schema.yaml` & `glean_parser-9.0.0/glean_parser/schemas/metrics.2-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/schemas/pings.1-0-0.schema.yaml` & `glean_parser-9.0.0/glean_parser/schemas/pings.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/schemas/pings.2-0-0.schema.yaml` & `glean_parser-9.0.0/glean_parser/schemas/pings.2-0-0.schema.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -72,14 +72,23 @@
         tags:
           title: Tags
           description: Which tags are specified for this ping.
           type: array
           items:
             type: string
             maxLength: 80
+        precise_timestamps:
+          title: Precise Timestamps
+          description: |
+            When `true` Glean uses millisecond-precise timestamps for
+            the ping's start/end time (the default).
+            When `false` Glean uses minute-precise timestamps for
+            the ping's start/end time.
+          type: boolean
+
       default: {}
 
     include_client_id:
       title: Include client id
       description: |
         **Required.**
```

### Comparing `glean_parser-8.1.1/glean_parser/schemas/tags.1-0-0.schema.yaml` & `glean_parser-9.0.0/glean_parser/schemas/tags.1-0-0.schema.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/swift.py` & `glean_parser-9.0.0/glean_parser/swift.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/tags.py` & `glean_parser-9.0.0/glean_parser/tags.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/templates/data_review.jinja2` & `glean_parser-9.0.0/glean_parser/templates/data_review.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/templates/javascript.jinja2` & `glean_parser-9.0.0/glean_parser/templates/javascript.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/templates/javascript_server.jinja2` & `glean_parser-9.0.0/glean_parser/templates/javascript_server.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
   {% endif %}
   /**
    * Create {{ ping|event_class_name }} instance.
    *
    * @param {string} applicationId - The application ID.
    * @param {string} appDisplayVersion - The application display version.
    * @param {string} channel - The channel.
+   * @param {LoggerOptions} logger_options - The logger options.
    */
   {% if lang == "typescript" %}
   constructor(
     applicationId: string,
     appDisplayVersion: string,
     channel: string,
     logger_options: LoggerOptions
@@ -63,28 +64,35 @@
       {% endif %}
     }
   }
   /**
    * Record and submit a server event object.
    * Event is logged using internal mozlog logger.
    *
+   * @param {string} user_agent - The user agent.
+   * @param {string} ip_address - The IP address. Will be used to decode Geo
+   *                              information and scrubbed at ingestion.
    {% for metric_type, metrics in metrics_by_type.items() %}
    {% for metric in metrics %}
    * @param { {{-metric|js_metric_type-}} } {{ metric|metric_argument_name }} - {{ metric|metric_argument_description }}.
    {% endfor %}
    {% endfor %}
    */
   record({
+    user_agent,
+    ip_address,
     {% for metric_type, metrics in metrics_by_type.items() %}
     {% for metric in metrics %}
     {{ metric|metric_argument_name }},
     {% endfor %}
     {% endfor %}
   {% if lang == "typescript" %}
   }: {
+    user_agent: string,
+    ip_address: string,
     {% for metric_type, metrics in metrics_by_type.items() %}
     {% for metric in metrics %}
     {{ metric|metric_argument_name }}: {{ metric|js_metric_type }};
     {% endfor %}
     {% endfor %}
   {% endif %}
   }) {
@@ -120,14 +128,16 @@
 
     // This is the message structure that Decoder expects: https://github.com/mozilla/gcp-ingestion/pull/2400
     const ping = {
       document_namespace: this._applicationId,
       document_type: '{{ ping }}',
       document_version: '1',
       document_id: uuidv4(),
+      user_agent: user_agent,
+      ip_address: ip_address,
       payload: eventPayloadSerialized,
     };
 
     // this is similar to how FxA currently logs with mozlog: https://github.com/mozilla/fxa/blob/4c5c702a7fcbf6f8c6b1f175e9172cdd21471eac/packages/fxa-auth-server/lib/log.js#L289
     _logger.info(GLEAN_EVENT_MOZLOG_TYPE, ping);
   }
 }
```

### Comparing `glean_parser-8.1.1/glean_parser/templates/kotlin.buildinfo.jinja2` & `glean_parser-9.0.0/glean_parser/templates/kotlin.buildinfo.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/templates/kotlin.geckoview.jinja2` & `glean_parser-9.0.0/glean_parser/templates/kotlin.geckoview.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/templates/kotlin.jinja2` & `glean_parser-9.0.0/glean_parser/templates/kotlin.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/templates/markdown.jinja2` & `glean_parser-9.0.0/glean_parser/templates/markdown.jinja2`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/templates/rust.jinja2` & `glean_parser-9.0.0/glean_parser/templates/rust.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 {% for category in categories %}
 {% if category.contains_pings %}
 {% for obj in category.objs.values() %}
 #[allow(non_upper_case_globals, dead_code)]
 /// {{ obj.description|wordwrap() | replace('\n', '\n/// ') }}
 #[rustfmt::skip]
 pub static {{ obj.name|snake_case }}: ::glean::private::__export::Lazy<::glean::private::PingType> =
-    ::glean::private::__export::Lazy::new(|| ::glean::private::PingType::new("{{ obj.name }}", {{ obj.include_client_id|rust }}, {{ obj.send_if_empty|rust }}, {{ obj.reason_codes|rust }}));
+    ::glean::private::__export::Lazy::new(|| ::glean::private::PingType::new("{{ obj.name }}", {{ obj.include_client_id|rust }}, {{ obj.send_if_empty|rust }}, {{ obj.precise_timestamps|rust }}, {{ obj.reason_codes|rust }}));
 {% endfor %}
 {% else %}
 pub mod {{ category.name|snake_case }} {
     #[allow(unused_imports)] // HistogramType might be unusued, let's avoid warnings
     use glean::{private::*, traits::ExtraKeys, traits::NoExtraKeys, CommonMetricData, HistogramType, Lifetime, TimeUnit, MemoryUnit};
     {% for obj in category.objs.values() %}
```

### Comparing `glean_parser-8.1.1/glean_parser/templates/swift.jinja2` & `glean_parser-9.0.0/glean_parser/templates/swift.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         {% endfor %}
         {% endif %}
         /// {{ obj.description|wordwrap() | replace('\n', '\n        /// ') }}
         let {{ obj.name|camelize|variable_name }} = {{obj|type_name}}(
             name: {{ obj.name|swift }},
             includeClientId: {{obj.include_client_id|swift}},
             sendIfEmpty: {{obj.send_if_empty|swift}},
+            preciseTimestamps: {{obj.precise_timestamps|swift}},
             reasonCodes: {{obj.reason_codes|swift}}
         )
 
       {% endfor %}
     }
 
     {% else %}
```

### Comparing `glean_parser-8.1.1/glean_parser/translate.py` & `glean_parser-9.0.0/glean_parser/translate.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/translation_options.py` & `glean_parser-9.0.0/glean_parser/translation_options.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser/util.py` & `glean_parser-9.0.0/glean_parser/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from collections import OrderedDict
 import datetime
 import functools
 import json
 from pathlib import Path
 import sys
 import textwrap
 from typing import Any, Callable, Iterable, Sequence, Tuple, Union, Optional
@@ -17,63 +16,36 @@
 import appdirs  # type: ignore
 import diskcache  # type: ignore
 import jinja2
 import jsonschema  # type: ignore
 from jsonschema import _utils  # type: ignore
 import yaml
 
-if sys.version_info < (3, 7):
-    import iso8601  # type: ignore
 
-    def date_fromisoformat(datestr: str) -> datetime.date:
-        try:
-            return iso8601.parse_date(datestr).date()
-        except iso8601.ParseError:
-            raise ValueError()
-
-    def datetime_fromisoformat(datestr: str) -> datetime.datetime:
-        try:
-            return iso8601.parse_date(datestr)
-        except iso8601.ParseError:
-            raise ValueError()
+def date_fromisoformat(datestr: str) -> datetime.date:
+    return datetime.date.fromisoformat(datestr)
 
-else:
 
-    def date_fromisoformat(datestr: str) -> datetime.date:
-        return datetime.date.fromisoformat(datestr)
-
-    def datetime_fromisoformat(datestr: str) -> datetime.datetime:
-        return datetime.datetime.fromisoformat(datestr)
+def datetime_fromisoformat(datestr: str) -> datetime.datetime:
+    return datetime.datetime.fromisoformat(datestr)
 
 
 TESTING_MODE = "pytest" in sys.modules
 
 
 JSONType = Union[list, dict, str, int, float, None]
 """
 The types supported by JSON.
 
 This is only an approximation -- this should really be a recursive type.
 """
 
-# Adapted from
-# https://stackoverflow.com/questions/34667108/ignore-dates-and-times-while-parsing-yaml
-
 
-# A wrapper around OrderedDict for Python < 3.7 (where dict ordering is not
-# maintained by default), and regular dict everywhere else.
-if sys.version_info < (3, 7):
-
-    class DictWrapper(OrderedDict):
-        pass
-
-else:
-
-    class DictWrapper(dict):
-        pass
+class DictWrapper(dict):
+    pass
 
 
 class _NoDatesSafeLoader(yaml.SafeLoader):
     @classmethod
     def remove_implicit_resolver(cls, tag_to_remove):
         """
         Remove implicit resolvers for a particular tag
@@ -548,13 +520,14 @@
 
 
 # Names of ping parameters to pass to constructors.
 ping_args = [
     "name",
     "include_client_id",
     "send_if_empty",
+    "precise_timestamps",
     "reason_codes",
 ]
 
 
 # Names of parameters to pass to both metric and ping constructors (no duplicates).
 extra_args = metric_args + [v for v in ping_args if v not in metric_args]
```

### Comparing `glean_parser-8.1.1/glean_parser/validate_ping.py` & `glean_parser-9.0.0/glean_parser/validate_ping.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/glean_parser.egg-info/PKG-INFO` & `glean_parser-9.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
-Name: glean-parser
-Version: 8.1.1
+Name: glean_parser
+Version: 9.0.0
 Summary: Parser tools for Mozilla's Glean telemetry
 Home-page: https://github.com/mozilla/glean_parser
 Author: The Glean Team
 Author-email: glean-team@mozilla.com
 Keywords: glean_parser
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -34,30 +33,26 @@
 
 - [How to Contribute](https://github.com/mozilla/glean_parser/blob/main/CONTRIBUTING.md). Please file bugs in [bugzilla](https://bugzilla.mozilla.org/enter_bug.cgi?assigned_to=nobody%40mozilla.org&bug_ignored=0&bug_severity=normal&bug_status=NEW&cf_fission_milestone=---&cf_fx_iteration=---&cf_fx_points=---&cf_status_firefox65=---&cf_status_firefox66=---&cf_status_firefox67=---&cf_status_firefox_esr60=---&cf_status_thunderbird_esr60=---&cf_tracking_firefox65=---&cf_tracking_firefox66=---&cf_tracking_firefox67=---&cf_tracking_firefox_esr60=---&cf_tracking_firefox_relnote=---&cf_tracking_thunderbird_esr60=---&product=Data%20Platform%20and%20Tools&component=Glean%3A%20SDK&contenttypemethod=list&contenttypeselection=text%2Fplain&defined_groups=1&flag_type-203=X&flag_type-37=X&flag_type-41=X&flag_type-607=X&flag_type-721=X&flag_type-737=X&flag_type-787=X&flag_type-799=X&flag_type-800=X&flag_type-803=X&flag_type-835=X&flag_type-846=X&flag_type-855=X&flag_type-864=X&flag_type-916=X&flag_type-929=X&flag_type-930=X&flag_type-935=X&flag_type-936=X&flag_type-937=X&form_name=enter_bug&maketemplate=Remember%20values%20as%20bookmarkable%20template&op_sys=Unspecified&priority=P3&&rep_platform=Unspecified&status_whiteboard=%5Btelemetry%3Aglean-rs%3Am%3F%5D&target_milestone=---&version=unspecified).
 - [User documentation for Glean](https://mozilla.github.io/glean/).
 - [`glean_parser` developer documentation](https://mozilla.github.io/glean_parser/).
 
 ## Requirements
 
--   Python 3.6 (or later)
+-   Python 3.7 (or later)
 
 The following library requirements are installed automatically when
 `glean_parser` is installed by `pip`.
 
 -   appdirs
 -   Click
 -   diskcache
 -   Jinja2
 -   jsonschema
 -   PyYAML
 
-Additionally on Python 3.6:
-
--   iso8601
-
 ## Usage
 
 ```sh
 $ glean_parser --help
 ```
 
 Read in `metrics.yaml`, translate to Kotlin format, and
@@ -74,14 +69,19 @@
 ```
 
 
 # Changelog
 
 ## Unreleased
 
+## 9.0.0
+
+- BREAKING CHANGE: Dropped support for Python 3.6 ([#615](https://github.com/mozilla/glean_parser/issues/615))
+- Allow metadata to configure precise timestamps in pings ([#592](https://github.com/mozilla/glean_parser/pull/592))
+
 ## 8.1.1
 
 - Small updates to the `javascript_server` tempalte to address lint warnings ([#598](https://github.com/mozilla/glean_parser/pull/598))
 
 ## 8.1.0
 
 - Increased the maximum metric name length in version 2.0.0 schema ([#596](https://github.com/mozilla/glean_parser/pull/596))
```

### Comparing `glean_parser-8.1.1/glean_parser.egg-info/SOURCES.txt` & `glean_parser-9.0.0/glean_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/setup.py` & `glean_parser-9.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,55 +8,51 @@
 """The setup script."""
 
 import sys
 
 from setuptools import setup, find_packages
 
 
-if sys.version_info < (3, 6):
-    print("glean_parser requires at least Python 3.6", file=sys.stderr)
+if sys.version_info < (3, 7):
+    print("glean_parser requires at least Python 3.7", file=sys.stderr)
     sys.exit(1)
 
 
 with open("README.md", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
 with open("CHANGELOG.md", encoding="utf-8") as history_file:
     history = history_file.read()
 
 requirements = [
     "appdirs>=1.4",
     "Click>=7",
     "diskcache>=4",
-    "iso8601>=0.1.10; python_version<='3.6'",
     "Jinja2>=2.10.1",
-    "MarkupSafe>=1.1.1,<=2.0.1",
     "jsonschema>=3.0.2",
     "PyYAML>=5.3.1",
 ]
 
 setup_requirements = [
     "pytest-runner",
-    "setuptools-scm<7; python_version<='3.6'",
-    "setuptools-scm>=7; python_version>'3.6'",
+    "setuptools-scm>=7",
 ]
 
 test_requirements = [
     "pytest",
 ]
 
 setup(
     author="The Glean Team",
     author_email="glean-team@mozilla.com",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
     ],
     description="Parser tools for Mozilla's Glean telemetry",
```

### Comparing `glean_parser-8.1.1/tests/data/all_metrics.yaml` & `glean_parser-9.0.0/tests/data/all_metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/all_pings.yaml` & `glean_parser-9.0.0/tests/data/all_pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/bad_ping.yamlx` & `glean_parser-9.0.0/tests/data/bad_ping.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/core.yaml` & `glean_parser-9.0.0/tests/data/core.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/duplicate_labeled.yaml` & `glean_parser-9.0.0/tests/data/duplicate_labeled.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/duplicate_send_in_ping.yaml` & `glean_parser-9.0.0/tests/data/duplicate_send_in_ping.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/event_key_ordering.yaml` & `glean_parser-9.0.0/tests/data/event_key_ordering.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/events_with_types.yaml` & `glean_parser-9.0.0/tests/data/events_with_types.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/gecko.yaml` & `glean_parser-9.0.0/tests/data/gecko.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/invalid-ping-names.yaml` & `glean_parser-9.0.0/tests/data/invalid-ping-names.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/metric-with-tags.yaml` & `glean_parser-9.0.0/tests/data/metric-with-tags.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/mixed-expirations.yaml` & `glean_parser-9.0.0/tests/data/mixed-expirations.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/old_event_api.yamlx` & `glean_parser-9.0.0/tests/data/old_event_api.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/ordering.yaml` & `glean_parser-9.0.0/tests/data/ordering.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/pings.yaml` & `glean_parser-9.0.0/tests/data/pings.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/rate.yaml` & `glean_parser-9.0.0/tests/data/rate.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/schema-violation.yaml` & `glean_parser-9.0.0/tests/data/schema-violation.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/send_if_empty_with_metrics.yaml` & `glean_parser-9.0.0/tests/data/send_if_empty_with_metrics.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/smaller.yaml` & `glean_parser-9.0.0/tests/data/smaller.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/telemetry_mirror.yaml` & `glean_parser-9.0.0/tests/data/telemetry_mirror.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/text.yaml` & `glean_parser-9.0.0/tests/data/text.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/text_invalid.yaml` & `glean_parser-9.0.0/tests/data/text_invalid.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/unknown_ping_used.yaml` & `glean_parser-9.0.0/tests/data/unknown_ping_used.yaml`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/wrong_key.yamlx` & `glean_parser-9.0.0/tests/data/wrong_key.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/data/yaml_nits.yamlx` & `glean_parser-9.0.0/tests/data/yaml_nits.yamlx`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_cli.py` & `glean_parser-9.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_javascript.py` & `glean_parser-9.0.0/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_javascript_server.py` & `glean_parser-9.0.0/tests/test_javascript_server.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_kotlin.py` & `glean_parser-9.0.0/tests/test_kotlin.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_lint.py` & `glean_parser-9.0.0/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_markdown.py` & `glean_parser-9.0.0/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_metrics.py` & `glean_parser-9.0.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_parser.py` & `glean_parser-9.0.0/tests/test_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # Any copyright is dedicated to the Public Domain.
 # http://creativecommons.org/publicdomain/zero/1.0/
 
 from pathlib import Path
 import json
 import re
-import sys
 import textwrap
 
 import pytest
 
 from glean_parser import metrics
 from glean_parser import parser
 
@@ -50,18 +49,14 @@
     """Test the basics of parsing a single file."""
     all_metrics = parser.parse_objects(ROOT / "data" / "invalid.yamlx")
     errors = list(all_metrics)
     assert len(errors) == 1
     assert "could not determine a constructor for the tag" in errors[0]
 
 
-@pytest.mark.skipif(
-    sys.version_info < (3, 7),
-    reason="Error messages have literal 'OrderedDict' in them on Python 3.6",
-)
 def test_parser_schema_violation():
     """1507792"""
     all_metrics = parser.parse_objects(ROOT / "data" / "schema-violation.yaml")
     errors = list(all_metrics)
 
     found_errors = set(
         re.sub(r"\s", "", str(error).split("\n", 1)[1].strip()) for error in errors
```

### Comparing `glean_parser-8.1.1/tests/test_pings.py` & `glean_parser-9.0.0/tests/test_pings.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_rust.py` & `glean_parser-9.0.0/tests/test_rust.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_swift.py` & `glean_parser-9.0.0/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_tags.py` & `glean_parser-9.0.0/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_translate.py` & `glean_parser-9.0.0/tests/test_translate.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_utils.py` & `glean_parser-9.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/test_validate_ping.py` & `glean_parser-9.0.0/tests/test_validate_ping.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tests/util.py` & `glean_parser-9.0.0/tests/util.py`

 * *Files identical despite different names*

### Comparing `glean_parser-8.1.1/tools/extract_data_categories.py` & `glean_parser-9.0.0/tools/extract_data_categories.py`

 * *Files identical despite different names*

