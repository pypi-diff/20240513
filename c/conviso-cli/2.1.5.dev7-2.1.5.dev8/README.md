# Comparing `tmp/conviso-cli-2.1.5.dev7.tar.gz` & `tmp/conviso-cli-2.1.5.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conviso-cli-2.1.5.dev7.tar", last modified: Thu May  2 18:57:43 2024, max compression
+gzip compressed data, was "conviso-cli-2.1.5.dev8.tar", last modified: Mon May 13 16:29:21 2024, max compression
```

## Comparing `conviso-cli-2.1.5.dev7.tar` & `conviso-cli-2.1.5.dev8.tar`

### file list

```diff
@@ -1,169 +1,169 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:43.001501 conviso-cli-2.1.5.dev7/
--rw-r--r--   0 root         (0) root         (0)      546 2024-05-02 18:57:42.997501 conviso-cli-2.1.5.dev7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      234 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.981501 conviso-cli-2.1.5.dev7/conviso_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      546 2024-05-02 18:57:42.000000 conviso-cli-2.1.5.dev7/conviso_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5691 2024-05-02 18:57:42.000000 conviso-cli-2.1.5.dev7/conviso_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-02 18:57:42.000000 conviso-cli-2.1.5.dev7/conviso_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      110 2024-05-02 18:57:42.000000 conviso-cli-2.1.5.dev7/conviso_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      251 2024-05-02 18:57:42.000000 conviso-cli-2.1.5.dev7/conviso_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-05-02 18:57:42.000000 conviso-cli-2.1.5.dev7/conviso_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.981501 conviso-cli-2.1.5.dev7/convisoappsec/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.981501 conviso-cli-2.1.5.dev7/convisoappsec/common/
--rw-r--r--   0 root         (0) root         (0)      105 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7686 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/common/box.py
--rw-r--r--   0 root         (0) root         (0)    12525 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/common/docker.py
--rw-r--r--   0 root         (0) root         (0)      230 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/common/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2067 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/common/git_data_parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.981501 conviso-cli-2.1.5.dev7/convisoappsec/common/graphql/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/common/graphql/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2055 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/common/graphql/error_handlers.py
--rw-r--r--   0 root         (0) root         (0)      247 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/common/graphql/errors.py
--rw-r--r--   0 root         (0) root         (0)     1323 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/common/graphql/low_client.py
--rw-r--r--   0 root         (0) root         (0)      185 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/common/strings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.981501 conviso-cli-2.1.5.dev7/convisoappsec/flow/
--rw-r--r--   0 root         (0) root         (0)       81 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12044 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.981501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.981501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/__init__.py
--rw-r--r--   0 root         (0) root         (0)      502 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/models/issues/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/models/issues/__init__.py
--rw-r--r--   0 root         (0) root         (0)      310 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/models/issues/iac.py
--rw-r--r--   0 root         (0) root         (0)      421 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/models/issues/normalize.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/models/issues/sast.py
--rw-r--r--   0 root         (0) root         (0)     1673 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/models/issues/sca.py
--rw-r--r--   0 root         (0) root         (0)     3614 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/resources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/schemas/mutations/
--rw-r--r--   0 root         (0) root         (0)      607 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/schemas/resolvers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/models/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)      345 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/models/asset.py
--rw-r--r--   0 root         (0) root         (0)      511 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/models/issues.py
--rw-r--r--   0 root         (0) root         (0)      972 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/models/project.py
--rw-r--r--   0 root         (0) root         (0)     6458 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/resources_api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/schemas/mutations/
--rw-r--r--   0 root         (0) root         (0)     1254 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/schemas/resolvers/
--rw-r--r--   0 root         (0) root         (0)     2352 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.985501 conviso-cli-2.1.5.dev7/convisoappsec/flow/source_code_scanner/
--rw-r--r--   0 root         (0) root         (0)      227 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/source_code_scanner/__init__.py
--rw-r--r--   0 root         (0) root         (0)       57 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/source_code_scanner/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1655 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/source_code_scanner/scc.py
--rw-r--r--   0 root         (0) root         (0)     4726 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/source_code_scanner/source_code_scanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.989501 conviso-cli-2.1.5.dev7/convisoappsec/flow/util/
--rw-r--r--   0 root         (0) root         (0)      160 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2093 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/util/ci_provider.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/util/metrics.py
--rw-r--r--   0 root         (0) root         (0)      508 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/util/source_code_compressor.py
--rw-r--r--   0 root         (0) root         (0)    14635 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/version_control_system_adapter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.989501 conviso-cli-2.1.5.dev7/convisoappsec/flow/version_searchers/
--rw-r--r--   0 root         (0) root         (0)      294 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/version_searchers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     1266 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/version_searchers/timebased_version_seacher.py
--rw-r--r--   0 root         (0) root         (0)      943 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/version_searchers/version_searcher_result.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.989501 conviso-cli-2.1.5.dev7/convisoappsec/flow/versioning_style/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/versioning_style/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1041 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flow/versioning_style/semantic_versioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.989501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/__init__.py
--rw-r--r--   0 root         (0) root         (0)       99 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.989501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/assets/
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2278 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/assets/create.py
--rw-r--r--   0 root         (0) root         (0)      310 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/assets/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     1484 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/assets/ls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.989501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/ast/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/ast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9410 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/ast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     5350 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.989501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/companies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/companies/__init__.py
--rw-r--r--   0 root         (0) root         (0)      892 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/companies/ls.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.993501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.993501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      190 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/context.py
--rw-r--r--   0 root         (0) root         (0)      677 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.993501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      346 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.993501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
--rw-r--r--   0 root         (0) root         (0)       64 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      194 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
--rw-r--r--   0 root         (0) root         (0)      675 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.993501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2815 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
--rw-r--r--   0 root         (0) root         (0)     3500 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
--rw-r--r--   0 root         (0) root         (0)     4681 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/values.py
--rw-r--r--   0 root         (0) root         (0)      353 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      763 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/ls.py
--rw-r--r--   0 root         (0) root         (0)      970 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/show.py
--rw-r--r--   0 root         (0) root         (0)     2878 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.993501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/
--rw-r--r--   0 root         (0) root         (0)       58 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.993501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/create/
--rw-r--r--   0 root         (0) root         (0)       54 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/create/__init__.py
--rw-r--r--   0 root         (0) root         (0)      269 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/create/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.993501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/create/with_/
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/create/with_/__init__.py
--rw-r--r--   0 root         (0) root         (0)      309 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/create/with_/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)     2769 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/create/with_/version_tracker.py
--rw-r--r--   0 root         (0) root         (0)      344 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.993501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/import_sarif/
--rw-r--r--   0 root         (0) root         (0)       66 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/import_sarif/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7209 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/import_sarif/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      331 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/help_option.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.997501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/iac/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/iac/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/iac/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    11269 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/iac/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.997501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/projects/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/projects/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/projects/ls.py
--rw-r--r--   0 root         (0) root         (0)     9438 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/requirements_verifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.997501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/sast/
--rw-r--r--   0 root         (0) root         (0)       49 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)      245 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/sast/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    19208 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/sast/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.997501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/sca/
--rw-r--r--   0 root         (0) root         (0)       47 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/sca/__init__.py
--rw-r--r--   0 root         (0) root         (0)      241 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/sca/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    10781 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/sca/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.997501 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/vulnerability/
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/vulnerability/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4937 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/vulnerability/assert_security_rules.py
--rw-r--r--   0 root         (0) root         (0)      386 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/vulnerability/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/vulnerability/rules_schema.json
--rw-r--r--   0 root         (0) root         (0)    16094 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/flowcli/vulnerability/run.py
--rw-r--r--   0 root         (0) root         (0)      231 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/logger.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.997501 conviso-cli-2.1.5.dev7/convisoappsec/sast/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/sast/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/sast/decision.py
--rw-r--r--   0 root         (0) root         (0)     9230 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/sast/sastbox.py
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/convisoappsec/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.977501 conviso-cli-2.1.5.dev7/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-02 18:57:42.997501 conviso-cli-2.1.5.dev7/scripts/shell_completer/
--rw-r--r--   0 root         (0) root         (0)      624 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/scripts/shell_completer/flow_bash_completer.sh
--rw-r--r--   0 root         (0) root         (0)      147 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/scripts/shell_completer/flow_fish_completer.fish
--rw-r--r--   0 root         (0) root         (0)      844 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/scripts/shell_completer/flow_zsh_completer.sh
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-02 18:57:43.001501 conviso-cli-2.1.5.dev7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1882 2024-05-02 18:57:40.000000 conviso-cli-2.1.5.dev7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/
+-rw-r--r--   0 root         (0) root         (0)      546 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      234 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.316273 conviso-cli-2.1.5.dev8/conviso_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      546 2024-05-13 16:29:21.000000 conviso-cli-2.1.5.dev8/conviso_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5691 2024-05-13 16:29:21.000000 conviso-cli-2.1.5.dev8/conviso_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 16:29:21.000000 conviso-cli-2.1.5.dev8/conviso_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2024-05-13 16:29:21.000000 conviso-cli-2.1.5.dev8/conviso_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      251 2024-05-13 16:29:21.000000 conviso-cli-2.1.5.dev8/conviso_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-05-13 16:29:21.000000 conviso-cli-2.1.5.dev8/conviso_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.316273 conviso-cli-2.1.5.dev8/convisoappsec/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.316273 conviso-cli-2.1.5.dev8/convisoappsec/common/
+-rw-r--r--   0 root         (0) root         (0)      105 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7686 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/common/box.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/common/docker.py
+-rw-r--r--   0 root         (0) root         (0)      230 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/common/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/common/git_data_parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.316273 conviso-cli-2.1.5.dev8/convisoappsec/common/graphql/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/common/graphql/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2055 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/common/graphql/error_handlers.py
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/common/graphql/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/common/graphql/low_client.py
+-rw-r--r--   0 root         (0) root         (0)      185 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/common/strings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.316273 conviso-cli-2.1.5.dev8/convisoappsec/flow/
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12044 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.316273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      502 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/models/issues/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/models/issues/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/models/issues/iac.py
+-rw-r--r--   0 root         (0) root         (0)      421 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/models/issues/normalize.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/models/issues/sast.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/models/issues/sca.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/resources_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/schemas/mutations/
+-rw-r--r--   0 root         (0) root         (0)      607 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/schemas/resolvers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/schemas/resolvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      345 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/models/asset.py
+-rw-r--r--   0 root         (0) root         (0)      511 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/models/issues.py
+-rw-r--r--   0 root         (0) root         (0)      972 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/models/project.py
+-rw-r--r--   0 root         (0) root         (0)     6458 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/resources_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/schemas/mutations/
+-rw-r--r--   0 root         (0) root         (0)     1254 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/schemas/resolvers/
+-rw-r--r--   0 root         (0) root         (0)     2352 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/source_code_scanner/
+-rw-r--r--   0 root         (0) root         (0)      227 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/source_code_scanner/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       57 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/source_code_scanner/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/source_code_scanner/scc.py
+-rw-r--r--   0 root         (0) root         (0)     4726 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/source_code_scanner/source_code_scanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/util/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2093 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/util/ci_provider.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/util/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      508 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/util/source_code_compressor.py
+-rw-r--r--   0 root         (0) root         (0)    14635 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/version_control_system_adapter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/version_searchers/
+-rw-r--r--   0 root         (0) root         (0)      294 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/version_searchers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py
+-rw-r--r--   0 root         (0) root         (0)     1266 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/version_searchers/timebased_version_seacher.py
+-rw-r--r--   0 root         (0) root         (0)      943 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/version_searchers/version_searcher_result.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.320273 conviso-cli-2.1.5.dev8/convisoappsec/flow/versioning_style/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/versioning_style/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flow/versioning_style/semantic_versioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/assets/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/assets/create.py
+-rw-r--r--   0 root         (0) root         (0)      310 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/assets/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/assets/ls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/ast/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/ast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9410 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/ast/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     5350 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/companies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/companies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      892 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/companies/ls.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      190 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/context.py
+-rw-r--r--   0 root         (0) root         (0)      677 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      346 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      194 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/context.py
+-rw-r--r--   0 root         (0) root         (0)      675 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2815 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py
+-rw-r--r--   0 root         (0) root         (0)     4681 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/values.py
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      763 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/ls.py
+-rw-r--r--   0 root         (0) root         (0)      970 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/show.py
+-rw-r--r--   0 root         (0) root         (0)     2878 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/create/
+-rw-r--r--   0 root         (0) root         (0)       54 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/create/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      269 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/create/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.324273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/create/with_/
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/create/with_/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      309 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/create/with_/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/create/with_/version_tracker.py
+-rw-r--r--   0 root         (0) root         (0)      344 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/import_sarif/
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/import_sarif/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7209 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/import_sarif/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      331 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/help_option.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/iac/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/iac/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/iac/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    11269 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/iac/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/projects/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/projects/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/projects/ls.py
+-rw-r--r--   0 root         (0) root         (0)     9438 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/requirements_verifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/sast/
+-rw-r--r--   0 root         (0) root         (0)       49 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/sast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      245 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/sast/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    19208 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/sast/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/sca/
+-rw-r--r--   0 root         (0) root         (0)       47 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/sca/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      241 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/sca/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    10781 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/sca/run.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/vulnerability/
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/vulnerability/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4937 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/vulnerability/assert_security_rules.py
+-rw-r--r--   0 root         (0) root         (0)      386 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/vulnerability/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/vulnerability/rules_schema.json
+-rw-r--r--   0 root         (0) root         (0)    16094 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/flowcli/vulnerability/run.py
+-rw-r--r--   0 root         (0) root         (0)      231 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/logger.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/convisoappsec/sast/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/sast/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/sast/decision.py
+-rw-r--r--   0 root         (0) root         (0)     8990 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/sast/sastbox.py
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/convisoappsec/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.316273 conviso-cli-2.1.5.dev8/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/scripts/shell_completer/
+-rw-r--r--   0 root         (0) root         (0)      624 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/scripts/shell_completer/flow_bash_completer.sh
+-rw-r--r--   0 root         (0) root         (0)      147 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/scripts/shell_completer/flow_fish_completer.fish
+-rw-r--r--   0 root         (0) root         (0)      844 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/scripts/shell_completer/flow_zsh_completer.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 16:29:21.328273 conviso-cli-2.1.5.dev8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1882 2024-05-13 16:29:18.000000 conviso-cli-2.1.5.dev8/setup.py
```

### Comparing `conviso-cli-2.1.5.dev7/PKG-INFO` & `conviso-cli-2.1.5.dev8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conviso-cli
-Version: 2.1.5.dev7
+Version: 2.1.5.dev8
 Summary: UNKNOWN
 Maintainer: Conviso
 Maintainer-email: development@convisoappsec.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/convisoappsec/convisocli/
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `conviso-cli-2.1.5.dev7/conviso_cli.egg-info/PKG-INFO` & `conviso-cli-2.1.5.dev8/conviso_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conviso-cli
-Version: 2.1.5.dev7
+Version: 2.1.5.dev8
 Summary: UNKNOWN
 Maintainer: Conviso
 Maintainer-email: development@convisoappsec.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/convisoappsec/convisocli/
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `conviso-cli-2.1.5.dev7/conviso_cli.egg-info/SOURCES.txt` & `conviso-cli-2.1.5.dev8/conviso_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/common/box.py` & `conviso-cli-2.1.5.dev8/convisoappsec/common/box.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/common/docker.py` & `conviso-cli-2.1.5.dev8/convisoappsec/common/docker.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/common/git_data_parser.py` & `conviso-cli-2.1.5.dev8/convisoappsec/common/git_data_parser.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/common/graphql/error_handlers.py` & `conviso-cli-2.1.5.dev8/convisoappsec/common/graphql/error_handlers.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/common/graphql/low_client.py` & `conviso-cli-2.1.5.dev8/convisoappsec/common/graphql/low_client.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/api.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/api.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/models/issues/sast.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/models/issues/sast.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/models/issues/sca.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/models/issues/sca.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/resources_api.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/resources_api.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/beta/schemas/mutations/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/client.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/client.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/models/project.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/models/project.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/resources_api.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/resources_api.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/schemas/mutations/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/graphql_api/v1/schemas/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/source_code_scanner/scc.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/source_code_scanner/scc.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/source_code_scanner/source_code_scanner.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/source_code_scanner/source_code_scanner.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/util/ci_provider.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/util/ci_provider.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/version_control_system_adapter.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/version_control_system_adapter.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/version_searchers/sorted_by_versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/version_searchers/timebased_version_seacher.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/version_searchers/timebased_version_seacher.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/version_searchers/version_searcher_result.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/version_searchers/version_searcher_result.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flow/versioning_style/semantic_versioning.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flow/versioning_style/semantic_versioning.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/assets/create.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/assets/create.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/assets/ls.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/assets/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/ast/entrypoint.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/ast/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/common.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/common.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/companies/ls.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/companies/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/context.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/context.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/entrypoint.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/time_.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/tag_tracker/sort_by/versioning_style.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/create/with_/values.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/create/with_/values.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/ls.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/deploy/show.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/deploy/show.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/entrypoint.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/create/with_/version_tracker.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/create/with_/version_tracker.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/findings/import_sarif/entrypoint.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/findings/import_sarif/entrypoint.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/iac/run.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/iac/run.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/projects/ls.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/projects/ls.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/requirements_verifier.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/requirements_verifier.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/sast/run.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/sast/run.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/sca/run.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/sca/run.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/vulnerability/assert_security_rules.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/vulnerability/assert_security_rules.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/vulnerability/rules_schema.json` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/vulnerability/rules_schema.json`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/flowcli/vulnerability/run.py` & `conviso-cli-2.1.5.dev8/convisoappsec/flowcli/vulnerability/run.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/sast/decision.py` & `conviso-cli-2.1.5.dev8/convisoappsec/sast/decision.py`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/convisoappsec/sast/sastbox.py` & `conviso-cli-2.1.5.dev8/convisoappsec/sast/sastbox.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,27 +102,21 @@
 
         command = (
             ''' -c {code_dir} -a -o {report} --dedup --diff={previous_commit},{current_commit}'''.format(
                 code_dir=self.CONTAINER_CODE_DIR, previous_commit=previous_commit, current_commit=current_commit,
                 report='output.sarif')
         )
 
-        volumes = {
-            '/var/run/docker.sock': {'bind': '/var/run/docker.sock', 'mode': 'rw'},
-            self.CONTAINER_CODE_DIR: {'bind': self.CONTAINER_CODE_DIR, 'mode': 'rw'}
-        }
-
         create_args = {
             'image': self.image,
-            'entrypoint': ['ruby', '/sastbox2-manager/sastbox_cli.rb'],
+            'entrypoint': ['ruby', 'manager/sastbox_cli.rb'],
             'command': command,
             'tty': True,
             'detach': True,
             'environment': environment,
-            'volumes': volumes,
         }
 
         # clean all containers not running
         for container in self.docker.containers.list(filters={'status': 'exited'}):
             container.remove(force=True)
 
         self.container = self.docker.containers.create(**create_args)
@@ -144,15 +138,15 @@
         source_code_tarball_file.close()
         self.container.start()
 
         for line in self.container.logs(stream=True):
             if log:
                 log(line, new_line=False)
 
-        self.recovery_technologies_file()
+        # self.recovery_technologies_file()
 
         wait_result = self.container.wait()
         status_code = wait_result.get('StatusCode')
 
         if not status_code == self.SUCCESS_EXIT_CODE:
             raise RuntimeError(
                 'SASTBox exiting with error status code'
```

### Comparing `conviso-cli-2.1.5.dev7/scripts/shell_completer/flow_bash_completer.sh` & `conviso-cli-2.1.5.dev8/scripts/shell_completer/flow_bash_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/scripts/shell_completer/flow_zsh_completer.sh` & `conviso-cli-2.1.5.dev8/scripts/shell_completer/flow_zsh_completer.sh`

 * *Files identical despite different names*

### Comparing `conviso-cli-2.1.5.dev7/setup.py` & `conviso-cli-2.1.5.dev8/setup.py`

 * *Files identical despite different names*

