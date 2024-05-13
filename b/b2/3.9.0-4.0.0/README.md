# Comparing `tmp/b2-3.9.0.tar.gz` & `tmp/b2-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b2-3.9.0.tar", last modified: Thu Apr 27 23:21:37 2023, max compression
+gzip compressed data, was "b2-4.0.0.tar", last modified: Mon May 13 08:03:01 2024, max compression
```

## Comparing `b2-3.9.0.tar` & `b2-4.0.0.tar`

### file list

```diff
@@ -1,137 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.100751 b2-3.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-27 23:21:13.000000 b2-3.9.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-27 23:21:13.000000 b2-3.9.0/.github/no-response.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-04-27 23:21:13.000000 b2-3.9.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-04-27 23:21:13.000000 b2-3.9.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 23:21:13.000000 b2-3.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-04-27 23:21:13.000000 b2-3.9.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16671 2023-04-27 23:21:13.000000 b2-3.9.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-27 23:21:13.000000 b2-3.9.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-27 23:21:13.000000 b2-3.9.0/Dockerfile.template
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-27 23:21:13.000000 b2-3.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-27 23:21:13.000000 b2-3.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-27 23:21:37.100751 b2-3.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11242 2023-04-27 23:21:13.000000 b2-3.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-04-27 23:21:13.000000 b2-3.9.0/README.release.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/b2/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-27 23:21:13.000000 b2-3.9.0/b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-27 23:21:13.000000 b2-3.9.0/b2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-27 23:21:13.000000 b2-3.9.0/b2/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/b2/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/argcompleters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/autocomplete_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/b2api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/const.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-04-27 23:21:13.000000 b2-3.9.0/b2/_cli/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-27 23:21:13.000000 b2-3.9.0/b2/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   128195 2023-04-27 23:21:13.000000 b2-3.9.0/b2/console_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-27 23:21:13.000000 b2-3.9.0/b2/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)   174088 2023-04-27 23:21:36.000000 b2-3.9.0/b2/licenses_output.txt
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-27 23:21:13.000000 b2-3.9.0/b2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/b2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-04-27 23:21:37.000000 b2-3.9.0/b2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-27 23:21:13.000000 b2-3.9.0/b2.spec
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/contrib/
--rwxr-xr-x   0 runner    (1001) docker     (123)      486 2023-04-27 23:21:13.000000 b2-3.9.0/contrib/color-b2-logs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-27 23:21:13.000000 b2-3.9.0/contrib/debug_logs.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/contrib/macos/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 23:21:13.000000 b2-3.9.0/contrib/macos/entitlements.plist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.088750 b2-3.9.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 23:21:13.000000 b2-3.9.0/doc/bash_completion.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.092750 b2-3.9.0/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/commands.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7243 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/quick_start.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/replication.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/doc/source/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/authorize_account.rst
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/cancel_all_unfinished_large_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/cancel_large_file.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/clear_account.rst
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/copy_file_by_id.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/create_bucket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/create_key.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/delete_bucket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/delete_file_version.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/delete_key.rst
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/download_file_by_id.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/download_file_by_name.rst
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/get_account_info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/get_bucket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/get_download_auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/get_download_url_with_auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/get_file_info.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/hide_file.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/install_autocomplete.rst
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/list_buckets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/list_keys.rst
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/list_parts.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/list_unfinished_large_files.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/ls.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/make_friendly_url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/make_url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/replication-setup.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/rm.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/sync.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/update_bucket.rst
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/update_file_legal_hold.rst
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/update_file_retention.rst
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/upload_file.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-27 23:21:13.000000 b2-3.9.0/doc/source/subcommands/version.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18652 2023-04-27 23:21:13.000000 b2-3.9.0/noxfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/pyinstaller-hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 23:21:13.000000 b2-3.9.0/pyinstaller-hooks/hook-b2.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-27 23:21:13.000000 b2-3.9.0/pyinstaller-hooks/hook-prettytable.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-27 23:21:13.000000 b2-3.9.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-27 23:21:13.000000 b2-3.9.0/requirements-license.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-27 23:21:13.000000 b2-3.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-27 23:21:37.100751 b2-3.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-04-27 23:21:13.000000 b2-3.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-27 23:21:13.000000 b2-3.9.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/cleanup_buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/test_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (123)    94117 2023-04-27 23:21:13.000000 b2-3.9.0/test/integration/test_b2_command_line.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/static/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-27 23:21:13.000000 b2-3.9.0/test/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-27 23:21:13.000000 b2-3.9.0/test/static/test_licenses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/_cli/test_autocomplete_install.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/_cli/test_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/fixtures/test_source_mod/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_source_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/fixtures/test_source_mod/c/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_source_mod/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_source_mod/c/d.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_source_mod/z.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.096751 b2-3.9.0/test/unit/fixtures/test_target_mod/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_target_mod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.100751 b2-3.9.0/test/unit/fixtures/test_target_mod/a/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_target_mod/a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_target_mod/a/b.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 23:21:37.100751 b2-3.9.0/test/unit/fixtures/test_target_mod/c/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_target_mod/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/fixtures/test_target_mod/z.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/test_arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)   100308 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/test_console_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-04-27 23:21:13.000000 b2-3.9.0/test/unit/test_represent_file_metadata.py
+-rw-r--r--   0        0        0     1350 2024-05-13 08:02:34.888871 b2-4.0.0/LICENSE
+-rw-r--r--   0        0        0     7546 2024-05-13 08:02:34.888871 b2-4.0.0/README.md
+lrwxr-xr-x   0        0        0        0 2024-05-13 08:02:34.888871 b2-4.0.0/b2/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0      554 2024-05-13 08:02:34.888871 b2-4.0.0/b2/__init__.py
+-rw-r--r--   0        0        0      291 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/__init__.py
+-rw-r--r--   0        0        0      422 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/__init__.py
+-rw-r--r--   0        0        0     2100 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/arg_parser_types.py
+-rw-r--r--   0        0        0     3345 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/argcompleters.py
+-rw-r--r--   0        0        0     5262 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/autocomplete_cache.py
+-rw-r--r--   0        0        0    11621 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/autocomplete_install.py
+-rw-r--r--   0        0        0     1898 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/b2api.py
+-rw-r--r--   0        0        0     6817 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/b2args.py
+-rw-r--r--   0        0        0     1129 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/const.py
+-rw-r--r--   0        0        0     2415 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/obj_dumps.py
+-rw-r--r--   0        0        0     1865 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/obj_loads.py
+-rw-r--r--   0        0        0      977 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_cli/shell.py
+-rw-r--r--   0        0        0      298 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_utils/__init__.py
+-rw-r--r--   0        0        0     1595 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_utils/python_compat.py
+-rw-r--r--   0        0        0     7443 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/_utils/uri.py
+-rw-r--r--   0        0        0     9135 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/arg_parser.py
+-rw-r--r--   0        0        0      378 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v3/__init__.py
+-rw-r--r--   0        0        0      349 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v3/__main__.py
+-rw-r--r--   0        0        0     4272 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v3/registry.py
+-rw-r--r--   0        0        0     1506 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v3/rm.py
+-rw-r--r--   0        0        0      446 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v3/sync.py
+-rw-r--r--   0        0        0      378 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v4/__init__.py
+-rw-r--r--   0        0        0      349 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v4/__main__.py
+-rw-r--r--   0        0        0     2230 2024-05-13 08:02:34.888871 b2-4.0.0/b2/_internal/b2v4/registry.py
+-rw-r--r--   0        0        0   193002 2024-05-13 08:02:34.892871 b2-4.0.0/b2/_internal/console_tool.py
+-rw-r--r--   0        0        0     1027 2024-05-13 08:02:34.892871 b2-4.0.0/b2/_internal/json_encoder.py
+-rw-r--r--   0        0        0      435 2024-05-13 08:02:34.892871 b2-4.0.0/b2/_internal/version.py
+-rw-r--r--   0        0        0      918 2024-05-13 08:02:34.892871 b2-4.0.0/b2/_internal/version_listing.py
+-rw-r--r--   0        0        0   157370 2024-05-13 08:02:59.952895 b2-4.0.0/b2/licenses_output.txt
+-rw-r--r--   0        0        0     5432 2024-05-13 08:03:01.464897 b2-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9947 1970-01-01 00:00:00.000000 b2-4.0.0/PKG-INFO
```

### Comparing `b2-3.9.0/LICENSE` & `b2-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `b2-3.9.0/b2/__init__.py` & `b2-4.0.0/b2/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 ######################################################################
 
 # Set default logging handler to avoid "No handler found" warnings.
 import logging  # noqa
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
-import b2.version
-__version__ = b2.version.VERSION
+import b2._internal.version  # noqa: E402
+
+__version__ = b2._internal.version.VERSION
 assert __version__  # PEP-0396
```

### Comparing `b2-3.9.0/b2/_cli/shell.py` & `b2-4.0.0/b2/_internal/_cli/shell.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,34 @@
 ######################################################################
 #
-# File: b2/_cli/shell.py
+# File: b2/_internal/_cli/shell.py
 #
 # Copyright 2023 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
 import os
 import os.path
+import shutil
 from typing import Optional
 
 
 def detect_shell() -> Optional[str]:
     """Detect the shell we are running in."""
     shell_var = os.environ.get('SHELL')
     if shell_var:
         return os.path.basename(shell_var)
     return None
+
+
+def resolve_short_call_name(binary_path: str) -> str:
+    """
+    Resolve the short name of the binary.
+
+    If binary is in PATH, return only basename, otherwise return a full path.
+    This method is to be used with sys.argv[0] to resolve handy name for the user instead of full path.
+    """
+    if shutil.which(binary_path) == binary_path:
+        return os.path.basename(binary_path)
+    return binary_path
```

### Comparing `b2-3.9.0/b2/console_tool.py` & `b2-4.0.0/b2/_internal/console_tool.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 #!/usr/bin/env python3
 # PYTHON_ARGCOMPLETE_OK
 ######################################################################
 #
-# File: b2/console_tool.py
+# File: b2/_internal/console_tool.py
 #
 # Copyright 2019 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
+# ruff: noqa: E402
+from __future__ import annotations
+
+import copy
+import tempfile
+import warnings
+
+from b2._internal._cli.autocomplete_cache import AUTOCOMPLETE  # noqa
+from b2._internal._utils.python_compat import removeprefix
+
+AUTOCOMPLETE.autocomplete_from_cache()
 
 import argparse
 import base64
+import contextlib
 import csv
 import dataclasses
 import datetime
 import functools
 import getpass
 import io
 import json
@@ -24,106 +36,138 @@
 import logging.config
 import os
 import pathlib
 import platform
 import queue
 import re
 import signal
+import subprocess
 import sys
 import threading
 import time
 import unicodedata
-from abc import ABCMeta, abstractclassmethod
+from abc import ABCMeta, abstractmethod
 from concurrent.futures import Executor, Future, ThreadPoolExecutor
 from contextlib import suppress
-
-import requests
-import rst2ansi
-
-import argcomplete
-from tabulate import tabulate
-
-from typing import Optional, Tuple, List, Any, Dict
 from enum import Enum
+from typing import Any, BinaryIO, List
 
 import b2sdk
+import requests
+import rst2ansi
 from b2sdk.v2 import (
     ALL_CAPABILITIES,
     B2_ACCOUNT_INFO_DEFAULT_FILE,
-    B2_ACCOUNT_INFO_PROFILE_FILE,
     B2_ACCOUNT_INFO_ENV_VAR,
+    B2_ACCOUNT_INFO_PROFILE_FILE,
+    DEFAULT_MIN_PART_SIZE,
     DEFAULT_SCAN_MANAGER,
     NO_RETENTION_BUCKET_SETTING,
     REALM_URLS,
     SRC_LAST_MODIFIED_MILLIS,
     SSE_C_KEY_ID_FILE_INFO_KEY_NAME,
+    STDOUT_FILEPATH,
     UNKNOWN_KEY_ID,
     XDG_CONFIG_HOME_ENV_VAR,
+    AbstractAccountInfo,
     ApplicationKey,
     B2Api,
     BasicSyncEncryptionSettingsProvider,
     Bucket,
     BucketRetentionSetting,
     CompareVersionMode,
     DownloadedFile,
     EncryptionAlgorithm,
     EncryptionKey,
     EncryptionMode,
     EncryptionSetting,
     FileRetentionSetting,
     FileVersion,
+    Filter,
     KeepOrDeleteMode,
     LegalHold,
+    LifecycleRule,
     NewerFileSyncMode,
+    ProgressReport,
     ReplicationConfiguration,
+    ReplicationMonitor,
     ReplicationRule,
     ReplicationSetupHelper,
     RetentionMode,
     ScanPoliciesManager,
     Synchronizer,
     SyncReport,
+    TqdmProgressListener,
     UploadMode,
     current_time_millis,
+    escape_control_chars,
     get_included_sources,
     make_progress_listener,
+    notification_rule_response_to_request,
     parse_sync_folder,
-    ReplicationMonitor,
-    ProgressReport,
+    points_to_fifo,
+    substitute_control_chars,
+    unprintable_to_hex,
 )
 from b2sdk.v2.exception import (
     B2Error,
     BadFileInfo,
     EmptyDirectory,
     FileNotPresent,
     MissingAccountData,
     NotADirectory,
     UnableToCreateDirectory,
 )
 from b2sdk.version import VERSION as b2sdk_version
 from class_registry import ClassRegistry
+from tabulate import tabulate
 
-from b2._cli.argcompleters import bucket_name_completer, file_name_completer
-from b2._cli.autocomplete_install import autocomplete_install, \
-    SUPPORTED_SHELLS, AutocompleteInstallError
-from b2._cli.b2api import _get_b2api_for_profile
-from b2._cli.const import B2_APPLICATION_KEY_ID_ENV_VAR, \
-    B2_APPLICATION_KEY_ENV_VAR, B2_USER_AGENT_APPEND_ENV_VAR, \
-    B2_ENVIRONMENT_ENV_VAR, B2_DESTINATION_SSE_C_KEY_B64_ENV_VAR, \
-    B2_DESTINATION_SSE_C_KEY_ID_ENV_VAR, B2_SOURCE_SSE_C_KEY_B64_ENV_VAR, \
-    CREATE_BUCKET_TYPES
-from b2._cli.shell import detect_shell
-from b2.arg_parser import (
-    ArgumentParser,
+from b2._internal._cli.arg_parser_types import (
     parse_comma_separated_list,
     parse_default_retention_period,
     parse_millis_from_float_timestamp,
     parse_range,
 )
-from b2.json_encoder import B2CliJsonEncoder
-from b2.version import VERSION
+from b2._internal._cli.argcompleters import file_name_completer
+from b2._internal._cli.autocomplete_install import (
+    SUPPORTED_SHELLS,
+    AutocompleteInstallError,
+    autocomplete_install,
+)
+from b2._internal._cli.b2api import _get_b2api_for_profile, _get_inmemory_b2api
+from b2._internal._cli.b2args import (
+    add_b2_bucket_uri_argument,
+    add_b2_uri_argument,
+    add_b2id_or_b2_bucket_uri_argument,
+    add_b2id_or_b2_uri_argument,
+    add_b2id_or_file_like_b2_uri_argument,
+    add_b2id_uri_argument,
+    add_bucket_name_argument,
+    get_keyid_and_key_from_env_vars,
+)
+from b2._internal._cli.const import (
+    B2_APPLICATION_KEY_ENV_VAR,
+    B2_APPLICATION_KEY_ID_ENV_VAR,
+    B2_CLI_DOCKER_ENV_VAR,
+    B2_DESTINATION_SSE_C_KEY_B64_ENV_VAR,
+    B2_DESTINATION_SSE_C_KEY_ID_ENV_VAR,
+    B2_ENVIRONMENT_ENV_VAR,
+    B2_ESCAPE_CONTROL_CHARACTERS,
+    B2_SOURCE_SSE_C_KEY_B64_ENV_VAR,
+    B2_USER_AGENT_APPEND_ENV_VAR,
+    CREATE_BUCKET_TYPES,
+    DEFAULT_THREADS,
+)
+from b2._internal._cli.obj_dumps import readable_yaml_dump
+from b2._internal._cli.obj_loads import validated_loads
+from b2._internal._cli.shell import detect_shell, resolve_short_call_name
+from b2._internal._utils.uri import B2URI, B2FileIdURI, B2URIAdapter, B2URIBase
+from b2._internal.arg_parser import B2ArgumentParser, add_normalized_argument
+from b2._internal.json_encoder import B2CliJsonEncoder
+from b2._internal.version import VERSION
 
 piplicenses = None
 prettytable = None
 with suppress(ImportError):
     import piplicenses
     import prettytable
 
@@ -131,29 +175,70 @@
 
 SEPARATOR = '=' * 40
 
 # Enable to get 0.* behavior in the command-line tool.
 # Disable for 1.* behavior.
 VERSION_0_COMPATIBILITY = False
 
-# The name of an executable entry point
-NAME = os.path.basename(sys.argv[0])
-if NAME.endswith('.py'):
-    NAME = 'b2'
+
+def filter_out_empty_values(v, empty_marker=None):
+    if isinstance(v, dict):
+        d = {}
+        for k, v in v.items():
+            new_v = filter_out_empty_values(v, empty_marker=empty_marker)
+            if new_v is not empty_marker:
+                d[k] = new_v
+        return d or empty_marker
+    return v
+
+
+def override_dict(base_dict, override):
+    result = copy.deepcopy(base_dict)
+    for k, v in override.items():
+        if isinstance(v, dict):
+            result[k] = override_dict(result.get(k, {}), v)
+        else:
+            result[k] = v
+    return result
+
+
+class NoControlCharactersStdout:
+    def __init__(self, stdout):
+        self.stdout = stdout
+
+    def __getattr__(self, attr):
+        return getattr(self.stdout, attr)
+
+    def write(self, s):
+        if s:
+            s, cc_present = substitute_control_chars(s)
+            if cc_present:
+                logger.warning('WARNING: Control Characters were detected in the output')
+        self.stdout.write(s)
+
+
+def resolve_b2_bin_call_name(argv: list[str] | None = None) -> str:
+    call_name = resolve_short_call_name((argv or sys.argv)[0])
+    if call_name.endswith('.py'):
+        version_name = re.search(r'[\\/]b2[\\/]_internal[\\/](_?b2v\d+)[\\/]__main__.py', call_name)
+        call_name = version_name.group(1) if version_name else 'b2'
+    if 'b2' not in call_name:  # prevent silliness when calling b2 from under different process
+        return 'b2'
+    return call_name
+
 
 FILE_RETENTION_COMPATIBILITY_WARNING = """
     .. warning::
        Setting file retention mode to '{}' is irreversible - such files can only be ever deleted after their retention
        period passes, regardless of keys (master or not) used. This is especially dangerous when setting bucket default
        retention, as it may lead to high storage costs.
 """.format(RetentionMode.COMPLIANCE.value)
 
 # Strings available to use when formatting doc strings.
 DOC_STRING_DATA = dict(
-    NAME=NAME,
     B2_ACCOUNT_INFO_ENV_VAR=B2_ACCOUNT_INFO_ENV_VAR,
     B2_ACCOUNT_INFO_DEFAULT_FILE=B2_ACCOUNT_INFO_DEFAULT_FILE,
     B2_ACCOUNT_INFO_PROFILE_FILE=B2_ACCOUNT_INFO_PROFILE_FILE,
     XDG_CONFIG_HOME_ENV_VAR=XDG_CONFIG_HOME_ENV_VAR,
     B2_APPLICATION_KEY_ID_ENV_VAR=B2_APPLICATION_KEY_ID_ENV_VAR,
     B2_APPLICATION_KEY_ENV_VAR=B2_APPLICATION_KEY_ENV_VAR,
     B2_USER_AGENT_APPEND_ENV_VAR=B2_USER_AGENT_APPEND_ENV_VAR,
@@ -170,15 +255,15 @@
     """
     b2 command error (user caused).  Accepts exactly one argument: message.
 
     We expect users of shell scripts will parse our ``__str__`` output.
     """
 
     def __init__(self, message):
-        super(CommandError, self).__init__()
+        super().__init__()
         self.message = message
 
     def __str__(self):
         return self.message
 
 
 def local_path_to_b2_path(path):
@@ -207,274 +292,396 @@
     """
     if value is None:
         return None
     else:
         return fcn(value)
 
 
+def format_account_info(account_info: AbstractAccountInfo) -> dict:
+    allowed = account_info.get_allowed()
+    allowed['capabilities'] = sorted(allowed['capabilities'])
+    return dict(
+        accountId=account_info.get_account_id(),
+        accountFilePath=getattr(
+            account_info,
+            'filename',
+            None,
+        ),  # missing in StubAccountInfo in tests
+        allowed=allowed,
+        applicationKeyId=account_info.get_application_key_id(),
+        applicationKey=account_info.get_application_key(),
+        isMasterKey=account_info.is_master_key(),
+        accountAuthToken=account_info.get_account_auth_token(),
+        apiUrl=account_info.get_api_url(),
+        downloadUrl=account_info.get_download_url(),
+        s3endpoint=account_info.get_s3_api_url(),
+    )
+
+
 class DescriptionGetter:
-    def __init__(self, described_cls):
+    def __init__(self, described_cls, **kwargs):
         self.described_cls = described_cls
+        self.kwargs = kwargs
 
     def __str__(self):
-        return self.described_cls._get_description()
+        return self.described_cls._get_description(**self.kwargs)
 
 
 class Described:
     """
     Base class for Commands, providing them with tools for evaluating docstrings to CLI help texts.
     Allows for including superclasses' evaluated docstrings.
     """
 
     @classmethod
-    def _get_description(cls):
+    def _get_description(cls, **kwargs):
         mro_docs = {
-            klass.__name__.upper(): klass.lazy_get_description()
+            klass.__name__: klass.lazy_get_description(**kwargs)
             for klass in cls.mro()
             if klass is not cls and klass.__doc__ and issubclass(klass, Described)
         }
-        return cls.__doc__.format(**DOC_STRING_DATA, **mro_docs)
+        return cls.__doc__.format(**kwargs, **DOC_STRING_DATA, **mro_docs)
+
+    @classmethod
+    def lazy_get_description(cls, **kwargs):
+        return DescriptionGetter(cls, **kwargs)
+
+
+class JSONOptionMixin(Described):
+    """
+    Use ``--json`` to get machine-readable output.
+    Unless ``--json`` is used, the output is human-readable, and may change from one minor version to the next.
+    Therefore, for scripting, it is strongly encouraged to use ``--json``.
+    """
 
     @classmethod
-    def lazy_get_description(cls):
-        return DescriptionGetter(cls)
+    def _setup_parser(cls, parser):
+        parser.add_argument(
+            '--json', action='store_true', help='output in JSON format to use in scripts'
+        )
+        super()._setup_parser(parser)  # noqa
 
 
 class DefaultSseMixin(Described):
     """
     If you want server-side encryption for all of the files that are uploaded to a bucket,
     you can enable SSE-B2 encryption as a default setting for the bucket.
-    In order to do that pass ``--defaultServerSideEncryption=SSE-B2``.
+    In order to do that pass ``--default-server-side-encryption=SSE-B2``.
     The default algorithm is set to AES256 which can by changed
-    with ``--defaultServerSideEncryptionAlgorithm`` parameter.
+    with ``--default-server-side-encryption-algorithm`` parameter.
     All uploads to that bucket, from the time default encryption is enabled onward,
     will then be encrypted with SSE-B2 by default.
 
-    To disable default bucket encryption, use ``--defaultServerSideEncryption=none``.
+    To disable default bucket encryption, use ``--default-server-side-encryption=none``.
 
-    If ``--defaultServerSideEncryption`` is not provided,
+    If ``--default-server-side-encryption`` is not provided,
     default server side encryption is determined by the server.
 
     .. note::
 
         Note that existing files in the bucket are not affected by default bucket encryption settings.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument(
-            '--defaultServerSideEncryption', default=None, choices=('SSE-B2', 'none')
+        add_normalized_argument(
+            parser, '--default-server-side-encryption', default=None, choices=('SSE-B2', 'none')
         )
-        parser.add_argument(
-            '--defaultServerSideEncryptionAlgorithm', default='AES256', choices=('AES256',)
+        add_normalized_argument(
+            parser,
+            '--default-server-side-encryption-algorithm',
+            default='AES256',
+            choices=('AES256',)
         )
 
         super()._setup_parser(parser)  # noqa
 
     @classmethod
     def _get_default_sse_setting(cls, args):
-        mode = apply_or_none(EncryptionMode, args.defaultServerSideEncryption)
+        mode = apply_or_none(EncryptionMode, args.default_server_side_encryption)
         if mode is not None:
             if mode == EncryptionMode.NONE:
-                args.defaultServerSideEncryptionAlgorithm = None
+                args.default_server_side_encryption_algorithm = None
 
             algorithm = apply_or_none(
-                EncryptionAlgorithm, args.defaultServerSideEncryptionAlgorithm
+                EncryptionAlgorithm, args.default_server_side_encryption_algorithm
             )
             return EncryptionSetting(mode=mode, algorithm=algorithm)
 
         return None
 
 
 class DestinationSseMixin(Described):
     """
     To request SSE-B2 or SSE-C encryption for destination files,
-    please set ``--destinationServerSideEncryption=SSE-B2/SSE-C``.
+    please set ``--destination-server-side-encryption=SSE-B2/SSE-C``.
     The default algorithm is set to AES256 which can be changed
-    with ``--destinationServerSideEncryptionAlgorithm`` parameter.
+    with ``--destination-server-side-encryption-algorithm`` parameter.
     Using SSE-C requires providing ``{B2_DESTINATION_SSE_C_KEY_B64_ENV_VAR}`` environment variable,
     containing the base64 encoded encryption key.
     If ``{B2_DESTINATION_SSE_C_KEY_ID_ENV_VAR}`` environment variable is provided,
     it's value will be saved as ``{SSE_C_KEY_ID_FILE_INFO_KEY_NAME}`` in the
     uploaded file's fileInfo.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument(
-            '--destinationServerSideEncryption', default=None, choices=('SSE-B2', 'SSE-C')
+        add_normalized_argument(
+            parser,
+            '--destination-server-side-encryption',
+            default=None,
+            choices=('SSE-B2', 'SSE-C')
         )
-        parser.add_argument(
-            '--destinationServerSideEncryptionAlgorithm', default='AES256', choices=('AES256',)
+        add_normalized_argument(
+            parser,
+            '--destination-server-side-encryption-algorithm',
+            default='AES256',
+            choices=('AES256',)
         )
 
         super()._setup_parser(parser)  # noqa
 
     def _get_destination_sse_setting(self, args):
-        mode = apply_or_none(EncryptionMode, args.destinationServerSideEncryption)
+        mode = apply_or_none(EncryptionMode, args.destination_server_side_encryption)
         if mode is not None:
             algorithm = apply_or_none(
-                EncryptionAlgorithm, args.destinationServerSideEncryptionAlgorithm
+                EncryptionAlgorithm, args.destination_server_side_encryption_algorithm
             )
             if mode == EncryptionMode.SSE_B2:
                 key = None
             elif mode == EncryptionMode.SSE_C:
                 encryption_key_b64 = os.environ.get(B2_DESTINATION_SSE_C_KEY_B64_ENV_VAR)
                 if not encryption_key_b64:
                     raise ValueError(
                         'Using SSE-C requires providing an encryption key via %s env var' %
                         B2_DESTINATION_SSE_C_KEY_B64_ENV_VAR
                     )
                 key_id = os.environ.get(B2_DESTINATION_SSE_C_KEY_ID_ENV_VAR)
                 if key_id is None:
                     self._print_stderr(
-                        'Encrypting file(s) with SSE-C without providing key id. Set %s to allow key '
-                        'identification' % (B2_DESTINATION_SSE_C_KEY_ID_ENV_VAR,)
+                        f'Encrypting file(s) with SSE-C without providing key id. '
+                        f'Set {B2_DESTINATION_SSE_C_KEY_ID_ENV_VAR} to allow key identification.'
                     )
                 key = EncryptionKey(secret=base64.b64decode(encryption_key_b64), key_id=key_id)
             else:
-                raise NotImplementedError(
-                    'Unsupported encryption mode for writes: %s' % (mode.value,)
-                )
+                raise NotImplementedError(f'Unsupported encryption mode for writes: {mode.value}')
             return EncryptionSetting(mode=mode, algorithm=algorithm, key=key)
 
         return None
 
 
 class FileRetentionSettingMixin(Described):
     """
     Setting file retention settings requires the **writeFileRetentions** capability, and only works in bucket
-    with fileLockEnabled=true. Providing ``--fileRetentionMode`` requires providing ``--retainUntil`` which has to
+    with fileLockEnabled=true. Providing ``--file-retention-mode`` requires providing ``--retain-until`` which has to
     be a future timestamp, in the form of an integer representing milliseconds
     since epoch. Leaving out these options results in a file retained according to bucket defaults.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument(
-            '--fileRetentionMode',
+        add_normalized_argument(
+            parser,
+            '--file-retention-mode',
             default=None,
             choices=(RetentionMode.COMPLIANCE.value, RetentionMode.GOVERNANCE.value)
         )
 
-        parser.add_argument(
-            '--retainUntil',
+        add_normalized_argument(
+            parser,
+            '--retain-until',
             type=parse_millis_from_float_timestamp,
             default=None,
             metavar='TIMESTAMP'
         )
         super()._setup_parser(parser)  # noqa
 
     @classmethod
     def _get_file_retention_setting(cls, args):
-        if (args.fileRetentionMode is None) != (args.retainUntil is None):
+        if (args.file_retention_mode is None) != (args.retain_until is None):
             raise ValueError(
-                'provide either both --retainUntil and --fileRetentionMode or none of them'
+                'provide either both --retain-until and --file-retention-mode or none of them'
             )
 
-        file_retention_mode = apply_or_none(RetentionMode, args.fileRetentionMode)
+        file_retention_mode = apply_or_none(RetentionMode, args.file_retention_mode)
         if file_retention_mode is None:
             return None
 
-        return FileRetentionSetting(file_retention_mode, args.retainUntil)
+        return FileRetentionSetting(file_retention_mode, args.retain_until)
+
+
+class HeaderFlagsMixin(Described):
+    @classmethod
+    def _setup_parser(cls, parser: argparse.ArgumentParser) -> None:
+        add_normalized_argument(
+            parser,
+            '--cache-control',
+            help=
+            "optional Cache-Control header, value based on RFC 2616 section 14.9, example: 'public, max-age=86400')"
+        )
+        add_normalized_argument(
+            parser,
+            '--content-disposition',
+            help=
+            "optional Content-Disposition header, value based on RFC 2616 section 19.5.1, example: 'attachment; filename=\"fname.ext\"'"
+        )
+        add_normalized_argument(
+            parser,
+            '--content-encoding',
+            help=
+            "optional Content-Encoding header, value based on RFC 2616 section 14.11, example: 'gzip'"
+        )
+        add_normalized_argument(
+            parser,
+            '--content-language',
+            help=
+            "optional Content-Language header, value based on RFC 2616 section 14.12, example: 'mi, en'"
+        )
+        add_normalized_argument(
+            parser,
+            '--expires',
+            help=
+            "optional Expires header, value based on RFC 2616 section 14.21, example: 'Thu, 01 Dec 2050 16:00:00 GMT'"
+        )
+        super()._setup_parser(parser)
+
+    def _file_info_with_header_args(self, args,
+                                    file_info: dict[str, str] | None) -> dict[str, str] | None:
+        """Construct an updated file_info dictionary.
+        Print a warning if any of file_info items will be overwritten by explicit header arguments.
+        """
+        add_file_info = {}
+        overwritten = []
+        if args.cache_control is not None:
+            add_file_info['b2-cache-control'] = args.cache_control
+        if args.content_disposition is not None:
+            add_file_info['b2-content-disposition'] = args.content_disposition
+        if args.content_encoding is not None:
+            add_file_info['b2-content-encoding'] = args.content_encoding
+        if args.content_language is not None:
+            add_file_info['b2-content-language'] = args.content_language
+        if args.expires is not None:
+            add_file_info['b2-expires'] = args.expires
+
+        for key, value in add_file_info.items():
+            if file_info is not None and key in file_info and file_info[key] != value:
+                overwritten.append(key)
+
+        if overwritten:
+            self._print_stderr(
+                'The following file info items will be overwritten by explicit arguments:\n    ' +
+                '\n    '.join(f'{key} = {add_file_info[key]}' for key in overwritten)
+            )
+
+        if add_file_info:
+            return {**(file_info or {}), **add_file_info}
+        return file_info
 
 
 class LegalHoldMixin(Described):
     """
     Setting legal holds requires the **writeFileLegalHolds** capability, and only works in bucket
     with fileLockEnabled=true.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument(
-            '--legalHold', default=None, choices=(LegalHold.ON.value, LegalHold.OFF.value)
+        add_normalized_argument(
+            parser, '--legal-hold', default=None, choices=(LegalHold.ON.value, LegalHold.OFF.value)
         )
         super()._setup_parser(parser)  # noqa
 
     @classmethod
     def _get_legal_hold_setting(cls, args) -> LegalHold:
-        return apply_or_none(LegalHold.from_string_or_none, args.legalHold)
+        return apply_or_none(LegalHold.from_string_or_none, args.legal_hold)
 
 
 class SourceSseMixin(Described):
     """
     To access SSE-C encrypted files,
-    please set ``--sourceServerSideEncryption=SSE-C``.
+    please set ``--source-server-side-encryption=SSE-C``.
     The default algorithm is set to AES256 which can by changed
-    with ``--sourceServerSideEncryptionAlgorithm`` parameter.
+    with ``--source-server-side-encryption-algorithm`` parameter.
     Using SSE-C requires providing ``{B2_SOURCE_SSE_C_KEY_B64_ENV_VAR}`` environment variable,
     containing the base64 encoded encryption key.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--sourceServerSideEncryption', default=None, choices=('SSE-C',))
-        parser.add_argument(
-            '--sourceServerSideEncryptionAlgorithm', default='AES256', choices=('AES256',)
+        add_normalized_argument(
+            parser, '--source-server-side-encryption', default=None, choices=('SSE-C',)
+        )
+        add_normalized_argument(
+            parser,
+            '--source-server-side-encryption-algorithm',
+            default='AES256',
+            choices=('AES256',)
         )
 
         super()._setup_parser(parser)  # noqa
 
     @classmethod
     def _get_source_sse_setting(cls, args):
-        mode = apply_or_none(EncryptionMode, args.sourceServerSideEncryption)
+        mode = apply_or_none(EncryptionMode, args.source_server_side_encryption)
         if mode is not None:
-            algorithm = apply_or_none(EncryptionAlgorithm, args.sourceServerSideEncryptionAlgorithm)
+            algorithm = apply_or_none(
+                EncryptionAlgorithm, args.source_server_side_encryption_algorithm
+            )
             key = None
             if mode == EncryptionMode.SSE_C:
                 encryption_key_b64 = os.environ.get(B2_SOURCE_SSE_C_KEY_B64_ENV_VAR)
                 if not encryption_key_b64:
                     raise ValueError(
                         'Using SSE-C requires providing an encryption key via %s env var' %
                         B2_SOURCE_SSE_C_KEY_B64_ENV_VAR
                     )
                 key = EncryptionKey(
                     secret=base64.b64decode(encryption_key_b64), key_id=UNKNOWN_KEY_ID
                 )
             else:
                 raise NotImplementedError(
-                    'Encryption modes other than %s are not supported in reads' %
-                    (EncryptionMode.SSE_C.value,)
+                    f'Encryption modes other than {EncryptionMode.SSE_C.value} are not supported in reads'
                 )
             return EncryptionSetting(mode=mode, algorithm=algorithm, key=key)
 
         return None
 
 
 class WriteBufferSizeMixin(Described):
     """
     Use --write-buffer-size to set the size (in bytes) of the buffer used to write files.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--write-buffer-size', type=int, metavar='BYTES')
+        add_normalized_argument(parser, '--write-buffer-size', type=int, metavar='BYTES')
         super()._setup_parser(parser)  # noqa
 
 
 class SkipHashVerificationMixin(Described):
     """
     Use --skip-hash-verification to disable hash check on downloaded files.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--skip-hash-verification', action='store_true', default=False)
+        add_normalized_argument(
+            parser, '--skip-hash-verification', action='store_true', default=False
+        )
         super()._setup_parser(parser)  # noqa
 
 
 class MaxDownloadStreamsMixin(Described):
     """
     Use --max-download-streams-per-file to set max num of streams for parallel downloader.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--max-download-streams-per-file', type=int)
+        add_normalized_argument(parser, '--max-download-streams-per-file', type=int)
         super()._setup_parser(parser)  # noqa
 
 
 class FileIdAndOptionalFileNameMixin(Described):
     """
     Specifying the ``fileName`` is more efficient than leaving it out.
     If you omit the ``fileName``, it requires an initial query to B2
@@ -482,119 +689,376 @@
     file.  This extra query requires the ``readFiles`` capability.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         parser.add_argument('fileName', nargs='?')
         parser.add_argument('fileId')
+        super()._setup_parser(parser)  # noqa
 
     def _get_file_name_from_args(self, args):
         if args.fileName is not None:
             return args.fileName
         file_info = self.api.get_file_info(args.fileId)
         return file_info.file_name
 
 
+class B2URIFileArgMixin:
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_b2id_or_file_like_b2_uri_argument(parser)
+        super()._setup_parser(parser)
+
+    def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2URIBase:
+        return args.B2_URI
+
+
+class B2URIFileIDArgMixin:
+    @classmethod
+    def _setup_parser(cls, parser):
+        parser.add_argument('fileId')
+        super()._setup_parser(parser)
+
+    def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2URIBase:
+        return B2FileIdURI(args.fileId)
+
+
+class B2URIBucketArgMixin:
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_bucket_name_argument(parser)
+        super()._setup_parser(parser)
+
+    def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2URIBase:
+        return B2URI(args.bucketName)
+
+
+class B2URIBucketNFilenameArgMixin:
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_bucket_name_argument(parser)
+        parser.add_argument('fileName').completion = file_name_completer
+        super()._setup_parser(parser)
+
+    def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2URIBase:
+        return B2URI(args.bucketName, args.fileName)
+
+
+class B2URIBucketNFolderNameArgMixin:
+    ALLOW_ALL_BUCKETS: bool = False
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_bucket_name_argument(parser, nargs='?' if cls.ALLOW_ALL_BUCKETS else None)
+        parser.add_argument('folderName', nargs='?').completer = file_name_completer
+        super()._setup_parser(parser)
+
+    def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2URI:
+        return B2URI(removeprefix(args.bucketName or '', "b2://"), args.folderName or '')
+
+
+class B2IDOrB2URIMixin:
+    ALLOW_ALL_BUCKETS: bool = False
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_b2id_or_b2_uri_argument(parser, allow_all_buckets=cls.ALLOW_ALL_BUCKETS)
+        super()._setup_parser(parser)
+
+    def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2URI | B2FileIdURI:
+        return args.B2_URI
+
+
+class B2IDOrB2BucketURIMixin:
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_b2id_or_b2_bucket_uri_argument(parser)
+        super()._setup_parser(parser)
+
+    def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2URI | B2FileIdURI:
+        return args.B2_URI
+
+
+class B2BucketURIMixin:
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_b2_bucket_uri_argument(parser)
+        super()._setup_parser(parser)
+
+    def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2URI:
+        return args.B2_URI
+
+
+class B2IDURIMixin:
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_b2id_uri_argument(parser)
+        super()._setup_parser(parser)
+
+    def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2FileIdURI:
+        return args.B2_URI
+
+
 class UploadModeMixin(Described):
     """
-    Use --incrementalMode to allow for incremental file uploads to safe bandwidth.  This will only affect files, which
+    Use --incremental-mode to allow for incremental file uploads to safe bandwidth.  This will only affect files, which
     have been appended to since last upload.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--incrementalMode', action='store_true')
+        add_normalized_argument(parser, '--incremental-mode', action='store_true')
+        super()._setup_parser(parser)  # noqa
 
     @staticmethod
     def _get_upload_mode_from_args(args):
-        if args.incrementalMode:
+        if args.incremental_mode:
             return UploadMode.INCREMENTAL
         return UploadMode.FULL
 
 
-class Command(Described):
+class ProgressMixin(Described):
+    """
+    If the ``tqdm`` library is installed, progress bar is displayed
+    on stderr.  Without it, simple text progress is printed.
+    Use ``--no-progress`` to disable progress reporting (marginally improves performance in some cases).
+    """
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_normalized_argument(
+            parser, '--no-progress', action='store_true', help="progress will not be reported"
+        )
+        super()._setup_parser(parser)  # noqa
+
+
+class LifecycleRulesMixin(Described):
+    """
+    Use `--lifecycle-rule` to set lifecycle rule for the bucket.
+    Multiple rules can be specified by repeating the option.
+
+    `--lifecycle-rules` option is deprecated and cannot be used together with --lifecycle-rule.
+    """
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        lifecycle_group = parser.add_mutually_exclusive_group()
+        add_normalized_argument(
+            lifecycle_group,
+            '--lifecycle-rule',
+            action='append',
+            default=None,
+            type=functools.partial(validated_loads, expected_type=LifecycleRule),
+            dest='lifecycle_rules',
+            help="Lifecycle rule in JSON format. Can be supplied multiple times.",
+        )
+        add_normalized_argument(
+            lifecycle_group,
+            '--lifecycle-rules',
+            type=functools.partial(validated_loads, expected_type=List[LifecycleRule]),
+            help=
+            "(deprecated; use --lifecycle-rule instead) List of lifecycle rules in JSON format.",
+        )
+
+        super()._setup_parser(parser)  # noqa
+
+
+class ThreadsMixin(Described):
+    """
+    Use --threads to manually adjust the number of threads used in the operation.
+    Otherwise, the number of threads will be automatically chosen.
+    """
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        parser.add_argument('--threads', type=int, default=None)
+        super()._setup_parser(parser)  # noqa
+
+    def _get_threads_from_args(self, args) -> int:
+        return args.threads or DEFAULT_THREADS
+
+    def _set_threads_from_args(self, args):
+        threads = self._get_threads_from_args(args)
+        self.api.services.download_manager.set_thread_pool_size(threads)
+        self.api.services.upload_manager.set_thread_pool_size(threads)
+
+
+class _TqdmCloser:
+    """
+    On OSX using Tqdm with b2sdk causes semaphore leaks. This fix is located here and not in b2sdk, because after this
+    cleanup Tqdm might not work properly, therefore it's best to do it when exiting a python process.
+    """
+
+    def __init__(self, progress_listener):
+        self.progress_listener = progress_listener
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if sys.platform != "darwin" or os.environ.get('B2_TEST_DISABLE_TQDM_CLOSER'):
+            return
+        try:
+            from multiprocessing.synchronize import SemLock
+            tqdm_lock = self.progress_listener.tqdm.get_lock()
+            if tqdm_lock.mp_lock._semlock.name is not None:
+                SemLock._cleanup(tqdm_lock.mp_lock._semlock.name)
+        except Exception as ex:
+            logger.debug('Error encountered during Tqdm cleanup', exc_info=ex)
+
+
+class Command(Described, metaclass=ABCMeta):
+    COMMAND_NAME: str | None = None
     # Set to True for commands that receive sensitive information in arguments
     FORBID_LOGGING_ARGUMENTS = False
 
+    deprecated = False
+
     # The registry for the subcommands, should be reinitialized  in subclass
     subcommands_registry = None
 
     # set to False for commands not requiring b2 authentication
     REQUIRES_AUTH = True
 
     def __init__(self, console_tool):
         self.console_tool = console_tool
-        self.api = console_tool.api
+        self.api = B2URIAdapter(console_tool.api)
         self.stdout = console_tool.stdout
         self.stderr = console_tool.stderr
+        self.quiet = False
+        self.escape_control_characters = True
+        self.exit_stack = contextlib.ExitStack()
+
+    def make_progress_listener(self, file_name: str, quiet: bool):
+        progress_listener = make_progress_listener(file_name, quiet)
+        self.exit_stack.enter_context(progress_listener)
+        if isinstance(progress_listener, TqdmProgressListener):
+            self.exit_stack.enter_context(_TqdmCloser(progress_listener))
+        return progress_listener
 
     @classmethod
     def name_and_alias(cls):
-        name = mixed_case_to_hyphens(cls.__name__)
+        name = cls.COMMAND_NAME or cls.__name__
+        if '-' not in name:
+            name = mixed_case_to_hyphens(name)
         alias = None
         if '-' in name:
             alias = name.replace('-', '_')
         return name, alias
 
     @classmethod
     def register_subcommand(cls, command_class):
         assert cls.subcommands_registry is not None, 'Initialize the registry class'
         name, _ = command_class.name_and_alias()
         decorator = cls.subcommands_registry.register(key=name)(command_class)
         return decorator
 
     @classmethod
-    def get_parser(cls, subparsers=None, parents=None, for_docs=False):
+    def create_parser(
+        cls,
+        subparsers: argparse._SubParsersAction | None = None,
+        parents=None,
+        for_docs=False,
+        name: str | None = None,
+        b2_binary_name: str | None = None,
+    ) -> argparse.ArgumentParser:
+        """
+        Creates a parser for the command.
+
+        :param subparsers: subparsers object to which add new parser
+        :param parents: created ArgumentParser `parents`, see `argparse.ArgumentParser`
+        :param for_docs: if parser is to be used for documentation generation
+        :param name: action name
+        :param b2_binary_name: B2 binary call name
+        :return: created parser
+        """
         if parents is None:
             parents = []
 
-        description = cls._get_description()
+        b2_binary_name = b2_binary_name or resolve_b2_bin_call_name()
+        description = cls._get_description(NAME=b2_binary_name)
 
-        if subparsers is None:
-            name, _ = cls.name_and_alias()
-            parser = ArgumentParser(
-                prog=name,
-                description=description,
-                parents=parents,
-                for_docs=for_docs,
-            )
+        if name:
+            alias = None
         else:
             name, alias = cls.name_and_alias()
+        parser_kwargs = dict(
+            prog=name,
+            description=description,
+            parents=parents,
+            for_docs=for_docs,
+            deprecated=cls.deprecated,
+        )
+
+        if subparsers is None:
+            parser = B2ArgumentParser(**parser_kwargs)
+        else:
             parser = subparsers.add_parser(
-                name,
-                description=description,
-                parents=parents,
+                parser_kwargs.pop('prog'),
+                **parser_kwargs,
                 aliases=[alias] if alias is not None and not for_docs else (),
-                for_docs=for_docs,
+                add_help_all=False,
             )
             # Register class that will handle this particular command, for both name and alias.
             parser.set_defaults(command_class=cls)
 
         cls._setup_parser(parser)
 
         if cls.subcommands_registry:
             if not parents:
-                common_parser = ArgumentParser(add_help=False)
-                common_parser.add_argument(
-                    '--debugLogs', action='store_true', help=argparse.SUPPRESS
+                common_parser = B2ArgumentParser(add_help=False, add_help_all=False)
+                add_normalized_argument(
+                    common_parser, '--debug-logs', action='store_true', help=argparse.SUPPRESS
                 )
                 common_parser.add_argument('--verbose', action='store_true', help=argparse.SUPPRESS)
-                common_parser.add_argument('--logConfig', help=argparse.SUPPRESS)
-                common_parser.add_argument('--profile', default=None)
+                add_normalized_argument(common_parser, '--log-config', help=argparse.SUPPRESS)
+                common_parser.add_argument('--profile', default=None, help=argparse.SUPPRESS)
+                common_parser.add_argument(
+                    '-q', '--quiet', action='store_true', default=False, help=argparse.SUPPRESS
+                )
+
+                common_parser.add_argument(
+                    '--escape-control-characters', action='store_true', help=argparse.SUPPRESS
+                )
+                common_parser.add_argument(
+                    '--no-escape-control-characters',
+                    dest='escape_control_characters',
+                    action='store_false',
+                    help=argparse.SUPPRESS
+                )
+
+                common_parser.set_defaults(escape_control_characters=None)
                 parents = [common_parser]
 
-            subparsers = parser.add_subparsers(prog=parser.prog, title='usages', dest='command')
+            subparsers = parser.add_subparsers(
+                prog=parser.prog,
+                title='usages',
+                dest='command',
+                parser_class=B2ArgumentParser,
+            )
             subparsers.required = True
             for subcommand in cls.subcommands_registry.values():
-                subcommand.get_parser(subparsers=subparsers, parents=parents, for_docs=for_docs)
+                subcommand.create_parser(
+                    subparsers=subparsers,
+                    parents=parents,
+                    for_docs=for_docs,
+                    b2_binary_name=b2_binary_name
+                )
 
         return parser
 
     def run(self, args):
-        pass
+        self.quiet = args.quiet
+        self.escape_control_characters = args.escape_control_characters
+        with self.exit_stack:
+            return self._run(args)
+
+    @abstractmethod
+    def _run(self, args) -> int:
+        ...
 
     @classmethod
     def _setup_parser(cls, parser):
         pass
 
     @classmethod
     def _parse_file_infos(cls, args_info):
@@ -602,73 +1066,162 @@
         for info in args_info:
             parts = info.split('=', 1)
             if len(parts) == 1:
                 raise BadFileInfo(info)
             file_infos[parts[0]] = parts[1]
         return file_infos
 
-    def _print_json(self, data):
-        self._print(json.dumps(data, indent=4, sort_keys=True, cls=B2CliJsonEncoder))
+    def _print_json(self, data) -> None:
+        return self._print(
+            json.dumps(data, indent=4, sort_keys=True, ensure_ascii=True, cls=B2CliJsonEncoder),
+            enforce_output=True
+        )
 
-    def _print(self, *args):
-        self._print_standard_descriptor(self.stdout, 'stdout', *args)
+    def _print_human_readable_structure(self, data) -> None:
+        output = io.StringIO()
+        readable_yaml_dump(data, output)
+        return self._print(output.getvalue().rstrip())
 
-    def _print_stderr(self, *args, **kwargs):
-        self._print_standard_descriptor(self.stderr, 'stderr', *args)
+    def _print(
+        self,
+        *args,
+        enforce_output: bool = False,
+        end: str | None = None,
+    ) -> None:
+        return self._print_standard_descriptor(
+            self.stdout,
+            "stdout",
+            *args,
+            enforce_output=enforce_output,
+            end=end,
+        )
 
-    @classmethod
-    def _print_standard_descriptor(cls, descriptor, descriptor_name, *args):
-        cls._print_helper(descriptor, descriptor.encoding, descriptor_name, *args)
+    def _print_stderr(self, *args, end: str | None = None) -> None:
+        return self._print_standard_descriptor(
+            self.stderr, "stderr", *args, enforce_output=True, end=end
+        )
+
+    def _print_standard_descriptor(
+        self,
+        descriptor,
+        descriptor_name: str,
+        *args,
+        enforce_output: bool = False,
+        end: str | None = None,
+    ) -> None:
+        """
+        Prints to fd, unless quiet is set.
+
+        :param descriptor: file descriptor to print to
+        :param descriptor_name: name of the descriptor, used for error reporting
+        :param args: object to be printed
+        :param enforce_output: overrides quiet setting; Should not be used for anything other than data
+        :param end: end of the line characters; None for default newline
+        """
+        if not self.quiet or enforce_output:
+            self._print_helper(
+                descriptor,
+                descriptor.encoding,
+                descriptor_name,
+                *args,
+                end=end,
+                sanitize=self.escape_control_characters
+            )
 
     @classmethod
-    def _print_helper(cls, descriptor, descriptor_encoding, descriptor_name, *args):
+    def _print_helper(
+        cls,
+        descriptor,
+        descriptor_encoding: str,
+        descriptor_name: str,
+        *args,
+        sanitize: bool = True,
+        end: str | None = None
+    ):
+        if sanitize:
+            args = tuple(unprintable_to_hex(arg) or '' for arg in args)
         try:
             descriptor.write(' '.join(args))
         except UnicodeEncodeError:
             sys.stderr.write(
-                "\nWARNING: Unable to print unicode.  Encoding for %s is: '%s'\n" % (
+                "\nWARNING: Unable to print unicode.  Encoding for {} is: '{}'\n".format(
                     descriptor_name,
                     descriptor_encoding,
                 )
             )
             args = [arg.encode('ascii', 'backslashreplace').decode() for arg in args]
             sys.stderr.write("Trying to print: %s\n" % args)
             descriptor.write(' '.join(args))
-        descriptor.write('\n')
+        descriptor.write("\n" if end is None else end)
 
     def __str__(self):
-        return '%s.%s' % (self.__class__.__module__, self.__class__.__name__)
+        return f'{self.__class__.__module__}.{self.__class__.__name__}'
+
+
+class CmdReplacedByMixin:
+    deprecated = True
+    replaced_by_cmd: type[Command] | tuple[type[Command], ...]
+
+    def run(self, args):
+        self._print_stderr(
+            f'WARNING: `{self.__class__.name_and_alias()[0]}` command is deprecated. '
+            f'Use `{self.get_replaced_command_name()}` instead.'
+        )
+        return super().run(args)
+
+    @classmethod
+    def _get_description(cls, **kwargs):
+        return (
+            f'{super()._get_description(**kwargs)}\n\n'
+            f'.. warning::\n'
+            f'   This command is deprecated. Use ``{cls.get_replaced_command_name()}`` instead.\n'
+        )
+
+    @classmethod
+    def get_replaced_command_name(cls) -> str:
+        if isinstance(cls.replaced_by_cmd, tuple):
+            return ' '.join(cmd.name_and_alias()[0] for cmd in cls.replaced_by_cmd)
+        return cls.replaced_by_cmd.name_and_alias()[0]
 
 
 class B2(Command):
     """
     This program provides command-line access to the B2 service.
 
     There are two flows of authorization:
 
-    * call ``{NAME} authorize-account`` and have the credentials cached in sqlite
+    * call ``{NAME} account authorize`` and have the credentials cached in sqlite
     * set ``{B2_APPLICATION_KEY_ID_ENV_VAR}`` and ``{B2_APPLICATION_KEY_ENV_VAR}`` environment
       variables when running this program
 
     This program caches authentication-related and other data in a local SQLite database.
     The location of this database is determined in the following way:
 
-    If ``profile`` arg is provided:
+    If ``--profile`` arg is provided:
+
     * ``{XDG_CONFIG_HOME_ENV_VAR}/b2/db-<profile>.sqlite``, if ``{XDG_CONFIG_HOME_ENV_VAR}`` env var is set
     * ``{B2_ACCOUNT_INFO_PROFILE_FILE}``
 
     Otherwise:
+
     * ``{B2_ACCOUNT_INFO_ENV_VAR}`` env var's value, if set
     * ``{B2_ACCOUNT_INFO_DEFAULT_FILE}``, if it exists
     * ``{XDG_CONFIG_HOME_ENV_VAR}/b2/account_info``, if ``{XDG_CONFIG_HOME_ENV_VAR}`` env var is set
     * ``{B2_ACCOUNT_INFO_DEFAULT_FILE}``, as default
 
     If the directory ``{XDG_CONFIG_HOME_ENV_VAR}/b2`` does not exist (and is needed), it is created.
     Please note that the above rules may be changed in next versions of b2sdk, and in order to get
-    reliable authentication file location you should use ``b2 get-account-info``.
+    reliable authentication file location you should use ``b2 account get``.
+
+    Control characters escaping is turned on if running under terminal.
+    You can override it by explicitly using `--escape-control-chars`/`--no-escape-control-chars`` option,
+    or by setting `B2_ESCAPE_CONTROL_CHARACTERS` environment variable to either `1` or `0`.
+
+    You can suppress command stdout & stderr output by using ``--quiet`` option.
+    To supress only progress bar, use ``--no-progress`` option.
 
     For more details on one command:
 
     .. code-block::
 
         {NAME} <command> --help
 
@@ -685,45 +1238,47 @@
 
     REQUIRES_AUTH = False
 
     subcommands_registry = ClassRegistry()
 
     @classmethod
     def name_and_alias(cls):
-        return NAME, None
+        return resolve_b2_bin_call_name(), None
 
-    def run(self, args):
+    def _run(self, args):
         # Commands could be named via name or alias, so we fetch
         # the command from args assigned during parser preparation.
         return args.command_class
 
 
-@B2.register_subcommand
-class AuthorizeAccount(Command):
+class AccountAuthorizeBase(Command):
     """
+    Authorize an account with credentials.
+
     Prompts for Backblaze ``applicationKeyId`` and ``applicationKey`` (unless they are given
     on the command line).
 
     You can authorize with either the master application key or
     a normal application key.
 
     To use the master application key, provide the application key ID and
     application key from the ``B2 Cloud Storage Buckets`` page on
     the web site: https://secure.backblaze.com/b2_buckets.htm
 
-    To use a normal application key, created with the ``create-key``
+    To use a normal application key, created with the ``key create``
     command or on the web site, provide the application key ID
     and the application key itself.
 
     You can also optionally provide application key ID and application key
     using environment variables ``{B2_APPLICATION_KEY_ID_ENV_VAR}`` and
     ``{B2_APPLICATION_KEY_ENV_VAR}`` respectively.
 
     Stores an account auth token in a local cache, see
 
+
     .. code-block::
 
         {NAME} --help
 
     for details on how the location of this cache is determined.
 
 
@@ -740,45 +1295,54 @@
         realm_group = parser.add_mutually_exclusive_group()
         realm_group.add_argument('--dev', action='store_true', help=argparse.SUPPRESS)
         realm_group.add_argument('--staging', action='store_true', help=argparse.SUPPRESS)
         realm_group.add_argument('--environment', help=argparse.SUPPRESS)
 
         parser.add_argument('applicationKeyId', nargs='?')
         parser.add_argument('applicationKey', nargs='?')
+        super()._setup_parser(parser)
 
-    def run(self, args):
+    def _run(self, args):
         # Handle internal options for testing inside Backblaze.
         # These are not documented in the usage string.
-        realm = self._get_realm(args)
+        realm = self._get_user_requested_realm(args)
 
         if args.applicationKeyId is None:
             args.applicationKeyId = (
                 os.environ.get(B2_APPLICATION_KEY_ID_ENV_VAR) or
                 input('Backblaze application key ID: ')
             )
 
         if args.applicationKey is None:
             args.applicationKey = (
                 os.environ.get(B2_APPLICATION_KEY_ENV_VAR) or
                 getpass.getpass('Backblaze application key: ')
             )
 
-        return self.authorize(args.applicationKeyId, args.applicationKey, realm)
+        status = self.authorize(args.applicationKeyId, args.applicationKey, realm)
+        if status == 0:
+            data = format_account_info(self.api.account_info)
+            self._print_json(data)
+        return status
 
-    def authorize(self, application_key_id, application_key, realm):
+    def authorize(self, application_key_id, application_key, realm: str | None):
         """
         Perform the authorization and capability checks, report errors.
 
         :param application_key_id: application key ID used to authenticate
         :param application_key: application key
-        :param realm: authorization realm
+        :param realm: authorization realm; if None, production is used
         :return: exit status
         """
+        verbose_realm = bool(realm)
+        realm = realm or 'production'
         url = REALM_URLS.get(realm, realm)
-        self._print('Using %s' % url)
+        logger.info(f"Using {url}")
+        if verbose_realm:
+            self._print_stderr(f'Using {url}')
         try:
             self.api.authorize_account(realm, application_key_id, application_key)
 
             allowed = self.api.account_info.get_allowed()
             if 'listBuckets' not in allowed['capabilities']:
                 logger.error(
                     'ConsoleTool cannot work with a bucket-restricted key and no listBuckets capability'
@@ -787,174 +1351,164 @@
                     'ERROR: application key has no listBuckets capability, which is required for the b2 command-line tool'
                 )
                 self.api.account_info.clear()
                 return 1
             if allowed['bucketId'] is not None and allowed['bucketName'] is None:
                 logger.error('ConsoleTool has bucket-restricted key and the bucket does not exist')
                 self._print_stderr(
-                    "ERROR: application key is restricted to bucket id '%s', which no longer exists"
-                    % (allowed['bucketId'],)
+                    "ERROR: application key is restricted to bucket id '{}', which no longer exists"
+                    .format(allowed['bucketId'])
                 )
                 self.api.account_info.clear()
                 return 1
             return 0
         except B2Error as e:
             logger.exception('ConsoleTool account authorization error')
             self._print_stderr('ERROR: unable to authorize account: ' + str(e))
             return 1
 
     @classmethod
-    def _get_realm(cls, args):
+    def _get_user_requested_realm(cls, args) -> str | None:
+        """
+        Determine the realm to use for authorization.
+        """
         if args.dev:
             return 'dev'
         if args.staging:
             return 'staging'
         if args.environment:
             return args.environment
 
-        return os.environ.get(B2_ENVIRONMENT_ENV_VAR, 'production')
-
-
-@B2.register_subcommand
-class CancelAllUnfinishedLargeFiles(Command):
-    """
-    Lists all large files that have been started but not
-    finished and cancels them.  Any parts that have been
-    uploaded will be deleted.
-
-    Requires capability:
-
-    - **listFiles**
-    - **writeFiles**
-    """
-
-    @classmethod
-    def _setup_parser(cls, parser):
-        parser.add_argument('bucketName').completer = bucket_name_completer
-
-    def run(self, args):
-        bucket = self.api.get_bucket_by_name(args.bucketName)
-        for file_version in bucket.list_unfinished_large_files():
-            bucket.cancel_large_file(file_version.file_id)
-            self._print(file_version.file_id, 'canceled')
-        return 0
+        return os.environ.get(B2_ENVIRONMENT_ENV_VAR)
 
 
-@B2.register_subcommand
-class CancelLargeFile(Command):
+class FileLargeUnfinishedCancelBase(Command):
     """
-    Cancels a large file upload.  Used to undo a ``start-large-file``.
-
+    When used with a b2id://fileId, cancels a large file upload.
     Cannot be used once the file is finished.  After finishing,
-    using ``delete-file-version`` to delete the large file.
+    use ``rm`` to delete the large file.
+
+    When used with a b2://bucketName, lists all large files that
+    have been started but not finished and cancels them.  Any parts
+    that have been uploaded will be deleted.
 
     Requires capability:
 
+    - **listFiles** (if canceling unfinished large files in a bucket)
     - **writeFiles**
     """
 
-    @classmethod
-    def _setup_parser(cls, parser):
-        parser.add_argument('fileId')
-
-    def run(self, args):
-        self.api.cancel_large_file(args.fileId)
-        self._print(args.fileId, 'canceled')
+    def _run(self, args):
+        b2_uri = self.get_b2_uri_from_arg(args)
+        if isinstance(b2_uri, B2FileIdURI):
+            self.api.cancel_large_file(b2_uri.file_id)
+            self._print(b2_uri.file_id, 'canceled')
+        elif isinstance(b2_uri, B2URI):
+            bucket = self.api.get_bucket_by_name(b2_uri.bucket_name)
+            for file_version in bucket.list_unfinished_large_files():
+                bucket.cancel_large_file(file_version.file_id)
+                self._print(file_version.file_id, 'canceled')
+        else:
+            self._print_stderr(f'ERROR: unsupported URI "{b2_uri}"')
+            return 1
         return 0
 
 
-@B2.register_subcommand
-class ClearAccount(Command):
+class AccountClearBase(Command):
     """
-    Erases everything in local cache.
+    Erase everything in local cache.
 
     See
 
     .. code-block::
 
         {NAME} --help
 
     for details on how the location of this cache is determined.
     """
 
     REQUIRES_AUTH = False
 
-    def run(self, args):
+    def _run(self, args):
         self.api.account_info.clear()
         return 0
 
 
-@B2.register_subcommand
-class CopyFileById(
-    DestinationSseMixin, SourceSseMixin, FileRetentionSettingMixin, LegalHoldMixin, Command
+class FileCopyByIdBase(
+    HeaderFlagsMixin, DestinationSseMixin, SourceSseMixin, FileRetentionSettingMixin,
+    LegalHoldMixin, Command
 ):
     """
     Copy a file version to the given bucket (server-side, **not** via download+upload).
+
     Copies the contents of the source B2 file to destination bucket
     and assigns the given name to the new B2 file,
     possibly setting options like server-side encryption and retention.
 
     {FILE_RETENTION_COMPATIBILITY_WARNING}
 
-    By default, it copies the file info and content type, therefore ``--contentType`` and ``--info`` are optional.
+    By default, it copies the file info and content type, therefore ``--content-type`` and ``--info`` are optional.
     If one of them is set, the other has to be set as well.
 
-    To force the destination file to have empty fileInfo, use ``--noInfo``.
+    To force the destination file to have empty fileInfo, use ``--no-info``.
 
     By default, the whole file gets copied, but you can copy an (inclusive!) range of bytes
     from the source file to the new file using ``--range`` option.
 
     Each ``--info`` entry is in the form ``a=b``, you can specify many.
 
     The maximum file size is 5GB or 10TB, depending on capability of installed ``b2sdk`` version.
 
-    {DESTINATIONSSEMIXIN}
-    {SOURCESSEMIXIN}
-    {FILERETENTIONSETTINGMIXIN}
-    {LEGALHOLDMIXIN}
+    {DestinationSseMixin}
+    {SourceSseMixin}
+    {FileRetentionSettingMixin}
+    {LegalHoldMixin}
 
-    If either the source or the destination uses SSE-C and ``--contentType`` and ``--info`` are not provided, then
+    If either the source or the destination uses SSE-C and ``--content-type`` and ``--info`` are not provided, then
     to perform the copy the source file's metadata has to be fetched first - an additional request to B2 cloud has
-    to be made. To achieve that, provide ``--fetchMetadata``. Without that flag, the command will fail.
+    to be made. To achieve that, provide ``--fetch-metadata``. Without that flag, the command will fail.
 
     Requires capability:
 
     - **readFiles** (if ``sourceFileId`` bucket is private)
     - **writeFiles**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--fetchMetadata', action='store_true', default=False)
-        parser.add_argument('--metadataDirective', default=None, help=argparse.SUPPRESS)
-        parser.add_argument('--contentType')
+        add_normalized_argument(parser, '--fetch-metadata', action='store_true', default=False)
+        add_normalized_argument(
+            parser, '--metadata-directive', default=None, help=argparse.SUPPRESS
+        )
+        add_normalized_argument(parser, '--content-type')
         parser.add_argument('--range', type=parse_range)
 
         info_group = parser.add_mutually_exclusive_group()
 
-        info_group.add_argument('--info', action='append', default=[])
-        info_group.add_argument('--noInfo', action='store_true', default=False)
+        add_normalized_argument(info_group, '--info', action='append')
+        add_normalized_argument(info_group, '--no-info', action='store_true', default=False)
 
         parser.add_argument('sourceFileId')
         parser.add_argument('destinationBucketName')
         parser.add_argument('b2FileName')
 
         super()._setup_parser(parser)  # add parameters from the mixins
 
-    def run(self, args):
+    def _run(self, args):
         file_infos = None
         if args.info:
             file_infos = self._parse_file_infos(args.info)
-        elif args.noInfo:
+        elif args.no_info:
             file_infos = {}
+        file_infos = self._file_info_with_header_args(args, file_infos)
 
-        if args.metadataDirective is not None:
+        if args.metadata_directive is not None:
             self._print_stderr(
-                '--metadataDirective is deprecated, the value of this argument is determined based on the existence of '
-                '--contentType and --info.'
+                '--metadata-directive is deprecated, the value of this argument is determined based on the existence of '
+                '--content-type and --info.'
             )
 
         bucket = self.api.get_bucket_by_name(args.destinationBucketName)
         destination_encryption_setting = self._get_destination_sse_setting(args)
         source_encryption_setting = self._get_source_sse_setting(args)
         legal_hold = self._get_legal_hold_setting(args)
         file_retention = self._get_file_retention_setting(args)
@@ -965,474 +1519,527 @@
             }
         else:
             range_args = {}
         source_file_info, source_content_type = self._determine_source_metadata(
             source_file_id=args.sourceFileId,
             source_encryption=source_encryption_setting,
             destination_encryption=destination_encryption_setting,
-            target_content_type=args.contentType,
+            target_content_type=args.content_type,
             target_file_info=file_infos,
-            fetch_if_necessary=args.fetchMetadata,
+            fetch_if_necessary=args.fetch_metadata,
         )
         file_version = bucket.copy(
             args.sourceFileId,
             args.b2FileName,
             **range_args,
-            content_type=args.contentType,
+            content_type=args.content_type,
             file_info=file_infos,
             destination_encryption=destination_encryption_setting,
             source_encryption=source_encryption_setting,
             legal_hold=legal_hold,
             file_retention=file_retention,
             source_file_info=source_file_info,
             source_content_type=source_content_type,
         )
         self._print_json(file_version)
         return 0
 
-    def _is_ssec(self, encryption: Optional[EncryptionSetting]):
+    def _is_ssec(self, encryption: EncryptionSetting | None):
         if encryption is not None and encryption.mode == EncryptionMode.SSE_C:
             return True
         return False
 
     def _determine_source_metadata(
         self,
         source_file_id: str,
-        destination_encryption: Optional[EncryptionSetting],
-        source_encryption: Optional[EncryptionSetting],
-        target_file_info: Optional[dict],
-        target_content_type: Optional[str],
+        destination_encryption: EncryptionSetting | None,
+        source_encryption: EncryptionSetting | None,
+        target_file_info: dict | None,
+        target_content_type: str | None,
         fetch_if_necessary: bool,
-    ) -> Tuple[Optional[dict], Optional[str]]:
+    ) -> tuple[dict | None, str | None]:
         """Determine if source file metadata is necessary to perform the copy - due to sse_c_key_id"""
         if not self._is_ssec(source_encryption) and not self._is_ssec(
             destination_encryption
         ):  # no sse-c, no problem
             return None, None
         if target_file_info is not None or target_content_type is not None:  # metadataDirective=REPLACE, no problem
             return None, None
         if not fetch_if_necessary:
             raise ValueError(
                 'Attempting to copy file with metadata while either source or destination uses '
-                'SSE-C. Use --fetchMetadata to fetch source file metadata before copying.'
+                'SSE-C. Use --fetch-metadata to fetch source file metadata before copying.'
             )
         source_file_version = self.api.get_file_info(source_file_id)
         return source_file_version.file_info, source_file_version.content_type
 
 
-@B2.register_subcommand
-class CreateBucket(DefaultSseMixin, Command):
+class BucketCreateBase(DefaultSseMixin, LifecycleRulesMixin, Command):
     """
-    Creates a new bucket.  Prints the ID of the bucket created.
+    Create a new bucket.
 
+    Prints the ID of the bucket created.
     Optionally stores bucket info, CORS rules and lifecycle rules with the bucket.
     These can be given as JSON on the command line.
 
-    {DEFAULTSSEMIXIN}
+    {DefaultSseMixin}
+    {LifecycleRulesMixin}
 
     Requires capability:
 
     - **writeBuckets**
     - **readBucketEncryption**
     - **writeBucketEncryption**
     - **writeBucketRetentions**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--bucketInfo', type=json.loads)
-        parser.add_argument('--corsRules', type=json.loads)
-        parser.add_argument('--lifecycleRules', type=json.loads)
-        parser.add_argument(
-            '--fileLockEnabled',
+        add_normalized_argument(parser, '--bucket-info', type=validated_loads)
+        add_normalized_argument(
+            parser,
+            '--cors-rules',
+            type=validated_loads,
+            help=
+            "If given, the bucket will have a 'custom' CORS configuration. Accepts a JSON string."
+        )
+        add_normalized_argument(
+            parser,
+            '--file-lock-enabled',
             action='store_true',
             help=
             "If given, the bucket will have the file lock mechanism enabled. This parameter cannot be changed after bucket creation."
         )
-        parser.add_argument('--replication', type=json.loads)
-        parser.add_argument('bucketName')
+        parser.add_argument('--replication', type=validated_loads)
+        add_bucket_name_argument(parser)
         parser.add_argument('bucketType', choices=CREATE_BUCKET_TYPES)
 
         super()._setup_parser(parser)  # add parameters from the mixins
 
-    def run(self, args):
+    def _run(self, args):
         encryption_setting = self._get_default_sse_setting(args)
         bucket = self.api.create_bucket(
             args.bucketName,
             args.bucketType,
-            bucket_info=args.bucketInfo,
-            cors_rules=args.corsRules,
-            lifecycle_rules=args.lifecycleRules,
+            bucket_info=args.bucket_info,
+            cors_rules=args.cors_rules,
+            lifecycle_rules=args.lifecycle_rules,
             default_server_side_encryption=encryption_setting,
-            is_file_lock_enabled=args.fileLockEnabled,
+            is_file_lock_enabled=args.file_lock_enabled,
             replication=args.replication and ReplicationConfiguration.from_dict(args.replication),
         )
         self._print(bucket.id_)
         return 0
 
 
-@B2.register_subcommand
-class CreateKey(Command):
+class KeyCreateBase(Command):
     """
-    Creates a new application key.  Prints the application key information.  This is the only
+    Create a new application key.
+
+    Prints the application key information.  This is the only
     time the application key itself will be returned.  Listing application keys will show
     their IDs, but not the secret keys.
 
     The capabilities are passed in as a comma-separated list, like ``readFiles,writeFiles``.
-    Optionally, you can pass all capabilities known to this client with ``--allCapabilities``.
+    Optionally, you can pass all capabilities known to this client with ``--all-capabilities``.
 
     The ``duration`` is the length of time (in seconds) the new application key will exist.
     When the time expires the key will disappear and will no longer be usable.  If not
     specified, the key will not expire.
 
     The ``bucket`` is the name of a bucket in the account.  When specified, the key
     will only allow access to that bucket.
 
     The ``namePrefix`` restricts file access to files whose names start with the prefix.
 
     The output is the new application key ID, followed by the application key itself.
-    The two values returned are the two that you pass to ``authorize-account`` to use the key.
+    The two values returned are the two that you pass to ``account authorize`` to use the key.
 
     Requires capability:
 
     - **writeKeys**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         parser.add_argument('--bucket')
-        parser.add_argument('--namePrefix')
+        add_normalized_argument(parser, '--name-prefix')
         parser.add_argument('--duration', type=int)
         parser.add_argument('keyName')
 
         capabilities = parser.add_mutually_exclusive_group(required=True)
         capabilities.add_argument('capabilities', type=parse_comma_separated_list, nargs='?')
-        capabilities.add_argument('--allCapabilities', action='store_true')
+        add_normalized_argument(capabilities, '--all-capabilities', action='store_true')
+        super()._setup_parser(parser)
 
-    def run(self, args):
+    def _run(self, args):
         # Translate the bucket name into a bucketId
         if args.bucket is None:
             bucket_id_or_none = None
         else:
             bucket_id_or_none = self.api.get_bucket_by_name(args.bucket).id_
 
-        if args.allCapabilities:
-            args.capabilities = ALL_CAPABILITIES
+        if args.all_capabilities:
+            current_key_caps = set(self.api.account_info.get_allowed()['capabilities'])
+            preview_feature_caps = {
+                'readBucketNotifications',
+                'writeBucketNotifications',
+            }
+            args.capabilities = sorted(
+                set(ALL_CAPABILITIES) - preview_feature_caps | current_key_caps
+            )
 
         application_key = self.api.create_key(
             capabilities=args.capabilities,
             key_name=args.keyName,
             valid_duration_seconds=args.duration,
             bucket_id=bucket_id_or_none,
-            name_prefix=args.namePrefix
+            name_prefix=args.name_prefix
         )
 
-        self._print('%s %s' % (application_key.id_, application_key.application_key))
+        self._print(f'{application_key.id_} {application_key.application_key}')
         return 0
 
 
-@B2.register_subcommand
-class DeleteBucket(Command):
+class BucketDeleteBase(Command):
     """
-    Deletes the bucket with the given name.
+    Delete the bucket with the given name.
 
     Requires capability:
 
     - **deleteBuckets**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('bucketName').completer = bucket_name_completer
+        add_bucket_name_argument(parser)
+        super()._setup_parser(parser)
 
-    def run(self, args):
+    def _run(self, args):
         bucket = self.api.get_bucket_by_name(args.bucketName)
         self.api.delete_bucket(bucket)
         return 0
 
 
-@B2.register_subcommand
-class DeleteFileVersion(FileIdAndOptionalFileNameMixin, Command):
+class DeleteFileVersionBase(FileIdAndOptionalFileNameMixin, Command):
     """
-    Permanently and irrevocably deletes one version of a file.
+    Permanently and irrevocably delete one version of a file.
+
+    {FileIdAndOptionalFileNameMixin}
 
-    {FILEIDANDOPTIONALFILENAMEMIXIN}
+    If a file is in governance retention mode, and the retention period has not expired, adding ``--bypass-governance``
+    is required.
 
     Requires capability:
 
     - **deleteFiles**
     - **readFiles** (if file name not provided)
+
+    and optionally:
+
+    - **bypassGovernance**
     """
 
-    def run(self, args):
-        file_name = self._get_file_name_from_args(args)
+    @classmethod
+    def _setup_parser(cls, parser):
+        super()._setup_parser(parser)
+        add_normalized_argument(parser, '--bypass-governance', action='store_true', default=False)
 
-        file_info = self.api.delete_file_version(args.fileId, file_name)
+    def _run(self, args):
+        file_name = self._get_file_name_from_args(args)
+        file_info = self.api.delete_file_version(args.fileId, file_name, args.bypass_governance)
         self._print_json(file_info)
         return 0
 
 
-@B2.register_subcommand
-class DeleteKey(Command):
+class KeyDeleteBase(Command):
     """
-    Deletes the specified application key by its ID.
+    Delete the specified application key by ID.
 
     Requires capability:
 
     - **deleteKeys**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         parser.add_argument('applicationKeyId')
+        super()._setup_parser(parser)
 
-    def run(self, args):
+    def _run(self, args):
         application_key = self.api.delete_key_by_id(application_key_id=args.applicationKeyId)
         self._print(application_key.id_)
         return 0
 
 
-class DownloadCommand(Command):
+class DownloadCommand(
+    ProgressMixin,
+    SourceSseMixin,
+    WriteBufferSizeMixin,
+    SkipHashVerificationMixin,
+    Command,
+    metaclass=ABCMeta
+):
     """ helper methods for returning results from download commands """
 
-    def _print_download_info(self, downloaded_file: DownloadedFile):
+    def _print_download_info(
+        self, downloaded_file: DownloadedFile, output_filepath: pathlib.Path
+    ) -> None:
         download_version = downloaded_file.download_version
+        output_filepath_string = 'stdout' if output_filepath == STDOUT_FILEPATH else str(
+            output_filepath.resolve()
+        )
         self._print_file_attribute('File name', download_version.file_name)
         self._print_file_attribute('File id', download_version.id_)
+        self._print_file_attribute('Output file path', output_filepath_string)
         self._print_file_attribute('File size', str(download_version.content_length))
         self._print_file_attribute('Content type', download_version.content_type)
         self._print_file_attribute('Content sha1', download_version.content_sha1)
         self._print_file_attribute(
             'Encryption', self._represent_encryption(download_version.server_side_encryption)
         )
         self._print_file_attribute(
             'Retention', self._represent_retention(download_version.file_retention)
         )
         self._print_file_attribute(
             'Legal hold', self._represent_legal_hold(download_version.legal_hold)
         )
         for label, attr_name in [
+            ('CacheControl', 'cache_control'),
+            ('Expires', 'expires'),
             ('ContentDisposition', 'content_disposition'),
             ('ContentLanguage', 'content_language'),
             ('ContentEncoding', 'content_encoding'),
         ]:
             attr_value = getattr(download_version, attr_name)
             if attr_value is not None:
                 self._print_file_attribute(label, attr_value)
         for name in sorted(download_version.file_info):
-            self._print_file_attribute('INFO %s' % (name,), download_version.file_info[name])
+            self._print_file_attribute(f'INFO {name}', download_version.file_info[name])
         if download_version.content_sha1 != 'none':
             self._print('Checksum matches')
         return 0
 
     @classmethod
     def _represent_encryption(cls, encryption: EncryptionSetting):
         # TODO: refactor to use "match" syntax after dropping python 3.9 support
         if encryption.mode is EncryptionMode.NONE:
             return 'none'
-        result = 'mode=%s, algorithm=%s' % (encryption.mode.value, encryption.algorithm.value)
+        result = f'mode={encryption.mode.value}, algorithm={encryption.algorithm.value}'
         if encryption.mode is EncryptionMode.SSE_B2:
             pass
         elif encryption.mode is EncryptionMode.SSE_C:
             if encryption.key.key_id is not None:
-                result += ', key_id=%s' % (encryption.key.key_id,)
+                result += f', key_id={encryption.key.key_id}'
         else:
-            raise ValueError('Unsupported encryption mode: %s' % (encryption.mode,))
+            raise ValueError(f'Unsupported encryption mode: {encryption.mode}')
 
         return result
 
     @classmethod
     def _represent_retention(cls, retention: FileRetentionSetting):
         if retention.mode is RetentionMode.NONE:
             return 'none'
         if retention.mode is RetentionMode.UNKNOWN:
             return '<unauthorized to read>'
         if retention.mode in (RetentionMode.COMPLIANCE, RetentionMode.GOVERNANCE):
-            return 'mode=%s, retainUntil=%s' % (
+            return 'mode={}, retainUntil={}'.format(
                 retention.mode.value,
-                datetime.datetime.
-                fromtimestamp(retention.retain_until / 1000, datetime.timezone.utc)
+                datetime.datetime.fromtimestamp(
+                    retention.retain_until / 1000, datetime.timezone.utc
+                )
             )
-        raise ValueError('Unsupported retention mode: %s' % (retention.mode,))
+        raise ValueError(f'Unsupported retention mode: {retention.mode}')
 
     @classmethod
     def _represent_legal_hold(cls, legal_hold: LegalHold):
         if legal_hold in (LegalHold.ON, LegalHold.OFF):
             return legal_hold.value
         if legal_hold is LegalHold.UNKNOWN:
             return '<unauthorized to read>'
         if legal_hold is LegalHold.UNSET:
             return '<unset>'
-        raise ValueError('Unsupported legal hold: %s' % (legal_hold,))
+        raise ValueError(f'Unsupported legal hold: {legal_hold}')
 
     def _print_file_attribute(self, label, value):
         self._print((label + ':').ljust(20) + ' ' + value)
 
+    def get_local_output_filepath(
+        self, filename: str, file_request: DownloadedFile
+    ) -> pathlib.Path:
+        if filename == '-':
+            return STDOUT_FILEPATH
+
+        output_filepath = pathlib.Path(filename)
+
+        # As longs as it's not a directory, we're overwriting everything.
+        if not output_filepath.is_dir():
+            return output_filepath
+
+        # If the output is directory, we're expected to download the file right there.
+        # Normally, we overwrite the target without asking any questions, but in this case
+        # user might be oblivious of the actual mistake he's about to commit.
+        # If he, e.g.: downloads file by ID, he might not know the name of the file
+        # and actually overwrite something unintended.
+        output_directory = output_filepath
+        output_filepath = output_directory / file_request.download_version.file_name
+        # If it doesn't exist, we stop worrying.
+        if not output_filepath.exists():
+            return output_filepath
+
+        # If it does exist, we make a unique file prefixed with the actual file name.
+        file_name_as_path = pathlib.Path(file_request.download_version.file_name)
+        file_name = file_name_as_path.stem
+        file_extension = file_name_as_path.suffix
+
+        # Default permissions are: readable and writable by this user only, executable by noone.
+        # This "temporary" file is not automatically removed, but still created in the safest way possible.
+        fd_handle, output_filepath_str = tempfile.mkstemp(
+            prefix=file_name,
+            suffix=file_extension,
+            dir=output_directory,
+        )
+        # Close the handle, so the file is not locked.
+        # This file is no longer 100% "safe", but that's acceptable.
+        os.close(fd_handle)
+
+        # "Normal" file created by Python has readable for everyone, writable for user only.
+        # We change the permissions, to match the default ones.
+        os.chmod(output_filepath_str, 0o644)
+
+        return pathlib.Path(output_filepath_str)
+
 
-@B2.register_subcommand
-class DownloadFileById(
-    SourceSseMixin, WriteBufferSizeMixin, SkipHashVerificationMixin, MaxDownloadStreamsMixin,
-    DownloadCommand
+class FileDownloadBase(
+    ThreadsMixin,
+    MaxDownloadStreamsMixin,
+    DownloadCommand,
 ):
     """
-    Downloads the given file, and stores it in the given local file.
+    Download the given file-like object, and store it in the given local file.
 
-    If the ``tqdm`` library is installed, progress bar is displayed
-    on stderr.  Without it, simple text progress is printed.
-    Use ``--noProgress`` to disable progress reporting.
-
-    {SOURCESSEMIXIN}
-    {WRITEBUFFERSIZEMIXIN}
-    {SKIPHASHVERIFICATIONMIXIN}
-    {MAXDOWNLOADSTREAMSMIXIN}
+    {ProgressMixin}
+    {ThreadsMixin}
+    {SourceSseMixin}
+    {WriteBufferSizeMixin}
+    {SkipHashVerificationMixin}
+    {MaxDownloadStreamsMixin}
 
     Requires capability:
 
     - **readFiles**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--noProgress', action='store_true')
-        parser.add_argument('--threads', type=int, default=10)
-        parser.add_argument('fileId')
-        parser.add_argument('localFileName')
         super()._setup_parser(parser)
+        parser.add_argument('localFileName')
 
-    def run(self, args):
-        progress_listener = make_progress_listener(args.localFileName, args.noProgress)
+    def _run(self, args):
+        progress_listener = self.make_progress_listener(
+            args.localFileName, args.no_progress or args.quiet
+        )
         encryption_setting = self._get_source_sse_setting(args)
-        if args.threads:
-            # FIXME: This is using deprecated API. It should be be replaced when moving to b2sdk apiver 3.
-            #        There is `max_download_workers` param in B2Api constructor for this.
-            self.api.services.download_manager.set_thread_pool_size(args.threads)
-        downloaded_file = self.api.download_file_by_id(
-            args.fileId, progress_listener, encryption=encryption_setting
+        self._set_threads_from_args(args)
+
+        b2_uri = self.get_b2_uri_from_arg(args)
+        downloaded_file = self.api.download_file_by_uri(
+            b2_uri, progress_listener, encryption=encryption_setting
         )
-        self._print_download_info(downloaded_file)
-        downloaded_file.save_to(args.localFileName)
+
+        output_filepath = self.get_local_output_filepath(args.localFileName, downloaded_file)
+        self._print_download_info(downloaded_file, output_filepath)
+        progress_listener.change_description(output_filepath.name)
+
+        downloaded_file.save_to(output_filepath)
         self._print('Download finished')
+
         return 0
 
 
-@B2.register_subcommand
-class DownloadFileByName(
-    SourceSseMixin,
-    WriteBufferSizeMixin,
-    SkipHashVerificationMixin,
-    MaxDownloadStreamsMixin,
-    DownloadCommand,
-):
+class FileCatBase(B2URIFileArgMixin, DownloadCommand):
     """
-    Downloads the given file, and stores it in the given local file.
+    Download content of a file-like object identified by B2 URI directly to stdout.
 
-    If the ``tqdm`` library is installed, progress bar is displayed
-    on stderr.  Without it, simple text progress is printed.
-    Use ``--noProgress`` to disable progress reporting.
-
-    {SOURCESSEMIXIN}
-    {WRITEBUFFERSIZEMIXIN}
-    {SKIPHASHVERIFICATIONMIXIN}
-    {MAXDOWNLOADSTREAMSMIXIN}
+    {ProgressMixin}
+    {SourceSseMixin}
+    {WriteBufferSizeMixin}
+    {SkipHashVerificationMixin}
 
     Requires capability:
 
     - **readFiles**
     """
 
-    @classmethod
-    def _setup_parser(cls, parser):
-        parser.add_argument('--noProgress', action='store_true')
-        parser.add_argument('--threads', type=int, default=10)
-        parser.add_argument('bucketName').completer = bucket_name_completer
-        parser.add_argument('b2FileName').completer = file_name_completer
-        parser.add_argument('localFileName')
-        super()._setup_parser(parser)
-
-    def run(self, args):
-        if args.threads:
-            # FIXME: This is using deprecated API. It should be be replaced when moving to b2sdk apiver 3.
-            #        There is `max_download_workers` param in B2Api constructor for this.
-            self.api.services.download_manager.set_thread_pool_size(args.threads)
-        bucket = self.api.get_bucket_by_name(args.bucketName)
-        progress_listener = make_progress_listener(args.localFileName, args.noProgress)
+    def _run(self, args):
+        target_filename = '-'
+        progress_listener = self.make_progress_listener(
+            target_filename, args.no_progress or args.quiet
+        )
         encryption_setting = self._get_source_sse_setting(args)
-        downloaded_file = bucket.download_file_by_name(
-            args.b2FileName, progress_listener, encryption=encryption_setting
+        file_request = self.api.download_file_by_uri(
+            args.B2_URI, progress_listener=progress_listener, encryption=encryption_setting
         )
-        self._print_download_info(downloaded_file)
-        downloaded_file.save_to(args.localFileName)
-        self._print('Download finished')
+        output_filepath = self.get_local_output_filepath(target_filename, file_request)
+        file_request.save_to(output_filepath)
         return 0
 
 
-@B2.register_subcommand
-class GetAccountInfo(Command):
+class AccountGetBase(Command):
     """
-    Shows the account ID, key, auth token, URLs, and what capabilities
+    Show current account info
+
+    Prints account ID, key, auth token, URLs, and what capabilities
     the current application keys has.
     """
 
-    def run(self, args):
-        account_info = self.api.account_info
-        data = dict(
-            accountId=account_info.get_account_id(),
-            accountFilePath=getattr(
-                account_info,
-                'filename',
-                None,
-            ),  # missing in StubAccountInfo in tests
-            allowed=account_info.get_allowed(),
-            applicationKeyId=account_info.get_application_key_id(),
-            applicationKey=account_info.get_application_key(),
-            isMasterKey=account_info.is_master_key(),
-            accountAuthToken=account_info.get_account_auth_token(),
-            apiUrl=account_info.get_api_url(),
-            downloadUrl=account_info.get_download_url(),
-        )
+    def _run(self, args):
+        data = format_account_info(self.api.account_info)
         self._print_json(data)
         return 0
 
 
-@B2.register_subcommand
-class GetBucket(Command):
+class BucketGetBase(Command):
     """
+    Display bucket info
+
     Prints all of the information about the bucket, including
     bucket info, CORS rules and lifecycle rules.
 
-    If ``--showSize`` is specified, then display the number of files
+    If ``--show-size`` is specified, then display the number of files
     (``fileCount``) in the bucket and the aggregate size of all files
     (``totalSize``). Hidden files and hide markers are accounted for
     in the reported number of files, and hidden files also
     contribute toward the reported aggregate size, whereas hide
     markers do not. Each version of a file counts as an individual
     file, and its size contributes toward the aggregate size.
     Analysis is recursive.
 
     .. note::
 
-        Note that ``--showSize`` requires multiple
+        Note that ``--show-size`` requires multiple
         API calls, and will therefore incur additional latency,
         computation, and Class C transactions.
 
     Requires capability:
 
     - **listBuckets**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--showSize', action='store_true')
-        parser.add_argument('bucketName').completer = bucket_name_completer
+        add_normalized_argument(parser, '--show-size', action='store_true')
+        add_bucket_name_argument(parser)
+        super()._setup_parser(parser)
 
-    def run(self, args):
+    def _run(self, args):
         # This always wants up-to-date info, so it does not use
         # the bucket cache.
         for b in self.api.list_buckets(args.bucketName):
-            if not args.showSize:
+            if not args.show_size:
                 self._print_json(b)
                 return 0
             else:
                 result = b.as_dict()
                 # `files` is a generator. We don't want to collect all of the values from the
                 # generator, as there many be billions of files in a large bucket.
                 files = b.ls("", latest_only=False, recursive=True)
@@ -1449,37 +2056,36 @@
                 result['totalSize'] = count_size_tuple[1]
                 self._print_json(result)
                 return 0
         self._print_stderr('bucket not found: ' + args.bucketName)
         return 1
 
 
-@B2.register_subcommand
-class GetFileInfo(Command):
+class FileInfoBase(Command):
     """
-    Prints all of the information about the file, but not its contents.
+    Print file info
+
+    Prints all of the information about the object, but not its contents.
 
     Requires capability:
 
     - **readFiles**
     """
 
-    @classmethod
-    def _setup_parser(cls, parser):
-        parser.add_argument('fileId')
-
-    def run(self, args):
-        file_version = self.api.get_file_info(args.fileId)
+    def _run(self, args):
+        b2_uri = self.get_b2_uri_from_arg(args)
+        file_version = self.api.get_file_info_by_uri(b2_uri)
         self._print_json(file_version)
         return 0
 
 
-@B2.register_subcommand
-class GetDownloadAuth(Command):
+class BucketGetDownloadAuthBase(Command):
     """
+    Display authorization token for downloading files
+
     Prints an authorization token that is valid only for downloading
     files from the given bucket.
 
     The token is valid for the duration specified, which defaults
     to 86400 seconds (one day).
 
     Only files that match that given prefix can be downloaded with
@@ -1491,29 +2097,31 @@
     - **shareFiles**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         parser.add_argument('--prefix', default='')
         parser.add_argument('--duration', type=int, default=86400)
-        parser.add_argument('bucketName').completer = bucket_name_completer
+        add_bucket_name_argument(parser)
+        super()._setup_parser(parser)
 
-    def run(self, args):
+    def _run(self, args):
         bucket = self.api.get_bucket_by_name(args.bucketName)
         auth_token = bucket.get_download_authorization(
             file_name_prefix=args.prefix, valid_duration_in_seconds=args.duration
         )
         self._print(auth_token)
         return 0
 
 
-@B2.register_subcommand
-class GetDownloadUrlWithAuth(Command):
+class GetDownloadUrlWithAuthBase(Command):
     """
-    Prints a URL to download the given file.  The URL includes an authorization
+    Print a URL to download the given file.
+
+    The URL includes an authorization
     token that allows downloads from the given bucket for files whose names
     start with the given file name.
 
     The URL will work for the given file, but is not specific to that file.  Files
     with longer names that start with the give file name can also be downloaded
     with the same auth token.
 
@@ -1524,54 +2132,54 @@
 
     - **shareFiles**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         parser.add_argument('--duration', type=int, default=86400)
-        parser.add_argument('bucketName').completer = bucket_name_completer
+        add_bucket_name_argument(parser)
         parser.add_argument('fileName').completer = file_name_completer
+        super()._setup_parser(parser)
 
-    def run(self, args):
+    def _run(self, args):
         bucket = self.api.get_bucket_by_name(args.bucketName)
         auth_token = bucket.get_download_authorization(
             file_name_prefix=args.fileName, valid_duration_in_seconds=args.duration
         )
         base_url = self.api.get_download_url_for_file_name(args.bucketName, args.fileName)
         url = base_url + '?Authorization=' + auth_token
         self._print(url)
         return 0
 
 
-@B2.register_subcommand
-class HideFile(Command):
+class FileHideBase(Command):
     """
-    Uploads a new, hidden, version of the given file.
+    Upload a new, hidden, version of the given file.
 
     Requires capability:
 
     - **writeFiles**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('bucketName').completer = bucket_name_completer
+        add_bucket_name_argument(parser)
         parser.add_argument('fileName').completer = file_name_completer
+        super()._setup_parser(parser)
 
-    def run(self, args):
+    def _run(self, args):
         bucket = self.api.get_bucket_by_name(args.bucketName)
         file_info = bucket.hide_file(args.fileName)
         self._print_json(file_info)
         return 0
 
 
-@B2.register_subcommand
-class ListBuckets(Command):
+class BucketListBase(Command):
     """
-    Lists all of the buckets in the current account.
+    List all of the buckets in the current account.
 
     Output lines list the bucket ID, bucket type, and bucket name,
     and look like this:
 
     .. code-block::
 
         98c960fd1cb4390c5e0f0519  allPublic   my-bucket
@@ -1583,30 +2191,34 @@
 
     - **listBuckets**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         parser.add_argument('--json', action='store_true')
+        super()._setup_parser(parser)
 
-    def run(self, args):
-        buckets = self.api.list_buckets()
-        if args.json:
-            self._print_json(list(buckets))
+    def _run(self, args):
+        return self.__class__.run_list_buckets(self, json_=args.json)
+
+    @classmethod
+    def run_list_buckets(cls, command: Command, *, json_: bool) -> int:
+        buckets = command.api.list_buckets()
+        if json_:
+            command._print_json(list(buckets))
             return 0
 
         for b in buckets:
-            self._print('%s  %-10s  %s' % (b.id_, b.type_, b.name))
+            command._print(f'{b.id_}  {b.type_:<10}  {b.name}')
         return 0
 
 
-@B2.register_subcommand
-class ListKeys(Command):
+class KeyListBase(Command):
     """
-    Lists the application keys for the current account.
+    List the application keys for the current account.
 
     The columns in the output are:
 
     - ID of the application key
     - Name of the application key
     - Name of the bucket the key is restricted to, or ``-`` for no restriction
     - Date of expiration, or ``-``
@@ -1624,20 +2236,21 @@
 
     - **listKeys**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         parser.add_argument('--long', action='store_true')
+        super()._setup_parser(parser)
 
     def __init__(self, console_tool):
-        super(ListKeys, self).__init__(console_tool)
+        super().__init__(console_tool)
         self.bucket_id_to_bucket_name = None
 
-    def run(self, args):
+    def _run(self, args):
         for key in self.api.list_keys():
             self.print_key(key, args.long)
 
         return 0
 
     def print_key(self, key: ApplicationKey, is_long_format: bool):
         if is_long_format:
@@ -1672,128 +2285,130 @@
         """
         Returns a pair (date_str, time_str) for the given timestamp
         """
         if timestamp_or_none is None:
             return '-', '-'
         else:
             timestamp = timestamp_or_none
-            dt = datetime.datetime.utcfromtimestamp(timestamp / 1000)
+            dt = datetime.datetime.fromtimestamp(timestamp / 1000, datetime.timezone.utc)
             return dt.strftime('%Y-%m-%d'), dt.strftime('%H:%M:%S')
 
 
-@B2.register_subcommand
-class ListParts(Command):
+class FileLargePartsBase(Command):
     """
     Lists all of the parts that have been uploaded for the given
     large file, which must be a file that was started but not
     finished or canceled.
 
     Requires capability:
 
     - **writeFiles**
     """
 
-    @classmethod
-    def _setup_parser(cls, parser):
-        parser.add_argument('largeFileId')
-
-    def run(self, args):
-        for part in self.api.list_parts(args.largeFileId):
+    def _run(self, args):
+        b2_uri = self.get_b2_uri_from_arg(args)
+        for part in self.api.list_parts(b2_uri.file_id):
             self._print('%5d  %9d  %s' % (part.part_number, part.content_length, part.content_sha1))
         return 0
 
 
-@B2.register_subcommand
-class ListUnfinishedLargeFiles(Command):
+class FileLargeUnfinishedListBase(Command):
     """
     Lists all of the large files in the bucket that were started,
     but not finished or canceled.
 
     Requires capability:
 
     - **listFiles**
     """
 
-    @classmethod
-    def _setup_parser(cls, parser):
-        parser.add_argument('bucketName').completer = bucket_name_completer
-
-    def run(self, args):
-        bucket = self.api.get_bucket_by_name(args.bucketName)
+    def _run(self, args):
+        b2_uri = self.get_b2_uri_from_arg(args)
+        bucket = self.api.get_bucket_by_name(b2_uri.bucket_name)
         for unfinished in bucket.list_unfinished_large_files():
             file_info_text = ' '.join(
-                '%s=%s' % (k, unfinished.file_info[k]) for k in sorted(unfinished.file_info)
+                f'{k}={unfinished.file_info[k]}' for k in sorted(unfinished.file_info)
             )
             self._print(
-                '%s %s %s %s' %
-                (unfinished.file_id, unfinished.file_name, unfinished.content_type, file_info_text)
+                f'{unfinished.file_id} {unfinished.file_name} {unfinished.content_type} {file_info_text}'
             )
         return 0
 
 
 class AbstractLsCommand(Command, metaclass=ABCMeta):
     """
     The ``--versions`` option selects all versions of each file, not
     just the most recent.
 
     The ``--recursive`` option will descend into folders, and will select
     only files, not folders.
 
-    The ``--withWildcard`` option will allow using ``*``, ``?`` and ```[]```
+    The ``--with-wildcard`` option will allow using ``*``, ``?`` and ```[]```
     characters in ``folderName`` as a greedy wildcard, single character
     wildcard and range of characters. It requires the ``--recursive`` option.
     Remember to quote ``folderName`` to avoid shell expansion.
+
+    The --include and --exclude flags can be used to filter the files returned
+    from the server using wildcards. You can specify multiple --include and --exclude filters.
+    The order of filters matters. The *last* matching filter decides whether a file
+    is included or excluded. If the given list of filters contains only INCLUDE filters,
+    then it is assumed that all files are excluded by default.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         parser.add_argument('--versions', action='store_true')
-        parser.add_argument('--recursive', action='store_true')
-        parser.add_argument('--withWildcard', action='store_true')
-        parser.add_argument('bucketName').completer = bucket_name_completer
-        parser.add_argument('folderName', nargs='?').completer = file_name_completer
+        parser.add_argument('-r', '--recursive', action='store_true')
+        add_normalized_argument(parser, '--with-wildcard', action='store_true')
+        parser.add_argument(
+            '--include', dest='filters', action='append', type=Filter.include, default=[]
+        )
+        parser.add_argument(
+            '--exclude', dest='filters', action='append', type=Filter.exclude, default=[]
+        )
+        super()._setup_parser(parser)
 
-    def run(self, args):
-        generator = self._get_ls_generator(args)
+    def _print_files(self, args, b2_uri: B2URI | None = None):
+        generator = self._get_ls_generator(args, b2_uri=b2_uri)
 
         for file_version, folder_name in generator:
             self._print_file_version(args, file_version, folder_name)
 
-        return 0
-
     def _print_file_version(
         self,
         args,
         file_version: FileVersion,
-        folder_name: Optional[str],
+        folder_name: str | None,
     ) -> None:
-        self._print(folder_name or file_version.file_name)
-
-    def _get_ls_generator(self, args):
-        start_file_name = args.folderName or ''
-
-        bucket = self.api.get_bucket_by_name(args.bucketName)
+        name = folder_name or file_version.file_name
+        if args.escape_control_characters:
+            name = escape_control_chars(name)
+        self._print(name)
 
+    def _get_ls_generator(self, args, b2_uri: B2URI | None = None):
+        b2_uri = b2_uri or self.get_b2_uri_from_arg(args)
         try:
-            for entry in bucket.ls(
-                start_file_name,
+            yield from self.api.list_file_versions_by_uri(
+                b2_uri,
                 latest_only=not args.versions,
                 recursive=args.recursive,
-                with_wildcard=args.withWildcard,
-            ):
-                yield entry
-        except ValueError as error:
-            # Wrap these errors into B2Error. At the time of writing there's
-            # exactly one – `with_wildcard` being passed without `recursive` option.
-            raise B2Error(error.args[0])
+                with_wildcard=args.with_wildcard,
+                filters=args.filters,
+            )
+        except Exception as err:
+            raise CommandError(unprintable_to_hex(str(err))) from err
+
+    def get_b2_uri_from_arg(self, args: argparse.Namespace) -> B2URI:
+        raise NotImplementedError
 
 
-@B2.register_subcommand
-class Ls(AbstractLsCommand):
+class BaseLs(AbstractLsCommand, metaclass=ABCMeta):
     """
+    List files in a given folder.
+
     Using the file naming convention that ``/`` separates folder
     names from their contents, returns a list of the files
     and folders in a given folder.  If no folder name is given,
     lists all files at the top level.
 
     The ``--long`` option produces very wide multi-column output
     showing the upload date/time, file size, file id, whether it
@@ -1802,297 +2417,299 @@
     shown with ``-`` in each of the fields other than the name.
 
     The ``--json`` option produces machine-readable output similar to
     the server api response format.
 
     The ``--replication`` option adds replication status
 
-    {ABSTRACTLSCOMMAND}
-
-    Examples
-
-    .. note::
-
-        Note the use of quotes, to ensure that special
-        characters are not expanded by the shell.
-
-
-    List csv and tsv files (in any directory, in the whole bucket):
-
-    .. code-block::
-
-        {NAME} ls --recursive --withWildcard bucketName "*.[ct]sv"
-
-
-    List all info.txt files from buckets bX, where X is any character:
-
-    .. code-block::
-
-        {NAME} ls --recursive --withWildcard bucketName "b?/info.txt"
-
-
-    List all pdf files from buckets b0 to b9 (including sub-directories):
-
-    .. code-block::
-
-        {NAME} ls --recursive --withWildcard bucketName "b[0-9]/*.pdf"
-
-
-    Requires capability:
-
-    - **listFiles**
+    {AbstractLsCommand}
     """
 
     # order is file_id, action, date, time, size(, replication), name
     LS_ENTRY_TEMPLATE = '%83s  %6s  %10s  %8s  %9d  %s'
     LS_ENTRY_TEMPLATE_REPLICATION = LS_ENTRY_TEMPLATE + '  %s'
 
     @classmethod
     def _setup_parser(cls, parser):
         parser.add_argument('--long', action='store_true')
         parser.add_argument('--json', action='store_true')
         parser.add_argument('--replication', action='store_true')
         super()._setup_parser(parser)
 
-    def run(self, args):
-        if args.json:
-            # TODO: Make this work for an infinite generation.
-            #   Use `_print_file_version` to print a single `file_version` and manage the external JSON list
-            #   e.g. manually. However, to do it right, some sort of state needs to be kept e.g. info whether
-            #   at least one element was written to the stream, so we can add a `,` on the start of another.
-            #   That would sadly lead to an ugly formatting, so `_print` needs to be expanded with an ability
-            #   to not print end-line character(s).
-            self._print_json([file_version for file_version, _ in self._get_ls_generator(args)])
-            return 0
+    def _run(self, args):
+        b2_uri = self.get_b2_uri_from_arg(args)
+        if args.long and args.json:
+            raise CommandError('Cannot use --long and --json options together')
+
+        if not b2_uri or b2_uri == B2URI(""):
+            for option_name in ('long', 'recursive', 'replication'):
+                if getattr(args, option_name, False):
+                    raise CommandError(
+                        f'Cannot use --{option_name} option without specifying a bucket name'
+                    )
+            return ListBuckets.run_list_buckets(self, json_=args.json)
 
-        return super().run(args)
+        if args.json:
+            i = -1
+            for i, (file_version, _) in enumerate(self._get_ls_generator(args, b2_uri=b2_uri)):
+                if i:
+                    self._print(',', end='')
+                else:
+                    self._print('[')
+                self._print_json(file_version)
+            self._print(']' if i >= 0 else '[]')
+        else:
+            self._print_files(args)
+        return 0
 
     def _print_file_version(
         self,
         args,
         file_version: FileVersion,
-        folder_name: Optional[str],
+        folder_name: str | None,
     ) -> None:
         if not args.long:
             super()._print_file_version(args, file_version, folder_name)
         elif folder_name is not None:
-            self._print(self.format_folder_ls_entry(folder_name, args.replication))
+            self._print(self.format_folder_ls_entry(args, folder_name, args.replication))
         else:
-            self._print(self.format_ls_entry(file_version, args.replication))
+            self._print(self.format_ls_entry(args, file_version, args.replication))
 
-    def format_folder_ls_entry(self, name, replication: bool):
+    def format_folder_ls_entry(self, args, name, replication: bool):
+        if args.escape_control_characters:
+            name = escape_control_chars(name)
         if replication:
             return self.LS_ENTRY_TEMPLATE_REPLICATION % ('-', '-', '-', '-', 0, '-', name)
         return self.LS_ENTRY_TEMPLATE % ('-', '-', '-', '-', 0, name)
 
-    def format_ls_entry(self, file_version: FileVersion, replication: bool):
-        dt = datetime.datetime.utcfromtimestamp(file_version.upload_timestamp / 1000)
+    def format_ls_entry(self, args, file_version: FileVersion, replication: bool):
+        dt = datetime.datetime.fromtimestamp(
+            file_version.upload_timestamp / 1000, datetime.timezone.utc
+        )
         date_str = dt.strftime('%Y-%m-%d')
         time_str = dt.strftime('%H:%M:%S')
         size = file_version.size or 0  # required if self.action == 'hide'
         template = replication and self.LS_ENTRY_TEMPLATE_REPLICATION or self.LS_ENTRY_TEMPLATE
         parameters = [
             file_version.id_,
             file_version.action,
             date_str,
             time_str,
             size,
         ]
         if replication:
             replication_status = file_version.replication_status
             parameters.append(replication_status.value if replication_status else '-')
-        parameters.append(file_version.file_name)
+        name = file_version.file_name
+        if args.escape_control_characters:
+            name = escape_control_chars(name)
+        parameters.append(name)
         return template % tuple(parameters)
 
 
-@B2.register_subcommand
-class Rm(AbstractLsCommand):
+class Ls(B2IDOrB2URIMixin, BaseLs):
     """
-    Removes a "folder" or a set of files matching a pattern.  Use with caution.
+    {BaseLs}
+
+    Examples
 
     .. note::
 
-        ``rm`` is a high-level command that under the hood utilizes multiple calls to the server,
-        which means the server cannot guarantee consistency between multiple operations. For
-        example if a file matching a pattern is uploaded during a run of ``rm`` command, it MIGHT
-        be deleted (as "latest") instead of the one present when the ``rm`` run has started.
+        Note the use of quotes, to ensure that special
+        characters are not expanded by the shell.
 
-    In order to safely delete a single file version, please use ``delete-file-version``.
 
-    To list (but not remove) files to be deleted, use ``--dryRun``.  You can also
-    list files via ``ls`` command - the listing behaviour is exactly the same.
+    List csv and tsv files (in any directory, in the whole bucket):
+
+    .. code-block::
 
-    Users with multiple files to be removed will benefit from multi-threaded
-    capabilities.  The default number of threads is 10.
+        {NAME} ls --recursive --with-wildcard "b2://bucketName/*.[ct]sv"
 
-    Progress is displayed on the console unless ``--noProgress`` is specified.
 
-    {ABSTRACTLSCOMMAND}
+    List all info.txt files from directories named `b?`, where `?` is any character:
 
-    The ``--dryRun`` option prints all the files that would be affected by
-    the command, but removes nothing.
+    .. code-block::
 
-    Normally, when an error happens during file removal, log is printed and the command
-    goes further. If any error should be immediately breaking the command,
-    ``--failFast`` can be passed to ensure that first error will stop the execution.
-    This could be useful to e.g. check whether provided credentials have **deleteFiles**
-    capabilities.
+        {NAME} ls --recursive --with-wildcard "b2://bucketName/b?/info.txt"
 
-    .. note::
 
-        Using ``--failFast`` doesn't prevent the command from trying to remove further files.
-        It just stops the progress. Since multiple files are removed in parallel, it's possible
-        that just some of them were not reported.
+    List all pdf files from directories b0 to b9 (including sub-directories):
 
-    Command returns 0 if all files were removed successfully and
-    a value different from 0 if any file was left.
+    .. code-block::
 
-    Examples.
+        {NAME} ls --recursive --with-wildcard "b2://bucketName/b[0-9]/*.pdf"
 
-    .. note::
 
-        Note the use of quotes, to ensure that special
-        characters are not expanded by the shell.
+    List all buckets:
 
+    .. code-block::
 
-    .. note::
+        {NAME} ls
 
-        Use with caution. Running examples presented below can cause data-loss.
 
+    Requires capability:
 
-    Remove all csv and tsv files (in any directory, in the whole bucket):
+    - **listFiles**
+    - **listBuckets** (if bucket name is not provided)
+    """
+    ALLOW_ALL_BUCKETS = True
 
-    .. code-block::
 
-        {NAME} rm --recursive --withWildcard bucketName "*.[ct]sv"
+class BaseRm(ThreadsMixin, AbstractLsCommand, metaclass=ABCMeta):
+    """
+    Remove a "folder" or a set of files matching a pattern.
 
+    Use with caution!
 
-    Remove all info.txt files from buckets bX, where X is any character:
+    .. note::
 
-    .. code-block::
+        ``rm`` is a high-level command that under the hood utilizes multiple calls to the server,
+        which means the server cannot guarantee consistency between multiple operations. For
+        example if a file matching a pattern is uploaded during a run of ``rm`` command, it MIGHT
+        be deleted (as "latest") instead of the one present when the ``rm`` run has started.
 
-        {NAME} rm --recursive --withWildcard bucketName "b?/info.txt"
+    If a file is in governance retention mode, and the retention period has not expired,
+    adding --bypass-governance is required.
 
+    To list (but not remove) files to be deleted, use ``--dry-run``.  You can also
+    list files via ``ls`` command - the listing behaviour is exactly the same.
 
-    Remove all pdf files from buckets b0 to b9 (including sub-directories):
+    Progress is displayed on the console unless ``--no-progress`` is specified.
+    {ThreadsMixin}
+    {AbstractLsCommand}
 
-    .. code-block::
+    The ``--dry-run`` option prints all the files that would be affected by
+    the command, but removes nothing.
 
-        {NAME} rm --recursive --withWildcard bucketName "b[0-9]/*.pdf"
+    Normally, when an error happens during file removal, log is printed and the command
+    goes further. If any error should be immediately breaking the command,
+    ``--fail-fast`` can be passed to ensure that first error will stop the execution.
+    This could be useful to e.g. check whether provided credentials have **deleteFiles**
+    capabilities.
 
+    .. note::
 
-    Requires capability:
+        Using ``--fail-fast`` doesn't prevent the command from trying to remove further files.
+        It just stops the progress. Since multiple files are removed in parallel, it's possible
+        that just some of them were not reported.
 
-    - **listFiles**
-    - **deleteFiles**
+    Command returns 0 if all files were removed successfully and
+    a value different from 0 if any file was left.
     """
 
-    DEFAULT_THREADS = 10
     PROGRESS_REPORT_CLASS = ProgressReport
 
     class SubmitThread(threading.Thread):
         END_MARKER = object()
         ERROR_TAG = 'error'
         EXCEPTION_TAG = 'general_exception'
 
         def __init__(
             self,
-            runner: 'Rm',
+            runner: BaseRm,
             args: argparse.Namespace,
             messages_queue: queue.Queue,
             reporter: ProgressReport,
+            threads: int,
         ):
             self.runner = runner
             self.args = args
             self.messages_queue = messages_queue
             self.reporter = reporter
-            removal_queue_size = self.args.queueSize or (2 * self.args.threads)
+            self.threads = threads
+            removal_queue_size = self.args.queue_size or (2 * self.threads)
             self.semaphore = threading.BoundedSemaphore(value=removal_queue_size)
             self.fail_fast_event = threading.Event()
             self.mapping_lock = threading.Lock()
             self.futures_mapping = {}
             super().__init__(daemon=True)
 
         def run(self) -> None:
             try:
-                with ThreadPoolExecutor(max_workers=self.args.threads) as executor:
+                with ThreadPoolExecutor(max_workers=self.threads) as executor:
                     self._run_removal(executor)
             except Exception as error:
                 self.messages_queue.put((self.EXCEPTION_TAG, error))
             finally:
                 self.messages_queue.put(self.END_MARKER)
 
         def _run_removal(self, executor: Executor):
-            for file_version, _ in self.runner._get_ls_generator(self.args):
+            for file_version, subdirectory in self.runner._get_ls_generator(self.args):
+                if subdirectory is not None:
+                    # This file_version is not for listing/deleting.
+                    # It is only here to list the subdirectory, so skip deleting it.
+                    continue
                 # Obtaining semaphore limits number of elements that we fetch from LS.
                 self.semaphore.acquire(blocking=True)
                 # This event is updated before the semaphore is released. This way,
                 # in a single threaded scenario, we get synchronous responses.
                 if self.fail_fast_event.is_set():
                     break
 
+                self.reporter.update_total(1)
                 future = executor.submit(
                     self.runner.api.delete_file_version,
                     file_version.id_,
                     file_version.file_name,
+                    self.args.bypass_governance,
                 )
                 with self.mapping_lock:
                     self.futures_mapping[future] = file_version
                 # Done callback is added after, so it's "sure" that mapping is updated earlier.
                 future.add_done_callback(self._removal_done)
 
-                self.reporter.update_total(1)
             self.reporter.end_total()
 
         def _removal_done(self, future: Future) -> None:
             with self.mapping_lock:
                 file_version = self.futures_mapping.pop(future)
 
             try:
                 future.result()
+                self.reporter.update_count(1)
             except FileNotPresent:
                 # We wanted to remove this file anyway.
-                pass
+                self.reporter.update_count(1)
             except B2Error as error:
-                if self.args.failFast:
+                if self.args.fail_fast:
                     # This is set before releasing the semaphore.
                     # It means that when the semaphore is released,
                     # we'll already have information about requirement to fail.
                     self.fail_fast_event.set()
                 self.messages_queue.put((self.ERROR_TAG, file_version, error))
             except Exception as error:
                 self.messages_queue.put((self.EXCEPTION_TAG, error))
             finally:
-                self.reporter.update_count(1)
                 self.semaphore.release()
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--dryRun', action='store_true')
-        parser.add_argument('--threads', type=int, default=cls.DEFAULT_THREADS)
-        parser.add_argument(
-            '--queueSize',
+        add_normalized_argument(parser, '--bypass-governance', action='store_true', default=False)
+        add_normalized_argument(parser, '--dry-run', action='store_true')
+        add_normalized_argument(parser,
+            '--queue-size',
             type=int,
             default=None,
             help='max elements fetched at once for removal, ' \
                  'if left unset defaults to twice the number of threads.',
         )
-        parser.add_argument('--noProgress', action='store_true')
-        parser.add_argument('--failFast', action='store_true')
+        add_normalized_argument(parser, '--no-progress', action='store_true')
+        add_normalized_argument(parser, '--fail-fast', action='store_true')
         super()._setup_parser(parser)
 
-    def run(self, args):
-        if args.dryRun:
-            return super().run(args)
-
+    def _run(self, args):
+        if args.dry_run:
+            self._print_files(args)
+            return 0
         failed_on_any_file = False
         messages_queue = queue.Queue()
 
-        with self.PROGRESS_REPORT_CLASS(self.stdout, args.noProgress) as reporter:
-            submit_thread = self.SubmitThread(self, args, messages_queue, reporter)
+        threads = self._get_threads_from_args(args)
+        with self.PROGRESS_REPORT_CLASS(self.stdout, args.no_progress or args.quiet) as reporter:
+            submit_thread = self.SubmitThread(self, args, messages_queue, reporter, threads=threads)
             # This thread is started in daemon mode, no joining needed.
             submit_thread.start()
 
             while True:
                 queue_entry = messages_queue.get(block=True)
                 if queue_entry is submit_thread.END_MARKER:
                     break
@@ -2101,289 +2718,358 @@
                 if event_type == submit_thread.ERROR_TAG:
                     file_version, error = data
                     message = f'Deletion of file "{file_version.file_name}" ' \
                               f'({file_version.id_}) failed: {str(error)}'
                     reporter.print_completion(message)
 
                     failed_on_any_file = True
-                    if args.failFast:
+                    if args.fail_fast:
                         break
 
                 elif event_type == submit_thread.EXCEPTION_TAG:
                     raise data[0]
 
         return 1 if failed_on_any_file else 0
 
 
-@B2.register_subcommand
-class MakeUrl(Command):
-    """
-    Prints an URL that can be used to download the given file, if
-    it is public.
+class Rm(B2IDOrB2URIMixin, BaseRm):
     """
+    {BaseRm}
 
-    @classmethod
-    def _setup_parser(cls, parser):
-        parser.add_argument('fileId')
+    Examples.
 
-    def run(self, args):
-        self._print(self.api.get_download_url_for_fileid(args.fileId))
-        return 0
+        .. note::
+
+            Note the use of quotes, to ensure that special
+            characters are not expanded by the shell.
+
+
+        .. note::
+
+            Use with caution. Running examples presented below can cause data-loss.
+
+
+        Remove all csv and tsv files (in any directory, in the whole bucket):
+
+        .. code-block::
+
+            {NAME} rm --recursive --with-wildcard "b2://bucketName/*.[ct]sv"
+
+
+        Remove all info.txt files from buckets bX, where X is any character:
 
+        .. code-block::
 
-@B2.register_subcommand
-class MakeFriendlyUrl(Command):
+            {NAME} rm --recursive --with-wildcard "b2://bucketName/b?/info.txt"
+
+
+        Remove all pdf files from buckets b0 to b9 (including sub-directories):
+
+        .. code-block::
+
+            {NAME} rm --recursive --with-wildcard "b2://bucketName/b[0-9]/*.pdf"
+
+
+    Requires capability:
+
+    - **listFiles**
+    - **deleteFiles**
+    - **bypassGovernance** (if --bypass-governance is used)
     """
-    Prints a short URL that can be used to download the given file, if
+
+
+class FileUrlBase(Command):
+    """
+    Display download URL for a file
+
+    Prints an URL that can be used to download the given file, if
     it is public.
+
+    If it is private, you can use --with-auth to include an authorization
+    token in the URL that allows downloads from the given bucket for files
+    whose names start with the given file name.
+
+    The URL will work for the given file, but is not specific to that file.  Files
+    with longer names that start with the give file name can also be downloaded
+    with the same auth token.
+
+    The token is valid for the duration specified, which defaults
+    to 86400 seconds (one day).
+
+
+    Requires capability:
+
+    - **shareFiles** (if using --with-auth)
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('bucketName').completer = bucket_name_completer
-        parser.add_argument('fileName').completer = file_name_completer
+        add_normalized_argument(parser, '--with-auth', action='store_true')
+        parser.add_argument('--duration', type=int, default=86400)
+        super()._setup_parser(parser)
 
-    def run(self, args):
-        self._print(self.api.get_download_url_for_file_name(args.bucketName, args.fileName))
+    def _run(self, args):
+        b2_uri = self.get_b2_uri_from_arg(args)
+        url = self.api.get_download_url_by_uri(b2_uri)
+        if args.with_auth:
+            bucket = self.api.get_bucket_by_name(b2_uri.bucket_name)
+            auth_token = bucket.get_download_authorization(
+                file_name_prefix=b2_uri.path, valid_duration_in_seconds=args.duration
+            )
+            url += '?Authorization=' + auth_token
+        self._print(url)
         return 0
 
 
-@B2.register_subcommand
 class Sync(
+    ThreadsMixin,
     DestinationSseMixin,
     SourceSseMixin,
     WriteBufferSizeMixin,
     SkipHashVerificationMixin,
     MaxDownloadStreamsMixin,
     UploadModeMixin,
     Command,
 ):
     """
-    Copies multiple files from source to destination.  Optionally
-    deletes or hides destination files that the source does not have.
+    Copy multiple files from source to destination.
+
+    Optionally deletes or hides destination files that the source does not have.
 
     The synchronizer can copy files:
 
     - From a B2 bucket to a local destination.
     - From a local source to a B2 bucket.
     - From one B2 bucket to another.
     - Between different folders in the same B2 bucket.
 
     Use ``b2://<bucketName>/<prefix>`` for B2 paths, e.g. ``b2://my-bucket-name/a/path/prefix/``.
 
-    Progress is displayed on the console unless ``--noProgress`` is
+    Progress is displayed on the console unless ``--no-progress`` is
     specified.  A list of actions taken is always printed.
 
-    Specify ``--dryRun`` to simulate the actions that would be taken.
+    Specify ``--dry-run`` to simulate the actions that would be taken.
 
     To allow sync to run when the source directory is empty, potentially
-    deleting all files in a bucket, specify ``--allowEmptySource``.
+    deleting all files in a bucket, specify ``--allow-empty-source``.
     The default is to fail when the specified source directory doesn't exist
     or is empty.  (This check only applies to version 1.0 and later.)
 
-    Users with high-performance networks, or file sets with very small
-    files, will benefit from multi-threaded uploads and downloads. The default
-    number of threads for syncing, downloading, and uploading is 10.
-    The number of files processed in parallel is set by ``--syncThreads``,
-    the number of files/file parts downloaded in parallel is set by``--downloadThreads``,
-    and the number of files/file parts uploaded in parallel is set by `--uploadThreads``.
+    {ThreadsMixin}
+
+    You can alternatively control number of threads per each operation.
+    The number of files processed in parallel is set by ``--sync-threads``,
+    the number of files/file parts downloaded in parallel is set by``--download-threads``,
+    and the number of files/file parts uploaded in parallel is set by `--upload-threads``.
     All the three parameters can be set to the same value by ``--threads``.
     Experiment with parameters if the defaults are not working well.
 
     Users with low-performance networks may benefit from reducing the
     number of threads.  Using just one thread will minimize the impact
     on other users of the network.
 
     .. note::
 
         Note that using multiple threads could be detrimental to
         the other users on your network.
 
-    You can specify ``--excludeRegex`` to selectively ignore files that
+    You can specify ``--exclude-regex`` to selectively ignore files that
     match the given pattern. Ignored files will not copy during
     the sync operation. The pattern is a regular expression
     that is tested against the full path of each file.
 
-    You can specify ``--includeRegex`` to selectively override ignoring
-    files that match the given ``--excludeRegex`` pattern by an
-    ``--includeRegex`` pattern. Similarly to ``--excludeRegex``, the pattern
+    You can specify ``--include-regex`` to selectively override ignoring
+    files that match the given ``--exclude-regex`` pattern by an
+    ``--include-regex`` pattern. Similarly to ``--exclude-regex``, the pattern
     is a regular expression that is tested against the full path
     of each file.
 
     .. note::
 
-        Note that ``--includeRegex`` cannot be used without ``--excludeRegex``.
+        Note that ``--include-regex`` cannot be used without ``--exclude-regex``.
 
-    You can specify ``--excludeAllSymlinks`` to skip symlinks when
+    You can specify ``--exclude-all-symlinks`` to skip symlinks when
     syncing from a local source.
 
-    When a directory is excluded by using ``--excludeDirRegex``, all of
-    the files within it are excluded, even if they match an ``--includeRegex``
+    When a directory is excluded by using ``--exclude-dir-regex``, all of
+    the files within it are excluded, even if they match an ``--include-regex``
     pattern.   This means that there is no need to look inside excluded
     directories, and you can exclude directories containing files for which
     you don't have read permission and avoid getting errors.
 
-    The ``--excludeDirRegex`` is a regular expression that is tested against
+    The ``--exclude-dir-regex`` is a regular expression that is tested against
     the full path of each directory.  The path being matched does not have
     a trailing ``/``, so don't include on in your regular expression.
 
     Multiple regex rules can be applied by supplying them as pipe
     delimited instructions. Note that the regex for this command
     is Python regex.
     Reference: `<https://docs.python.org/3/library/re.html>`_
 
     Regular expressions are considered a match if they match a substring
     starting at the first character.  ``.*e`` will match ``hello``.  This is
     not ideal, but we will maintain this behavior for compatibility.
     If you want to match the entire path, put a ``$`` at the end of the
     regex, such as ``.*llo$``.
 
-    You can specify ``--excludeIfModifiedAfter`` to selectively ignore file versions
+    You can specify ``--exclude-if-modified-after`` to selectively ignore file versions
     (including hide markers) which were synced after given time (for local source)
     or ignore only specific file versions (for b2 source).
     Ignored files or file versions will not be taken for consideration during sync.
     The time should be given as a seconds timestamp (e.g. "1367900664")
     If you need milliseconds precision, put it after the comma (e.g. "1367900664.152")
 
     Files are considered to be the same if they have the same name
     and modification time.  This behaviour can be changed using the
-    ``--compareVersions`` option. Possible values are:
+    ``--compare-versions`` option. Possible values are:
 
     - ``none``:    Comparison using the file name only
     - ``modTime``: Comparison using the modification time (default)
     - ``size``:    Comparison using the file size
 
     A future enhancement may add the ability to compare the SHA1 checksum
     of the files.
 
     Fuzzy comparison of files based on modTime or size can be enabled by
-    specifying the ``--compareThreshold`` option.  This will treat modTimes
+    specifying the ``--compare-threshold`` option.  This will treat modTimes
     (in milliseconds) or sizes (in bytes) as the same if they are within
     the comparison threshold.  Files that match, within the threshold, will
-    not be synced. Specifying ``--verbose`` and ``--dryRun`` can be useful to
+    not be synced. Specifying ``--verbose`` and ``--dry-run`` can be useful to
     determine comparison value differences.
 
     When a destination file is present that is not in the source, the
     default is to leave it there.  Specifying ``--delete`` means to delete
     destination files that are not in the source.
 
     When the destination is B2, you have the option of leaving older
-    versions in place.  Specifying ``--keepDays`` will delete any older
+    versions in place.  Specifying ``--keep-days`` will delete any older
     versions more than the given number of days old, based on the
     modification time of the file.  This option is not available when
     the destination is a local folder.
 
     Files at the source that have a newer modification time are always
     copied to the destination.  If the destination file is newer, the
-    default is to report an error and stop.  But with ``--skipNewer`` set,
-    those files will just be skipped.  With ``--replaceNewer`` set, the
+    default is to report an error and stop.  But with ``--skip-newer`` set,
+    those files will just be skipped.  With ``--replace-newer`` set, the
     old file from the source will replace the newer one in the destination.
 
     To make the destination exactly match the source, use:
 
     .. code-block::
 
-        {NAME} sync --delete --replaceNewer ... ...
+        {NAME} sync --delete --replace-newer ... ...
 
     .. warning::
 
         Using ``--delete`` deletes files!  We recommend not using it.
-        If you use ``--keepDays`` instead, you will have some time to recover your
+        If you use ``--keep-days`` instead, you will have some time to recover your
         files if you discover they are missing on the source end.
 
     To make the destination match the source, but retain previous versions
     for 30 days:
 
     .. code-block::
 
-        {NAME} sync --keepDays 30 --replaceNewer ... b2://...
+        {NAME} sync --keep-days 30 --replace-newer ... b2://...
 
-    Example of sync being used with ``--excludeRegex``. This will ignore ``.DS_Store`` files
+    Example of sync being used with ``--exclude-regex``. This will ignore ``.DS_Store`` files
     and ``.Spotlight-V100`` folders:
 
     .. code-block::
 
-        {NAME} sync --excludeRegex '(.*\\.DS_Store)|(.*\\.Spotlight-V100)' ... b2://...
+        {NAME} sync --exclude-regex '(.*\\.DS_Store)|(.*\\.Spotlight-V100)' ... b2://...
 
-    {DESTINATIONSSEMIXIN}
-    {SOURCESSEMIXIN}
+    {DestinationSseMixin}
+    {SourceSseMixin}
 
-    {WRITEBUFFERSIZEMIXIN}
-    {SKIPHASHVERIFICATIONMIXIN}
-    {MAXDOWNLOADSTREAMSMIXIN}
-    {UPLOADMODEMIXIN}
+    {WriteBufferSizeMixin}
+    {SkipHashVerificationMixin}
+    {MaxDownloadStreamsMixin}
+    {UploadModeMixin}
 
     Requires capabilities:
 
     - **listFiles**
     - **readFiles** (for downloading)
     - **writeFiles** (for uploading)
     """
 
     DEFAULT_SYNC_THREADS = 10
     DEFAULT_DOWNLOAD_THREADS = 10
     DEFAULT_UPLOAD_THREADS = 10
 
+    FAIL_ON_REPORTER_ERRORS_OR_WARNINGS = True
+
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--noProgress', action='store_true')
-        parser.add_argument('--dryRun', action='store_true')
-        parser.add_argument('--allowEmptySource', action='store_true')
-        parser.add_argument('--excludeAllSymlinks', action='store_true')
-        parser.add_argument('--threads', type=int)
-        parser.add_argument('--syncThreads', type=int, default=cls.DEFAULT_SYNC_THREADS)
-        parser.add_argument('--downloadThreads', type=int, default=cls.DEFAULT_DOWNLOAD_THREADS)
-        parser.add_argument('--uploadThreads', type=int, default=cls.DEFAULT_UPLOAD_THREADS)
-        parser.add_argument(
-            '--compareVersions', default='modTime', choices=('none', 'modTime', 'size')
+        add_normalized_argument(parser, '--no-progress', action='store_true')
+        add_normalized_argument(parser, '--dry-run', action='store_true')
+        add_normalized_argument(parser, '--allow-empty-source', action='store_true')
+        add_normalized_argument(parser, '--exclude-all-symlinks', action='store_true')
+        add_normalized_argument(
+            parser, '--sync-threads', type=int, default=cls.DEFAULT_SYNC_THREADS
         )
-        parser.add_argument('--compareThreshold', type=int, metavar='MILLIS')
-        parser.add_argument('--excludeRegex', action='append', default=[], metavar='REGEX')
-        parser.add_argument('--includeRegex', action='append', default=[], metavar='REGEX')
-        parser.add_argument('--excludeDirRegex', action='append', default=[], metavar='REGEX')
-        parser.add_argument(
-            '--excludeIfModifiedAfter',
+        add_normalized_argument(
+            parser, '--download-threads', type=int, default=cls.DEFAULT_DOWNLOAD_THREADS
+        )
+        add_normalized_argument(
+            parser, '--upload-threads', type=int, default=cls.DEFAULT_UPLOAD_THREADS
+        )
+        add_normalized_argument(
+            parser, '--compare-versions', default='modTime', choices=('none', 'modTime', 'size')
+        )
+        add_normalized_argument(parser, '--compare-threshold', type=int, metavar='MILLIS')
+        add_normalized_argument(
+            parser, '--exclude-regex', action='append', default=[], metavar='REGEX'
+        )
+        add_normalized_argument(
+            parser, '--include-regex', action='append', default=[], metavar='REGEX'
+        )
+        add_normalized_argument(
+            parser, '--exclude-dir-regex', action='append', default=[], metavar='REGEX'
+        )
+        add_normalized_argument(
+            parser,
+            '--exclude-if-modified-after',
             type=parse_millis_from_float_timestamp,
             default=None,
             metavar='TIMESTAMP'
         )
-        super()._setup_parser(parser)  # add parameters from the mixins
+        super()._setup_parser(parser)  # add parameters from the mixins, and the parent class
         parser.add_argument('source')
         parser.add_argument('destination')
 
         skip_group = parser.add_mutually_exclusive_group()
-        skip_group.add_argument('--skipNewer', action='store_true')
-        skip_group.add_argument('--replaceNewer', action='store_true')
+        add_normalized_argument(skip_group, '--skip-newer', action='store_true')
+        add_normalized_argument(skip_group, '--replace-newer', action='store_true')
 
         del_keep_group = parser.add_mutually_exclusive_group()
-        del_keep_group.add_argument('--delete', action='store_true')
-        del_keep_group.add_argument('--keepDays', type=float, metavar='DAYS')
+        add_normalized_argument(del_keep_group, '--delete', action='store_true')
+        add_normalized_argument(del_keep_group, '--keep-days', type=float, metavar='DAYS')
 
-    def run(self, args):
+    def _run(self, args):
         policies_manager = self.get_policies_manager_from_args(args)
 
         if args.threads is not None:
-            if args.syncThreads != self.DEFAULT_SYNC_THREADS \
-                    or args.uploadThreads != self.DEFAULT_UPLOAD_THREADS \
-                    or args.downloadThreads != self.DEFAULT_DOWNLOAD_THREADS:
+            if args.sync_threads != self.DEFAULT_SYNC_THREADS \
+                    or args.upload_threads != self.DEFAULT_UPLOAD_THREADS \
+                    or args.download_threads != self.DEFAULT_DOWNLOAD_THREADS:
                 raise ValueError("--threads cannot be used with other thread options")
             sync_threads = upload_threads = download_threads = args.threads
         else:
-            sync_threads = args.syncThreads
-            upload_threads = args.uploadThreads
-            download_threads = args.downloadThreads
+            sync_threads = args.sync_threads
+            upload_threads = args.upload_threads
+            download_threads = args.download_threads
 
-        # FIXME: This is using deprecated API. It should be be replaced when moving to b2sdk apiver 3.
-        #        There are `max_X_workers` params in B2Api constructor for this.
         self.api.services.upload_manager.set_thread_pool_size(upload_threads)
         self.api.services.download_manager.set_thread_pool_size(download_threads)
 
         source = parse_sync_folder(args.source, self.console_tool.api)
         destination = parse_sync_folder(args.destination, self.console_tool.api)
-        allow_empty_source = args.allowEmptySource or VERSION_0_COMPATIBILITY
+        allow_empty_source = args.allow_empty_source or VERSION_0_COMPATIBILITY
 
         synchronizer = self.get_synchronizer_from_args(
             args,
             sync_threads,
             policies_manager,
             allow_empty_source,
             self.api.session.account_info.get_absolute_minimum_part_size(),
@@ -2409,111 +3095,113 @@
 
         if read_encryption_settings or write_encryption_settings:
             kwargs['encryption_settings_provider'] = BasicSyncEncryptionSettingsProvider(
                 read_bucket_settings=read_encryption_settings,
                 write_bucket_settings=write_encryption_settings,
             )
 
-        with SyncReport(self.stdout, args.noProgress) as reporter:
+        with SyncReport(self.stdout, args.no_progress or args.quiet) as reporter:
             try:
                 synchronizer.sync_folders(
                     source_folder=source,
                     dest_folder=destination,
                     now_millis=current_time_millis(),
                     reporter=reporter,
                     **kwargs
                 )
             except EmptyDirectory as ex:
                 raise CommandError(
-                    'Directory %s is empty.  Use --allowEmptySource to sync anyway.' % (ex.path,)
+                    f'Directory {ex.path} is empty.  Use --allow-empty-source to sync anyway.'
                 )
             except NotADirectory as ex:
-                raise CommandError('%s is not a directory' % (ex.path,))
+                raise CommandError(f'{ex.path} is not a directory')
             except UnableToCreateDirectory as ex:
-                raise CommandError('unable to create directory %s' % (ex.path,))
+                raise CommandError(f'unable to create directory {ex.path}')
+            if self.FAIL_ON_REPORTER_ERRORS_OR_WARNINGS and reporter.has_errors_or_warnings():
+                return 1
         return 0
 
     def get_policies_manager_from_args(self, args):
         return ScanPoliciesManager(
-            exclude_dir_regexes=args.excludeDirRegex,
-            exclude_file_regexes=args.excludeRegex,
-            include_file_regexes=args.includeRegex,
-            exclude_all_symlinks=args.excludeAllSymlinks,
-            exclude_modified_after=args.excludeIfModifiedAfter,
+            exclude_dir_regexes=args.exclude_dir_regex,
+            exclude_file_regexes=args.exclude_regex,
+            include_file_regexes=args.include_regex,
+            exclude_all_symlinks=args.exclude_all_symlinks,
+            exclude_modified_after=args.exclude_if_modified_after,
         )
 
     def get_synchronizer_from_args(
         self,
         args,
         max_workers,
         policies_manager=DEFAULT_SCAN_MANAGER,
         allow_empty_source=False,
         absolute_minimum_part_size=None,
     ):
-        if args.replaceNewer:
+        if args.replace_newer:
             newer_file_mode = NewerFileSyncMode.REPLACE
-        elif args.skipNewer:
+        elif args.skip_newer:
             newer_file_mode = NewerFileSyncMode.SKIP
         else:
             newer_file_mode = NewerFileSyncMode.RAISE_ERROR
 
-        if args.compareVersions == 'none':
+        if args.compare_versions == 'none':
             compare_version_mode = CompareVersionMode.NONE
-        elif args.compareVersions == 'modTime':
+        elif args.compare_versions == 'modTime':
             compare_version_mode = CompareVersionMode.MODTIME
-        elif args.compareVersions == 'size':
+        elif args.compare_versions == 'size':
             compare_version_mode = CompareVersionMode.SIZE
         else:
             compare_version_mode = CompareVersionMode.MODTIME
-        compare_threshold = args.compareThreshold
+        compare_threshold = args.compare_threshold
 
         keep_days = None
 
         if args.delete:
             keep_days_or_delete = KeepOrDeleteMode.DELETE
-        elif args.keepDays:
+        elif args.keep_days:
             keep_days_or_delete = KeepOrDeleteMode.KEEP_BEFORE_DELETE
-            keep_days = args.keepDays
+            keep_days = args.keep_days
         else:
             keep_days_or_delete = KeepOrDeleteMode.NO_DELETE
 
         upload_mode = self._get_upload_mode_from_args(args)
 
         return Synchronizer(
             max_workers,
             policies_manager=policies_manager,
-            dry_run=args.dryRun,
+            dry_run=args.dry_run,
             allow_empty_source=allow_empty_source,
             newer_file_mode=newer_file_mode,
             keep_days_or_delete=keep_days_or_delete,
             compare_version_mode=compare_version_mode,
             compare_threshold=compare_threshold,
             keep_days=keep_days,
             upload_mode=upload_mode,
             absolute_minimum_part_size=absolute_minimum_part_size,
         )
 
 
-@B2.register_subcommand
-class UpdateBucket(DefaultSseMixin, Command):
+class BucketUpdateBase(DefaultSseMixin, LifecycleRulesMixin, Command):
     """
-    Updates the ``bucketType`` of an existing bucket.  Prints the ID
-    of the bucket updated.
+    Updates the ``bucketType`` of an existing bucket.
 
+    Prints the ID of the bucket updated.
     Optionally stores bucket info, CORS rules and lifecycle rules with the bucket.
     These can be given as JSON on the command line.
 
-    {DEFAULTSSEMIXIN}
+    {DefaultSseMixin}
+    {LifecycleRulesMixin}
 
-    To set a default retention for files in the bucket ``--defaultRetentionMode`` and
-    ``--defaultRetentionPeriod`` have to be specified. The latter one is of the form "X days|years".
+    To set a default retention for files in the bucket ``--default-retention-mode`` and
+    ``--default-retention-period`` have to be specified. The latter one is of the form "X days|years".
 
     {FILE_RETENTION_COMPATIBILITY_WARNING}
 
-    This command can be used to set the bucket's ``fileLockEnabled`` flag to ``true`` using the ``--fileLockEnabled``
+    This command can be used to set the bucket's ``fileLockEnabled`` flag to ``true`` using the ``--file-lock-enabled``
     option.  This can only be done if the bucket is not set up as a replication source.
 
     .. warning::
 
         Once ``fileLockEnabled`` is set, it can NOT be reverted back to ``false``
 
     Please note that replication from file-lock-enabled bucket to file-lock-disabled bucket is not allowed, therefore
@@ -2532,221 +3220,502 @@
 
     - **writeBucketRetentions**
     - **writeBucketEncryption**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--bucketInfo', type=json.loads)
-        parser.add_argument('--corsRules', type=json.loads)
-        parser.add_argument('--lifecycleRules', type=json.loads)
-        parser.add_argument(
-            '--defaultRetentionMode',
+        add_normalized_argument(parser, '--bucket-info', type=validated_loads)
+        add_normalized_argument(
+            parser,
+            '--cors-rules',
+            type=validated_loads,
+            help=
+            "If given, the bucket will have a 'custom' CORS configuration. Accepts a JSON string."
+        )
+        add_normalized_argument(
+            parser,
+            '--default-retention-mode',
             choices=(
                 RetentionMode.COMPLIANCE.value,
                 RetentionMode.GOVERNANCE.value,
                 'none',
             ),
             default=None,
         )
-        parser.add_argument(
-            '--defaultRetentionPeriod',
+        add_normalized_argument(
+            parser,
+            '--default-retention-period',
             type=parse_default_retention_period,
             metavar='period',
         )
-        parser.add_argument('--replication', type=json.loads)
-        parser.add_argument(
-            '--fileLockEnabled',
+        parser.add_argument('--replication', type=validated_loads)
+        add_normalized_argument(
+            parser,
+            '--file-lock-enabled',
             action='store_true',
             default=None,
             help=
             "If given, the bucket will have the file lock mechanism enabled. This parameter cannot be changed back."
         )
-        parser.add_argument('bucketName').completer = bucket_name_completer
+        add_bucket_name_argument(parser)
         parser.add_argument('bucketType', nargs='?', choices=CREATE_BUCKET_TYPES)
 
-        super()._setup_parser(parser)  # add parameters from the mixins
+        super()._setup_parser(parser)  # add parameters from the mixins and the parent class
 
-    def run(self, args):
-        if args.defaultRetentionMode is not None:
-            if args.defaultRetentionMode == 'none':
+    def _run(self, args):
+        if args.default_retention_mode is not None:
+            if args.default_retention_mode == 'none':
                 default_retention = NO_RETENTION_BUCKET_SETTING
             else:
                 default_retention = BucketRetentionSetting(
-                    RetentionMode(args.defaultRetentionMode), args.defaultRetentionPeriod
+                    RetentionMode(args.default_retention_mode), args.default_retention_period
                 )
         else:
             default_retention = None
         encryption_setting = self._get_default_sse_setting(args)
         if args.replication is None:
             replication = None
         else:
             replication = ReplicationConfiguration.from_dict(args.replication)
         bucket = self.api.get_bucket_by_name(args.bucketName)
         bucket = bucket.update(
             bucket_type=args.bucketType,
-            bucket_info=args.bucketInfo,
-            cors_rules=args.corsRules,
-            lifecycle_rules=args.lifecycleRules,
+            bucket_info=args.bucket_info,
+            cors_rules=args.cors_rules,
+            lifecycle_rules=args.lifecycle_rules,
             default_server_side_encryption=encryption_setting,
             default_retention=default_retention,
             replication=replication,
-            is_file_lock_enabled=args.fileLockEnabled,
+            is_file_lock_enabled=args.file_lock_enabled,
         )
         self._print_json(bucket)
         return 0
 
 
-@B2.register_subcommand
-class UploadFile(
-    DestinationSseMixin, LegalHoldMixin, FileRetentionSettingMixin, UploadModeMixin, Command
+class MinPartSizeMixin(Described):
+    """
+    By default, the file is broken into many parts to maximize upload parallelism and increase speed.
+    Setting ``--min-part-size`` controls the minimal upload file part size.
+    Part size must be in 5MB to 5GB range.
+    Reference: `<https://www.backblaze.com/docs/cloud-storage-create-large-files-with-the-native-api>`_
+    """
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_normalized_argument(
+            parser,
+            '--min-part-size',
+            type=int,
+            help="minimum part size in bytes",
+            default=None,
+        )
+        super()._setup_parser(parser)  # noqa
+
+
+class UploadFileMixin(
+    HeaderFlagsMixin,
+    MinPartSizeMixin,
+    ThreadsMixin,
+    ProgressMixin,
+    DestinationSseMixin,
+    LegalHoldMixin,
+    FileRetentionSettingMixin,
+    metaclass=ABCMeta
 ):
     """
-    Uploads one file to the given bucket.  Uploads the contents
-    of the local file, and assigns the given name to the B2 file,
+    Content type is optional.
+    If not set, it will be guessed.
+
+    The maximum number of upload threads to use to upload parts of a large file is specified by ``--threads``.
+    It has no effect on "small" files (under 200MB as of writing this).
+
+    Each fileInfo is of the form ``a=b``.
+    """
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_normalized_argument(
+            parser,
+            '--content-type',
+            help="MIME type of the file being uploaded. If not set it will be guessed."
+        )
+        parser.add_argument(
+            '--sha1', help="SHA-1 of the data being uploaded for verifying file integrity"
+        )
+        parser.add_argument(
+            '--info',
+            action='append',
+            default=[],
+            help=
+            "additional file info to be stored with the file. Can be used multiple times for different information."
+        )
+        add_normalized_argument(
+            parser,
+            '--custom-upload-timestamp',
+            type=int,
+            help="overrides object creation date. Expressed as a number of milliseconds since epoch."
+        )
+        add_bucket_name_argument(parser, help="name of the bucket where the file will be stored")
+        parser.add_argument('localFilePath', help="path of the local file or stream to be uploaded")
+        parser.add_argument('b2FileName', help="name file will be given when stored in B2")
+
+        super()._setup_parser(parser)  # add parameters from the mixins
+
+    def _run(self, args):
+        self._set_threads_from_args(args)
+        upload_kwargs = self.get_execute_kwargs(args)
+        file_info = self.execute_operation(**upload_kwargs)
+        bucket = upload_kwargs["bucket"]
+        self._print("URL by file name: " + bucket.get_download_url(file_info.file_name))
+        self._print("URL by fileId: " + self.api.get_download_url_for_fileid(file_info.id_))
+        self._print_json(file_info)
+        return 0
+
+    def get_execute_kwargs(self, args) -> dict:
+        file_infos = self._parse_file_infos(args.info)
+
+        if SRC_LAST_MODIFIED_MILLIS not in file_infos and os.path.exists(args.localFilePath):
+            try:
+                mtime = os.path.getmtime(args.localFilePath)
+            except OSError:
+                if not points_to_fifo(pathlib.Path(args.localFilePath)):
+                    self._print_stderr(
+                        "WARNING: Unable to determine file modification timestamp. "
+                        f"{SRC_LAST_MODIFIED_MILLIS!r} file info won't be set."
+                    )
+            else:
+                file_infos[SRC_LAST_MODIFIED_MILLIS] = str(int(mtime * 1000))
+
+        file_infos = self._file_info_with_header_args(args, file_infos)
+
+        return {
+            "bucket":
+                self.api.get_bucket_by_name(args.bucketName),
+            "content_type":
+                args.content_type,
+            "custom_upload_timestamp":
+                args.custom_upload_timestamp,
+            "encryption":
+                self._get_destination_sse_setting(args),
+            "file_info":
+                file_infos,
+            "file_name":
+                args.b2FileName,
+            "file_retention":
+                self._get_file_retention_setting(args),
+            "legal_hold":
+                self._get_legal_hold_setting(args),
+            "local_file":
+                args.localFilePath,
+            "min_part_size":
+                args.min_part_size,
+            "progress_listener":
+                self.make_progress_listener(args.localFilePath, args.no_progress or args.quiet),
+            "sha1_sum":
+                args.sha1,
+            "threads":
+                self._get_threads_from_args(args),
+        }
+
+    @abstractmethod
+    def execute_operation(self, **kwargs) -> b2sdk.file_version.FileVersion:
+        raise NotImplementedError
+
+    def upload_file_kwargs_to_unbound_upload(self, **kwargs):
+        """
+        Translate `file upload` kwargs to unbound_upload equivalents
+        """
+        kwargs["large_file_sha1"] = kwargs.pop("sha1_sum", None)
+        kwargs["buffers_count"] = kwargs["threads"] + 1
+        kwargs["read_size"] = kwargs["min_part_size"] or DEFAULT_MIN_PART_SIZE
+        return kwargs
+
+    def get_input_stream(self, filename: str) -> str | int | io.BinaryIO:
+        """Get input stream IF filename points to a FIFO or stdin."""
+        if filename == "-":
+            if os.path.exists('-'):
+                self._print_stderr(
+                    "WARNING: Filename `-` won't be supported in the future and will always be treated as stdin alias."
+                )
+            else:
+                return sys.stdin.buffer if platform.system() == "Windows" else sys.stdin.fileno()
+        elif points_to_fifo(pathlib.Path(filename)):
+            return filename
+
+        raise self.NotAnInputStream()
+
+    def file_identifier_to_read_stream(self, file_id: str | int | BinaryIO, buffering) -> BinaryIO:
+        if isinstance(file_id, (str, int)):
+            return open(
+                file_id,
+                mode="rb",
+                closefd=not isinstance(file_id, int),
+                buffering=buffering,
+            )
+        return file_id
+
+    class NotAnInputStream(Exception):
+        pass
+
+
+class FileUploadBase(UploadFileMixin, UploadModeMixin, Command):
+    """
+    Upload single file to the given bucket.
+
+    Uploads the contents of the local file, and assigns the given name to the B2 file,
     possibly setting options like server-side encryption and retention.
 
-    {FILE_RETENTION_COMPATIBILITY_WARNING}
+    A FIFO file (such as named pipe) can be given instead of regular file.
 
-    By default, upload_file will compute the sha1 checksum of the file
+    By default, `file upload` will compute the sha1 checksum of the file
     to be uploaded.  But, if you already have it, you can provide it
     on the command line to save a little time.
 
-    Content type is optional.  If not set, it will be set based on the
-    file extension.
+    {FILE_RETENTION_COMPATIBILITY_WARNING}
+    {UploadFileMixin}
+    {MinPartSizeMixin}
+    {ProgressMixin}
+    {ThreadsMixin}
+    {DestinationSseMixin}
+    {FileRetentionSettingMixin}
+    {LegalHoldMixin}
+    {UploadModeMixin}
 
-    By default, the file is broken into as many parts as possible to
-    maximize upload parallelism and increase speed.  The minimum that
-    B2 allows is 100MB.  Setting ``--minPartSize`` to a larger value will
-    reduce the number of parts uploaded when uploading a large file.
-
-    The maximum number of upload threads to use to upload parts of a large file
-    is specified by ``--threads``.  It has no effect on small files (under 200MB).
-    Default is 10.
+    The ``--custom-upload-timestamp``, in milliseconds-since-epoch, can be used
+    to artificially change the upload timestamp of the file for the purpose
+    of preserving retention policies after migration of data from other storage.
+    The access to this feature is restricted - if you really need it, you'll
+    need to contact customer support to enable it temporarily for your account.
 
-    If the ``tqdm`` library is installed, progress bar is displayed
-    on stderr.  Without it, simple text progress is printed.
-    Use ``--noProgress`` to disable progress reporting.
+    Requires capability:
 
-    Each fileInfo is of the form ``a=b``.
+    - **writeFiles**
+    """
 
-    {DESTINATIONSSEMIXIN}
-    {FILERETENTIONSETTINGMIXIN}
-    {LEGALHOLDMIXIN}
-    {UPLOADMODEMIXIN}
+    def get_execute_kwargs(self, args) -> dict:
+        kwargs = super().get_execute_kwargs(args)
+        kwargs["upload_mode"] = self._get_upload_mode_from_args(args)
+        return kwargs
+
+    def execute_operation(self, local_file, bucket, threads, **kwargs):
+        try:
+            input_stream = self.get_input_stream(local_file)
+        except self.NotAnInputStream:  # it is a regular file
+            file_version = bucket.upload_local_file(local_file=local_file, **kwargs)
+        else:
+            if kwargs.pop("upload_mode", None) != UploadMode.FULL:
+                self._print_stderr(
+                    "WARNING: Ignoring upload mode setting as we are uploading a stream."
+                )
+            kwargs = self.upload_file_kwargs_to_unbound_upload(threads=threads, **kwargs)
+            del kwargs["threads"]
+            input_stream = self.file_identifier_to_read_stream(
+                input_stream, kwargs["min_part_size"] or DEFAULT_MIN_PART_SIZE
+            )
+            with input_stream:
+                file_version = bucket.upload_unbound_stream(read_only_object=input_stream, **kwargs)
+        return file_version
+
+
+class UploadUnboundStreamBase(UploadFileMixin, Command):
+    """
+    Uploads an unbound stream to the given bucket.
+
+    Uploads the contents of the unbound stream such as stdin or named pipe,
+    and assigns the given name to the resulting B2 file.
+
+    {FILE_RETENTION_COMPATIBILITY_WARNING}
+    {UploadFileMixin}
+    {MinPartSizeMixin}
+
+    As opposed to ``b2 file upload``, ``b2 upload-unbound-stream`` cannot choose optimal `partSize` on its own.
+    So on memory constrained system it is best to use ``--part-size`` option to set it manually.
+    During upload of unbound stream ``--part-size`` as well as ``--threads`` determine the amount of memory used.
+    The maximum memory use for the upload buffers can be estimated at ``partSize * threads``, that is ~1GB by default.
+    What is more, B2 Large File may consist of at most 10,000 parts, so ``minPartSize`` should be adjusted accordingly,
+    if you expect the stream to be larger than 50GB.
+
+    {ProgressMixin}
+    {ThreadsMixin}
+    {DestinationSseMixin}
+    {FileRetentionSettingMixin}
+    {LegalHoldMixin}
 
     The ``--custom-upload-timestamp``, in milliseconds-since-epoch, can be used
     to artificially change the upload timestamp of the file for the purpose
     of preserving retention policies after migration of data from other storage.
     The access to this feature is restricted - if you really need it, you'll
     need to contact customer support to enable it temporarily for your account.
 
     Requires capability:
 
     - **writeFiles**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--noProgress', action='store_true')
-        parser.add_argument('--quiet', action='store_true')
-        parser.add_argument('--contentType')
-        parser.add_argument('--minPartSize', type=int)
-        parser.add_argument('--sha1')
-        parser.add_argument('--threads', type=int, default=10)
-        parser.add_argument('--info', action='append', default=[])
-        parser.add_argument('--custom-upload-timestamp', type=int)
-        parser.add_argument('bucketName').completer = bucket_name_completer
-        parser.add_argument('localFilePath')
-        parser.add_argument('b2FileName')
-
-        super()._setup_parser(parser)  # add parameters from the mixins
+        add_normalized_argument(
+            parser,
+            '--part-size',
+            type=int,
+            default=None,
+            help=("part size in bytes. Must be in range of <minPartSize, 5GB>"),
+        )
+        add_normalized_argument(
+            parser,
+            '--unused-buffer-timeout-seconds',
+            type=float,
+            default=3600.0,
+            help=(
+                "maximum time in seconds that not a single part may sit in the queue,"
+                " waiting to be uploaded, before an error is returned"
+            ),
+        )
+        super()._setup_parser(parser)
 
-    def run(self, args):
-        file_infos = self._parse_file_infos(args.info)
+    def get_execute_kwargs(self, args) -> dict:
+        kwargs = super().get_execute_kwargs(args)
+        kwargs = self.upload_file_kwargs_to_unbound_upload(**kwargs)
+        kwargs["recommended_upload_part_size"] = args.part_size
+        kwargs["unused_buffer_timeout_seconds"] = args.unused_buffer_timeout_seconds
+        return kwargs
 
-        if SRC_LAST_MODIFIED_MILLIS not in file_infos:
-            file_infos[SRC_LAST_MODIFIED_MILLIS] = str(
-                int(os.path.getmtime(args.localFilePath) * 1000)
+    def execute_operation(self, local_file, bucket, threads, **kwargs):
+        try:
+            input_stream = self.get_input_stream(local_file)
+        except self.NotAnInputStream:  # it is a regular file
+            self._print_stderr(
+                "WARNING: You are using a stream upload command to upload a regular file. "
+                "While it will work, it is inefficient. "
+                "Use of `file upload` command is recommended."
             )
+            input_stream = local_file
 
-        # FIXME: This is using deprecated API. It should be be replaced when moving to b2sdk apiver 3.
-        #        There is `max_upload_workers` param in B2Api constructor for this.
-        self.api.services.upload_manager.set_thread_pool_size(args.threads)
+        input_stream = self.file_identifier_to_read_stream(
+            input_stream, kwargs["min_part_size"] or DEFAULT_MIN_PART_SIZE
+        )
+        with input_stream:
+            file_version = bucket.upload_unbound_stream(read_only_object=input_stream, **kwargs)
+        return file_version
 
-        bucket = self.api.get_bucket_by_name(args.bucketName)
-        encryption_setting = self._get_destination_sse_setting(args)
-        legal_hold = self._get_legal_hold_setting(args)
-        file_retention = self._get_file_retention_setting(args)
-        file_info = bucket.upload_local_file(
-            local_file=args.localFilePath,
-            file_name=args.b2FileName,
-            content_type=args.contentType,
-            file_infos=file_infos,
-            sha1_sum=args.sha1,
-            min_part_size=args.minPartSize,
-            progress_listener=make_progress_listener(args.localFilePath, args.noProgress),
-            encryption=encryption_setting,
-            file_retention=file_retention,
-            legal_hold=legal_hold,
-            upload_mode=self._get_upload_mode_from_args(args),
-            custom_upload_timestamp=args.custom_upload_timestamp,
+
+class FileUpdateBase(B2URIFileArgMixin, LegalHoldMixin, Command):
+    """
+    Update file settings.
+
+    Setting legal holds only works in bucket with fileLockEnabled=true.
+
+    Retention:
+
+      Only works in bucket with fileLockEnabled=true. Providing a ``retention-mode`` other than ``none`` requires
+      providing ``retainUntil``, which has to be a future timestamp in the form of an integer representing milliseconds
+      since epoch.
+
+      If a file already is in governance mode, disabling retention or shortening it's period requires providing
+      ``--bypass-governance``.
+
+      If a file already is in compliance mode, disabling retention or shortening it's period is impossible.
+
+      In both cases prolonging the retention period is possible. Changing from governance to compliance is also supported.
+
+      {FILE_RETENTION_COMPATIBILITY_WARNING}
+
+    Requires capability:
+
+    - **readFiles**
+    - **writeFileLegalHolds** (if updating legal holds)
+    - **writeFileRetentions** (if updating retention)
+    - **bypassGovernance** (if --bypass-governance is used)
+    """
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        super()._setup_parser(parser)
+
+        add_normalized_argument(
+            parser,
+            '--file-retention-mode',
+            default=None,
+            choices=(RetentionMode.COMPLIANCE.value, RetentionMode.GOVERNANCE.value, 'none')
         )
-        if not args.quiet:
-            self._print("URL by file name: " + bucket.get_download_url(args.b2FileName))
-            self._print("URL by fileId: " + self.api.get_download_url_for_fileid(file_info.id_))
-        self._print_json(file_info)
+        add_normalized_argument(
+            parser,
+            '--retain-until',
+            type=parse_millis_from_float_timestamp,
+            metavar='TIMESTAMP',
+            default=None
+        )
+        add_normalized_argument(parser, '--bypass-governance', action='store_true', default=False)
+
+    def _run(self, args):
+        b2_uri = self.get_b2_uri_from_arg(args)
+        file_version = self.api.get_file_info_by_uri(b2_uri)
+
+        if args.legal_hold is not None:
+            self.api.update_file_legal_hold(
+                file_version.id_, file_version.file_name, LegalHold(args.legal_hold)
+            )
+
+        if args.file_retention_mode is not None:
+            if args.file_retention_mode == 'none':
+                file_retention = FileRetentionSetting(RetentionMode.NONE)
+            else:
+                file_retention = FileRetentionSetting(
+                    RetentionMode(args.file_retention_mode), args.retain_until
+                )
+
+            self.api.update_file_retention(
+                file_version.id_, file_version.file_name, file_retention, args.bypass_governance
+            )
+
         return 0
 
 
-@B2.register_subcommand
-class UpdateFileLegalHold(FileIdAndOptionalFileNameMixin, Command):
+class UpdateFileLegalHoldBase(FileIdAndOptionalFileNameMixin, Command):
     """
     Only works in buckets with fileLockEnabled=true.
 
-    {FILEIDANDOPTIONALFILENAMEMIXIN}
+    {FileIdAndOptionalFileNameMixin}
 
     Requires capability:
 
     - **writeFileLegalHolds**
     - **readFiles** (if file name not provided)
 
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         super()._setup_parser(parser)
         parser.add_argument('legalHold', choices=(LegalHold.ON.value, LegalHold.OFF.value))
 
-    def run(self, args):
+    def _run(self, args):
         file_name = self._get_file_name_from_args(args)
-
         legal_hold = LegalHold(args.legalHold)
-
         self.api.update_file_legal_hold(args.fileId, file_name, legal_hold)
         return 0
 
 
-@B2.register_subcommand
-class UpdateFileRetention(FileIdAndOptionalFileNameMixin, Command):
+class UpdateFileRetentionBase(FileIdAndOptionalFileNameMixin, Command):
     """
-    Only works in buckets with fileLockEnabled=true. Providing a ``retentionMode`` other than ``none`` requires
+    Only works in buckets with fileLockEnabled=true. Providing a ``retention-mode`` other than ``none`` requires
     providing ``retainUntil``, which has to be a future timestamp in the form of an integer representing milliseconds
     since epoch.
 
     If a file already is in governance mode, disabling retention or shortening it's period requires providing
-    ``--bypassGovernance``.
+    ``--bypass-governance``.
 
     If a file already is in compliance mode, disabling retention or shortening it's period is impossible.
 
     {FILE_RETENTION_COMPATIBILITY_WARNING}
 
     In both cases prolonging the retention period is possible. Changing from governance to compliance is also supported.
 
-    {FILEIDANDOPTIONALFILENAMEMIXIN}
+    {FileIdAndOptionalFileNameMixin}
 
     Requires capability:
 
     - **writeFileRetentions**
     - **readFiles** (if file name not provided)
 
     and optionally:
@@ -2757,81 +3726,88 @@
     @classmethod
     def _setup_parser(cls, parser):
         super()._setup_parser(parser)
         parser.add_argument(
             'retentionMode',
             choices=(RetentionMode.GOVERNANCE.value, RetentionMode.COMPLIANCE.value, 'none')
         )
-        parser.add_argument(
-            '--retainUntil',
+        add_normalized_argument(
+            parser,
+            '--retain-until',
             type=parse_millis_from_float_timestamp,
             metavar='TIMESTAMP',
             default=None
         )
-        parser.add_argument('--bypassGovernance', action='store_true', default=False)
+        add_normalized_argument(parser, '--bypass-governance', action='store_true', default=False)
 
-    def run(self, args):
+    def _run(self, args):
         file_name = self._get_file_name_from_args(args)
 
         if args.retentionMode == 'none':
             file_retention = FileRetentionSetting(RetentionMode.NONE)
         else:
             file_retention = FileRetentionSetting(
-                RetentionMode(args.retentionMode), args.retainUntil
+                RetentionMode(args.retentionMode), args.retain_until
             )
 
         self.api.update_file_retention(
-            args.fileId, file_name, file_retention, args.bypassGovernance
+            args.fileId, file_name, file_retention, args.bypass_governance
         )
         return 0
 
 
-@B2.register_subcommand
-class ReplicationSetup(Command):
+class ReplicationSetupBase(Command):
     """
+    Set up replication between two buckets.
+
     Sets up replication between two buckets (potentially from different accounts), creating and replacing keys if necessary.
 
     Requires capabilities on both profiles:
 
     - **listKeys**
     - **createKeys**
     - **readReplications**
     - **writeReplications**
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         super()._setup_parser(parser)
-        parser.add_argument('--destination-profile', default=None)
+        add_normalized_argument(parser, '--destination-profile', default=None)
         parser.add_argument('source', metavar='SOURCE_BUCKET_NAME')
         parser.add_argument('destination', metavar='DESTINATION_BUCKET_NAME')
-        parser.add_argument('--name', help='name for the new replication rule on the source side')
-        parser.add_argument(
+        add_normalized_argument(
+            parser, '--name', help='name for the new replication rule on the source side'
+        )
+        add_normalized_argument(
+            parser,
             '--priority',
             help=
             'priority for the new replication rule on the source side [%d-%d]. Will be set automatically when not specified.'
             % (
                 ReplicationRule.MIN_PRIORITY,
                 ReplicationRule.MAX_PRIORITY,
             ),
             type=int,
             default=None,
         )
-        parser.add_argument(
+        add_normalized_argument(
+            parser,
             '--file-name-prefix',
             metavar='PREFIX',
             help='only replicate files starting with PREFIX'
         )
-        parser.add_argument(
+        add_normalized_argument(
+            parser,
             '--include-existing-files',
             action='store_true',
             help='if given, also replicates files uploaded prior to creation of the replication rule'
         )
 
-    def run(self, args):
+    def _run(self, args):
         if args.destination_profile is None:
             destination_api = self.api
         else:
             destination_api = _get_b2api_for_profile(args.destination_profile)
 
         helper = ReplicationSetupHelper()
         helper.setup_both(
@@ -2849,27 +3825,27 @@
 class ReplicationRuleChanger(Command, metaclass=ABCMeta):
     @classmethod
     def _setup_parser(cls, parser):
         super()._setup_parser(parser)
         parser.add_argument('source', metavar='SOURCE_BUCKET_NAME')
         parser.add_argument('rule_name', metavar='REPLICATION_RULE_NAME')
 
-    def run(self, args):
+    def _run(self, args):
         bucket = self.api.get_bucket_by_name(args.source).get_fresh_state()
         found, altered = self.alter_rule_by_name(bucket, args.rule_name)
         if not found:
             print('ERROR: replication rule could not be found!')
             return 1
         elif not altered:
             print('ERROR: replication rule was found, but could not be changed!')
             return 1
         return 0
 
     @classmethod
-    def alter_rule_by_name(cls, bucket: Bucket, name: str) -> Tuple[bool, bool]:
+    def alter_rule_by_name(cls, bucket: Bucket, name: str) -> tuple[bool, bool]:
         """ returns False if rule could not be found """
         if not bucket.replication or not bucket.replication.rules:
             return False, False
 
         found = False
         altered = False
 
@@ -2896,113 +3872,113 @@
             )
             bucket.update(
                 if_revision_is=bucket.revision,
                 replication=new_replication_configuration,
             )
         return found, altered
 
-    @abstractclassmethod
-    def alter_one_rule(cls, rule: ReplicationRule) -> Optional[ReplicationRule]:
+    @classmethod
+    @abstractmethod
+    def alter_one_rule(cls, rule: ReplicationRule) -> ReplicationRule | None:
         """ return None to delete a rule """
         pass
 
 
-@B2.register_subcommand
-class ReplicationDelete(ReplicationRuleChanger):
+class ReplicationDeleteBase(ReplicationRuleChanger):
     """
-    Deletes a replication rule
+    Delete a replication rule
 
     Requires capabilities:
 
     - **readReplications**
     - **writeReplications**
     """
 
     @classmethod
-    def alter_one_rule(cls, rule: ReplicationRule) -> Optional[ReplicationRule]:
+    def alter_one_rule(cls, rule: ReplicationRule) -> ReplicationRule | None:
         """ return None to delete rule """
         return None
 
 
-@B2.register_subcommand
-class ReplicationPause(ReplicationRuleChanger):
+class ReplicationPauseBase(ReplicationRuleChanger):
     """
-    Pauses a replication rule
+    Pause a replication rule
 
     Requires capabilities:
 
     - **readReplications**
     - **writeReplications**
     """
 
     @classmethod
-    def alter_one_rule(cls, rule: ReplicationRule) -> Optional[ReplicationRule]:
+    def alter_one_rule(cls, rule: ReplicationRule) -> ReplicationRule | None:
         """ return None to delete rule """
         rule.is_enabled = False
         return rule
 
 
-@B2.register_subcommand
-class ReplicationUnpause(ReplicationRuleChanger):
+class ReplicationUnpauseBase(ReplicationRuleChanger):
     """
-    Unpauses a replication rule
+    Unpause a replication rule
 
     Requires capabilities:
 
     - **readReplications**
     - **writeReplications**
     """
 
     @classmethod
-    def alter_one_rule(cls, rule: ReplicationRule) -> Optional[ReplicationRule]:
+    def alter_one_rule(cls, rule: ReplicationRule) -> ReplicationRule | None:
         """ return None to delete rule """
         rule.is_enabled = True
         return rule
 
 
-@B2.register_subcommand
-class ReplicationStatus(Command):
+class ReplicationStatusBase(Command):
     """
+    Display detailed replication statistics
+
     Inspects files in only source or both source and destination buckets
     (potentially from different accounts) and provides detailed replication statistics.
 
     Please be aware that only latest file versions are inspected, so any previous
     file versions are not represented in these statistics.
 
     --output-format
     "Console" output format is meant to be human-readable and is subject to change
     in any further release. One should use "json" for reliable "no-breaking-changes"
     output format. When piping "csv" format to some .csv file, it's handy to use
-    --noProgress flag which will disable interactive reporting output, otherwise it will
+    --no-progress flag which will disable interactive reporting output, otherwise it will
     also go to target csv file's first line.
 
     --columns
     Comma-separated list of columns to be shown. The rows are still grouped by _all_
     columns, no matter which of them are shown / hidden when using --columns flag.
     """
 
     @classmethod
     def _setup_parser(cls, parser):
         super()._setup_parser(parser)
         parser.add_argument('source', metavar='SOURCE_BUCKET_NAME')
-        parser.add_argument('--rule', metavar='REPLICATION_RULE_NAME', default=None)
-        parser.add_argument('--destination-profile')
-        parser.add_argument('--dont-scan-destination', action='store_true')
-        parser.add_argument(
-            '--output-format', default='console', choices=('console', 'json', 'csv')
-        )
-        parser.add_argument('--noProgress', action='store_true')
-        parser.add_argument(
+        add_normalized_argument(parser, '--rule', metavar='REPLICATION_RULE_NAME', default=None)
+        add_normalized_argument(parser, '--destination-profile')
+        add_normalized_argument(parser, '--dont-scan-destination', action='store_true')
+        add_normalized_argument(
+            parser, '--output-format', default='console', choices=('console', 'json', 'csv')
+        )
+        add_normalized_argument(parser, '--no-progress', action='store_true')
+        add_normalized_argument(
+            parser,
             '--columns',
             default=['all'],
             type=lambda value: re.split(r', ?', value),
             metavar='COLUMN ONE,COLUMN TWO'
         )
 
-    def run(self, args):
+    def _run(self, args):
         destination_api = args.destination_profile and _get_b2api_for_profile(
             args.destination_profile
         )
 
         try:
             bucket = self.api.list_buckets(args.source)[0]
         except IndexError:
@@ -3020,15 +3996,15 @@
 
         results = {
             rule.name: self.get_results_for_rule(
                 bucket=bucket,
                 rule=rule,
                 destination_api=destination_api,
                 scan_destination=not args.dont_scan_destination,
-                quiet=args.noProgress,
+                quiet=args.no_progress or args.quiet,
             )
             for rule in rules
         }
 
         if args.columns[0] != 'all':
             results = {
                 rule_name: self.filter_results_columns(
@@ -3048,17 +4024,17 @@
         else:
             self._print_stderr(f'ERROR: format "{args.output_format}" is not supported')
 
         return 0
 
     @classmethod
     def get_results_for_rule(
-        cls, bucket: Bucket, rule: ReplicationRule, destination_api: Optional[B2Api],
+        cls, bucket: Bucket, rule: ReplicationRule, destination_api: B2Api | None,
         scan_destination: bool, quiet: bool
-    ) -> List[dict]:
+    ) -> list[dict]:
         monitor = ReplicationMonitor(
             bucket=bucket,
             rule=rule,
             destination_api=destination_api,
             report=ProgressReport(sys.stdout, quiet),
         )
         report = monitor.scan(scan_destination=scan_destination)
@@ -3067,15 +4043,15 @@
             {
                 **dataclasses.asdict(result),
                 'count': count,
             } for result, count in report.counter_by_status.items()
         ]
 
     @classmethod
-    def filter_results_columns(cls, results: List[dict], columns: List[str]) -> List[dict]:
+    def filter_results_columns(cls, results: list[dict], columns: list[str]) -> list[dict]:
         return [{key: result[key] for key in columns} for result in results]
 
     @classmethod
     def to_human_readable(cls, value: Any) -> str:
         if isinstance(value, Enum):
             return value.name
 
@@ -3083,30 +4059,30 @@
             return 'Yes' if value else 'No'
 
         if value is None:
             return ''
 
         return str(value)
 
-    def output_json(self, results: Dict[str, List[dict]]) -> None:
+    def output_json(self, results: dict[str, list[dict]]) -> None:
         self._print_json(results)
 
-    def output_console(self, results: Dict[str, List[dict]]) -> None:
+    def output_console(self, results: dict[str, list[dict]]) -> None:
         for rule_name, rule_results in results.items():
             self._print(f'Replication "{rule_name}":')
             rule_results = [
                 {
                     key.replace('_', '\n'):  # split key to minimize column size
                     self.to_human_readable(value)
                     for key, value in result.items()
                 } for result in rule_results
             ]
             self._print(tabulate(rule_results, headers='keys', tablefmt='grid'))
 
-    def output_csv(self, results: Dict[str, List[dict]]) -> None:
+    def output_csv(self, results: dict[str, list[dict]]) -> None:
 
         rows = []
 
         for rule_name, rule_results in results.items():
             rows += [
                 {
                     'rule name': rule_name,
@@ -3122,81 +4098,95 @@
             return
 
         writer = csv.DictWriter(sys.stdout, fieldnames=list(rows[0].keys()))
         writer.writeheader()
         writer.writerows(rows)
 
 
-@B2.register_subcommand
 class Version(Command):
     """
-    Prints the version number of this tool.
+    Print the version number of this tool.
     """
 
     REQUIRES_AUTH = False
 
-    def run(self, args):
-        self._print('b2 command line tool, version', VERSION)
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_normalized_argument(parser, '--short', action='store_true')
+        super()._setup_parser(parser)
+
+    def _run(self, args):
+        if args.short:
+            self._print(VERSION)
+        else:
+            self._print('b2 command line tool, version', VERSION)
         return 0
 
 
-@B2.register_subcommand
 class License(Command):  # pragma: no cover
     """
-    Prints the license of B2 Command line tool and all libraries shipped with it.
+    Print the license information for this tool.
+
+    Displays the license of B2 Command line tool and all libraries shipped with it.
     """
-    LICENSE_OUTPUT_FILE = pathlib.Path(__file__).parent / 'licenses_output.txt'
+    LICENSE_OUTPUT_FILE = pathlib.Path(__file__).parent.parent / 'licenses_output.txt'
 
     REQUIRES_AUTH = False
     IGNORE_MODULES = {'b2', 'distlib', 'patchelf-wrapper', 'platformdirs'}
     REQUEST_TIMEOUT_S = 5
 
     # In case of some modules, we provide manual
     # overrides to the license text extracted by piplicenses.
     # Thanks to this set, we make sure the module is still used
     # PTable is used on versions below Python 3.11
     MODULES_TO_OVERRIDE_LICENSE_TEXT = {'rst2ansi', 'b2sdk'}
 
     LICENSES = {
+        'argcomplete':
+            'https://raw.githubusercontent.com/kislyuk/argcomplete/develop/LICENSE.rst',
         'atomicwrites':
             'https://raw.githubusercontent.com/untitaker/python-atomicwrites/master/LICENSE',
         'platformdirs':
             'https://raw.githubusercontent.com/platformdirs/platformdirs/main/LICENSE.txt',
         'PTable':
             'https://raw.githubusercontent.com/jazzband/prettytable/main/LICENSE',
         'pipx':
             'https://raw.githubusercontent.com/pypa/pipx/main/LICENSE',
         'userpath':
             'https://raw.githubusercontent.com/ofek/userpath/master/LICENSE.txt',
         'future':
             'https://raw.githubusercontent.com/PythonCharmers/python-future/master/LICENSE.txt',
         'pefile':
             'https://raw.githubusercontent.com/erocarrera/pefile/master/LICENSE',
+        'https://github.com/python/typeshed':
+            'https://raw.githubusercontent.com/python/typeshed/main/LICENSE',
     }
 
     class NormalizingStringIO(io.StringIO):
         def write(self, text, *args, **kwargs):
             super().write(unicodedata.normalize('NFKD', text), *args, **kwargs)
 
     def __init__(self, console_tool):
         super().__init__(console_tool)
         self.request_session = requests.session()
 
     @classmethod
     def _setup_parser(cls, parser):
         # these are for building, users should not call it:
-        parser.add_argument('--dump', action='store_true', default=False, help=argparse.SUPPRESS)
-        parser.add_argument(
-            '--with-packages', action='store_true', default=False, help=argparse.SUPPRESS
+        add_normalized_argument(
+            parser, '--dump', action='store_true', default=False, help=argparse.SUPPRESS
+        )
+        add_normalized_argument(
+            parser, '--with-packages', action='store_true', default=False, help=argparse.SUPPRESS
         )
         super()._setup_parser(parser)
 
-    def run(self, args):
+    def _run(self, args):
         if self.LICENSE_OUTPUT_FILE.exists() and not args.dump:
-            self._print(self.LICENSE_OUTPUT_FILE.read_text())
+            self._print(self.LICENSE_OUTPUT_FILE.read_text(encoding='utf8'))
             return 0
 
         if args.dump:
             with self.LICENSE_OUTPUT_FILE.open('w', encoding='utf8') as file:
                 self._put_license_text(file, with_packages=args.with_packages)
         else:
             stream = self.NormalizingStringIO()
@@ -3206,33 +4196,34 @@
 
         return 0
 
     def _put_license_text(self, stream: io.StringIO, with_packages: bool = False):
         if with_packages:
             self._put_license_text_for_packages(stream)
 
+        b2_call_name = self.console_tool.b2_binary_name
         included_sources = get_included_sources()
         if included_sources:
             stream.write(
-                '\n\nThird party libraries modified and included in %s or %s:\n' %
-                (NAME, b2sdk.__name__)
+                f'\n\nThird party libraries modified and included in {b2_call_name} or {b2sdk.__name__}:\n'
             )
         for src in included_sources:
             stream.write('\n')
             stream.write(src.name)
             stream.write('\n')
             stream.write(src.comment)
             stream.write('\n')
             stream.write('Files included for legal compliance reasons:\n')
             files_table = prettytable.PrettyTable(['File name', 'Content'], hrules=prettytable.ALL)
             for file_name, file_content in src.files.items():
                 files_table.add_row([file_name, file_content])
             stream.write(str(files_table))
-        stream.write('\n\n%s license:\n' % (NAME,))
-        b2_license_file_text = (pathlib.Path(__file__).parent / 'LICENSE').read_text()
+        stream.write(f'\n\n{b2_call_name} license:\n')
+        b2_license_file_text = (pathlib.Path(__file__).parent.parent /
+                                'LICENSE').read_text(encoding='utf8')
         stream.write(b2_license_file_text)
 
     def _put_license_text_for_packages(self, stream: io.StringIO):
         license_table = prettytable.PrettyTable(
             ['Module name', 'License text'], hrules=prettytable.ALL
         )
         summary_table = prettytable.PrettyTable(
@@ -3253,39 +4244,51 @@
                     module_info['URL'],
                 ]
             )
             license_table.add_row([module_info['Name'], self._get_single_license(module_info)])
             modules_added.add(module_info['Name'])
 
         assert not (self.MODULES_TO_OVERRIDE_LICENSE_TEXT - modules_added)
+        b2_call_name = self.console_tool.b2_binary_name
         stream.write(
-            'Licenses of all modules used by %s, shipped with it in binary form:\n' % (NAME,)
+            f'Licenses of all modules used by {b2_call_name}, shipped with it in binary form:\n'
         )
         stream.write(str(license_table))
         stream.write(
-            '\n\nSummary of all modules used by %s, shipped with it in binary form:\n' % (NAME,)
+            f'\n\nSummary of all modules used by {b2_call_name}, shipped with it in binary form:\n'
         )
         stream.write(str(summary_table))
 
     @classmethod
-    def _get_licenses_dicts(cls) -> List[Dict]:
+    def _get_licenses_dicts(cls) -> list[dict]:
         assert piplicenses, 'In order to run this command, you need to install the `license` extra: pip install b2[license]'
+        pipdeptree_run = subprocess.run(
+            ["pipdeptree", "--json", "-p", "b2"],
+            capture_output=True,
+            text=True,
+            check=True,
+        )
+        pipdeptree = json.loads(pipdeptree_run.stdout)
+        used_packages = [dep["package"]['package_name'] for dep in pipdeptree]
+
         parser = piplicenses.create_parser()
         args = parser.parse_args(
             [
                 '--format',
                 'j',
                 '--with-system',
                 '--with-authors',
                 '--with-urls',
                 '--with-license-file',
+                '--packages',
+                *used_packages,
             ]
         )
         licenses_output = piplicenses.create_output_string(args)
-        licenses = json.loads(licenses_output)
+        licenses = validated_loads(licenses_output)
         return licenses
 
     def _fetch_license_from_url(self, url: str) -> str:
         response = self.request_session.get(url, timeout=self.REQUEST_TIMEOUT_S)
         response.raise_for_status()
         return response.text
 
@@ -3295,26 +4298,29 @@
         if module_name == 'rst2ansi':
             # this one module is problematic, we need to extract the license text from its docstring
             assert license_ == piplicenses.LICENSE_UNKNOWN  # let's make sure they didn't fix it
             license_ = rst2ansi.__doc__
             assert 'MIT License' in license_  # let's make sure the license is still there
         elif module_name == 'b2sdk':
             license_ = (pathlib.Path(b2sdk.__file__).parent / 'LICENSE').read_text()
-        elif module_name in self.LICENSES:
-            license_ = self._fetch_license_from_url(self.LICENSES[module_name])
+        else:
+            license_url = self.LICENSES.get(module_name) or self.LICENSES.get(
+                module_dict.get('URL')
+            )
+            if license_url:
+                license_ = self._fetch_license_from_url(license_url)
 
         assert license_ != piplicenses.LICENSE_UNKNOWN, module_name
 
         return license_
 
 
-@B2.register_subcommand
 class InstallAutocomplete(Command):
     """
-    Installs autocomplete for supported shells.
+    Install autocomplete for supported shells.
 
     Autocomplete is installed for the current user only and will become available after shell reload.
     Any existing autocomplete configuration for same executable name will be overwritten.
 
     --shell SHELL
     Shell to install autocomplete for. Autodetected if not specified.
     Manually specify "bash" to force bash autocomplete installation when running under different shell.
@@ -3324,213 +4330,1144 @@
         Please note this command WILL modify your shell configuration file (e.g. ~/.bashrc).
     """
 
     REQUIRES_AUTH = False
 
     @classmethod
     def _setup_parser(cls, parser):
-        parser.add_argument('--shell', choices=SUPPORTED_SHELLS, default=None)
+        add_normalized_argument(parser, '--shell', choices=SUPPORTED_SHELLS, default=None)
         super()._setup_parser(parser)
 
-    def run(self, args):
+    def _run(self, args):
         shell = args.shell or detect_shell()
         if shell not in SUPPORTED_SHELLS:
             self._print_stderr(
                 f'ERROR: unsupported shell: {shell}. Supported shells: {SUPPORTED_SHELLS}. Use --shell to specify a target shell manually.'
             )
             return 1
 
         try:
-            autocomplete_install(NAME, shell=shell)
+            autocomplete_install(self.console_tool.b2_binary_name, shell=shell)
         except AutocompleteInstallError as e:
             raise CommandError(str(e)) from e
         self._print(f'Autocomplete successfully installed for {shell}.')
         self._print(
             f'Spawn a new shell instance to use it (log in again or just type `{shell}` in your current shell to start a new session inside of the existing session).'
         )
         return 0
 
 
-class ConsoleTool(object):
+class BucketNotificationRuleWarningMixin(Described):
+    """
+    .. warning::
+
+        Event Notifications feature is in \"Private Preview\" state and may change without notice.
+        See https://www.backblaze.com/blog/announcing-event-notifications/ for details.
+    """
+
+
+class BucketNotificationRuleBase(BucketNotificationRuleWarningMixin, Command):
+    """
+    Bucket notification rules management subcommands.
+
+    {BucketNotificationRuleWarningMixin}
+
+    For more information on each subcommand, use ``{NAME} bucket notification-rule SUBCOMMAND --help``.
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} bucket notification-rule create b2://bucketName/optionalSubPath/ ruleName --event-type "b2:ObjectCreated:*" --webhook-url https://example.com/webhook
+        {NAME} bucket notification-rule list b2://bucketName
+        {NAME} bucket notification-rule update b2://bucketName/newPath/ ruleName --disable --event-type "b2:ObjectCreated:*" --event-type "b2:ObjectHidden:*"
+        {NAME} bucket notification-rule delete b2://bucketName ruleName
+    """
+    subcommands_registry = ClassRegistry(attr_name='COMMAND_NAME')
+
+
+@BucketNotificationRuleBase.subcommands_registry.register
+class BucketNotificationRuleList(JSONOptionMixin, BucketNotificationRuleWarningMixin, Command):
+    """
+    Allows listing bucket notification rules of the given bucket.
+
+    {BucketNotificationRuleWarningMixin}
+
+    {JSONOptionMixin}
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} notification-rule list b2://bucketName
+
+
+    Requires capability:
+
+    - **readBucketNotifications**
+    """
+    COMMAND_NAME = 'list'
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_b2_uri_argument(
+            parser,
+            help=
+            "B2 URI of the bucket with optional path prefix, e.g. b2://bucketName or b2://bucketName/optionalSubPath/"
+        )
+        super()._setup_parser(parser)
+
+    def _run(self, args):
+        bucket = self.api.get_bucket_by_name(args.B2_URI.bucket_name)
+        rules = sorted(
+            (
+                rule for rule in bucket.get_notification_rules()
+                if rule["objectNamePrefix"].startswith(args.B2_URI.path)
+            ),
+            key=lambda rule: rule["name"]
+        )
+        if args.json:
+            self._print_json(rules)
+        else:
+            if rules:
+                self._print(f'Notification rules for {args.B2_URI} :')
+                self._print_human_readable_structure(rules)
+            else:
+                self._print(f'No notification rules for {args.B2_URI}')
+        return 0
+
+
+class BucketNotificationRuleCreateBase(
+    JSONOptionMixin, BucketNotificationRuleWarningMixin, Command
+):
+    @classmethod
+    def _validate_secret(cls, value: str) -> str:
+        if not re.match(r'^[a-zA-Z0-9]{32}$', value):
+            raise argparse.ArgumentTypeError(
+                f'the secret has to be exactly 32 alphanumeric characters, got: {value!r}'
+            )
+        return value
+
+    @classmethod
+    def setup_rule_fields_parser(cls, parser, creation: bool):
+        add_b2_uri_argument(
+            parser,
+            help=
+            "B2 URI of the bucket with optional path prefix, e.g. b2://bucketName or b2://bucketName/optionalSubPath/"
+        )
+        parser.add_argument('ruleName', help="Name of the rule")
+        parser.add_argument(
+            '--event-type',
+            action='append',
+            help=
+            "Events scope, e.g., 'b2:ObjectCreated:*'. Can be used multiple times to set multiple scopes.",
+            required=creation
+        )
+        parser.add_argument(
+            '--webhook-url', help="URL to send the notification to", required=creation
+        )
+        parser.add_argument(
+            '--sign-secret',
+            help="optional signature key consisting of 32 alphanumeric characters ",
+            type=cls._validate_secret,
+            default=None,
+        )
+        parser.add_argument(
+            '--custom-header',
+            action='append',
+            help=
+            "Custom header to be sent with the notification. Can be used multiple times to set multiple headers. Format: HEADER_NAME=VALUE"
+        )
+        parser.add_argument(
+            '--enable',
+            action='store_true',
+            help="Flag to enable the notification rule",
+            default=None
+        )
+        parser.add_argument(
+            '--disable',
+            action='store_false',
+            help="Flag to disable the notification rule",
+            dest='enable'
+        )
+
+    def get_rule_from_args(self, args):
+        custom_headers = None
+        if args.custom_header is not None:
+            custom_headers = {}
+            for header in args.custom_header:
+                try:
+                    name, value = header.split('=', 1)
+                except ValueError:
+                    name, value = header, ''
+                custom_headers[name] = value
+
+        rule = {
+            'name': args.ruleName,
+            'eventTypes': args.event_type,
+            'isEnabled': args.enable,
+            'objectNamePrefix': args.B2_URI.path,
+            'targetConfiguration':
+                {
+                    'url': args.webhook_url,
+                    'customHeaders': custom_headers,
+                    'hmacSha256SigningSecret': args.sign_secret,
+                },
+        }
+        return filter_out_empty_values(rule)
+
+    def print_rule(self, args, rule):
+        if args.json:
+            self._print_json(rule)
+        else:
+            self._print_human_readable_structure(rule)
+
+
+class BucketNotificationRuleUpdateBase(BucketNotificationRuleCreateBase):
+    def _run(self, args):
+        bucket = self.api.get_bucket_by_name(args.B2_URI.bucket_name)
+        rules_by_name = {rule["name"]: rule for rule in bucket.get_notification_rules()}
+        rule = rules_by_name.get(args.ruleName)
+        if not rule:
+            raise CommandError(
+                f'rule with name {args.ruleName!r} does not exist on bucket {bucket.name!r}, '
+                f'available rules: {sorted(rules_by_name)}'
+            )
+
+        rules_by_name[args.ruleName] = override_dict(
+            rule,
+            self.get_rule_from_args(args),
+        )
+
+        rules = bucket.set_notification_rules(
+            [notification_rule_response_to_request(rule) for rule in rules_by_name.values()]
+        )
+        rule = next(rule for rule in rules if rule["name"] == args.ruleName)
+        self.print_rule(args=args, rule=rule)
+        return 0
+
+
+@BucketNotificationRuleBase.subcommands_registry.register
+class BucketNotificationRuleCreate(BucketNotificationRuleCreateBase):
+    """
+    Allows creating bucket notification rules for the given bucket.
+
+    {BucketNotificationRuleWarningMixin}
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} notification-rule create b2://bucketName/optionalSubPath/ ruleName --event-type "b2:ObjectCreated:*" --webhook-url https://example.com/webhook
+
+
+    Requires capability:
+
+    - **readBucketNotifications**
+    - **writeBucketNotifications**
+    """
+    COMMAND_NAME = 'create'
+
+    NEW_RULE_DEFAULTS = {
+        'isEnabled': True,
+        'objectNamePrefix': '',
+        'targetConfiguration': {
+            'targetType': 'webhook',
+        },
+    }
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        cls.setup_rule_fields_parser(parser, creation=True)
+        super()._setup_parser(parser)
+
+    def _run(self, args):
+        bucket = self.api.get_bucket_by_name(args.B2_URI.bucket_name)
+        rules_by_name = {rule["name"]: rule for rule in bucket.get_notification_rules()}
+        if args.ruleName in rules_by_name:
+            raise CommandError(
+                f'rule with name {args.ruleName!r} already exists on bucket {bucket.name!r}'
+            )
+
+        rule = override_dict(
+            self.NEW_RULE_DEFAULTS,
+            self.get_rule_from_args(args),
+        )
+        rules_by_name[args.ruleName] = rule
+
+        rules = bucket.set_notification_rules(
+            [
+                notification_rule_response_to_request(rule)
+                for rule in sorted(rules_by_name.values(), key=lambda r: r["name"])
+            ]
+        )
+        rule = next(rule for rule in rules if rule["name"] == args.ruleName)
+        self.print_rule(args=args, rule=rule)
+        return 0
+
+
+@BucketNotificationRuleBase.subcommands_registry.register
+class BucketNotificationRuleUpdate(BucketNotificationRuleUpdateBase):
+    """
+    Allows updating notification rule of the given bucket.
+
+    {BucketNotificationRuleWarningMixin}
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} notification-rule update b2://bucketName/newPath/ ruleName --disable --event-type "b2:ObjectCreated:*" --event-type "b2:ObjectHidden:*"
+        {NAME} notification-rule update b2://bucketName/newPath/ ruleName --enable
+
+
+    Requires capability:
+
+    - **readBucketNotifications**
+    - **writeBucketNotifications**
+    """
+
+    COMMAND_NAME = 'update'
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        cls.setup_rule_fields_parser(parser, creation=False)
+        super()._setup_parser(parser)
+
+
+@BucketNotificationRuleBase.subcommands_registry.register
+class BucketNotificationRuleEnable(BucketNotificationRuleUpdateBase):
+    """
+    Allows enabling notification rule of the given bucket.
+
+    {BucketNotificationRuleWarningMixin}
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} notification-rule enable b2://bucketName/ ruleName
+
+
+    Requires capability:
+
+    - **readBucketNotifications**
+    - **writeBucketNotifications**
+    """
+
+    COMMAND_NAME = 'enable'
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_b2_uri_argument(
+            parser, help="B2 URI of the bucket to enable the rule for, e.g. b2://bucketName"
+        )
+        parser.add_argument('ruleName', help="Name of the rule to enable")
+        super()._setup_parser(parser)
+
+    def get_rule_from_args(self, args):
+        logger.warning("WARNING: ignoring path from %r", args.B2_URI)
+        return {'name': args.ruleName, 'isEnabled': True}
+
+
+@BucketNotificationRuleBase.subcommands_registry.register
+class BucketNotificationRuleDisable(BucketNotificationRuleUpdateBase):
+    """
+    Allows disabling notification rule of the given bucket.
+
+    {BucketNotificationRuleWarningMixin}
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} notification-rule disable b2://bucketName/ ruleName
+
+
+    Requires capability:
+
+    - **readBucketNotifications**
+    - **writeBucketNotifications**
+    """
+
+    COMMAND_NAME = 'disable'
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_b2_uri_argument(
+            parser, help="B2 URI of the bucket to enable the rule for, e.g. b2://bucketName"
+        )
+        parser.add_argument('ruleName', help="Name of the rule to enable")
+        super()._setup_parser(parser)
+
+    def get_rule_from_args(self, args):
+        logger.warning("WARNING: ignoring path from %r", args.B2_URI)
+        return {'name': args.ruleName, 'isEnabled': False}
+
+
+@BucketNotificationRuleBase.subcommands_registry.register
+class BucketNotificationRuleDelete(Command):
+    """
+    Allows deleting bucket notification rule of the given bucket.
+
+    Requires capability:
+
+    - **readBucketNotifications**
+    - **writeBucketNotifications**
+    """
+
+    COMMAND_NAME = 'delete'
+
+    @classmethod
+    def _setup_parser(cls, parser):
+        add_b2_uri_argument(
+            parser, help="B2 URI of the bucket to delete the rule from, e.g. b2://bucketName"
+        )
+        parser.add_argument('ruleName', help="Name of the rule to delete")
+        super()._setup_parser(parser)
+
+    def _run(self, args):
+        bucket = self.api.get_bucket_by_name(args.B2_URI.bucket_name)
+        rules_by_name = {rule["name"]: rule for rule in bucket.get_notification_rules()}
+
+        try:
+            del rules_by_name[args.ruleName]
+        except KeyError:
+            raise CommandError(
+                f'no such rule to delete: {args.ruleName!r}, '
+                f'available rules: {sorted(rules_by_name.keys())!r}; No rules have been deleted.'
+            )
+        bucket.set_notification_rules(
+            [notification_rule_response_to_request(rule) for rule in rules_by_name.values()]
+        )
+        self._print(f'Rule {args.ruleName!r} has been deleted from {args.B2_URI}')
+        return 0
+
+
+class Key(Command):
+    """
+    Application keys management subcommands.
+
+    For more information on each subcommand, use ``{NAME} key SUBCOMMAND --help``.
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} key list
+        {NAME} key create my-key listFiles,deleteFiles
+        {NAME} key delete 005c398ac3212400000000010
+    """
+    subcommands_registry = ClassRegistry(attr_name='COMMAND_NAME')
+
+
+@Key.subcommands_registry.register
+class KeyListSubcommand(KeyListBase):
+    __doc__ = KeyListBase.__doc__
+    COMMAND_NAME = 'list'
+
+
+@Key.subcommands_registry.register
+class KeyCreateSubcommand(KeyCreateBase):
+    __doc__ = KeyCreateBase.__doc__
+    COMMAND_NAME = 'create'
+
+
+@Key.subcommands_registry.register
+class KeyDeleteSubcommand(KeyDeleteBase):
+    __doc__ = KeyDeleteBase.__doc__
+    COMMAND_NAME = 'delete'
+
+
+class ListKeys(CmdReplacedByMixin, KeyListBase):
+    __doc__ = KeyListBase.__doc__
+    replaced_by_cmd = (Key, KeyListSubcommand)
+
+
+class CreateKey(CmdReplacedByMixin, KeyCreateBase):
+    __doc__ = KeyCreateBase.__doc__
+    replaced_by_cmd = (Key, KeyCreateSubcommand)
+
+
+class DeleteKey(CmdReplacedByMixin, KeyDeleteBase):
+    __doc__ = KeyDeleteBase.__doc__
+    replaced_by_cmd = (Key, KeyDeleteSubcommand)
+
+
+class Replication(Command):
+    """
+    Replication rule management subcommands.
+
+    For more information on each subcommand, use ``{NAME} replication SUBCOMMAND --help``.
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} replication setup --name=my-repl-rule src-bucket dest-bucket
+        {NAME} replication status --rule=my-repl-rule src-bucket
+        {NAME} replication pause src-bucket my-repl-rule
+        {NAME} replication unpause src-bucket my-repl-rule
+        {NAME} replication delete src-bucket my-repl-rule
+    """
+    subcommands_registry = ClassRegistry(attr_name='COMMAND_NAME')
+
+
+@Replication.subcommands_registry.register
+class ReplicationSetupSubcommand(ReplicationSetupBase):
+    __doc__ = ReplicationSetupBase.__doc__
+    COMMAND_NAME = 'setup'
+
+
+@Replication.subcommands_registry.register
+class ReplicationStatusSubcommand(ReplicationStatusBase):
+    __doc__ = ReplicationStatusBase.__doc__
+    COMMAND_NAME = 'status'
+
+
+@Replication.subcommands_registry.register
+class ReplicationPauseSubcommand(ReplicationPauseBase):
+    __doc__ = ReplicationPauseBase.__doc__
+    COMMAND_NAME = 'pause'
+
+
+@Replication.subcommands_registry.register
+class ReplicationUnpauseSubcommand(ReplicationUnpauseBase):
+    __doc__ = ReplicationUnpauseBase.__doc__
+    COMMAND_NAME = 'unpause'
+
+
+@Replication.subcommands_registry.register
+class ReplicationDeleteSubcommand(ReplicationDeleteBase):
+    __doc__ = ReplicationDeleteBase.__doc__
+    COMMAND_NAME = 'delete'
+
+
+class ReplicationSetup(CmdReplacedByMixin, ReplicationSetupBase):
+    __doc__ = ReplicationSetupBase.__doc__
+    replaced_by_cmd = (Replication, ReplicationSetupSubcommand)
+
+
+class ReplicationStatus(CmdReplacedByMixin, ReplicationStatusBase):
+    __doc__ = ReplicationStatusBase.__doc__
+    replaced_by_cmd = (Replication, ReplicationStatusSubcommand)
+
+
+class ReplicationPause(CmdReplacedByMixin, ReplicationPauseBase):
+    __doc__ = ReplicationPauseBase.__doc__
+    replaced_by_cmd = (Replication, ReplicationPauseSubcommand)
+
+
+class ReplicationUnpause(CmdReplacedByMixin, ReplicationUnpauseBase):
+    __doc__ = ReplicationUnpauseBase.__doc__
+    replaced_by_cmd = (Replication, ReplicationUnpauseSubcommand)
+
+
+class ReplicationDelete(CmdReplacedByMixin, ReplicationDeleteBase):
+    __doc__ = ReplicationDeleteBase.__doc__
+    replaced_by_cmd = (Replication, ReplicationDeleteSubcommand)
+
+
+class Account(Command):
+    """
+    Account management subcommands.
+
+    For more information on each subcommand, use ``{NAME} account SUBCOMMAND --help``.
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} account authorize [applicationKeyId] [applicationKey]
+        {NAME} account get
+        {NAME} account clear
+    """
+    subcommands_registry = ClassRegistry(attr_name='COMMAND_NAME')
+
+
+@Account.subcommands_registry.register
+class AccountAuthorize(AccountAuthorizeBase):
+    __doc__ = AccountAuthorizeBase.__doc__
+    COMMAND_NAME = 'authorize'
+
+
+@Account.subcommands_registry.register
+class AccountGet(AccountGetBase):
+    __doc__ = AccountGetBase.__doc__
+    COMMAND_NAME = 'get'
+
+
+@Account.subcommands_registry.register
+class AccountClear(AccountClearBase):
+    __doc__ = AccountClearBase.__doc__
+    COMMAND_NAME = 'clear'
+
+
+class AuthorizeAccount(CmdReplacedByMixin, AccountAuthorizeBase):
+    __doc__ = AccountAuthorizeBase.__doc__
+    replaced_by_cmd = (Account, AccountAuthorize)
+
+
+class GetAccountInfo(CmdReplacedByMixin, AccountGetBase):
+    __doc__ = AccountGetBase.__doc__
+    replaced_by_cmd = (Account, AccountGet)
+
+
+class ClearAccount(CmdReplacedByMixin, AccountClearBase):
+    __doc__ = AccountClearBase.__doc__
+    replaced_by_cmd = (Account, AccountClear)
+
+
+class BucketCmd(Command):
+    """
+    Bucket management subcommands.
+
+    For more information on each subcommand, use ``{NAME} bucket SUBCOMMAND --help``.
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} bucket list
+        {NAME} bucket get
+        {NAME} bucket create
+        {NAME} bucket update
+        {NAME} bucket delete
+        {NAME} bucket get-download-auth
+    """
+    # to avoid conflicts with the Bucket class this class is named BucketCmd
+    COMMAND_NAME = "bucket"
+
+    subcommands_registry = ClassRegistry(attr_name='COMMAND_NAME')
+
+
+@BucketCmd.subcommands_registry.register
+class BucketList(BucketListBase):
+    __doc__ = BucketListBase.__doc__
+    COMMAND_NAME = 'list'
+
+
+@BucketCmd.subcommands_registry.register
+class BucketGet(BucketGetBase):
+    __doc__ = BucketGetBase.__doc__
+    COMMAND_NAME = 'get'
+
+
+@BucketCmd.subcommands_registry.register
+class BucketCreate(BucketCreateBase):
+    __doc__ = BucketCreateBase.__doc__
+    COMMAND_NAME = 'create'
+
+
+@BucketCmd.subcommands_registry.register
+class BucketUpdate(BucketUpdateBase):
+    __doc__ = BucketUpdateBase.__doc__
+    COMMAND_NAME = 'update'
+
+
+@BucketCmd.subcommands_registry.register
+class BucketDelete(BucketDeleteBase):
+    __doc__ = BucketDeleteBase.__doc__
+    COMMAND_NAME = 'delete'
+
+
+@BucketCmd.subcommands_registry.register
+class BucketGetDownloadAuth(BucketGetDownloadAuthBase):
+    __doc__ = BucketGetDownloadAuthBase.__doc__
+    COMMAND_NAME = 'get-download-auth'
+
+
+@BucketCmd.subcommands_registry.register
+class BucketNotificationRule(BucketNotificationRuleBase):
+    __doc__ = BucketNotificationRuleBase.__doc__
+    COMMAND_NAME = 'notification-rule'
+
+
+class ListBuckets(CmdReplacedByMixin, BucketListBase):
+    __doc__ = BucketListBase.__doc__
+    replaced_by_cmd = (BucketCmd, BucketList)
+
+
+class GetBucket(CmdReplacedByMixin, BucketGetBase):
+    __doc__ = BucketGetBase.__doc__
+    replaced_by_cmd = (BucketCmd, BucketGet)
+
+
+class CreateBucket(CmdReplacedByMixin, BucketCreateBase):
+    __doc__ = BucketCreateBase.__doc__
+    replaced_by_cmd = (BucketCmd, BucketCreate)
+
+
+class UpdateBucket(CmdReplacedByMixin, BucketUpdateBase):
+    __doc__ = BucketUpdateBase.__doc__
+    replaced_by_cmd = (BucketCmd, BucketUpdate)
+
+
+class DeleteBucket(CmdReplacedByMixin, BucketDeleteBase):
+    __doc__ = BucketDeleteBase.__doc__
+    replaced_by_cmd = (BucketCmd, BucketDelete)
+
+
+class GetDownloadAuth(CmdReplacedByMixin, BucketGetDownloadAuthBase):
+    __doc__ = BucketGetDownloadAuthBase.__doc__
+    replaced_by_cmd = (BucketCmd, BucketGetDownloadAuth)
+
+
+class NotificationRules(CmdReplacedByMixin, BucketNotificationRuleBase):
+    __doc__ = BucketNotificationRuleBase.__doc__
+    replaced_by_cmd = (BucketCmd, BucketNotificationRule)
+
+
+class File(Command):
+    """
+    File management subcommands.
+
+    For more information on each subcommand, use ``{NAME} file SUBCOMMAND --help``.
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} file cat b2://yourBucket/file.txt
+        {NAME} file copy-by-id sourceFileId yourBucket file.txt
+        {NAME} file download b2://yourBucket/file.txt localFile.txt
+        {NAME} file hide yourBucket file.txt
+        {NAME} file info b2://yourBucket/file.txt
+        {NAME} file update --legal-hold off b2://yourBucket/file.txt
+        {NAME} file upload yourBucket localFile.txt file.txt
+        {NAME} file url b2://yourBucket/file.txt
+    """
+    subcommands_registry = ClassRegistry(attr_name='COMMAND_NAME')
+
+
+@File.subcommands_registry.register
+class FileInfo(B2URIFileArgMixin, FileInfoBase):
+    __doc__ = FileInfoBase.__doc__
+    COMMAND_NAME = 'info'
+
+
+@File.subcommands_registry.register
+class FileUrl(B2URIFileArgMixin, FileUrlBase):
+    __doc__ = FileUrlBase.__doc__
+    COMMAND_NAME = 'url'
+
+
+@File.subcommands_registry.register
+class FileCat(FileCatBase):
+    __doc__ = FileCatBase.__doc__
+    COMMAND_NAME = 'cat'
+
+
+@File.subcommands_registry.register
+class FileUpload(FileUploadBase):
+    __doc__ = FileUploadBase.__doc__
+    COMMAND_NAME = 'upload'
+
+
+@File.subcommands_registry.register
+class FileDownload(B2URIFileArgMixin, FileDownloadBase):
+    __doc__ = FileDownloadBase.__doc__
+    COMMAND_NAME = 'download'
+
+
+@File.subcommands_registry.register
+class FileCopyById(FileCopyByIdBase):
+    __doc__ = FileCopyByIdBase.__doc__
+    COMMAND_NAME = 'copy-by-id'
+
+
+@File.subcommands_registry.register
+class FileHide(FileHideBase):
+    __doc__ = FileHideBase.__doc__
+    COMMAND_NAME = 'hide'
+
+
+@File.subcommands_registry.register
+class FileUpdate(FileUpdateBase):
+    __doc__ = FileUpdateBase.__doc__
+    COMMAND_NAME = 'update'
+
+
+class FileInfo2(CmdReplacedByMixin, B2URIFileArgMixin, FileInfoBase):
+    __doc__ = FileInfoBase.__doc__
+    replaced_by_cmd = (File, FileInfo)
+    COMMAND_NAME = 'file-info'
+
+
+class GetFileInfo(CmdReplacedByMixin, B2URIFileIDArgMixin, FileInfoBase):
+    __doc__ = FileInfoBase.__doc__
+    replaced_by_cmd = (File, FileInfo)
+
+
+class GetUrl(CmdReplacedByMixin, B2URIFileArgMixin, FileUrlBase):
+    __doc__ = FileUrlBase.__doc__
+    replaced_by_cmd = (File, FileUrl)
+
+
+class MakeUrl(CmdReplacedByMixin, B2URIFileIDArgMixin, FileUrlBase):
+    __doc__ = FileUrlBase.__doc__
+    replaced_by_cmd = (File, FileUrl)
+
+
+class MakeFriendlyUrl(CmdReplacedByMixin, B2URIBucketNFilenameArgMixin, FileUrlBase):
+    __doc__ = FileUrlBase.__doc__
+    replaced_by_cmd = (File, FileUrl)
+
+
+class Cat(CmdReplacedByMixin, FileCatBase):
+    __doc__ = FileCatBase.__doc__
+    replaced_by_cmd = (File, FileCat)
+
+
+class UploadFile(CmdReplacedByMixin, FileUploadBase):
+    __doc__ = FileUploadBase.__doc__
+    replaced_by_cmd = (File, FileUpload)
+
+
+class UploadUnboundStream(CmdReplacedByMixin, UploadUnboundStreamBase):
+    __doc__ = UploadUnboundStreamBase.__doc__
+    replaced_by_cmd = (File, FileUpload)
+
+
+class DownloadFile(CmdReplacedByMixin, B2URIFileArgMixin, FileDownloadBase):
+    __doc__ = FileDownloadBase.__doc__
+    replaced_by_cmd = (File, FileDownload)
+
+
+class DownloadFileById(CmdReplacedByMixin, B2URIFileIDArgMixin, FileDownloadBase):
+    __doc__ = FileDownloadBase.__doc__
+    replaced_by_cmd = (File, FileDownload)
+
+
+class DownloadFileByName(CmdReplacedByMixin, B2URIBucketNFilenameArgMixin, FileDownloadBase):
+    __doc__ = FileDownloadBase.__doc__
+    replaced_by_cmd = (File, FileDownload)
+
+
+class CopyFileById(CmdReplacedByMixin, FileCopyByIdBase):
+    __doc__ = FileCopyByIdBase.__doc__
+    replaced_by_cmd = (File, FileCopyById)
+
+
+class HideFile(CmdReplacedByMixin, FileHideBase):
+    __doc__ = FileHideBase.__doc__
+    replaced_by_cmd = (File, FileHide)
+
+
+class UpdateFileLegalHold(CmdReplacedByMixin, UpdateFileLegalHoldBase):
+    __doc__ = UpdateFileLegalHoldBase.__doc__
+    replaced_by_cmd = (File, FileUpdate)
+
+
+class UpdateFileRetention(CmdReplacedByMixin, UpdateFileRetentionBase):
+    __doc__ = UpdateFileRetentionBase.__doc__
+    replaced_by_cmd = (File, FileUpdate)
+
+
+class GetDownloadUrlWithAuth(CmdReplacedByMixin, GetDownloadUrlWithAuthBase):
+    __doc__ = GetDownloadUrlWithAuthBase.__doc__
+    replaced_by_cmd = (File, FileUrl)
+
+
+class DeleteFileVersion(CmdReplacedByMixin, DeleteFileVersionBase):
+    __doc__ = DeleteFileVersionBase.__doc__
+    replaced_by_cmd = Rm
+
+
+@File.subcommands_registry.register
+class FileLarge(Command):
+    """
+    Large file uploads management subcommands.
+
+    For more information on each subcommand, use ``{NAME} file large SUBCOMMAND --help``.
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} file large parts b2id://yourFileId
+        {NAME} file large unfinished list b2://yourBucket
+        {NAME} file large unfinished cancel b2://yourBucket
+        {NAME} file large unfinished cancel b2id://yourFileId
+    """
+    COMMAND_NAME = 'large'
+    subcommands_registry = ClassRegistry(attr_name='COMMAND_NAME')
+
+
+@FileLarge.subcommands_registry.register
+class FileLargeParts(B2IDURIMixin, FileLargePartsBase):
+    __doc__ = FileLargePartsBase.__doc__
+    COMMAND_NAME = 'parts'
+
+
+@FileLarge.subcommands_registry.register
+class FileLargeUnfinished(Command):
+    """
+    Large file unfinished uploads management subcommands.
+
+    For more information on each subcommand, use ``{NAME} file large unfinished SUBCOMMAND --help``.
+
+    Examples:
+
+    .. code-block::
+
+        {NAME} file large unfinished list b2://yourBucket
+        {NAME} file large unfinished cancel b2://yourBucket
+        {NAME} file large unfinished cancel b2id://yourFileId
+    """
+    COMMAND_NAME = 'unfinished'
+    subcommands_registry = ClassRegistry(attr_name='COMMAND_NAME')
+
+
+@FileLargeUnfinished.subcommands_registry.register
+class FileLargeUnfinishedList(B2BucketURIMixin, FileLargeUnfinishedListBase):
+    __doc__ = FileLargePartsBase.__doc__
+    COMMAND_NAME = 'list'
+
+
+@FileLargeUnfinished.subcommands_registry.register
+class FileLargeUnfinishedCancel(B2IDOrB2BucketURIMixin, FileLargeUnfinishedCancelBase):
+    __doc__ = FileLargeUnfinishedCancelBase.__doc__
+    COMMAND_NAME = 'cancel'
+
+
+class ListParts(CmdReplacedByMixin, B2URIFileIDArgMixin, FileLargePartsBase):
+    __doc__ = FileLargePartsBase.__doc__
+    replaced_by_cmd = (File, FileLarge, FileLargeParts)
+
+
+class ListUnfinishedLargeFiles(
+    CmdReplacedByMixin, B2URIBucketArgMixin, FileLargeUnfinishedListBase
+):
+    __doc__ = FileLargeUnfinishedListBase.__doc__
+    replaced_by_cmd = (File, FileLarge, FileLargeUnfinished, FileLargeUnfinishedList)
+
+
+class CancelAllUnfinishedLargeFiles(
+    CmdReplacedByMixin, B2URIBucketArgMixin, FileLargeUnfinishedCancelBase
+):
+    """
+    Lists all large files that have been started but not
+    finished and cancels them.  Any parts that have been
+    uploaded will be deleted.
+
+    Requires capability:
+
+    - **listFiles**
+    - **writeFiles**
+    """
+    replaced_by_cmd = (File, FileLarge, FileLargeUnfinished, FileLargeUnfinishedCancel)
+
+
+class CancelLargeFile(CmdReplacedByMixin, B2URIFileIDArgMixin, FileLargeUnfinishedCancelBase):
+    """
+    Cancels a large file upload.  Used to undo a ``start-large-file``.
+
+    Cannot be used once the file is finished.  After finishing,
+    using ``delete-file-version`` to delete the large file.
+
+    Requires capability:
+
+    - **writeFiles**
+    """
+    replaced_by_cmd = (File, FileLarge, FileLargeUnfinished, FileLargeUnfinishedCancel)
+
+
+class ConsoleTool:
     """
     Implements the commands available in the B2 command-line tool
     using the B2Api library.
 
-    Uses a ``b2sdk.SqlitedAccountInfo`` object to keep account data between runs.
+    Uses a ``b2sdk.SqlitedAccountInfo`` object to keep account data between runs
+    (unless authorization is performed via environment variables).
     """
 
-    def __init__(self, b2_api: Optional[B2Api], stdout, stderr):
-        self.api = b2_api
+    def __init__(self, stdout, stderr):
         self.stdout = stdout
         self.stderr = stderr
+        self.b2_binary_name = 'b2'
+
+    def _get_default_escape_cc_setting(self):
+        escape_cc_env_var = os.environ.get(B2_ESCAPE_CONTROL_CHARACTERS, None)
+        if escape_cc_env_var is not None:
+            if int(escape_cc_env_var) in (0, 1):
+                return int(escape_cc_env_var) == 1
+            else:
+                logger.warning(
+                    "WARNING: invalid value for {B2_ESCAPE_CONTROL_CHARACTERS} environment variable, available options are 0 or 1 - will assume variable is not set"
+                )
+        return self.stdout.isatty()
 
     def run_command(self, argv):
         signal.signal(signal.SIGINT, keyboard_interrupt_handler)
-        parser = B2.get_parser()
-        argcomplete.autocomplete(parser)
+        self.b2_binary_name = resolve_b2_bin_call_name(argv)
+        parser = B2.create_parser(name=self.b2_binary_name, b2_binary_name=self.b2_binary_name)
+        AUTOCOMPLETE.cache_and_autocomplete(parser)
         args = parser.parse_args(argv[1:])
         self._setup_logging(args, argv)
 
-        if self.api:
-            if (
-                args.profile or getattr(args, 'write_buffer_size', None) or
-                getattr(args, 'skip_hash_verification', None) or
-                getattr(args, 'max_download_streams_per_file', None)
-            ):
-                self._print_stderr(
-                    'ERROR: cannot change configuration on already initialized object'
-                )
-                return 1
-
-        else:
-            kwargs = {
-                'profile': args.profile,
-            }
-
-            if 'write_buffer_size' in args:
-                kwargs['save_to_buffer_size'] = args.write_buffer_size
+        if args.escape_control_characters is None:
+            args.escape_control_characters = self._get_default_escape_cc_setting()
 
-            if 'skip_hash_verification' in args:
-                kwargs['check_download_hash'] = not args.skip_hash_verification
+        if args.escape_control_characters:
+            # in case any control characters slip through escaping, just delete them
+            self.stdout = NoControlCharactersStdout(self.stdout)
+            self.stderr = NoControlCharactersStdout(self.stderr)
 
-            if 'max_download_streams_per_file' in args:
-                kwargs['max_download_streams_per_file'] = args.max_download_streams_per_file
+        kwargs = {}
+        with suppress(AttributeError):
+            kwargs['save_to_buffer_size'] = args.write_buffer_size
+        with suppress(AttributeError):
+            kwargs['check_download_hash'] = not args.skip_hash_verification
+        with suppress(AttributeError):
+            kwargs['max_download_streams_per_file'] = args.max_download_streams_per_file
 
-            self.api = _get_b2api_for_profile(**kwargs)
+        self.api = self._initialize_b2_api(args=args, kwargs=kwargs)
 
         b2_command = B2(self)
         command_class = b2_command.run(args)
         command = command_class(self)
 
         if command.FORBID_LOGGING_ARGUMENTS:
             logger.info('starting command [%s] (arguments hidden)', command)
         else:
             logger.info('starting command [%s] with arguments: %s', command, argv)
 
         try:
-            auth_ret = self.authorize_from_env(command_class)
-            if auth_ret:
-                return auth_ret
+            if command_class.REQUIRES_AUTH:
+                auth_ret = self.authorize_from_env()
+                if auth_ret:
+                    return auth_ret
             return command.run(args)
         except MissingAccountData as e:
             logger.exception('ConsoleTool missing account data error')
             self._print_stderr(
-                'ERROR: %s  Use: %s authorize-account or provide auth data with "%s" and "%s"'
-                ' environment variables' %
-                (str(e), NAME, B2_APPLICATION_KEY_ID_ENV_VAR, B2_APPLICATION_KEY_ENV_VAR)
+                f'ERROR: {e}  Use: \'{self.b2_binary_name} account authorize\' or provide auth data with '
+                f'{B2_APPLICATION_KEY_ID_ENV_VAR!r} and {B2_APPLICATION_KEY_ENV_VAR!r} environment variables'
             )
             return 1
         except B2Error as e:
             logger.exception('ConsoleTool command error')
-            self._print_stderr('ERROR: %s' % (str(e),))
+            self._print_stderr(f'ERROR: {e}')
             return 1
         except KeyboardInterrupt:
             logger.exception('ConsoleTool command interrupt')
             self._print_stderr('\nInterrupted.  Shutting down...\n')
             return 1
         except Exception:
             logger.exception('ConsoleTool unexpected exception')
             raise
 
-    def authorize_from_env(self, command_class):
-        if not command_class.REQUIRES_AUTH:
-            return 0
+    @classmethod
+    def _initialize_b2_api(cls, args: argparse.Namespace, kwargs: dict) -> B2Api:
+        b2_api = None
+        key_id, key = get_keyid_and_key_from_env_vars()
+        if key_id and key:
+            try:
+                # here we initialize regular b2 api on disk and check whether it matches
+                # the keys from env vars; if they indeed match then there's no need to
+                # initialize in-memory account info cause it's already stored on disk
+                b2_api = _get_b2api_for_profile(
+                    profile=args.profile, raise_if_does_not_exist=True, **kwargs
+                )
+                realm = os.environ.get(B2_ENVIRONMENT_ENV_VAR) or 'production'
+                is_same_key_on_disk = b2_api.account_info.is_same_key(key_id, realm)
+            except MissingAccountData:
+                is_same_key_on_disk = False
+
+            if not is_same_key_on_disk and not issubclass(
+                args.command_class, (AccountAuthorizeBase, AccountClearBase)
+            ):
+                # when user specifies keys via env variables, we switch to in-memory account info
+                return _get_inmemory_b2api(**kwargs)
 
-        key_id = os.environ.get(B2_APPLICATION_KEY_ID_ENV_VAR)
-        key = os.environ.get(B2_APPLICATION_KEY_ENV_VAR)
+        return b2_api or _get_b2api_for_profile(profile=args.profile, **kwargs)
+
+    def authorize_from_env(self) -> int:
+
+        key_id, key = get_keyid_and_key_from_env_vars()
 
         if key_id is None and key is None:
             return 0
 
         if (key_id is None) or (key is None):
             self._print_stderr(
-                'Please provide both "%s" and "%s" environment variables or none of them' %
-                (B2_APPLICATION_KEY_ENV_VAR, B2_APPLICATION_KEY_ID_ENV_VAR)
+                f'Please provide both "{B2_APPLICATION_KEY_ENV_VAR}" and "{B2_APPLICATION_KEY_ID_ENV_VAR}" environment variables or none of them'
             )
             return 1
-        realm = os.environ.get(B2_ENVIRONMENT_ENV_VAR, 'production')
+        realm = os.environ.get(B2_ENVIRONMENT_ENV_VAR)
 
-        if self.api.account_info.is_same_key(key_id, realm):
+        if self.api.account_info.is_same_key(key_id, realm or 'production'):
             return 0
 
-        logger.info('authorize-account is being run from env variables')
-        return AuthorizeAccount(self).authorize(key_id, key, realm)
+        logger.info('`account authorize` is being run from env variables')
+        return AccountAuthorizeBase(self).authorize(key_id, key, realm)
 
     def _print(self, *args, **kwargs):
         print(*args, file=self.stdout, **kwargs)
 
     def _print_stderr(self, *args, **kwargs):
         print(*args, file=self.stderr, **kwargs)
 
     @classmethod
     def _setup_logging(cls, args, argv):
-        if args.logConfig and (args.verbose or args.debugLogs):
-            raise ValueError('Please provide either --logConfig or --verbose/--debugLogs')
-        if args.logConfig:
-            logging.config.fileConfig(args.logConfig)
-        elif args.verbose or args.debugLogs:
+        if args.log_config and (args.verbose or args.debug_logs):
+            raise ValueError('Please provide either --log-config or --verbose/--debug-logs')
+        errors_kwarg = {'errors': 'backslashreplace'} if sys.version_info >= (3, 9) else {}
+        if args.log_config:
+            logging.config.fileConfig(args.log_config)
+        elif args.verbose or args.debug_logs:
             # set log level to DEBUG for ALL loggers (even those not belonging to B2), but without any handlers,
             # those will added as needed (file and/or stderr)
-            logging.basicConfig(level=logging.DEBUG, handlers=[])
+            logging.basicConfig(level=logging.DEBUG, handlers=[], **errors_kwarg)
         else:
             logger.setLevel(logging.CRITICAL + 1)  # No logs!
         if args.verbose:
             formatter = logging.Formatter('%(levelname)s:%(name)s:%(message)s')
             handler = logging.StreamHandler()
             handler.setFormatter(formatter)
 
             # logs from ALL loggers sent to stderr should be formatted this way
             logging.root.addHandler(handler)
-        if args.debugLogs:
+        if args.debug_logs:
             formatter = logging.Formatter(
                 '%(asctime)s\t%(process)d\t%(thread)d\t%(name)s\t%(levelname)s\t%(message)s'
             )
             formatter.converter = time.gmtime
-            handler = logging.FileHandler('b2_cli.log')
+            handler = logging.FileHandler('b2_cli.log', **errors_kwarg)
             handler.setFormatter(formatter)
 
             # logs from ALL loggers sent to the log file should be formatted this way
             logging.root.addHandler(handler)
+        if not args.debug_logs and not args.verbose:
+            warnings.showwarning = lambda message, category, *arg_, **_: print(
+                f'{category.__name__}: {message}', file=sys.stderr
+            )
 
         logger.info(r'// %s %s %s \\', SEPARATOR, VERSION.center(8), SEPARATOR)
         logger.debug('platform is %s', platform.platform())
+        if os.environ.get(B2_CLI_DOCKER_ENV_VAR) == "1":
+            logger.debug('running as a Docker container')
         logger.debug(
             'Python version is %s %s', platform.python_implementation(),
             sys.version.replace('\n', ' ')
         )
         logger.debug('b2sdk version is %s', b2sdk_version)
         logger.debug('locale is %s', locale.getlocale())
         logger.debug('filesystem encoding is %s', sys.getfilesystemencoding())
+        logger.debug('default encoding is %s', sys.getdefaultencoding())
+        logger.debug('flags.utf8_mode is %s', sys.flags.utf8_mode)
 
 
 # used by Sphinx
-get_parser = functools.partial(B2.get_parser, for_docs=True)
-
-
-# TODO: import from b2sdk as soon as we rely on 1.0.0
-class InvalidArgument(B2Error):
-    """
-    Raised when one or more arguments are invalid
-    """
-
-    def __init__(self, parameter_name, message):
-        """
-        :param parameter_name: name of the function argument
-        :param message: brief explanation of misconfiguration
-        """
-        super(InvalidArgument, self).__init__()
-        self.parameter_name = parameter_name
-        self.message = message
-
-    def __str__(self):
-        return "%s %s" % (self.parameter_name, self.message)
+get_parser = functools.partial(B2.create_parser, for_docs=True)
 
 
 def main():
-    ct = ConsoleTool(b2_api=None, stdout=sys.stdout, stderr=sys.stderr)
+    ct = ConsoleTool(stdout=sys.stdout, stderr=sys.stderr)
     exit_status = ct.run_command(sys.argv)
     logger.info('\\\\ %s %s %s //', SEPARATOR, ('exit=%s' % exit_status).center(8), SEPARATOR)
 
     # I haven't tracked down the root cause yet, but in Python 2.7, the futures
     # packages is hanging on exit sometimes, waiting for a thread to finish.
     # This happens when using sync to upload files.
     sys.stdout.flush()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `b2-3.9.0/b2/json_encoder.py` & `b2-4.0.0/b2/_internal/json_encoder.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 ######################################################################
 #
-# File: b2/json_encoder.py
+# File: b2/_internal/json_encoder.py
 #
 # Copyright 2020 Backblaze Inc. All Rights Reserved.
 #
 # License https://www.backblaze.com/using_b2_code.html
 #
 ######################################################################
 
 import json
-
 from enum import Enum
 
-from b2sdk.v2 import Bucket, FileIdAndName, FileVersion
+from b2sdk.v2 import Bucket, DownloadVersion, FileIdAndName, FileVersion
 
 
 class B2CliJsonEncoder(json.JSONEncoder):
     """
     Makes it possible to serialize b2sdk objects
     (specifically bucket['options'] set and FileVersionInfo/FileIdAndName) to json.
 
@@ -24,12 +23,12 @@
     '[1, 2, 3, "c", "b", "a"]'
     >>>
     """
 
     def default(self, obj):
         if isinstance(obj, set):
             return list(obj)
-        elif isinstance(obj, (FileVersion, FileIdAndName, Bucket)):
+        elif isinstance(obj, (DownloadVersion, FileVersion, FileIdAndName, Bucket)):
             return obj.as_dict()
         elif isinstance(obj, Enum):
             return obj.value
         return super().default(obj)
```

### Comparing `b2-3.9.0/b2/licenses_output.txt` & `b2-4.0.0/b2/licenses_output.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4417,6465 +4417,5420 @@
 00011400: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011440: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00011450: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00011460: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00011470: 2020 2020 2020 4365 7274 6966 6963 6174        Certificat
-00011480: 6520 6461 7461 2066 726f 6d20 4d6f 7a69  e data from Mozi
-00011490: 6c6c 6120 6173 206f 663a 2054 6875 204e  lla as of: Thu N
-000114a0: 6f76 2020 3320 3139 3a30 343a 3139 2032  ov  3 19:04:19 2
-000114b0: 3031 3123 2020 2020 2020 2020 2020 2020  011#            
+00011470: 2054 6869 7320 6973 2061 2062 756e 646c   This is a bundl
+00011480: 6520 6f66 2058 2e35 3039 2063 6572 7469  e of X.509 certi
+00011490: 6669 6361 7465 7320 6f66 2070 7562 6c69  ficates of publi
+000114a0: 6320 4365 7274 6966 6963 6174 6520 4175  c Certificate Au
+000114b0: 7468 6f72 6974 6965 7320 2020 2020 2020  thorities       
 000114c0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 000114d0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000114e0: 2020 2020 2020 5468 6973 2069 7320 6120        This is a 
-000114f0: 6275 6e64 6c65 206f 6620 582e 3530 3920  bundle of X.509 
-00011500: 6365 7274 6966 6963 6174 6573 206f 6620  certificates of 
-00011510: 7075 626c 6963 2043 6572 7469 6669 6361  public Certifica
-00011520: 7465 2041 7574 686f 7269 7469 6573 2020  te Authorities  
+000114e0: 2020 2020 2028 4341 292e 2054 6865 7365       (CA). These
+000114f0: 2077 6572 6520 6175 746f 6d61 7469 6361   were automatica
+00011500: 6c6c 7920 6578 7472 6163 7465 6420 6672  lly extracted fr
+00011510: 6f6d 204d 6f7a 696c 6c61 2773 2072 6f6f  om Mozilla's roo
+00011520: 7420 6365 7274 6966 6963 6174 6573 2020  t certificates  
 00011530: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00011540: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00011550: 2020 2020 2020 2020 2020 2843 4129 2e20            (CA). 
-00011560: 5468 6573 6520 7765 7265 2061 7574 6f6d  These were autom
-00011570: 6174 6963 616c 6c79 2065 7874 7261 6374  atically extract
-00011580: 6564 2066 726f 6d20 4d6f 7a69 6c6c 6127  ed from Mozilla'
-00011590: 7320 726f 6f74 2063 6572 7469 6669 6361  s root certifica
-000115a0: 7465 7320 2020 2020 2020 2020 207c 0a7c  tes          |.|
+00011550: 2020 2020 2020 2020 2020 2066 696c 6520             file 
+00011560: 2863 6572 7464 6174 612e 7478 7429 2e20  (certdata.txt). 
+00011570: 2054 6869 7320 6669 6c65 2063 616e 2062   This file can b
+00011580: 6520 666f 756e 6420 696e 2074 6865 206d  e found in the m
+00011590: 6f7a 696c 6c61 2073 6f75 7263 6520 7472  ozilla source tr
+000115a0: 6565 3a20 2020 2020 2020 2020 207c 0a7c  ee:          |.|
 000115b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000115c0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-000115d0: 6669 6c65 2028 6365 7274 6461 7461 2e74  file (certdata.t
-000115e0: 7874 292e 2020 5468 6973 2066 696c 6520  xt).  This file 
-000115f0: 6361 6e20 6265 2066 6f75 6e64 2069 6e20  can be found in 
-00011600: 7468 6520 6d6f 7a69 6c6c 6120 736f 7572  the mozilla sour
-00011610: 6365 2074 7265 653a 2020 2020 2020 2020  ce tree:        
-00011620: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00011630: 2020 2020 2020 2020 207c 2068 7474 7073           | https
-00011640: 3a2f 2f68 672e 6d6f 7a69 6c6c 612e 6f72  ://hg.mozilla.or
-00011650: 672f 6d6f 7a69 6c6c 612d 6365 6e74 7261  g/mozilla-centra
-00011660: 6c2f 6669 6c65 2f74 6970 2f73 6563 7572  l/file/tip/secur
-00011670: 6974 792f 6e73 732f 6c69 622f 636b 6677  ity/nss/lib/ckfw
-00011680: 2f62 7569 6c74 696e 732f 6365 7274 6461  /builtins/certda
-00011690: 7461 2e74 7874 207c 0a7c 2020 2020 2020  ta.txt |.|      
+000115c0: 2020 2020 7c20 6874 7470 733a 2f2f 6867      | https://hg
+000115d0: 2e6d 6f7a 696c 6c61 2e6f 7267 2f6d 6f7a  .mozilla.org/moz
+000115e0: 696c 6c61 2d63 656e 7472 616c 2f66 696c  illa-central/fil
+000115f0: 652f 7469 702f 7365 6375 7269 7479 2f6e  e/tip/security/n
+00011600: 7373 2f6c 6962 2f63 6b66 772f 6275 696c  ss/lib/ckfw/buil
+00011610: 7469 6e73 2f63 6572 7464 6174 612e 7478  tins/certdata.tx
+00011620: 7420 7c0a 7c20 2020 2020 2020 2020 2020  t |.|           
+00011630: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00011640: 2020 2020 2020 2020 2020 2020 2049 7420               It 
+00011650: 636f 6e74 6169 6e73 2074 6865 2063 6572  contains the cer
+00011660: 7469 6669 6361 7465 7320 696e 2050 454d  tificates in PEM
+00011670: 2066 6f72 6d61 7420 616e 6420 7468 6572   format and ther
+00011680: 6566 6f72 6520 2020 2020 2020 2020 2020  efore           
+00011690: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 000116a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116c0: 2020 4974 2063 6f6e 7461 696e 7320 7468    It contains th
-000116d0: 6520 6365 7274 6966 6963 6174 6573 2069  e certificates i
-000116e0: 6e20 5045 4d20 666f 726d 6174 2061 6e64  n PEM format and
-000116f0: 2074 6865 7265 666f 7265 2020 2020 2020   therefore      
+000116c0: 6361 6e20 6265 2064 6972 6563 746c 7920  can be directly 
+000116d0: 7573 6564 2077 6974 6820 6375 726c 202f  used with curl /
+000116e0: 206c 6962 6375 726c 202f 2070 6870 5f63   libcurl / php_c
+000116f0: 7572 6c2c 206f 7220 7769 7468 2020 2020  url, or with    
 00011700: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00011710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011720: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00011730: 2020 2020 2063 616e 2062 6520 6469 7265       can be dire
-00011740: 6374 6c79 2075 7365 6420 7769 7468 2063  ctly used with c
-00011750: 7572 6c20 2f20 6c69 6263 7572 6c20 2f20  url / libcurl / 
-00011760: 7068 705f 6375 726c 2c20 6f72 2077 6974  php_curl, or wit
-00011770: 6820 2020 2020 2020 2020 2020 2020 2020  h               
+00011730: 2020 2020 2020 616e 2041 7061 6368 652b        an Apache+
+00011740: 6d6f 645f 7373 6c20 7765 6273 6572 7665  mod_ssl webserve
+00011750: 7220 666f 7220 5353 4c20 636c 6965 6e74  r for SSL client
+00011760: 2061 7574 6865 6e74 6963 6174 696f 6e2e   authentication.
+00011770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011780: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00011790: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000117a0: 2020 2020 2020 2020 2020 2061 6e20 4170             an Ap
-000117b0: 6163 6865 2b6d 6f64 5f73 736c 2077 6562  ache+mod_ssl web
-000117c0: 7365 7276 6572 2066 6f72 2053 534c 2063  server for SSL c
-000117d0: 6c69 656e 7420 6175 7468 656e 7469 6361  lient authentica
-000117e0: 7469 6f6e 2e20 2020 2020 2020 2020 2020  tion.           
+000117a0: 2020 2020 2020 2020 2020 2020 204a 7573               Jus
+000117b0: 7420 636f 6e66 6967 7572 6520 7468 6973  t configure this
+000117c0: 2066 696c 6520 6173 2074 6865 2053 534c   file as the SSL
+000117d0: 4341 4365 7274 6966 6963 6174 6546 696c  CACertificateFil
+000117e0: 652e 2320 2020 2020 2020 2020 2020 2020  e.#             
 000117f0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00011800: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 00011810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011820: 2020 4a75 7374 2063 6f6e 6669 6775 7265    Just configure
-00011830: 2074 6869 7320 6669 6c65 2061 7320 7468   this file as th
-00011840: 6520 5353 4c43 4143 6572 7469 6669 6361  e SSLCACertifica
-00011850: 7465 4669 6c65 2e23 2020 2020 2020 2020  teFile.#        
+00011820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011860: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00011870: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011880: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
 00011890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000118c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000118a0: 2020 2a2a 2a2a 2a20 4245 4749 4e20 4c49    ***** BEGIN LI
+000118b0: 4345 4e53 4520 424c 4f43 4b20 2a2a 2a2a  CENSE BLOCK ****
+000118c0: 2a20 2020 2020 2020 2020 2020 2020 2020  *               
 000118d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000118e0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 000118f0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011910: 2020 2020 2020 202a 2a2a 2a2a 2042 4547         ***** BEG
-00011920: 494e 204c 4943 454e 5345 2042 4c4f 434b  IN LICENSE BLOCK
-00011930: 202a 2a2a 2a2a 2020 2020 2020 2020 2020   *****          
-00011940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011900: 2054 6869 7320 536f 7572 6365 2043 6f64   This Source Cod
+00011910: 6520 466f 726d 2069 7320 7375 626a 6563  e Form is subjec
+00011920: 7420 746f 2074 6865 2074 6572 6d73 206f  t to the terms o
+00011930: 6620 7468 6520 4d6f 7a69 6c6c 6120 5075  f the Mozilla Pu
+00011940: 626c 6963 204c 6963 656e 7365 2c20 2020  blic License,   
 00011950: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00011960: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00011970: 2020 2020 2020 5468 6973 2053 6f75 7263        This Sourc
-00011980: 6520 436f 6465 2046 6f72 6d20 6973 2073  e Code Form is s
-00011990: 7562 6a65 6374 2074 6f20 7468 6520 7465  ubject to the te
-000119a0: 726d 7320 6f66 2074 6865 204d 6f7a 696c  rms of the Mozil
-000119b0: 6c61 2050 7562 6c69 6320 4c69 6365 6e73  la Public Licens
-000119c0: 652c 2020 2020 2020 2020 7c0a 7c20 2020  e,        |.|   
+00011970: 2020 2020 762e 2032 2e30 2e20 4966 2061      v. 2.0. If a
+00011980: 2063 6f70 7920 6f66 2074 6865 204d 504c   copy of the MPL
+00011990: 2077 6173 206e 6f74 2064 6973 7472 6962   was not distrib
+000119a0: 7574 6564 2077 6974 6820 7468 6973 2066  uted with this f
+000119b0: 696c 652c 2059 6f75 2063 616e 206f 6274  ile, You can obt
+000119c0: 6169 6e20 2020 2020 2020 7c0a 7c20 2020  ain       |.|   
 000119d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119e0: 207c 2020 2020 2020 2076 2e20 322e 302e   |       v. 2.0.
-000119f0: 2049 6620 6120 636f 7079 206f 6620 7468   If a copy of th
-00011a00: 6520 4d50 4c20 7761 7320 6e6f 7420 6469  e MPL was not di
-00011a10: 7374 7269 6275 7465 6420 7769 7468 2074  stributed with t
-00011a20: 6869 7320 6669 6c65 2c20 596f 7520 6361  his file, You ca
-00011a30: 6e20 6f62 7461 696e 2020 2020 2020 207c  n obtain       |
+000119e0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+000119f0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+00011a00: 6e65 2061 7420 6874 7470 3a2f 2f6d 6f7a  ne at http://moz
+00011a10: 696c 6c61 2e6f 7267 2f4d 504c 2f32 2e30  illa.org/MPL/2.0
+00011a20: 2f2e 2020 2020 2020 2020 2020 2020 2020  /.              
+00011a30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00011a40: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00011a50: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 00011a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a70: 2020 2020 6f6e 6520 6174 2068 7474 703a      one at http:
-00011a80: 2f2f 6d6f 7a69 6c6c 612e 6f72 672f 4d50  //mozilla.org/MP
-00011a90: 4c2f 322e 302f 2e20 2020 2020 2020 2020  L/2.0/.         
+00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011ab0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00011ac0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
 00011ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ae0: 2020 2020 2020 2020 2020 2020 2a2a 2a2a              ****
+00011af0: 2a20 454e 4420 4c49 4345 4e53 4520 424c  * END LICENSE BL
+00011b00: 4f43 4b20 2a2a 2a2a 2a20 2020 2020 2020  OCK *****       
 00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011b20: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00011b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b40: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b60: 202a 2a2a 2a2a 2045 4e44 204c 4943 454e   ***** END LICEN
-00011b70: 5345 2042 4c4f 434b 202a 2a2a 2a2a 2020  SE BLOCK *****  
-00011b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b90: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00011b40: 7c20 2020 2020 2020 2040 2823 2920 2452  |        @(#) $R
+00011b50: 4353 6669 6c65 3a20 6365 7274 6461 7461  CSfile: certdata
+00011b60: 2e74 7874 2c76 2024 2024 5265 7669 7369  .txt,v $ $Revisi
+00011b70: 6f6e 3a20 312e 3830 2024 2024 4461 7465  on: 1.80 $ $Date
+00011b80: 3a20 3230 3131 2f31 312f 3033 2031 353a  : 2011/11/03 15:
+00011b90: 3131 3a35 3820 2420 2020 2020 2020 7c0a  11:58 $       |.
 00011ba0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00011bb0: 2020 2020 207c 2020 2020 2020 2020 4028       |        @(
-00011bc0: 2329 2024 5243 5366 696c 653a 2063 6572  #) $RCSfile: cer
-00011bd0: 7464 6174 612e 7478 742c 7620 2420 2452  tdata.txt,v $ $R
-00011be0: 6576 6973 696f 6e3a 2031 2e38 3020 2420  evision: 1.80 $ 
-00011bf0: 2444 6174 653a 2032 3031 312f 3131 2f30  $Date: 2011/11/0
-00011c00: 3320 3135 3a31 313a 3538 2024 2020 2020  3 15:11:58 $    
-00011c10: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00011c20: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00011c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011c80: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
-00011c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00011ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00011cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
-00011d00: 2063 6861 7273 6574 2d6e 6f72 6d61 6c69   charset-normali
-00011d10: 7a65 7220 7c20 2020 2020 2020 2020 2020  zer |           
+00011bb0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00011bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c10: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
+00011c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00011c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00011c80: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 6368 6172  --------+.| char
+00011c90: 7365 742d 6e6f 726d 616c 697a 6572 207c  set-normalizer |
+00011ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cc0: 2020 2020 2020 2020 204d 4954 204c 6963           MIT Lic
+00011cd0: 656e 7365 2020 2020 2020 2020 2020 2020  ense            
+00011ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011cf0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00011d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d10: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
 00011d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d30: 2020 2020 2020 2020 2020 2020 2020 4d49                MI
-00011d40: 5420 4c69 6365 6e73 6520 2020 2020 2020  T License       
+00011d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011d70: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00011d80: 2020 2020 2020 2020 207c 2020 2020 2020           |      
 00011d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011da0: 2020 2020 2020 2020 436f 7079 7269 6768          Copyrigh
+00011db0: 7420 2863 2920 3230 3139 2054 4148 5249  t (c) 2019 TAHRI
+00011dc0: 2041 686d 6564 2052 2e20 2020 2020 2020   Ahmed R.       
 00011dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011de0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00011df0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 00011e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e10: 2020 2020 2020 2020 2020 2020 2043 6f70               Cop
-00011e20: 7972 6967 6874 2028 6329 2032 3031 3920  yright (c) 2019 
-00011e30: 5441 4852 4920 4168 6d65 6420 522e 2020  TAHRI Ahmed R.  
+00011e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00011e50: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00011e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e70: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00011e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011e70: 2020 207c 2020 2020 2020 2020 2050 6572     |         Per
+00011e80: 6d69 7373 696f 6e20 6973 2068 6572 6562  mission is hereb
+00011e90: 7920 6772 616e 7465 642c 2066 7265 6520  y granted, free 
+00011ea0: 6f66 2063 6861 7267 652c 2074 6f20 616e  of charge, to an
+00011eb0: 7920 7065 7273 6f6e 206f 6274 6169 6e69  y person obtaini
+00011ec0: 6e67 2061 2063 6f70 7920 2020 2020 2020  ng a copy       
 00011ed0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00011ee0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00011ef0: 2020 5065 726d 6973 7369 6f6e 2069 7320    Permission is 
-00011f00: 6865 7265 6279 2067 7261 6e74 6564 2c20  hereby granted, 
-00011f10: 6672 6565 206f 6620 6368 6172 6765 2c20  free of charge, 
-00011f20: 746f 2061 6e79 2070 6572 736f 6e20 6f62  to any person ob
-00011f30: 7461 696e 696e 6720 6120 636f 7079 2020  taining a copy  
+00011ef0: 206f 6620 7468 6973 2073 6f66 7477 6172   of this softwar
+00011f00: 6520 616e 6420 6173 736f 6369 6174 6564  e and associated
+00011f10: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
+00011f20: 696c 6573 2028 7468 6520 2253 6f66 7477  iles (the "Softw
+00011f30: 6172 6522 292c 2074 6f20 6465 616c 2020  are"), to deal  
 00011f40: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00011f50: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00011f60: 2020 2020 2020 6f66 2074 6869 7320 736f        of this so
-00011f70: 6674 7761 7265 2061 6e64 2061 7373 6f63  ftware and assoc
-00011f80: 6961 7465 6420 646f 6375 6d65 6e74 6174  iated documentat
-00011f90: 696f 6e20 6669 6c65 7320 2874 6865 2022  ion files (the "
-00011fa0: 536f 6674 7761 7265 2229 2c20 746f 2064  Software"), to d
-00011fb0: 6561 6c20 2020 2020 2020 207c 0a7c 2020  eal        |.|  
+00011f60: 2020 2020 2020 2069 6e20 7468 6520 536f         in the So
+00011f70: 6674 7761 7265 2077 6974 686f 7574 2072  ftware without r
+00011f80: 6573 7472 6963 7469 6f6e 2c20 696e 636c  estriction, incl
+00011f90: 7564 696e 6720 7769 7468 6f75 7420 6c69  uding without li
+00011fa0: 6d69 7461 7469 6f6e 2074 6865 2072 6967  mitation the rig
+00011fb0: 6874 7320 2020 2020 2020 207c 0a7c 2020  hts        |.|  
 00011fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011fd0: 2020 7c20 2020 2020 2020 2020 696e 2074    |         in t
-00011fe0: 6865 2053 6f66 7477 6172 6520 7769 7468  he Software with
-00011ff0: 6f75 7420 7265 7374 7269 6374 696f 6e2c  out restriction,
-00012000: 2069 6e63 6c75 6469 6e67 2077 6974 686f   including witho
-00012010: 7574 206c 696d 6974 6174 696f 6e20 7468  ut limitation th
-00012020: 6520 7269 6768 7473 2020 2020 2020 2020  e rights        
+00011fd0: 2020 7c20 2020 2020 2020 2020 2074 6f20    |          to 
+00011fe0: 7573 652c 2063 6f70 792c 206d 6f64 6966  use, copy, modif
+00011ff0: 792c 206d 6572 6765 2c20 7075 626c 6973  y, merge, publis
+00012000: 682c 2064 6973 7472 6962 7574 652c 2073  h, distribute, s
+00012010: 7562 6c69 6365 6e73 652c 2061 6e64 2f6f  ublicense, and/o
+00012020: 7220 7365 6c6c 2020 2020 2020 2020 2020  r sell          
 00012030: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00012040: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00012050: 2020 746f 2075 7365 2c20 636f 7079 2c20    to use, copy, 
-00012060: 6d6f 6469 6679 2c20 6d65 7267 652c 2070  modify, merge, p
-00012070: 7562 6c69 7368 2c20 6469 7374 7269 6275  ublish, distribu
-00012080: 7465 2c20 7375 626c 6963 656e 7365 2c20  te, sublicense, 
-00012090: 616e 642f 6f72 2073 656c 6c20 2020 2020  and/or sell     
+00012050: 2020 2020 636f 7069 6573 206f 6620 7468      copies of th
+00012060: 6520 536f 6674 7761 7265 2c20 616e 6420  e Software, and 
+00012070: 746f 2070 6572 6d69 7420 7065 7273 6f6e  to permit person
+00012080: 7320 746f 2077 686f 6d20 7468 6520 536f  s to whom the So
+00012090: 6674 7761 7265 2069 7320 2020 2020 2020  ftware is       
 000120a0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 000120b0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000120c0: 2020 2020 2020 2020 2063 6f70 6965 7320           copies 
-000120d0: 6f66 2074 6865 2053 6f66 7477 6172 652c  of the Software,
-000120e0: 2061 6e64 2074 6f20 7065 726d 6974 2070   and to permit p
-000120f0: 6572 736f 6e73 2074 6f20 7768 6f6d 2074  ersons to whom t
-00012100: 6865 2053 6f66 7477 6172 6520 6973 2020  he Software is  
+000120c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000120d0: 6675 726e 6973 6865 6420 746f 2064 6f20  furnished to do 
+000120e0: 736f 2c20 7375 626a 6563 7420 746f 2074  so, subject to t
+000120f0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
+00012100: 6469 7469 6f6e 733a 2020 2020 2020 2020  ditions:        
 00012110: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00012120: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012130: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00012140: 2020 2020 2066 7572 6e69 7368 6564 2074       furnished t
-00012150: 6f20 646f 2073 6f2c 2073 7562 6a65 6374  o do so, subject
-00012160: 2074 6f20 7468 6520 666f 6c6c 6f77 696e   to the followin
-00012170: 6720 636f 6e64 6974 696f 6e73 3a20 2020  g conditions:   
+00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012180: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00012190: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-000121a0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121a0: 2020 2020 2020 7c20 2020 2020 2020 2054        |        T
+000121b0: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
+000121c0: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
+000121d0: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
+000121e0: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
+000121f0: 636c 7564 6564 2069 6e20 616c 6c20 2020  cluded in all   
 00012200: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00012210: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00012220: 2020 2020 5468 6520 6162 6f76 6520 636f      The above co
-00012230: 7079 7269 6768 7420 6e6f 7469 6365 2061  pyright notice a
-00012240: 6e64 2074 6869 7320 7065 726d 6973 7369  nd this permissi
-00012250: 6f6e 206e 6f74 6963 6520 7368 616c 6c20  on notice shall 
-00012260: 6265 2069 6e63 6c75 6465 6420 696e 2061  be included in a
-00012270: 6c6c 2020 2020 2020 207c 0a7c 2020 2020  ll       |.|    
+00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012230: 2020 2063 6f70 6965 7320 6f72 2073 7562     copies or sub
+00012240: 7374 616e 7469 616c 2070 6f72 7469 6f6e  stantial portion
+00012250: 7320 6f66 2074 6865 2053 6f66 7477 6172  s of the Softwar
+00012260: 652e 2020 2020 2020 2020 2020 2020 2020  e.              
+00012270: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00012280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012290: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000122a0: 2020 2020 2020 2020 636f 7069 6573 206f          copies o
-000122b0: 7220 7375 6273 7461 6e74 6961 6c20 706f  r substantial po
-000122c0: 7274 696f 6e73 206f 6620 7468 6520 536f  rtions of the So
-000122d0: 6674 7761 7265 2e20 2020 2020 2020 2020  ftware.         
+000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000122e0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 000122f0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00012300: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00012310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012310: 5448 4520 534f 4654 5741 5245 2049 5320  THE SOFTWARE IS 
+00012320: 5052 4f56 4944 4544 2022 4153 2049 5322  PROVIDED "AS IS"
+00012330: 2c20 5749 5448 4f55 5420 5741 5252 414e  , WITHOUT WARRAN
+00012340: 5459 204f 4620 414e 5920 4b49 4e44 2c20  TY OF ANY KIND, 
+00012350: 4558 5052 4553 5320 4f52 2020 2020 2020  EXPRESS OR      
 00012360: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00012370: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00012380: 2020 2020 2054 4845 2053 4f46 5457 4152       THE SOFTWAR
-00012390: 4520 4953 2050 524f 5649 4445 4420 2241  E IS PROVIDED "A
-000123a0: 5320 4953 222c 2057 4954 484f 5554 2057  S IS", WITHOUT W
-000123b0: 4152 5241 4e54 5920 4f46 2041 4e59 204b  ARRANTY OF ANY K
-000123c0: 494e 442c 2045 5850 5245 5353 204f 5220  IND, EXPRESS OR 
+00012380: 2020 2020 2020 494d 504c 4945 442c 2049        IMPLIED, I
+00012390: 4e43 4c55 4449 4e47 2042 5554 204e 4f54  NCLUDING BUT NOT
+000123a0: 204c 494d 4954 4544 2054 4f20 5448 4520   LIMITED TO THE 
+000123b0: 5741 5252 414e 5449 4553 204f 4620 4d45  WARRANTIES OF ME
+000123c0: 5243 4841 4e54 4142 494c 4954 592c 2020  RCHANTABILITY,  
 000123d0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 000123e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000123f0: 2020 2020 2020 2020 2020 2049 4d50 4c49             IMPLI
-00012400: 4544 2c20 494e 434c 5544 494e 4720 4255  ED, INCLUDING BU
-00012410: 5420 4e4f 5420 4c49 4d49 5445 4420 544f  T NOT LIMITED TO
-00012420: 2054 4845 2057 4152 5241 4e54 4945 5320   THE WARRANTIES 
-00012430: 4f46 204d 4552 4348 414e 5441 4249 4c49  OF MERCHANTABILI
-00012440: 5459 2c20 2020 2020 2020 2020 207c 0a7c  TY,          |.|
+000123f0: 2020 2020 2020 2020 2046 4954 4e45 5353           FITNESS
+00012400: 2046 4f52 2041 2050 4152 5449 4355 4c41   FOR A PARTICULA
+00012410: 5220 5055 5250 4f53 4520 414e 4420 4e4f  R PURPOSE AND NO
+00012420: 4e49 4e46 5249 4e47 454d 454e 542e 2049  NINFRINGEMENT. I
+00012430: 4e20 4e4f 2045 5645 4e54 2053 4841 4c4c  N NO EVENT SHALL
+00012440: 2054 4845 2020 2020 2020 2020 207c 0a7c   THE         |.|
 00012450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012460: 2020 2020 7c20 2020 2020 2020 2020 4649      |         FI
-00012470: 544e 4553 5320 464f 5220 4120 5041 5254  TNESS FOR A PART
-00012480: 4943 554c 4152 2050 5552 504f 5345 2041  ICULAR PURPOSE A
-00012490: 4e44 204e 4f4e 494e 4652 494e 4745 4d45  ND NONINFRINGEME
-000124a0: 4e54 2e20 494e 204e 4f20 4556 454e 5420  NT. IN NO EVENT 
-000124b0: 5348 414c 4c20 5448 4520 2020 2020 2020  SHALL THE       
+00012460: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00012470: 2041 5554 484f 5253 204f 5220 434f 5059   AUTHORS OR COPY
+00012480: 5249 4748 5420 484f 4c44 4552 5320 4245  RIGHT HOLDERS BE
+00012490: 204c 4941 424c 4520 464f 5220 414e 5920   LIABLE FOR ANY 
+000124a0: 434c 4149 4d2c 2044 414d 4147 4553 204f  CLAIM, DAMAGES O
+000124b0: 5220 4f54 4845 5220 2020 2020 2020 2020  R OTHER         
 000124c0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 000124d0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000124e0: 2020 2020 2020 4155 5448 4f52 5320 4f52        AUTHORS OR
-000124f0: 2043 4f50 5952 4947 4854 2048 4f4c 4445   COPYRIGHT HOLDE
-00012500: 5253 2042 4520 4c49 4142 4c45 2046 4f52  RS BE LIABLE FOR
-00012510: 2041 4e59 2043 4c41 494d 2c20 4441 4d41   ANY CLAIM, DAMA
-00012520: 4745 5320 4f52 204f 5448 4552 2020 2020  GES OR OTHER    
+000124e0: 2020 4c49 4142 494c 4954 592c 2057 4845    LIABILITY, WHE
+000124f0: 5448 4552 2049 4e20 414e 2041 4354 494f  THER IN AN ACTIO
+00012500: 4e20 4f46 2043 4f4e 5452 4143 542c 2054  N OF CONTRACT, T
+00012510: 4f52 5420 4f52 204f 5448 4552 5749 5345  ORT OR OTHERWISE
+00012520: 2c20 4152 4953 494e 4720 4652 4f4d 2c20  , ARISING FROM, 
 00012530: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00012540: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00012550: 2020 2020 2020 204c 4941 4249 4c49 5459         LIABILITY
-00012560: 2c20 5748 4554 4845 5220 494e 2041 4e20  , WHETHER IN AN 
-00012570: 4143 5449 4f4e 204f 4620 434f 4e54 5241  ACTION OF CONTRA
-00012580: 4354 2c20 544f 5254 204f 5220 4f54 4845  CT, TORT OR OTHE
-00012590: 5257 4953 452c 2041 5249 5349 4e47 2046  RWISE, ARISING F
-000125a0: 524f 4d2c 2020 2020 2020 2020 7c0a 7c20  ROM,        |.| 
+00012550: 2020 2020 2020 204f 5554 204f 4620 4f52         OUT OF OR
+00012560: 2049 4e20 434f 4e4e 4543 5449 4f4e 2057   IN CONNECTION W
+00012570: 4954 4820 5448 4520 534f 4654 5741 5245  ITH THE SOFTWARE
+00012580: 204f 5220 5448 4520 5553 4520 4f52 204f   OR THE USE OR O
+00012590: 5448 4552 2044 4541 4c49 4e47 5320 494e  THER DEALINGS IN
+000125a0: 2054 4845 2020 2020 2020 2020 7c0a 7c20   THE        |.| 
 000125b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125c0: 2020 207c 2020 2020 2020 2020 4f55 5420     |        OUT 
-000125d0: 4f46 204f 5220 494e 2043 4f4e 4e45 4354  OF OR IN CONNECT
-000125e0: 494f 4e20 5749 5448 2054 4845 2053 4f46  ION WITH THE SOF
-000125f0: 5457 4152 4520 4f52 2054 4845 2055 5345  TWARE OR THE USE
-00012600: 204f 5220 4f54 4845 5220 4445 414c 494e   OR OTHER DEALIN
-00012610: 4753 2049 4e20 5448 4520 2020 2020 2020  GS IN THE       
-00012620: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00012630: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00012640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012660: 2020 2053 4f46 5457 4152 452e 2020 2020     SOFTWARE.    
-00012670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012690: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
-000126a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-000126b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000126c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000126d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000126e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000126f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00012700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020  -----------+.|  
-00012710: 2020 2020 646f 6375 7469 6c73 2020 2020      docutils    
+000125c0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+000125d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000125e0: 2020 2020 2020 2020 2020 2020 2020 534f                SO
+000125f0: 4654 5741 5245 2e20 2020 2020 2020 2020  FTWARE.         
+00012600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012620: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+00012630: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00012640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00012690: 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020 2064  ------+.|      d
+000126a0: 6f63 7574 696c 7320 2020 2020 207c 2020  ocutils      |  
+000126b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000126d0: 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d      ============
+000126e0: 3d3d 3d3d 3d3d 2020 2020 2020 2020 2020  ======          
+000126f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012700: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00012710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012720: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
 00012730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012740: 2020 2020 2020 2020 203d 3d3d 3d3d 3d3d           =======
-00012750: 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 2020 2020  ===========     
+00012740: 2020 2020 2020 2020 2020 436f 7079 696e            Copyin
+00012750: 6720 446f 6375 7469 6c73 2020 2020 2020  g Docutils      
 00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012780: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00012790: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 000127a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127b0: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-000127c0: 6f70 7969 6e67 2044 6f63 7574 696c 7320  opying Docutils 
+000127b0: 2020 2020 2020 2020 2020 2020 2020 3d3d                ==
+000127c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000127d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000127e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000127f0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00012800: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00012810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012830: 2020 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d     =============
-00012840: 3d3d 3d3d 3d20 2020 2020 2020 2020 2020  =====           
+00012830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012860: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00012870: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012880: 207c 2020 2020 2020 2020 2020 2020 2020   |              
 00012890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000128b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000128a0: 2020 2020 2020 3a41 7574 686f 723a 2044        :Author: D
+000128b0: 6176 6964 2047 6f6f 6467 6572 2020 2020  avid Goodger    
 000128c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000128d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 000128e0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 000128f0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 00012900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012910: 2020 2020 2020 2020 2020 203a 4175 7468             :Auth
-00012920: 6f72 3a20 4461 7669 6420 476f 6f64 6765  or: David Goodge
-00012930: 7220 2020 2020 2020 2020 2020 2020 2020  r               
+00012910: 2020 2020 2020 2020 3a43 6f6e 7461 6374          :Contact
+00012920: 3a20 676f 6f64 6765 7240 7079 7468 6f6e  : goodger@python
+00012930: 2e6f 7267 2020 2020 2020 2020 2020 2020  .org            
 00012940: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012950: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00012960: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00012970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012980: 2020 2020 2020 2020 2020 2020 203a 436f               :Co
-00012990: 6e74 6163 743a 2067 6f6f 6467 6572 4070  ntact: goodger@p
-000129a0: 7974 686f 6e2e 6f72 6720 2020 2020 2020  ython.org       
-000129b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012970: 2020 2020 2020 2020 2020 2020 203a 4461               :Da
+00012980: 7465 3a20 2444 6174 653a 2032 3032 312d  te: $Date: 2021-
+00012990: 3131 2d31 3920 3133 3a34 363a 3338 202b  11-19 13:46:38 +
+000129a0: 3031 3030 2028 4672 2c20 3139 2e20 4e6f  0100 (Fr, 19. No
+000129b0: 7620 3230 3231 2920 2420 2020 2020 2020  v 2021) $       
 000129c0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 000129d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000129e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000129f0: 2020 3a44 6174 653a 2024 4461 7465 3a20    :Date: $Date: 
-00012a00: 3230 3232 2d30 352d 3330 2031 383a 3534  2022-05-30 18:54
-00012a10: 3a34 3620 2b30 3230 3020 284d 6f2c 2033  :46 +0200 (Mo, 3
-00012a20: 302e 204d 6169 2032 3032 3229 2024 2020  0. Mai 2022) $  
+000129f0: 2020 2020 2020 2020 2020 3a57 6562 2073            :Web s
+00012a00: 6974 653a 2068 7474 703a 2f2f 646f 6375  ite: http://docu
+00012a10: 7469 6c73 2e73 6f75 7263 6566 6f72 6765  tils.sourceforge
+00012a20: 2e6e 6574 2f20 2020 2020 2020 2020 2020  .net/           
 00012a30: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00012a40: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00012a50: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00012a60: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-00012a70: 5765 6220 7369 7465 3a20 6874 7470 733a  Web site: https:
-00012a80: 2f2f 646f 6375 7469 6c73 2e73 6f75 7263  //docutils.sourc
-00012a90: 6566 6f72 6765 2e69 6f2f 2020 2020 2020  eforge.io/      
-00012aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012a60: 2020 2020 203a 436f 7079 7269 6768 743a       :Copyright:
+00012a70: 2054 6869 7320 646f 6375 6d65 6e74 2068   This document h
+00012a80: 6173 2062 6565 6e20 706c 6163 6564 2069  as been placed i
+00012a90: 6e20 7468 6520 7075 626c 6963 2064 6f6d  n the public dom
+00012aa0: 6169 6e2e 2020 2020 2020 2020 2020 2020  ain.            
 00012ab0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00012ac0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00012ad0: 2020 2020 2020 2020 2020 3a43 6f70 7972            :Copyr
-00012ae0: 6967 6874 3a20 5468 6973 2064 6f63 756d  ight: This docum
-00012af0: 656e 7420 6861 7320 6265 656e 2070 6c61  ent has been pla
-00012b00: 6365 6420 696e 2074 6865 2070 7562 6c69  ced in the publi
-00012b10: 6320 646f 6d61 696e 2e20 2020 2020 2020  c domain.       
+00012ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012b20: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00012b30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00012b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b40: 2020 2020 2020 2020 2020 2020 2020 4d6f                Mo
+00012b50: 7374 206f 6620 7468 6520 6669 6c65 7320  st of the files 
+00012b60: 696e 636c 7564 6564 2069 6e20 7468 6973  included in this
+00012b70: 2070 726f 6a65 6374 2068 6176 6520 6265   project have be
+00012b80: 656e 2070 6c61 6365 6420 696e 2074 6865  en placed in the
 00012b90: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00012ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012bb0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00012bc0: 2020 204d 6f73 7420 6f66 2074 6865 2066     Most of the f
-00012bd0: 696c 6573 2069 6e63 6c75 6465 6420 696e  iles included in
-00012be0: 2074 6869 7320 7072 6f6a 6563 7420 6861   this project ha
-00012bf0: 7665 2062 6565 6e20 706c 6163 6564 2069  ve been placed i
-00012c00: 6e20 7468 6520 2020 2020 2020 2020 2020  n the           
+00012bc0: 2020 2020 7075 626c 6963 2064 6f6d 6169      public domai
+00012bd0: 6e2c 2061 6e64 2074 6865 7265 666f 7265  n, and therefore
+00012be0: 2068 6176 6520 6e6f 206c 6963 656e 7365   have no license
+00012bf0: 2072 6571 7569 7265 6d65 6e74 7320 616e   requirements an
+00012c00: 6420 6e6f 2020 2020 2020 2020 2020 2020  d no            
 00012c10: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00012c20: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00012c30: 2020 2020 2020 2020 2070 7562 6c69 6320           public 
-00012c40: 646f 6d61 696e 2c20 616e 6420 7468 6572  domain, and ther
-00012c50: 6566 6f72 6520 6861 7665 206e 6f20 6c69  efore have no li
-00012c60: 6365 6e73 6520 7265 7175 6972 656d 656e  cense requiremen
-00012c70: 7473 2061 6e64 206e 6f20 2020 2020 2020  ts and no       
+00012c30: 2020 2020 2020 7265 7374 7269 6374 696f        restrictio
+00012c40: 6e73 206f 6e20 636f 7079 696e 6720 6f72  ns on copying or
+00012c50: 2075 7361 6765 3b20 7365 6520 7468 6520   usage; see the 
+00012c60: 6050 7562 6c69 6320 446f 6d61 696e 2044  `Public Domain D
+00012c70: 6564 6963 6174 696f 6e60 5f20 2020 2020  edication`_     
 00012c80: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00012c90: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00012ca0: 2020 2020 2020 2020 2020 2072 6573 7472             restr
-00012cb0: 6963 7469 6f6e 7320 6f6e 2063 6f70 7969  ictions on copyi
-00012cc0: 6e67 206f 7220 7573 6167 653b 2073 6565  ng or usage; see
-00012cd0: 2074 6865 2060 5075 626c 6963 2044 6f6d   the `Public Dom
-00012ce0: 6169 6e20 4465 6469 6361 7469 6f6e 605f  ain Dedication`_
+00012ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012cb0: 2020 2020 2062 656c 6f77 2e20 2054 6865       below.  The
+00012cc0: 7265 2061 7265 2061 2066 6577 2065 7863  re are a few exc
+00012cd0: 6570 7469 6f6e 735f 2c20 6c69 7374 6564  eptions_, listed
+00012ce0: 2062 656c 6f77 2e20 2020 2020 2020 2020   below.         
 00012cf0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012d10: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00012d20: 2020 2020 2020 2020 2020 6265 6c6f 772e            below.
-00012d30: 2020 5468 6572 6520 6172 6520 6120 6665    There are a fe
-00012d40: 7720 6578 6365 7074 696f 6e73 5f2c 206c  w exceptions_, l
-00012d50: 6973 7465 6420 6265 6c6f 772e 2020 2020  isted below.    
-00012d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012d20: 2046 696c 6573 2069 6e20 7468 6520 5361   Files in the Sa
+00012d30: 6e64 626f 785f 2061 7265 206e 6f74 2064  ndbox_ are not d
+00012d40: 6973 7472 6962 7574 6564 2077 6974 6820  istributed with 
+00012d50: 446f 6375 7469 6c73 2072 656c 6561 7365  Docutils release
+00012d60: 7320 616e 6420 2020 2020 2020 2020 2020  s and           
 00012d70: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00012d80: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00012d90: 2020 2020 2020 4669 6c65 7320 696e 2074        Files in t
-00012da0: 6865 2053 616e 6462 6f78 5f20 6172 6520  he Sandbox_ are 
-00012db0: 6e6f 7420 6469 7374 7269 6275 7465 6420  not distributed 
-00012dc0: 7769 7468 2044 6f63 7574 696c 7320 7265  with Docutils re
-00012dd0: 6c65 6173 6573 2061 6e64 2020 2020 2020  leases and      
+00012d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012da0: 2020 2020 2020 206d 6179 2068 6176 6520         may have 
+00012db0: 6469 6666 6572 656e 7420 6c69 6365 6e73  different licens
+00012dc0: 6520 7465 726d 732e 2020 2020 2020 2020  e terms.        
+00012dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012de0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00012df0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 00012e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012e10: 2020 2020 2020 2020 2020 2020 6d61 7920              may 
-00012e20: 6861 7665 2064 6966 6665 7265 6e74 206c  have different l
-00012e30: 6963 656e 7365 2074 6572 6d73 2e20 2020  icense terms.   
+00012e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012e50: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00012e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012e70: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
 00012e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012ed0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00012ee0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 00012ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f00: 2020 2020 2020 2020 2020 2050 7562 6c69             Publi
+00012f10: 6320 446f 6d61 696e 2044 6564 6963 6174  c Domain Dedicat
+00012f20: 696f 6e20 2020 2020 2020 2020 2020 2020  ion             
 00012f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012f40: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00012f50: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00012f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012f80: 5075 626c 6963 2044 6f6d 6169 6e20 4465  Public Domain De
-00012f90: 6469 6361 7469 6f6e 2020 2020 2020 2020  dication        
+00012f80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00012f90: 3d3d 3d3d 3d3d 3d3d 2020 2020 2020 2020  ========        
 00012fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012fb0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00012fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012fd0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
 00012fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012ff0: 2020 2020 203d 3d3d 3d3d 3d3d 3d3d 3d3d       ===========
-00013000: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 2020  =============   
+00012ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013010: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013020: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00013030: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00013040: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00013050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013050: 2020 2020 2054 6865 2070 6572 736f 6e73       The persons
+00013060: 2077 686f 2068 6176 6520 6173 736f 6369   who have associ
+00013070: 6174 6564 2074 6865 6972 2077 6f72 6b20  ated their work 
+00013080: 7769 7468 2074 6869 7320 7072 6f6a 6563  with this projec
+00013090: 7420 2874 6865 2020 2020 2020 2020 2020  t (the          
 000130a0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 000130b0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000130c0: 2020 2020 2020 2020 2020 5468 6520 7065            The pe
-000130d0: 7273 6f6e 7320 7768 6f20 6861 7665 2061  rsons who have a
-000130e0: 7373 6f63 6961 7465 6420 7468 6569 7220  ssociated their 
-000130f0: 776f 726b 2077 6974 6820 7468 6973 2070  work with this p
-00013100: 726f 6a65 6374 2028 7468 6520 2020 2020  roject (the     
+000130c0: 2020 2020 2020 2020 2022 4465 6469 6361           "Dedica
+000130d0: 746f 7222 3a20 4461 7669 6420 476f 6f64  tor": David Good
+000130e0: 6765 7220 616e 6420 7468 6520 6d61 6e79  ger and the many
+000130f0: 2063 6f6e 7472 6962 7574 6f72 7320 746f   contributors to
+00013100: 2074 6865 2044 6f63 7574 696c 7320 2020   the Docutils   
 00013110: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00013120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013130: 7c20 2020 2020 2020 2020 2020 2020 2244  |             "D
-00013140: 6564 6963 6174 6f72 223a 2044 6176 6964  edicator": David
-00013150: 2047 6f6f 6467 6572 2061 6e64 2074 6865   Goodger and the
-00013160: 206d 616e 7920 636f 6e74 7269 6275 746f   many contributo
-00013170: 7273 2074 6f20 7468 6520 446f 6375 7469  rs to the Docuti
-00013180: 6c73 2020 2020 2020 2020 2020 2020 7c0a  ls            |.
+00013130: 7c20 2020 2020 2020 2020 2020 2020 7072  |             pr
+00013140: 6f6a 6563 7429 2068 6572 6562 7920 6465  oject) hereby de
+00013150: 6469 6361 7465 2074 6865 2065 6e74 6972  dicate the entir
+00013160: 6520 636f 7079 7269 6768 742c 206c 6573  e copyright, les
+00013170: 7320 7468 6520 6578 6365 7074 696f 6e73  s the exceptions
+00013180: 5f20 2020 2020 2020 2020 2020 2020 7c0a  _             |.
 00013190: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 000131a0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000131b0: 2020 2070 726f 6a65 6374 2920 6865 7265     project) here
-000131c0: 6279 2064 6564 6963 6174 6520 7468 6520  by dedicate the 
-000131d0: 656e 7469 7265 2063 6f70 7972 6967 6874  entire copyright
-000131e0: 2c20 6c65 7373 2074 6865 2065 7863 6570  , less the excep
-000131f0: 7469 6f6e 735f 2020 2020 2020 2020 2020  tions_          
+000131b0: 2020 6c69 7374 6564 2062 656c 6f77 2c20    listed below, 
+000131c0: 696e 2074 6865 2077 6f72 6b20 6f66 2061  in the work of a
+000131d0: 7574 686f 7273 6869 7020 6b6e 6f77 6e20  uthorship known 
+000131e0: 6173 2022 446f 6375 7469 6c73 2220 6964  as "Docutils" id
+000131f0: 656e 7469 6669 6564 2020 2020 2020 2020  entified        
 00013200: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00013210: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00013220: 2020 2020 2020 206c 6973 7465 6420 6265         listed be
-00013230: 6c6f 772c 2069 6e20 7468 6520 776f 726b  low, in the work
-00013240: 206f 6620 6175 7468 6f72 7368 6970 206b   of authorship k
-00013250: 6e6f 776e 2061 7320 2244 6f63 7574 696c  nown as "Docutil
-00013260: 7322 2069 6465 6e74 6966 6965 6420 2020  s" identified   
+00013220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013230: 2020 2020 2020 6265 6c6f 7720 2874 6865        below (the
+00013240: 2022 576f 726b 2229 2074 6f20 7468 6520   "Work") to the 
+00013250: 7075 626c 6963 2064 6f6d 6169 6e2e 2020  public domain.  
+00013260: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013270: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00013280: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00013290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132a0: 2020 2020 2020 2020 2020 2062 656c 6f77             below
-000132b0: 2028 7468 6520 2257 6f72 6b22 2920 746f   (the "Work") to
-000132c0: 2074 6865 2070 7562 6c69 6320 646f 6d61   the public doma
-000132d0: 696e 2e20 2020 2020 2020 2020 2020 2020  in.             
+000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000132e0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013300: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00013310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013310: 2020 2054 6865 2070 7269 6d61 7279 2072     The primary r
+00013320: 6570 6f73 6974 6f72 7920 666f 7220 7468  epository for th
+00013330: 6520 576f 726b 2069 7320 7468 6520 496e  e Work is the In
+00013340: 7465 726e 6574 2057 6f72 6c64 2057 6964  ternet World Wid
+00013350: 6520 5765 6220 2020 2020 2020 2020 2020  e Web           
 00013360: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00013370: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00013380: 2020 2020 2020 2020 5468 6520 7072 696d          The prim
-00013390: 6172 7920 7265 706f 7369 746f 7279 2066  ary repository f
-000133a0: 6f72 2074 6865 2057 6f72 6b20 6973 2074  or the Work is t
-000133b0: 6865 2049 6e74 6572 6e65 7420 576f 726c  he Internet Worl
-000133c0: 6420 5769 6465 2057 6562 2020 2020 2020  d Wide Web      
+00013380: 2020 2020 2020 2020 7369 7465 203c 6874          site <ht
+00013390: 7470 3a2f 2f64 6f63 7574 696c 732e 736f  tp://docutils.so
+000133a0: 7572 6365 666f 7267 652e 6e65 742f 3e2e  urceforge.net/>.
+000133b0: 2020 5468 6520 576f 726b 2063 6f6e 7369    The Work consi
+000133c0: 7374 7320 6f66 2074 6865 2020 2020 2020  sts of the      
 000133d0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 000133e0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000133f0: 2020 2020 2020 2020 2020 2020 2073 6974               sit
-00013400: 6520 3c68 7474 7073 3a2f 2f64 6f63 7574  e <https://docut
-00013410: 696c 732e 736f 7572 6365 666f 7267 652e  ils.sourceforge.
-00013420: 696f 2f3e 2e20 2054 6865 2057 6f72 6b20  io/>.  The Work 
-00013430: 636f 6e73 6973 7473 206f 6620 7468 6520  consists of the 
+000133f0: 2020 2020 2020 2020 2020 2066 696c 6573             files
+00013400: 2077 6974 6869 6e20 7468 6520 2264 6f63   within the "doc
+00013410: 7574 696c 7322 206d 6f64 756c 6520 6f66  utils" module of
+00013420: 2074 6865 2044 6f63 7574 696c 7320 7072   the Docutils pr
+00013430: 6f6a 6563 7420 5375 6276 6572 7369 6f6e  oject Subversion
 00013440: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00013450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013460: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00013470: 6669 6c65 7320 7769 7468 696e 2074 6865  files within the
-00013480: 2022 646f 6375 7469 6c73 2220 6d6f 6475   "docutils" modu
-00013490: 6c65 206f 6620 7468 6520 446f 6375 7469  le of the Docuti
-000134a0: 6c73 2070 726f 6a65 6374 2053 7562 7665  ls project Subve
-000134b0: 7273 696f 6e20 2020 2020 2020 2020 2020  rsion           
+00013460: 2020 207c 2020 2020 2020 2020 2020 2072     |           r
+00013470: 6570 6f73 6974 6f72 7920 2849 6e74 6572  epository (Inter
+00013480: 6e65 7420 686f 7374 2064 6f63 7574 696c  net host docutil
+00013490: 732e 7376 6e2e 736f 7572 6365 666f 7267  s.svn.sourceforg
+000134a0: 652e 6e65 742c 2066 696c 6573 7973 7465  e.net, filesyste
+000134b0: 6d20 7061 7468 2020 2020 2020 2020 2020  m path          
 000134c0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 000134d0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000134e0: 2020 2020 2020 2020 2020 2020 2072 6570               rep
-000134f0: 6f73 6974 6f72 7920 2868 7474 703a 2f2f  ository (http://
-00013500: 7376 6e2e 636f 6465 2e73 662e 6e65 742f  svn.code.sf.net/
-00013510: 702f 646f 6375 7469 6c73 2f63 6f64 652f  p/docutils/code/
-00013520: 292c 2020 2020 2020 2020 2020 2020 2020  ),              
+000134e0: 2020 2020 2020 2020 202f 7376 6e72 6f6f           /svnroo
+000134f0: 742f 646f 6375 7469 6c73 292c 2077 686f  t/docutils), who
+00013500: 7365 2049 6e74 6572 6e65 7420 7765 6220  se Internet web 
+00013510: 696e 7465 7266 6163 6520 6973 206c 6f63  interface is loc
+00013520: 6174 6564 2061 7420 2020 2020 2020 2020  ated at         
 00013530: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00013540: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00013550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013560: 2020 2020 2020 2020 7768 6f73 6520 496e          whose In
-00013570: 7465 726e 6574 2077 6562 2069 6e74 6572  ternet web inter
-00013580: 6661 6365 2069 7320 6c6f 6361 7465 6420  face is located 
-00013590: 6174 2020 2020 2020 2020 2020 2020 2020  at              
-000135a0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00013550: 2020 2020 203c 6874 7470 3a2f 2f64 6f63       <http://doc
+00013560: 7574 696c 732e 7376 6e2e 736f 7572 6365  utils.svn.source
+00013570: 666f 7267 652e 6e65 742f 7669 6577 7663  forge.net/viewvc
+00013580: 2f64 6f63 7574 696c 732f 3e2e 2020 4669  /docutils/>.  Fi
+00013590: 6c65 7320 6465 6469 6361 7465 6420 746f  les dedicated to
+000135a0: 2074 6865 2020 2020 2020 207c 0a7c 2020   the       |.|  
 000135b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000135c0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-000135d0: 203c 6874 7470 733a 2f2f 736f 7572 6365   <https://source
-000135e0: 666f 7267 652e 6e65 742f 702f 646f 6375  forge.net/p/docu
-000135f0: 7469 6c73 2f63 6f64 653e 2e20 2046 696c  tils/code>.  Fil
-00013600: 6573 2064 6564 6963 6174 6564 2074 6f20  es dedicated to 
-00013610: 7468 6520 2020 2020 2020 2020 2020 2020  the             
+000135d0: 7075 626c 6963 2064 6f6d 6169 6e20 6d61  public domain ma
+000135e0: 7920 6265 2069 6465 6e74 6966 6965 6420  y be identified 
+000135f0: 6279 2074 6865 2069 6e63 6c75 7369 6f6e  by the inclusion
+00013600: 2c20 6e65 6172 2074 6865 2062 6567 696e  , near the begin
+00013610: 6e69 6e67 2020 2020 2020 2020 2020 2020  ning            
 00013620: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00013630: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00013640: 2020 2020 2070 7562 6c69 6320 646f 6d61       public doma
-00013650: 696e 206d 6179 2062 6520 6964 656e 7469  in may be identi
-00013660: 6669 6564 2062 7920 7468 6520 696e 636c  fied by the incl
-00013670: 7573 696f 6e2c 206e 6561 7220 7468 6520  usion, near the 
-00013680: 6265 6769 6e6e 696e 6720 2020 2020 2020  beginning       
+00013640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013650: 206f 6620 6561 6368 2066 696c 652c 206f   of each file, o
+00013660: 6620 6120 6465 636c 6172 6174 696f 6e20  f a declaration 
+00013670: 6f66 2074 6865 2066 6f72 6d3a 3a20 2020  of the form::   
+00013680: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013690: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 000136a0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 000136b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136c0: 2020 2020 2020 6f66 2065 6163 6820 6669        of each fi
-000136d0: 6c65 2c20 6f66 2061 2064 6563 6c61 7261  le, of a declara
-000136e0: 7469 6f6e 206f 6620 7468 6520 666f 726d  tion of the form
-000136f0: 3a3a 2020 2020 2020 2020 2020 2020 2020  ::              
+000136c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000136f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013700: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00013710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013720: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00013730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013770: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00013730: 2020 436f 7079 7269 6768 743a 2054 6869    Copyright: Thi
+00013740: 7320 646f 6375 6d65 6e74 2f6d 6f64 756c  s document/modul
+00013750: 652f 4454 442f 7374 796c 6573 6865 6574  e/DTD/stylesheet
+00013760: 2f66 696c 652f 6574 632e 2068 6173 2062  /file/etc. has b
+00013770: 6565 6e20 2020 2020 2020 2020 2020 207c  een            |
 00013780: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00013790: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000137a0: 2020 2020 2020 2043 6f70 7972 6967 6874         Copyright
-000137b0: 3a20 5468 6973 2064 6f63 756d 656e 742f  : This document/
-000137c0: 6d6f 6475 6c65 2f44 5444 2f73 7479 6c65  module/DTD/style
-000137d0: 7368 6565 742f 6669 6c65 2f65 7463 2e20  sheet/file/etc. 
-000137e0: 6861 7320 6265 656e 2020 2020 2020 2020  has been        
+000137a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000137c0: 6c61 6365 6420 696e 2074 6865 2070 7562  laced in the pub
+000137d0: 6c69 6320 646f 6d61 696e 2e20 2020 2020  lic domain.     
+000137e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000137f0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00013800: 2020 2020 2020 2020 2020 207c 2020 2020             |    
 00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013830: 2020 2020 706c 6163 6564 2069 6e20 7468      placed in th
-00013840: 6520 7075 626c 6963 2064 6f6d 6169 6e2e  e public domain.
+00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013860: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00013870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013880: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00013890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138d0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00013880: 7c20 2020 2020 2020 2020 2020 2044 6564  |            Ded
+00013890: 6963 6174 6f72 206d 616b 6573 2074 6869  icator makes thi
+000138a0: 7320 6465 6469 6361 7469 6f6e 2066 6f72  s dedication for
+000138b0: 2074 6865 2062 656e 6566 6974 206f 6620   the benefit of 
+000138c0: 7468 6520 7075 626c 6963 2061 7420 6c61  the public at la
+000138d0: 7267 6520 2020 2020 2020 2020 2020 7c0a  rge           |.
 000138e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 000138f0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00013900: 2020 4465 6469 6361 746f 7220 6d61 6b65    Dedicator make
-00013910: 7320 7468 6973 2064 6564 6963 6174 696f  s this dedicatio
-00013920: 6e20 666f 7220 7468 6520 6265 6e65 6669  n for the benefi
-00013930: 7420 6f66 2074 6865 2070 7562 6c69 6320  t of the public 
-00013940: 6174 206c 6172 6765 2020 2020 2020 2020  at large        
+00013900: 2020 2061 6e64 2074 6f20 7468 6520 6465     and to the de
+00013910: 7472 696d 656e 7420 6f66 2044 6564 6963  triment of Dedic
+00013920: 6174 6f72 2773 2068 6569 7273 2061 6e64  ator's heirs and
+00013930: 2073 7563 6365 7373 6f72 732e 2020 4465   successors.  De
+00013940: 6469 6361 746f 7220 2020 2020 2020 2020  dicator         
 00013950: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00013960: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00013970: 2020 2020 2020 2020 616e 6420 746f 2074          and to t
-00013980: 6865 2064 6574 7269 6d65 6e74 206f 6620  he detriment of 
-00013990: 4465 6469 6361 746f 7227 7320 6865 6972  Dedicator's heir
-000139a0: 7320 616e 6420 7375 6363 6573 736f 7273  s and successors
-000139b0: 2e20 2044 6564 6963 6174 6f72 2020 2020  .  Dedicator    
+00013970: 2020 2020 2020 2020 2020 696e 7465 6e64            intend
+00013980: 7320 7468 6973 2064 6564 6963 6174 696f  s this dedicatio
+00013990: 6e20 746f 2062 6520 616e 206f 7665 7274  n to be an overt
+000139a0: 2061 6374 206f 6620 7265 6c69 6e71 7569   act of relinqui
+000139b0: 7368 6d65 6e74 2069 6e20 2020 2020 2020  shment in       
 000139c0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 000139d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000139e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000139f0: 6e74 656e 6473 2074 6869 7320 6465 6469  ntends this dedi
-00013a00: 6361 7469 6f6e 2074 6f20 6265 2061 6e20  cation to be an 
-00013a10: 6f76 6572 7420 6163 7420 6f66 2072 656c  overt act of rel
-00013a20: 696e 7175 6973 686d 656e 7420 696e 2020  inquishment in  
+000139e0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000139f0: 6572 7065 7475 6974 7920 6f66 2061 6c6c  erpetuity of all
+00013a00: 2070 7265 7365 6e74 2061 6e64 2066 7574   present and fut
+00013a10: 7572 6520 7269 6768 7473 2075 6e64 6572  ure rights under
+00013a20: 2063 6f70 7972 6967 6874 206c 6177 2c20   copyright law, 
 00013a30: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00013a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013a50: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00013a60: 2020 2020 7065 7270 6574 7569 7479 206f      perpetuity o
-00013a70: 6620 616c 6c20 7072 6573 656e 7420 616e  f all present an
-00013a80: 6420 6675 7475 7265 2072 6967 6874 7320  d future rights 
-00013a90: 756e 6465 7220 636f 7079 7269 6768 7420  under copyright 
-00013aa0: 6c61 772c 2020 2020 2020 2020 2020 2020  law,            
+00013a60: 2077 6865 7468 6572 2076 6573 7465 6420   whether vested 
+00013a70: 6f72 2063 6f6e 7469 6e67 656e 742c 2069  or contingent, i
+00013a80: 6e20 7468 6520 576f 726b 2e20 2044 6564  n the Work.  Ded
+00013a90: 6963 6174 6f72 2075 6e64 6572 7374 616e  icator understan
+00013aa0: 6473 2074 6861 7420 2020 2020 2020 2020  ds that         
 00013ab0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00013ac0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00013ad0: 2020 2020 2020 7768 6574 6865 7220 7665        whether ve
-00013ae0: 7374 6564 206f 7220 636f 6e74 696e 6765  sted or continge
-00013af0: 6e74 2c20 696e 2074 6865 2057 6f72 6b2e  nt, in the Work.
-00013b00: 2020 4465 6469 6361 746f 7220 756e 6465    Dedicator unde
-00013b10: 7273 7461 6e64 7320 7468 6174 2020 2020  rstands that    
+00013ad0: 2020 2020 2020 2073 7563 6820 7265 6c69         such reli
+00013ae0: 6e71 7569 7368 6d65 6e74 206f 6620 616c  nquishment of al
+00013af0: 6c20 7269 6768 7473 2069 6e63 6c75 6465  l rights include
+00013b00: 7320 7468 6520 7265 6c69 6e71 7569 7368  s the relinquish
+00013b10: 6d65 6e74 206f 6620 616c 6c20 2020 2020  ment of all     
 00013b20: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00013b30: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00013b40: 2020 2020 2020 2020 2020 2020 7375 6368              such
-00013b50: 2072 656c 696e 7175 6973 686d 656e 7420   relinquishment 
-00013b60: 6f66 2061 6c6c 2072 6967 6874 7320 696e  of all rights in
-00013b70: 636c 7564 6573 2074 6865 2072 656c 696e  cludes the relin
-00013b80: 7175 6973 686d 656e 7420 6f66 2061 6c6c  quishment of all
+00013b40: 2020 2020 2020 2020 2020 2020 7269 6768              righ
+00013b50: 7473 2074 6f20 656e 666f 7263 6520 2862  ts to enforce (b
+00013b60: 7920 6c61 7773 7569 7420 6f72 206f 7468  y lawsuit or oth
+00013b70: 6572 7769 7365 2920 7468 6f73 6520 636f  erwise) those co
+00013b80: 7079 7269 6768 7473 2069 6e20 7468 6520  pyrights in the 
 00013b90: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00013ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013bb0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00013bc0: 2072 6967 6874 7320 746f 2065 6e66 6f72   rights to enfor
-00013bd0: 6365 2028 6279 206c 6177 7375 6974 206f  ce (by lawsuit o
-00013be0: 7220 6f74 6865 7277 6973 6529 2074 686f  r otherwise) tho
-00013bf0: 7365 2063 6f70 7972 6967 6874 7320 696e  se copyrights in
-00013c00: 2074 6865 2020 2020 2020 2020 2020 2020   the            
+00013bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013be0: 576f 726b 2e20 2020 2020 2020 2020 2020  Work.           
+00013bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013c10: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00013c20: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
 00013c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c50: 2020 2020 2057 6f72 6b2e 2020 2020 2020       Work.      
+00013c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013c80: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00013c90: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ca0: 2020 2020 2020 2020 2020 4465 6469 6361            Dedica
+00013cb0: 746f 7220 7265 636f 676e 697a 6573 2074  tor recognizes t
+00013cc0: 6861 742c 206f 6e63 6520 706c 6163 6564  hat, once placed
+00013cd0: 2069 6e20 7468 6520 7075 626c 6963 2064   in the public d
+00013ce0: 6f6d 6169 6e2c 2074 6865 2057 6f72 6b20  omain, the Work 
 00013cf0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00013d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d10: 2020 7c20 2020 2020 2020 2020 2020 2044    |            D
-00013d20: 6564 6963 6174 6f72 2072 6563 6f67 6e69  edicator recogni
-00013d30: 7a65 7320 7468 6174 2c20 6f6e 6365 2070  zes that, once p
-00013d40: 6c61 6365 6420 696e 2074 6865 2070 7562  laced in the pub
-00013d50: 6c69 6320 646f 6d61 696e 2c20 7468 6520  lic domain, the 
-00013d60: 576f 726b 2020 2020 2020 2020 2020 2020  Work            
+00013d10: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00013d20: 6d61 7920 6265 2066 7265 656c 7920 7265  may be freely re
+00013d30: 7072 6f64 7563 6564 2c20 6469 7374 7269  produced, distri
+00013d40: 6275 7465 642c 2074 7261 6e73 6d69 7474  buted, transmitt
+00013d50: 6564 2c20 7573 6564 2c20 6d6f 6469 6669  ed, used, modifi
+00013d60: 6564 2c20 2020 2020 2020 2020 2020 2020  ed,             
 00013d70: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00013d80: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00013d90: 2020 2020 206d 6179 2062 6520 6672 6565       may be free
-00013da0: 6c79 2072 6570 726f 6475 6365 642c 2064  ly reproduced, d
-00013db0: 6973 7472 6962 7574 6564 2c20 7472 616e  istributed, tran
-00013dc0: 736d 6974 7465 642c 2075 7365 642c 206d  smitted, used, m
-00013dd0: 6f64 6966 6965 642c 2020 2020 2020 2020  odified,        
+00013d90: 2020 2020 2020 2020 6275 696c 7420 7570          built up
+00013da0: 6f6e 2c20 6f72 206f 7468 6572 7769 7365  on, or otherwise
+00013db0: 2065 7870 6c6f 6974 6564 2062 7920 616e   exploited by an
+00013dc0: 796f 6e65 2066 6f72 2061 6e79 2070 7572  yone for any pur
+00013dd0: 706f 7365 2c20 2020 2020 2020 2020 2020  pose,           
 00013de0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00013df0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00013e00: 2020 2020 2020 2020 2020 2020 2062 7569               bui
-00013e10: 6c74 2075 706f 6e2c 206f 7220 6f74 6865  lt upon, or othe
-00013e20: 7277 6973 6520 6578 706c 6f69 7465 6420  rwise exploited 
-00013e30: 6279 2061 6e79 6f6e 6520 666f 7220 616e  by anyone for an
-00013e40: 7920 7075 7270 6f73 652c 2020 2020 2020  y purpose,      
+00013e00: 2020 2020 2020 2020 2020 2063 6f6d 6d65             comme
+00013e10: 7263 6961 6c20 6f72 206e 6f6e 2d63 6f6d  rcial or non-com
+00013e20: 6d65 7263 6961 6c2c 2061 6e64 2069 6e20  mercial, and in 
+00013e30: 616e 7920 7761 792c 2069 6e63 6c75 6469  any way, includi
+00013e40: 6e67 2062 7920 6d65 7468 6f64 7320 2020  ng by methods   
 00013e50: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00013e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013e70: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00013e80: 636f 6d6d 6572 6369 616c 206f 7220 6e6f  commercial or no
-00013e90: 6e2d 636f 6d6d 6572 6369 616c 2c20 616e  n-commercial, an
-00013ea0: 6420 696e 2061 6e79 2077 6179 2c20 696e  d in any way, in
-00013eb0: 636c 7564 696e 6720 6279 206d 6574 686f  cluding by metho
-00013ec0: 6473 2020 2020 2020 2020 2020 2020 207c  ds             |
+00013e80: 2020 2020 2020 2020 2020 7468 6174 2068            that h
+00013e90: 6176 6520 6e6f 7420 7965 7420 6265 656e  ave not yet been
+00013ea0: 2069 6e76 656e 7465 6420 6f72 2063 6f6e   invented or con
+00013eb0: 6365 6976 6564 2e20 2020 2020 2020 2020  ceived.         
+00013ec0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00013ed0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00013ee0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00013ef0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00013f00: 6861 7420 6861 7665 206e 6f74 2079 6574  hat have not yet
-00013f10: 2062 6565 6e20 696e 7665 6e74 6564 206f   been invented o
-00013f20: 7220 636f 6e63 6569 7665 642e 2020 2020  r conceived.    
+00013ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013f40: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00013f50: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00013f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f60: 2020 2020 2020 2020 2020 2854 6869 7320            (This 
+00013f70: 6465 6469 6361 7469 6f6e 2069 7320 6465  dedication is de
+00013f80: 7269 7665 6420 6672 6f6d 2074 6865 2074  rived from the t
+00013f90: 6578 7420 6f66 2074 6865 2060 4372 6561  ext of the `Crea
+00013fa0: 7469 7665 2043 6f6d 6d6f 6e73 2020 2020  tive Commons    
 00013fb0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013fd0: 7c20 2020 2020 2020 2020 2020 2020 2028  |              (
-00013fe0: 5468 6973 2064 6564 6963 6174 696f 6e20  This dedication 
-00013ff0: 6973 2064 6572 6976 6564 2066 726f 6d20  is derived from 
-00014000: 7468 6520 7465 7874 206f 6620 7468 6520  the text of the 
-00014010: 6043 7265 6174 6976 6520 436f 6d6d 6f6e  `Creative Common
-00014020: 7320 2020 2020 2020 2020 2020 2020 7c0a  s             |.
+00013fd0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00013fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013ff0: 5075 626c 6963 2044 6f6d 6169 6e20 4465  Public Domain De
+00014000: 6469 6361 7469 6f6e 602e 205b 235d 5f29  dication`. [#]_)
+00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014020: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00014030: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00014040: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 00014050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014060: 2020 2020 2050 7562 6c69 6320 446f 6d61       Public Doma
-00014070: 696e 2044 6564 6963 6174 696f 6e60 2e20  in Dedication`. 
-00014080: 5b23 5d5f 2920 2020 2020 2020 2020 2020  [#]_)           
+00014060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000140a0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 000140b0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000140c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000140c0: 2020 2020 2020 2020 2e2e 205b 235d 2043          .. [#] C
+000140d0: 7265 6174 6976 6520 436f 6d6d 6f6e 7320  reative Commons 
+000140e0: 6861 7320 6072 6574 6972 6564 2074 6869  has `retired thi
+000140f0: 7320 6c65 6761 6c20 746f 6f6c 605f 5f20  s legal tool`__ 
+00014100: 616e 6420 646f 6573 206e 6f74 2020 2020  and does not    
 00014110: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00014120: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00014130: 2020 2020 2020 2020 2020 2020 202e 2e20               .. 
-00014140: 5b23 5d20 4372 6561 7469 7665 2043 6f6d  [#] Creative Com
-00014150: 6d6f 6e73 2068 6173 2060 7265 7469 7265  mons has `retire
-00014160: 6420 7468 6973 206c 6567 616c 2074 6f6f  d this legal too
-00014170: 6c60 5f5f 2061 6e64 2064 6f65 7320 6e6f  l`__ and does no
-00014180: 7420 2020 2020 2020 2020 2020 207c 0a7c  t            |.|
+00014130: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00014140: 6563 6f6d 6d65 6e64 2074 6861 7420 6974  ecommend that it
+00014150: 2062 6520 6170 706c 6965 6420 746f 2077   be applied to w
+00014160: 6f72 6b73 3a20 5468 6973 2074 6f6f 6c20  orks: This tool 
+00014170: 6973 2062 6173 6564 206f 6e20 556e 6974  is based on Unit
+00014180: 6564 2020 2020 2020 2020 2020 207c 0a7c  ed           |.|
 00014190: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000141a0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-000141b0: 2020 2020 7265 636f 6d6d 656e 6420 7468      recommend th
-000141c0: 6174 2069 7420 6265 2061 7070 6c69 6564  at it be applied
-000141d0: 2074 6f20 776f 726b 733a 2054 6869 7320   to works: This 
-000141e0: 746f 6f6c 2069 7320 6261 7365 6420 6f6e  tool is based on
-000141f0: 2055 6e69 7465 6420 2020 2020 2020 2020   United         
+000141b0: 2020 5374 6174 6573 206c 6177 2061 6e64    States law and
+000141c0: 206d 6179 206e 6f74 2062 6520 6170 706c   may not be appl
+000141d0: 6963 6162 6c65 206f 7574 7369 6465 2074  icable outside t
+000141e0: 6865 2055 532e 2046 6f72 2064 6564 6963  he US. For dedic
+000141f0: 6174 696e 6720 6e65 7720 2020 2020 2020  ating new       
 00014200: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00014210: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00014220: 2020 2020 2020 2053 7461 7465 7320 6c61         States la
-00014230: 7720 616e 6420 6d61 7920 6e6f 7420 6265  w and may not be
-00014240: 2061 7070 6c69 6361 626c 6520 6f75 7473   applicable outs
-00014250: 6964 6520 7468 6520 5553 2e20 466f 7220  ide the US. For 
-00014260: 6465 6469 6361 7469 6e67 206e 6577 2020  dedicating new  
+00014220: 2020 2020 2020 2077 6f72 6b73 2074 6f20         works to 
+00014230: 7468 6520 7075 626c 6963 2064 6f6d 6169  the public domai
+00014240: 6e2c 2043 7265 6174 6976 6520 436f 6d6d  n, Creative Comm
+00014250: 6f6e 7320 7265 636f 6d6d 656e 6420 7468  ons recommend th
+00014260: 6520 7265 706c 6163 656d 656e 7420 2020  e replacement   
 00014270: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00014280: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00014290: 2020 2020 2020 2020 2020 2020 776f 726b              work
-000142a0: 7320 746f 2074 6865 2070 7562 6c69 6320  s to the public 
-000142b0: 646f 6d61 696e 2c20 4372 6561 7469 7665  domain, Creative
-000142c0: 2043 6f6d 6d6f 6e73 2072 6563 6f6d 6d65   Commons recomme
-000142d0: 6e64 2074 6865 2072 6570 6c61 6365 6d65  nd the replaceme
-000142e0: 6e74 2020 2020 2020 2020 2020 7c0a 7c20  nt          |.| 
+00014290: 2020 2020 2020 2020 2020 2020 5075 626c              Publ
+000142a0: 6963 2044 6f6d 6169 6e20 4465 6469 6361  ic Domain Dedica
+000142b0: 7469 6f6e 2043 4330 5f20 2843 4320 7a65  tion CC0_ (CC ze
+000142c0: 726f 2c20 224e 6f20 5269 6768 7473 2052  ro, "No Rights R
+000142d0: 6573 6572 7665 6422 292e 2053 6f20 646f  eserved"). So do
+000142e0: 6573 2020 2020 2020 2020 2020 7c0a 7c20  es          |.| 
 000142f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014300: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00014310: 2050 7562 6c69 6320 446f 6d61 696e 2044   Public Domain D
-00014320: 6564 6963 6174 696f 6e20 4343 305f 2028  edication CC0_ (
-00014330: 4343 207a 6572 6f2c 2022 4e6f 2052 6967  CC zero, "No Rig
-00014340: 6874 7320 5265 7365 7276 6564 2229 2e20  hts Reserved"). 
-00014350: 536f 2064 6f65 7320 2020 2020 2020 2020  So does         
+00014310: 2020 2020 2020 2020 2020 2074 6865 2046             the F
+00014320: 7265 6520 536f 6674 7761 7265 2046 6f75  ree Software Fou
+00014330: 6e64 6174 696f 6e20 696e 2069 7473 206c  ndation in its l
+00014340: 6963 656e 7365 2d6c 6973 745f 2e20 2020  icense-list_.   
+00014350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014360: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00014370: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
 00014380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014390: 7468 6520 4672 6565 2053 6f66 7477 6172  the Free Softwar
-000143a0: 6520 466f 756e 6461 7469 6f6e 2069 6e20  e Foundation in 
-000143b0: 6974 7320 6c69 6365 6e73 652d 6c69 7374  its license-list
-000143c0: 5f2e 2020 2020 2020 2020 2020 2020 2020  _.              
+00014390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000143d0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 000143e0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 000143f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014400: 2020 2020 2020 205f 5f20 2068 7474 703a         __  http:
+00014410: 2f2f 6372 6561 7469 7665 636f 6d6d 6f6e  //creativecommon
+00014420: 732e 6f72 672f 7265 7469 7265 646c 6963  s.org/retiredlic
+00014430: 656e 7365 7320 2020 2020 2020 2020 2020  enses           
 00014440: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00014450: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014460: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00014470: 2020 2020 2020 2020 2020 2020 5f5f 2020              __  
-00014480: 6874 7470 3a2f 2f63 7265 6174 6976 6563  http://creativec
-00014490: 6f6d 6d6f 6e73 2e6f 7267 2f72 6574 6972  ommons.org/retir
-000144a0: 6564 6c69 6365 6e73 6573 2020 2020 2020  edlicenses      
+00014470: 2020 2020 2020 2020 2020 2020 202e 2e20               .. 
+00014480: 5f43 4330 3a20 6874 7470 3a2f 2f63 7265  _CC0: http://cre
+00014490: 6174 6976 6563 6f6d 6d6f 6e73 2e6f 7267  ativecommons.org
+000144a0: 2f61 626f 7574 2f63 6330 2020 2020 2020  /about/cc0      
 000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000144c0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 000144d0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 000144e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144f0: 2020 2e2e 205f 4343 303a 2068 7474 703a    .. _CC0: http:
-00014500: 2f2f 6372 6561 7469 7665 636f 6d6d 6f6e  //creativecommon
-00014510: 732e 6f72 672f 6162 6f75 742f 6363 3020  s.org/about/cc0 
+000144f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014530: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00014540: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00014550: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014570: 2020 2020 2020 2045 7863 6570 7469 6f6e         Exception
+00014580: 7320 2020 2020 2020 2020 2020 2020 2020  s               
 00014590: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000145a0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 000145b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000145c0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
 000145d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000145e0: 2020 2020 2020 2020 2020 2020 4578 6365              Exce
-000145f0: 7074 696f 6e73 2020 2020 2020 2020 2020  ptions          
+000145e0: 2020 2020 2020 2020 2020 2020 3d3d 3d3d              ====
+000145f0: 3d3d 3d3d 3d3d 2020 2020 2020 2020 2020  ======          
 00014600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014610: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00014620: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00014630: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 00014640: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014660: 203d 3d3d 3d3d 3d3d 3d3d 3d20 2020 2020   ==========     
+00014660: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014670: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014680: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014690: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 000146a0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000146b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000146f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000146b0: 2020 2020 2020 2020 2020 2020 2054 6865               The
+000146c0: 2065 7863 6570 7469 6f6e 7320 746f 2074   exceptions to t
+000146d0: 6865 2060 5075 626c 6963 2044 6f6d 6169  he `Public Domai
+000146e0: 6e20 4465 6469 6361 7469 6f6e 605f 2061  n Dedication`_ a
+000146f0: 626f 7665 2061 7265 3a20 2020 2020 2020  bove are:       
 00014700: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00014710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014720: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00014730: 2020 5468 6520 6578 6365 7074 696f 6e73    The exceptions
-00014740: 2074 6f20 7468 6520 6050 7562 6c69 6320   to the `Public 
-00014750: 446f 6d61 696e 2044 6564 6963 6174 696f  Domain Dedicatio
-00014760: 6e60 5f20 6162 6f76 6520 6172 653a 2020  n`_ above are:  
+00014730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014760: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014770: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00014780: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00014790: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000147b0: 2020 2020 202a 2064 6f63 7574 696c 732f       * docutils/
+000147c0: 7574 696c 732f 736d 6172 7471 756f 7465  utils/smartquote
+000147d0: 732e 7079 2020 2020 2020 2020 2020 2020  s.py            
 000147e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000147f0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00014800: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 00014810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014820: 2020 2020 2020 2020 2020 2a20 646f 6375            * docu
-00014830: 7469 6c73 2f75 7469 6c73 2f73 6d61 7274  tils/utils/smart
-00014840: 7175 6f74 6573 2e70 7920 2020 2020 2020  quotes.py       
+00014820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014840: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014850: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014860: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00014870: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00014880: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148d0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-000148e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148f0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+000148a0: 2043 6f70 7972 6967 6874 20c2 a920 3230   Copyright .. 20
+000148b0: 3131 2047 c3bc 6e74 6572 204d 696c 6465  11 G..nter Milde
+000148c0: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
+000148d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000148e0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+000148f0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014910: 2020 2020 2020 436f 7079 7269 6768 7420        Copyright 
-00014920: c2a9 2032 3031 3120 47c3 bc6e 7465 7220  .. 2011 G..nter 
-00014930: 4d69 6c64 652c 2020 2020 2020 2020 2020  Milde,          
+00014910: 2020 6261 7365 6420 6f6e 2060 536d 6172    based on `Smar
+00014920: 7479 5061 6e74 7360 5f20 c2a9 2032 3030  tyPants`_ .. 200
+00014930: 3320 4a6f 686e 2047 7275 6265 7220 2020  3 John Gruber   
 00014940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014950: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00014960: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00014970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014980: 2020 2020 2020 2062 6173 6564 206f 6e20         based on 
-00014990: 6053 6d61 7274 7950 616e 7473 605f 20c2  `SmartyPants`_ .
-000149a0: a920 3230 3033 204a 6f68 6e20 4772 7562  . 2003 John Grub
-000149b0: 6572 2020 2020 2020 2020 2020 2020 2020  er              
-000149c0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00014950: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+00014960: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00014970: 2020 2020 2020 2020 2872 656c 6561 7365          (release
+00014980: 6420 756e 6465 7220 6120 2272 6576 6973  d under a "revis
+00014990: 6564 2220 6042 5344 2033 2d43 6c61 7573  ed" `BSD 3-Claus
+000149a0: 6520 4c69 6365 6e73 6560 5f20 696e 636c  e License`_ incl
+000149b0: 7564 6564 2069 6e20 7468 6520 6669 6c65  uded in the file
+000149c0: 2920 2020 2020 2020 2020 7c0a 7c20 2020  )         |.|   
 000149d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149e0: 207c 2020 2020 2020 2020 2020 2028 7265   |           (re
-000149f0: 6c65 6173 6564 2075 6e64 6572 2061 2022  leased under a "
-00014a00: 7265 7669 7365 6422 2060 4253 4420 332d  revised" `BSD 3-
-00014a10: 436c 6175 7365 204c 6963 656e 7365 605f  Clause License`_
-00014a20: 2069 6e63 6c75 6465 6420 696e 2074 6865   included in the
-00014a30: 2066 696c 6529 2020 2020 2020 2020 207c   file)         |
-00014a40: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00014a50: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00014a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a70: 2061 6e64 2073 6d61 7274 7970 616e 7473   and smartypants
-00014a80: 2e70 7920 c2a9 2032 3030 342c 2032 3030  .py .. 2004, 200
-00014a90: 3720 4368 6164 204d 696c 6c65 722e 2020  7 Chad Miller.  
-00014aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149e0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+000149f0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
+00014a00: 736d 6172 7479 7061 6e74 732e 7079 20c2  smartypants.py .
+00014a10: a920 3230 3034 2c20 3230 3037 2043 6861  . 2004, 2007 Cha
+00014a20: 6420 4d69 6c6c 6572 2e20 2020 2020 2020  d Miller.       
+00014a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a40: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00014a50: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00014a60: 2020 2020 2020 2020 2020 2020 5265 6c65              Rele
+00014a70: 6173 6564 2075 6e64 6572 2074 6865 2074  ased under the t
+00014a80: 6572 6d73 206f 6620 7468 6520 6042 5344  erms of the `BSD
+00014a90: 2032 2d43 6c61 7573 6520 4c69 6365 6e73   2-Clause Licens
+00014aa0: 6560 5f20 2020 2020 2020 2020 2020 2020  e`_             
 00014ab0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00014ac0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00014ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ae0: 2052 656c 6561 7365 6420 756e 6465 7220   Released under 
-00014af0: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
-00014b00: 2060 4253 4420 322d 436c 6175 7365 204c   `BSD 2-Clause L
-00014b10: 6963 656e 7365 605f 2020 2020 2020 2020  icense`_        
+00014ae0: 2020 2020 2020 2860 6c6f 6361 6c20 636f        (`local co
+00014af0: 7079 203c 6c69 6365 6e73 6573 2f42 5344  py <licenses/BSD
+00014b00: 2d32 2d43 6c61 7573 652e 7478 743e 605f  -2-Clause.txt>`_
+00014b10: 5f29 2e20 2020 2020 2020 2020 2020 2020  _).             
 00014b20: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00014b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014b40: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00014b50: 2020 2020 2020 2020 2020 2028 606c 6f63             (`loc
-00014b60: 616c 2063 6f70 7920 3c6c 6963 656e 7365  al copy <license
-00014b70: 732f 4253 442d 322d 436c 6175 7365 2e74  s/BSD-2-Clause.t
-00014b80: 7874 3e60 5f5f 292e 2020 2020 2020 2020  xt>`__).        
+00014b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014b90: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00014ba0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00014bb0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00014bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bc0: 2020 2020 2020 202e 2e20 5f53 6d61 7274         .. _Smart
+00014bd0: 7950 616e 7473 3a20 6874 7470 3a2f 2f64  yPants: http://d
+00014be0: 6172 696e 6766 6972 6562 616c 6c2e 6e65  aringfireball.ne
+00014bf0: 742f 7072 6f6a 6563 7473 2f73 6d61 7274  t/projects/smart
+00014c00: 7970 616e 7473 2f20 2020 2020 2020 2020  ypants/         
 00014c10: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00014c20: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00014c30: 2020 2020 2020 2020 2020 2020 2e2e 205f              .. _
-00014c40: 536d 6172 7479 5061 6e74 733a 2068 7474  SmartyPants: htt
-00014c50: 703a 2f2f 6461 7269 6e67 6669 7265 6261  p://daringfireba
-00014c60: 6c6c 2e6e 6574 2f70 726f 6a65 6374 732f  ll.net/projects/
-00014c70: 736d 6172 7479 7061 6e74 732f 2020 2020  smartypants/    
+00014c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014c80: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00014c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014ca0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00014cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014cb0: 2020 2020 2020 2020 2020 2020 202a 2064               * d
+00014cc0: 6f63 7574 696c 732f 7574 696c 732f 6d61  ocutils/utils/ma
+00014cd0: 7468 2f6c 6174 6578 326d 6174 686d 6c2e  th/latex2mathml.
+00014ce0: 7079 2020 2020 2020 2020 2020 2020 2020  py              
 00014cf0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00014d00: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00014d10: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 00014d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d30: 2020 2a20 646f 6375 7469 6c73 2f75 7469    * docutils/uti
-00014d40: 6c73 2f6d 6174 682f 6c61 7465 7832 6d61  ls/math/latex2ma
-00014d50: 7468 6d6c 2e70 7920 2020 2020 2020 2020  thml.py         
+00014d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014d70: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00014d80: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 00014d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014de0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00014df0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00014e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e10: 2020 2020 2020 2020 436f 7079 7269 6768          Copyrigh
-00014e20: 7420 c2a9 204a 656e 7320 4ac3 b872 6765  t .. Jens J..rge
-00014e30: 6e20 4d6f 7274 656e 7365 6e2c 2047 c3bc  n Mortensen, G..
-00014e40: 6e74 6572 204d 696c 6465 2e20 2020 2020  nter Milde.     
+00014da0: 2020 2043 6f70 7972 6967 6874 20c2 a920     Copyright .. 
+00014db0: 4a65 6e73 204a c3b8 7267 656e 204d 6f72  Jens J..rgen Mor
+00014dc0: 7465 6e73 656e 2c20 47c3 bc6e 7465 7220  tensen, G..nter 
+00014dd0: 4d69 6c64 652e 2020 2020 2020 2020 2020  Milde.          
+00014de0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00014df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e00: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00014e10: 2020 2020 2020 2052 656c 6561 7365 6420         Released 
+00014e20: 756e 6465 7220 7468 6520 7465 726d 7320  under the terms 
+00014e30: 6f66 2074 6865 2060 4253 4420 322d 436c  of the `BSD 2-Cl
+00014e40: 6175 7365 204c 6963 656e 7365 605f 2020  ause License`_  
 00014e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014e60: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00014e70: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00014e80: 2020 2020 2020 2020 2020 2020 5265 6c65              Rele
-00014e90: 6173 6564 2075 6e64 6572 2074 6865 2074  ased under the t
-00014ea0: 6572 6d73 206f 6620 7468 6520 6042 5344  erms of the `BSD
-00014eb0: 2032 2d43 6c61 7573 6520 4c69 6365 6e73   2-Clause Licens
-00014ec0: 6560 5f20 2020 2020 2020 2020 2020 2020  e`_             
+00014e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e90: 2028 606c 6f63 616c 2063 6f70 7920 3c6c   (`local copy <l
+00014ea0: 6963 656e 7365 732f 4253 442d 322d 436c  icenses/BSD-2-Cl
+00014eb0: 6175 7365 2e74 7874 3e60 5f5f 292e 2020  ause.txt>`__).  
+00014ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014ed0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00014ee0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00014ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f00: 2020 2020 2020 2860 6c6f 6361 6c20 636f        (`local co
-00014f10: 7079 203c 6c69 6365 6e73 6573 2f42 5344  py <licenses/BSD
-00014f20: 2d32 2d43 6c61 7573 652e 7478 743e 605f  -2-Clause.txt>`_
-00014f30: 5f29 2e20 2020 2020 2020 2020 2020 2020  _).             
+00014f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014f40: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00014f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00014f60: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00014f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f70: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+00014f80: 2064 6f63 7574 696c 732f 7574 696c 732f   docutils/utils/
+00014f90: 6d61 7468 2f6d 6174 6832 6874 6d6c 2e70  math/math2html.p
+00014fa0: 792c 2020 2020 2020 2020 2020 2020 2020  y,              
 00014fb0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00014fc0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00014fd0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 00014fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ff0: 2020 2020 2a20 646f 6375 7469 6c73 2f75      * docutils/u
-00015000: 7469 6c73 2f6d 6174 682f 6d61 7468 3268  tils/math/math2h
-00015010: 746d 6c2e 7079 2c20 2020 2020 2020 2020  tml.py,         
+00014ff0: 2020 2064 6f63 7574 696c 732f 7772 6974     docutils/writ
+00015000: 6572 732f 6874 6d6c 355f 706f 6c79 676c  ers/html5_polygl
+00015010: 6f74 2f6d 6174 682e 6373 7320 2020 2020  ot/math.css     
 00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015030: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00015040: 2020 2020 2020 2020 2020 207c 2020 2020             |    
 00015050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015060: 2020 2020 2020 2020 646f 6375 7469 6c73          docutils
-00015070: 2f77 7269 7465 7273 2f68 746d 6c35 5f70  /writers/html5_p
-00015080: 6f6c 7967 6c6f 742f 6d61 7468 2e63 7373  olyglot/math.css
+00015060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000150a0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 000150b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000150c0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015110: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00015120: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00015130: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00015140: 2020 2020 2020 2020 2020 436f 7079 7269            Copyri
-00015150: 6768 7420 c2a9 2032 3030 392c 3230 3130  ght .. 2009,2010
-00015160: 2041 6c65 7820 4665 726e c3a1 6e64 657a   Alex Fern..ndez
-00015170: 3b20 3230 3231 2047 c3bc 6e74 6572 204d  ; 2021 G..nter M
-00015180: 696c 6465 2020 2020 2020 2020 2020 2020  ilde            
+000150d0: 2020 2020 2043 6f70 7972 6967 6874 20c2       Copyright .
+000150e0: a920 3230 3039 2c32 3031 3020 416c 6578  . 2009,2010 Alex
+000150f0: 2046 6572 6ec3 a16e 6465 7a3b 2032 3032   Fern..ndez; 202
+00015100: 3120 47c3 bc6e 7465 7220 4d69 6c64 6520  1 G..nter Milde 
+00015110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015120: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00015130: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00015140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015180: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015190: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 000151a0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 000151b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151c0: 2054 6865 7365 2066 696c 6573 2077 6572   These files wer
+000151d0: 6520 7061 7274 206f 6620 654c 7958 6572  e part of eLyXer
+000151e0: 5f2c 2072 656c 6561 7365 6420 756e 6465  _, released unde
+000151f0: 7220 7468 6520 6047 4e55 2020 2020 2020  r the `GNU      
 00015200: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00015210: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015220: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00015230: 2020 2020 2020 5468 6573 6520 6669 6c65        These file
-00015240: 7320 7765 7265 2070 6172 7420 6f66 2065  s were part of e
-00015250: 4c79 5865 725f 2c20 7265 6c65 6173 6564  LyXer_, released
-00015260: 2075 6e64 6572 2074 6865 2060 474e 5520   under the `GNU 
-00015270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015230: 2020 4765 6e65 7261 6c20 5075 626c 6963    General Public
+00015240: 204c 6963 656e 7365 605f 2076 6572 7369   License`_ versi
+00015250: 6f6e 2033 206f 7220 6c61 7465 722e 2054  on 3 or later. T
+00015260: 6865 2061 7574 686f 7220 7265 6c69 6365  he author relice
+00015270: 6e73 6564 2020 2020 2020 2020 2020 2020  nsed            
 00015280: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00015290: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-000152a0: 2020 2020 2020 2047 656e 6572 616c 2050         General P
-000152b0: 7562 6c69 6320 4c69 6365 6e73 6560 5f20  ublic License`_ 
-000152c0: 7665 7273 696f 6e20 3320 6f72 206c 6174  version 3 or lat
-000152d0: 6572 2e20 5468 6520 6175 7468 6f72 2072  er. The author r
-000152e0: 656c 6963 656e 7365 6420 2020 2020 2020  elicensed       
+000152a0: 2020 2020 2020 2020 7468 656d 2066 6f72          them for
+000152b0: 2044 6f63 7574 696c 7320 756e 6465 7220   Docutils under 
+000152c0: 7468 6520 7465 726d 7320 6f66 2074 6865  the terms of the
+000152d0: 2060 4253 4420 322d 436c 6175 7365 204c   `BSD 2-Clause L
+000152e0: 6963 656e 7365 605f 2020 2020 2020 2020  icense`_        
 000152f0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00015300: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00015310: 2020 2020 2020 2020 2020 2020 2074 6865               the
-00015320: 6d20 666f 7220 446f 6375 7469 6c73 2075  m for Docutils u
-00015330: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
-00015340: 6620 7468 6520 6042 5344 2032 2d43 6c61  f the `BSD 2-Cla
-00015350: 7573 6520 4c69 6365 6e73 6560 5f20 2020  use License`_   
+00015310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015320: 2020 2020 2020 2860 6c6f 6361 6c20 636f        (`local co
+00015330: 7079 203c 6c69 6365 6e73 6573 2f42 5344  py <licenses/BSD
+00015340: 2d32 2d43 6c61 7573 652e 7478 743e 605f  -2-Clause.txt>`_
+00015350: 5f29 2e20 2020 2020 2020 2020 2020 2020  _).             
 00015360: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00015370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015380: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00015390: 2020 2020 2020 2020 2020 2028 606c 6f63             (`loc
-000153a0: 616c 2063 6f70 7920 3c6c 6963 656e 7365  al copy <license
-000153b0: 732f 4253 442d 322d 436c 6175 7365 2e74  s/BSD-2-Clause.t
-000153c0: 7874 3e60 5f5f 292e 2020 2020 2020 2020  xt>`__).        
+00015390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000153c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000153d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 000153e0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 000153f0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00015400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015400: 2020 2020 2020 2020 2020 2020 202e 2e20               .. 
+00015410: 5f65 4c79 5865 723a 2068 7474 7073 3a2f  _eLyXer: https:/
+00015420: 2f67 6974 6875 622e 636f 6d2f 616c 6578  /github.com/alex
+00015430: 6665 726e 616e 6465 7a2f 656c 7978 6572  fernandez/elyxer
 00015440: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015450: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00015460: 2020 2020 2020 2020 2020 207c 2020 2020             |    
 00015470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015480: 2020 2e2e 205f 654c 7958 6572 3a20 6874    .. _eLyXer: ht
-00015490: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000154a0: 2f61 6c65 7866 6572 6e61 6e64 657a 2f65  /alexfernandez/e
-000154b0: 6c79 7865 7220 2020 2020 2020 2020 2020  lyxer           
+00015480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000154c0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 000154d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000154e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000154f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000154f0: 2020 2020 2020 2020 2020 2a20 646f 6375            * docu
+00015500: 7469 6c73 2f70 6172 7365 7273 2f72 6563  tils/parsers/rec
+00015510: 6f6d 6d6f 6e6d 6172 6b5f 7772 6170 7065  ommonmark_wrappe
+00015520: 722e 7079 2c20 2020 2020 2020 2020 2020  r.py,           
 00015530: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00015540: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00015550: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015570: 2020 2020 2020 2020 202a 2064 6f63 7574           * docut
-00015580: 696c 732f 5f5f 6d61 696e 5f5f 2e70 792c  ils/__main__.py,
-00015590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015570: 2020 2020 2064 6f63 7574 696c 732f 7574       docutils/ut
+00015580: 696c 732f 6572 726f 725f 7265 706f 7274  ils/error_report
+00015590: 696e 672e 7079 2c20 2020 2020 2020 2020  ing.py,         
 000155a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000155b0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 000155c0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 000155d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000155e0: 2020 2020 2020 2064 6f63 7574 696c 732f         docutils/
-000155f0: 7061 7273 6572 732f 636f 6d6d 6f6e 6d61  parsers/commonma
-00015600: 726b 5f77 7261 7070 6572 2e70 792c 2020  rk_wrapper.py,  
+000155e0: 2020 2020 2020 2020 2020 2064 6f63 7574             docut
+000155f0: 696c 732f 7574 696c 732f 6d61 7468 2f5f  ils/utils/math/_
+00015600: 5f69 6e69 745f 5f2e 7079 2c20 2020 2020  _init__.py,     
 00015610: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015620: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00015630: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00015640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015650: 2020 2020 2020 2020 2020 2064 6f63 7574             docut
-00015660: 696c 732f 7061 7273 6572 732f 7265 636f  ils/parsers/reco
-00015670: 6d6d 6f6e 6d61 726b 5f77 7261 7070 6572  mmonmark_wrapper
-00015680: 2e70 792c 2020 2020 2020 2020 2020 2020  .py,            
+00015650: 2020 2020 2020 2020 2020 2020 2020 646f                do
+00015660: 6375 7469 6c73 2f75 7469 6c73 2f6d 6174  cutils/utils/mat
+00015670: 682f 6c61 7465 7832 6d61 7468 6d6c 2e70  h/latex2mathml.p
+00015680: 792c 2020 2020 2020 2020 2020 2020 2020  y,              
 00015690: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 000156a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000156b0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
 000156c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000156d0: 2020 2020 646f 6375 7469 6c73 2f75 7469      docutils/uti
-000156e0: 6c73 2f65 7272 6f72 5f72 6570 6f72 7469  ls/error_reporti
-000156f0: 6e67 2e70 792c 2020 2020 2020 2020 2020  ng.py,          
+000156d0: 646f 6375 7469 6c73 2f75 7469 6c73 2f6d  docutils/utils/m
+000156e0: 6174 682f 7465 7832 6d61 7468 6d6c 5f65  ath/tex2mathml_e
+000156f0: 7874 6572 6e2e 7079 2c20 2020 2020 2020  xtern.py,       
 00015700: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015710: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00015720: 2020 2020 2020 2020 207c 2020 2020 2020           |      
 00015730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015740: 2020 2020 2020 2020 2020 646f 6375 7469            docuti
-00015750: 6c73 2f75 7469 6c73 2f6d 6174 682f 5f5f  ls/utils/math/__
-00015760: 696e 6974 5f5f 2e70 792c 2020 2020 2020  init__.py,      
+00015740: 2020 2020 2020 2020 646f 6375 7469 6c73          docutils
+00015750: 2f75 7469 6c73 2f70 756e 6374 7561 7469  /utils/punctuati
+00015760: 6f6e 5f63 6861 7273 2e70 792c 2020 2020  on_chars.py,    
 00015770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015780: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00015790: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 000157a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157b0: 2020 2020 2020 2020 2020 2020 2064 6f63               doc
-000157c0: 7574 696c 732f 7574 696c 732f 6d61 7468  utils/utils/math
-000157d0: 2f6c 6174 6578 326d 6174 686d 6c2e 7079  /latex2mathml.py
-000157e0: 2c20 2020 2020 2020 2020 2020 2020 2020  ,               
+000157b0: 2020 2020 2020 2020 2064 6f63 7574 696c           docutil
+000157c0: 732f 7772 6974 6572 732f 6874 6d6c 355f  s/writers/html5_
+000157d0: 706f 6c79 676c 6f74 2f5f 5f69 6e69 745f  polyglot/__init_
+000157e0: 5f2e 7079 2c20 2020 2020 2020 2020 2020  _.py,           
 000157f0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00015800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015810: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00015820: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00015830: 6f63 7574 696c 732f 7574 696c 732f 6d61  ocutils/utils/ma
-00015840: 7468 2f74 6578 326d 6174 686d 6c5f 6578  th/tex2mathml_ex
-00015850: 7465 726e 2e70 792c 2020 2020 2020 2020  tern.py,        
+00015820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015830: 2020 646f 6375 7469 6c73 2f77 7269 7465    docutils/write
+00015840: 7273 2f78 6574 6578 2f5f 5f69 6e69 745f  rs/xetex/__init_
+00015850: 5f2e 7079 2c20 2020 2020 2020 2020 2020  _.py,           
 00015860: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015870: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00015880: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
 00015890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158a0: 2020 2020 2020 2064 6f63 7574 696c 732f         docutils/
-000158b0: 7574 696c 732f 7075 6e63 7475 6174 696f  utils/punctuatio
-000158c0: 6e5f 6368 6172 732e 7079 2c20 2020 2020  n_chars.py,     
+000158a0: 2020 2020 7465 7374 2f74 6573 745f 7061      test/test_pa
+000158b0: 7273 6572 732f 7465 7374 5f72 6563 6f6d  rsers/test_recom
+000158c0: 6d6f 6e6d 6172 6b2f 5c2a 2e70 792c 2020  monmark/\*.py,  
 000158d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000158e0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 000158f0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 00015900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015910: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00015920: 6f63 7574 696c 732f 7574 696c 732f 736d  ocutils/utils/sm
-00015930: 6172 7471 756f 7465 732e 7079 2c20 2020  artquotes.py,   
-00015940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015910: 7465 7374 2f74 6573 745f 7061 7273 6572  test/test_parser
+00015920: 732f 7465 7374 5f72 7374 2f74 6573 745f  s/test_rst/test_
+00015930: 6469 7265 6374 6976 6573 2f74 6573 745f  directives/test_
+00015940: 5f69 6e69 745f 5f2e 7079 2c20 2020 2020  _init__.py,     
 00015950: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00015960: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015970: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00015980: 2020 2020 2020 2020 2020 2020 2064 6f63               doc
-00015990: 7574 696c 732f 7772 6974 6572 732f 6874  utils/writers/ht
-000159a0: 6d6c 355f 706f 6c79 676c 6f74 2f5f 5f69  ml5_polyglot/__i
-000159b0: 6e69 745f 5f2e 7079 2c20 2020 2020 2020  nit__.py,       
-000159c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015980: 2020 2074 6573 742f 7465 7374 5f70 6172     test/test_par
+00015990: 7365 7273 2f74 6573 745f 7273 742f 7465  sers/test_rst/te
+000159a0: 7374 5f64 6972 6563 7469 7665 732f 7465  st_directives/te
+000159b0: 7374 5f63 6f64 655f 7061 7273 696e 672e  st_code_parsing.
+000159c0: 7079 2c20 2020 2020 2020 2020 2020 2020  py,             
 000159d0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 000159e0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-000159f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a00: 2020 2020 2064 6f63 7574 696c 732f 7772       docutils/wr
-00015a10: 6974 6572 732f 6874 6d6c 355f 706f 6c79  iters/html5_poly
-00015a20: 676c 6f74 2f2a 2e63 7373 2c20 2020 2020  glot/*.css,     
-00015a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000159f0: 2020 2020 2020 2020 2074 6573 742f 7465           test/te
+00015a00: 7374 5f70 6172 7365 7273 2f74 6573 745f  st_parsers/test_
+00015a10: 7273 742f 7465 7374 5f6c 696e 655f 6c65  rst/test_line_le
+00015a20: 6e67 7468 5f6c 696d 6974 5f64 6566 6175  ngth_limit_defau
+00015a30: 6c74 2e70 792c 2020 2020 2020 2020 2020  lt.py,          
 00015a40: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00015a50: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00015a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a70: 2020 2020 2020 2020 2020 646f 6375 7469            docuti
-00015a80: 6c73 2f77 7269 7465 7273 2f6c 6174 6578  ls/writers/latex
-00015a90: 3265 2f64 6f63 7574 696c 732e 7374 792c  2e/docutils.sty,
-00015aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a70: 2020 7465 7374 2f74 6573 745f 7061 7273    test/test_pars
+00015a80: 6572 732f 7465 7374 5f72 7374 2f74 6573  ers/test_rst/tes
+00015a90: 745f 6c69 6e65 5f6c 656e 6774 685f 6c69  t_line_length_li
+00015aa0: 6d69 742e 7079 2c20 2020 2020 2020 2020  mit.py,         
 00015ab0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00015ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015ad0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00015ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015af0: 646f 6375 7469 6c73 2f77 7269 7465 7273  docutils/writers
-00015b00: 2f78 6574 6578 2f5f 5f69 6e69 745f 5f2e  /xetex/__init__.
-00015b10: 7079 2c20 2020 2020 2020 2020 2020 2020  py,             
+00015ae0: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00015af0: 7374 2f74 6573 745f 7772 6974 6572 732f  st/test_writers/
+00015b00: 7465 7374 5f6c 6174 6578 3265 5f6d 6973  test_latex2e_mis
+00015b10: 632e 7079 2c20 2020 2020 2020 2020 2020  c.py,           
 00015b20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00015b30: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00015b40: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 00015b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015b60: 2020 7465 7374 2f74 6573 745f 7061 7273    test/test_pars
-00015b70: 6572 732f 7465 7374 5f72 6563 6f6d 6d6f  ers/test_recommo
-00015b80: 6e6d 6172 6b2f 5c2a 2e70 792c 2020 2020  nmark/\*.py,    
+00015b60: 2020 2020 2074 6573 742f 7472 616e 7366       test/transf
+00015b70: 6f72 6d73 2f74 6573 745f 736d 6172 7471  orms/test_smartq
+00015b80: 756f 7465 732e 7079 2c20 2020 2020 2020  uotes.py,       
 00015b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015ba0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00015bb0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00015bc0: 2020 2020 2020 2020 2020 2020 2020 7465                te
-00015bd0: 7374 2f74 6573 745f 7061 7273 6572 732f  st/test_parsers/
-00015be0: 7465 7374 5f72 7374 2f74 6573 745f 6469  test_rst/test_di
-00015bf0: 7265 6374 6976 6573 2f74 6573 745f 5f69  rectives/test__i
-00015c00: 6e69 745f 5f2e 7079 2c20 2020 2020 2020  nit__.py,       
+00015bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015be0: 2074 6f6f 6c73 2f64 6f63 7574 696c 732d   tools/docutils-
+00015bf0: 636c 692e 7079 2c20 2020 2020 2020 2020  cli.py,         
+00015c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015c10: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00015c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015c30: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00015c40: 2074 6573 742f 7465 7374 5f70 6172 7365   test/test_parse
-00015c50: 7273 2f74 6573 745f 7273 742f 7465 7374  rs/test_rst/test
-00015c60: 5f64 6972 6563 7469 7665 732f 7465 7374  _directives/test
-00015c70: 5f63 6f64 655f 7061 7273 696e 672e 7079  _code_parsing.py
-00015c80: 2c20 2020 2020 2020 2020 2020 2020 7c0a  ,             |.
+00015c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c50: 2020 2020 2020 2020 746f 6f6c 732f 7273          tools/rs
+00015c60: 7432 6874 6d6c 352e 7079 2020 2020 2020  t2html5.py      
+00015c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c80: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00015c90: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00015ca0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00015cb0: 2020 2020 2020 2074 6573 742f 7465 7374         test/test
-00015cc0: 5f70 6172 7365 7273 2f74 6573 745f 7273  _parsers/test_rs
-00015cd0: 742f 7465 7374 5f6c 696e 655f 6c65 6e67  t/test_line_leng
-00015ce0: 7468 5f6c 696d 6974 5f64 6566 6175 6c74  th_limit_default
-00015cf0: 2e70 792c 2020 2020 2020 2020 2020 2020  .py,            
+00015cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015d00: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00015d10: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 00015d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d30: 7465 7374 2f74 6573 745f 7061 7273 6572  test/test_parser
-00015d40: 732f 7465 7374 5f72 7374 2f74 6573 745f  s/test_rst/test_
-00015d50: 6c69 6e65 5f6c 656e 6774 685f 6c69 6d69  line_length_limi
-00015d60: 742e 7079 2c20 2020 2020 2020 2020 2020  t.py,           
-00015d70: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00015d80: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00015d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015da0: 2020 2020 2020 2020 2020 2020 7465 7374              test
-00015db0: 2f74 6573 745f 7772 6974 6572 732f 7465  /test_writers/te
-00015dc0: 7374 5f6c 6174 6578 3265 5f6d 6973 632e  st_latex2e_misc.
-00015dd0: 7079 2c20 2020 2020 2020 2020 2020 2020  py,             
-00015de0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00015df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e00: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00015d30: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+00015d40: 7079 7269 6768 7420 c2a9 2047 c3bc 6e74  pyright .. G..nt
+00015d50: 6572 204d 696c 6465 2e20 2020 2020 2020  er Milde.       
+00015d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d70: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00015d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015d90: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00015da0: 2020 2020 2020 5265 6c65 6173 6564 2075        Released u
+00015db0: 6e64 6572 2074 6865 2074 6572 6d73 206f  nder the terms o
+00015dc0: 6620 7468 6520 6042 5344 2032 2d43 6c61  f the `BSD 2-Cla
+00015dd0: 7573 6520 4c69 6365 6e73 6560 5f20 2020  use License`_   
+00015de0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00015df0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00015e00: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 00015e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e20: 2020 2074 6573 742f 7472 616e 7366 6f72     test/transfor
-00015e30: 6d73 2f74 6573 745f 736d 6172 7471 756f  ms/test_smartquo
-00015e40: 7465 732e 7079 2c20 2020 2020 2020 2020  tes.py,         
+00015e20: 2860 6c6f 6361 6c20 636f 7079 203c 6c69  (`local copy <li
+00015e30: 6365 6e73 6573 2f42 5344 2d32 2d43 6c61  censes/BSD-2-Cla
+00015e40: 7573 652e 7478 743e 605f 5f29 2e20 2020  use.txt>`__).   
 00015e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e60: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00015e70: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00015e60: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+00015e70: 2020 2020 2020 2020 2020 207c 2020 2020             |    
 00015e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015e90: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00015ea0: 6f6f 6c73 2f64 6f63 7574 696c 732d 636c  ools/docutils-cl
-00015eb0: 692e 7079 2c20 2020 2020 2020 2020 2020  i.py,           
+00015e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ed0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00015ee0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00015ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ed0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+00015ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ef0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00015f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f10: 2020 2020 2020 746f 6f6c 732f 7273 7432        tools/rst2
-00015f20: 6874 6d6c 352e 7079 2020 2020 2020 2020  html5.py        
+00015f10: 2020 202a 2064 6f63 7574 696c 732f 7574     * docutils/ut
+00015f20: 696c 732f 726f 6d61 6e2e 7079 2020 2020  ils/roman.py    
 00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f40: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00015f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f60: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+00015f40: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00015f50: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00015f60: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 00015f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00015fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015fc0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00015fd0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00015fc0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+00015fd0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 00015fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ff0: 2020 2020 2020 2020 2020 2020 436f 7079              Copy
-00016000: 7269 6768 7420 c2a9 2047 c3bc 6e74 6572  right .. G..nter
-00016010: 204d 696c 6465 2e20 2020 2020 2020 2020   Milde.         
-00016020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015ff0: 2020 2020 636f 7079 7269 6768 7420 6279      copyright by
+00016000: 204d 6172 6b20 5069 6c67 7269 6d2c 2072   Mark Pilgrim, r
+00016010: 656c 6561 7365 6420 756e 6465 7220 7468  eleased under th
+00016020: 6520 2020 2020 2020 2020 2020 2020 2020  e               
 00016030: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00016040: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00016050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016060: 2020 2020 5265 6c65 6173 6564 2075 6e64      Released und
-00016070: 6572 2074 6865 2074 6572 6d73 206f 6620  er the terms of 
-00016080: 7468 6520 6042 5344 2032 2d43 6c61 7573  the `BSD 2-Claus
-00016090: 6520 4c69 6365 6e73 6560 5f20 2020 2020  e License`_     
+00016060: 2020 2020 2020 2020 2020 2060 5079 7468             `Pyth
+00016070: 6f6e 2032 2e31 2e31 206c 6963 656e 7365  on 2.1.1 license
+00016080: 605f 2028 606c 6f63 616c 2063 6f70 7960  `_ (`local copy`
+00016090: 5f5f 292e 2020 2020 2020 2020 2020 2020  __).            
 000160a0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 000160b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000160c0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-000160d0: 2020 2020 2020 2020 2020 2020 2020 2860                (`
-000160e0: 6c6f 6361 6c20 636f 7079 203c 6c69 6365  local copy <lice
-000160f0: 6e73 6573 2f42 5344 2d32 2d43 6c61 7573  nses/BSD-2-Claus
-00016100: 652e 7478 743e 605f 5f29 2e20 2020 2020  e.txt>`__).     
+000160d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000160f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016120: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00016130: 2020 2020 2020 2020 207c 2020 2020 2020           |      
 00016140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016150: 2020 2020 2020 2020 2020 2020 5f5f 206c              __ l
+00016160: 6963 656e 7365 732f 7079 7468 6f6e 2d32  icenses/python-2
+00016170: 2d31 2d31 2e74 7874 2020 2020 2020 2020  -1-1.txt        
 00016180: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016190: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 000161a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 000161b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000161c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161d0: 202a 2064 6f63 7574 696c 732f 7574 696c   * docutils/util
-000161e0: 732f 726f 6d61 6e2e 7079 2020 2020 2020  s/roman.py      
+000161d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000161e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000161f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016200: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00016210: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016220: 2020 207c 2020 2020 2020 2020 2020 2020     |            
 00016230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016240: 2020 2020 202a 2074 6f6f 6c73 2f65 6469       * tools/edi
+00016250: 746f 7273 2f65 6d61 6373 2f72 7374 2e65  tors/emacs/rst.e
+00016260: 6c20 2020 2020 2020 2020 2020 2020 2020  l               
 00016270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016280: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00016290: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
 000162a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000162b0: 2020 636f 7079 7269 6768 7420 6279 204d    copyright by M
-000162c0: 6172 6b20 5069 6c67 7269 6d2c 2072 656c  ark Pilgrim, rel
-000162d0: 6561 7365 6420 756e 6465 7220 7468 6520  eased under the 
+000162b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000162d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000162e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000162f0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00016300: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 00016310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016320: 2020 2020 2020 2020 2060 5079 7468 6f6e           `Python
-00016330: 2032 2e31 2e31 206c 6963 656e 7365 605f   2.1.1 license`_
-00016340: 2028 606c 6f63 616c 2063 6f70 7960 5f5f   (`local copy`__
-00016350: 292e 2020 2020 2020 2020 2020 2020 2020  ).              
+00016320: 2020 2020 2020 2020 636f 7079 7269 6768          copyrigh
+00016330: 7420 6279 2046 7265 6520 536f 6674 7761  t by Free Softwa
+00016340: 7265 2046 6f75 6e64 6174 696f 6e2c 2049  re Foundation, I
+00016350: 6e63 2e2c 2020 2020 2020 2020 2020 2020  nc.,            
 00016360: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00016370: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016380: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00016390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000163d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016390: 2072 656c 6561 7365 6420 756e 6465 7220   released under 
+000163a0: 7468 6520 6047 4e55 2047 656e 6572 616c  the `GNU General
+000163b0: 2050 7562 6c69 6320 4c69 6365 6e73 6560   Public License`
+000163c0: 5f20 7665 7273 696f 6e20 3320 6f72 206c  _ version 3 or l
+000163d0: 6174 6572 2020 2020 2020 2020 2020 2020  ater            
 000163e0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 000163f0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 00016400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016410: 2020 2020 2020 2020 2020 5f5f 206c 6963            __ lic
-00016420: 656e 7365 732f 7079 7468 6f6e 2d32 2d31  enses/python-2-1
-00016430: 2d31 2e74 7874 2020 2020 2020 2020 2020  -1.txt          
+00016410: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00016420: 606c 6f63 616c 2063 6f70 7960 5f5f 292e  `local copy`__).
+00016430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016440: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016450: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00016460: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00016470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016480: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000164a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000164b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000164c0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 000164d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000164e0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
 000164f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016500: 2020 202a 2074 6f6f 6c73 2f65 6469 746f     * tools/edito
-00016510: 7273 2f65 6d61 6373 2f72 7374 2e65 6c20  rs/emacs/rst.el 
+00016500: 2020 2020 2020 5f5f 206c 6963 656e 7365        __ license
+00016510: 732f 6770 6c2d 332d 302e 7478 7420 2020  s/gpl-3-0.txt   
 00016520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016530: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00016540: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00016550: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 00016560: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016570: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016580: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016590: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000165a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000165b0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 000165c0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000165d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165e0: 2020 2020 2020 636f 7079 7269 6768 7420        copyright 
-000165f0: 6279 2046 7265 6520 536f 6674 7761 7265  by Free Software
-00016600: 2046 6f75 6e64 6174 696f 6e2c 2049 6e63   Foundation, Inc
-00016610: 2e2c 2020 2020 2020 2020 2020 2020 2020  .,              
+000165d0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+000165e0: 6c6c 2075 7365 6420 6c69 6365 6e73 6573  ll used licenses
+000165f0: 2061 7265 204f 5349 2d61 7070 726f 7665   are OSI-approve
+00016600: 645f 2061 6e64 2047 504c 2d63 6f6d 7061  d_ and GPL-compa
+00016610: 7469 626c 655f 2e20 2020 2020 2020 2020  tible_.         
 00016620: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00016630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016640: 7c20 2020 2020 2020 2020 2020 2020 2072  |              r
-00016650: 656c 6561 7365 6420 756e 6465 7220 7468  eleased under th
-00016660: 6520 6047 4e55 2047 656e 6572 616c 2050  e `GNU General P
-00016670: 7562 6c69 6320 4c69 6365 6e73 6560 5f20  ublic License`_ 
-00016680: 7665 7273 696f 6e20 3320 6f72 206c 6174  version 3 or lat
-00016690: 6572 2020 2020 2020 2020 2020 2020 7c0a  er            |.
+00016640: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00016650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016690: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 000166a0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 000166b0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000166c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000166d0: 2020 2020 2020 2020 2020 2020 2028 606c               (`l
-000166e0: 6f63 616c 2063 6f70 7960 5f5f 292e 2020  ocal copy`__).  
-000166f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000166c0: 2020 2050 6c61 696e 7465 7874 2076 6572     Plaintext ver
+000166d0: 7369 6f6e 7320 6f66 2061 6c6c 2074 6865  sions of all the
+000166e0: 206c 696e 6b65 642d 746f 206c 6963 656e   linked-to licen
+000166f0: 7365 7320 6172 6520 7072 6f76 6964 6564  ses are provided
+00016700: 2069 6e20 7468 6520 2020 2020 2020 2020   in the         
 00016710: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00016720: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 00016730: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016750: 6c69 6365 6e73 6573 5f20 6469 7265 6374  licenses_ direct
+00016760: 6f72 792e 2020 2020 2020 2020 2020 2020  ory.            
 00016770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016780: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00016790: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 000167a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000167b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167c0: 2020 2020 5f5f 206c 6963 656e 7365 732f      __ licenses/
-000167d0: 6770 6c2d 332d 302e 7478 7420 2020 2020  gpl-3-0.txt     
+000167c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000167d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000167e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000167f0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00016800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016810: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00016820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016820: 2020 2020 2e2e 205f 7361 6e64 626f 783a      .. _sandbox:
+00016830: 2068 7474 703a 2f2f 646f 6375 7469 6c73   http://docutils
+00016840: 2e73 6f75 7263 6566 6f72 6765 2e6e 6574  .sourceforge.net
+00016850: 2f73 616e 6462 6f78 2f52 4541 444d 452e  /sandbox/README.
+00016860: 6874 6d6c 2020 2020 2020 2020 2020 2020  html            
 00016870: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00016880: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00016890: 2020 2020 2020 2020 2020 2020 2041 6c6c               All
-000168a0: 2075 7365 6420 6c69 6365 6e73 6573 2061   used licenses a
-000168b0: 7265 204f 5349 2d61 7070 726f 7665 645f  re OSI-approved_
-000168c0: 2061 6e64 2047 504c 2d63 6f6d 7061 7469   and GPL-compati
-000168d0: 626c 655f 2e20 2020 2020 2020 2020 2020  ble_.           
+00016890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168a0: 2020 2020 2020 2020 2020 2020 202e 2e20               .. 
+000168b0: 5f6c 6963 656e 7365 733a 206c 6963 656e  _licenses: licen
+000168c0: 7365 732f 2020 2020 2020 2020 2020 2020  ses/            
+000168d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000168e0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 000168f0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00016900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016900: 2020 2020 2020 2020 2020 2020 202e 2e20               .. 
+00016910: 5f50 7974 686f 6e20 322e 312e 3120 6c69  _Python 2.1.1 li
+00016920: 6365 6e73 653a 2068 7474 703a 2f2f 7777  cense: http://ww
+00016930: 772e 7079 7468 6f6e 2e6f 7267 2f32 2e31  w.python.org/2.1
+00016940: 2e31 2f6c 6963 656e 7365 2e68 746d 6c20  .1/license.html 
 00016950: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00016960: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016970: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00016980: 2050 6c61 696e 7465 7874 2076 6572 7369   Plaintext versi
-00016990: 6f6e 7320 6f66 2061 6c6c 2074 6865 206c  ons of all the l
-000169a0: 696e 6b65 642d 746f 206c 6963 656e 7365  inked-to license
-000169b0: 7320 6172 6520 7072 6f76 6964 6564 2069  s are provided i
-000169c0: 6e20 7468 6520 2020 2020 2020 2020 2020  n the           
+00016980: 202e 2e20 5f47 4e55 2047 656e 6572 616c   .. _GNU General
+00016990: 2050 7562 6c69 6320 4c69 6365 6e73 653a   Public License:
+000169a0: 2068 7474 703a 2f2f 7777 772e 676e 752e   http://www.gnu.
+000169b0: 6f72 672f 636f 7079 6c65 6674 2f67 706c  org/copyleft/gpl
+000169c0: 2e68 746d 6c20 2020 2020 2020 2020 2020  .html           
 000169d0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 000169e0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000169f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a00: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-00016a10: 6365 6e73 6573 5f20 6469 7265 6374 6f72  censes_ director
-00016a20: 792e 2020 2020 2020 2020 2020 2020 2020  y.              
-00016a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000169f0: 2020 2020 202e 2e20 5f42 5344 2032 2d43       .. _BSD 2-C
+00016a00: 6c61 7573 6520 4c69 6365 6e73 653a 2068  lause License: h
+00016a10: 7474 703a 2f2f 6f70 656e 736f 7572 6365  ttp://opensource
+00016a20: 2e6f 7267 2f6c 6963 656e 7365 732f 4253  .org/licenses/BS
+00016a30: 442d 322d 436c 6175 7365 2020 2020 2020  D-2-Clause      
 00016a40: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00016a50: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00016a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a60: 2020 2020 2020 2020 2020 2e2e 205f 4253            .. _BS
+00016a70: 4420 332d 436c 6175 7365 204c 6963 656e  D 3-Clause Licen
+00016a80: 7365 3a20 6874 7470 733a 2f2f 6f70 656e  se: https://open
+00016a90: 736f 7572 6365 2e6f 7267 2f6c 6963 656e  source.org/licen
+00016aa0: 7365 732f 4253 442d 332d 436c 6175 7365  ses/BSD-3-Clause
 00016ab0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00016ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016ad0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00016ae0: 2020 2e2e 205f 7361 6e64 626f 783a 2068    .. _sandbox: h
-00016af0: 7474 7073 3a2f 2f64 6f63 7574 696c 732e  ttps://docutils.
-00016b00: 736f 7572 6365 666f 7267 652e 696f 2f73  sourceforge.io/s
-00016b10: 616e 6462 6f78 2f52 4541 444d 452e 6874  andbox/README.ht
-00016b20: 6d6c 2020 2020 2020 2020 2020 2020 2020  ml              
+00016ae0: 2020 2020 2020 2020 202e 2e20 5f4f 5349           .. _OSI
+00016af0: 2d61 7070 726f 7665 643a 2068 7474 703a  -approved: http:
+00016b00: 2f2f 6f70 656e 736f 7572 6365 2e6f 7267  //opensource.org
+00016b10: 2f6c 6963 656e 7365 732f 2020 2020 2020  /licenses/      
+00016b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016b30: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00016b40: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 00016b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b60: 2020 2020 2020 2020 2020 202e 2e20 5f6c             .. _l
-00016b70: 6963 656e 7365 733a 206c 6963 656e 7365  icenses: license
-00016b80: 732f 2020 2020 2020 2020 2020 2020 2020  s/              
+00016b60: 2020 2020 2020 2020 2020 2020 2020 2e2e                ..
+00016b70: 205f 6c69 6365 6e73 652d 6c69 7374 3a20   _license-list: 
+00016b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016ba0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00016bb0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00016bc0: 2020 2020 2020 2020 2020 2020 2e2e 205f              .. _
-00016bd0: 5079 7468 6f6e 2032 2e31 2e31 206c 6963  Python 2.1.1 lic
-00016be0: 656e 7365 3a20 6874 7470 733a 2f2f 646f  ense: https://do
-00016bf0: 6373 2e70 7974 686f 6e2e 6f72 672f 332f  cs.python.org/3/
-00016c00: 6c69 6365 6e73 652e 6874 6d6c 2020 2020  license.html    
+00016bc0: 2020 2020 2020 2020 2020 202e 2e20 5f47             .. _G
+00016bd0: 504c 2d63 6f6d 7061 7469 626c 653a 2068  PL-compatible: h
+00016be0: 7474 703a 2f2f 7777 772e 676e 752e 6f72  ttp://www.gnu.or
+00016bf0: 672f 6c69 6365 6e73 6573 2f6c 6963 656e  g/licenses/licen
+00016c00: 7365 2d6c 6973 742e 6874 6d6c 2020 2020  se-list.html    
 00016c10: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00016c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c30: 207c 2020 2020 2020 2020 2020 2020 2e2e   |            ..
-00016c40: 205f 474e 5520 4765 6e65 7261 6c20 5075   _GNU General Pu
-00016c50: 626c 6963 204c 6963 656e 7365 3a20 6874  blic License: ht
-00016c60: 7470 733a 2f2f 7777 772e 676e 752e 6f72  tps://www.gnu.or
-00016c70: 672f 636f 7079 6c65 6674 2f67 706c 2e68  g/copyleft/gpl.h
-00016c80: 746d 6c20 2020 2020 2020 2020 2020 207c  tml            |
-00016c90: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00016ca0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00016cb0: 2020 202e 2e20 5f42 5344 2032 2d43 6c61     .. _BSD 2-Cla
-00016cc0: 7573 6520 4c69 6365 6e73 653a 2068 7474  use License: htt
-00016cd0: 703a 2f2f 6f70 656e 736f 7572 6365 2e6f  p://opensource.o
-00016ce0: 7267 2f6c 6963 656e 7365 732f 4253 442d  rg/licenses/BSD-
-00016cf0: 322d 436c 6175 7365 2020 2020 2020 2020  2-Clause        
-00016d00: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00016d10: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00016d20: 2020 2020 2020 2020 2e2e 205f 4253 4420          .. _BSD 
-00016d30: 332d 436c 6175 7365 204c 6963 656e 7365  3-Clause License
-00016d40: 3a20 6874 7470 733a 2f2f 6f70 656e 736f  : https://openso
-00016d50: 7572 6365 2e6f 7267 2f6c 6963 656e 7365  urce.org/license
-00016d60: 732f 4253 442d 332d 436c 6175 7365 2020  s/BSD-3-Clause  
+00016c30: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00016c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016c80: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00016c90: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+00016ca0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00016cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00016d00: 2d2d 2d2d 2b0a 7c20 2020 2020 2020 2069  ----+.|        i
+00016d10: 646e 6120 2020 2020 2020 207c 2020 2020  dna        |    
+00016d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016d40: 2042 5344 2033 2d43 6c61 7573 6520 4c69   BSD 3-Clause Li
+00016d50: 6365 6e73 6520 2020 2020 2020 2020 2020  cense           
+00016d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016d70: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00016d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016d90: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00016da0: 2020 2020 2020 202e 2e20 5f4f 5349 2d61         .. _OSI-a
-00016db0: 7070 726f 7665 643a 2068 7474 703a 2f2f  pproved: http://
-00016dc0: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
-00016dd0: 6963 656e 7365 732f 2020 2020 2020 2020  icenses/        
+00016da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016de0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00016df0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00016e00: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00016e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e20: 2020 2020 2020 2020 2020 2020 2e2e 205f              .. _
-00016e30: 6c69 6365 6e73 652d 6c69 7374 3a20 2020  license-list:   
-00016e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e10: 2020 2020 2020 2020 2020 436f 7079 7269            Copyri
+00016e20: 6768 7420 2863 2920 3230 3133 2d32 3032  ght (c) 2013-202
+00016e30: 332c 204b 696d 2044 6176 6965 7320 616e  3, Kim Davies an
+00016e40: 6420 636f 6e74 7269 6275 746f 7273 2e20  d contributors. 
 00016e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016e60: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00016e70: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00016e80: 2020 2020 2020 2020 202e 2e20 5f47 504c           .. _GPL
-00016e90: 2d63 6f6d 7061 7469 626c 653a 2068 7474  -compatible: htt
-00016ea0: 7073 3a2f 2f77 7777 2e67 6e75 2e6f 7267  ps://www.gnu.org
-00016eb0: 2f6c 6963 656e 7365 732f 6c69 6365 6e73  /licenses/licens
-00016ec0: 652d 6c69 7374 2e68 746d 6c20 2020 2020  e-list.html     
+00016e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ea0: 416c 6c20 7269 6768 7473 2072 6573 6572  All rights reser
+00016eb0: 7665 642e 2020 2020 2020 2020 2020 2020  ved.            
+00016ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016ed0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00016ee0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00016ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00016f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016f40: 2020 2020 2020 2020 2020 2020 207c 0a2b               |.+
-00016f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016f60: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00016f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00016fc0: 2d2d 2b0a 7c20 2020 2020 2020 2069 646e  --+.|        idn
-00016fd0: 6120 2020 2020 2020 207c 2020 2020 2020  a        |      
-00016fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016ff0: 2020 2020 2020 2020 2020 2020 2020 2042                 B
-00017000: 5344 2033 2d43 6c61 7573 6520 4c69 6365  SD 3-Clause Lice
-00017010: 6e73 6520 2020 2020 2020 2020 2020 2020  nse             
-00017020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f40: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00016f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f60: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00016f70: 2020 2052 6564 6973 7472 6962 7574 696f     Redistributio
+00016f80: 6e20 616e 6420 7573 6520 696e 2073 6f75  n and use in sou
+00016f90: 7263 6520 616e 6420 6269 6e61 7279 2066  rce and binary f
+00016fa0: 6f72 6d73 2c20 7769 7468 206f 7220 7769  orms, with or wi
+00016fb0: 7468 6f75 7420 2020 2020 2020 2020 2020  thout           
+00016fc0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+00016fd0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00016fe0: 2020 2020 2020 6d6f 6469 6669 6361 7469        modificati
+00016ff0: 6f6e 2c20 6172 6520 7065 726d 6974 7465  on, are permitte
+00017000: 6420 7072 6f76 6964 6564 2074 6861 7420  d provided that 
+00017010: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
+00017020: 6e64 6974 696f 6e73 2061 7265 2020 2020  nditions are    
 00017030: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00017040: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 00017050: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017070: 2020 2020 2020 2020 2020 2020 6d65 743a              met:
 00017080: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000170a0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 000170b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000170c0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
 000170d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170e0: 2043 6f70 7972 6967 6874 2028 6329 2032   Copyright (c) 2
-000170f0: 3031 332d 3230 3231 2c20 4b69 6d20 4461  013-2021, Kim Da
-00017100: 7669 6573 2020 2020 2020 2020 2020 2020  vies            
+000170e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000170f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017120: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00017130: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00017140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017150: 2020 2020 2020 2020 2020 2020 2020 416c                Al
-00017160: 6c20 7269 6768 7473 2072 6573 6572 7665  l rights reserve
-00017170: 642e 2020 2020 2020 2020 2020 2020 2020  d.              
-00017180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017140: 2020 2020 2020 2031 2e20 5265 6469 7374         1. Redist
+00017150: 7269 6275 7469 6f6e 7320 6f66 2073 6f75  ributions of sou
+00017160: 7263 6520 636f 6465 206d 7573 7420 7265  rce code must re
+00017170: 7461 696e 2074 6865 2061 626f 7665 2063  tain the above c
+00017180: 6f70 7972 6967 6874 2020 2020 2020 2020  opyright        
 00017190: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 000171a0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 000171b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000171f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171c0: 6e6f 7469 6365 2c20 7468 6973 206c 6973  notice, this lis
+000171d0: 7420 6f66 2063 6f6e 6469 7469 6f6e 7320  t of conditions 
+000171e0: 616e 6420 7468 6520 666f 6c6c 6f77 696e  and the followin
+000171f0: 6720 6469 7363 6c61 696d 6572 2e20 2020  g disclaimer.   
 00017200: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00017210: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017220: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00017230: 2052 6564 6973 7472 6962 7574 696f 6e20   Redistribution 
-00017240: 616e 6420 7573 6520 696e 2073 6f75 7263  and use in sourc
-00017250: 6520 616e 6420 6269 6e61 7279 2066 6f72  e and binary for
-00017260: 6d73 2c20 7769 7468 206f 7220 7769 7468  ms, with or with
-00017270: 6f75 7420 2020 2020 2020 2020 2020 2020  out             
+00017230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017280: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00017290: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-000172a0: 206d 6f64 6966 6963 6174 696f 6e2c 2061   modification, a
-000172b0: 7265 2070 6572 6d69 7474 6564 2070 726f  re permitted pro
-000172c0: 7669 6465 6420 7468 6174 2074 6865 2066  vided that the f
-000172d0: 6f6c 6c6f 7769 6e67 2063 6f6e 6469 7469  ollowing conditi
-000172e0: 6f6e 7320 6172 6520 6d65 743a 2020 2020  ons are met:    
+000172a0: 2020 2020 2032 2e20 5265 6469 7374 7269       2. Redistri
+000172b0: 6275 7469 6f6e 7320 696e 2062 696e 6172  butions in binar
+000172c0: 7920 666f 726d 206d 7573 7420 7265 7072  y form must repr
+000172d0: 6f64 7563 6520 7468 6520 6162 6f76 6520  oduce the above 
+000172e0: 636f 7079 7269 6768 7420 2020 2020 2020  copyright       
 000172f0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00017300: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00017310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017310: 2020 2020 2020 2020 2020 2020 6e6f 7469              noti
+00017320: 6365 2c20 7468 6973 206c 6973 7420 6f66  ce, this list of
+00017330: 2063 6f6e 6469 7469 6f6e 7320 616e 6420   conditions and 
+00017340: 7468 6520 666f 6c6c 6f77 696e 6720 6469  the following di
+00017350: 7363 6c61 696d 6572 2069 6e20 7468 6520  sclaimer in the 
 00017360: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00017370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017380: 207c 2020 2020 2020 2020 312e 2052 6564   |        1. Red
-00017390: 6973 7472 6962 7574 696f 6e73 206f 6620  istributions of 
-000173a0: 736f 7572 6365 2063 6f64 6520 6d75 7374  source code must
-000173b0: 2072 6574 6169 6e20 7468 6520 6162 6f76   retain the abov
-000173c0: 6520 636f 7079 7269 6768 7420 6e6f 7469  e copyright noti
-000173d0: 6365 2c20 7468 6973 2020 2020 2020 207c  ce, this       |
+00017380: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00017390: 646f 6375 6d65 6e74 6174 696f 6e20 616e  documentation an
+000173a0: 642f 6f72 206f 7468 6572 206d 6174 6572  d/or other mater
+000173b0: 6961 6c73 2070 726f 7669 6465 6420 7769  ials provided wi
+000173c0: 7468 2074 6865 2064 6973 7472 6962 7574  th the distribut
+000173d0: 696f 6e2e 2020 2020 2020 2020 2020 207c  ion.           |
 000173e0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 000173f0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00017400: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00017410: 6973 7420 6f66 2063 6f6e 6469 7469 6f6e  ist of condition
-00017420: 7320 616e 6420 7468 6520 666f 6c6c 6f77  s and the follow
-00017430: 696e 6720 6469 7363 6c61 696d 6572 2e20  ing disclaimer. 
+00017400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017440: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017450: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00017460: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00017470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017470: 2020 2020 2020 2020 2020 2033 2e20 4e65             3. Ne
+00017480: 6974 6865 7220 7468 6520 6e61 6d65 206f  ither the name o
+00017490: 6620 7468 6520 636f 7079 7269 6768 7420  f the copyright 
+000174a0: 686f 6c64 6572 206e 6f72 2074 6865 206e  holder nor the n
+000174b0: 616d 6573 206f 6620 6974 7320 2020 2020  ames of its     
 000174c0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 000174d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174e0: 7c20 2020 2020 2020 2020 322e 2052 6564  |         2. Red
-000174f0: 6973 7472 6962 7574 696f 6e73 2069 6e20  istributions in 
-00017500: 6269 6e61 7279 2066 6f72 6d20 6d75 7374  binary form must
-00017510: 2072 6570 726f 6475 6365 2074 6865 2061   reproduce the a
-00017520: 626f 7665 2063 6f70 7972 6967 6874 206e  bove copyright n
-00017530: 6f74 6963 652c 2020 2020 2020 2020 7c0a  otice,        |.
+000174e0: 7c20 2020 2020 2020 2020 2020 2020 2063  |              c
+000174f0: 6f6e 7472 6962 7574 6f72 7320 6d61 7920  ontributors may 
+00017500: 6265 2075 7365 6420 746f 2065 6e64 6f72  be used to endor
+00017510: 7365 206f 7220 7072 6f6d 6f74 6520 7072  se or promote pr
+00017520: 6f64 7563 7473 2064 6572 6976 6564 2066  oducts derived f
+00017530: 726f 6d20 2020 2020 2020 2020 2020 7c0a  rom           |.
 00017540: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00017550: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00017560: 2020 7468 6973 206c 6973 7420 6f66 2063    this list of c
-00017570: 6f6e 6469 7469 6f6e 7320 616e 6420 7468  onditions and th
-00017580: 6520 666f 6c6c 6f77 696e 6720 6469 7363  e following disc
-00017590: 6c61 696d 6572 2069 6e20 7468 6520 646f  laimer in the do
-000175a0: 6375 6d65 6e74 6174 696f 6e20 2020 2020  cumentation     
+00017560: 2020 2020 2020 2020 2020 7468 6973 2073            this s
+00017570: 6f66 7477 6172 6520 7769 7468 6f75 7420  oftware without 
+00017580: 7370 6563 6966 6963 2070 7269 6f72 2077  specific prior w
+00017590: 7269 7474 656e 2070 6572 6d69 7373 696f  ritten permissio
+000175a0: 6e2e 2020 2020 2020 2020 2020 2020 2020  n.              
 000175b0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 000175c0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 000175d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175e0: 616e 642f 6f72 206f 7468 6572 206d 6174  and/or other mat
-000175f0: 6572 6961 6c73 2070 726f 7669 6465 6420  erials provided 
-00017600: 7769 7468 2074 6865 2064 6973 7472 6962  with the distrib
-00017610: 7574 696f 6e2e 2020 2020 2020 2020 2020  ution.          
+000175e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000175f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017610: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017620: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00017630: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00017640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017640: 2020 2020 2020 2020 2020 2020 2054 4849               THI
+00017650: 5320 534f 4654 5741 5245 2049 5320 5052  S SOFTWARE IS PR
+00017660: 4f56 4944 4544 2042 5920 5448 4520 434f  OVIDED BY THE CO
+00017670: 5059 5249 4748 5420 484f 4c44 4552 5320  PYRIGHT HOLDERS 
+00017680: 414e 4420 434f 4e54 5249 4255 544f 5253  AND CONTRIBUTORS
 00017690: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 000176a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000176b0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-000176c0: 2020 2020 332e 204e 6569 7468 6572 2074      3. Neither t
-000176d0: 6865 206e 616d 6520 6f66 2074 6865 2063  he name of the c
-000176e0: 6f70 7972 6967 6874 2068 6f6c 6465 7220  opyright holder 
-000176f0: 6e6f 7220 7468 6520 6e61 6d65 7320 6f66  nor the names of
-00017700: 2069 7473 2020 2020 2020 2020 2020 2020   its            
+000176c0: 2020 2022 4153 2049 5322 2041 4e44 2041     "AS IS" AND A
+000176d0: 4e59 2045 5850 5245 5353 204f 5220 494d  NY EXPRESS OR IM
+000176e0: 504c 4945 4420 5741 5252 414e 5449 4553  PLIED WARRANTIES
+000176f0: 2c20 494e 434c 5544 494e 472c 2042 5554  , INCLUDING, BUT
+00017700: 204e 4f54 2020 2020 2020 2020 2020 2020   NOT            
 00017710: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00017720: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00017730: 2020 2020 2020 2020 636f 6e74 7269 6275          contribu
-00017740: 746f 7273 206d 6179 2062 6520 7573 6564  tors may be used
-00017750: 2074 6f20 656e 646f 7273 6520 6f72 2070   to endorse or p
-00017760: 726f 6d6f 7465 2070 726f 6475 6374 7320  romote products 
-00017770: 6465 7269 7665 6420 6672 6f6d 2020 2020  derived from    
+00017730: 2020 2020 2020 4c49 4d49 5445 4420 544f        LIMITED TO
+00017740: 2c20 5448 4520 494d 504c 4945 4420 5741  , THE IMPLIED WA
+00017750: 5252 414e 5449 4553 204f 4620 4d45 5243  RRANTIES OF MERC
+00017760: 4841 4e54 4142 494c 4954 5920 414e 4420  HANTABILITY AND 
+00017770: 4649 544e 4553 5320 464f 5220 2020 2020  FITNESS FOR     
 00017780: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00017790: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000177a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177b0: 2020 2074 6869 7320 736f 6674 7761 7265     this software
-000177c0: 2077 6974 686f 7574 2073 7065 6369 6669   without specifi
-000177d0: 6320 7072 696f 7220 7772 6974 7465 6e20  c prior written 
-000177e0: 7065 726d 6973 7369 6f6e 2e20 2020 2020  permission.     
+000177a0: 2020 2020 2020 2020 2020 2020 4120 5041              A PA
+000177b0: 5254 4943 554c 4152 2050 5552 504f 5345  RTICULAR PURPOSE
+000177c0: 2041 5245 2044 4953 434c 4149 4d45 442e   ARE DISCLAIMED.
+000177d0: 2049 4e20 4e4f 2045 5645 4e54 2053 4841   IN NO EVENT SHA
+000177e0: 4c4c 2054 4845 2043 4f50 5952 4947 4854  LL THE COPYRIGHT
 000177f0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00017800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017810: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00017820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017820: 484f 4c44 4552 204f 5220 434f 4e54 5249  HOLDER OR CONTRI
+00017830: 4255 544f 5253 2042 4520 4c49 4142 4c45  BUTORS BE LIABLE
+00017840: 2046 4f52 2041 4e59 2044 4952 4543 542c   FOR ANY DIRECT,
+00017850: 2049 4e44 4952 4543 542c 2049 4e43 4944   INDIRECT, INCID
+00017860: 454e 5441 4c2c 2020 2020 2020 2020 2020  ENTAL,          
 00017870: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00017880: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00017890: 2020 5448 4953 2053 4f46 5457 4152 4520    THIS SOFTWARE 
-000178a0: 4953 2050 524f 5649 4445 4420 4259 2054  IS PROVIDED BY T
-000178b0: 4845 2043 4f50 5952 4947 4854 2048 4f4c  HE COPYRIGHT HOL
-000178c0: 4445 5253 2041 4e44 2043 4f4e 5452 4942  DERS AND CONTRIB
-000178d0: 5554 4f52 5320 2241 5320 4953 2220 2020  UTORS "AS IS"   
+00017890: 2020 2020 5350 4543 4941 4c2c 2045 5845      SPECIAL, EXE
+000178a0: 4d50 4c41 5259 2c20 4f52 2043 4f4e 5345  MPLARY, OR CONSE
+000178b0: 5155 454e 5449 414c 2044 414d 4147 4553  QUENTIAL DAMAGES
+000178c0: 2028 494e 434c 5544 494e 472c 2042 5554   (INCLUDING, BUT
+000178d0: 204e 4f54 204c 494d 4954 4544 2020 2020   NOT LIMITED    
 000178e0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 000178f0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00017900: 2020 2020 2020 2020 414e 4420 414e 5920          AND ANY 
-00017910: 4558 5052 4553 5320 4f52 2049 4d50 4c49  EXPRESS OR IMPLI
-00017920: 4544 2057 4152 5241 4e54 4945 532c 2049  ED WARRANTIES, I
-00017930: 4e43 4c55 4449 4e47 2c20 4255 5420 4e4f  NCLUDING, BUT NO
-00017940: 5420 4c49 4d49 5445 4420 544f 2c20 5448  T LIMITED TO, TH
-00017950: 4520 2020 2020 2020 2020 207c 0a7c 2020  E          |.|  
+00017900: 2020 2020 2020 2020 2020 544f 2c20 5052            TO, PR
+00017910: 4f43 5552 454d 454e 5420 4f46 2053 5542  OCUREMENT OF SUB
+00017920: 5354 4954 5554 4520 474f 4f44 5320 4f52  STITUTE GOODS OR
+00017930: 2053 4552 5649 4345 533b 204c 4f53 5320   SERVICES; LOSS 
+00017940: 4f46 2055 5345 2c20 4441 5441 2c20 4f52  OF USE, DATA, OR
+00017950: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00017960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017970: 2020 7c20 2020 2020 2020 2049 4d50 4c49    |        IMPLI
-00017980: 4544 2057 4152 5241 4e54 4945 5320 4f46  ED WARRANTIES OF
-00017990: 204d 4552 4348 414e 5441 4249 4c49 5459   MERCHANTABILITY
-000179a0: 2041 4e44 2046 4954 4e45 5353 2046 4f52   AND FITNESS FOR
-000179b0: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
-000179c0: 5250 4f53 4520 4152 4520 2020 2020 2020  RPOSE ARE       
+00017970: 2020 7c20 2020 2020 2020 2020 2020 2050    |            P
+00017980: 524f 4649 5453 3b20 4f52 2042 5553 494e  ROFITS; OR BUSIN
+00017990: 4553 5320 494e 5445 5252 5550 5449 4f4e  ESS INTERRUPTION
+000179a0: 2920 484f 5745 5645 5220 4341 5553 4544  ) HOWEVER CAUSED
+000179b0: 2041 4e44 204f 4e20 414e 5920 5448 454f   AND ON ANY THEO
+000179c0: 5259 204f 4620 2020 2020 2020 2020 2020  RY OF           
 000179d0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 000179e0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-000179f0: 2044 4953 434c 4149 4d45 442e 2049 4e20   DISCLAIMED. IN 
-00017a00: 4e4f 2045 5645 4e54 2053 4841 4c4c 2054  NO EVENT SHALL T
-00017a10: 4845 2043 4f50 5952 4947 4854 2048 4f4c  HE COPYRIGHT HOL
-00017a20: 4445 5220 4f52 2043 4f4e 5452 4942 5554  DER OR CONTRIBUT
-00017a30: 4f52 5320 4245 204c 4941 424c 4520 2020  ORS BE LIABLE   
+000179f0: 2020 2020 204c 4941 4249 4c49 5459 2c20       LIABILITY, 
+00017a00: 5748 4554 4845 5220 494e 2043 4f4e 5452  WHETHER IN CONTR
+00017a10: 4143 542c 2053 5452 4943 5420 4c49 4142  ACT, STRICT LIAB
+00017a20: 494c 4954 592c 204f 5220 544f 5254 2028  ILITY, OR TORT (
+00017a30: 494e 434c 5544 494e 4720 2020 2020 2020  INCLUDING       
 00017a40: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00017a50: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00017a60: 2020 2020 2020 2046 4f52 2041 4e59 2044         FOR ANY D
-00017a70: 4952 4543 542c 2049 4e44 4952 4543 542c  IRECT, INDIRECT,
-00017a80: 2049 4e43 4944 454e 5441 4c2c 2053 5045   INCIDENTAL, SPE
-00017a90: 4349 414c 2c20 4558 454d 504c 4152 592c  CIAL, EXEMPLARY,
-00017aa0: 204f 5220 434f 4e53 4551 5545 4e54 4941   OR CONSEQUENTIA
-00017ab0: 4c20 2020 2020 2020 2020 7c0a 7c20 2020  L         |.|   
+00017a60: 2020 2020 2020 2020 2020 204e 4547 4c49             NEGLI
+00017a70: 4745 4e43 4520 4f52 204f 5448 4552 5749  GENCE OR OTHERWI
+00017a80: 5345 2920 4152 4953 494e 4720 494e 2041  SE) ARISING IN A
+00017a90: 4e59 2057 4159 204f 5554 204f 4620 5448  NY WAY OUT OF TH
+00017aa0: 4520 5553 4520 4f46 2054 4849 5320 2020  E USE OF THIS   
+00017ab0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ad0: 207c 2020 2020 2020 2020 2020 4441 4d41   |          DAMA
-00017ae0: 4745 5320 2849 4e43 4c55 4449 4e47 2c20  GES (INCLUDING, 
-00017af0: 4255 5420 4e4f 5420 4c49 4d49 5445 4420  BUT NOT LIMITED 
-00017b00: 544f 2c20 5052 4f43 5552 454d 454e 5420  TO, PROCUREMENT 
-00017b10: 4f46 2053 5542 5354 4954 5554 4520 474f  OF SUBSTITUTE GO
-00017b20: 4f44 5320 4f52 2020 2020 2020 2020 207c  ODS OR         |
+00017ad0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00017ae0: 2020 2053 4f46 5457 4152 452c 2045 5645     SOFTWARE, EVE
+00017af0: 4e20 4946 2041 4456 4953 4544 204f 4620  N IF ADVISED OF 
+00017b00: 5448 4520 504f 5353 4942 494c 4954 5920  THE POSSIBILITY 
+00017b10: 4f46 2053 5543 4820 4441 4d41 4745 2e20  OF SUCH DAMAGE. 
+00017b20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00017b30: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00017b40: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00017b50: 2053 4552 5649 4345 533b 204c 4f53 5320   SERVICES; LOSS 
-00017b60: 4f46 2055 5345 2c20 4441 5441 2c20 4f52  OF USE, DATA, OR
-00017b70: 2050 524f 4649 5453 3b20 4f52 2042 5553   PROFITS; OR BUS
-00017b80: 494e 4553 5320 494e 5445 5252 5550 5449  INESS INTERRUPTI
-00017b90: 4f4e 2920 484f 5745 5645 5220 2020 2020  ON) HOWEVER     
-00017ba0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00017bb0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00017bc0: 2020 2020 4341 5553 4544 2041 4e44 204f      CAUSED AND O
-00017bd0: 4e20 414e 5920 5448 454f 5259 204f 4620  N ANY THEORY OF 
-00017be0: 4c49 4142 494c 4954 592c 2057 4845 5448  LIABILITY, WHETH
-00017bf0: 4552 2049 4e20 434f 4e54 5241 4354 2c20  ER IN CONTRACT, 
-00017c00: 5354 5249 4354 204c 4941 4249 4c49 5459  STRICT LIABILITY
-00017c10: 2c20 2020 2020 2020 207c 0a7c 2020 2020  ,        |.|    
-00017c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c30: 7c20 2020 2020 2020 204f 5220 544f 5254  |        OR TORT
-00017c40: 2028 494e 434c 5544 494e 4720 4e45 474c   (INCLUDING NEGL
-00017c50: 4947 454e 4345 204f 5220 4f54 4845 5257  IGENCE OR OTHERW
-00017c60: 4953 4529 2041 5249 5349 4e47 2049 4e20  ISE) ARISING IN 
-00017c70: 414e 5920 5741 5920 4f55 5420 4f46 2054  ANY WAY OUT OF T
-00017c80: 4845 2055 5345 2020 2020 2020 2020 7c0a  HE USE        |.
+00017b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ba0: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
+00017bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00017bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00017bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00017be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00017bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00017c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00017c10: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020  ---------+.|    
+00017c20: 2020 6c6f 6766 7572 7920 2020 2020 2020    logfury       
+00017c30: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00017c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c50: 2020 2020 2020 4253 4420 332d 636c 6175        BSD 3-clau
+00017c60: 7365 206c 6963 656e 7365 2020 2020 2020  se license      
+00017c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c80: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00017c90: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00017ca0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00017cb0: 2020 204f 4620 5448 4953 2053 4f46 5457     OF THIS SOFTW
-00017cc0: 4152 452c 2045 5645 4e20 4946 2041 4456  ARE, EVEN IF ADV
-00017cd0: 4953 4544 204f 4620 5448 4520 504f 5353  ISED OF THE POSS
-00017ce0: 4942 494c 4954 5920 4f46 2053 5543 4820  IBILITY OF SUCH 
-00017cf0: 4441 4d41 4745 2e20 2020 2020 2020 2020  DAMAGE.         
+00017cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017d00: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00017d10: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 00017d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d30: 2020 2020 2020 2020 436f 7079 7269 6768          Copyrigh
+00017d40: 7420 2863 2920 3230 3136 2c20 5061 7765  t (c) 2016, Pawe
+00017d50: 6c20 506f 6c65 7769 637a 2e20 2020 2020  l Polewicz.     
 00017d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d70: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
-00017d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00017d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017db0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00017de0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
-00017df0: 2020 2020 2020 6c6f 6766 7572 7920 2020        logfury   
+00017d70: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+00017d80: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00017d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017db0: 2020 2020 2041 6c6c 2072 6967 6874 7320       All rights 
+00017dc0: 7265 7365 7276 6564 2e20 2020 2020 2020  reserved.       
+00017dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017de0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00017df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017e00: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
 00017e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e20: 2020 2020 2020 2020 2020 4253 4420 332d            BSD 3-
-00017e30: 636c 6175 7365 206c 6963 656e 7365 2020  clause license  
+00017e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017e60: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00017e70: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00017e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017e80: 2020 2020 2020 2020 5265 6469 7374 7269          Redistri
+00017e90: 6275 7469 6f6e 2061 6e64 2075 7365 2069  bution and use i
+00017ea0: 6e20 736f 7572 6365 2061 6e64 2062 696e  n source and bin
+00017eb0: 6172 7920 666f 726d 732c 2077 6974 6820  ary forms, with 
+00017ec0: 6f72 2077 6974 686f 7574 2020 2020 2020  or without      
 00017ed0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00017ee0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00017ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f00: 2020 2020 2020 2020 2020 2020 436f 7079              Copy
-00017f10: 7269 6768 7420 2863 2920 3230 3136 2c20  right (c) 2016, 
-00017f20: 5061 7765 6c20 506f 6c65 7769 637a 2e20  Pawel Polewicz. 
-00017f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f40: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00017ef0: 2020 2020 2020 2020 6d6f 6469 6669 6361          modifica
+00017f00: 7469 6f6e 2c20 6172 6520 7065 726d 6974  tion, are permit
+00017f10: 7465 6420 7072 6f76 6964 6564 2074 6861  ted provided tha
+00017f20: 7420 7468 6520 666f 6c6c 6f77 696e 6720  t the following 
+00017f30: 636f 6e64 6974 696f 6e73 2061 7265 206d  conditions are m
+00017f40: 6574 3a20 2020 2020 2020 2020 7c0a 7c20  et:         |.| 
 00017f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017f60: 2020 207c 2020 2020 2020 2020 2020 2020     |            
 00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017f80: 2020 2020 2020 2020 2041 6c6c 2072 6967           All rig
-00017f90: 6874 7320 7265 7365 7276 6564 2e20 2020  hts reserved.   
+00017f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00017fc0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00017fd0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00017fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fe0: 202a 2052 6564 6973 7472 6962 7574 696f   * Redistributio
+00017ff0: 6e73 206f 6620 736f 7572 6365 2063 6f64  ns of source cod
+00018000: 6520 6d75 7374 2072 6574 6169 6e20 7468  e must retain th
+00018010: 6520 6162 6f76 6520 636f 7079 7269 6768  e above copyrigh
+00018020: 7420 6e6f 7469 6365 2c20 7468 6973 2020  t notice, this  
 00018030: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00018040: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00018050: 2020 2020 2020 2020 2020 2020 5265 6469              Redi
-00018060: 7374 7269 6275 7469 6f6e 2061 6e64 2075  stribution and u
-00018070: 7365 2069 6e20 736f 7572 6365 2061 6e64  se in source and
-00018080: 2062 696e 6172 7920 666f 726d 732c 2077   binary forms, w
-00018090: 6974 6820 6f72 2077 6974 686f 7574 2020  ith or without  
+00018050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018060: 2020 2020 2020 6c69 7374 206f 6620 636f        list of co
+00018070: 6e64 6974 696f 6e73 2061 6e64 2074 6865  nditions and the
+00018080: 2066 6f6c 6c6f 7769 6e67 2064 6973 636c   following discl
+00018090: 6169 6d65 722e 2020 2020 2020 2020 2020  aimer.          
 000180a0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 000180b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000180c0: 2020 7c20 2020 2020 2020 2020 6d6f 6469    |         modi
-000180d0: 6669 6361 7469 6f6e 2c20 6172 6520 7065  fication, are pe
-000180e0: 726d 6974 7465 6420 7072 6f76 6964 6564  rmitted provided
-000180f0: 2074 6861 7420 7468 6520 666f 6c6c 6f77   that the follow
-00018100: 696e 6720 636f 6e64 6974 696f 6e73 2061  ing conditions a
-00018110: 7265 206d 6574 3a20 2020 2020 2020 2020  re met:         
+000180c0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+000180d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000180f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018110: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00018120: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00018130: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00018140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018140: 202a 2052 6564 6973 7472 6962 7574 696f   * Redistributio
+00018150: 6e73 2069 6e20 6269 6e61 7279 2066 6f72  ns in binary for
+00018160: 6d20 6d75 7374 2072 6570 726f 6475 6365  m must reproduce
+00018170: 2074 6865 2061 626f 7665 2063 6f70 7972   the above copyr
+00018180: 6967 6874 206e 6f74 6963 652c 2020 2020  ight notice,    
 00018190: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 000181a0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000181b0: 2020 2020 202a 2052 6564 6973 7472 6962       * Redistrib
-000181c0: 7574 696f 6e73 206f 6620 736f 7572 6365  utions of source
-000181d0: 2063 6f64 6520 6d75 7374 2072 6574 6169   code must retai
-000181e0: 6e20 7468 6520 6162 6f76 6520 636f 7079  n the above copy
-000181f0: 7269 6768 7420 6e6f 7469 6365 2c20 7468  right notice, th
-00018200: 6973 2020 2020 2020 2020 7c0a 7c20 2020  is        |.|   
+000181b0: 2020 2020 2020 2020 7468 6973 206c 6973          this lis
+000181c0: 7420 6f66 2063 6f6e 6469 7469 6f6e 7320  t of conditions 
+000181d0: 616e 6420 7468 6520 666f 6c6c 6f77 696e  and the followin
+000181e0: 6720 6469 7363 6c61 696d 6572 2069 6e20  g disclaimer in 
+000181f0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00018200: 6e20 2020 2020 2020 2020 7c0a 7c20 2020  n         |.|   
 00018210: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00018220: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00018230: 2020 2020 2020 2020 2020 6c69 7374 206f            list o
-00018240: 6620 636f 6e64 6974 696f 6e73 2061 6e64  f conditions and
-00018250: 2074 6865 2066 6f6c 6c6f 7769 6e67 2064   the following d
-00018260: 6973 636c 6169 6d65 722e 2020 2020 2020  isclaimer.      
+00018230: 2020 2020 2020 2061 6e64 2f6f 7220 6f74         and/or ot
+00018240: 6865 7220 6d61 7465 7269 616c 7320 7072  her materials pr
+00018250: 6f76 6964 6564 2077 6974 6820 7468 6520  ovided with the 
+00018260: 6469 7374 7269 6275 7469 6f6e 2e20 2020  distribution.   
 00018270: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00018280: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00018290: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 000182a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000182b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000182c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000182d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000182e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000182f0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00018300: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00018310: 2020 2020 202a 2052 6564 6973 7472 6962       * Redistrib
-00018320: 7574 696f 6e73 2069 6e20 6269 6e61 7279  utions in binary
-00018330: 2066 6f72 6d20 6d75 7374 2072 6570 726f   form must repro
-00018340: 6475 6365 2074 6865 2061 626f 7665 2063  duce the above c
-00018350: 6f70 7972 6967 6874 206e 6f74 6963 652c  opyright notice,
+00018310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018320: 2020 2a20 4e65 6974 6865 7220 7468 6520    * Neither the 
+00018330: 6e61 6d65 206f 6620 6c6f 6766 7572 7920  name of logfury 
+00018340: 6e6f 7220 7468 6520 6e61 6d65 7320 6f66  nor the names of
+00018350: 2069 7473 2020 2020 2020 2020 2020 2020   its            
 00018360: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00018370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018380: 7c20 2020 2020 2020 2020 2020 7468 6973  |           this
-00018390: 206c 6973 7420 6f66 2063 6f6e 6469 7469   list of conditi
-000183a0: 6f6e 7320 616e 6420 7468 6520 666f 6c6c  ons and the foll
-000183b0: 6f77 696e 6720 6469 7363 6c61 696d 6572  owing disclaimer
-000183c0: 2069 6e20 7468 6520 646f 6375 6d65 6e74   in the document
-000183d0: 6174 696f 6e20 2020 2020 2020 2020 7c0a  ation         |.
+00018380: 7c20 2020 2020 2020 2020 2020 2020 2063  |              c
+00018390: 6f6e 7472 6962 7574 6f72 7320 6d61 7920  ontributors may 
+000183a0: 6265 2075 7365 6420 746f 2065 6e64 6f72  be used to endor
+000183b0: 7365 206f 7220 7072 6f6d 6f74 6520 7072  se or promote pr
+000183c0: 6f64 7563 7473 2064 6572 6976 6564 2066  oducts derived f
+000183d0: 726f 6d20 2020 2020 2020 2020 2020 7c0a  rom           |.
 000183e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 000183f0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00018400: 2020 2020 2020 2020 2020 2061 6e64 2f6f             and/o
-00018410: 7220 6f74 6865 7220 6d61 7465 7269 616c  r other material
-00018420: 7320 7072 6f76 6964 6564 2077 6974 6820  s provided with 
-00018430: 7468 6520 6469 7374 7269 6275 7469 6f6e  the distribution
-00018440: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00018400: 2020 2020 2020 2020 2020 7468 6973 2073            this s
+00018410: 6f66 7477 6172 6520 7769 7468 6f75 7420  oftware without 
+00018420: 7370 6563 6966 6963 2070 7269 6f72 2077  specific prior w
+00018430: 7269 7474 656e 2070 6572 6d69 7373 696f  ritten permissio
+00018440: 6e2e 2020 2020 2020 2020 2020 2020 2020  n.              
 00018450: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00018460: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 00018470: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00018480: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00018490: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000184a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000184b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000184c0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 000184d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000184e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184f0: 2020 2020 2020 2a20 4e65 6974 6865 7220        * Neither 
-00018500: 7468 6520 6e61 6d65 206f 6620 6c6f 6766  the name of logf
-00018510: 7572 7920 6e6f 7220 7468 6520 6e61 6d65  ury nor the name
-00018520: 7320 6f66 2069 7473 2020 2020 2020 2020  s of its        
-00018530: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000184e0: 2020 2020 2020 2020 2054 4849 5320 534f           THIS SO
+000184f0: 4654 5741 5245 2049 5320 5052 4f56 4944  FTWARE IS PROVID
+00018500: 4544 2042 5920 5448 4520 434f 5059 5249  ED BY THE COPYRI
+00018510: 4748 5420 484f 4c44 4552 5320 414e 4420  GHT HOLDERS AND 
+00018520: 434f 4e54 5249 4255 544f 5253 2022 4153  CONTRIBUTORS "AS
+00018530: 2049 5322 2020 2020 2020 2020 207c 0a7c   IS"         |.|
 00018540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018550: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00018560: 2020 2063 6f6e 7472 6962 7574 6f72 7320     contributors 
-00018570: 6d61 7920 6265 2075 7365 6420 746f 2065  may be used to e
-00018580: 6e64 6f72 7365 206f 7220 7072 6f6d 6f74  ndorse or promot
-00018590: 6520 7072 6f64 7563 7473 2064 6572 6976  e products deriv
-000185a0: 6564 2066 726f 6d20 2020 2020 2020 2020  ed from         
+00018550: 2020 2020 7c20 2020 2020 2020 2020 2041      |          A
+00018560: 4e44 2041 4e59 2045 5850 5245 5353 204f  ND ANY EXPRESS O
+00018570: 5220 494d 504c 4945 4420 5741 5252 414e  R IMPLIED WARRAN
+00018580: 5449 4553 2c20 494e 434c 5544 494e 472c  TIES, INCLUDING,
+00018590: 2042 5554 204e 4f54 204c 494d 4954 4544   BUT NOT LIMITED
+000185a0: 2054 4f2c 2054 4845 2020 2020 2020 2020   TO, THE        
 000185b0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 000185c0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000185d0: 2020 2020 2020 2020 2020 2020 2020 7468                th
-000185e0: 6973 2073 6f66 7477 6172 6520 7769 7468  is software with
-000185f0: 6f75 7420 7370 6563 6966 6963 2070 7269  out specific pri
-00018600: 6f72 2077 7269 7474 656e 2070 6572 6d69  or written permi
-00018610: 7373 696f 6e2e 2020 2020 2020 2020 2020  ssion.          
+000185d0: 2020 494d 504c 4945 4420 5741 5252 414e    IMPLIED WARRAN
+000185e0: 5449 4553 204f 4620 4d45 5243 4841 4e54  TIES OF MERCHANT
+000185f0: 4142 494c 4954 5920 414e 4420 4649 544e  ABILITY AND FITN
+00018600: 4553 5320 464f 5220 4120 5041 5254 4943  ESS FOR A PARTIC
+00018610: 554c 4152 2050 5552 504f 5345 2041 5245  ULAR PURPOSE ARE
 00018620: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00018630: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00018640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018690: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00018640: 2020 2020 2020 2020 4449 5343 4c41 494d          DISCLAIM
+00018650: 4544 2e20 494e 204e 4f20 4556 454e 5420  ED. IN NO EVENT 
+00018660: 5348 414c 4c20 5448 4520 434f 5059 5249  SHALL THE COPYRI
+00018670: 4748 5420 484f 4c44 4552 204f 5220 434f  GHT HOLDER OR CO
+00018680: 4e54 5249 4255 544f 5253 2042 4520 4c49  NTRIBUTORS BE LI
+00018690: 4142 4c45 2020 2020 2020 2020 7c0a 7c20  ABLE        |.| 
 000186a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186b0: 2020 207c 2020 2020 2020 2020 2054 4849     |         THI
-000186c0: 5320 534f 4654 5741 5245 2049 5320 5052  S SOFTWARE IS PR
-000186d0: 4f56 4944 4544 2042 5920 5448 4520 434f  OVIDED BY THE CO
-000186e0: 5059 5249 4748 5420 484f 4c44 4552 5320  PYRIGHT HOLDERS 
-000186f0: 414e 4420 434f 4e54 5249 4255 544f 5253  AND CONTRIBUTORS
-00018700: 2022 4153 2049 5322 2020 2020 2020 2020   "AS IS"        
+000186b0: 2020 207c 2020 2020 2020 2020 2020 464f     |          FO
+000186c0: 5220 414e 5920 4449 5245 4354 2c20 494e  R ANY DIRECT, IN
+000186d0: 4449 5245 4354 2c20 494e 4349 4445 4e54  DIRECT, INCIDENT
+000186e0: 414c 2c20 5350 4543 4941 4c2c 2045 5845  AL, SPECIAL, EXE
+000186f0: 4d50 4c41 5259 2c20 4f52 2043 4f4e 5345  MPLARY, OR CONSE
+00018700: 5155 454e 5449 414c 2020 2020 2020 2020  QUENTIAL        
 00018710: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00018720: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00018730: 2020 2041 4e44 2041 4e59 2045 5850 5245     AND ANY EXPRE
-00018740: 5353 204f 5220 494d 504c 4945 4420 5741  SS OR IMPLIED WA
-00018750: 5252 414e 5449 4553 2c20 494e 434c 5544  RRANTIES, INCLUD
-00018760: 494e 472c 2042 5554 204e 4f54 204c 494d  ING, BUT NOT LIM
-00018770: 4954 4544 2054 4f2c 2054 4845 2020 2020  ITED TO, THE    
+00018730: 2020 2044 414d 4147 4553 2028 494e 434c     DAMAGES (INCL
+00018740: 5544 494e 472c 2042 5554 204e 4f54 204c  UDING, BUT NOT L
+00018750: 494d 4954 4544 2054 4f2c 2050 524f 4355  IMITED TO, PROCU
+00018760: 5245 4d45 4e54 204f 4620 5355 4253 5449  REMENT OF SUBSTI
+00018770: 5455 5445 2047 4f4f 4453 204f 5220 2020  TUTE GOODS OR   
 00018780: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00018790: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-000187a0: 2020 2020 2020 494d 504c 4945 4420 5741        IMPLIED WA
-000187b0: 5252 414e 5449 4553 204f 4620 4d45 5243  RRANTIES OF MERC
-000187c0: 4841 4e54 4142 494c 4954 5920 414e 4420  HANTABILITY AND 
-000187d0: 4649 544e 4553 5320 464f 5220 4120 5041  FITNESS FOR A PA
-000187e0: 5254 4943 554c 4152 2050 5552 504f 5345  RTICULAR PURPOSE
-000187f0: 2041 5245 2020 2020 2020 207c 0a7c 2020   ARE       |.|  
+000187a0: 2020 2020 2020 2020 5345 5256 4943 4553          SERVICES
+000187b0: 3b20 4c4f 5353 204f 4620 5553 452c 2044  ; LOSS OF USE, D
+000187c0: 4154 412c 204f 5220 5052 4f46 4954 533b  ATA, OR PROFITS;
+000187d0: 204f 5220 4255 5349 4e45 5353 2049 4e54   OR BUSINESS INT
+000187e0: 4552 5255 5054 494f 4e29 2048 4f57 4556  ERRUPTION) HOWEV
+000187f0: 4552 2020 2020 2020 2020 207c 0a7c 2020  ER         |.|  
 00018800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018810: 2020 7c20 2020 2020 2020 2020 4449 5343    |         DISC
-00018820: 4c41 494d 4544 2e20 494e 204e 4f20 4556  LAIMED. IN NO EV
-00018830: 454e 5420 5348 414c 4c20 5448 4520 434f  ENT SHALL THE CO
-00018840: 5059 5249 4748 5420 484f 4c44 4552 204f  PYRIGHT HOLDER O
-00018850: 5220 434f 4e54 5249 4255 544f 5253 2042  R CONTRIBUTORS B
-00018860: 4520 4c49 4142 4c45 2020 2020 2020 2020  E LIABLE        
+00018810: 2020 7c20 2020 2020 2020 2043 4155 5345    |        CAUSE
+00018820: 4420 414e 4420 4f4e 2041 4e59 2054 4845  D AND ON ANY THE
+00018830: 4f52 5920 4f46 204c 4941 4249 4c49 5459  ORY OF LIABILITY
+00018840: 2c20 5748 4554 4845 5220 494e 2043 4f4e  , WHETHER IN CON
+00018850: 5452 4143 542c 2053 5452 4943 5420 4c49  TRACT, STRICT LI
+00018860: 4142 494c 4954 592c 2020 2020 2020 2020  ABILITY,        
 00018870: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00018880: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00018890: 2020 464f 5220 414e 5920 4449 5245 4354    FOR ANY DIRECT
-000188a0: 2c20 494e 4449 5245 4354 2c20 494e 4349  , INDIRECT, INCI
-000188b0: 4445 4e54 414c 2c20 5350 4543 4941 4c2c  DENTAL, SPECIAL,
-000188c0: 2045 5845 4d50 4c41 5259 2c20 4f52 2043   EXEMPLARY, OR C
-000188d0: 4f4e 5345 5155 454e 5449 414c 2020 2020  ONSEQUENTIAL    
+00018890: 4f52 2054 4f52 5420 2849 4e43 4c55 4449  OR TORT (INCLUDI
+000188a0: 4e47 204e 4547 4c49 4745 4e43 4520 4f52  NG NEGLIGENCE OR
+000188b0: 204f 5448 4552 5749 5345 2920 4152 4953   OTHERWISE) ARIS
+000188c0: 494e 4720 494e 2041 4e59 2057 4159 204f  ING IN ANY WAY O
+000188d0: 5554 204f 4620 5448 4520 5553 4520 2020  UT OF THE USE   
 000188e0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 000188f0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00018900: 2020 2020 2020 2044 414d 4147 4553 2028         DAMAGES (
-00018910: 494e 434c 5544 494e 472c 2042 5554 204e  INCLUDING, BUT N
-00018920: 4f54 204c 494d 4954 4544 2054 4f2c 2050  OT LIMITED TO, P
-00018930: 524f 4355 5245 4d45 4e54 204f 4620 5355  ROCUREMENT OF SU
-00018940: 4253 5449 5455 5445 2047 4f4f 4453 204f  BSTITUTE GOODS O
-00018950: 5220 2020 2020 2020 2020 7c0a 7c20 2020  R         |.|   
+00018900: 2020 2020 2020 2020 2020 4f46 2054 4849            OF THI
+00018910: 5320 534f 4654 5741 5245 2c20 4556 454e  S SOFTWARE, EVEN
+00018920: 2049 4620 4144 5649 5345 4420 4f46 2054   IF ADVISED OF T
+00018930: 4845 2050 4f53 5349 4249 4c49 5459 204f  HE POSSIBILITY O
+00018940: 4620 5355 4348 2044 414d 4147 452e 2020  F SUCH DAMAGE.  
+00018950: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00018960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018970: 207c 2020 2020 2020 2020 2020 5345 5256   |          SERV
-00018980: 4943 4553 3b20 4c4f 5353 204f 4620 5553  ICES; LOSS OF US
-00018990: 452c 2044 4154 412c 204f 5220 5052 4f46  E, DATA, OR PROF
-000189a0: 4954 533b 204f 5220 4255 5349 4e45 5353  ITS; OR BUSINESS
-000189b0: 2049 4e54 4552 5255 5054 494f 4e29 2048   INTERRUPTION) H
-000189c0: 4f57 4556 4552 2020 2020 2020 2020 207c  OWEVER         |
-000189d0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-000189e0: 2020 2020 2020 7c20 2020 2020 2020 2043        |        C
-000189f0: 4155 5345 4420 414e 4420 4f4e 2041 4e59  AUSED AND ON ANY
-00018a00: 2054 4845 4f52 5920 4f46 204c 4941 4249   THEORY OF LIABI
-00018a10: 4c49 5459 2c20 5748 4554 4845 5220 494e  LITY, WHETHER IN
-00018a20: 2043 4f4e 5452 4143 542c 2053 5452 4943   CONTRACT, STRIC
-00018a30: 5420 4c49 4142 494c 4954 592c 2020 2020  T LIABILITY,    
-00018a40: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00018a50: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00018a60: 2020 2020 4f52 2054 4f52 5420 2849 4e43      OR TORT (INC
-00018a70: 4c55 4449 4e47 204e 4547 4c49 4745 4e43  LUDING NEGLIGENC
-00018a80: 4520 4f52 204f 5448 4552 5749 5345 2920  E OR OTHERWISE) 
-00018a90: 4152 4953 494e 4720 494e 2041 4e59 2057  ARISING IN ANY W
-00018aa0: 4159 204f 5554 204f 4620 5448 4520 5553  AY OUT OF THE US
-00018ab0: 4520 2020 2020 2020 207c 0a7c 2020 2020  E        |.|    
+00018970: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00018980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189c0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000189d0: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+000189e0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+000189f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00018a00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00018a10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00018a20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00018a30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00018a40: 2d2d 2d2d 2b0a 7c20 7068 782d 636c 6173  ----+.| phx-clas
+00018a50: 732d 7265 6769 7374 7279 207c 2020 2020  s-registry |    
+00018a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a80: 2020 2020 204d 4954 204c 6963 656e 6365       MIT Licence
+00018a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ab0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00018ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ad0: 7c20 2020 2020 2020 2020 2020 2020 4f46  |             OF
-00018ae0: 2054 4849 5320 534f 4654 5741 5245 2c20   THIS SOFTWARE, 
-00018af0: 4556 454e 2049 4620 4144 5649 5345 4420  EVEN IF ADVISED 
-00018b00: 4f46 2054 4845 2050 4f53 5349 4249 4c49  OF THE POSSIBILI
-00018b10: 5459 204f 4620 5355 4348 2044 414d 4147  TY OF SUCH DAMAG
-00018b20: 452e 2020 2020 2020 2020 2020 2020 7c0a  E.            |.
+00018ad0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00018ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b20: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00018b30: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00018b40: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 00018b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b60: 2020 2020 2020 436f 7079 7269 6768 7420        Copyright 
+00018b70: 2863 2920 3230 3137 2045 464c 2047 6c6f  (c) 2017 EFL Glo
+00018b80: 6261 6c20 2020 2020 2020 2020 2020 2020  bal             
 00018b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ba0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-00018bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00018bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00018bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00018be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00018bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00018c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00018c10: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 7068 782d  --------+.| phx-
-00018c20: 636c 6173 732d 7265 6769 7374 7279 207c  class-registry |
-00018c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c50: 2020 2020 2020 2020 204d 4954 204c 6963           MIT Lic
-00018c60: 656e 6365 2020 2020 2020 2020 2020 2020  ence            
-00018c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c80: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00018ba0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+00018bb0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00018bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c10: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+00018c20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00018c30: 2020 2020 2020 2020 2050 6572 6d69 7373           Permiss
+00018c40: 696f 6e20 6973 2068 6572 6562 7920 6772  ion is hereby gr
+00018c50: 616e 7465 642c 2066 7265 6520 6f66 2063  anted, free of c
+00018c60: 6861 7267 652c 2074 6f20 616e 7920 7065  harge, to any pe
+00018c70: 7273 6f6e 206f 6274 6169 6e69 6e67 2061  rson obtaining a
+00018c80: 2063 6f70 7920 2020 2020 2020 207c 0a7c   copy        |.|
 00018c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ca0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00018cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018ca0: 2020 2020 7c20 2020 2020 2020 206f 6620      |        of 
+00018cb0: 7468 6973 2073 6f66 7477 6172 6520 616e  this software an
+00018cc0: 6420 6173 736f 6369 6174 6564 2064 6f63  d associated doc
+00018cd0: 756d 656e 7461 7469 6f6e 2066 696c 6573  umentation files
+00018ce0: 2028 7468 6520 2253 6f66 7477 6172 6522   (the "Software"
+00018cf0: 292c 2074 6f20 6465 616c 2020 2020 2020  ), to deal      
 00018d00: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00018d10: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00018d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d30: 2020 2020 2020 2020 2020 436f 7079 7269            Copyri
-00018d40: 6768 7420 2863 2920 3230 3137 2045 464c  ght (c) 2017 EFL
-00018d50: 2047 6c6f 6261 6c20 2020 2020 2020 2020   Global         
-00018d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018d20: 2020 2069 6e20 7468 6520 536f 6674 7761     in the Softwa
+00018d30: 7265 2077 6974 686f 7574 2072 6573 7472  re without restr
+00018d40: 6963 7469 6f6e 2c20 696e 636c 7564 696e  iction, includin
+00018d50: 6720 7769 7468 6f75 7420 6c69 6d69 7461  g without limita
+00018d60: 7469 6f6e 2074 6865 2072 6967 6874 7320  tion the rights 
 00018d70: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00018d80: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00018d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018de0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00018d90: 2020 2020 2020 2020 2074 6f20 7573 652c           to use,
+00018da0: 2063 6f70 792c 206d 6f64 6966 792c 206d   copy, modify, m
+00018db0: 6572 6765 2c20 7075 626c 6973 682c 2064  erge, publish, d
+00018dc0: 6973 7472 6962 7574 652c 2073 7562 6c69  istribute, subli
+00018dd0: 6365 6e73 652c 2061 6e64 2f6f 7220 7365  cense, and/or se
+00018de0: 6c6c 2020 2020 2020 2020 2020 7c0a 7c20  ll          |.| 
 00018df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e00: 2020 207c 2020 2020 2020 2020 2050 6572     |         Per
-00018e10: 6d69 7373 696f 6e20 6973 2068 6572 6562  mission is hereb
-00018e20: 7920 6772 616e 7465 642c 2066 7265 6520  y granted, free 
-00018e30: 6f66 2063 6861 7267 652c 2074 6f20 616e  of charge, to an
-00018e40: 7920 7065 7273 6f6e 206f 6274 6169 6e69  y person obtaini
-00018e50: 6e67 2061 2063 6f70 7920 2020 2020 2020  ng a copy       
+00018e00: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+00018e10: 636f 7069 6573 206f 6620 7468 6520 536f  copies of the So
+00018e20: 6674 7761 7265 2c20 616e 6420 746f 2070  ftware, and to p
+00018e30: 6572 6d69 7420 7065 7273 6f6e 7320 746f  ermit persons to
+00018e40: 2077 686f 6d20 7468 6520 536f 6674 7761   whom the Softwa
+00018e50: 7265 2069 7320 2020 2020 2020 2020 2020  re is           
 00018e60: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00018e70: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00018e80: 206f 6620 7468 6973 2073 6f66 7477 6172   of this softwar
-00018e90: 6520 616e 6420 6173 736f 6369 6174 6564  e and associated
-00018ea0: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
-00018eb0: 696c 6573 2028 7468 6520 2253 6f66 7477  iles (the "Softw
-00018ec0: 6172 6522 292c 2074 6f20 6465 616c 2020  are"), to deal  
+00018e80: 2020 2020 2020 2020 2020 2020 6675 726e              furn
+00018e90: 6973 6865 6420 746f 2064 6f20 736f 2c20  ished to do so, 
+00018ea0: 7375 626a 6563 7420 746f 2074 6865 2066  subject to the f
+00018eb0: 6f6c 6c6f 7769 6e67 2063 6f6e 6469 7469  ollowing conditi
+00018ec0: 6f6e 733a 2020 2020 2020 2020 2020 2020  ons:            
 00018ed0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00018ee0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00018ef0: 2020 2020 2020 2069 6e20 7468 6520 536f         in the So
-00018f00: 6674 7761 7265 2077 6974 686f 7574 2072  ftware without r
-00018f10: 6573 7472 6963 7469 6f6e 2c20 696e 636c  estriction, incl
-00018f20: 7564 696e 6720 7769 7468 6f75 7420 6c69  uding without li
-00018f30: 6d69 7461 7469 6f6e 2074 6865 2072 6967  mitation the rig
-00018f40: 6874 7320 2020 2020 2020 207c 0a7c 2020  hts        |.|  
+00018ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f40: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00018f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018f60: 2020 7c20 2020 2020 2020 2020 2074 6f20    |          to 
-00018f70: 7573 652c 2063 6f70 792c 206d 6f64 6966  use, copy, modif
-00018f80: 792c 206d 6572 6765 2c20 7075 626c 6973  y, merge, publis
-00018f90: 682c 2064 6973 7472 6962 7574 652c 2073  h, distribute, s
-00018fa0: 7562 6c69 6365 6e73 652c 2061 6e64 2f6f  ublicense, and/o
-00018fb0: 7220 7365 6c6c 2020 2020 2020 2020 2020  r sell          
+00018f60: 2020 7c20 2020 2020 2020 2054 6865 2061    |        The a
+00018f70: 626f 7665 2063 6f70 7972 6967 6874 206e  bove copyright n
+00018f80: 6f74 6963 6520 616e 6420 7468 6973 2070  otice and this p
+00018f90: 6572 6d69 7373 696f 6e20 6e6f 7469 6365  ermission notice
+00018fa0: 2073 6861 6c6c 2062 6520 696e 636c 7564   shall be includ
+00018fb0: 6564 2069 6e20 616c 6c20 2020 2020 2020  ed in all       
 00018fc0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00018fd0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00018fe0: 2020 2020 636f 7069 6573 206f 6620 7468      copies of th
-00018ff0: 6520 536f 6674 7761 7265 2c20 616e 6420  e Software, and 
-00019000: 746f 2070 6572 6d69 7420 7065 7273 6f6e  to permit person
-00019010: 7320 746f 2077 686f 6d20 7468 6520 536f  s to whom the So
-00019020: 6674 7761 7265 2069 7320 2020 2020 2020  ftware is       
+00018fe0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00018ff0: 6f70 6965 7320 6f72 2073 7562 7374 616e  opies or substan
+00019000: 7469 616c 2070 6f72 7469 6f6e 7320 6f66  tial portions of
+00019010: 2074 6865 2053 6f66 7477 6172 652e 2020   the Software.  
+00019020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019030: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00019040: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 00019050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019060: 6675 726e 6973 6865 6420 746f 2064 6f20  furnished to do 
-00019070: 736f 2c20 7375 626a 6563 7420 746f 2074  so, subject to t
-00019080: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
-00019090: 6469 7469 6f6e 733a 2020 2020 2020 2020  ditions:        
+00019060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000190a0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 000190b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190c0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-000190d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000190f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019110: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000190c0: 207c 2020 2020 2020 2020 2020 5448 4520   |          THE 
+000190d0: 534f 4654 5741 5245 2049 5320 5052 4f56  SOFTWARE IS PROV
+000190e0: 4944 4544 2022 4153 2049 5322 2c20 5749  IDED "AS IS", WI
+000190f0: 5448 4f55 5420 5741 5252 414e 5459 204f  THOUT WARRANTY O
+00019100: 4620 414e 5920 4b49 4e44 2c20 4558 5052  F ANY KIND, EXPR
+00019110: 4553 5320 4f52 2020 2020 2020 2020 207c  ESS OR         |
 00019120: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00019130: 2020 2020 2020 7c20 2020 2020 2020 2054        |        T
-00019140: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
-00019150: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
-00019160: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
-00019170: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
-00019180: 636c 7564 6564 2069 6e20 616c 6c20 2020  cluded in all   
+00019130: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00019140: 2020 494d 504c 4945 442c 2049 4e43 4c55    IMPLIED, INCLU
+00019150: 4449 4e47 2042 5554 204e 4f54 204c 494d  DING BUT NOT LIM
+00019160: 4954 4544 2054 4f20 5448 4520 5741 5252  ITED TO THE WARR
+00019170: 414e 5449 4553 204f 4620 4d45 5243 4841  ANTIES OF MERCHA
+00019180: 4e54 4142 494c 4954 592c 2020 2020 2020  NTABILITY,      
 00019190: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 000191a0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000191b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000191c0: 2020 2063 6f70 6965 7320 6f72 2073 7562     copies or sub
-000191d0: 7374 616e 7469 616c 2070 6f72 7469 6f6e  stantial portion
-000191e0: 7320 6f66 2074 6865 2053 6f66 7477 6172  s of the Softwar
-000191f0: 652e 2020 2020 2020 2020 2020 2020 2020  e.              
+000191b0: 2020 2020 2046 4954 4e45 5353 2046 4f52       FITNESS FOR
+000191c0: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
+000191d0: 5250 4f53 4520 414e 4420 4e4f 4e49 4e46  RPOSE AND NONINF
+000191e0: 5249 4e47 454d 454e 542e 2049 4e20 4e4f  RINGEMENT. IN NO
+000191f0: 2045 5645 4e54 2053 4841 4c4c 2054 4845   EVENT SHALL THE
 00019200: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00019210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019220: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00019230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019270: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00019220: 7c20 2020 2020 2020 2020 2020 2041 5554  |            AUT
+00019230: 484f 5253 204f 5220 434f 5059 5249 4748  HORS OR COPYRIGH
+00019240: 5420 484f 4c44 4552 5320 4245 204c 4941  T HOLDERS BE LIA
+00019250: 424c 4520 464f 5220 414e 5920 434c 4149  BLE FOR ANY CLAI
+00019260: 4d2c 2044 414d 4147 4553 204f 5220 4f54  M, DAMAGES OR OT
+00019270: 4845 5220 2020 2020 2020 2020 2020 7c0a  HER           |.
 00019280: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00019290: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000192a0: 5448 4520 534f 4654 5741 5245 2049 5320  THE SOFTWARE IS 
-000192b0: 5052 4f56 4944 4544 2022 4153 2049 5322  PROVIDED "AS IS"
-000192c0: 2c20 5749 5448 4f55 5420 5741 5252 414e  , WITHOUT WARRAN
-000192d0: 5459 204f 4620 414e 5920 4b49 4e44 2c20  TY OF ANY KIND, 
-000192e0: 4558 5052 4553 5320 4f52 2020 2020 2020  EXPRESS OR      
+00019290: 2020 2020 207c 2020 2020 2020 2020 4c49       |        LI
+000192a0: 4142 494c 4954 592c 2057 4845 5448 4552  ABILITY, WHETHER
+000192b0: 2049 4e20 414e 2041 4354 494f 4e20 4f46   IN AN ACTION OF
+000192c0: 2043 4f4e 5452 4143 542c 2054 4f52 5420   CONTRACT, TORT 
+000192d0: 4f52 204f 5448 4552 5749 5345 2c20 4152  OR OTHERWISE, AR
+000192e0: 4953 494e 4720 4652 4f4d 2c20 2020 2020  ISING FROM,     
 000192f0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00019300: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00019310: 2020 2020 2020 494d 504c 4945 442c 2049        IMPLIED, I
-00019320: 4e43 4c55 4449 4e47 2042 5554 204e 4f54  NCLUDING BUT NOT
-00019330: 204c 494d 4954 4544 2054 4f20 5448 4520   LIMITED TO THE 
-00019340: 5741 5252 414e 5449 4553 204f 4620 4d45  WARRANTIES OF ME
-00019350: 5243 4841 4e54 4142 494c 4954 592c 2020  RCHANTABILITY,  
+00019310: 2020 204f 5554 204f 4620 4f52 2049 4e20     OUT OF OR IN 
+00019320: 434f 4e4e 4543 5449 4f4e 2057 4954 4820  CONNECTION WITH 
+00019330: 5448 4520 534f 4654 5741 5245 204f 5220  THE SOFTWARE OR 
+00019340: 5448 4520 5553 4520 4f52 204f 5448 4552  THE USE OR OTHER
+00019350: 2044 4541 4c49 4e47 5320 494e 2054 4845   DEALINGS IN THE
 00019360: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00019370: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00019380: 2020 2020 2020 2020 2046 4954 4e45 5353           FITNESS
-00019390: 2046 4f52 2041 2050 4152 5449 4355 4c41   FOR A PARTICULA
-000193a0: 5220 5055 5250 4f53 4520 414e 4420 4e4f  R PURPOSE AND NO
-000193b0: 4e49 4e46 5249 4e47 454d 454e 542e 2049  NINFRINGEMENT. I
-000193c0: 4e20 4e4f 2045 5645 4e54 2053 4841 4c4c  N NO EVENT SHALL
-000193d0: 2054 4845 2020 2020 2020 2020 207c 0a7c   THE         |.|
+00019380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193a0: 2020 2020 2020 2020 2020 534f 4654 5741            SOFTWA
+000193b0: 5245 2e20 2020 2020 2020 2020 2020 2020  RE.             
+000193c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000193d0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 000193e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000193f0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00019400: 2041 5554 484f 5253 204f 5220 434f 5059   AUTHORS OR COPY
-00019410: 5249 4748 5420 484f 4c44 4552 5320 4245  RIGHT HOLDERS BE
-00019420: 204c 4941 424c 4520 464f 5220 414e 5920   LIABLE FOR ANY 
-00019430: 434c 4149 4d2c 2044 414d 4147 4553 204f  CLAIM, DAMAGES O
-00019440: 5220 4f54 4845 5220 2020 2020 2020 2020  R OTHER         
-00019450: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00019460: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00019470: 2020 4c49 4142 494c 4954 592c 2057 4845    LIABILITY, WHE
-00019480: 5448 4552 2049 4e20 414e 2041 4354 494f  THER IN AN ACTIO
-00019490: 4e20 4f46 2043 4f4e 5452 4143 542c 2054  N OF CONTRACT, T
-000194a0: 4f52 5420 4f52 204f 5448 4552 5749 5345  ORT OR OTHERWISE
-000194b0: 2c20 4152 4953 494e 4720 4652 4f4d 2c20  , ARISING FROM, 
-000194c0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-000194d0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000194e0: 2020 2020 2020 204f 5554 204f 4620 4f52         OUT OF OR
-000194f0: 2049 4e20 434f 4e4e 4543 5449 4f4e 2057   IN CONNECTION W
-00019500: 4954 4820 5448 4520 534f 4654 5741 5245  ITH THE SOFTWARE
-00019510: 204f 5220 5448 4520 5553 4520 4f52 204f   OR THE USE OR O
-00019520: 5448 4552 2044 4541 4c49 4e47 5320 494e  THER DEALINGS IN
-00019530: 2054 4845 2020 2020 2020 2020 7c0a 7c20   THE        |.| 
+00019400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019450: 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.+-----------
+00019460: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00019470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00019480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00019490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000194a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000194b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000194c0: 2d2d 2d2d 2d2d 2d2b 0a7c 2020 7079 7468  -------+.|  pyth
+000194d0: 6f6e 2d64 6174 6575 7469 6c20 2020 7c20  on-dateutil   | 
+000194e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000194f0: 2020 2020 2020 2043 6f70 7972 6967 6874         Copyright
+00019500: 2032 3031 372d 2050 6175 6c20 4761 6e73   2017- Paul Gans
+00019510: 736c 6520 3c70 6175 6c40 6761 6e73 736c  sle <paul@ganssl
+00019520: 652e 696f 3e20 2020 2020 2020 2020 2020  e.io>           
+00019530: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00019540: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019550: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00019560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019570: 2020 2020 2020 2020 2020 2020 2020 534f                SO
-00019580: 4654 5741 5245 2e20 2020 2020 2020 2020  FTWARE.         
-00019590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019560: 2020 2020 2020 2043 6f70 7972 6967 6874         Copyright
+00019570: 2032 3031 372d 2064 6174 6575 7469 6c20   2017- dateutil 
+00019580: 636f 6e74 7269 6275 746f 7273 2028 7365  contributors (se
+00019590: 6520 4155 5448 4f52 5320 6669 6c65 2920  e AUTHORS file) 
 000195a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000195b0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 000195c0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
 000195d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000195e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000195f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019600: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019620: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
-00019630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00019640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00019650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00019660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00019670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00019680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00019690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020  -----------+.|  
-000196a0: 2020 2020 2020 7069 7020 2020 2020 2020        pip       
+00019620: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+00019630: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00019640: 2020 2020 2020 2020 2020 2020 2020 204c                 L
+00019650: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
+00019660: 6520 4170 6163 6865 204c 6963 656e 7365  e Apache License
+00019670: 2c20 5665 7273 696f 6e20 322e 3020 2874  , Version 2.0 (t
+00019680: 6865 2022 4c69 6365 6e73 6522 293b 2020  he "License");  
+00019690: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+000196a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000196b0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-000196c0: 436f 7079 7269 6768 7420 2863 2920 3230  Copyright (c) 20
-000196d0: 3038 2d70 7265 7365 6e74 2054 6865 2070  08-present The p
-000196e0: 6970 2064 6576 656c 6f70 6572 7320 2873  ip developers (s
-000196f0: 6565 2041 5554 484f 5253 2e74 7874 2066  ee AUTHORS.txt f
-00019700: 696c 6529 2020 2020 2020 2020 2020 2020  ile)            
+000196c0: 2020 2079 6f75 206d 6179 206e 6f74 2075     you may not u
+000196d0: 7365 2074 6869 7320 6669 6c65 2065 7863  se this file exc
+000196e0: 6570 7420 696e 2063 6f6d 706c 6961 6e63  ept in complianc
+000196f0: 6520 7769 7468 2074 6865 204c 6963 656e  e with the Licen
+00019700: 7365 2e20 2020 2020 2020 2020 2020 2020  se.             
 00019710: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00019720: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 00019730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019740: 2020 2020 2059 6f75 206d 6179 206f 6274       You may obt
+00019750: 6169 6e20 6120 636f 7079 206f 6620 7468  ain a copy of th
+00019760: 6520 4c69 6365 6e73 6520 6174 2020 2020  e License at    
 00019770: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019780: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00019790: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000197a0: 2020 2020 2020 2020 2050 6572 6d69 7373           Permiss
-000197b0: 696f 6e20 6973 2068 6572 6562 7920 6772  ion is hereby gr
-000197c0: 616e 7465 642c 2066 7265 6520 6f66 2063  anted, free of c
-000197d0: 6861 7267 652c 2074 6f20 616e 7920 7065  harge, to any pe
-000197e0: 7273 6f6e 206f 6274 6169 6e69 6e67 2020  rson obtaining  
+000197a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000197e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000197f0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00019800: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019810: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00019820: 2061 2063 6f70 7920 6f66 2074 6869 7320   a copy of this 
-00019830: 736f 6674 7761 7265 2061 6e64 2061 7373  software and ass
-00019840: 6f63 6961 7465 6420 646f 6375 6d65 6e74  ociated document
-00019850: 6174 696f 6e20 6669 6c65 7320 2874 6865  ation files (the
+00019820: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00019830: 7474 703a 2f2f 7777 772e 6170 6163 6865  ttp://www.apache
+00019840: 2e6f 7267 2f6c 6963 656e 7365 732f 4c49  .org/licenses/LI
+00019850: 4345 4e53 452d 322e 3020 2020 2020 2020  CENSE-2.0       
 00019860: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00019870: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00019880: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00019890: 2020 2020 2253 6f66 7477 6172 6522 292c      "Software"),
-000198a0: 2074 6f20 6465 616c 2069 6e20 7468 6520   to deal in the 
-000198b0: 536f 6674 7761 7265 2077 6974 686f 7574  Software without
-000198c0: 2072 6573 7472 6963 7469 6f6e 2c20 696e   restriction, in
-000198d0: 636c 7564 696e 6720 2020 2020 2020 2020  cluding         
+00019890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000198e0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 000198f0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00019900: 2020 2020 2020 2020 2077 6974 686f 7574           without
-00019910: 206c 696d 6974 6174 696f 6e20 7468 6520   limitation the 
-00019920: 7269 6768 7473 2074 6f20 7573 652c 2063  rights to use, c
-00019930: 6f70 792c 206d 6f64 6966 792c 206d 6572  opy, modify, mer
-00019940: 6765 2c20 7075 626c 6973 682c 2020 2020  ge, publish,    
+00019900: 2020 2020 2020 2020 2020 2055 6e6c 6573             Unles
+00019910: 7320 7265 7175 6972 6564 2062 7920 6170  s required by ap
+00019920: 706c 6963 6162 6c65 206c 6177 206f 7220  plicable law or 
+00019930: 6167 7265 6564 2074 6f20 696e 2077 7269  agreed to in wri
+00019940: 7469 6e67 2c20 736f 6674 7761 7265 2020  ting, software  
 00019950: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00019960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019970: 7c20 2020 2020 2020 2020 2020 2020 2064  |              d
-00019980: 6973 7472 6962 7574 652c 2073 7562 6c69  istribute, subli
-00019990: 6365 6e73 652c 2061 6e64 2f6f 7220 7365  cense, and/or se
-000199a0: 6c6c 2063 6f70 6965 7320 6f66 2074 6865  ll copies of the
-000199b0: 2053 6f66 7477 6172 652c 2061 6e64 2074   Software, and t
-000199c0: 6f20 2020 2020 2020 2020 2020 2020 7c0a  o             |.
+00019970: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00019980: 2064 6973 7472 6962 7574 6564 2075 6e64   distributed und
+00019990: 6572 2074 6865 204c 6963 656e 7365 2069  er the License i
+000199a0: 7320 6469 7374 7269 6275 7465 6420 6f6e  s distributed on
+000199b0: 2061 6e20 2241 5320 4953 2220 4241 5349   an "AS IS" BASI
+000199c0: 532c 2020 2020 2020 2020 2020 2020 7c0a  S,            |.
 000199d0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 000199e0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000199f0: 2020 7065 726d 6974 2070 6572 736f 6e73    permit persons
-00019a00: 2074 6f20 7768 6f6d 2074 6865 2053 6f66   to whom the Sof
-00019a10: 7477 6172 6520 6973 2066 7572 6e69 7368  tware is furnish
-00019a20: 6564 2074 6f20 646f 2073 6f2c 2073 7562  ed to do so, sub
-00019a30: 6a65 6374 2074 6f20 2020 2020 2020 2020  ject to         
+000199f0: 2020 5749 5448 4f55 5420 5741 5252 414e    WITHOUT WARRAN
+00019a00: 5449 4553 204f 5220 434f 4e44 4954 494f  TIES OR CONDITIO
+00019a10: 4e53 204f 4620 414e 5920 4b49 4e44 2c20  NS OF ANY KIND, 
+00019a20: 6569 7468 6572 2065 7870 7265 7373 206f  either express o
+00019a30: 7220 696d 706c 6965 642e 2020 2020 2020  r implied.      
 00019a40: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00019a50: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00019a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a70: 2020 2020 2020 2020 2020 2020 2074 6865               the
-00019a80: 2066 6f6c 6c6f 7769 6e67 2063 6f6e 6469   following condi
-00019a90: 7469 6f6e 733a 2020 2020 2020 2020 2020  tions:          
-00019aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a60: 2020 2020 2020 2020 2020 5365 6520 7468            See th
+00019a70: 6520 4c69 6365 6e73 6520 666f 7220 7468  e License for th
+00019a80: 6520 7370 6563 6966 6963 206c 616e 6775  e specific langu
+00019a90: 6167 6520 676f 7665 726e 696e 6720 7065  age governing pe
+00019aa0: 726d 6973 7369 6f6e 7320 616e 6420 2020  rmissions and   
 00019ab0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00019ac0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00019ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019af0: 206c 696d 6974 6174 696f 6e73 2075 6e64   limitations und
+00019b00: 6572 2074 6865 204c 6963 656e 7365 2e20  er the License. 
 00019b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019b20: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00019b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019b40: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00019b50: 2020 2020 2054 6865 2061 626f 7665 2063       The above c
-00019b60: 6f70 7972 6967 6874 206e 6f74 6963 6520  opyright notice 
-00019b70: 616e 6420 7468 6973 2070 6572 6d69 7373  and this permiss
-00019b80: 696f 6e20 6e6f 7469 6365 2073 6861 6c6c  ion notice shall
-00019b90: 2062 6520 2020 2020 2020 2020 2020 2020   be             
+00019b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019ba0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00019bb0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00019bc0: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
-00019bd0: 6420 696e 2061 6c6c 2063 6f70 6965 7320  d in all copies 
-00019be0: 6f72 2073 7562 7374 616e 7469 616c 2070  or substantial p
-00019bf0: 6f72 7469 6f6e 7320 6f66 2074 6865 2053  ortions of the S
-00019c00: 6f66 7477 6172 652e 2020 2020 2020 2020  oftware.        
+00019bc0: 2020 2054 6865 2061 626f 7665 206c 6963     The above lic
+00019bd0: 656e 7365 2061 7070 6c69 6573 2074 6f20  ense applies to 
+00019be0: 616c 6c20 636f 6e74 7269 6275 7469 6f6e  all contribution
+00019bf0: 7320 6166 7465 7220 3230 3137 2d31 322d  s after 2017-12-
+00019c00: 3031 2c20 6173 2077 656c 6c20 6173 2020  01, as well as  
 00019c10: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00019c20: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00019c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c80: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00019c30: 2020 2020 2020 2061 6c6c 2063 6f6e 7472         all contr
+00019c40: 6962 7574 696f 6e73 2074 6861 7420 6861  ibutions that ha
+00019c50: 7665 2062 6565 6e20 7265 2d6c 6963 656e  ve been re-licen
+00019c60: 7365 6420 2873 6565 2041 5554 484f 5253  sed (see AUTHORS
+00019c70: 2066 696c 6520 666f 7220 7468 6520 6c69   file for the li
+00019c80: 7374 206f 6620 2020 2020 2020 7c0a 7c20  st of       |.| 
 00019c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019ca0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00019cb0: 2020 2054 4845 2053 4f46 5457 4152 4520     THE SOFTWARE 
-00019cc0: 4953 2050 524f 5649 4445 4420 2241 5320  IS PROVIDED "AS 
-00019cd0: 4953 222c 2057 4954 484f 5554 2057 4152  IS", WITHOUT WAR
-00019ce0: 5241 4e54 5920 4f46 2041 4e59 204b 494e  RANTY OF ANY KIN
-00019cf0: 442c 2020 2020 2020 2020 2020 2020 2020  D,              
+00019cb0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00019cc0: 7269 6275 746f 7273 2077 686f 2068 6176  ributors who hav
+00019cd0: 6520 7265 2d6c 6963 656e 7365 6420 7468  e re-licensed th
+00019ce0: 6569 7220 636f 6465 292e 2020 2020 2020  eir code).      
+00019cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019d00: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00019d10: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00019d20: 2020 2020 2020 2045 5850 5245 5353 204f         EXPRESS O
-00019d30: 5220 494d 504c 4945 442c 2049 4e43 4c55  R IMPLIED, INCLU
-00019d40: 4449 4e47 2042 5554 204e 4f54 204c 494d  DING BUT NOT LIM
-00019d50: 4954 4544 2054 4f20 5448 4520 5741 5252  ITED TO THE WARR
-00019d60: 414e 5449 4553 204f 4620 2020 2020 2020  ANTIES OF       
+00019d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00019d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00019d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00019d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00019d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00019d70: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00019d80: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00019d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019da0: 2020 4d45 5243 4841 4e54 4142 494c 4954    MERCHANTABILIT
-00019db0: 592c 2046 4954 4e45 5353 2046 4f52 2041  Y, FITNESS FOR A
-00019dc0: 2050 4152 5449 4355 4c41 5220 5055 5250   PARTICULAR PURP
-00019dd0: 4f53 4520 414e 4420 2020 2020 2020 2020  OSE AND         
+00019d90: 2020 2020 2020 2020 2020 2020 2020 6461                da
+00019da0: 7465 7574 696c 202d 2045 7874 656e 7369  teutil - Extensi
+00019db0: 6f6e 7320 746f 2074 6865 2073 7461 6e64  ons to the stand
+00019dc0: 6172 6420 5079 7468 6f6e 2064 6174 6574  ard Python datet
+00019dd0: 696d 6520 6d6f 6475 6c65 2e20 2020 2020  ime module.     
 00019de0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00019df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019e00: 2020 7c20 2020 2020 2020 2020 2020 204e    |            N
-00019e10: 4f4e 494e 4652 494e 4745 4d45 4e54 2e20  ONINFRINGEMENT. 
-00019e20: 494e 204e 4f20 4556 454e 5420 5348 414c  IN NO EVENT SHAL
-00019e30: 4c20 5448 4520 4155 5448 4f52 5320 4f52  L THE AUTHORS OR
-00019e40: 2043 4f50 5952 4947 4854 2048 4f4c 4445   COPYRIGHT HOLDE
-00019e50: 5253 2042 4520 2020 2020 2020 2020 2020  RS BE           
+00019e00: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00019e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00019e60: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00019e70: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00019e80: 2020 2020 4c49 4142 4c45 2046 4f52 2041      LIABLE FOR A
-00019e90: 4e59 2043 4c41 494d 2c20 4441 4d41 4745  NY CLAIM, DAMAGE
-00019ea0: 5320 4f52 204f 5448 4552 204c 4941 4249  S OR OTHER LIABI
-00019eb0: 4c49 5459 2c20 5748 4554 4845 5220 494e  LITY, WHETHER IN
-00019ec0: 2041 4e20 4143 5449 4f4e 2020 2020 2020   AN ACTION      
+00019e80: 2020 2020 2020 436f 7079 7269 6768 7420        Copyright 
+00019e90: 2863 2920 3230 3033 2d32 3031 3120 2d20  (c) 2003-2011 - 
+00019ea0: 4775 7374 6176 6f20 4e69 656d 6579 6572  Gustavo Niemeyer
+00019eb0: 203c 6775 7374 6176 6f40 6e69 656d 6579   <gustavo@niemey
+00019ec0: 6572 2e6e 6574 3e20 2020 2020 2020 2020  er.net>         
 00019ed0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00019ee0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00019ef0: 2020 2020 2020 2020 204f 4620 434f 4e54           OF CONT
-00019f00: 5241 4354 2c20 544f 5254 204f 5220 4f54  RACT, TORT OR OT
-00019f10: 4845 5257 4953 452c 2041 5249 5349 4e47  HERWISE, ARISING
-00019f20: 2046 524f 4d2c 204f 5554 204f 4620 4f52   FROM, OUT OF OR
-00019f30: 2049 4e20 434f 4e4e 4543 5449 4f4e 2020   IN CONNECTION  
-00019f40: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00019ef0: 2020 2020 2020 2020 2020 436f 7079 7269            Copyri
+00019f00: 6768 7420 2863 2920 3230 3132 2d32 3031  ght (c) 2012-201
+00019f10: 3420 2d20 546f 6d69 2050 6965 7669 6cc3  4 - Tomi Pievil.
+00019f20: a469 6e65 6e20 3c74 6f6d 692e 7069 6576  .inen <tomi.piev
+00019f30: 696c 6169 6e65 6e40 696b 692e 6669 3e20  ilainen@iki.fi> 
+00019f40: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00019f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f60: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00019f70: 2057 4954 4820 5448 4520 534f 4654 5741   WITH THE SOFTWA
-00019f80: 5245 204f 5220 5448 4520 5553 4520 4f52  RE OR THE USE OR
-00019f90: 204f 5448 4552 2044 4541 4c49 4e47 5320   OTHER DEALINGS 
-00019fa0: 494e 2054 4845 2053 4f46 5457 4152 452e  IN THE SOFTWARE.
-00019fb0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00019fc0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00019fd0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00019fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a030: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
-0001a040: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-0001a050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001a060: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001a070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001a080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001a090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001a0a0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020  ---------+.|    
-0001a0b0: 7069 702d 6c69 6365 6e73 6573 2020 2020  pip-licenses    
-0001a0c0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00019f60: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00019f70: 2020 2020 2043 6f70 7972 6967 6874 2028       Copyright (
+00019f80: 6329 2032 3031 342d 3230 3136 202d 2059  c) 2014-2016 - Y
+00019f90: 6172 6f6e 2064 6520 4c65 6575 7720 3c6d  aron de Leeuw <m
+00019fa0: 6540 6a61 726f 6e64 6c2e 6e65 743e 2020  e@jarondl.net>  
+00019fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019fc0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00019fd0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00019fe0: 2020 2020 2020 2020 2020 2043 6f70 7972             Copyr
+00019ff0: 6967 6874 2028 6329 2032 3031 352d 2020  ight (c) 2015-  
+0001a000: 2020 202d 2050 6175 6c20 4761 6e73 736c     - Paul Ganssl
+0001a010: 6520 3c70 6175 6c40 6761 6e73 736c 652e  e <paul@ganssle.
+0001a020: 696f 3e20 2020 2020 2020 2020 2020 2020  io>             
+0001a030: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001a040: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0001a050: 2020 2020 2020 2020 2020 2043 6f70 7972             Copyr
+0001a060: 6967 6874 2028 6329 2032 3031 352d 2020  ight (c) 2015-  
+0001a070: 2020 202d 2064 6174 6575 7469 6c20 636f     - dateutil co
+0001a080: 6e74 7269 6275 746f 7273 2028 7365 6520  ntributors (see 
+0001a090: 4155 5448 4f52 5320 6669 6c65 2920 2020  AUTHORS file)   
+0001a0a0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+0001a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a0c0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
 0001a0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a0e0: 2020 2020 2020 2020 2020 4d49 5420 4c69            MIT Li
-0001a0f0: 6365 6e73 6520 2020 2020 2020 2020 2020  cense           
+0001a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a110: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-0001a120: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001a130: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0001a110: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001a120: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0001a130: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 0001a140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a150: 2020 2020 2020 2020 2020 2020 416c 6c20              All 
+0001a160: 7269 6768 7473 2072 6573 6572 7665 642e  rights reserved.
 0001a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a190: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0001a1a0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+0001a190: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+0001a1a0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
 0001a1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a1c0: 2020 2020 2020 2020 2020 2020 2043 6f70               Cop
-0001a1d0: 7972 6967 6874 2028 6329 2032 3031 3820  yright (c) 2018 
-0001a1e0: 7261 696d 6f6e 2020 2020 2020 2020 2020  raimon          
+0001a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001a1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a200: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-0001a210: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0001a220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a270: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-0001a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a290: 2020 2020 7c20 2020 2020 2020 2020 5065      |         Pe
-0001a2a0: 726d 6973 7369 6f6e 2069 7320 6865 7265  rmission is here
-0001a2b0: 6279 2067 7261 6e74 6564 2c20 6672 6565  by granted, free
-0001a2c0: 206f 6620 6368 6172 6765 2c20 746f 2061   of charge, to a
-0001a2d0: 6e79 2070 6572 736f 6e20 6f62 7461 696e  ny person obtain
-0001a2e0: 696e 6720 6120 636f 7079 2020 2020 2020  ing a copy      
-0001a2f0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-0001a300: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001a310: 2020 6f66 2074 6869 7320 736f 6674 7761    of this softwa
-0001a320: 7265 2061 6e64 2061 7373 6f63 6961 7465  re and associate
-0001a330: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
-0001a340: 6669 6c65 7320 2874 6865 2022 536f 6674  files (the "Soft
-0001a350: 7761 7265 2229 2c20 746f 2064 6561 6c20  ware"), to deal 
-0001a360: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-0001a370: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0001a380: 2020 2020 2020 2020 696e 2074 6865 2053          in the S
-0001a390: 6f66 7477 6172 6520 7769 7468 6f75 7420  oftware without 
-0001a3a0: 7265 7374 7269 6374 696f 6e2c 2069 6e63  restriction, inc
-0001a3b0: 6c75 6469 6e67 2077 6974 686f 7574 206c  luding without l
-0001a3c0: 696d 6974 6174 696f 6e20 7468 6520 7269  imitation the ri
-0001a3d0: 6768 7473 2020 2020 2020 2020 7c0a 7c20  ghts        |.| 
+0001a200: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+0001a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a220: 7c20 2020 2020 2020 2020 2020 2020 2052  |              R
+0001a230: 6564 6973 7472 6962 7574 696f 6e20 616e  edistribution an
+0001a240: 6420 7573 6520 696e 2073 6f75 7263 6520  d use in source 
+0001a250: 616e 6420 6269 6e61 7279 2066 6f72 6d73  and binary forms
+0001a260: 2c20 7769 7468 206f 7220 7769 7468 6f75  , with or withou
+0001a270: 7420 2020 2020 2020 2020 2020 2020 7c0a  t             |.
+0001a280: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001a290: 2020 2020 207c 2020 2020 2020 2020 206d       |         m
+0001a2a0: 6f64 6966 6963 6174 696f 6e2c 2061 7265  odification, are
+0001a2b0: 2070 6572 6d69 7474 6564 2070 726f 7669   permitted provi
+0001a2c0: 6465 6420 7468 6174 2074 6865 2066 6f6c  ded that the fol
+0001a2d0: 6c6f 7769 6e67 2063 6f6e 6469 7469 6f6e  lowing condition
+0001a2e0: 7320 6172 6520 6d65 743a 2020 2020 2020  s are met:      
+0001a2f0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+0001a300: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+0001a310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a360: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001a370: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001a380: 2020 2020 2020 2020 2020 2020 202a 2052               * R
+0001a390: 6564 6973 7472 6962 7574 696f 6e73 206f  edistributions o
+0001a3a0: 6620 736f 7572 6365 2063 6f64 6520 6d75  f source code mu
+0001a3b0: 7374 2072 6574 6169 6e20 7468 6520 6162  st retain the ab
+0001a3c0: 6f76 6520 636f 7079 7269 6768 7420 6e6f  ove copyright no
+0001a3d0: 7469 6365 2c20 2020 2020 2020 207c 0a7c  tice,        |.|
 0001a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3f0: 2020 207c 2020 2020 2020 2020 2020 746f     |          to
-0001a400: 2075 7365 2c20 636f 7079 2c20 6d6f 6469   use, copy, modi
-0001a410: 6679 2c20 6d65 7267 652c 2070 7562 6c69  fy, merge, publi
-0001a420: 7368 2c20 6469 7374 7269 6275 7465 2c20  sh, distribute, 
-0001a430: 7375 626c 6963 656e 7365 2c20 616e 642f  sublicense, and/
-0001a440: 6f72 2073 656c 6c20 2020 2020 2020 2020  or sell         
-0001a450: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-0001a460: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001a470: 2020 2020 2063 6f70 6965 7320 6f66 2074       copies of t
-0001a480: 6865 2053 6f66 7477 6172 652c 2061 6e64  he Software, and
-0001a490: 2074 6f20 7065 726d 6974 2070 6572 736f   to permit perso
-0001a4a0: 6e73 2074 6f20 7768 6f6d 2074 6865 2053  ns to whom the S
-0001a4b0: 6f66 7477 6172 6520 6973 2020 2020 2020  oftware is      
-0001a4c0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001a4d0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-0001a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4f0: 2066 7572 6e69 7368 6564 2074 6f20 646f   furnished to do
-0001a500: 2073 6f2c 2073 7562 6a65 6374 2074 6f20   so, subject to 
-0001a510: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-0001a520: 6e64 6974 696f 6e73 3a20 2020 2020 2020  nditions:       
-0001a530: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001a3f0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001a400: 2020 2020 2020 2020 2020 2020 7468 6973              this
+0001a410: 206c 6973 7420 6f66 2063 6f6e 6469 7469   list of conditi
+0001a420: 6f6e 7320 616e 6420 7468 6520 666f 6c6c  ons and the foll
+0001a430: 6f77 696e 6720 6469 7363 6c61 696d 6572  owing disclaimer
+0001a440: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a450: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+0001a460: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001a470: 2020 2020 202a 2052 6564 6973 7472 6962       * Redistrib
+0001a480: 7574 696f 6e73 2069 6e20 6269 6e61 7279  utions in binary
+0001a490: 2066 6f72 6d20 6d75 7374 2072 6570 726f   form must repro
+0001a4a0: 6475 6365 2074 6865 2061 626f 7665 2063  duce the above c
+0001a4b0: 6f70 7972 6967 6874 206e 6f74 6963 652c  opyright notice,
+0001a4c0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0001a4d0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+0001a4e0: 2020 2020 2020 2020 2020 2020 7468 6973              this
+0001a4f0: 206c 6973 7420 6f66 2063 6f6e 6469 7469   list of conditi
+0001a500: 6f6e 7320 616e 6420 7468 6520 666f 6c6c  ons and the foll
+0001a510: 6f77 696e 6720 6469 7363 6c61 696d 6572  owing disclaimer
+0001a520: 2069 6e20 7468 6520 646f 6375 6d65 6e74   in the document
+0001a530: 6174 696f 6e20 2020 2020 2020 7c0a 7c20  ation       |.| 
 0001a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a550: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001a560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a5b0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-0001a5c0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001a5d0: 5468 6520 6162 6f76 6520 636f 7079 7269  The above copyri
-0001a5e0: 6768 7420 6e6f 7469 6365 2061 6e64 2074  ght notice and t
-0001a5f0: 6869 7320 7065 726d 6973 7369 6f6e 206e  his permission n
-0001a600: 6f74 6963 6520 7368 616c 6c20 6265 2069  otice shall be i
-0001a610: 6e63 6c75 6465 6420 696e 2061 6c6c 2020  ncluded in all  
-0001a620: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-0001a630: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a650: 2020 2020 636f 7069 6573 206f 7220 7375      copies or su
-0001a660: 6273 7461 6e74 6961 6c20 706f 7274 696f  bstantial portio
-0001a670: 6e73 206f 6620 7468 6520 536f 6674 7761  ns of the Softwa
-0001a680: 7265 2e20 2020 2020 2020 2020 2020 2020  re.             
-0001a690: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+0001a550: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001a560: 2020 2020 2020 2020 2020 2061 6e64 2f6f             and/o
+0001a570: 7220 6f74 6865 7220 6d61 7465 7269 616c  r other material
+0001a580: 7320 7072 6f76 6964 6564 2077 6974 6820  s provided with 
+0001a590: 7468 6520 6469 7374 7269 6275 7469 6f6e  the distribution
+0001a5a0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a5b0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0001a5c0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+0001a5d0: 2020 2020 2020 2020 2020 2a20 4e65 6974            * Neit
+0001a5e0: 6865 7220 7468 6520 6e61 6d65 206f 6620  her the name of 
+0001a5f0: 7468 6520 636f 7079 7269 6768 7420 686f  the copyright ho
+0001a600: 6c64 6572 206e 6f72 2074 6865 206e 616d  lder nor the nam
+0001a610: 6573 206f 6620 6974 7320 2020 2020 2020  es of its       
+0001a620: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+0001a630: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0001a640: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0001a650: 6e74 7269 6275 746f 7273 206d 6179 2062  ntributors may b
+0001a660: 6520 7573 6564 2074 6f20 656e 646f 7273  e used to endors
+0001a670: 6520 6f72 2070 726f 6d6f 7465 2070 726f  e or promote pro
+0001a680: 6475 6374 7320 6465 7269 7665 6420 6672  ducts derived fr
+0001a690: 6f6d 2020 2020 2020 2020 207c 0a7c 2020  om         |.|  
 0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6b0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-0001a6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a700: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0001a710: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-0001a720: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-0001a730: 2054 4845 2053 4f46 5457 4152 4520 4953   THE SOFTWARE IS
-0001a740: 2050 524f 5649 4445 4420 2241 5320 4953   PROVIDED "AS IS
-0001a750: 222c 2057 4954 484f 5554 2057 4152 5241  ", WITHOUT WARRA
-0001a760: 4e54 5920 4f46 2041 4e59 204b 494e 442c  NTY OF ANY KIND,
-0001a770: 2045 5850 5245 5353 204f 5220 2020 2020   EXPRESS OR     
-0001a780: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-0001a790: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-0001a7a0: 2020 2020 2020 2049 4d50 4c49 4544 2c20         IMPLIED, 
-0001a7b0: 494e 434c 5544 494e 4720 4255 5420 4e4f  INCLUDING BUT NO
-0001a7c0: 5420 4c49 4d49 5445 4420 544f 2054 4845  T LIMITED TO THE
-0001a7d0: 2057 4152 5241 4e54 4945 5320 4f46 204d   WARRANTIES OF M
-0001a7e0: 4552 4348 414e 5441 4249 4c49 5459 2c20  ERCHANTABILITY, 
-0001a7f0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+0001a6b0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+0001a6c0: 2020 2020 2020 2020 2074 6869 7320 736f           this so
+0001a6d0: 6674 7761 7265 2077 6974 686f 7574 2073  ftware without s
+0001a6e0: 7065 6369 6669 6320 7072 696f 7220 7772  pecific prior wr
+0001a6f0: 6974 7465 6e20 7065 726d 6973 7369 6f6e  itten permission
+0001a700: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a710: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0001a720: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+0001a730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a780: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001a790: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0001a7a0: 2020 2020 2020 2020 2020 5448 4953 2053            THIS S
+0001a7b0: 4f46 5457 4152 4520 4953 2050 524f 5649  OFTWARE IS PROVI
+0001a7c0: 4445 4420 4259 2054 4845 2043 4f50 5952  DED BY THE COPYR
+0001a7d0: 4947 4854 2048 4f4c 4445 5253 2041 4e44  IGHT HOLDERS AND
+0001a7e0: 2043 4f4e 5452 4942 5554 4f52 5320 2020   CONTRIBUTORS   
+0001a7f0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a810: 7c20 2020 2020 2020 2020 4649 544e 4553  |         FITNES
-0001a820: 5320 464f 5220 4120 5041 5254 4943 554c  S FOR A PARTICUL
-0001a830: 4152 2050 5552 504f 5345 2041 4e44 204e  AR PURPOSE AND N
-0001a840: 4f4e 494e 4652 494e 4745 4d45 4e54 2e20  ONINFRINGEMENT. 
-0001a850: 494e 204e 4f20 4556 454e 5420 5348 414c  IN NO EVENT SHAL
-0001a860: 4c20 5448 4520 2020 2020 2020 2020 7c0a  L THE         |.
-0001a870: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001a880: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0001a890: 2020 4155 5448 4f52 5320 4f52 2043 4f50    AUTHORS OR COP
-0001a8a0: 5952 4947 4854 2048 4f4c 4445 5253 2042  YRIGHT HOLDERS B
-0001a8b0: 4520 4c49 4142 4c45 2046 4f52 2041 4e59  E LIABLE FOR ANY
-0001a8c0: 2043 4c41 494d 2c20 4441 4d41 4745 5320   CLAIM, DAMAGES 
-0001a8d0: 4f52 204f 5448 4552 2020 2020 2020 2020  OR OTHER        
-0001a8e0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0001a8f0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001a900: 2020 204c 4941 4249 4c49 5459 2c20 5748     LIABILITY, WH
-0001a910: 4554 4845 5220 494e 2041 4e20 4143 5449  ETHER IN AN ACTI
-0001a920: 4f4e 204f 4620 434f 4e54 5241 4354 2c20  ON OF CONTRACT, 
-0001a930: 544f 5254 204f 5220 4f54 4845 5257 4953  TORT OR OTHERWIS
-0001a940: 452c 2041 5249 5349 4e47 2046 524f 4d2c  E, ARISING FROM,
-0001a950: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-0001a960: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0001a970: 2020 2020 2020 2020 4f55 5420 4f46 204f          OUT OF O
-0001a980: 5220 494e 2043 4f4e 4e45 4354 494f 4e20  R IN CONNECTION 
-0001a990: 5749 5448 2054 4845 2053 4f46 5457 4152  WITH THE SOFTWAR
-0001a9a0: 4520 4f52 2054 4845 2055 5345 204f 5220  E OR THE USE OR 
-0001a9b0: 4f54 4845 5220 4445 414c 494e 4753 2049  OTHER DEALINGS I
-0001a9c0: 4e20 5448 4520 2020 2020 2020 207c 0a7c  N THE        |.|
-0001a9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a9e0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-0001a9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa00: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-0001aa10: 4f46 5457 4152 452e 2020 2020 2020 2020  OFTWARE.        
-0001aa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa40: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-0001aa50: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001aa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aab0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
-0001aac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-0001aad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001aae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001aaf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001ab00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001ab10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001ab20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20  ------------+.| 
-0001ab30: 2020 2070 7265 7474 7974 6162 6c65 2020     prettytable  
-0001ab40: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-0001ab50: 2020 2020 2023 2043 6f70 7972 6967 6874       # Copyright
-0001ab60: 2028 6329 2032 3030 392d 3230 3134 204c   (c) 2009-2014 L
-0001ab70: 756b 6520 4d61 7572 6974 7320 3c6c 756b  uke Maurits <luk
-0001ab80: 6540 6d61 7572 6974 732e 6964 2e61 753e  e@maurits.id.au>
-0001ab90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aba0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-0001abb0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001abc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001abd0: 2020 2020 2020 2020 2020 2020 2023 2041               # A
-0001abe0: 6c6c 2072 6967 6874 7320 7265 7365 7276  ll rights reserv
-0001abf0: 6564 2e20 2020 2020 2020 2020 2020 2020  ed.             
-0001ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac10: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001ac20: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0001a810: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001a820: 2241 5320 4953 2220 414e 4420 414e 5920  "AS IS" AND ANY 
+0001a830: 4558 5052 4553 5320 4f52 2049 4d50 4c49  EXPRESS OR IMPLI
+0001a840: 4544 2057 4152 5241 4e54 4945 532c 2049  ED WARRANTIES, I
+0001a850: 4e43 4c55 4449 4e47 2c20 4255 5420 4e4f  NCLUDING, BUT NO
+0001a860: 5420 2020 2020 2020 2020 2020 2020 207c  T              |
+0001a870: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0001a880: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+0001a890: 2020 204c 494d 4954 4544 2054 4f2c 2054     LIMITED TO, T
+0001a8a0: 4845 2049 4d50 4c49 4544 2057 4152 5241  HE IMPLIED WARRA
+0001a8b0: 4e54 4945 5320 4f46 204d 4552 4348 414e  NTIES OF MERCHAN
+0001a8c0: 5441 4249 4c49 5459 2041 4e44 2046 4954  TABILITY AND FIT
+0001a8d0: 4e45 5353 2046 4f52 2020 2020 2020 2020  NESS FOR        
+0001a8e0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+0001a8f0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001a900: 2020 2020 4120 5041 5254 4943 554c 4152      A PARTICULAR
+0001a910: 2050 5552 504f 5345 2041 5245 2044 4953   PURPOSE ARE DIS
+0001a920: 434c 4149 4d45 442e 2049 4e20 4e4f 2045  CLAIMED. IN NO E
+0001a930: 5645 4e54 2053 4841 4c4c 2054 4845 2043  VENT SHALL THE C
+0001a940: 4f50 5952 4947 4854 204f 574e 4552 204f  OPYRIGHT OWNER O
+0001a950: 5220 2020 2020 2020 207c 0a7c 2020 2020  R        |.|    
+0001a960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a970: 7c20 2020 2020 2020 2020 2020 2043 4f4e  |            CON
+0001a980: 5452 4942 5554 4f52 5320 4245 204c 4941  TRIBUTORS BE LIA
+0001a990: 424c 4520 464f 5220 414e 5920 4449 5245  BLE FOR ANY DIRE
+0001a9a0: 4354 2c20 494e 4449 5245 4354 2c20 494e  CT, INDIRECT, IN
+0001a9b0: 4349 4445 4e54 414c 2c20 5350 4543 4941  CIDENTAL, SPECIA
+0001a9c0: 4c2c 2020 2020 2020 2020 2020 2020 7c0a  L,            |.
+0001a9d0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001a9e0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0001a9f0: 2020 2045 5845 4d50 4c41 5259 2c20 4f52     EXEMPLARY, OR
+0001aa00: 2043 4f4e 5345 5155 454e 5449 414c 2044   CONSEQUENTIAL D
+0001aa10: 414d 4147 4553 2028 494e 434c 5544 494e  AMAGES (INCLUDIN
+0001aa20: 472c 2042 5554 204e 4f54 204c 494d 4954  G, BUT NOT LIMIT
+0001aa30: 4544 2054 4f2c 2020 2020 2020 2020 2020  ED TO,          
+0001aa40: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+0001aa50: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+0001aa60: 2020 2020 2020 2020 2050 524f 4355 5245           PROCURE
+0001aa70: 4d45 4e54 204f 4620 5355 4253 5449 5455  MENT OF SUBSTITU
+0001aa80: 5445 2047 4f4f 4453 204f 5220 5345 5256  TE GOODS OR SERV
+0001aa90: 4943 4553 3b20 4c4f 5353 204f 4620 5553  ICES; LOSS OF US
+0001aaa0: 452c 2044 4154 412c 204f 5220 2020 2020  E, DATA, OR     
+0001aab0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001aac0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001aad0: 2020 2020 2020 2020 2020 2020 5052 4f46              PROF
+0001aae0: 4954 533b 204f 5220 4255 5349 4e45 5353  ITS; OR BUSINESS
+0001aaf0: 2049 4e54 4552 5255 5054 494f 4e29 2048   INTERRUPTION) H
+0001ab00: 4f57 4556 4552 2043 4155 5345 4420 414e  OWEVER CAUSED AN
+0001ab10: 4420 4f4e 2041 4e59 2054 4845 4f52 5920  D ON ANY THEORY 
+0001ab20: 4f46 2020 2020 2020 2020 2020 207c 0a7c  OF           |.|
+0001ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ab40: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001ab50: 2020 4c49 4142 494c 4954 592c 2057 4845    LIABILITY, WHE
+0001ab60: 5448 4552 2049 4e20 434f 4e54 5241 4354  THER IN CONTRACT
+0001ab70: 2c20 5354 5249 4354 204c 4941 4249 4c49  , STRICT LIABILI
+0001ab80: 5459 2c20 4f52 2054 4f52 5420 2849 4e43  TY, OR TORT (INC
+0001ab90: 4c55 4449 4e47 2020 2020 2020 2020 2020  LUDING          
+0001aba0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+0001abb0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001abc0: 2020 2020 2020 2020 4e45 474c 4947 454e          NEGLIGEN
+0001abd0: 4345 204f 5220 4f54 4845 5257 4953 4529  CE OR OTHERWISE)
+0001abe0: 2041 5249 5349 4e47 2049 4e20 414e 5920   ARISING IN ANY 
+0001abf0: 5741 5920 4f55 5420 4f46 2054 4845 2055  WAY OUT OF THE U
+0001ac00: 5345 204f 4620 5448 4953 2020 2020 2020  SE OF THIS      
+0001ac10: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0001ac20: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 0001ac30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac50: 2320 5769 7468 2063 6f6e 7472 6962 7574  # With contribut
-0001ac60: 696f 6e73 2066 726f 6d3a 2020 2020 2020  ions from:      
-0001ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ac80: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001ac40: 534f 4654 5741 5245 2c20 4556 454e 2049  SOFTWARE, EVEN I
+0001ac50: 4620 4144 5649 5345 4420 4f46 2054 4845  F ADVISED OF THE
+0001ac60: 2050 4f53 5349 4249 4c49 5459 204f 4620   POSSIBILITY OF 
+0001ac70: 5355 4348 2044 414d 4147 452e 2020 2020  SUCH DAMAGE.    
+0001ac80: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 0001ac90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aca0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+0001aca0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
 0001acb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001acc0: 2020 2020 2020 2020 2020 2320 202a 2043            #  * C
-0001acd0: 6872 6973 2043 6c61 726b 2020 2020 2020  hris Clark      
+0001acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001acd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ace0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001acf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad00: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-0001ad10: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001ad20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad30: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-0001ad40: 2a20 4b6c 6569 6e20 5374 6570 6861 6e65  * Klein Stephane
-0001ad50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ad70: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-0001ad80: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001ad90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ada0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001adb0: 2020 2023 2020 2a20 4a6f 686e 2046 696c     #  * John Fil
-0001adc0: 6c65 6175 2020 2020 2020 2020 2020 2020  leau            
-0001add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ade0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-0001adf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae00: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001ad00: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0001ad10: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+0001ad20: 5468 6520 6162 6f76 6520 4253 4420 4c69  The above BSD Li
+0001ad30: 6365 6e73 6520 4170 706c 6965 7320 746f  cense Applies to
+0001ad40: 2061 6c6c 2063 6f64 652c 2065 7665 6e20   all code, even 
+0001ad50: 7468 6174 2061 6c73 6f20 636f 7665 7265  that also covere
+0001ad60: 6420 6279 2041 7061 6368 6520 322e 302e  d by Apache 2.0.
+0001ad70: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
+0001ad80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+0001ad90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001ada0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001adb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001adc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001add0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001ade0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020  -----------+.|  
+0001adf0: 2020 2020 7265 7175 6573 7473 2020 2020      requests    
+0001ae00: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
 0001ae10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ae20: 2020 2020 2020 2023 2020 2a20 566c 6164         #  * Vlad
-0001ae30: 696d 6972 2056 727a 69c4 8720 2020 2020  imir Vrzi..     
+0001ae20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ae30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ae40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ae50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ae60: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 0001ae70: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 0001ae80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aea0: 2020 2020 2020 2320 2020 2020 2020 2020        #         
-0001aeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aeb0: 4170 6163 6865 204c 6963 656e 7365 2020  Apache License  
 0001aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001aed0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 0001aee0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001aef0: 2020 2020 2020 2020 2020 2320 5265 6469            # Redi
-0001af00: 7374 7269 6275 7469 6f6e 2061 6e64 2075  stribution and u
-0001af10: 7365 2069 6e20 736f 7572 6365 2061 6e64  se in source and
-0001af20: 2062 696e 6172 7920 666f 726d 732c 2077   binary forms, w
-0001af30: 6974 6820 6f72 2077 6974 686f 7574 2020  ith or without  
+0001aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af10: 2020 2020 2020 2020 2020 2020 2056 6572               Ver
+0001af20: 7369 6f6e 2032 2e30 2c20 4a61 6e75 6172  sion 2.0, Januar
+0001af30: 7920 3230 3034 2020 2020 2020 2020 2020  y 2004          
 0001af40: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001af50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001af60: 207c 2020 2020 2020 2020 2320 6d6f 6469   |        # modi
-0001af70: 6669 6361 7469 6f6e 2c20 6172 6520 7065  fication, are pe
-0001af80: 726d 6974 7465 6420 7072 6f76 6964 6564  rmitted provided
-0001af90: 2074 6861 7420 7468 6520 666f 6c6c 6f77   that the follow
-0001afa0: 696e 6720 636f 6e64 6974 696f 6e73 2061  ing conditions a
-0001afb0: 7265 206d 6574 3a20 2020 2020 2020 207c  re met:        |
+0001af60: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001af80: 2020 2020 2020 2020 2020 2020 2068 7474               htt
+0001af90: 703a 2f2f 7777 772e 6170 6163 6865 2e6f  p://www.apache.o
+0001afa0: 7267 2f6c 6963 656e 7365 732f 2020 2020  rg/licenses/    
+0001afb0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 0001afc0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 0001afd0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
 0001afe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001aff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b000: 2020 2020 2023 2020 2020 2020 2020 2020       #          
+0001b000: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b010: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b030: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 0001b040: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-0001b050: 2020 2020 2020 2320 2a20 5265 6469 7374        # * Redist
-0001b060: 7269 6275 7469 6f6e 7320 6f66 2073 6f75  ributions of sou
-0001b070: 7263 6520 636f 6465 206d 7573 7420 7265  rce code must re
-0001b080: 7461 696e 2074 6865 2061 626f 7665 2063  tain the above c
-0001b090: 6f70 7972 6967 6874 206e 6f74 6963 652c  opyright notice,
+0001b050: 2020 2020 2020 2020 2020 2020 2020 5445                TE
+0001b060: 524d 5320 414e 4420 434f 4e44 4954 494f  RMS AND CONDITIO
+0001b070: 4e53 2046 4f52 2055 5345 2c20 5245 5052  NS FOR USE, REPR
+0001b080: 4f44 5543 5449 4f4e 2c20 414e 4420 4449  ODUCTION, AND DI
+0001b090: 5354 5249 4255 5449 4f4e 2020 2020 2020  STRIBUTION      
 0001b0a0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001b0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b0c0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001b0d0: 2020 2023 2020 2074 6869 7320 6c69 7374     #   this list
-0001b0e0: 206f 6620 636f 6e64 6974 696f 6e73 2061   of conditions a
-0001b0f0: 6e64 2074 6865 2066 6f6c 6c6f 7769 6e67  nd the following
-0001b100: 2064 6973 636c 6169 6d65 722e 2020 2020   disclaimer.    
+0001b0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b110: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 0001b120: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001b130: 2020 2020 207c 2020 2020 2020 2020 2320       |        # 
-0001b140: 2a20 5265 6469 7374 7269 6275 7469 6f6e  * Redistribution
-0001b150: 7320 696e 2062 696e 6172 7920 666f 726d  s in binary form
-0001b160: 206d 7573 7420 7265 7072 6f64 7563 6520   must reproduce 
-0001b170: 7468 6520 6162 6f76 6520 636f 7079 7269  the above copyri
-0001b180: 6768 7420 6e6f 7469 6365 2c20 2020 2020  ght notice,     
+0001b130: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0001b140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b150: 2020 2020 2020 2020 2020 2020 2020 2031                 1
+0001b160: 2e20 4465 6669 6e69 7469 6f6e 732e 2020  . Definitions.  
+0001b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b190: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 0001b1a0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001b1b0: 2020 2023 2020 2074 6869 7320 6c69 7374     #   this list
-0001b1c0: 206f 6620 636f 6e64 6974 696f 6e73 2061   of conditions a
-0001b1d0: 6e64 2074 6865 2066 6f6c 6c6f 7769 6e67  nd the following
-0001b1e0: 2064 6973 636c 6169 6d65 7220 696e 2074   disclaimer in t
-0001b1f0: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+0001b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b200: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 0001b210: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 0001b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b230: 2020 2320 2020 616e 642f 6f72 206f 7468    #   and/or oth
-0001b240: 6572 206d 6174 6572 6961 6c73 2070 726f  er materials pro
-0001b250: 7669 6465 6420 7769 7468 2074 6865 2064  vided with the d
-0001b260: 6973 7472 6962 7574 696f 6e2e 2020 2020  istribution.    
-0001b270: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+0001b230: 224c 6963 656e 7365 2220 7368 616c 6c20  "License" shall 
+0001b240: 6d65 616e 2074 6865 2074 6572 6d73 2061  mean the terms a
+0001b250: 6e64 2063 6f6e 6469 7469 6f6e 7320 666f  nd conditions fo
+0001b260: 7220 7573 652c 2072 6570 726f 6475 6374  r use, reproduct
+0001b270: 696f 6e2c 2020 2020 2020 2020 207c 0a7c  ion,         |.|
 0001b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b290: 2020 2020 7c20 2020 2020 2020 2020 2023      |          #
-0001b2a0: 202a 2054 6865 206e 616d 6520 6f66 2074   * The name of t
-0001b2b0: 6865 2061 7574 686f 7220 6d61 7920 6e6f  he author may no
-0001b2c0: 7420 6265 2075 7365 6420 746f 2065 6e64  t be used to end
-0001b2d0: 6f72 7365 206f 7220 7072 6f6d 6f74 6520  orse or promote 
-0001b2e0: 7072 6f64 7563 7473 2020 2020 2020 2020  products        
+0001b290: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001b2a0: 2020 2020 616e 6420 6469 7374 7269 6275      and distribu
+0001b2b0: 7469 6f6e 2061 7320 6465 6669 6e65 6420  tion as defined 
+0001b2c0: 6279 2053 6563 7469 6f6e 7320 3120 7468  by Sections 1 th
+0001b2d0: 726f 7567 6820 3920 6f66 2074 6869 7320  rough 9 of this 
+0001b2e0: 646f 6375 6d65 6e74 2e20 2020 2020 2020  document.       
 0001b2f0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 0001b300: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001b310: 2020 2020 2320 2020 6465 7269 7665 6420      #   derived 
-0001b320: 6672 6f6d 2074 6869 7320 736f 6674 7761  from this softwa
-0001b330: 7265 2077 6974 686f 7574 2073 7065 6369  re without speci
-0001b340: 6669 6320 7072 696f 7220 7772 6974 7465  fic prior writte
-0001b350: 6e20 7065 726d 6973 7369 6f6e 2e20 2020  n permission.   
+0001b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b360: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 0001b370: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 0001b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3a0: 2020 2020 2020 2020 2020 2020 2023 2020               #  
-0001b3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3d0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+0001b390: 224c 6963 656e 736f 7222 2073 6861 6c6c  "Licensor" shall
+0001b3a0: 206d 6561 6e20 7468 6520 636f 7079 7269   mean the copyri
+0001b3b0: 6768 7420 6f77 6e65 7220 6f72 2065 6e74  ght owner or ent
+0001b3c0: 6974 7920 6175 7468 6f72 697a 6564 2062  ity authorized b
+0001b3d0: 7920 2020 2020 2020 2020 2020 7c0a 7c20  y           |.| 
 0001b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b3f0: 2020 207c 2020 2020 2020 2020 2320 5448     |        # TH
-0001b400: 4953 2053 4f46 5457 4152 4520 4953 2050  IS SOFTWARE IS P
-0001b410: 524f 5649 4445 4420 4259 2054 4845 2043  ROVIDED BY THE C
-0001b420: 4f50 5952 4947 4854 2048 4f4c 4445 5253  OPYRIGHT HOLDERS
-0001b430: 2041 4e44 2043 4f4e 5452 4942 5554 4f52   AND CONTRIBUTOR
-0001b440: 5320 2241 5320 4953 2220 2020 2020 2020  S "AS IS"       
+0001b3f0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001b400: 2020 2020 2020 2020 2020 2020 2074 6865               the
+0001b410: 2063 6f70 7972 6967 6874 206f 776e 6572   copyright owner
+0001b420: 2074 6861 7420 6973 2067 7261 6e74 696e   that is grantin
+0001b430: 6720 7468 6520 4c69 6365 6e73 652e 2020  g the License.  
+0001b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b450: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 0001b460: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001b470: 2020 2320 414e 4420 414e 5920 4558 5052    # AND ANY EXPR
-0001b480: 4553 5320 4f52 2049 4d50 4c49 4544 2057  ESS OR IMPLIED W
-0001b490: 4152 5241 4e54 4945 532c 2049 4e43 4c55  ARRANTIES, INCLU
-0001b4a0: 4449 4e47 2c20 4255 5420 4e4f 5420 4c49  DING, BUT NOT LI
-0001b4b0: 4d49 5445 4420 544f 2c20 5448 4520 2020  MITED TO, THE   
+0001b470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001b4c0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 0001b4d0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-0001b4e0: 2020 2020 2020 2023 2049 4d50 4c49 4544         # IMPLIED
-0001b4f0: 2057 4152 5241 4e54 4945 5320 4f46 204d   WARRANTIES OF M
-0001b500: 4552 4348 414e 5441 4249 4c49 5459 2041  ERCHANTABILITY A
-0001b510: 4e44 2046 4954 4e45 5353 2046 4f52 2041  ND FITNESS FOR A
-0001b520: 2050 4152 5449 4355 4c41 5220 5055 5250   PARTICULAR PURP
-0001b530: 4f53 4520 2020 2020 2020 207c 0a7c 2020  OSE        |.|  
+0001b4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b4f0: 224c 6567 616c 2045 6e74 6974 7922 2073  "Legal Entity" s
+0001b500: 6861 6c6c 206d 6561 6e20 7468 6520 756e  hall mean the un
+0001b510: 696f 6e20 6f66 2074 6865 2061 6374 696e  ion of the actin
+0001b520: 6720 656e 7469 7479 2061 6e64 2061 6c6c  g entity and all
+0001b530: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 0001b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b550: 2020 7c20 2020 2020 2020 2020 2023 2041    |          # A
-0001b560: 5245 2044 4953 434c 4149 4d45 442e 2049  RE DISCLAIMED. I
-0001b570: 4e20 4e4f 2045 5645 4e54 2053 4841 4c4c  N NO EVENT SHALL
-0001b580: 2054 4845 2043 4f50 5952 4947 4854 204f   THE COPYRIGHT O
-0001b590: 574e 4552 204f 5220 434f 4e54 5249 4255  WNER OR CONTRIBU
-0001b5a0: 544f 5253 2042 4520 2020 2020 2020 2020  TORS BE         
+0001b550: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+0001b560: 2020 206f 7468 6572 2065 6e74 6974 6965     other entitie
+0001b570: 7320 7468 6174 2063 6f6e 7472 6f6c 2c20  s that control, 
+0001b580: 6172 6520 636f 6e74 726f 6c6c 6564 2062  are controlled b
+0001b590: 792c 206f 7220 6172 6520 756e 6465 7220  y, or are under 
+0001b5a0: 636f 6d6d 6f6e 2020 2020 2020 2020 2020  common          
 0001b5b0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 0001b5c0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001b5d0: 2020 2020 2320 4c49 4142 4c45 2046 4f52      # LIABLE FOR
-0001b5e0: 2041 4e59 2044 4952 4543 542c 2049 4e44   ANY DIRECT, IND
-0001b5f0: 4952 4543 542c 2049 4e43 4944 454e 5441  IRECT, INCIDENTA
-0001b600: 4c2c 2053 5045 4349 414c 2c20 4558 454d  L, SPECIAL, EXEM
-0001b610: 504c 4152 592c 204f 5220 2020 2020 2020  PLARY, OR       
+0001b5d0: 2020 2020 2020 2020 2020 2063 6f6e 7472             contr
+0001b5e0: 6f6c 2077 6974 6820 7468 6174 2065 6e74  ol with that ent
+0001b5f0: 6974 792e 2046 6f72 2074 6865 2070 7572  ity. For the pur
+0001b600: 706f 7365 7320 6f66 2074 6869 7320 6465  poses of this de
+0001b610: 6669 6e69 7469 6f6e 2c20 2020 2020 2020  finition,       
 0001b620: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 0001b630: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001b640: 2020 2020 2020 2020 2023 2043 4f4e 5345           # CONSE
-0001b650: 5155 454e 5449 414c 2044 414d 4147 4553  QUENTIAL DAMAGES
-0001b660: 2028 494e 434c 5544 494e 472c 2042 5554   (INCLUDING, BUT
-0001b670: 204e 4f54 204c 494d 4954 4544 2054 4f2c   NOT LIMITED TO,
-0001b680: 2050 524f 4355 5245 4d45 4e54 204f 4620   PROCUREMENT OF 
+0001b640: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0001b650: 636f 6e74 726f 6c22 206d 6561 6e73 2028  control" means (
+0001b660: 6929 2074 6865 2070 6f77 6572 2c20 6469  i) the power, di
+0001b670: 7265 6374 206f 7220 696e 6469 7265 6374  rect or indirect
+0001b680: 2c20 746f 2063 6175 7365 2074 6865 2020  , to cause the  
 0001b690: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001b6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b6b0: 207c 2020 2020 2020 2020 2020 2320 5355   |          # SU
-0001b6c0: 4253 5449 5455 5445 2047 4f4f 4453 204f  BSTITUTE GOODS O
-0001b6d0: 5220 5345 5256 4943 4553 3b20 4c4f 5353  R SERVICES; LOSS
-0001b6e0: 204f 4620 5553 452c 2044 4154 412c 204f   OF USE, DATA, O
-0001b6f0: 5220 5052 4f46 4954 533b 204f 5220 4255  R PROFITS; OR BU
-0001b700: 5349 4e45 5353 2020 2020 2020 2020 207c  SINESS         |
+0001b6b0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001b6c0: 2020 2020 2064 6972 6563 7469 6f6e 206f       direction o
+0001b6d0: 7220 6d61 6e61 6765 6d65 6e74 206f 6620  r management of 
+0001b6e0: 7375 6368 2065 6e74 6974 792c 2077 6865  such entity, whe
+0001b6f0: 7468 6572 2062 7920 636f 6e74 7261 6374  ther by contract
+0001b700: 206f 7220 2020 2020 2020 2020 2020 207c   or            |
 0001b710: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 0001b720: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-0001b730: 2023 2049 4e54 4552 5255 5054 494f 4e29   # INTERRUPTION)
-0001b740: 2048 4f57 4556 4552 2043 4155 5345 4420   HOWEVER CAUSED 
-0001b750: 414e 4420 4f4e 2041 4e59 2054 4845 4f52  AND ON ANY THEOR
-0001b760: 5920 4f46 204c 4941 4249 4c49 5459 2c20  Y OF LIABILITY, 
-0001b770: 5748 4554 4845 5220 494e 2020 2020 2020  WHETHER IN      
+0001b730: 2020 2020 2020 2020 6f74 6865 7277 6973          otherwis
+0001b740: 652c 206f 7220 2869 6929 206f 776e 6572  e, or (ii) owner
+0001b750: 7368 6970 206f 6620 6669 6674 7920 7065  ship of fifty pe
+0001b760: 7263 656e 7420 2835 3025 2920 6f72 206d  rcent (50%) or m
+0001b770: 6f72 6520 6f66 2074 6865 2020 2020 2020  ore of the      
 0001b780: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 0001b790: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-0001b7a0: 2020 2020 2020 2320 434f 4e54 5241 4354        # CONTRACT
-0001b7b0: 2c20 5354 5249 4354 204c 4941 4249 4c49  , STRICT LIABILI
-0001b7c0: 5459 2c20 4f52 2054 4f52 5420 2849 4e43  TY, OR TORT (INC
-0001b7d0: 4c55 4449 4e47 204e 4547 4c49 4745 4e43  LUDING NEGLIGENC
-0001b7e0: 4520 4f52 204f 5448 4552 5749 5345 2920  E OR OTHERWISE) 
+0001b7a0: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0001b7b0: 7374 616e 6469 6e67 2073 6861 7265 732c  standing shares,
+0001b7c0: 206f 7220 2869 6969 2920 6265 6e65 6669   or (iii) benefi
+0001b7d0: 6369 616c 206f 776e 6572 7368 6970 206f  cial ownership o
+0001b7e0: 6620 7375 6368 2065 6e74 6974 792e 2020  f such entity.  
 0001b7f0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001b800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b810: 7c20 2020 2020 2020 2020 2320 4152 4953  |         # ARIS
-0001b820: 494e 4720 494e 2041 4e59 2057 4159 204f  ING IN ANY WAY O
-0001b830: 5554 204f 4620 5448 4520 5553 4520 4f46  UT OF THE USE OF
-0001b840: 2054 4849 5320 534f 4654 5741 5245 2c20   THIS SOFTWARE, 
-0001b850: 4556 454e 2049 4620 4144 5649 5345 4420  EVEN IF ADVISED 
-0001b860: 4f46 2054 4845 2020 2020 2020 2020 7c0a  OF THE        |.
+0001b810: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b860: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 0001b870: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 0001b880: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0001b890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b8a0: 2020 2020 2020 2320 504f 5353 4942 494c        # POSSIBIL
-0001b8b0: 4954 5920 4f46 2053 5543 4820 4441 4d41  ITY OF SUCH DAMA
-0001b8c0: 4745 2e20 2020 2020 2020 2020 2020 2020  GE.             
-0001b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b890: 2020 2020 2020 2020 2020 2022 596f 7522             "You"
+0001b8a0: 2028 6f72 2022 596f 7572 2229 2073 6861   (or "Your") sha
+0001b8b0: 6c6c 206d 6561 6e20 616e 2069 6e64 6976  ll mean an indiv
+0001b8c0: 6964 7561 6c20 6f72 204c 6567 616c 2045  idual or Legal E
+0001b8d0: 6e74 6974 7920 2020 2020 2020 2020 2020  ntity           
 0001b8e0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 0001b8f0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 0001b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b950: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
-0001b960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-0001b970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001b980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001b990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001b9a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001b9b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001b9c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
-0001b9d0: 2020 7079 7468 6f6e 2d64 6174 6575 7469    python-dateuti
-0001b9e0: 6c20 2020 7c20 2020 2020 2020 2020 2020  l   |           
-0001b9f0: 2020 2020 2020 2020 2020 2020 2043 6f70               Cop
-0001ba00: 7972 6967 6874 2032 3031 372d 2050 6175  yright 2017- Pau
-0001ba10: 6c20 4761 6e73 736c 6520 3c70 6175 6c40  l Ganssle <paul@
-0001ba20: 6761 6e73 736c 652e 696f 3e20 2020 2020  ganssle.io>     
-0001ba30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b910: 2020 2020 2065 7865 7263 6973 696e 6720       exercising 
+0001b920: 7065 726d 6973 7369 6f6e 7320 6772 616e  permissions gran
+0001b930: 7465 6420 6279 2074 6869 7320 4c69 6365  ted by this Lice
+0001b940: 6e73 652e 2020 2020 2020 2020 2020 2020  nse.            
+0001b950: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001b960: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001b970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9c0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+0001b9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b9e0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001b9f0: 2020 2020 2253 6f75 7263 6522 2066 6f72      "Source" for
+0001ba00: 6d20 7368 616c 6c20 6d65 616e 2074 6865  m shall mean the
+0001ba10: 2070 7265 6665 7272 6564 2066 6f72 6d20   preferred form 
+0001ba20: 666f 7220 6d61 6b69 6e67 206d 6f64 6966  for making modif
+0001ba30: 6963 6174 696f 6e73 2c20 2020 2020 2020  ications,       
 0001ba40: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 0001ba50: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001ba60: 2020 2020 2020 2020 2020 2020 2043 6f70               Cop
-0001ba70: 7972 6967 6874 2032 3031 372d 2064 6174  yright 2017- dat
-0001ba80: 6575 7469 6c20 636f 6e74 7269 6275 746f  eutil contributo
-0001ba90: 7273 2028 7365 6520 4155 5448 4f52 5320  rs (see AUTHORS 
-0001baa0: 6669 6c65 2920 2020 2020 2020 2020 2020  file)           
+0001ba60: 2020 2020 2020 2020 2020 2020 696e 636c              incl
+0001ba70: 7564 696e 6720 6275 7420 6e6f 7420 6c69  uding but not li
+0001ba80: 6d69 7465 6420 746f 2073 6f66 7477 6172  mited to softwar
+0001ba90: 6520 736f 7572 6365 2063 6f64 652c 2064  e source code, d
+0001baa0: 6f63 756d 656e 7461 7469 6f6e 2020 2020  ocumentation    
 0001bab0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 0001bac0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 0001bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001baf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001baf0: 2073 6f75 7263 652c 2061 6e64 2063 6f6e   source, and con
+0001bb00: 6669 6775 7261 7469 6f6e 2066 696c 6573  figuration files
+0001bb10: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
 0001bb20: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 0001bb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bb40: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-0001bb50: 2020 2020 204c 6963 656e 7365 6420 756e       Licensed un
-0001bb60: 6465 7220 7468 6520 4170 6163 6865 204c  der the Apache L
-0001bb70: 6963 656e 7365 2c20 5665 7273 696f 6e20  icense, Version 
-0001bb80: 322e 3020 2874 6865 2022 4c69 6365 6e73  2.0 (the "Licens
-0001bb90: 6522 293b 2020 2020 2020 2020 2020 2020  e");            
+0001bb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bba0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 0001bbb0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001bbc0: 2020 2020 2020 2020 2079 6f75 206d 6179           you may
-0001bbd0: 206e 6f74 2075 7365 2074 6869 7320 6669   not use this fi
-0001bbe0: 6c65 2065 7863 6570 7420 696e 2063 6f6d  le except in com
-0001bbf0: 706c 6961 6e63 6520 7769 7468 2074 6865  pliance with the
-0001bc00: 204c 6963 656e 7365 2e20 2020 2020 2020   License.       
+0001bbc0: 2020 2020 2020 2020 2020 2020 2022 4f62               "Ob
+0001bbd0: 6a65 6374 2220 666f 726d 2073 6861 6c6c  ject" form shall
+0001bbe0: 206d 6561 6e20 616e 7920 666f 726d 2072   mean any form r
+0001bbf0: 6573 756c 7469 6e67 2066 726f 6d20 6d65  esulting from me
+0001bc00: 6368 616e 6963 616c 2020 2020 2020 2020  chanical        
 0001bc10: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 0001bc20: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 0001bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bc40: 2020 2020 2020 2020 2020 2059 6f75 206d             You m
-0001bc50: 6179 206f 6274 6169 6e20 6120 636f 7079  ay obtain a copy
-0001bc60: 206f 6620 7468 6520 4c69 6365 6e73 6520   of the License 
-0001bc70: 6174 2020 2020 2020 2020 2020 2020 2020  at              
+0001bc40: 2074 7261 6e73 666f 726d 6174 696f 6e20   transformation 
+0001bc50: 6f72 2074 7261 6e73 6c61 7469 6f6e 206f  or translation o
+0001bc60: 6620 6120 536f 7572 6365 2066 6f72 6d2c  f a Source form,
+0001bc70: 2069 6e63 6c75 6469 6e67 2062 7574 2020   including but  
 0001bc80: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 0001bc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bca0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bcb0: 2020 2020 2020 6e6f 7420 6c69 6d69 7465        not limite
+0001bcc0: 6420 746f 2063 6f6d 7069 6c65 6420 6f62  d to compiled ob
+0001bcd0: 6a65 6374 2063 6f64 652c 2067 656e 6572  ject code, gener
+0001bce0: 6174 6564 2064 6f63 756d 656e 7461 7469  ated documentati
+0001bcf0: 6f6e 2c20 2020 2020 2020 2020 2020 2020  on,             
 0001bd00: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 0001bd10: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 0001bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bd30: 2020 2020 2068 7474 703a 2f2f 7777 772e       http://www.
-0001bd40: 6170 6163 6865 2e6f 7267 2f6c 6963 656e  apache.org/licen
-0001bd50: 7365 732f 4c49 4345 4e53 452d 322e 3020  ses/LICENSE-2.0 
+0001bd30: 2020 2020 2020 2061 6e64 2063 6f6e 7665         and conve
+0001bd40: 7273 696f 6e73 2074 6f20 6f74 6865 7220  rsions to other 
+0001bd50: 6d65 6469 6120 7479 7065 732e 2020 2020  media types.    
 0001bd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bd70: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 0001bd80: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 0001bd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bde0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001be00: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-0001be10: 2055 6e6c 6573 7320 7265 7175 6972 6564   Unless required
-0001be20: 2062 7920 6170 706c 6963 6162 6c65 206c   by applicable l
-0001be30: 6177 206f 7220 6167 7265 6564 2074 6f20  aw or agreed to 
-0001be40: 696e 2077 7269 7469 6e67 2c20 736f 6674  in writing, soft
-0001be50: 7761 7265 2020 2020 2020 2020 2020 207c  ware           |
+0001be10: 2020 2020 2022 576f 726b 2220 7368 616c       "Work" shal
+0001be20: 6c20 6d65 616e 2074 6865 2077 6f72 6b20  l mean the work 
+0001be30: 6f66 2061 7574 686f 7273 6869 702c 2077  of authorship, w
+0001be40: 6865 7468 6572 2069 6e20 536f 7572 6365  hether in Source
+0001be50: 206f 7220 2020 2020 2020 2020 2020 207c   or            |
 0001be60: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 0001be70: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-0001be80: 2020 2020 2020 2064 6973 7472 6962 7574         distribut
-0001be90: 6564 2075 6e64 6572 2074 6865 204c 6963  ed under the Lic
-0001bea0: 656e 7365 2069 7320 6469 7374 7269 6275  ense is distribu
-0001beb0: 7465 6420 6f6e 2061 6e20 2241 5320 4953  ted on an "AS IS
-0001bec0: 2220 4241 5349 532c 2020 2020 2020 2020  " BASIS,        
+0001be80: 2020 2020 2020 2020 204f 626a 6563 7420           Object 
+0001be90: 666f 726d 2c20 6d61 6465 2061 7661 696c  form, made avail
+0001bea0: 6162 6c65 2075 6e64 6572 2074 6865 204c  able under the L
+0001beb0: 6963 656e 7365 2c20 6173 2069 6e64 6963  icense, as indic
+0001bec0: 6174 6564 2062 7920 6120 2020 2020 2020  ated by a       
 0001bed0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 0001bee0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-0001bef0: 2020 2020 2020 2020 5749 5448 4f55 5420          WITHOUT 
-0001bf00: 5741 5252 414e 5449 4553 204f 5220 434f  WARRANTIES OR CO
-0001bf10: 4e44 4954 494f 4e53 204f 4620 414e 5920  NDITIONS OF ANY 
-0001bf20: 4b49 4e44 2c20 6569 7468 6572 2065 7870  KIND, either exp
-0001bf30: 7265 7373 206f 7220 696d 706c 6965 642e  ress or implied.
+0001bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001bf00: 636f 7079 7269 6768 7420 6e6f 7469 6365  copyright notice
+0001bf10: 2074 6861 7420 6973 2069 6e63 6c75 6465   that is include
+0001bf20: 6420 696e 206f 7220 6174 7461 6368 6564  d in or attached
+0001bf30: 2074 6f20 7468 6520 776f 726b 2020 2020   to the work    
 0001bf40: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001bf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001bf60: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001bf70: 5365 6520 7468 6520 4c69 6365 6e73 6520  See the License 
-0001bf80: 666f 7220 7468 6520 7370 6563 6966 6963  for the specific
-0001bf90: 206c 616e 6775 6167 6520 676f 7665 726e   language govern
-0001bfa0: 696e 6720 7065 726d 6973 7369 6f6e 7320  ing permissions 
-0001bfb0: 616e 6420 2020 2020 2020 2020 2020 7c0a  and           |.
+0001bf70: 2020 2020 2020 2020 2020 2028 616e 2065             (an e
+0001bf80: 7861 6d70 6c65 2069 7320 7072 6f76 6964  xample is provid
+0001bf90: 6564 2069 6e20 7468 6520 4170 7065 6e64  ed in the Append
+0001bfa0: 6978 2062 656c 6f77 292e 2020 2020 2020  ix below).      
+0001bfb0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 0001bfc0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 0001bfd0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 0001bfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001bff0: 2020 2020 2020 206c 696d 6974 6174 696f         limitatio
-0001c000: 6e73 2075 6e64 6572 2074 6865 204c 6963  ns under the Lic
-0001c010: 656e 7365 2e20 2020 2020 2020 2020 2020  ense.           
+0001bff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c010: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c030: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 0001c040: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c050: 2020 2020 2020 2020 2020 2022 4465 7269             "Deri
+0001c060: 7661 7469 7665 2057 6f72 6b73 2220 7368  vative Works" sh
+0001c070: 616c 6c20 6d65 616e 2061 6e79 2077 6f72  all mean any wor
+0001c080: 6b2c 2077 6865 7468 6572 2069 6e20 536f  k, whether in So
+0001c090: 7572 6365 206f 7220 4f62 6a65 6374 2020  urce or Object  
 0001c0a0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 0001c0b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0001c0c0: 2020 2020 2020 2020 2054 6865 2061 626f           The abo
-0001c0d0: 7665 206c 6963 656e 7365 2061 7070 6c69  ve license appli
-0001c0e0: 6573 2074 6f20 616c 6c20 636f 6e74 7269  es to all contri
-0001c0f0: 6275 7469 6f6e 7320 6166 7465 7220 3230  butions after 20
-0001c100: 3137 2d31 322d 3031 2c20 6173 2077 656c  17-12-01, as wel
-0001c110: 6c20 6173 2020 2020 2020 2020 207c 0a7c  l as         |.|
+0001c0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c0d0: 666f 726d 2c20 7468 6174 2069 7320 6261  form, that is ba
+0001c0e0: 7365 6420 6f6e 2028 6f72 2064 6572 6976  sed on (or deriv
+0001c0f0: 6564 2066 726f 6d29 2074 6865 2057 6f72  ed from) the Wor
+0001c100: 6b20 616e 6420 666f 7220 7768 6963 6820  k and for which 
+0001c110: 7468 6520 2020 2020 2020 2020 207c 0a7c  the          |.|
 0001c120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c130: 2020 2020 7c20 2020 2020 2020 2061 6c6c      |        all
-0001c140: 2063 6f6e 7472 6962 7574 696f 6e73 2074   contributions t
-0001c150: 6861 7420 6861 7665 2062 6565 6e20 7265  hat have been re
-0001c160: 2d6c 6963 656e 7365 6420 2873 6565 2041  -licensed (see A
-0001c170: 5554 484f 5253 2066 696c 6520 666f 7220  UTHORS file for 
-0001c180: 7468 6520 6c69 7374 206f 6620 2020 2020  the list of     
+0001c130: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001c140: 2020 2020 6564 6974 6f72 6961 6c20 7265      editorial re
+0001c150: 7669 7369 6f6e 732c 2061 6e6e 6f74 6174  visions, annotat
+0001c160: 696f 6e73 2c20 656c 6162 6f72 6174 696f  ions, elaboratio
+0001c170: 6e73 2c20 6f72 206f 7468 6572 206d 6f64  ns, or other mod
+0001c180: 6966 6963 6174 696f 6e73 2020 2020 2020  ifications      
 0001c190: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 0001c1a0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001c1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c1c0: 2020 636f 6e74 7269 6275 746f 7273 2077    contributors w
-0001c1d0: 686f 2068 6176 6520 7265 2d6c 6963 656e  ho have re-licen
-0001c1e0: 7365 6420 7468 6569 7220 636f 6465 292e  sed their code).
-0001c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c1b0: 2020 2020 2020 2020 7265 7072 6573 656e          represen
+0001c1c0: 742c 2061 7320 6120 7768 6f6c 652c 2061  t, as a whole, a
+0001c1d0: 6e20 6f72 6967 696e 616c 2077 6f72 6b20  n original work 
+0001c1e0: 6f66 2061 7574 686f 7273 6869 702e 2046  of authorship. F
+0001c1f0: 6f72 2074 6865 2070 7572 706f 7365 7320  or the purposes 
 0001c200: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 0001c210: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0001c220: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-0001c230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001c240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001c250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001c260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001c270: 2d2d 2d2d 2d2d 2020 2020 2020 7c0a 7c20  ------      |.| 
+0001c220: 2020 2020 2020 2020 2020 2020 2020 6f66                of
+0001c230: 2074 6869 7320 4c69 6365 6e73 652c 2044   this License, D
+0001c240: 6572 6976 6174 6976 6520 576f 726b 7320  erivative Works 
+0001c250: 7368 616c 6c20 6e6f 7420 696e 636c 7564  shall not includ
+0001c260: 6520 776f 726b 7320 7468 6174 2072 656d  e works that rem
+0001c270: 6169 6e20 2020 2020 2020 2020 7c0a 7c20  ain         |.| 
 0001c280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c290: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-0001c2a0: 2020 2020 6461 7465 7574 696c 202d 2045      dateutil - E
-0001c2b0: 7874 656e 7369 6f6e 7320 746f 2074 6865  xtensions to the
-0001c2c0: 2073 7461 6e64 6172 6420 5079 7468 6f6e   standard Python
-0001c2d0: 2064 6174 6574 696d 6520 6d6f 6475 6c65   datetime module
-0001c2e0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+0001c2a0: 2020 2073 6570 6172 6162 6c65 2066 726f     separable fro
+0001c2b0: 6d2c 206f 7220 6d65 7265 6c79 206c 696e  m, or merely lin
+0001c2c0: 6b20 286f 7220 6269 6e64 2062 7920 6e61  k (or bind by na
+0001c2d0: 6d65 2920 746f 2074 6865 2069 6e74 6572  me) to the inter
+0001c2e0: 6661 6365 7320 6f66 2c20 2020 2020 2020  faces of,       
 0001c2f0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 0001c300: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
 0001c310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c320: 2020 2020 2020 2020 7468 6520 576f 726b          the Work
+0001c330: 2061 6e64 2044 6572 6976 6174 6976 6520   and Derivative 
+0001c340: 576f 726b 7320 7468 6572 656f 662e 2020  Works thereof.  
 0001c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c360: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 0001c370: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-0001c380: 2020 2020 2020 2020 2020 2020 436f 7079              Copy
-0001c390: 7269 6768 7420 2863 2920 3230 3033 2d32  right (c) 2003-2
-0001c3a0: 3031 3120 2d20 4775 7374 6176 6f20 4e69  011 - Gustavo Ni
-0001c3b0: 656d 6579 6572 203c 6775 7374 6176 6f40  emeyer <gustavo@
-0001c3c0: 6e69 656d 6579 6572 2e6e 6574 3e20 2020  niemeyer.net>   
+0001c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c3d0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 0001c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001c3f0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001c400: 436f 7079 7269 6768 7420 2863 2920 3230  Copyright (c) 20
-0001c410: 3132 2d32 3031 3420 2d20 546f 6d69 2050  12-2014 - Tomi P
-0001c420: 6965 7669 6cc3 a469 6e65 6e20 3c74 6f6d  ievil..inen <tom
-0001c430: 692e 7069 6576 696c 6169 6e65 6e40 696b  i.pievilainen@ik
-0001c440: 692e 6669 3e20 2020 2020 2020 2020 2020  i.fi>           
-0001c450: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-0001c460: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001c470: 2020 2020 2020 2020 2020 2043 6f70 7972             Copyr
-0001c480: 6967 6874 2028 6329 2032 3031 342d 3230  ight (c) 2014-20
-0001c490: 3136 202d 2059 6172 6f6e 2064 6520 4c65  16 - Yaron de Le
-0001c4a0: 6575 7720 3c6d 6540 6a61 726f 6e64 6c2e  euw <me@jarondl.
-0001c4b0: 6e65 743e 2020 2020 2020 2020 2020 2020  net>            
-0001c4c0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001c4d0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-0001c4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c4f0: 2043 6f70 7972 6967 6874 2028 6329 2032   Copyright (c) 2
-0001c500: 3031 352d 2020 2020 202d 2050 6175 6c20  015-     - Paul 
-0001c510: 4761 6e73 736c 6520 3c70 6175 6c40 6761  Ganssle <paul@ga
-0001c520: 6e73 736c 652e 696f 3e20 2020 2020 2020  nssle.io>       
-0001c530: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001c400: 2020 2020 2020 2022 436f 6e74 7269 6275         "Contribu
+0001c410: 7469 6f6e 2220 7368 616c 6c20 6d65 616e  tion" shall mean
+0001c420: 2061 6e79 2077 6f72 6b20 6f66 2061 7574   any work of aut
+0001c430: 686f 7273 6869 702c 2069 6e63 6c75 6469  horship, includi
+0001c440: 6e67 2020 2020 2020 2020 2020 2020 2020  ng              
+0001c450: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0001c460: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+0001c470: 2020 2020 2020 2020 7468 6520 6f72 6967          the orig
+0001c480: 696e 616c 2076 6572 7369 6f6e 206f 6620  inal version of 
+0001c490: 7468 6520 576f 726b 2061 6e64 2061 6e79  the Work and any
+0001c4a0: 206d 6f64 6966 6963 6174 696f 6e73 206f   modifications o
+0001c4b0: 7220 6164 6469 7469 6f6e 7320 2020 2020  r additions     
+0001c4c0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001c4d0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0001c4e0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0001c4f0: 6f20 7468 6174 2057 6f72 6b20 6f72 2044  o that Work or D
+0001c500: 6572 6976 6174 6976 6520 576f 726b 7320  erivative Works 
+0001c510: 7468 6572 656f 662c 2074 6861 7420 6973  thereof, that is
+0001c520: 2069 6e74 656e 7469 6f6e 616c 6c79 2020   intentionally  
+0001c530: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c550: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001c560: 2043 6f70 7972 6967 6874 2028 6329 2032   Copyright (c) 2
-0001c570: 3031 352d 2020 2020 202d 2064 6174 6575  015-     - dateu
-0001c580: 7469 6c20 636f 6e74 7269 6275 746f 7273  til contributors
-0001c590: 2028 7365 6520 4155 5448 4f52 5320 6669   (see AUTHORS fi
-0001c5a0: 6c65 2920 2020 2020 2020 2020 2020 2020  le)             
-0001c5b0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-0001c5c0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c620: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-0001c630: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001c640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c660: 2020 416c 6c20 7269 6768 7473 2072 6573    All rights res
-0001c670: 6572 7665 642e 2020 2020 2020 2020 2020  erved.          
-0001c680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c690: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+0001c550: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001c560: 2073 7562 6d69 7474 6564 2074 6f20 4c69   submitted to Li
+0001c570: 6365 6e73 6f72 2066 6f72 2069 6e63 6c75  censor for inclu
+0001c580: 7369 6f6e 2069 6e20 7468 6520 576f 726b  sion in the Work
+0001c590: 2062 7920 7468 6520 636f 7079 7269 6768   by the copyrigh
+0001c5a0: 7420 6f77 6e65 7220 2020 2020 2020 207c  t owner        |
+0001c5b0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0001c5c0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+0001c5d0: 2020 2020 2020 6f72 2062 7920 616e 2069        or by an i
+0001c5e0: 6e64 6976 6964 7561 6c20 6f72 204c 6567  ndividual or Leg
+0001c5f0: 616c 2045 6e74 6974 7920 6175 7468 6f72  al Entity author
+0001c600: 697a 6564 2074 6f20 7375 626d 6974 206f  ized to submit o
+0001c610: 6e20 6265 6861 6c66 206f 6620 2020 2020  n behalf of     
+0001c620: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+0001c630: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001c640: 2020 2020 2020 2020 2020 2074 6865 2063             the c
+0001c650: 6f70 7972 6967 6874 206f 776e 6572 2e20  opyright owner. 
+0001c660: 466f 7220 7468 6520 7075 7270 6f73 6573  For the purposes
+0001c670: 206f 6620 7468 6973 2064 6566 696e 6974   of this definit
+0001c680: 696f 6e2c 2022 7375 626d 6974 7465 6422  ion, "submitted"
+0001c690: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001c6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6b0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-0001c6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c700: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0001c710: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-0001c720: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-0001c730: 2020 2020 2052 6564 6973 7472 6962 7574       Redistribut
-0001c740: 696f 6e20 616e 6420 7573 6520 696e 2073  ion and use in s
-0001c750: 6f75 7263 6520 616e 6420 6269 6e61 7279  ource and binary
-0001c760: 2066 6f72 6d73 2c20 7769 7468 206f 7220   forms, with or 
-0001c770: 7769 7468 6f75 7420 2020 2020 2020 2020  without         
-0001c780: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-0001c790: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-0001c7a0: 2020 2020 206d 6f64 6966 6963 6174 696f       modificatio
-0001c7b0: 6e2c 2061 7265 2070 6572 6d69 7474 6564  n, are permitted
-0001c7c0: 2070 726f 7669 6465 6420 7468 6174 2074   provided that t
-0001c7d0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
-0001c7e0: 6469 7469 6f6e 7320 6172 6520 6d65 743a  ditions are met:
-0001c7f0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0001c800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c810: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001c820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c860: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-0001c870: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001c880: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0001c890: 2020 202a 2052 6564 6973 7472 6962 7574     * Redistribut
-0001c8a0: 696f 6e73 206f 6620 736f 7572 6365 2063  ions of source c
-0001c8b0: 6f64 6520 6d75 7374 2072 6574 6169 6e20  ode must retain 
-0001c8c0: 7468 6520 6162 6f76 6520 636f 7079 7269  the above copyri
-0001c8d0: 6768 7420 6e6f 7469 6365 2c20 2020 2020  ght notice,     
-0001c8e0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0001c8f0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001c900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c910: 2020 7468 6973 206c 6973 7420 6f66 2063    this list of c
-0001c920: 6f6e 6469 7469 6f6e 7320 616e 6420 7468  onditions and th
-0001c930: 6520 666f 6c6c 6f77 696e 6720 6469 7363  e following disc
-0001c940: 6c61 696d 6572 2e20 2020 2020 2020 2020  laimer.         
-0001c950: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-0001c960: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0001c970: 2020 2020 2020 2020 2020 202a 2052 6564             * Red
-0001c980: 6973 7472 6962 7574 696f 6e73 2069 6e20  istributions in 
-0001c990: 6269 6e61 7279 2066 6f72 6d20 6d75 7374  binary form must
-0001c9a0: 2072 6570 726f 6475 6365 2074 6865 2061   reproduce the a
-0001c9b0: 626f 7665 2063 6f70 7972 6967 6874 206e  bove copyright n
-0001c9c0: 6f74 6963 652c 2020 2020 2020 207c 0a7c  otice,       |.|
+0001c6b0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001c6c0: 206d 6561 6e73 2061 6e79 2066 6f72 6d20   means any form 
+0001c6d0: 6f66 2065 6c65 6374 726f 6e69 632c 2076  of electronic, v
+0001c6e0: 6572 6261 6c2c 206f 7220 7772 6974 7465  erbal, or writte
+0001c6f0: 6e20 636f 6d6d 756e 6963 6174 696f 6e20  n communication 
+0001c700: 7365 6e74 2020 2020 2020 2020 2020 7c0a  sent          |.
+0001c710: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001c720: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0001c730: 2020 2020 2020 746f 2074 6865 204c 6963        to the Lic
+0001c740: 656e 736f 7220 6f72 2069 7473 2072 6570  ensor or its rep
+0001c750: 7265 7365 6e74 6174 6976 6573 2c20 696e  resentatives, in
+0001c760: 636c 7564 696e 6720 6275 7420 6e6f 7420  cluding but not 
+0001c770: 6c69 6d69 7465 6420 746f 2020 2020 2020  limited to      
+0001c780: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+0001c790: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+0001c7a0: 2020 2020 2020 2020 2063 6f6d 6d75 6e69           communi
+0001c7b0: 6361 7469 6f6e 206f 6e20 656c 6563 7472  cation on electr
+0001c7c0: 6f6e 6963 206d 6169 6c69 6e67 206c 6973  onic mailing lis
+0001c7d0: 7473 2c20 736f 7572 6365 2063 6f64 6520  ts, source code 
+0001c7e0: 636f 6e74 726f 6c20 7379 7374 656d 732c  control systems,
+0001c7f0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001c800: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001c810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c820: 616e 6420 6973 7375 6520 7472 6163 6b69  and issue tracki
+0001c830: 6e67 2073 7973 7465 6d73 2074 6861 7420  ng systems that 
+0001c840: 6172 6520 6d61 6e61 6765 6420 6279 2c20  are managed by, 
+0001c850: 6f72 206f 6e20 6265 6861 6c66 206f 662c  or on behalf of,
+0001c860: 2074 6865 2020 2020 2020 2020 207c 0a7c   the         |.|
+0001c870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c880: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001c890: 2020 2020 2020 4c69 6365 6e73 6f72 2066        Licensor f
+0001c8a0: 6f72 2074 6865 2070 7572 706f 7365 206f  or the purpose o
+0001c8b0: 6620 6469 7363 7573 7369 6e67 2061 6e64  f discussing and
+0001c8c0: 2069 6d70 726f 7669 6e67 2074 6865 2057   improving the W
+0001c8d0: 6f72 6b2c 2062 7574 2020 2020 2020 2020  ork, but        
+0001c8e0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+0001c8f0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001c900: 2020 2020 2020 2020 2020 2065 7863 6c75             exclu
+0001c910: 6469 6e67 2063 6f6d 6d75 6e69 6361 7469  ding communicati
+0001c920: 6f6e 2074 6861 7420 6973 2063 6f6e 7370  on that is consp
+0001c930: 6963 756f 7573 6c79 206d 6172 6b65 6420  icuously marked 
+0001c940: 6f72 206f 7468 6572 7769 7365 2020 2020  or otherwise    
+0001c950: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0001c960: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+0001c970: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0001c980: 7369 676e 6174 6564 2069 6e20 7772 6974  signated in writ
+0001c990: 696e 6720 6279 2074 6865 2063 6f70 7972  ing by the copyr
+0001c9a0: 6967 6874 206f 776e 6572 2061 7320 224e  ight owner as "N
+0001c9b0: 6f74 2061 2043 6f6e 7472 6962 7574 696f  ot a Contributio
+0001c9c0: 6e2e 2220 2020 2020 2020 2020 7c0a 7c20  n."         |.| 
 0001c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c9e0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-0001c9f0: 2020 7468 6973 206c 6973 7420 6f66 2063    this list of c
-0001ca00: 6f6e 6469 7469 6f6e 7320 616e 6420 7468  onditions and th
-0001ca10: 6520 666f 6c6c 6f77 696e 6720 6469 7363  e following disc
-0001ca20: 6c61 696d 6572 2069 6e20 7468 6520 646f  laimer in the do
-0001ca30: 6375 6d65 6e74 6174 696f 6e20 2020 2020  cumentation     
-0001ca40: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-0001ca50: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001ca60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ca70: 2061 6e64 2f6f 7220 6f74 6865 7220 6d61   and/or other ma
-0001ca80: 7465 7269 616c 7320 7072 6f76 6964 6564  terials provided
-0001ca90: 2077 6974 6820 7468 6520 6469 7374 7269   with the distri
-0001caa0: 6275 7469 6f6e 2e20 2020 2020 2020 2020  bution.         
-0001cab0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-0001cac0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0001cad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cae0: 2a20 4e65 6974 6865 7220 7468 6520 6e61  * Neither the na
-0001caf0: 6d65 206f 6620 7468 6520 636f 7079 7269  me of the copyri
-0001cb00: 6768 7420 686f 6c64 6572 206e 6f72 2074  ght holder nor t
-0001cb10: 6865 206e 616d 6573 206f 6620 6974 7320  he names of its 
-0001cb20: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+0001c9e0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001c9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ca40: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0001ca50: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+0001ca60: 2020 2020 2020 2020 2022 436f 6e74 7269           "Contri
+0001ca70: 6275 746f 7222 2073 6861 6c6c 206d 6561  butor" shall mea
+0001ca80: 6e20 4c69 6365 6e73 6f72 2061 6e64 2061  n Licensor and a
+0001ca90: 6e79 2069 6e64 6976 6964 7561 6c20 6f72  ny individual or
+0001caa0: 204c 6567 616c 2045 6e74 6974 7920 2020   Legal Entity   
+0001cab0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+0001cac0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0001cad0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0001cae0: 6e20 6265 6861 6c66 206f 6620 7768 6f6d  n behalf of whom
+0001caf0: 2061 2043 6f6e 7472 6962 7574 696f 6e20   a Contribution 
+0001cb00: 6861 7320 6265 656e 2072 6563 6569 7665  has been receive
+0001cb10: 6420 6279 204c 6963 656e 736f 7220 616e  d by Licensor an
+0001cb20: 6420 2020 2020 2020 2020 207c 0a7c 2020  d          |.|  
 0001cb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cb40: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-0001cb50: 2020 2020 636f 6e74 7269 6275 746f 7273      contributors
-0001cb60: 206d 6179 2062 6520 7573 6564 2074 6f20   may be used to 
-0001cb70: 656e 646f 7273 6520 6f72 2070 726f 6d6f  endorse or promo
-0001cb80: 7465 2070 726f 6475 6374 7320 6465 7269  te products deri
-0001cb90: 7665 6420 6672 6f6d 2020 2020 2020 2020  ved from        
-0001cba0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-0001cbb0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001cbc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001cbd0: 6869 7320 736f 6674 7761 7265 2077 6974  his software wit
-0001cbe0: 686f 7574 2073 7065 6369 6669 6320 7072  hout specific pr
-0001cbf0: 696f 7220 7772 6974 7465 6e20 7065 726d  ior written perm
-0001cc00: 6973 7369 6f6e 2e20 2020 2020 2020 2020  ission.         
-0001cc10: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001cc20: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-0001cc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cc80: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001cb40: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+0001cb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cb60: 7375 6273 6571 7565 6e74 6c79 2069 6e63  subsequently inc
+0001cb70: 6f72 706f 7261 7465 6420 7769 7468 696e  orporated within
+0001cb80: 2074 6865 2057 6f72 6b2e 2020 2020 2020   the Work.      
+0001cb90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cba0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0001cbb0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+0001cbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cbf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cc00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cc10: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001cc20: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0001cc30: 2020 2020 2020 2020 2020 2032 2e20 4772             2. Gr
+0001cc40: 616e 7420 6f66 2043 6f70 7972 6967 6874  ant of Copyright
+0001cc50: 204c 6963 656e 7365 2e20 5375 626a 6563   License. Subjec
+0001cc60: 7420 746f 2074 6865 2074 6572 6d73 2061  t to the terms a
+0001cc70: 6e64 2063 6f6e 6469 7469 6f6e 7320 6f66  nd conditions of
+0001cc80: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001cc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cca0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001ccb0: 5448 4953 2053 4f46 5457 4152 4520 4953  THIS SOFTWARE IS
-0001ccc0: 2050 524f 5649 4445 4420 4259 2054 4845   PROVIDED BY THE
-0001ccd0: 2043 4f50 5952 4947 4854 2048 4f4c 4445   COPYRIGHT HOLDE
-0001cce0: 5253 2041 4e44 2043 4f4e 5452 4942 5554  RS AND CONTRIBUT
-0001ccf0: 4f52 5320 2020 2020 2020 2020 2020 2020  ORS             
-0001cd00: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-0001cd10: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001cd20: 2020 2020 2020 2241 5320 4953 2220 414e        "AS IS" AN
-0001cd30: 4420 414e 5920 4558 5052 4553 5320 4f52  D ANY EXPRESS OR
-0001cd40: 2049 4d50 4c49 4544 2057 4152 5241 4e54   IMPLIED WARRANT
-0001cd50: 4945 532c 2049 4e43 4c55 4449 4e47 2c20  IES, INCLUDING, 
-0001cd60: 4255 5420 4e4f 5420 2020 2020 2020 2020  BUT NOT         
-0001cd70: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-0001cd80: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001cd90: 2020 2020 2020 2020 204c 494d 4954 4544           LIMITED
-0001cda0: 2054 4f2c 2054 4845 2049 4d50 4c49 4544   TO, THE IMPLIED
-0001cdb0: 2057 4152 5241 4e54 4945 5320 4f46 204d   WARRANTIES OF M
-0001cdc0: 4552 4348 414e 5441 4249 4c49 5459 2041  ERCHANTABILITY A
-0001cdd0: 4e44 2046 4954 4e45 5353 2046 4f52 2020  ND FITNESS FOR  
-0001cde0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+0001cca0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001ccb0: 2020 2020 7468 6973 204c 6963 656e 7365      this License
+0001ccc0: 2c20 6561 6368 2043 6f6e 7472 6962 7574  , each Contribut
+0001ccd0: 6f72 2068 6572 6562 7920 6772 616e 7473  or hereby grants
+0001cce0: 2074 6f20 596f 7520 6120 7065 7270 6574   to You a perpet
+0001ccf0: 7561 6c2c 2020 2020 2020 2020 2020 207c  ual,           |
+0001cd00: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0001cd10: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+0001cd20: 2020 2020 2020 2020 2020 776f 726c 6477            worldw
+0001cd30: 6964 652c 206e 6f6e 2d65 7863 6c75 7369  ide, non-exclusi
+0001cd40: 7665 2c20 6e6f 2d63 6861 7267 652c 2072  ve, no-charge, r
+0001cd50: 6f79 616c 7479 2d66 7265 652c 2069 7272  oyalty-free, irr
+0001cd60: 6576 6f63 6162 6c65 2020 2020 2020 2020  evocable        
+0001cd70: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+0001cd80: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001cd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cda0: 636f 7079 7269 6768 7420 6c69 6365 6e73  copyright licens
+0001cdb0: 6520 746f 2072 6570 726f 6475 6365 2c20  e to reproduce, 
+0001cdc0: 7072 6570 6172 6520 4465 7269 7661 7469  prepare Derivati
+0001cdd0: 7665 2057 6f72 6b73 206f 662c 2020 2020  ve Works of,    
+0001cde0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ce00: 207c 2020 2020 2020 2020 4120 5041 5254   |        A PART
-0001ce10: 4943 554c 4152 2050 5552 504f 5345 2041  ICULAR PURPOSE A
-0001ce20: 5245 2044 4953 434c 4149 4d45 442e 2049  RE DISCLAIMED. I
-0001ce30: 4e20 4e4f 2045 5645 4e54 2053 4841 4c4c  N NO EVENT SHALL
-0001ce40: 2054 4845 2043 4f50 5952 4947 4854 204f   THE COPYRIGHT O
-0001ce50: 574e 4552 204f 5220 2020 2020 2020 207c  WNER OR        |
-0001ce60: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-0001ce70: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-0001ce80: 2020 2043 4f4e 5452 4942 5554 4f52 5320     CONTRIBUTORS 
-0001ce90: 4245 204c 4941 424c 4520 464f 5220 414e  BE LIABLE FOR AN
-0001cea0: 5920 4449 5245 4354 2c20 494e 4449 5245  Y DIRECT, INDIRE
-0001ceb0: 4354 2c20 494e 4349 4445 4e54 414c 2c20  CT, INCIDENTAL, 
-0001cec0: 5350 4543 4941 4c2c 2020 2020 2020 2020  SPECIAL,        
-0001ced0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-0001cee0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-0001cef0: 2020 2020 2020 2020 2045 5845 4d50 4c41           EXEMPLA
-0001cf00: 5259 2c20 4f52 2043 4f4e 5345 5155 454e  RY, OR CONSEQUEN
-0001cf10: 5449 414c 2044 414d 4147 4553 2028 494e  TIAL DAMAGES (IN
-0001cf20: 434c 5544 494e 472c 2042 5554 204e 4f54  CLUDING, BUT NOT
-0001cf30: 204c 494d 4954 4544 2054 4f2c 2020 2020   LIMITED TO,    
-0001cf40: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0001cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001cf60: 7c20 2020 2020 2020 2020 2020 2020 2050  |              P
-0001cf70: 524f 4355 5245 4d45 4e54 204f 4620 5355  ROCUREMENT OF SU
-0001cf80: 4253 5449 5455 5445 2047 4f4f 4453 204f  BSTITUTE GOODS O
-0001cf90: 5220 5345 5256 4943 4553 3b20 4c4f 5353  R SERVICES; LOSS
-0001cfa0: 204f 4620 5553 452c 2044 4154 412c 204f   OF USE, DATA, O
-0001cfb0: 5220 2020 2020 2020 2020 2020 2020 7c0a  R             |.
-0001cfc0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001cfd0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0001cfe0: 2020 5052 4f46 4954 533b 204f 5220 4255    PROFITS; OR BU
-0001cff0: 5349 4e45 5353 2049 4e54 4552 5255 5054  SINESS INTERRUPT
-0001d000: 494f 4e29 2048 4f57 4556 4552 2043 4155  ION) HOWEVER CAU
-0001d010: 5345 4420 414e 4420 4f4e 2041 4e59 2054  SED AND ON ANY T
-0001d020: 4845 4f52 5920 4f46 2020 2020 2020 2020  HEORY OF        
-0001d030: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0001d040: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001d050: 2020 2020 2020 2020 4c49 4142 494c 4954          LIABILIT
-0001d060: 592c 2057 4845 5448 4552 2049 4e20 434f  Y, WHETHER IN CO
-0001d070: 4e54 5241 4354 2c20 5354 5249 4354 204c  NTRACT, STRICT L
-0001d080: 4941 4249 4c49 5459 2c20 4f52 2054 4f52  IABILITY, OR TOR
-0001d090: 5420 2849 4e43 4c55 4449 4e47 2020 2020  T (INCLUDING    
-0001d0a0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-0001d0b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0001d0c0: 2020 2020 2020 2020 2020 2020 2020 4e45                NE
-0001d0d0: 474c 4947 454e 4345 204f 5220 4f54 4845  GLIGENCE OR OTHE
-0001d0e0: 5257 4953 4529 2041 5249 5349 4e47 2049  RWISE) ARISING I
-0001d0f0: 4e20 414e 5920 5741 5920 4f55 5420 4f46  N ANY WAY OUT OF
-0001d100: 2054 4845 2055 5345 204f 4620 5448 4953   THE USE OF THIS
-0001d110: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+0001ce00: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001ce10: 2020 7075 626c 6963 6c79 2064 6973 706c    publicly displ
+0001ce20: 6179 2c20 7075 626c 6963 6c79 2070 6572  ay, publicly per
+0001ce30: 666f 726d 2c20 7375 626c 6963 656e 7365  form, sublicense
+0001ce40: 2c20 616e 6420 6469 7374 7269 6275 7465  , and distribute
+0001ce50: 2074 6865 2020 2020 2020 2020 2020 7c0a   the          |.
+0001ce60: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001ce70: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0001ce80: 2020 2020 2020 2020 2020 2020 576f 726b              Work
+0001ce90: 2061 6e64 2073 7563 6820 4465 7269 7661   and such Deriva
+0001cea0: 7469 7665 2057 6f72 6b73 2069 6e20 536f  tive Works in So
+0001ceb0: 7572 6365 206f 7220 4f62 6a65 6374 2066  urce or Object f
+0001cec0: 6f72 6d2e 2020 2020 2020 2020 2020 2020  orm.            
+0001ced0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+0001cee0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+0001cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cf40: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001cf50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001cf60: 2020 2020 2020 2020 2020 2020 2020 2033                 3
+0001cf70: 2e20 4772 616e 7420 6f66 2050 6174 656e  . Grant of Paten
+0001cf80: 7420 4c69 6365 6e73 652e 2053 7562 6a65  t License. Subje
+0001cf90: 6374 2074 6f20 7468 6520 7465 726d 7320  ct to the terms 
+0001cfa0: 616e 6420 636f 6e64 6974 696f 6e73 206f  and conditions o
+0001cfb0: 6620 2020 2020 2020 2020 2020 207c 0a7c  f            |.|
+0001cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001cfd0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001cfe0: 2020 2020 2020 2074 6869 7320 4c69 6365         this Lice
+0001cff0: 6e73 652c 2065 6163 6820 436f 6e74 7269  nse, each Contri
+0001d000: 6275 746f 7220 6865 7265 6279 2067 7261  butor hereby gra
+0001d010: 6e74 7320 746f 2059 6f75 2061 2070 6572  nts to You a per
+0001d020: 7065 7475 616c 2c20 2020 2020 2020 2020  petual,         
+0001d030: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+0001d040: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001d050: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
+0001d060: 6c64 7769 6465 2c20 6e6f 6e2d 6578 636c  ldwide, non-excl
+0001d070: 7573 6976 652c 206e 6f2d 6368 6172 6765  usive, no-charge
+0001d080: 2c20 726f 7961 6c74 792d 6672 6565 2c20  , royalty-free, 
+0001d090: 6972 7265 766f 6361 626c 6520 2020 2020  irrevocable     
+0001d0a0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0001d0b0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+0001d0c0: 2020 2020 2020 2020 2020 2020 2020 2865                (e
+0001d0d0: 7863 6570 7420 6173 2073 7461 7465 6420  xcept as stated 
+0001d0e0: 696e 2074 6869 7320 7365 6374 696f 6e29  in this section)
+0001d0f0: 2070 6174 656e 7420 6c69 6365 6e73 6520   patent license 
+0001d100: 746f 206d 616b 652c 2068 6176 6520 6d61  to make, have ma
+0001d110: 6465 2c20 2020 2020 2020 2020 7c0a 7c20  de,         |.| 
 0001d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d130: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-0001d140: 2020 2020 2020 534f 4654 5741 5245 2c20        SOFTWARE, 
-0001d150: 4556 454e 2049 4620 4144 5649 5345 4420  EVEN IF ADVISED 
-0001d160: 4f46 2054 4845 2050 4f53 5349 4249 4c49  OF THE POSSIBILI
-0001d170: 5459 204f 4620 5355 4348 2044 414d 4147  TY OF SUCH DAMAG
-0001d180: 452e 2020 2020 2020 2020 2020 2020 2020  E.              
-0001d190: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-0001d1a0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001d1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d200: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-0001d210: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0001d220: 2020 2020 2020 5468 6520 6162 6f76 6520        The above 
-0001d230: 4253 4420 4c69 6365 6e73 6520 4170 706c  BSD License Appl
-0001d240: 6965 7320 746f 2061 6c6c 2063 6f64 652c  ies to all code,
-0001d250: 2065 7665 6e20 7468 6174 2061 6c73 6f20   even that also 
-0001d260: 636f 7665 7265 6420 6279 2041 7061 6368  covered by Apach
-0001d270: 6520 322e 302e 2020 2020 2020 7c0a 2b2d  e 2.0.      |.+-
-0001d280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001d290: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-0001d2a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001d2b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001d2c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001d2d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001d2e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0001d2f0: 2d2b 0a7c 2020 2020 2020 7265 7175 6573  -+.|      reques
-0001d300: 7473 2020 2020 2020 7c20 2020 2020 2020  ts      |       
-0001d310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d360: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001d370: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0001d130: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001d140: 2020 2020 2075 7365 2c20 6f66 6665 7220       use, offer 
+0001d150: 746f 2073 656c 6c2c 2073 656c 6c2c 2069  to sell, sell, i
+0001d160: 6d70 6f72 742c 2061 6e64 206f 7468 6572  mport, and other
+0001d170: 7769 7365 2074 7261 6e73 6665 7220 7468  wise transfer th
+0001d180: 6520 576f 726b 2c20 2020 2020 2020 2020  e Work,         
+0001d190: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0001d1a0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+0001d1b0: 2020 2020 2020 2020 2020 7768 6572 6520            where 
+0001d1c0: 7375 6368 206c 6963 656e 7365 2061 7070  such license app
+0001d1d0: 6c69 6573 206f 6e6c 7920 746f 2074 686f  lies only to tho
+0001d1e0: 7365 2070 6174 656e 7420 636c 6169 6d73  se patent claims
+0001d1f0: 206c 6963 656e 7361 626c 6520 2020 2020   licensable     
+0001d200: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+0001d210: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0001d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d230: 2020 6279 2073 7563 6820 436f 6e74 7269    by such Contri
+0001d240: 6275 746f 7220 7468 6174 2061 7265 206e  butor that are n
+0001d250: 6563 6573 7361 7269 6c79 2069 6e66 7269  ecessarily infri
+0001d260: 6e67 6564 2062 7920 7468 6569 7220 2020  nged by their   
+0001d270: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d290: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+0001d2a0: 2020 2020 2043 6f6e 7472 6962 7574 696f       Contributio
+0001d2b0: 6e28 7329 2061 6c6f 6e65 206f 7220 6279  n(s) alone or by
+0001d2c0: 2063 6f6d 6269 6e61 7469 6f6e 206f 6620   combination of 
+0001d2d0: 7468 6569 7220 436f 6e74 7269 6275 7469  their Contributi
+0001d2e0: 6f6e 2873 2920 2020 2020 2020 2020 2020  on(s)           
+0001d2f0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0001d300: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+0001d310: 2020 2020 2020 2020 2077 6974 6820 7468           with th
+0001d320: 6520 576f 726b 2074 6f20 7768 6963 6820  e Work to which 
+0001d330: 7375 6368 2043 6f6e 7472 6962 7574 696f  such Contributio
+0001d340: 6e28 7329 2077 6173 2073 7562 6d69 7474  n(s) was submitt
+0001d350: 6564 2e20 4966 2059 6f75 2020 2020 2020  ed. If You      
+0001d360: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001d370: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 0001d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3b0: 2020 2020 2020 4170 6163 6865 204c 6963        Apache Lic
-0001d3c0: 656e 7365 2020 2020 2020 2020 2020 2020  ense            
-0001d3d0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001d390: 2069 6e73 7469 7475 7465 2070 6174 656e   institute paten
+0001d3a0: 7420 6c69 7469 6761 7469 6f6e 2061 6761  t litigation aga
+0001d3b0: 696e 7374 2061 6e79 2065 6e74 6974 7920  inst any entity 
+0001d3c0: 2869 6e63 6c75 6469 6e67 2061 2020 2020  (including a    
+0001d3d0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001d3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3f0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001d400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d420: 2020 2056 6572 7369 6f6e 2032 2e30 2c20     Version 2.0, 
-0001d430: 4a61 6e75 6172 7920 3230 3034 2020 2020  January 2004    
-0001d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d450: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-0001d460: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d490: 2020 2068 7474 703a 2f2f 7777 772e 6170     http://www.ap
-0001d4a0: 6163 6865 2e6f 7267 2f6c 6963 656e 7365  ache.org/license
-0001d4b0: 732f 2020 2020 2020 2020 2020 2020 2020  s/              
-0001d4c0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-0001d4d0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001d4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d530: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+0001d3f0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001d400: 2020 2020 6372 6f73 732d 636c 6169 6d20      cross-claim 
+0001d410: 6f72 2063 6f75 6e74 6572 636c 6169 6d20  or counterclaim 
+0001d420: 696e 2061 206c 6177 7375 6974 2920 616c  in a lawsuit) al
+0001d430: 6c65 6769 6e67 2074 6861 7420 7468 6520  leging that the 
+0001d440: 576f 726b 2020 2020 2020 2020 2020 207c  Work           |
+0001d450: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0001d460: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+0001d470: 2020 2020 2020 2020 6f72 2061 2043 6f6e          or a Con
+0001d480: 7472 6962 7574 696f 6e20 696e 636f 7270  tribution incorp
+0001d490: 6f72 6174 6564 2077 6974 6869 6e20 7468  orated within th
+0001d4a0: 6520 576f 726b 2063 6f6e 7374 6974 7574  e Work constitut
+0001d4b0: 6573 2064 6972 6563 7420 2020 2020 2020  es direct       
+0001d4c0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+0001d4d0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001d4e0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0001d4f0: 7220 636f 6e74 7269 6275 746f 7279 2070  r contributory p
+0001d500: 6174 656e 7420 696e 6672 696e 6765 6d65  atent infringeme
+0001d510: 6e74 2c20 7468 656e 2061 6e79 2070 6174  nt, then any pat
+0001d520: 656e 7420 6c69 6365 6e73 6573 2020 2020  ent licenses    
+0001d530: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001d540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d550: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-0001d560: 2020 2020 5445 524d 5320 414e 4420 434f      TERMS AND CO
-0001d570: 4e44 4954 494f 4e53 2046 4f52 2055 5345  NDITIONS FOR USE
-0001d580: 2c20 5245 5052 4f44 5543 5449 4f4e 2c20  , REPRODUCTION, 
-0001d590: 414e 4420 4449 5354 5249 4255 5449 4f4e  AND DISTRIBUTION
-0001d5a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0001d5b0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-0001d5c0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+0001d550: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001d560: 2020 2067 7261 6e74 6564 2074 6f20 596f     granted to Yo
+0001d570: 7520 756e 6465 7220 7468 6973 204c 6963  u under this Lic
+0001d580: 656e 7365 2066 6f72 2074 6861 7420 576f  ense for that Wo
+0001d590: 726b 2073 6861 6c6c 2074 6572 6d69 6e61  rk shall termina
+0001d5a0: 7465 2020 2020 2020 2020 2020 2020 7c0a  te            |.
+0001d5b0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001d5c0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 0001d5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5e0: 2020 2020 6173 206f 6620 7468 6520 6461      as of the da
+0001d5f0: 7465 2073 7563 6820 6c69 7469 6761 7469  te such litigati
+0001d600: 6f6e 2069 7320 6669 6c65 642e 2020 2020  on is filed.    
 0001d610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d620: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-0001d630: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001d620: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+0001d630: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 0001d640: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d660: 2020 2020 2031 2e20 4465 6669 6e69 7469       1. Definiti
-0001d670: 6f6e 732e 2020 2020 2020 2020 2020 2020  ons.            
+0001d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d690: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0001d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6b0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d700: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-0001d710: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001d720: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0001d730: 2020 2020 2020 224c 6963 656e 7365 2220        "License" 
-0001d740: 7368 616c 6c20 6d65 616e 2074 6865 2074  shall mean the t
-0001d750: 6572 6d73 2061 6e64 2063 6f6e 6469 7469  erms and conditi
-0001d760: 6f6e 7320 666f 7220 7573 652c 2072 6570  ons for use, rep
-0001d770: 726f 6475 6374 696f 6e2c 2020 2020 2020  roduction,      
-0001d780: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0001d790: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001d7a0: 2020 2020 2020 2020 2020 616e 6420 6469            and di
-0001d7b0: 7374 7269 6275 7469 6f6e 2061 7320 6465  stribution as de
-0001d7c0: 6669 6e65 6420 6279 2053 6563 7469 6f6e  fined by Section
-0001d7d0: 7320 3120 7468 726f 7567 6820 3920 6f66  s 1 through 9 of
-0001d7e0: 2074 6869 7320 646f 6375 6d65 6e74 2e20   this document. 
-0001d7f0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-0001d800: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001d690: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001d6a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d6c0: 342e 2052 6564 6973 7472 6962 7574 696f  4. Redistributio
+0001d6d0: 6e2e 2059 6f75 206d 6179 2072 6570 726f  n. You may repro
+0001d6e0: 6475 6365 2061 6e64 2064 6973 7472 6962  duce and distrib
+0001d6f0: 7574 6520 636f 7069 6573 206f 6620 7468  ute copies of th
+0001d700: 6520 2020 2020 2020 2020 2020 207c 0a7c  e            |.|
+0001d710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d720: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001d730: 2020 2020 2020 2057 6f72 6b20 6f72 2044         Work or D
+0001d740: 6572 6976 6174 6976 6520 576f 726b 7320  erivative Works 
+0001d750: 7468 6572 656f 6620 696e 2061 6e79 206d  thereof in any m
+0001d760: 6564 6975 6d2c 2077 6974 6820 6f72 2077  edium, with or w
+0001d770: 6974 686f 7574 2020 2020 2020 2020 2020  ithout          
+0001d780: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+0001d790: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001d7a0: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
+0001d7b0: 6966 6963 6174 696f 6e73 2c20 616e 6420  ifications, and 
+0001d7c0: 696e 2053 6f75 7263 6520 6f72 204f 626a  in Source or Obj
+0001d7d0: 6563 7420 666f 726d 2c20 7072 6f76 6964  ect form, provid
+0001d7e0: 6564 2074 6861 7420 596f 7520 2020 2020  ed that You     
+0001d7f0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0001d800: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 0001d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001d820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d830: 2020 6d65 6574 2074 6865 2066 6f6c 6c6f    meet the follo
+0001d840: 7769 6e67 2063 6f6e 6469 7469 6f6e 733a  wing conditions:
 0001d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d860: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+0001d860: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 0001d870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d880: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-0001d890: 2020 2020 2020 224c 6963 656e 736f 7222        "Licensor"
-0001d8a0: 2073 6861 6c6c 206d 6561 6e20 7468 6520   shall mean the 
-0001d8b0: 636f 7079 7269 6768 7420 6f77 6e65 7220  copyright owner 
-0001d8c0: 6f72 2065 6e74 6974 7920 6175 7468 6f72  or entity author
-0001d8d0: 697a 6564 2062 7920 2020 2020 2020 2020  ized by         
-0001d8e0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-0001d8f0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001d880: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8e0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0001d8f0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
 0001d900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d910: 2020 2074 6865 2063 6f70 7972 6967 6874     the copyright
-0001d920: 206f 776e 6572 2074 6861 7420 6973 2067   owner that is g
-0001d930: 7261 6e74 696e 6720 7468 6520 4c69 6365  ranting the Lice
-0001d940: 6e73 652e 2020 2020 2020 2020 2020 2020  nse.            
-0001d950: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-0001d960: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+0001d910: 2861 2920 596f 7520 6d75 7374 2067 6976  (a) You must giv
+0001d920: 6520 616e 7920 6f74 6865 7220 7265 6369  e any other reci
+0001d930: 7069 656e 7473 206f 6620 7468 6520 576f  pients of the Wo
+0001d940: 726b 206f 7220 2020 2020 2020 2020 2020  rk or           
+0001d950: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+0001d960: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 0001d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d9c0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+0001d980: 2020 2020 2020 2020 2020 2020 4465 7269              Deri
+0001d990: 7661 7469 7665 2057 6f72 6b73 2061 2063  vative Works a c
+0001d9a0: 6f70 7920 6f66 2074 6869 7320 4c69 6365  opy of this Lice
+0001d9b0: 6e73 653b 2061 6e64 2020 2020 2020 2020  nse; and        
+0001d9c0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 0001d9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d9e0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-0001d9f0: 2020 2020 2020 224c 6567 616c 2045 6e74        "Legal Ent
-0001da00: 6974 7922 2073 6861 6c6c 206d 6561 6e20  ity" shall mean 
-0001da10: 7468 6520 756e 696f 6e20 6f66 2074 6865  the union of the
-0001da20: 2061 6374 696e 6720 656e 7469 7479 2061   acting entity a
-0001da30: 6e64 2061 6c6c 2020 2020 2020 2020 2020  nd all          
-0001da40: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-0001da50: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001da60: 2020 2020 2020 2020 206f 7468 6572 2065           other e
-0001da70: 6e74 6974 6965 7320 7468 6174 2063 6f6e  ntities that con
-0001da80: 7472 6f6c 2c20 6172 6520 636f 6e74 726f  trol, are contro
-0001da90: 6c6c 6564 2062 792c 206f 7220 6172 6520  lled by, or are 
-0001daa0: 756e 6465 7220 636f 6d6d 6f6e 2020 2020  under common    
-0001dab0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001dac0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0001d9e0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+0001d9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da40: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0001da50: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+0001da60: 2020 2020 2020 2020 2020 2862 2920 596f            (b) Yo
+0001da70: 7520 6d75 7374 2063 6175 7365 2061 6e79  u must cause any
+0001da80: 206d 6f64 6966 6965 6420 6669 6c65 7320   modified files 
+0001da90: 746f 2063 6172 7279 2070 726f 6d69 6e65  to carry promine
+0001daa0: 6e74 206e 6f74 6963 6573 2020 2020 2020  nt notices      
+0001dab0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001dac0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 0001dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dae0: 2063 6f6e 7472 6f6c 2077 6974 6820 7468   control with th
-0001daf0: 6174 2065 6e74 6974 792e 2046 6f72 2074  at entity. For t
-0001db00: 6865 2070 7572 706f 7365 7320 6f66 2074  he purposes of t
-0001db10: 6869 7320 6465 6669 6e69 7469 6f6e 2c20  his definition, 
-0001db20: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001dae0: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0001daf0: 7469 6e67 2074 6861 7420 596f 7520 6368  ting that You ch
+0001db00: 616e 6765 6420 7468 6520 6669 6c65 733b  anged the files;
+0001db10: 2061 6e64 2020 2020 2020 2020 2020 2020   and            
+0001db20: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001db30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db40: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001db50: 2020 2020 2022 636f 6e74 726f 6c22 206d       "control" m
-0001db60: 6561 6e73 2028 6929 2074 6865 2070 6f77  eans (i) the pow
-0001db70: 6572 2c20 6469 7265 6374 206f 7220 696e  er, direct or in
-0001db80: 6469 7265 6374 2c20 746f 2063 6175 7365  direct, to cause
-0001db90: 2074 6865 2020 2020 2020 2020 2020 2020   the            
-0001dba0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-0001dbb0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001dbc0: 2020 2020 2020 2020 2020 2064 6972 6563             direc
-0001dbd0: 7469 6f6e 206f 7220 6d61 6e61 6765 6d65  tion or manageme
-0001dbe0: 6e74 206f 6620 7375 6368 2065 6e74 6974  nt of such entit
-0001dbf0: 792c 2077 6865 7468 6572 2062 7920 636f  y, whether by co
-0001dc00: 6e74 7261 6374 206f 7220 2020 2020 2020  ntract or       
-0001dc10: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-0001dc20: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001dc30: 2020 2020 2020 2020 2020 2020 2020 6f74                ot
-0001dc40: 6865 7277 6973 652c 206f 7220 2869 6929  herwise, or (ii)
-0001dc50: 206f 776e 6572 7368 6970 206f 6620 6669   ownership of fi
-0001dc60: 6674 7920 7065 7263 656e 7420 2835 3025  fty percent (50%
-0001dc70: 2920 6f72 206d 6f72 6520 6f66 2074 6865  ) or more of the
-0001dc80: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+0001db40: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001db50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db90: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001dba0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0001dbb0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+0001dbc0: 2020 2020 2020 2020 2028 6329 2059 6f75           (c) You
+0001dbd0: 206d 7573 7420 7265 7461 696e 2c20 696e   must retain, in
+0001dbe0: 2074 6865 2053 6f75 7263 6520 666f 726d   the Source form
+0001dbf0: 206f 6620 616e 7920 4465 7269 7661 7469   of any Derivati
+0001dc00: 7665 2057 6f72 6b73 2020 2020 2020 2020  ve Works        
+0001dc10: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+0001dc20: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001dc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dc40: 2020 2074 6861 7420 596f 7520 6469 7374     that You dist
+0001dc50: 7269 6275 7465 2c20 616c 6c20 636f 7079  ribute, all copy
+0001dc60: 7269 6768 742c 2070 6174 656e 742c 2074  right, patent, t
+0001dc70: 7261 6465 6d61 726b 2c20 616e 6420 2020  rademark, and   
+0001dc80: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001dc90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dca0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-0001dcb0: 2020 206f 7574 7374 616e 6469 6e67 2073     outstanding s
-0001dcc0: 6861 7265 732c 206f 7220 2869 6969 2920  hares, or (iii) 
-0001dcd0: 6265 6e65 6669 6369 616c 206f 776e 6572  beneficial owner
-0001dce0: 7368 6970 206f 6620 7375 6368 2065 6e74  ship of such ent
-0001dcf0: 6974 792e 2020 2020 2020 2020 2020 207c  ity.           |
-0001dd00: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-0001dd10: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-0001dd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dd70: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-0001dd80: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001dca0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001dcb0: 2020 2020 2020 2020 2020 6174 7472 6962            attrib
+0001dcc0: 7574 696f 6e20 6e6f 7469 6365 7320 6672  ution notices fr
+0001dcd0: 6f6d 2074 6865 2053 6f75 7263 6520 666f  om the Source fo
+0001dce0: 726d 206f 6620 7468 6520 576f 726b 2c20  rm of the Work, 
+0001dcf0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+0001dd00: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001dd10: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0001dd20: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+0001dd30: 6c75 6469 6e67 2074 686f 7365 206e 6f74  luding those not
+0001dd40: 6963 6573 2074 6861 7420 646f 206e 6f74  ices that do not
+0001dd50: 2070 6572 7461 696e 2074 6f20 616e 7920   pertain to any 
+0001dd60: 7061 7274 206f 6620 2020 2020 2020 2020  part of         
+0001dd70: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+0001dd80: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 0001dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dda0: 2022 596f 7522 2028 6f72 2022 596f 7572   "You" (or "Your
-0001ddb0: 2229 2073 6861 6c6c 206d 6561 6e20 616e  ") shall mean an
-0001ddc0: 2069 6e64 6976 6964 7561 6c20 6f72 204c   individual or L
-0001ddd0: 6567 616c 2045 6e74 6974 7920 2020 2020  egal Entity     
-0001dde0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0001ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de00: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001de10: 2020 2020 2020 2020 2020 2065 7865 7263             exerc
-0001de20: 6973 696e 6720 7065 726d 6973 7369 6f6e  ising permission
-0001de30: 7320 6772 616e 7465 6420 6279 2074 6869  s granted by thi
-0001de40: 7320 4c69 6365 6e73 652e 2020 2020 2020  s License.      
-0001de50: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-0001de60: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001de70: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0001de80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001deb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ded0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0001dee0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001def0: 2020 2020 2020 2020 2020 2253 6f75 7263            "Sourc
-0001df00: 6522 2066 6f72 6d20 7368 616c 6c20 6d65  e" form shall me
-0001df10: 616e 2074 6865 2070 7265 6665 7272 6564  an the preferred
-0001df20: 2066 6f72 6d20 666f 7220 6d61 6b69 6e67   form for making
-0001df30: 206d 6f64 6966 6963 6174 696f 6e73 2c20   modifications, 
-0001df40: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-0001df50: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001dda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ddb0: 2020 7468 6520 4465 7269 7661 7469 7665    the Derivative
+0001ddc0: 2057 6f72 6b73 3b20 616e 6420 2020 2020   Works; and     
+0001ddd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dde0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001ddf0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de50: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+0001de60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de70: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001de80: 2020 2020 2020 2020 2028 6429 2049 6620           (d) If 
+0001de90: 7468 6520 576f 726b 2069 6e63 6c75 6465  the Work include
+0001dea0: 7320 6120 224e 4f54 4943 4522 2074 6578  s a "NOTICE" tex
+0001deb0: 7420 6669 6c65 2061 7320 7061 7274 206f  t file as part o
+0001dec0: 6620 6974 7320 2020 2020 2020 2020 2020  f its           
+0001ded0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+0001dee0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001def0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+0001df00: 7374 7269 6275 7469 6f6e 2c20 7468 656e  stribution, then
+0001df10: 2061 6e79 2044 6572 6976 6174 6976 6520   any Derivative 
+0001df20: 576f 726b 7320 7468 6174 2059 6f75 2064  Works that You d
+0001df30: 6973 7472 6962 7574 6520 6d75 7374 2020  istribute must  
+0001df40: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0001df50: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 0001df60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df70: 2020 696e 636c 7564 696e 6720 6275 7420    including but 
-0001df80: 6e6f 7420 6c69 6d69 7465 6420 746f 2073  not limited to s
-0001df90: 6f66 7477 6172 6520 736f 7572 6365 2063  oftware source c
-0001dfa0: 6f64 652c 2064 6f63 756d 656e 7461 7469  ode, documentati
-0001dfb0: 6f6e 2020 2020 2020 2020 2020 207c 0a7c  on           |.|
+0001df70: 2020 2020 2069 6e63 6c75 6465 2061 2072       include a r
+0001df80: 6561 6461 626c 6520 636f 7079 206f 6620  eadable copy of 
+0001df90: 7468 6520 6174 7472 6962 7574 696f 6e20  the attribution 
+0001dfa0: 6e6f 7469 6365 7320 636f 6e74 6169 6e65  notices containe
+0001dfb0: 6420 2020 2020 2020 2020 2020 7c0a 7c20  d           |.| 
 0001dfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dfd0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-0001dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dff0: 2020 2020 2020 2073 6f75 7263 652c 2061         source, a
-0001e000: 6e64 2063 6f6e 6669 6775 7261 7469 6f6e  nd configuration
-0001e010: 2066 696c 6573 2e20 2020 2020 2020 2020   files.         
-0001e020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e030: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-0001e040: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0a0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-0001e0b0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+0001dfd0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001dfe0: 2020 2020 2020 2020 2020 7769 7468 696e            within
+0001dff0: 2073 7563 6820 4e4f 5449 4345 2066 696c   such NOTICE fil
+0001e000: 652c 2065 7863 6c75 6469 6e67 2074 686f  e, excluding tho
+0001e010: 7365 206e 6f74 6963 6573 2074 6861 7420  se notices that 
+0001e020: 646f 206e 6f74 2020 2020 2020 2020 2020  do not          
+0001e030: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0001e040: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+0001e050: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001e060: 6572 7461 696e 2074 6f20 616e 7920 7061  ertain to any pa
+0001e070: 7274 206f 6620 7468 6520 4465 7269 7661  rt of the Deriva
+0001e080: 7469 7665 2057 6f72 6b73 2c20 696e 2061  tive Works, in a
+0001e090: 7420 6c65 6173 7420 6f6e 6520 2020 2020  t least one     
+0001e0a0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+0001e0b0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 0001e0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e0d0: 2020 2022 4f62 6a65 6374 2220 666f 726d     "Object" form
-0001e0e0: 2073 6861 6c6c 206d 6561 6e20 616e 7920   shall mean any 
-0001e0f0: 666f 726d 2072 6573 756c 7469 6e67 2066  form resulting f
-0001e100: 726f 6d20 6d65 6368 616e 6963 616c 2020  rom mechanical  
-0001e110: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+0001e0d0: 2020 206f 6620 7468 6520 666f 6c6c 6f77     of the follow
+0001e0e0: 696e 6720 706c 6163 6573 3a20 7769 7468  ing places: with
+0001e0f0: 696e 2061 204e 4f54 4943 4520 7465 7874  in a NOTICE text
+0001e100: 2066 696c 6520 6469 7374 7269 6275 7465   file distribute
+0001e110: 6420 2020 2020 2020 2020 207c 0a7c 2020  d          |.|  
 0001e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e130: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-0001e140: 2020 2020 2020 2074 7261 6e73 666f 726d         transform
-0001e150: 6174 696f 6e20 6f72 2074 7261 6e73 6c61  ation or transla
-0001e160: 7469 6f6e 206f 6620 6120 536f 7572 6365  tion of a Source
-0001e170: 2066 6f72 6d2c 2069 6e63 6c75 6469 6e67   form, including
-0001e180: 2062 7574 2020 2020 2020 2020 2020 2020   but            
-0001e190: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-0001e1a0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001e1b0: 2020 2020 2020 2020 2020 2020 6e6f 7420              not 
-0001e1c0: 6c69 6d69 7465 6420 746f 2063 6f6d 7069  limited to compi
-0001e1d0: 6c65 6420 6f62 6a65 6374 2063 6f64 652c  led object code,
-0001e1e0: 2067 656e 6572 6174 6564 2064 6f63 756d   generated docum
-0001e1f0: 656e 7461 7469 6f6e 2c20 2020 2020 2020  entation,       
-0001e200: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001e210: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0001e130: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+0001e140: 2020 2020 2020 2020 2020 6173 2070 6172            as par
+0001e150: 7420 6f66 2074 6865 2044 6572 6976 6174  t of the Derivat
+0001e160: 6976 6520 576f 726b 733b 2077 6974 6869  ive Works; withi
+0001e170: 6e20 7468 6520 536f 7572 6365 2066 6f72  n the Source for
+0001e180: 6d20 6f72 2020 2020 2020 2020 2020 2020  m or            
+0001e190: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0001e1a0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+0001e1b0: 2020 2020 2020 2020 2020 2020 646f 6375              docu
+0001e1c0: 6d65 6e74 6174 696f 6e2c 2069 6620 7072  mentation, if pr
+0001e1d0: 6f76 6964 6564 2061 6c6f 6e67 2077 6974  ovided along wit
+0001e1e0: 6820 7468 6520 4465 7269 7661 7469 7665  h the Derivative
+0001e1f0: 2057 6f72 6b73 3b20 6f72 2c20 2020 2020   Works; or,     
+0001e200: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001e210: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 0001e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e230: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-0001e240: 2063 6f6e 7665 7273 696f 6e73 2074 6f20   conversions to 
-0001e250: 6f74 6865 7220 6d65 6469 6120 7479 7065  other media type
-0001e260: 732e 2020 2020 2020 2020 2020 2020 2020  s.              
-0001e270: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001e230: 2020 2020 7769 7468 696e 2061 2064 6973      within a dis
+0001e240: 706c 6179 2067 656e 6572 6174 6564 2062  play generated b
+0001e250: 7920 7468 6520 4465 7269 7661 7469 7665  y the Derivative
+0001e260: 2057 6f72 6b73 2c20 6966 2061 6e64 2020   Works, if and  
+0001e270: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001e280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e290: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001e2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2f0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-0001e300: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001e310: 2020 2020 2020 2020 2020 2022 576f 726b             "Work
-0001e320: 2220 7368 616c 6c20 6d65 616e 2074 6865  " shall mean the
-0001e330: 2077 6f72 6b20 6f66 2061 7574 686f 7273   work of authors
-0001e340: 6869 702c 2077 6865 7468 6572 2069 6e20  hip, whether in 
-0001e350: 536f 7572 6365 206f 7220 2020 2020 2020  Source or       
-0001e360: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-0001e370: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001e380: 2020 2020 2020 2020 2020 2020 2020 204f                 O
-0001e390: 626a 6563 7420 666f 726d 2c20 6d61 6465  bject form, made
-0001e3a0: 2061 7661 696c 6162 6c65 2075 6e64 6572   available under
-0001e3b0: 2074 6865 204c 6963 656e 7365 2c20 6173   the License, as
-0001e3c0: 2069 6e64 6963 6174 6564 2062 7920 6120   indicated by a 
-0001e3d0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+0001e290: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001e2a0: 2020 2020 2020 7768 6572 6576 6572 2073        wherever s
+0001e2b0: 7563 6820 7468 6972 642d 7061 7274 7920  uch third-party 
+0001e2c0: 6e6f 7469 6365 7320 6e6f 726d 616c 6c79  notices normally
+0001e2d0: 2061 7070 6561 722e 2054 6865 2063 6f6e   appear. The con
+0001e2e0: 7465 6e74 7320 2020 2020 2020 2020 207c  tents          |
+0001e2f0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0001e300: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+0001e310: 2020 2020 2020 2020 2020 2020 2020 6f66                of
+0001e320: 2074 6865 204e 4f54 4943 4520 6669 6c65   the NOTICE file
+0001e330: 2061 7265 2066 6f72 2069 6e66 6f72 6d61   are for informa
+0001e340: 7469 6f6e 616c 2070 7572 706f 7365 7320  tional purposes 
+0001e350: 6f6e 6c79 2061 6e64 2020 2020 2020 2020  only and        
+0001e360: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+0001e370: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e390: 2020 646f 206e 6f74 206d 6f64 6966 7920    do not modify 
+0001e3a0: 7468 6520 4c69 6365 6e73 652e 2059 6f75  the License. You
+0001e3b0: 206d 6179 2061 6464 2059 6f75 7220 6f77   may add Your ow
+0001e3c0: 6e20 6174 7472 6962 7574 696f 6e20 2020  n attribution   
+0001e3d0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001e3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e3f0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-0001e400: 2020 2020 2020 636f 7079 7269 6768 7420        copyright 
-0001e410: 6e6f 7469 6365 2074 6861 7420 6973 2069  notice that is i
-0001e420: 6e63 6c75 6465 6420 696e 206f 7220 6174  ncluded in or at
-0001e430: 7461 6368 6564 2074 6f20 7468 6520 776f  tached to the wo
-0001e440: 726b 2020 2020 2020 2020 2020 2020 207c  rk             |
-0001e450: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-0001e460: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-0001e470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e480: 2028 616e 2065 7861 6d70 6c65 2069 7320   (an example is 
-0001e490: 7072 6f76 6964 6564 2069 6e20 7468 6520  provided in the 
-0001e4a0: 4170 7065 6e64 6978 2062 656c 6f77 292e  Appendix below).
-0001e4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e4c0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-0001e4d0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001e3f0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001e400: 2020 2020 2020 6e6f 7469 6365 7320 7769        notices wi
+0001e410: 7468 696e 2044 6572 6976 6174 6976 6520  thin Derivative 
+0001e420: 576f 726b 7320 7468 6174 2059 6f75 2064  Works that You d
+0001e430: 6973 7472 6962 7574 652c 2061 6c6f 6e67  istribute, along
+0001e440: 7369 6465 2020 2020 2020 2020 2020 7c0a  side          |.
+0001e450: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001e460: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0001e470: 2020 2020 2020 2020 2020 2020 6f72 2061              or a
+0001e480: 7320 616e 2061 6464 656e 6475 6d20 746f  s an addendum to
+0001e490: 2074 6865 204e 4f54 4943 4520 7465 7874   the NOTICE text
+0001e4a0: 2066 726f 6d20 7468 6520 576f 726b 2c20   from the Work, 
+0001e4b0: 7072 6f76 6964 6564 2020 2020 2020 2020  provided        
+0001e4c0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+0001e4d0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 0001e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e530: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0001e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e550: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001e560: 2022 4465 7269 7661 7469 7665 2057 6f72   "Derivative Wor
-0001e570: 6b73 2220 7368 616c 6c20 6d65 616e 2061  ks" shall mean a
-0001e580: 6e79 2077 6f72 6b2c 2077 6865 7468 6572  ny work, whether
-0001e590: 2069 6e20 536f 7572 6365 206f 7220 4f62   in Source or Ob
-0001e5a0: 6a65 6374 2020 2020 2020 2020 2020 7c0a  ject          |.
-0001e5b0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001e5c0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0001e5d0: 2020 2020 2020 666f 726d 2c20 7468 6174        form, that
-0001e5e0: 2069 7320 6261 7365 6420 6f6e 2028 6f72   is based on (or
-0001e5f0: 2064 6572 6976 6564 2066 726f 6d29 2074   derived from) t
-0001e600: 6865 2057 6f72 6b20 616e 6420 666f 7220  he Work and for 
-0001e610: 7768 6963 6820 7468 6520 2020 2020 2020  which the       
-0001e620: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0001e630: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001e640: 2020 2020 2020 2020 2020 6564 6974 6f72            editor
-0001e650: 6961 6c20 7265 7669 7369 6f6e 732c 2061  ial revisions, a
-0001e660: 6e6e 6f74 6174 696f 6e73 2c20 656c 6162  nnotations, elab
-0001e670: 6f72 6174 696f 6e73 2c20 6f72 206f 7468  orations, or oth
-0001e680: 6572 206d 6f64 6966 6963 6174 696f 6e73  er modifications
-0001e690: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-0001e6a0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0001e6b0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0001e6c0: 7072 6573 656e 742c 2061 7320 6120 7768  present, as a wh
-0001e6d0: 6f6c 652c 2061 6e20 6f72 6967 696e 616c  ole, an original
-0001e6e0: 2077 6f72 6b20 6f66 2061 7574 686f 7273   work of authors
-0001e6f0: 6869 702e 2046 6f72 2074 6865 2070 7572  hip. For the pur
-0001e700: 706f 7365 7320 2020 2020 2020 207c 0a7c  poses        |.|
+0001e4f0: 2074 6861 7420 7375 6368 2061 6464 6974   that such addit
+0001e500: 696f 6e61 6c20 6174 7472 6962 7574 696f  ional attributio
+0001e510: 6e20 6e6f 7469 6365 7320 6361 6e6e 6f74  n notices cannot
+0001e520: 2062 6520 636f 6e73 7472 7565 6420 2020   be construed   
+0001e530: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001e540: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e570: 2020 2020 2020 2061 7320 6d6f 6469 6679         as modify
+0001e580: 696e 6720 7468 6520 4c69 6365 6e73 652e  ing the License.
+0001e590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e5a0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+0001e5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e5c0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e620: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+0001e630: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001e640: 2020 2020 2020 2020 2020 2059 6f75 206d             You m
+0001e650: 6179 2061 6464 2059 6f75 7220 6f77 6e20  ay add Your own 
+0001e660: 636f 7079 7269 6768 7420 7374 6174 656d  copyright statem
+0001e670: 656e 7420 746f 2059 6f75 7220 6d6f 6469  ent to Your modi
+0001e680: 6669 6361 7469 6f6e 7320 616e 6420 2020  fications and   
+0001e690: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0001e6a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+0001e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e6c0: 206d 6179 2070 726f 7669 6465 2061 6464   may provide add
+0001e6d0: 6974 696f 6e61 6c20 6f72 2064 6966 6665  itional or diffe
+0001e6e0: 7265 6e74 206c 6963 656e 7365 2074 6572  rent license ter
+0001e6f0: 6d73 2061 6e64 2063 6f6e 6469 7469 6f6e  ms and condition
+0001e700: 7320 2020 2020 2020 2020 2020 7c0a 7c20  s           |.| 
 0001e710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e720: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-0001e730: 2020 2020 6f66 2074 6869 7320 4c69 6365      of this Lice
-0001e740: 6e73 652c 2044 6572 6976 6174 6976 6520  nse, Derivative 
-0001e750: 576f 726b 7320 7368 616c 6c20 6e6f 7420  Works shall not 
-0001e760: 696e 636c 7564 6520 776f 726b 7320 7468  include works th
-0001e770: 6174 2072 656d 6169 6e20 2020 2020 2020  at remain       
-0001e780: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-0001e790: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001e7a0: 2020 2020 2020 2020 2073 6570 6172 6162           separab
-0001e7b0: 6c65 2066 726f 6d2c 206f 7220 6d65 7265  le from, or mere
-0001e7c0: 6c79 206c 696e 6b20 286f 7220 6269 6e64  ly link (or bind
-0001e7d0: 2062 7920 6e61 6d65 2920 746f 2074 6865   by name) to the
-0001e7e0: 2069 6e74 6572 6661 6365 7320 6f66 2c20   interfaces of, 
-0001e7f0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-0001e800: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0001e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e820: 2020 2020 2020 2020 2020 2020 2020 7468                th
-0001e830: 6520 576f 726b 2061 6e64 2044 6572 6976  e Work and Deriv
-0001e840: 6174 6976 6520 576f 726b 7320 7468 6572  ative Works ther
-0001e850: 656f 662e 2020 2020 2020 2020 2020 2020  eof.            
-0001e860: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+0001e720: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001e730: 2020 2020 2020 666f 7220 7573 652c 2072        for use, r
+0001e740: 6570 726f 6475 6374 696f 6e2c 206f 7220  eproduction, or 
+0001e750: 6469 7374 7269 6275 7469 6f6e 206f 6620  distribution of 
+0001e760: 596f 7572 206d 6f64 6966 6963 6174 696f  Your modificatio
+0001e770: 6e73 2c20 6f72 2020 2020 2020 2020 2020  ns, or          
+0001e780: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0001e790: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+0001e7a0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0001e7b0: 2061 6e79 2073 7563 6820 4465 7269 7661   any such Deriva
+0001e7c0: 7469 7665 2057 6f72 6b73 2061 7320 6120  tive Works as a 
+0001e7d0: 7768 6f6c 652c 2070 726f 7669 6465 6420  whole, provided 
+0001e7e0: 596f 7572 2075 7365 2c20 2020 2020 2020  Your use,       
+0001e7f0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+0001e800: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0001e810: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0001e820: 6570 726f 6475 6374 696f 6e2c 2061 6e64  eproduction, and
+0001e830: 2064 6973 7472 6962 7574 696f 6e20 6f66   distribution of
+0001e840: 2074 6865 2057 6f72 6b20 6f74 6865 7277   the Work otherw
+0001e850: 6973 6520 636f 6d70 6c69 6573 2077 6974  ise complies wit
+0001e860: 6820 2020 2020 2020 2020 207c 0a7c 2020  h          |.|  
 0001e870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e880: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001e880: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
 0001e890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e8a0: 2020 7468 6520 636f 6e64 6974 696f 6e73    the conditions
+0001e8b0: 2073 7461 7465 6420 696e 2074 6869 7320   stated in this 
+0001e8c0: 4c69 6365 6e73 652e 2020 2020 2020 2020  License.        
 0001e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8e0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-0001e8f0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001e900: 2020 2020 2020 2020 2020 2020 2022 436f               "Co
-0001e910: 6e74 7269 6275 7469 6f6e 2220 7368 616c  ntribution" shal
-0001e920: 6c20 6d65 616e 2061 6e79 2077 6f72 6b20  l mean any work 
-0001e930: 6f66 2061 7574 686f 7273 6869 702c 2069  of authorship, i
-0001e940: 6e63 6c75 6469 6e67 2020 2020 2020 2020  ncluding        
-0001e950: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001e960: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-0001e970: 2020 2020 2020 2020 2020 2020 2020 7468                th
-0001e980: 6520 6f72 6967 696e 616c 2076 6572 7369  e original versi
-0001e990: 6f6e 206f 6620 7468 6520 576f 726b 2061  on of the Work a
-0001e9a0: 6e64 2061 6e79 206d 6f64 6966 6963 6174  nd any modificat
-0001e9b0: 696f 6e73 206f 7220 6164 6469 7469 6f6e  ions or addition
-0001e9c0: 7320 2020 2020 2020 2020 207c 0a7c 2020  s          |.|  
+0001e8e0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0001e8f0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+0001e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e950: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001e960: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0001e970: 2020 2020 2020 2020 2020 352e 2053 7562            5. Sub
+0001e980: 6d69 7373 696f 6e20 6f66 2043 6f6e 7472  mission of Contr
+0001e990: 6962 7574 696f 6e73 2e20 556e 6c65 7373  ibutions. Unless
+0001e9a0: 2059 6f75 2065 7870 6c69 6369 746c 7920   You explicitly 
+0001e9b0: 7374 6174 6520 6f74 6865 7277 6973 652c  state otherwise,
+0001e9c0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e9e0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001e9f0: 2020 2020 2074 6f20 7468 6174 2057 6f72       to that Wor
-0001ea00: 6b20 6f72 2044 6572 6976 6174 6976 6520  k or Derivative 
-0001ea10: 576f 726b 7320 7468 6572 656f 662c 2074  Works thereof, t
-0001ea20: 6861 7420 6973 2069 6e74 656e 7469 6f6e  hat is intention
-0001ea30: 616c 6c79 2020 2020 2020 2020 2020 2020  ally            
-0001ea40: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-0001ea50: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001ea60: 2020 2020 2020 2073 7562 6d69 7474 6564         submitted
-0001ea70: 2074 6f20 4c69 6365 6e73 6f72 2066 6f72   to Licensor for
-0001ea80: 2069 6e63 6c75 7369 6f6e 2069 6e20 7468   inclusion in th
-0001ea90: 6520 576f 726b 2062 7920 7468 6520 636f  e Work by the co
-0001eaa0: 7079 7269 6768 7420 6f77 6e65 7220 2020  pyright owner   
-0001eab0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-0001eac0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001ead0: 2020 2020 2020 2020 2020 2020 6f72 2062              or b
-0001eae0: 7920 616e 2069 6e64 6976 6964 7561 6c20  y an individual 
-0001eaf0: 6f72 204c 6567 616c 2045 6e74 6974 7920  or Legal Entity 
-0001eb00: 6175 7468 6f72 697a 6564 2074 6f20 7375  authorized to su
-0001eb10: 626d 6974 206f 6e20 6265 6861 6c66 206f  bmit on behalf o
-0001eb20: 6620 2020 2020 2020 2020 7c0a 7c20 2020  f         |.|   
+0001e9e0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001e9f0: 2020 2061 6e79 2043 6f6e 7472 6962 7574     any Contribut
+0001ea00: 696f 6e20 696e 7465 6e74 696f 6e61 6c6c  ion intentionall
+0001ea10: 7920 7375 626d 6974 7465 6420 666f 7220  y submitted for 
+0001ea20: 696e 636c 7573 696f 6e20 696e 2074 6865  inclusion in the
+0001ea30: 2057 6f72 6b20 2020 2020 2020 2020 207c   Work          |
+0001ea40: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0001ea50: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+0001ea60: 2020 2020 2020 2020 6279 2059 6f75 2074          by You t
+0001ea70: 6f20 7468 6520 4c69 6365 6e73 6f72 2073  o the Licensor s
+0001ea80: 6861 6c6c 2062 6520 756e 6465 7220 7468  hall be under th
+0001ea90: 6520 7465 726d 7320 616e 6420 636f 6e64  e terms and cond
+0001eaa0: 6974 696f 6e73 206f 6620 2020 2020 2020  itions of       
+0001eab0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+0001eac0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eae0: 2074 6869 7320 4c69 6365 6e73 652c 2077   this License, w
+0001eaf0: 6974 686f 7574 2061 6e79 2061 6464 6974  ithout any addit
+0001eb00: 696f 6e61 6c20 7465 726d 7320 6f72 2063  ional terms or c
+0001eb10: 6f6e 6469 7469 6f6e 732e 2020 2020 2020  onditions.      
+0001eb20: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb40: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-0001eb50: 2074 6865 2063 6f70 7972 6967 6874 206f   the copyright o
-0001eb60: 776e 6572 2e20 466f 7220 7468 6520 7075  wner. For the pu
-0001eb70: 7270 6f73 6573 206f 6620 7468 6973 2064  rposes of this d
-0001eb80: 6566 696e 6974 696f 6e2c 2022 7375 626d  efinition, "subm
-0001eb90: 6974 7465 6422 2020 2020 2020 2020 207c  itted"         |
-0001eba0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-0001ebb0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-0001ebc0: 2020 2020 2020 206d 6561 6e73 2061 6e79         means any
-0001ebd0: 2066 6f72 6d20 6f66 2065 6c65 6374 726f   form of electro
-0001ebe0: 6e69 632c 2076 6572 6261 6c2c 206f 7220  nic, verbal, or 
-0001ebf0: 7772 6974 7465 6e20 636f 6d6d 756e 6963  written communic
-0001ec00: 6174 696f 6e20 7365 6e74 2020 2020 2020  ation sent      
-0001ec10: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-0001ec20: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-0001ec30: 2020 2020 2020 2020 2020 2020 746f 2074              to t
-0001ec40: 6865 204c 6963 656e 736f 7220 6f72 2069  he Licensor or i
-0001ec50: 7473 2072 6570 7265 7365 6e74 6174 6976  ts representativ
-0001ec60: 6573 2c20 696e 636c 7564 696e 6720 6275  es, including bu
-0001ec70: 7420 6e6f 7420 6c69 6d69 7465 6420 746f  t not limited to
-0001ec80: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0001ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eca0: 7c20 2020 2020 2020 2020 2020 2020 2063  |              c
-0001ecb0: 6f6d 6d75 6e69 6361 7469 6f6e 206f 6e20  ommunication on 
-0001ecc0: 656c 6563 7472 6f6e 6963 206d 6169 6c69  electronic maili
-0001ecd0: 6e67 206c 6973 7473 2c20 736f 7572 6365  ng lists, source
-0001ece0: 2063 6f64 6520 636f 6e74 726f 6c20 7379   code control sy
-0001ecf0: 7374 656d 732c 2020 2020 2020 2020 7c0a  stems,        |.
-0001ed00: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001ed10: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0001ed20: 2020 2020 2020 616e 6420 6973 7375 6520        and issue 
-0001ed30: 7472 6163 6b69 6e67 2073 7973 7465 6d73  tracking systems
-0001ed40: 2074 6861 7420 6172 6520 6d61 6e61 6765   that are manage
-0001ed50: 6420 6279 2c20 6f72 206f 6e20 6265 6861  d by, or on beha
-0001ed60: 6c66 206f 662c 2074 6865 2020 2020 2020  lf of, the      
-0001ed70: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0001ed80: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001ed90: 2020 2020 2020 2020 2020 2020 4c69 6365              Lice
-0001eda0: 6e73 6f72 2066 6f72 2074 6865 2070 7572  nsor for the pur
-0001edb0: 706f 7365 206f 6620 6469 7363 7573 7369  pose of discussi
-0001edc0: 6e67 2061 6e64 2069 6d70 726f 7669 6e67  ng and improving
-0001edd0: 2074 6865 2057 6f72 6b2c 2062 7574 2020   the Work, but  
-0001ede0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-0001edf0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-0001ee00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ee10: 2065 7863 6c75 6469 6e67 2063 6f6d 6d75   excluding commu
-0001ee20: 6e69 6361 7469 6f6e 2074 6861 7420 6973  nication that is
-0001ee30: 2063 6f6e 7370 6963 756f 7573 6c79 206d   conspicuously m
-0001ee40: 6172 6b65 6420 6f72 206f 7468 6572 7769  arked or otherwi
-0001ee50: 7365 2020 2020 2020 2020 2020 207c 0a7c  se           |.|
+0001eb40: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001eb50: 204e 6f74 7769 7468 7374 616e 6469 6e67   Notwithstanding
+0001eb60: 2074 6865 2061 626f 7665 2c20 6e6f 7468   the above, noth
+0001eb70: 696e 6720 6865 7265 696e 2073 6861 6c6c  ing herein shall
+0001eb80: 2073 7570 6572 7365 6465 206f 7220 6d6f   supersede or mo
+0001eb90: 6469 6679 2020 2020 2020 2020 2020 7c0a  dify          |.
+0001eba0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001ebb0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0001ebc0: 2020 2020 2020 2074 6865 2074 6572 6d73         the terms
+0001ebd0: 206f 6620 616e 7920 7365 7061 7261 7465   of any separate
+0001ebe0: 206c 6963 656e 7365 2061 6772 6565 6d65   license agreeme
+0001ebf0: 6e74 2079 6f75 206d 6179 2068 6176 6520  nt you may have 
+0001ec00: 6578 6563 7574 6564 2020 2020 2020 2020  executed        
+0001ec10: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+0001ec20: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+0001ec30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec40: 2020 2020 2020 2077 6974 6820 4c69 6365         with Lice
+0001ec50: 6e73 6f72 2072 6567 6172 6469 6e67 2073  nsor regarding s
+0001ec60: 7563 6820 436f 6e74 7269 6275 7469 6f6e  uch Contribution
+0001ec70: 732e 2020 2020 2020 2020 2020 2020 2020  s.              
+0001ec80: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001ec90: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ecb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ece0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ecf0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+0001ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed10: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001ed20: 2020 362e 2054 7261 6465 6d61 726b 732e    6. Trademarks.
+0001ed30: 2054 6869 7320 4c69 6365 6e73 6520 646f   This License do
+0001ed40: 6573 206e 6f74 2067 7261 6e74 2070 6572  es not grant per
+0001ed50: 6d69 7373 696f 6e20 746f 2075 7365 2074  mission to use t
+0001ed60: 6865 2074 7261 6465 2020 2020 2020 2020  he trade        
+0001ed70: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+0001ed80: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001ed90: 2020 2020 2020 2020 2020 6e61 6d65 732c            names,
+0001eda0: 2074 7261 6465 6d61 726b 732c 2073 6572   trademarks, ser
+0001edb0: 7669 6365 206d 6172 6b73 2c20 6f72 2070  vice marks, or p
+0001edc0: 726f 6475 6374 206e 616d 6573 206f 6620  roduct names of 
+0001edd0: 7468 6520 4c69 6365 6e73 6f72 2c20 2020  the Licensor,   
+0001ede0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0001edf0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+0001ee00: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+0001ee10: 6365 7074 2061 7320 7265 7175 6972 6564  cept as required
+0001ee20: 2066 6f72 2072 6561 736f 6e61 626c 6520   for reasonable 
+0001ee30: 616e 6420 6375 7374 6f6d 6172 7920 7573  and customary us
+0001ee40: 6520 696e 2064 6573 6372 6962 696e 6720  e in describing 
+0001ee50: 7468 6520 2020 2020 2020 2020 7c0a 7c20  the         |.| 
 0001ee60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ee70: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-0001ee80: 2020 2020 6465 7369 676e 6174 6564 2069      designated i
-0001ee90: 6e20 7772 6974 696e 6720 6279 2074 6865  n writing by the
-0001eea0: 2063 6f70 7972 6967 6874 206f 776e 6572   copyright owner
-0001eeb0: 2061 7320 224e 6f74 2061 2043 6f6e 7472   as "Not a Contr
-0001eec0: 6962 7574 696f 6e2e 2220 2020 2020 2020  ibution."       
-0001eed0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-0001eee0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001ee70: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001ee80: 2020 2020 206f 7269 6769 6e20 6f66 2074       origin of t
+0001ee90: 6865 2057 6f72 6b20 616e 6420 7265 7072  he Work and repr
+0001eea0: 6f64 7563 696e 6720 7468 6520 636f 6e74  oducing the cont
+0001eeb0: 656e 7420 6f66 2074 6865 204e 4f54 4943  ent of the NOTIC
+0001eec0: 4520 6669 6c65 2e20 2020 2020 2020 2020  E file.         
+0001eed0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0001eee0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
 0001eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ef00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ef20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ef30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef40: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-0001ef50: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-0001ef60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0001ef70: 436f 6e74 7269 6275 746f 7222 2073 6861  Contributor" sha
-0001ef80: 6c6c 206d 6561 6e20 4c69 6365 6e73 6f72  ll mean Licensor
-0001ef90: 2061 6e64 2061 6e79 2069 6e64 6976 6964   and any individ
-0001efa0: 7561 6c20 6f72 204c 6567 616c 2045 6e74  ual or Legal Ent
-0001efb0: 6974 7920 2020 2020 2020 2020 7c0a 7c20  ity         |.| 
+0001ef40: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+0001ef50: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0001ef60: 2020 2020 2020 2020 2020 2020 2020 2037                 7
+0001ef70: 2e20 4469 7363 6c61 696d 6572 206f 6620  . Disclaimer of 
+0001ef80: 5761 7272 616e 7479 2e20 556e 6c65 7373  Warranty. Unless
+0001ef90: 2072 6571 7569 7265 6420 6279 2061 7070   required by app
+0001efa0: 6c69 6361 626c 6520 6c61 7720 6f72 2020  licable law or  
+0001efb0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 0001efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001efd0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-0001efe0: 2020 2020 206f 6e20 6265 6861 6c66 206f       on behalf o
-0001eff0: 6620 7768 6f6d 2061 2043 6f6e 7472 6962  f whom a Contrib
-0001f000: 7574 696f 6e20 6861 7320 6265 656e 2072  ution has been r
-0001f010: 6563 6569 7665 6420 6279 204c 6963 656e  eceived by Licen
-0001f020: 736f 7220 616e 6420 2020 2020 2020 2020  sor and         
-0001f030: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-0001f040: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001f050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f060: 2020 2020 2020 7375 6273 6571 7565 6e74        subsequent
-0001f070: 6c79 2069 6e63 6f72 706f 7261 7465 6420  ly incorporated 
-0001f080: 7769 7468 696e 2074 6865 2057 6f72 6b2e  within the Work.
-0001f090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0a0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001f0b0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-0001f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f110: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001efd0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+0001efe0: 2020 2020 2020 2020 6167 7265 6564 2074          agreed t
+0001eff0: 6f20 696e 2077 7269 7469 6e67 2c20 4c69  o in writing, Li
+0001f000: 6365 6e73 6f72 2070 726f 7669 6465 7320  censor provides 
+0001f010: 7468 6520 576f 726b 2028 616e 6420 6561  the Work (and ea
+0001f020: 6368 2020 2020 2020 2020 2020 2020 2020  ch              
+0001f030: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0001f040: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+0001f050: 2020 2020 2020 2020 2020 2020 436f 6e74              Cont
+0001f060: 7269 6275 746f 7220 7072 6f76 6964 6573  ributor provides
+0001f070: 2069 7473 2043 6f6e 7472 6962 7574 696f   its Contributio
+0001f080: 6e73 2920 6f6e 2061 6e20 2241 5320 4953  ns) on an "AS IS
+0001f090: 2220 4241 5349 532c 2020 2020 2020 2020  " BASIS,        
+0001f0a0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001f0b0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0001f0c0: 2020 2020 2020 2020 2020 2020 2020 2057                 W
+0001f0d0: 4954 484f 5554 2057 4152 5241 4e54 4945  ITHOUT WARRANTIE
+0001f0e0: 5320 4f52 2043 4f4e 4449 5449 4f4e 5320  S OR CONDITIONS 
+0001f0f0: 4f46 2041 4e59 204b 494e 442c 2065 6974  OF ANY KIND, eit
+0001f100: 6865 7220 6578 7072 6573 7320 6f72 2020  her express or  
+0001f110: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001f120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f130: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001f140: 2032 2e20 4772 616e 7420 6f66 2043 6f70   2. Grant of Cop
-0001f150: 7972 6967 6874 204c 6963 656e 7365 2e20  yright License. 
-0001f160: 5375 626a 6563 7420 746f 2074 6865 2074  Subject to the t
-0001f170: 6572 6d73 2061 6e64 2063 6f6e 6469 7469  erms and conditi
-0001f180: 6f6e 7320 6f66 2020 2020 2020 2020 2020  ons of          
-0001f190: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-0001f1a0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001f1b0: 2020 2020 2020 2020 2020 7468 6973 204c            this L
-0001f1c0: 6963 656e 7365 2c20 6561 6368 2043 6f6e  icense, each Con
-0001f1d0: 7472 6962 7574 6f72 2068 6572 6562 7920  tributor hereby 
-0001f1e0: 6772 616e 7473 2074 6f20 596f 7520 6120  grants to You a 
-0001f1f0: 7065 7270 6574 7561 6c2c 2020 2020 2020  perpetual,      
-0001f200: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-0001f210: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f230: 776f 726c 6477 6964 652c 206e 6f6e 2d65  worldwide, non-e
-0001f240: 7863 6c75 7369 7665 2c20 6e6f 2d63 6861  xclusive, no-cha
-0001f250: 7267 652c 2072 6f79 616c 7479 2d66 7265  rge, royalty-fre
-0001f260: 652c 2069 7272 6576 6f63 6162 6c65 2020  e, irrevocable  
-0001f270: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+0001f130: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001f140: 2020 696d 706c 6965 642c 2069 6e63 6c75    implied, inclu
+0001f150: 6469 6e67 2c20 7769 7468 6f75 7420 6c69  ding, without li
+0001f160: 6d69 7461 7469 6f6e 2c20 616e 7920 7761  mitation, any wa
+0001f170: 7272 616e 7469 6573 206f 7220 636f 6e64  rranties or cond
+0001f180: 6974 696f 6e73 2020 2020 2020 2020 207c  itions         |
+0001f190: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0001f1a0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+0001f1b0: 2020 2020 2020 2020 2020 6f66 2054 4954            of TIT
+0001f1c0: 4c45 2c20 4e4f 4e2d 494e 4652 494e 4745  LE, NON-INFRINGE
+0001f1d0: 4d45 4e54 2c20 4d45 5243 4841 4e54 4142  MENT, MERCHANTAB
+0001f1e0: 494c 4954 592c 206f 7220 4649 544e 4553  ILITY, or FITNES
+0001f1f0: 5320 464f 5220 4120 2020 2020 2020 2020  S FOR A         
+0001f200: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+0001f210: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001f220: 2020 2020 2020 2020 2020 2020 2050 4152               PAR
+0001f230: 5449 4355 4c41 5220 5055 5250 4f53 452e  TICULAR PURPOSE.
+0001f240: 2059 6f75 2061 7265 2073 6f6c 656c 7920   You are solely 
+0001f250: 7265 7370 6f6e 7369 626c 6520 666f 7220  responsible for 
+0001f260: 6465 7465 726d 696e 696e 6720 7468 6520  determining the 
+0001f270: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001f280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f290: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-0001f2a0: 2020 2020 2020 636f 7079 7269 6768 7420        copyright 
-0001f2b0: 6c69 6365 6e73 6520 746f 2072 6570 726f  license to repro
-0001f2c0: 6475 6365 2c20 7072 6570 6172 6520 4465  duce, prepare De
-0001f2d0: 7269 7661 7469 7665 2057 6f72 6b73 206f  rivative Works o
-0001f2e0: 662c 2020 2020 2020 2020 2020 2020 207c  f,             |
-0001f2f0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-0001f300: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-0001f310: 2020 2020 2020 2020 7075 626c 6963 6c79          publicly
-0001f320: 2064 6973 706c 6179 2c20 7075 626c 6963   display, public
-0001f330: 6c79 2070 6572 666f 726d 2c20 7375 626c  ly perform, subl
-0001f340: 6963 656e 7365 2c20 616e 6420 6469 7374  icense, and dist
-0001f350: 7269 6275 7465 2074 6865 2020 2020 2020  ribute the      
-0001f360: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-0001f370: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001f290: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001f2a0: 2020 6170 7072 6f70 7269 6174 656e 6573    appropriatenes
+0001f2b0: 7320 6f66 2075 7369 6e67 206f 7220 7265  s of using or re
+0001f2c0: 6469 7374 7269 6275 7469 6e67 2074 6865  distributing the
+0001f2d0: 2057 6f72 6b20 616e 6420 6173 7375 6d65   Work and assume
+0001f2e0: 2061 6e79 2020 2020 2020 2020 2020 7c0a   any          |.
+0001f2f0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001f300: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0001f310: 2020 2020 2072 6973 6b73 2061 7373 6f63       risks assoc
+0001f320: 6961 7465 6420 7769 7468 2059 6f75 7220  iated with Your 
+0001f330: 6578 6572 6369 7365 206f 6620 7065 726d  exercise of perm
+0001f340: 6973 7369 6f6e 7320 756e 6465 7220 7468  issions under th
+0001f350: 6973 204c 6963 656e 7365 2e20 2020 2020  is License.     
+0001f360: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+0001f370: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
 0001f380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f390: 2020 576f 726b 2061 6e64 2073 7563 6820    Work and such 
-0001f3a0: 4465 7269 7661 7469 7665 2057 6f72 6b73  Derivative Works
-0001f3b0: 2069 6e20 536f 7572 6365 206f 7220 4f62   in Source or Ob
-0001f3c0: 6a65 6374 2066 6f72 6d2e 2020 2020 2020  ject form.      
-0001f3d0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0001f3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f3f0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001f400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f440: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-0001f450: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001f460: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0001f470: 2020 2020 2033 2e20 4772 616e 7420 6f66       3. Grant of
-0001f480: 2050 6174 656e 7420 4c69 6365 6e73 652e   Patent License.
-0001f490: 2053 7562 6a65 6374 2074 6f20 7468 6520   Subject to the 
-0001f4a0: 7465 726d 7320 616e 6420 636f 6e64 6974  terms and condit
-0001f4b0: 696f 6e73 206f 6620 2020 2020 2020 2020  ions of         
-0001f4c0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0001f4d0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001f4e0: 2020 2020 2020 2020 2020 2020 2074 6869               thi
-0001f4f0: 7320 4c69 6365 6e73 652c 2065 6163 6820  s License, each 
-0001f500: 436f 6e74 7269 6275 746f 7220 6865 7265  Contributor here
-0001f510: 6279 2067 7261 6e74 7320 746f 2059 6f75  by grants to You
-0001f520: 2061 2070 6572 7065 7475 616c 2c20 2020   a perpetual,   
-0001f530: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-0001f540: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001f390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f3d0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001f3e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001f3f0: 2020 2020 2020 2020 2020 2020 2020 2038                 8
+0001f400: 2e20 4c69 6d69 7461 7469 6f6e 206f 6620  . Limitation of 
+0001f410: 4c69 6162 696c 6974 792e 2049 6e20 6e6f  Liability. In no
+0001f420: 2065 7665 6e74 2061 6e64 2075 6e64 6572   event and under
+0001f430: 206e 6f20 6c65 6761 6c20 7468 656f 7279   no legal theory
+0001f440: 2c20 2020 2020 2020 2020 2020 207c 0a7c  ,            |.|
+0001f450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f460: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001f470: 2020 2020 2020 2077 6865 7468 6572 2069         whether i
+0001f480: 6e20 746f 7274 2028 696e 636c 7564 696e  n tort (includin
+0001f490: 6720 6e65 676c 6967 656e 6365 292c 2063  g negligence), c
+0001f4a0: 6f6e 7472 6163 742c 206f 7220 6f74 6865  ontract, or othe
+0001f4b0: 7277 6973 652c 2020 2020 2020 2020 2020  rwise,          
+0001f4c0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+0001f4d0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001f4e0: 2020 2020 2020 2020 2020 2075 6e6c 6573             unles
+0001f4f0: 7320 7265 7175 6972 6564 2062 7920 6170  s required by ap
+0001f500: 706c 6963 6162 6c65 206c 6177 2028 7375  plicable law (su
+0001f510: 6368 2061 7320 6465 6c69 6265 7261 7465  ch as deliberate
+0001f520: 2061 6e64 2067 726f 7373 6c79 2020 2020   and grossly    
+0001f530: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0001f540: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 0001f550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f560: 2020 2077 6f72 6c64 7769 6465 2c20 6e6f     worldwide, no
-0001f570: 6e2d 6578 636c 7573 6976 652c 206e 6f2d  n-exclusive, no-
-0001f580: 6368 6172 6765 2c20 726f 7961 6c74 792d  charge, royalty-
-0001f590: 6672 6565 2c20 6972 7265 766f 6361 626c  free, irrevocabl
-0001f5a0: 6520 2020 2020 2020 2020 2020 207c 0a7c  e            |.|
+0001f560: 6e65 676c 6967 656e 7420 6163 7473 2920  negligent acts) 
+0001f570: 6f72 2061 6772 6565 6420 746f 2069 6e20  or agreed to in 
+0001f580: 7772 6974 696e 672c 2073 6861 6c6c 2061  writing, shall a
+0001f590: 6e79 2043 6f6e 7472 6962 7574 6f72 2062  ny Contributor b
+0001f5a0: 6520 2020 2020 2020 2020 2020 7c0a 7c20  e           |.| 
 0001f5b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f5c0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-0001f5d0: 2020 2020 2865 7863 6570 7420 6173 2073      (except as s
-0001f5e0: 7461 7465 6420 696e 2074 6869 7320 7365  tated in this se
-0001f5f0: 6374 696f 6e29 2070 6174 656e 7420 6c69  ction) patent li
-0001f600: 6365 6e73 6520 746f 206d 616b 652c 2068  cense to make, h
-0001f610: 6176 6520 6d61 6465 2c20 2020 2020 2020  ave made,       
-0001f620: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-0001f630: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001f640: 2020 2020 2020 2020 2020 2075 7365 2c20             use, 
-0001f650: 6f66 6665 7220 746f 2073 656c 6c2c 2073  offer to sell, s
-0001f660: 656c 6c2c 2069 6d70 6f72 742c 2061 6e64  ell, import, and
-0001f670: 206f 7468 6572 7769 7365 2074 7261 6e73   otherwise trans
-0001f680: 6665 7220 7468 6520 576f 726b 2c20 2020  fer the Work,   
-0001f690: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-0001f6a0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+0001f5c0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001f5d0: 2020 2020 6c69 6162 6c65 2074 6f20 596f      liable to Yo
+0001f5e0: 7520 666f 7220 6461 6d61 6765 732c 2069  u for damages, i
+0001f5f0: 6e63 6c75 6469 6e67 2061 6e79 2064 6972  ncluding any dir
+0001f600: 6563 742c 2069 6e64 6972 6563 742c 2073  ect, indirect, s
+0001f610: 7065 6369 616c 2c20 2020 2020 2020 2020  pecial,         
+0001f620: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0001f630: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+0001f640: 2020 2020 2020 2020 2020 696e 6369 6465            incide
+0001f650: 6e74 616c 2c20 6f72 2063 6f6e 7365 7175  ntal, or consequ
+0001f660: 656e 7469 616c 2064 616d 6167 6573 206f  ential damages o
+0001f670: 6620 616e 7920 6368 6172 6163 7465 7220  f any character 
+0001f680: 6172 6973 696e 6720 6173 2061 2020 2020  arising as a    
+0001f690: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+0001f6a0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 0001f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f6c0: 7768 6572 6520 7375 6368 206c 6963 656e  where such licen
-0001f6d0: 7365 2061 7070 6c69 6573 206f 6e6c 7920  se applies only 
-0001f6e0: 746f 2074 686f 7365 2070 6174 656e 7420  to those patent 
-0001f6f0: 636c 6169 6d73 206c 6963 656e 7361 626c  claims licensabl
-0001f700: 6520 2020 2020 2020 2020 2020 7c0a 7c20  e           |.| 
+0001f6c0: 7265 7375 6c74 206f 6620 7468 6973 204c  result of this L
+0001f6d0: 6963 656e 7365 206f 7220 6f75 7420 6f66  icense or out of
+0001f6e0: 2074 6865 2075 7365 206f 7220 696e 6162   the use or inab
+0001f6f0: 696c 6974 7920 746f 2075 7365 2074 6865  ility to use the
+0001f700: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 0001f710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f720: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-0001f730: 2020 2020 2020 2020 6279 2073 7563 6820          by such 
-0001f740: 436f 6e74 7269 6275 746f 7220 7468 6174  Contributor that
-0001f750: 2061 7265 206e 6563 6573 7361 7269 6c79   are necessarily
-0001f760: 2069 6e66 7269 6e67 6564 2062 7920 7468   infringed by th
-0001f770: 6569 7220 2020 2020 2020 2020 2020 2020  eir             
-0001f780: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-0001f790: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-0001f7a0: 2020 2020 2020 2020 2020 2043 6f6e 7472             Contr
-0001f7b0: 6962 7574 696f 6e28 7329 2061 6c6f 6e65  ibution(s) alone
-0001f7c0: 206f 7220 6279 2063 6f6d 6269 6e61 7469   or by combinati
-0001f7d0: 6f6e 206f 6620 7468 6569 7220 436f 6e74  on of their Cont
-0001f7e0: 7269 6275 7469 6f6e 2873 2920 2020 2020  ribution(s)     
-0001f7f0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001f800: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-0001f810: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0001f820: 6974 6820 7468 6520 576f 726b 2074 6f20  ith the Work to 
-0001f830: 7768 6963 6820 7375 6368 2043 6f6e 7472  which such Contr
-0001f840: 6962 7574 696f 6e28 7329 2077 6173 2073  ibution(s) was s
-0001f850: 7562 6d69 7474 6564 2e20 4966 2059 6f75  ubmitted. If You
-0001f860: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001f720: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+0001f730: 2020 2020 2057 6f72 6b20 2869 6e63 6c75       Work (inclu
+0001f740: 6469 6e67 2062 7574 206e 6f74 206c 696d  ding but not lim
+0001f750: 6974 6564 2074 6f20 6461 6d61 6765 7320  ited to damages 
+0001f760: 666f 7220 6c6f 7373 206f 6620 676f 6f64  for loss of good
+0001f770: 7769 6c6c 2c20 2020 2020 2020 2020 2020  will,           
+0001f780: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+0001f790: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+0001f7a0: 2020 2020 2020 2020 2020 2077 6f72 6b20             work 
+0001f7b0: 7374 6f70 7061 6765 2c20 636f 6d70 7574  stoppage, comput
+0001f7c0: 6572 2066 6169 6c75 7265 206f 7220 6d61  er failure or ma
+0001f7d0: 6c66 756e 6374 696f 6e2c 206f 7220 616e  lfunction, or an
+0001f7e0: 7920 616e 6420 616c 6c20 2020 2020 2020  y and all       
+0001f7f0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001f800: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+0001f810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f820: 6f74 6865 7220 636f 6d6d 6572 6369 616c  other commercial
+0001f830: 2064 616d 6167 6573 206f 7220 6c6f 7373   damages or loss
+0001f840: 6573 292c 2065 7665 6e20 6966 2073 7563  es), even if suc
+0001f850: 6820 436f 6e74 7269 6275 746f 7220 2020  h Contributor   
+0001f860: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f880: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-0001f890: 2020 2020 2020 2069 6e73 7469 7475 7465         institute
-0001f8a0: 2070 6174 656e 7420 6c69 7469 6761 7469   patent litigati
-0001f8b0: 6f6e 2061 6761 696e 7374 2061 6e79 2065  on against any e
-0001f8c0: 6e74 6974 7920 2869 6e63 6c75 6469 6e67  ntity (including
-0001f8d0: 2061 2020 2020 2020 2020 2020 2020 2020   a              
-0001f8e0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-0001f8f0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-0001f900: 2020 2020 2020 2020 2020 6372 6f73 732d            cross-
-0001f910: 636c 6169 6d20 6f72 2063 6f75 6e74 6572  claim or counter
-0001f920: 636c 6169 6d20 696e 2061 206c 6177 7375  claim in a lawsu
-0001f930: 6974 2920 616c 6c65 6769 6e67 2074 6861  it) alleging tha
-0001f940: 7420 7468 6520 576f 726b 2020 2020 2020  t the Work      
-0001f950: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-0001f960: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-0001f970: 2020 2020 2020 2020 2020 2020 2020 6f72                or
-0001f980: 2061 2043 6f6e 7472 6962 7574 696f 6e20   a Contribution 
-0001f990: 696e 636f 7270 6f72 6174 6564 2077 6974  incorporated wit
-0001f9a0: 6869 6e20 7468 6520 576f 726b 2063 6f6e  hin the Work con
-0001f9b0: 7374 6974 7574 6573 2064 6972 6563 7420  stitutes direct 
-0001f9c0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+0001f880: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+0001f890: 2020 2020 2020 2020 2020 6861 7320 6265            has be
+0001f8a0: 656e 2061 6476 6973 6564 206f 6620 7468  en advised of th
+0001f8b0: 6520 706f 7373 6962 696c 6974 7920 6f66  e possibility of
+0001f8c0: 2073 7563 6820 6461 6d61 6765 732e 2020   such damages.  
+0001f8d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001f8e0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+0001f8f0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+0001f900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f950: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+0001f960: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+0001f970: 2020 2020 2020 2020 2020 2039 2e20 4163             9. Ac
+0001f980: 6365 7074 696e 6720 5761 7272 616e 7479  cepting Warranty
+0001f990: 206f 7220 4164 6469 7469 6f6e 616c 204c   or Additional L
+0001f9a0: 6961 6269 6c69 7479 2e20 5768 696c 6520  iability. While 
+0001f9b0: 7265 6469 7374 7269 6275 7469 6e67 2020  redistributing  
+0001f9c0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 0001f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f9e0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-0001f9f0: 2020 2020 206f 7220 636f 6e74 7269 6275       or contribu
-0001fa00: 746f 7279 2070 6174 656e 7420 696e 6672  tory patent infr
-0001fa10: 696e 6765 6d65 6e74 2c20 7468 656e 2061  ingement, then a
-0001fa20: 6e79 2070 6174 656e 7420 6c69 6365 6e73  ny patent licens
-0001fa30: 6573 2020 2020 2020 2020 2020 2020 207c  es             |
-0001fa40: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-0001fa50: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-0001fa60: 2020 2020 2020 2020 2067 7261 6e74 6564           granted
-0001fa70: 2074 6f20 596f 7520 756e 6465 7220 7468   to You under th
-0001fa80: 6973 204c 6963 656e 7365 2066 6f72 2074  is License for t
-0001fa90: 6861 7420 576f 726b 2073 6861 6c6c 2074  hat Work shall t
-0001faa0: 6572 6d69 6e61 7465 2020 2020 2020 2020  erminate        
-0001fab0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-0001fac0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-0001fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fae0: 2020 2020 2020 2020 2020 6173 206f 6620            as of 
-0001faf0: 7468 6520 6461 7465 2073 7563 6820 6c69  the date such li
-0001fb00: 7469 6761 7469 6f6e 2069 7320 6669 6c65  tigation is file
-0001fb10: 642e 2020 2020 2020 2020 2020 2020 2020  d.              
-0001fb20: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-0001fb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb40: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001fb50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fb90: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-0001fba0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-0001fbb0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0001fbc0: 2020 2020 2020 342e 2052 6564 6973 7472        4. Redistr
-0001fbd0: 6962 7574 696f 6e2e 2059 6f75 206d 6179  ibution. You may
-0001fbe0: 2072 6570 726f 6475 6365 2061 6e64 2064   reproduce and d
-0001fbf0: 6973 7472 6962 7574 6520 636f 7069 6573  istribute copies
-0001fc00: 206f 6620 7468 6520 2020 2020 2020 2020   of the         
-0001fc10: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-0001fc20: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-0001fc30: 2020 2020 2020 2020 2020 2020 2057 6f72               Wor
-0001fc40: 6b20 6f72 2044 6572 6976 6174 6976 6520  k or Derivative 
-0001fc50: 576f 726b 7320 7468 6572 656f 6620 696e  Works thereof in
-0001fc60: 2061 6e79 206d 6564 6975 6d2c 2077 6974   any medium, wit
-0001fc70: 6820 6f72 2077 6974 686f 7574 2020 2020  h or without    
-0001fc80: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-0001fc90: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001f9e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001f9f0: 2020 2020 7468 6520 576f 726b 206f 7220      the Work or 
+0001fa00: 4465 7269 7661 7469 7665 2057 6f72 6b73  Derivative Works
+0001fa10: 2074 6865 7265 6f66 2c20 596f 7520 6d61   thereof, You ma
+0001fa20: 7920 6368 6f6f 7365 2074 6f20 6f66 6665  y choose to offe
+0001fa30: 722c 2020 2020 2020 2020 2020 2020 7c0a  r,            |.
+0001fa40: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+0001fa50: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+0001fa60: 2020 2020 2020 2061 6e64 2063 6861 7267         and charg
+0001fa70: 6520 6120 6665 6520 666f 722c 2061 6363  e a fee for, acc
+0001fa80: 6570 7461 6e63 6520 6f66 2073 7570 706f  eptance of suppo
+0001fa90: 7274 2c20 7761 7272 616e 7479 2c20 696e  rt, warranty, in
+0001faa0: 6465 6d6e 6974 792c 2020 2020 2020 2020  demnity,        
+0001fab0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+0001fac0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+0001fad0: 2020 2020 2020 2020 2020 2020 6f72 206f              or o
+0001fae0: 7468 6572 206c 6961 6269 6c69 7479 206f  ther liability o
+0001faf0: 626c 6967 6174 696f 6e73 2061 6e64 2f6f  bligations and/o
+0001fb00: 7220 7269 6768 7473 2063 6f6e 7369 7374  r rights consist
+0001fb10: 656e 7420 7769 7468 2074 6869 7320 2020  ent with this   
+0001fb20: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+0001fb30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+0001fb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fb50: 204c 6963 656e 7365 2e20 486f 7765 7665   License. Howeve
+0001fb60: 722c 2069 6e20 6163 6365 7074 696e 6720  r, in accepting 
+0001fb70: 7375 6368 206f 626c 6967 6174 696f 6e73  such obligations
+0001fb80: 2c20 596f 7520 6d61 7920 6163 7420 6f6e  , You may act on
+0001fb90: 6c79 2020 2020 2020 2020 2020 207c 0a7c  ly           |.|
+0001fba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fbb0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+0001fbc0: 2020 2020 2020 6f6e 2059 6f75 7220 6f77        on Your ow
+0001fbd0: 6e20 6265 6861 6c66 2061 6e64 206f 6e20  n behalf and on 
+0001fbe0: 596f 7572 2073 6f6c 6520 7265 7370 6f6e  Your sole respon
+0001fbf0: 7369 6269 6c69 7479 2c20 6e6f 7420 6f6e  sibility, not on
+0001fc00: 2062 6568 616c 6620 2020 2020 2020 2020   behalf         
+0001fc10: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+0001fc20: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+0001fc30: 2020 2020 2020 2020 2020 2020 206f 6620               of 
+0001fc40: 616e 7920 6f74 6865 7220 436f 6e74 7269  any other Contri
+0001fc50: 6275 746f 722c 2061 6e64 206f 6e6c 7920  butor, and only 
+0001fc60: 6966 2059 6f75 2061 6772 6565 2074 6f20  if You agree to 
+0001fc70: 696e 6465 6d6e 6966 792c 2020 2020 2020  indemnify,      
+0001fc80: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+0001fc90: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 0001fca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fcb0: 2020 206d 6f64 6966 6963 6174 696f 6e73     modifications
-0001fcc0: 2c20 616e 6420 696e 2053 6f75 7263 6520  , and in Source 
-0001fcd0: 6f72 204f 626a 6563 7420 666f 726d 2c20  or Object form, 
-0001fce0: 7072 6f76 6964 6564 2074 6861 7420 596f  provided that Yo
-0001fcf0: 7520 2020 2020 2020 2020 2020 207c 0a7c  u            |.|
+0001fcb0: 2020 2064 6566 656e 642c 2061 6e64 2068     defend, and h
+0001fcc0: 6f6c 6420 6561 6368 2043 6f6e 7472 6962  old each Contrib
+0001fcd0: 7574 6f72 2068 6172 6d6c 6573 7320 666f  utor harmless fo
+0001fce0: 7220 616e 7920 6c69 6162 696c 6974 7920  r any liability 
+0001fcf0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 0001fd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd10: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-0001fd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd30: 2020 2020 2020 2020 6d65 6574 2074 6865          meet the
-0001fd40: 2066 6f6c 6c6f 7769 6e67 2063 6f6e 6469   following condi
-0001fd50: 7469 6f6e 733a 2020 2020 2020 2020 2020  tions:          
-0001fd60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fd70: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-0001fd80: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-0001fd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fda0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fdb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fdd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fde0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-0001fdf0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+0001fd10: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+0001fd20: 2020 2020 696e 6375 7272 6564 2062 792c      incurred by,
+0001fd30: 206f 7220 636c 6169 6d73 2061 7373 6572   or claims asser
+0001fd40: 7465 6420 6167 6169 6e73 742c 2073 7563  ted against, suc
+0001fd50: 6820 436f 6e74 7269 6275 746f 7220 6279  h Contributor by
+0001fd60: 2072 6561 736f 6e20 2020 2020 2020 2020   reason         
+0001fd70: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+0001fd80: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+0001fd90: 2020 2020 2020 2020 2020 2020 206f 6620               of 
+0001fda0: 796f 7572 2061 6363 6570 7469 6e67 2061  your accepting a
+0001fdb0: 6e79 2073 7563 6820 7761 7272 616e 7479  ny such warranty
+0001fdc0: 206f 7220 6164 6469 7469 6f6e 616c 206c   or additional l
+0001fdd0: 6961 6269 6c69 7479 2e20 2020 2020 2020  iability.       
+0001fde0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+0001fdf0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 0001fe00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fe10: 2020 2020 2020 2861 2920 596f 7520 6d75        (a) You mu
-0001fe20: 7374 2067 6976 6520 616e 7920 6f74 6865  st give any othe
-0001fe30: 7220 7265 6369 7069 656e 7473 206f 6620  r recipients of 
-0001fe40: 7468 6520 576f 726b 206f 7220 2020 2020  the Work or     
-0001fe50: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-0001fe60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fe70: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-0001fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fe90: 2020 4465 7269 7661 7469 7665 2057 6f72    Derivative Wor
-0001fea0: 6b73 2061 2063 6f70 7920 6f66 2074 6869  ks a copy of thi
-0001feb0: 7320 4c69 6365 6e73 653b 2061 6e64 2020  s License; and  
-0001fec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fed0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-0001fee0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+0001fe10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fe20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fe30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fe40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fe50: 2020 2020 2020 2020 2020 207c 0a2b 2d2d             |.+--
+0001fe60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001fe70: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+0001fe80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001fe90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001fea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001feb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001fec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+0001fed0: 2b0a 7c20 2020 2020 2072 7374 3261 6e73  +.|      rst2ans
+0001fee0: 6920 2020 2020 207c 2020 2020 2020 2020  i      |        
 0001fef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ff00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ff10: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ff20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ff30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff40: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-0001ff50: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+0001ff40: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+0001ff50: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 0001ff60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ff70: 2862 2920 596f 7520 6d75 7374 2063 6175  (b) You must cau
-0001ff80: 7365 2061 6e79 206d 6f64 6966 6965 6420  se any modified 
-0001ff90: 6669 6c65 7320 746f 2063 6172 7279 2070  files to carry p
-0001ffa0: 726f 6d69 6e65 6e74 206e 6f74 6963 6573  rominent notices
-0001ffb0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+0001ff70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ff80: 2054 6865 204d 4954 204c 6963 656e 7365   The MIT License
+0001ff90: 2028 4d49 5429 2020 2020 2020 2020 2020   (MIT)          
+0001ffa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ffb0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 0001ffc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ffd0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+0001ffd0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
 0001ffe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fff0: 2020 2073 7461 7469 6e67 2074 6861 7420     stating that 
-00020000: 596f 7520 6368 616e 6765 6420 7468 6520  You changed the 
-00020010: 6669 6c65 733b 2061 6e64 2020 2020 2020  files; and      
-00020020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020030: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00020040: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00020050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001fff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020020: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00020030: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00020040: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00020050: 2020 2020 2043 6f70 7972 6967 6874 20c2       Copyright .
+00020060: a920 3230 3135 2d32 3031 3620 4672 616e  . 2015-2016 Fran
+00020070: 6b6c 696e 2022 536e 6169 7065 2220 4d61  klin "Snaipe" Ma
+00020080: 7468 6965 7520 3c68 7474 703a 2f2f 736e  thieu <http://sn
+00020090: 6169 2e70 652f 3e20 2020 2020 2020 2020  ai.pe/>         
 000200a0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 000200b0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000200c0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000200d0: 6329 2059 6f75 206d 7573 7420 7265 7461  c) You must reta
-000200e0: 696e 2c20 696e 2074 6865 2053 6f75 7263  in, in the Sourc
-000200f0: 6520 666f 726d 206f 6620 616e 7920 4465  e form of any De
-00020100: 7269 7661 7469 7665 2057 6f72 6b73 2020  rivative Works  
+000200c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000200d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000200e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000200f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020110: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00020120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020130: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00020140: 2020 2020 2020 2020 2074 6861 7420 596f           that Yo
-00020150: 7520 6469 7374 7269 6275 7465 2c20 616c  u distribute, al
-00020160: 6c20 636f 7079 7269 6768 742c 2070 6174  l copyright, pat
-00020170: 656e 742c 2074 7261 6465 6d61 726b 2c20  ent, trademark, 
-00020180: 616e 6420 2020 2020 2020 2020 2020 207c  and            |
+00020130: 207c 2020 2020 2020 2020 2050 6572 6d69   |         Permi
+00020140: 7373 696f 6e20 6973 2068 6572 6562 7920  ssion is hereby 
+00020150: 6772 616e 7465 642c 2066 7265 6520 6f66  granted, free of
+00020160: 2063 6861 7267 652c 2074 6f20 616e 7920   charge, to any 
+00020170: 7065 7273 6f6e 206f 6274 6169 6e69 6e67  person obtaining
+00020180: 2061 2063 6f70 7920 2020 2020 2020 207c   a copy        |
 00020190: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-000201a0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000201b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000201c0: 6174 7472 6962 7574 696f 6e20 6e6f 7469  attribution noti
-000201d0: 6365 7320 6672 6f6d 2074 6865 2053 6f75  ces from the Sou
-000201e0: 7263 6520 666f 726d 206f 6620 7468 6520  rce form of the 
-000201f0: 576f 726b 2c20 2020 2020 2020 2020 2020  Work,           
+000201a0: 2020 2020 2020 7c20 2020 2020 2020 206f        |        o
+000201b0: 6620 7468 6973 2073 6f66 7477 6172 6520  f this software 
+000201c0: 616e 6420 6173 736f 6369 6174 6564 2064  and associated d
+000201d0: 6f63 756d 656e 7461 7469 6f6e 2066 696c  ocumentation fil
+000201e0: 6573 2028 7468 6520 2253 6f66 7477 6172  es (the "Softwar
+000201f0: 6522 292c 2074 6f20 6465 616c 2020 2020  e"), to deal    
 00020200: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00020210: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00020220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020230: 2020 2065 7863 6c75 6469 6e67 2074 686f     excluding tho
-00020240: 7365 206e 6f74 6963 6573 2074 6861 7420  se notices that 
-00020250: 646f 206e 6f74 2070 6572 7461 696e 2074  do not pertain t
-00020260: 6f20 616e 7920 7061 7274 206f 6620 2020  o any part of   
-00020270: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+00020220: 2020 2020 2069 6e20 7468 6520 536f 6674       in the Soft
+00020230: 7761 7265 2077 6974 686f 7574 2072 6573  ware without res
+00020240: 7472 6963 7469 6f6e 2c20 696e 636c 7564  triction, includ
+00020250: 696e 6720 7769 7468 6f75 7420 6c69 6d69  ing without limi
+00020260: 7461 7469 6f6e 2074 6865 2072 6967 6874  tation the right
+00020270: 7320 2020 2020 2020 207c 0a7c 2020 2020  s        |.|    
 00020280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020290: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000202a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000202b0: 2020 2020 2020 2020 7468 6520 4465 7269          the Deri
-000202c0: 7661 7469 7665 2057 6f72 6b73 3b20 616e  vative Works; an
-000202d0: 6420 2020 2020 2020 2020 2020 2020 2020  d               
-000202e0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00020290: 7c20 2020 2020 2020 2020 2074 6f20 7573  |          to us
+000202a0: 652c 2063 6f70 792c 206d 6f64 6966 792c  e, copy, modify,
+000202b0: 206d 6572 6765 2c20 7075 626c 6973 682c   merge, publish,
+000202c0: 2064 6973 7472 6962 7574 652c 2073 7562   distribute, sub
+000202d0: 6c69 6365 6e73 652c 2061 6e64 2f6f 7220  license, and/or 
+000202e0: 7365 6c6c 2020 2020 2020 2020 2020 7c0a  sell          |.
 000202f0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00020300: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00020310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020310: 2020 636f 7069 6573 206f 6620 7468 6520    copies of the 
+00020320: 536f 6674 7761 7265 2c20 616e 6420 746f  Software, and to
+00020330: 2070 6572 6d69 7420 7065 7273 6f6e 7320   permit persons 
+00020340: 746f 2077 686f 6d20 7468 6520 536f 6674  to whom the Soft
+00020350: 7761 7265 2069 7320 2020 2020 2020 2020  ware is         
 00020360: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00020370: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00020380: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-00020390: 6429 2049 6620 7468 6520 576f 726b 2069  d) If the Work i
-000203a0: 6e63 6c75 6465 7320 6120 224e 4f54 4943  ncludes a "NOTIC
-000203b0: 4522 2074 6578 7420 6669 6c65 2061 7320  E" text file as 
-000203c0: 7061 7274 206f 6620 6974 7320 2020 2020  part of its     
+00020380: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+00020390: 726e 6973 6865 6420 746f 2064 6f20 736f  rnished to do so
+000203a0: 2c20 7375 626a 6563 7420 746f 2074 6865  , subject to the
+000203b0: 2066 6f6c 6c6f 7769 6e67 2063 6f6e 6469   following condi
+000203c0: 7469 6f6e 733a 2020 2020 2020 2020 2020  tions:          
 000203d0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 000203e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 000203f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020400: 2020 2020 6469 7374 7269 6275 7469 6f6e      distribution
-00020410: 2c20 7468 656e 2061 6e79 2044 6572 6976  , then any Deriv
-00020420: 6174 6976 6520 576f 726b 7320 7468 6174  ative Works that
-00020430: 2059 6f75 2064 6973 7472 6962 7574 6520   You distribute 
-00020440: 6d75 7374 2020 2020 2020 2020 207c 0a7c  must         |.|
+00020400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020440: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00020450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020460: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00020470: 2020 2020 2020 2020 2020 2069 6e63 6c75             inclu
-00020480: 6465 2061 2072 6561 6461 626c 6520 636f  de a readable co
-00020490: 7079 206f 6620 7468 6520 6174 7472 6962  py of the attrib
-000204a0: 7574 696f 6e20 6e6f 7469 6365 7320 636f  ution notices co
-000204b0: 6e74 6169 6e65 6420 2020 2020 2020 2020  ntained         
+00020460: 2020 2020 7c20 2020 2020 2020 2020 2054      |          T
+00020470: 6865 2061 626f 7665 2063 6f70 7972 6967  he above copyrig
+00020480: 6874 206e 6f74 6963 6520 616e 6420 7468  ht notice and th
+00020490: 6973 2070 6572 6d69 7373 696f 6e20 6e6f  is permission no
+000204a0: 7469 6365 2073 6861 6c6c 2062 6520 696e  tice shall be in
+000204b0: 636c 7564 6564 2069 6e20 2020 2020 2020  cluded in       
 000204c0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 000204d0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000204e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000204f0: 7769 7468 696e 2073 7563 6820 4e4f 5449  within such NOTI
-00020500: 4345 2066 696c 652c 2065 7863 6c75 6469  CE file, excludi
-00020510: 6e67 2074 686f 7365 206e 6f74 6963 6573  ng those notices
-00020520: 2074 6861 7420 646f 206e 6f74 2020 2020   that do not    
+000204e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+000204f0: 6c6c 2063 6f70 6965 7320 6f72 2073 7562  ll copies or sub
+00020500: 7374 616e 7469 616c 2070 6f72 7469 6f6e  stantial portion
+00020510: 7320 6f66 2074 6865 2053 6f66 7477 6172  s of the Softwar
+00020520: 652e 2020 2020 2020 2020 2020 2020 2020  e.              
 00020530: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00020540: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 00020550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020560: 2020 2020 2070 6572 7461 696e 2074 6f20       pertain to 
-00020570: 616e 7920 7061 7274 206f 6620 7468 6520  any part of the 
-00020580: 4465 7269 7661 7469 7665 2057 6f72 6b73  Derivative Works
-00020590: 2c20 696e 2061 7420 6c65 6173 7420 6f6e  , in at least on
-000205a0: 6520 2020 2020 2020 2020 2020 7c0a 7c20  e           |.| 
+00020560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000205a0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 000205b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000205c0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-000205d0: 2020 2020 2020 2020 206f 6620 7468 6520           of the 
-000205e0: 666f 6c6c 6f77 696e 6720 706c 6163 6573  following places
-000205f0: 3a20 7769 7468 696e 2061 204e 4f54 4943  : within a NOTIC
-00020600: 4520 7465 7874 2066 696c 6520 6469 7374  E text file dist
-00020610: 7269 6275 7465 6420 2020 2020 2020 2020  ributed         
+000205c0: 2020 207c 2020 2020 2020 2020 2020 5448     |          TH
+000205d0: 4520 534f 4654 5741 5245 2049 5320 5052  E SOFTWARE IS PR
+000205e0: 4f56 4944 4544 2022 4153 2049 5322 2c20  OVIDED "AS IS", 
+000205f0: 5749 5448 4f55 5420 5741 5252 414e 5459  WITHOUT WARRANTY
+00020600: 204f 4620 414e 5920 4b49 4e44 2c20 4558   OF ANY KIND, EX
+00020610: 5052 4553 5320 4f52 2020 2020 2020 2020  PRESS OR        
 00020620: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00020630: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00020640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020650: 6173 2070 6172 7420 6f66 2074 6865 2044  as part of the D
-00020660: 6572 6976 6174 6976 6520 576f 726b 733b  erivative Works;
-00020670: 2077 6974 6869 6e20 7468 6520 536f 7572   within the Sour
-00020680: 6365 2066 6f72 6d20 6f72 2020 2020 2020  ce form or      
+00020640: 2020 2020 494d 504c 4945 442c 2049 4e43      IMPLIED, INC
+00020650: 4c55 4449 4e47 2042 5554 204e 4f54 204c  LUDING BUT NOT L
+00020660: 494d 4954 4544 2054 4f20 5448 4520 5741  IMITED TO THE WA
+00020670: 5252 414e 5449 4553 204f 4620 4d45 5243  RRANTIES OF MERC
+00020680: 4841 4e54 4142 494c 4954 592c 2020 2020  HANTABILITY,    
 00020690: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 000206a0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-000206b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000206c0: 2020 646f 6375 6d65 6e74 6174 696f 6e2c    documentation,
-000206d0: 2069 6620 7072 6f76 6964 6564 2061 6c6f   if provided alo
-000206e0: 6e67 2077 6974 6820 7468 6520 4465 7269  ng with the Deri
-000206f0: 7661 7469 7665 2057 6f72 6b73 3b20 6f72  vative Works; or
-00020700: 2c20 2020 2020 2020 2020 207c 0a7c 2020  ,          |.|  
+000206b0: 2020 2020 2020 2046 4954 4e45 5353 2046         FITNESS F
+000206c0: 4f52 2041 2050 4152 5449 4355 4c41 5220  OR A PARTICULAR 
+000206d0: 5055 5250 4f53 4520 414e 4420 4e4f 4e49  PURPOSE AND NONI
+000206e0: 4e46 5249 4e47 454d 454e 542e 2049 4e20  NFRINGEMENT. IN 
+000206f0: 4e4f 2045 5645 4e54 2053 4841 4c4c 2054  NO EVENT SHALL T
+00020700: 4845 2020 2020 2020 2020 207c 0a7c 2020  HE         |.|  
 00020710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020720: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00020730: 2020 2020 2020 2020 2020 7769 7468 696e            within
-00020740: 2061 2064 6973 706c 6179 2067 656e 6572   a display gener
-00020750: 6174 6564 2062 7920 7468 6520 4465 7269  ated by the Deri
-00020760: 7661 7469 7665 2057 6f72 6b73 2c20 6966  vative Works, if
-00020770: 2061 6e64 2020 2020 2020 2020 2020 2020   and            
+00020720: 2020 7c20 2020 2020 2020 2020 2020 2041    |            A
+00020730: 5554 484f 5253 204f 5220 434f 5059 5249  UTHORS OR COPYRI
+00020740: 4748 5420 484f 4c44 4552 5320 4245 204c  GHT HOLDERS BE L
+00020750: 4941 424c 4520 464f 5220 414e 5920 434c  IABLE FOR ANY CL
+00020760: 4149 4d2c 2044 414d 4147 4553 204f 5220  AIM, DAMAGES OR 
+00020770: 4f54 4845 5220 2020 2020 2020 2020 2020  OTHER           
 00020780: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00020790: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-000207a0: 2020 2020 2020 2020 2020 2020 7768 6572              wher
-000207b0: 6576 6572 2073 7563 6820 7468 6972 642d  ever such third-
-000207c0: 7061 7274 7920 6e6f 7469 6365 7320 6e6f  party notices no
-000207d0: 726d 616c 6c79 2061 7070 6561 722e 2054  rmally appear. T
-000207e0: 6865 2063 6f6e 7465 6e74 7320 2020 2020  he contents     
+000207a0: 4c49 4142 494c 4954 592c 2057 4845 5448  LIABILITY, WHETH
+000207b0: 4552 2049 4e20 414e 2041 4354 494f 4e20  ER IN AN ACTION 
+000207c0: 4f46 2043 4f4e 5452 4143 542c 2054 4f52  OF CONTRACT, TOR
+000207d0: 5420 4f52 204f 5448 4552 5749 5345 2c20  T OR OTHERWISE, 
+000207e0: 4152 4953 494e 4720 4652 4f4d 2c20 2020  ARISING FROM,   
 000207f0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00020800: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00020810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020820: 2020 2020 6f66 2074 6865 204e 4f54 4943      of the NOTIC
-00020830: 4520 6669 6c65 2061 7265 2066 6f72 2069  E file are for i
-00020840: 6e66 6f72 6d61 7469 6f6e 616c 2070 7572  nformational pur
-00020850: 706f 7365 7320 6f6e 6c79 2061 6e64 2020  poses only and  
+00020810: 2020 2020 2020 204f 5554 204f 4620 4f52         OUT OF OR
+00020820: 2049 4e20 434f 4e4e 4543 5449 4f4e 2057   IN CONNECTION W
+00020830: 4954 4820 5448 4520 534f 4654 5741 5245  ITH THE SOFTWARE
+00020840: 204f 5220 5448 4520 5553 4520 4f52 204f   OR THE USE OR O
+00020850: 5448 4552 2044 4541 4c49 4e47 5320 494e  THER DEALINGS IN
 00020860: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00020870: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020880: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00020890: 2020 2020 2020 2020 646f 206e 6f74 206d          do not m
-000208a0: 6f64 6966 7920 7468 6520 4c69 6365 6e73  odify the Licens
-000208b0: 652e 2059 6f75 206d 6179 2061 6464 2059  e. You may add Y
-000208c0: 6f75 7220 6f77 6e20 6174 7472 6962 7574  our own attribut
-000208d0: 696f 6e20 2020 2020 2020 2020 2020 207c  ion            |
+00020890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000208a0: 2020 2020 2020 2020 2020 5448 4520 534f            THE SO
+000208b0: 4654 5741 5245 2e20 2020 2020 2020 2020  FTWARE.         
+000208c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000208d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 000208e0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 000208f0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00020900: 2020 2020 2020 2020 2020 2020 6e6f 7469              noti
-00020910: 6365 7320 7769 7468 696e 2044 6572 6976  ces within Deriv
-00020920: 6174 6976 6520 576f 726b 7320 7468 6174  ative Works that
-00020930: 2059 6f75 2064 6973 7472 6962 7574 652c   You distribute,
-00020940: 2061 6c6f 6e67 7369 6465 2020 2020 2020   alongside      
-00020950: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00020960: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00020970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020980: 2020 6f72 2061 7320 616e 2061 6464 656e    or as an adden
-00020990: 6475 6d20 746f 2074 6865 204e 4f54 4943  dum to the NOTIC
-000209a0: 4520 7465 7874 2066 726f 6d20 7468 6520  E text from the 
-000209b0: 576f 726b 2c20 7072 6f76 6964 6564 2020  Work, provided  
-000209c0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-000209d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020920: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020950: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
+00020960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00020970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00020980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00020990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000209a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000209b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000209c0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020  ---------+.|    
+000209d0: 2020 2020 7369 7820 2020 2020 2020 2020      six         
 000209e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000209f0: 2020 2020 2020 2074 6861 7420 7375 6368         that such
-00020a00: 2061 6464 6974 696f 6e61 6c20 6174 7472   additional attr
-00020a10: 6962 7574 696f 6e20 6e6f 7469 6365 7320  ibution notices 
-00020a20: 6361 6e6e 6f74 2062 6520 636f 6e73 7472  cannot be constr
-00020a30: 7565 6420 2020 2020 2020 2020 2020 7c0a  ued           |.
+000209f0: 2020 2020 2020 2020 2020 2043 6f70 7972             Copyr
+00020a00: 6967 6874 2028 6329 2032 3031 302d 3230  ight (c) 2010-20
+00020a10: 3230 2042 656e 6a61 6d69 6e20 5065 7465  20 Benjamin Pete
+00020a20: 7273 6f6e 2020 2020 2020 2020 2020 2020  rson            
+00020a30: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00020a40: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00020a50: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 00020a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020a70: 2020 2020 2020 2020 2020 2020 2061 7320               as 
-00020a80: 6d6f 6469 6679 696e 6720 7468 6520 4c69  modifying the Li
-00020a90: 6365 6e73 652e 2020 2020 2020 2020 2020  cense.          
+00020a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020ab0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00020ac0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00020ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b20: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+00020ad0: 2020 5065 726d 6973 7369 6f6e 2069 7320    Permission is 
+00020ae0: 6865 7265 6279 2067 7261 6e74 6564 2c20  hereby granted, 
+00020af0: 6672 6565 206f 6620 6368 6172 6765 2c20  free of charge, 
+00020b00: 746f 2061 6e79 2070 6572 736f 6e20 6f62  to any person ob
+00020b10: 7461 696e 696e 6720 6120 636f 7079 206f  taining a copy o
+00020b20: 6620 2020 2020 2020 7c0a 7c20 2020 2020  f       |.|     
 00020b30: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00020b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020b50: 2059 6f75 206d 6179 2061 6464 2059 6f75   You may add You
-00020b60: 7220 6f77 6e20 636f 7079 7269 6768 7420  r own copyright 
-00020b70: 7374 6174 656d 656e 7420 746f 2059 6f75  statement to You
-00020b80: 7220 6d6f 6469 6669 6361 7469 6f6e 7320  r modifications 
-00020b90: 616e 6420 2020 2020 2020 2020 207c 0a7c  and          |.|
+00020b40: 2020 2020 2020 2020 7468 6973 2073 6f66          this sof
+00020b50: 7477 6172 6520 616e 6420 6173 736f 6369  tware and associ
+00020b60: 6174 6564 2064 6f63 756d 656e 7461 7469  ated documentati
+00020b70: 6f6e 2066 696c 6573 2028 7468 6520 2253  on files (the "S
+00020b80: 6f66 7477 6172 6522 292c 2074 6f20 6465  oftware"), to de
+00020b90: 616c 2069 6e20 2020 2020 2020 207c 0a7c  al in        |.|
 00020ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020bb0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00020bc0: 2020 2020 2020 206d 6179 2070 726f 7669         may provi
-00020bd0: 6465 2061 6464 6974 696f 6e61 6c20 6f72  de additional or
-00020be0: 2064 6966 6665 7265 6e74 206c 6963 656e   different licen
-00020bf0: 7365 2074 6572 6d73 2061 6e64 2063 6f6e  se terms and con
-00020c00: 6469 7469 6f6e 7320 2020 2020 2020 2020  ditions         
+00020bb0: 2020 2020 7c20 2020 2020 2020 2020 7468      |         th
+00020bc0: 6520 536f 6674 7761 7265 2077 6974 686f  e Software witho
+00020bd0: 7574 2072 6573 7472 6963 7469 6f6e 2c20  ut restriction, 
+00020be0: 696e 636c 7564 696e 6720 7769 7468 6f75  including withou
+00020bf0: 7420 6c69 6d69 7461 7469 6f6e 2074 6865  t limitation the
+00020c00: 2072 6967 6874 7320 746f 2020 2020 2020   rights to      
 00020c10: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00020c20: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00020c30: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00020c40: 7573 652c 2072 6570 726f 6475 6374 696f  use, reproductio
-00020c50: 6e2c 206f 7220 6469 7374 7269 6275 7469  n, or distributi
-00020c60: 6f6e 206f 6620 596f 7572 206d 6f64 6966  on of Your modif
-00020c70: 6963 6174 696f 6e73 2c20 6f72 2020 2020  ications, or    
-00020c80: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+00020c30: 2075 7365 2c20 636f 7079 2c20 6d6f 6469   use, copy, modi
+00020c40: 6679 2c20 6d65 7267 652c 2070 7562 6c69  fy, merge, publi
+00020c50: 7368 2c20 6469 7374 7269 6275 7465 2c20  sh, distribute, 
+00020c60: 7375 626c 6963 656e 7365 2c20 616e 642f  sublicense, and/
+00020c70: 6f72 2073 656c 6c20 636f 7069 6573 206f  or sell copies o
+00020c80: 6620 2020 2020 207c 0a7c 2020 2020 2020  f      |.|      
 00020c90: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00020ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020cb0: 2020 2066 6f72 2061 6e79 2073 7563 6820     for any such 
-00020cc0: 4465 7269 7661 7469 7665 2057 6f72 6b73  Derivative Works
-00020cd0: 2061 7320 6120 7768 6f6c 652c 2070 726f   as a whole, pro
-00020ce0: 7669 6465 6420 596f 7572 2075 7365 2c20  vided Your use, 
-00020cf0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00020ca0: 2020 2020 2020 7468 6520 536f 6674 7761        the Softwa
+00020cb0: 7265 2c20 616e 6420 746f 2070 6572 6d69  re, and to permi
+00020cc0: 7420 7065 7273 6f6e 7320 746f 2077 686f  t persons to who
+00020cd0: 6d20 7468 6520 536f 6674 7761 7265 2069  m the Software i
+00020ce0: 7320 6675 726e 6973 6865 6420 746f 2064  s furnished to d
+00020cf0: 6f20 736f 2c20 2020 2020 2020 7c0a 7c20  o so,       |.| 
 00020d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020d10: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00020d20: 2020 2020 2072 6570 726f 6475 6374 696f       reproductio
-00020d30: 6e2c 2061 6e64 2064 6973 7472 6962 7574  n, and distribut
-00020d40: 696f 6e20 6f66 2074 6865 2057 6f72 6b20  ion of the Work 
-00020d50: 6f74 6865 7277 6973 6520 636f 6d70 6c69  otherwise compli
-00020d60: 6573 2077 6974 6820 2020 2020 2020 2020  es with         
+00020d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020d30: 2073 7562 6a65 6374 2074 6f20 7468 6520   subject to the 
+00020d40: 666f 6c6c 6f77 696e 6720 636f 6e64 6974  following condit
+00020d50: 696f 6e73 3a20 2020 2020 2020 2020 2020  ions:           
+00020d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020d70: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00020d80: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
 00020d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020da0: 2020 2020 2020 2020 7468 6520 636f 6e64          the cond
-00020db0: 6974 696f 6e73 2073 7461 7465 6420 696e  itions stated in
-00020dc0: 2074 6869 7320 4c69 6365 6e73 652e 2020   this License.  
+00020da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020de0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00020df0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00020e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020e50: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00020e00: 2020 2020 2020 5468 6520 6162 6f76 6520        The above 
+00020e10: 636f 7079 7269 6768 7420 6e6f 7469 6365  copyright notice
+00020e20: 2061 6e64 2074 6869 7320 7065 726d 6973   and this permis
+00020e30: 7369 6f6e 206e 6f74 6963 6520 7368 616c  sion notice shal
+00020e40: 6c20 6265 2069 6e63 6c75 6465 6420 696e  l be included in
+00020e50: 2061 6c6c 2020 2020 2020 207c 0a7c 2020   all       |.|  
 00020e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020e70: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00020e80: 352e 2053 7562 6d69 7373 696f 6e20 6f66  5. Submission of
-00020e90: 2043 6f6e 7472 6962 7574 696f 6e73 2e20   Contributions. 
-00020ea0: 556e 6c65 7373 2059 6f75 2065 7870 6c69  Unless You expli
-00020eb0: 6369 746c 7920 7374 6174 6520 6f74 6865  citly state othe
-00020ec0: 7277 6973 652c 2020 2020 2020 2020 2020  rwise,          
+00020e80: 2020 2020 2020 2020 2020 636f 7069 6573            copies
+00020e90: 206f 7220 7375 6273 7461 6e74 6961 6c20   or substantial 
+00020ea0: 706f 7274 696f 6e73 206f 6620 7468 6520  portions of the 
+00020eb0: 536f 6674 7761 7265 2e20 2020 2020 2020  Software.       
+00020ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020ed0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00020ee0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00020ef0: 2020 2020 2020 2020 2061 6e79 2043 6f6e           any Con
-00020f00: 7472 6962 7574 696f 6e20 696e 7465 6e74  tribution intent
-00020f10: 696f 6e61 6c6c 7920 7375 626d 6974 7465  ionally submitte
-00020f20: 6420 666f 7220 696e 636c 7573 696f 6e20  d for inclusion 
-00020f30: 696e 2074 6865 2057 6f72 6b20 2020 2020  in the Work     
+00020ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00020f40: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00020f50: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00020f60: 2020 2020 2020 2020 2020 2020 2020 6279                by
-00020f70: 2059 6f75 2074 6f20 7468 6520 4c69 6365   You to the Lice
-00020f80: 6e73 6f72 2073 6861 6c6c 2062 6520 756e  nsor shall be un
-00020f90: 6465 7220 7468 6520 7465 726d 7320 616e  der the terms an
-00020fa0: 6420 636f 6e64 6974 696f 6e73 206f 6620  d conditions of 
-00020fb0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
+00020f60: 2020 2020 2020 2054 4845 2053 4f46 5457         THE SOFTW
+00020f70: 4152 4520 4953 2050 524f 5649 4445 4420  ARE IS PROVIDED 
+00020f80: 2241 5320 4953 222c 2057 4954 484f 5554  "AS IS", WITHOUT
+00020f90: 2057 4152 5241 4e54 5920 4f46 2041 4e59   WARRANTY OF ANY
+00020fa0: 204b 494e 442c 2045 5850 5245 5353 204f   KIND, EXPRESS O
+00020fb0: 5220 2020 2020 2020 2020 7c0a 7c20 2020  R         |.|   
 00020fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00020fd0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00020fe0: 2020 2020 2020 2074 6869 7320 4c69 6365         this Lice
-00020ff0: 6e73 652c 2077 6974 686f 7574 2061 6e79  nse, without any
-00021000: 2061 6464 6974 696f 6e61 6c20 7465 726d   additional term
-00021010: 7320 6f72 2063 6f6e 6469 7469 6f6e 732e  s or conditions.
-00021020: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00020fd0: 207c 2020 2020 2020 2049 4d50 4c49 4544   |       IMPLIED
+00020fe0: 2c20 494e 434c 5544 494e 4720 4255 5420  , INCLUDING BUT 
+00020ff0: 4e4f 5420 4c49 4d49 5445 4420 544f 2054  NOT LIMITED TO T
+00021000: 4845 2057 4152 5241 4e54 4945 5320 4f46  HE WARRANTIES OF
+00021010: 204d 4552 4348 414e 5441 4249 4c49 5459   MERCHANTABILITY
+00021020: 2c20 4649 544e 4553 5320 2020 2020 207c  , FITNESS      |
 00021030: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00021040: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00021050: 2020 2020 2020 204e 6f74 7769 7468 7374         Notwithst
-00021060: 616e 6469 6e67 2074 6865 2061 626f 7665  anding the above
-00021070: 2c20 6e6f 7468 696e 6720 6865 7265 696e  , nothing herein
-00021080: 2073 6861 6c6c 2073 7570 6572 7365 6465   shall supersede
-00021090: 206f 7220 6d6f 6469 6679 2020 2020 2020   or modify      
+00021040: 2020 2020 2020 7c20 2020 2020 2020 2046        |        F
+00021050: 4f52 2041 2050 4152 5449 4355 4c41 5220  OR A PARTICULAR 
+00021060: 5055 5250 4f53 4520 414e 4420 4e4f 4e49  PURPOSE AND NONI
+00021070: 4e46 5249 4e47 454d 454e 542e 2049 4e20  NFRINGEMENT. IN 
+00021080: 4e4f 2045 5645 4e54 2053 4841 4c4c 2054  NO EVENT SHALL T
+00021090: 4845 2041 5554 484f 5253 204f 5220 2020  HE AUTHORS OR   
 000210a0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 000210b0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000210c0: 2020 2020 2020 2020 2020 2020 2074 6865               the
-000210d0: 2074 6572 6d73 206f 6620 616e 7920 7365   terms of any se
-000210e0: 7061 7261 7465 206c 6963 656e 7365 2061  parate license a
-000210f0: 6772 6565 6d65 6e74 2079 6f75 206d 6179  greement you may
-00021100: 2068 6176 6520 6578 6563 7574 6564 2020   have executed  
-00021110: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+000210c0: 2020 2020 434f 5059 5249 4748 5420 484f      COPYRIGHT HO
+000210d0: 4c44 4552 5320 4245 204c 4941 424c 4520  LDERS BE LIABLE 
+000210e0: 464f 5220 414e 5920 434c 4149 4d2c 2044  FOR ANY CLAIM, D
+000210f0: 414d 4147 4553 204f 5220 4f54 4845 5220  AMAGES OR OTHER 
+00021100: 4c49 4142 494c 4954 592c 2057 4845 5448  LIABILITY, WHETH
+00021110: 4552 2020 2020 2020 207c 0a7c 2020 2020  ER       |.|    
 00021120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021130: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00021140: 2020 2020 2020 2020 2020 2020 2077 6974               wit
-00021150: 6820 4c69 6365 6e73 6f72 2072 6567 6172  h Licensor regar
-00021160: 6469 6e67 2073 7563 6820 436f 6e74 7269  ding such Contri
-00021170: 6275 7469 6f6e 732e 2020 2020 2020 2020  butions.        
-00021180: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00021130: 7c20 2020 2020 2020 2020 2020 494e 2041  |           IN A
+00021140: 4e20 4143 5449 4f4e 204f 4620 434f 4e54  N ACTION OF CONT
+00021150: 5241 4354 2c20 544f 5254 204f 5220 4f54  RACT, TORT OR OT
+00021160: 4845 5257 4953 452c 2041 5249 5349 4e47  HERWISE, ARISING
+00021170: 2046 524f 4d2c 204f 5554 204f 4620 4f52   FROM, OUT OF OR
+00021180: 2049 4e20 2020 2020 2020 2020 2020 7c0a   IN           |.
 00021190: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 000211a0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000211b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000211f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000211b0: 434f 4e4e 4543 5449 4f4e 2057 4954 4820  CONNECTION WITH 
+000211c0: 5448 4520 534f 4654 5741 5245 204f 5220  THE SOFTWARE OR 
+000211d0: 5448 4520 5553 4520 4f52 204f 5448 4552  THE USE OR OTHER
+000211e0: 2044 4541 4c49 4e47 5320 494e 2054 4845   DEALINGS IN THE
+000211f0: 2053 4f46 5457 4152 452e 2020 2020 2020   SOFTWARE.      
 00021200: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00021210: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00021220: 2020 2020 2020 2020 362e 2054 7261 6465          6. Trade
-00021230: 6d61 726b 732e 2054 6869 7320 4c69 6365  marks. This Lice
-00021240: 6e73 6520 646f 6573 206e 6f74 2067 7261  nse does not gra
-00021250: 6e74 2070 6572 6d69 7373 696f 6e20 746f  nt permission to
-00021260: 2075 7365 2074 6865 2074 7261 6465 2020   use the trade  
-00021270: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00021280: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00021290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000212a0: 6e61 6d65 732c 2074 7261 6465 6d61 726b  names, trademark
-000212b0: 732c 2073 6572 7669 6365 206d 6172 6b73  s, service marks
-000212c0: 2c20 6f72 2070 726f 6475 6374 206e 616d  , or product nam
-000212d0: 6573 206f 6620 7468 6520 4c69 6365 6e73  es of the Licens
-000212e0: 6f72 2c20 2020 2020 2020 2020 207c 0a7c  or,          |.|
-000212f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021270: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
+00021280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00021290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000212a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000212b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000212c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000212d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000212e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
+000212f0: 2020 2020 2020 7461 6275 6c61 7465 2020        tabulate  
 00021300: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00021310: 2020 2020 6578 6365 7074 2061 7320 7265      except as re
-00021320: 7175 6972 6564 2066 6f72 2072 6561 736f  quired for reaso
-00021330: 6e61 626c 6520 616e 6420 6375 7374 6f6d  nable and custom
-00021340: 6172 7920 7573 6520 696e 2064 6573 6372  ary use in descr
-00021350: 6962 696e 6720 7468 6520 2020 2020 2020  ibing the       
+00021310: 2020 2020 2020 2020 436f 7079 7269 6768          Copyrigh
+00021320: 7420 2863 2920 3230 3131 2d32 3032 3020  t (c) 2011-2020 
+00021330: 5365 7267 6579 2041 7374 616e 696e 2061  Sergey Astanin a
+00021340: 6e64 2063 6f6e 7472 6962 7574 6f72 7320  nd contributors 
+00021350: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021360: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00021370: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00021380: 2020 2020 2020 2020 2020 206f 7269 6769             origi
-00021390: 6e20 6f66 2074 6865 2057 6f72 6b20 616e  n of the Work an
-000213a0: 6420 7265 7072 6f64 7563 696e 6720 7468  d reproducing th
-000213b0: 6520 636f 6e74 656e 7420 6f66 2074 6865  e content of the
-000213c0: 204e 4f54 4943 4520 6669 6c65 2e20 2020   NOTICE file.   
+00021380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000213a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000213b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000213c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000213d0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 000213e0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000213f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000213f0: 2020 2020 2020 2020 2020 2050 6572 6d69             Permi
+00021400: 7373 696f 6e20 6973 2068 6572 6562 7920  ssion is hereby 
+00021410: 6772 616e 7465 642c 2066 7265 6520 6f66  granted, free of
+00021420: 2063 6861 7267 652c 2074 6f20 616e 7920   charge, to any 
+00021430: 7065 7273 6f6e 206f 6274 6169 6e69 6e67  person obtaining
 00021440: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00021450: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021460: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00021470: 2020 2020 2037 2e20 4469 7363 6c61 696d       7. Disclaim
-00021480: 6572 206f 6620 5761 7272 616e 7479 2e20  er of Warranty. 
-00021490: 556e 6c65 7373 2072 6571 7569 7265 6420  Unless required 
-000214a0: 6279 2061 7070 6c69 6361 626c 6520 6c61  by applicable la
-000214b0: 7720 6f72 2020 2020 2020 2020 2020 2020  w or            
+00021470: 2020 2061 2063 6f70 7920 6f66 2074 6869     a copy of thi
+00021480: 7320 736f 6674 7761 7265 2061 6e64 2061  s software and a
+00021490: 7373 6f63 6961 7465 6420 646f 6375 6d65  ssociated docume
+000214a0: 6e74 6174 696f 6e20 6669 6c65 7320 2874  ntation files (t
+000214b0: 6865 2020 2020 2020 2020 2020 2020 2020  he              
 000214c0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 000214d0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000214e0: 2020 2020 2020 2020 2020 2020 2020 6167                ag
-000214f0: 7265 6564 2074 6f20 696e 2077 7269 7469  reed to in writi
-00021500: 6e67 2c20 4c69 6365 6e73 6f72 2070 726f  ng, Licensor pro
-00021510: 7669 6465 7320 7468 6520 576f 726b 2028  vides the Work (
-00021520: 616e 6420 6561 6368 2020 2020 2020 2020  and each        
+000214e0: 2020 2020 2020 2253 6f66 7477 6172 6522        "Software"
+000214f0: 292c 2074 6f20 6465 616c 2069 6e20 7468  ), to deal in th
+00021500: 6520 536f 6674 7761 7265 2077 6974 686f  e Software witho
+00021510: 7574 2072 6573 7472 6963 7469 6f6e 2c20  ut restriction, 
+00021520: 696e 636c 7564 696e 6720 2020 2020 2020  including       
 00021530: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
 00021540: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00021550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021560: 2020 436f 6e74 7269 6275 746f 7220 7072    Contributor pr
-00021570: 6f76 6964 6573 2069 7473 2043 6f6e 7472  ovides its Contr
-00021580: 6962 7574 696f 6e73 2920 6f6e 2061 6e20  ibutions) on an 
-00021590: 2241 5320 4953 2220 4241 5349 532c 2020  "AS IS" BASIS,  
+00021550: 2020 2020 2020 2020 2020 2077 6974 686f             witho
+00021560: 7574 206c 696d 6974 6174 696f 6e20 7468  ut limitation th
+00021570: 6520 7269 6768 7473 2074 6f20 7573 652c  e rights to use,
+00021580: 2063 6f70 792c 206d 6f64 6966 792c 206d   copy, modify, m
+00021590: 6572 6765 2c20 7075 626c 6973 682c 2020  erge, publish,  
 000215a0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 000215b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000215c0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-000215d0: 2020 2020 2057 4954 484f 5554 2057 4152       WITHOUT WAR
-000215e0: 5241 4e54 4945 5320 4f52 2043 4f4e 4449  RANTIES OR CONDI
-000215f0: 5449 4f4e 5320 4f46 2041 4e59 204b 494e  TIONS OF ANY KIN
-00021600: 442c 2065 6974 6865 7220 6578 7072 6573  D, either expres
-00021610: 7320 6f72 2020 2020 2020 2020 2020 2020  s or            
+000215d0: 2064 6973 7472 6962 7574 652c 2073 7562   distribute, sub
+000215e0: 6c69 6365 6e73 652c 2061 6e64 2f6f 7220  license, and/or 
+000215f0: 7365 6c6c 2063 6f70 6965 7320 6f66 2074  sell copies of t
+00021600: 6865 2053 6f66 7477 6172 652c 2061 6e64  he Software, and
+00021610: 2074 6f20 2020 2020 2020 2020 2020 2020   to             
 00021620: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00021630: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00021640: 2020 2020 2020 2020 696d 706c 6965 642c          implied,
-00021650: 2069 6e63 6c75 6469 6e67 2c20 7769 7468   including, with
-00021660: 6f75 7420 6c69 6d69 7461 7469 6f6e 2c20  out limitation, 
-00021670: 616e 7920 7761 7272 616e 7469 6573 206f  any warranties o
-00021680: 7220 636f 6e64 6974 696f 6e73 2020 2020  r conditions    
+00021640: 2020 2020 7065 726d 6974 2070 6572 736f      permit perso
+00021650: 6e73 2074 6f20 7768 6f6d 2074 6865 2053  ns to whom the S
+00021660: 6f66 7477 6172 6520 6973 2066 7572 6e69  oftware is furni
+00021670: 7368 6564 2074 6f20 646f 2073 6f2c 2073  shed to do so, s
+00021680: 7562 6a65 6374 2074 6f20 2020 2020 2020  ubject to       
 00021690: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 000216a0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
 000216b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000216c0: 6f66 2054 4954 4c45 2c20 4e4f 4e2d 494e  of TITLE, NON-IN
-000216d0: 4652 494e 4745 4d45 4e54 2c20 4d45 5243  FRINGEMENT, MERC
-000216e0: 4841 4e54 4142 494c 4954 592c 206f 7220  HANTABILITY, or 
-000216f0: 4649 544e 4553 5320 464f 5220 4120 2020  FITNESS FOR A   
+000216c0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000216d0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
+000216e0: 6469 7469 6f6e 733a 2020 2020 2020 2020  ditions:        
+000216f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021700: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00021710: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021720: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00021730: 2020 2050 4152 5449 4355 4c41 5220 5055     PARTICULAR PU
-00021740: 5250 4f53 452e 2059 6f75 2061 7265 2073  RPOSE. You are s
-00021750: 6f6c 656c 7920 7265 7370 6f6e 7369 626c  olely responsibl
-00021760: 6520 666f 7220 6465 7465 726d 696e 696e  e for determinin
-00021770: 6720 7468 6520 2020 2020 2020 2020 207c  g the          |
+00021730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021770: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00021780: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00021790: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000217a0: 2020 2020 2020 2020 6170 7072 6f70 7269          appropri
-000217b0: 6174 656e 6573 7320 6f66 2075 7369 6e67  ateness of using
-000217c0: 206f 7220 7265 6469 7374 7269 6275 7469   or redistributi
-000217d0: 6e67 2074 6865 2057 6f72 6b20 616e 6420  ng the Work and 
-000217e0: 6173 7375 6d65 2061 6e79 2020 2020 2020  assume any      
+000217a0: 2020 2020 2020 2054 6865 2061 626f 7665         The above
+000217b0: 2063 6f70 7972 6967 6874 206e 6f74 6963   copyright notic
+000217c0: 6520 616e 6420 7468 6973 2070 6572 6d69  e and this permi
+000217d0: 7373 696f 6e20 6e6f 7469 6365 2073 6861  ssion notice sha
+000217e0: 6c6c 2062 6520 2020 2020 2020 2020 2020  ll be           
 000217f0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00021800: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00021810: 2020 2020 2020 2020 2020 2072 6973 6b73             risks
-00021820: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00021830: 2059 6f75 7220 6578 6572 6369 7365 206f   Your exercise o
-00021840: 6620 7065 726d 6973 7369 6f6e 7320 756e  f permissions un
-00021850: 6465 7220 7468 6973 204c 6963 656e 7365  der this License
-00021860: 2e20 2020 2020 2020 207c 0a7c 2020 2020  .        |.|    
+00021810: 2020 2020 2020 2020 2020 2069 6e63 6c75             inclu
+00021820: 6465 6420 696e 2061 6c6c 2063 6f70 6965  ded in all copie
+00021830: 7320 6f72 2073 7562 7374 616e 7469 616c  s or substantial
+00021840: 2070 6f72 7469 6f6e 7320 6f66 2074 6865   portions of the
+00021850: 2053 6f66 7477 6172 652e 2020 2020 2020   Software.      
+00021860: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00021870: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021880: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00021890: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000218a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000218b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000218c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000218d0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 000218e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 000218f0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00021900: 2020 2020 2038 2e20 4c69 6d69 7461 7469       8. Limitati
-00021910: 6f6e 206f 6620 4c69 6162 696c 6974 792e  on of Liability.
-00021920: 2049 6e20 6e6f 2065 7665 6e74 2061 6e64   In no event and
-00021930: 2075 6e64 6572 206e 6f20 6c65 6761 6c20   under no legal 
-00021940: 7468 656f 7279 2c20 2020 2020 2020 2020  theory,         
+00021900: 2020 2020 2054 4845 2053 4f46 5457 4152       THE SOFTWAR
+00021910: 4520 4953 2050 524f 5649 4445 4420 2241  E IS PROVIDED "A
+00021920: 5320 4953 222c 2057 4954 484f 5554 2057  S IS", WITHOUT W
+00021930: 4152 5241 4e54 5920 4f46 2041 4e59 204b  ARRANTY OF ANY K
+00021940: 494e 442c 2020 2020 2020 2020 2020 2020  IND,            
 00021950: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 00021960: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00021970: 2020 2020 2020 2020 2020 2020 2077 6865               whe
-00021980: 7468 6572 2069 6e20 746f 7274 2028 696e  ther in tort (in
-00021990: 636c 7564 696e 6720 6e65 676c 6967 656e  cluding negligen
-000219a0: 6365 292c 2063 6f6e 7472 6163 742c 206f  ce), contract, o
-000219b0: 7220 6f74 6865 7277 6973 652c 2020 2020  r otherwise,    
+00021970: 2020 2020 2020 2020 2045 5850 5245 5353           EXPRESS
+00021980: 204f 5220 494d 504c 4945 442c 2049 4e43   OR IMPLIED, INC
+00021990: 4c55 4449 4e47 2042 5554 204e 4f54 204c  LUDING BUT NOT L
+000219a0: 494d 4954 4544 2054 4f20 5448 4520 5741  IMITED TO THE WA
+000219b0: 5252 414e 5449 4553 204f 4620 2020 2020  RRANTIES OF     
 000219c0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 000219d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 000219e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000219f0: 2075 6e6c 6573 7320 7265 7175 6972 6564   unless required
-00021a00: 2062 7920 6170 706c 6963 6162 6c65 206c   by applicable l
-00021a10: 6177 2028 7375 6368 2061 7320 6465 6c69  aw (such as deli
-00021a20: 6265 7261 7465 2061 6e64 2067 726f 7373  berate and gross
-00021a30: 6c79 2020 2020 2020 2020 2020 207c 0a7c  ly           |.|
+000219f0: 2020 2020 4d45 5243 4841 4e54 4142 494c      MERCHANTABIL
+00021a00: 4954 592c 2046 4954 4e45 5353 2046 4f52  ITY, FITNESS FOR
+00021a10: 2041 2050 4152 5449 4355 4c41 5220 5055   A PARTICULAR PU
+00021a20: 5250 4f53 4520 414e 4420 2020 2020 2020  RPOSE AND       
+00021a30: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00021a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021a50: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00021a60: 2020 2020 2020 6e65 676c 6967 656e 7420        negligent 
-00021a70: 6163 7473 2920 6f72 2061 6772 6565 6420  acts) or agreed 
-00021a80: 746f 2069 6e20 7772 6974 696e 672c 2073  to in writing, s
-00021a90: 6861 6c6c 2061 6e79 2043 6f6e 7472 6962  hall any Contrib
-00021aa0: 7574 6f72 2062 6520 2020 2020 2020 2020  utor be         
+00021a60: 204e 4f4e 494e 4652 494e 4745 4d45 4e54   NONINFRINGEMENT
+00021a70: 2e20 494e 204e 4f20 4556 454e 5420 5348  . IN NO EVENT SH
+00021a80: 414c 4c20 5448 4520 4155 5448 4f52 5320  ALL THE AUTHORS 
+00021a90: 4f52 2043 4f50 5952 4947 4854 2048 4f4c  OR COPYRIGHT HOL
+00021aa0: 4445 5253 2042 4520 2020 2020 2020 2020  DERS BE         
 00021ab0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00021ac0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00021ad0: 2020 2020 2020 2020 2020 6c69 6162 6c65            liable
-00021ae0: 2074 6f20 596f 7520 666f 7220 6461 6d61   to You for dama
-00021af0: 6765 732c 2069 6e63 6c75 6469 6e67 2061  ges, including a
-00021b00: 6e79 2064 6972 6563 742c 2069 6e64 6972  ny direct, indir
-00021b10: 6563 742c 2073 7065 6369 616c 2c20 2020  ect, special,   
+00021ad0: 2020 2020 2020 4c49 4142 4c45 2046 4f52        LIABLE FOR
+00021ae0: 2041 4e59 2043 4c41 494d 2c20 4441 4d41   ANY CLAIM, DAMA
+00021af0: 4745 5320 4f52 204f 5448 4552 204c 4941  GES OR OTHER LIA
+00021b00: 4249 4c49 5459 2c20 5748 4554 4845 5220  BILITY, WHETHER 
+00021b10: 494e 2041 4e20 4143 5449 4f4e 2020 2020  IN AN ACTION    
 00021b20: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00021b30: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00021b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021b50: 696e 6369 6465 6e74 616c 2c20 6f72 2063  incidental, or c
-00021b60: 6f6e 7365 7175 656e 7469 616c 2064 616d  onsequential dam
-00021b70: 6167 6573 206f 6620 616e 7920 6368 6172  ages of any char
-00021b80: 6163 7465 7220 6172 6973 696e 6720 6173  acter arising as
-00021b90: 2061 2020 2020 2020 2020 2020 7c0a 7c20   a          |.| 
+00021b40: 2020 2020 2020 2020 2020 204f 4620 434f             OF CO
+00021b50: 4e54 5241 4354 2c20 544f 5254 204f 5220  NTRACT, TORT OR 
+00021b60: 4f54 4845 5257 4953 452c 2041 5249 5349  OTHERWISE, ARISI
+00021b70: 4e47 2046 524f 4d2c 204f 5554 204f 4620  NG FROM, OUT OF 
+00021b80: 4f52 2049 4e20 434f 4e4e 4543 5449 4f4e  OR IN CONNECTION
+00021b90: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00021ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021bb0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00021bc0: 2020 2020 2020 7265 7375 6c74 206f 6620        result of 
-00021bd0: 7468 6973 204c 6963 656e 7365 206f 7220  this License or 
-00021be0: 6f75 7420 6f66 2074 6865 2075 7365 206f  out of the use o
-00021bf0: 7220 696e 6162 696c 6974 7920 746f 2075  r inability to u
-00021c00: 7365 2074 6865 2020 2020 2020 2020 2020  se the          
+00021bc0: 2020 2057 4954 4820 5448 4520 534f 4654     WITH THE SOFT
+00021bd0: 5741 5245 204f 5220 5448 4520 5553 4520  WARE OR THE USE 
+00021be0: 4f52 204f 5448 4552 2044 4541 4c49 4e47  OR OTHER DEALING
+00021bf0: 5320 494e 2054 4845 2053 4f46 5457 4152  S IN THE SOFTWAR
+00021c00: 452e 2020 2020 2020 2020 2020 2020 2020  E.              
 00021c10: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
 00021c20: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00021c30: 2020 2020 2020 2020 2020 2057 6f72 6b20             Work 
-00021c40: 2869 6e63 6c75 6469 6e67 2062 7574 206e  (including but n
-00021c50: 6f74 206c 696d 6974 6564 2074 6f20 6461  ot limited to da
-00021c60: 6d61 6765 7320 666f 7220 6c6f 7373 206f  mages for loss o
-00021c70: 6620 676f 6f64 7769 6c6c 2c20 2020 2020  f goodwill,     
-00021c80: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00021c90: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00021ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021cb0: 2077 6f72 6b20 7374 6f70 7061 6765 2c20   work stoppage, 
-00021cc0: 636f 6d70 7574 6572 2066 6169 6c75 7265  computer failure
-00021cd0: 206f 7220 6d61 6c66 756e 6374 696f 6e2c   or malfunction,
-00021ce0: 206f 7220 616e 7920 616e 6420 616c 6c20   or any and all 
-00021cf0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00021d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021c80: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
+00021c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00021ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00021cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00021cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00021cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00021ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00021cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020  -----------+.|  
+00021d00: 2020 2020 2020 7471 646d 2020 2020 2020        tqdm      
 00021d10: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00021d20: 2020 2020 2020 6f74 6865 7220 636f 6d6d        other comm
-00021d30: 6572 6369 616c 2064 616d 6167 6573 206f  ercial damages o
-00021d40: 7220 6c6f 7373 6573 292c 2065 7665 6e20  r losses), even 
-00021d50: 6966 2073 7563 6820 436f 6e74 7269 6275  if such Contribu
-00021d60: 746f 7220 2020 2020 2020 2020 2020 2020  tor             
+00021d20: 2020 2020 2020 2020 2020 2020 2060 7471               `tq
+00021d30: 646d 6020 6973 2061 2070 726f 6475 6374  dm` is a product
+00021d40: 206f 6620 636f 6c6c 6162 6f72 6174 6976   of collaborativ
+00021d50: 6520 776f 726b 2e20 2020 2020 2020 2020  e work.         
+00021d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021d70: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 00021d80: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00021d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021da0: 6861 7320 6265 656e 2061 6476 6973 6564  has been advised
-00021db0: 206f 6620 7468 6520 706f 7373 6962 696c   of the possibil
-00021dc0: 6974 7920 6f66 2073 7563 6820 6461 6d61  ity of such dama
-00021dd0: 6765 732e 2020 2020 2020 2020 2020 2020  ges.            
+00021d90: 2020 2055 6e6c 6573 7320 6f74 6865 7277     Unless otherw
+00021da0: 6973 6520 7374 6174 6564 2c20 616c 6c20  ise stated, all 
+00021db0: 6175 7468 6f72 7320 2873 6565 2063 6f6d  authors (see com
+00021dc0: 6d69 7420 6c6f 6773 2920 7265 7461 696e  mit logs) retain
+00021dd0: 2063 6f70 7972 6967 6874 2020 2020 2020   copyright      
 00021de0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00021df0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00021e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021e00: 2020 2020 2020 2020 2066 6f72 2074 6865           for the
+00021e10: 6972 2072 6573 7065 6374 6976 6520 776f  ir respective wo
+00021e20: 726b 2c20 616e 6420 7265 6c65 6173 6520  rk, and release 
+00021e30: 7468 6520 776f 726b 2075 6e64 6572 2074  the work under t
+00021e40: 6865 204d 4954 206c 6963 656e 6365 2020  he MIT licence  
 00021e50: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00021e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021e70: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00021e80: 2039 2e20 4163 6365 7074 696e 6720 5761   9. Accepting Wa
-00021e90: 7272 616e 7479 206f 7220 4164 6469 7469  rranty or Additi
-00021ea0: 6f6e 616c 204c 6961 6269 6c69 7479 2e20  onal Liability. 
-00021eb0: 5768 696c 6520 7265 6469 7374 7269 6275  While redistribu
-00021ec0: 7469 6e67 2020 2020 2020 2020 2020 207c  ting           |
+00021e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021e90: 2020 2020 2020 2020 2020 2874 6578 7420            (text 
+00021ea0: 6265 6c6f 7729 2e20 2020 2020 2020 2020  below).         
+00021eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021ec0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00021ed0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
 00021ee0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00021ef0: 2020 2020 2020 2020 2020 7468 6520 576f            the Wo
-00021f00: 726b 206f 7220 4465 7269 7661 7469 7665  rk or Derivative
-00021f10: 2057 6f72 6b73 2074 6865 7265 6f66 2c20   Works thereof, 
-00021f20: 596f 7520 6d61 7920 6368 6f6f 7365 2074  You may choose t
-00021f30: 6f20 6f66 6665 722c 2020 2020 2020 2020  o offer,        
+00021ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021f40: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
 00021f50: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00021f60: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00021f70: 2063 6861 7267 6520 6120 6665 6520 666f   charge a fee fo
-00021f80: 722c 2061 6363 6570 7461 6e63 6520 6f66  r, acceptance of
-00021f90: 2073 7570 706f 7274 2c20 7761 7272 616e   support, warran
-00021fa0: 7479 2c20 696e 6465 6d6e 6974 792c 2020  ty, indemnity,  
+00021f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021f70: 2020 2020 4578 6365 7074 696f 6e73 206f      Exceptions o
+00021f80: 7220 6e6f 7461 626c 6520 6175 7468 6f72  r notable author
+00021f90: 7320 6172 6520 6c69 7374 6564 2062 656c  s are listed bel
+00021fa0: 6f77 2020 2020 2020 2020 2020 2020 2020  ow              
 00021fb0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00021fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00021fd0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00021fe0: 2020 6f72 206f 7468 6572 206c 6961 6269    or other liabi
-00021ff0: 6c69 7479 206f 626c 6967 6174 696f 6e73  lity obligations
-00022000: 2061 6e64 2f6f 7220 7269 6768 7473 2063   and/or rights c
-00022010: 6f6e 7369 7374 656e 7420 7769 7468 2074  onsistent with t
-00022020: 6869 7320 2020 2020 2020 2020 2020 7c0a  his           |.
+00021fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021ff0: 696e 2072 6576 6572 7365 2063 6872 6f6e  in reverse chron
+00022000: 6f6c 6f67 6963 616c 206f 7264 6572 3a20  ological order: 
+00022010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022020: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
 00022030: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00022040: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00022050: 2020 2020 2020 204c 6963 656e 7365 2e20         License. 
-00022060: 486f 7765 7665 722c 2069 6e20 6163 6365  However, in acce
-00022070: 7074 696e 6720 7375 6368 206f 626c 6967  pting such oblig
-00022080: 6174 696f 6e73 2c20 596f 7520 6d61 7920  ations, You may 
-00022090: 6163 7420 6f6e 6c79 2020 2020 2020 2020  act only        
+00022050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022090: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000220a0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
 000220b0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000220c0: 2020 2020 2020 2020 2020 2020 6f6e 2059              on Y
-000220d0: 6f75 7220 6f77 6e20 6265 6861 6c66 2061  our own behalf a
-000220e0: 6e64 206f 6e20 596f 7572 2073 6f6c 6520  nd on Your sole 
-000220f0: 7265 7370 6f6e 7369 6269 6c69 7479 2c20  responsibility, 
-00022100: 6e6f 7420 6f6e 2062 6568 616c 6620 2020  not on behalf   
+000220c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000220d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000220e0: 2020 2020 202a 2066 696c 6573 3a20 2a20       * files: * 
+000220f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022110: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
 00022120: 2020 2020 2020 2020 2020 2020 2020 207c                 |
 00022130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022140: 2020 206f 6620 616e 7920 6f74 6865 7220     of any other 
-00022150: 436f 6e74 7269 6275 746f 722c 2061 6e64  Contributor, and
-00022160: 206f 6e6c 7920 6966 2059 6f75 2061 6772   only if You agr
-00022170: 6565 2074 6f20 696e 6465 6d6e 6966 792c  ee to indemnify,
+00022140: 2020 2020 2020 2020 2020 204d 504c 2d32             MPL-2
+00022150: 2e30 2032 3031 352d 3230 3234 2028 6329  .0 2015-2024 (c)
+00022160: 2043 6173 7065 7220 6461 2043 6f73 7461   Casper da Costa
+00022170: 2d4c 7569 7320 2020 2020 2020 2020 2020  -Luis           
 00022180: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00022190: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000221a0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-000221b0: 2020 2020 2020 2020 2064 6566 656e 642c           defend,
-000221c0: 2061 6e64 2068 6f6c 6420 6561 6368 2043   and hold each C
-000221d0: 6f6e 7472 6962 7574 6f72 2068 6172 6d6c  ontributor harml
-000221e0: 6573 7320 666f 7220 616e 7920 6c69 6162  ess for any liab
-000221f0: 696c 6974 7920 2020 2020 2020 2020 2020  ility           
+000221b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000221c0: 5b63 6173 7065 7264 636c 5d28 6874 7470  [casperdcl](http
+000221d0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f63  s://github.com/c
+000221e0: 6173 7065 7264 636c 292e 2020 2020 2020  asperdcl).      
+000221f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022200: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
 00022210: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00022220: 2020 2020 2020 2020 2020 696e 6375 7272            incurr
-00022230: 6564 2062 792c 206f 7220 636c 6169 6d73  ed by, or claims
-00022240: 2061 7373 6572 7465 6420 6167 6169 6e73   asserted agains
-00022250: 742c 2073 7563 6820 436f 6e74 7269 6275  t, such Contribu
-00022260: 746f 7220 6279 2072 6561 736f 6e20 2020  tor by reason   
+00022220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022230: 2020 2020 2020 2020 2020 2020 2020 2a20                * 
+00022240: 6669 6c65 733a 2074 7164 6d2f 5f74 7164  files: tqdm/_tqd
+00022250: 6d2e 7079 2020 2020 2020 2020 2020 2020  m.py            
+00022260: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022270: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
 00022280: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 00022290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000222a0: 2020 206f 6620 796f 7572 2061 6363 6570     of your accep
-000222b0: 7469 6e67 2061 6e79 2073 7563 6820 7761  ting any such wa
-000222c0: 7272 616e 7479 206f 7220 6164 6469 7469  rranty or additi
-000222d0: 6f6e 616c 206c 6961 6269 6c69 7479 2e20  onal liability. 
+000222a0: 2020 2020 2020 2020 4d49 5420 3230 3136          MIT 2016
+000222b0: 2028 6329 205b 5052 2023 3936 5d20 6f6e   (c) [PR #96] on
+000222c0: 2062 6568 616c 6620 6f66 2047 6f6f 676c   behalf of Googl
+000222d0: 6520 496e 632e 2020 2020 2020 2020 2020  e Inc.          
 000222e0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 000222f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022300: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00022310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022310: 2020 2020 2020 2020 2020 2020 202a 2066               * f
+00022320: 696c 6573 3a20 7471 646d 2f5f 7471 646d  iles: tqdm/_tqdm
+00022330: 2e70 7920 5245 4144 4d45 2e72 7374 202e  .py README.rst .
+00022340: 6769 7469 676e 6f72 6520 2020 2020 2020  gitignore       
 00022350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022360: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
-00022370: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00022380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00022390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000223a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000223b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000223c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000223d0: 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020 2072  ------+.|      r
-000223e0: 7374 3261 6e73 6920 2020 2020 207c 2020  st2ansi      |  
+00022360: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00022370: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00022380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022390: 4d49 5420 3230 3133 2028 6329 204e 6f61  MIT 2013 (c) Noa
+000223a0: 6d20 596f 7261 762d 5261 7068 6165 6c2c  m Yorav-Raphael,
+000223b0: 206f 7269 6769 6e61 6c20 6175 7468 6f72   original author
+000223c0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+000223d0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+000223e0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
 000223f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022400: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022410: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022420: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022430: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022440: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00022450: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022460: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00022470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022480: 2020 2020 2020 2054 6865 204d 4954 204c         The MIT L
-00022490: 6963 656e 7365 2028 4d49 5429 2020 2020  icense (MIT)    
-000224a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022470: 2020 2020 2020 2020 2020 205b 5052 2023             [PR #
+00022480: 3936 5d3a 2068 7474 7073 3a2f 2f67 6974  96]: https://git
+00022490: 6875 622e 636f 6d2f 7471 646d 2f74 7164  hub.com/tqdm/tqd
+000224a0: 6d2f 7075 6c6c 2f39 3620 2020 2020 2020  m/pull/96       
 000224b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000224c0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
 000224d0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
 000224e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000224f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022500: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022510: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022520: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022530: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
 00022540: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00022550: 2020 2020 2020 2020 2020 2043 6f70 7972             Copyr
-00022560: 6967 6874 20c2 a920 3230 3135 2d32 3031  ight .. 2015-201
-00022570: 3620 4672 616e 6b6c 696e 2022 536e 6169  6 Franklin "Snai
-00022580: 7065 2220 4d61 7468 6965 7520 3c68 7474  pe" Mathieu <htt
-00022590: 703a 2f2f 736e 6169 2e70 652f 3e20 2020  p://snai.pe/>   
-000225a0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00022550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000225a0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 000225b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000225c0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-000225d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000225e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000225f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022620: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00022630: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00022640: 2050 6572 6d69 7373 696f 6e20 6973 2068   Permission is h
-00022650: 6572 6562 7920 6772 616e 7465 642c 2066  ereby granted, f
-00022660: 7265 6520 6f66 2063 6861 7267 652c 2074  ree of charge, t
-00022670: 6f20 616e 7920 7065 7273 6f6e 206f 6274  o any person obt
-00022680: 6169 6e69 6e67 2061 2063 6f70 7920 2020  aining a copy   
-00022690: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-000226a0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000226b0: 2020 2020 206f 6620 7468 6973 2073 6f66       of this sof
-000226c0: 7477 6172 6520 616e 6420 6173 736f 6369  tware and associ
-000226d0: 6174 6564 2064 6f63 756d 656e 7461 7469  ated documentati
-000226e0: 6f6e 2066 696c 6573 2028 7468 6520 2253  on files (the "S
-000226f0: 6f66 7477 6172 6522 292c 2074 6f20 6465  oftware"), to de
-00022700: 616c 2020 2020 2020 2020 7c0a 7c20 2020  al        |.|   
+000225c0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+000225d0: 2020 2020 2020 2020 204d 6f7a 696c 6c61           Mozilla
+000225e0: 2050 7562 6c69 6320 4c69 6365 6e63 6520   Public Licence 
+000225f0: 284d 504c 2920 762e 2032 2e30 202d 2045  (MPL) v. 2.0 - E
+00022600: 7868 6962 6974 2041 2020 2020 2020 2020  xhibit A        
+00022610: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00022620: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00022630: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00022640: 2020 2020 2020 2020 2020 2020 2020 2d2d                --
+00022650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00022660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00022670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 2020  -------------   
+00022680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022690: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+000226a0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+000226b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000226c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000226d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000226e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000226f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022700: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 00022710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022720: 207c 2020 2020 2020 2020 2069 6e20 7468   |         in th
-00022730: 6520 536f 6674 7761 7265 2077 6974 686f  e Software witho
-00022740: 7574 2072 6573 7472 6963 7469 6f6e 2c20  ut restriction, 
-00022750: 696e 636c 7564 696e 6720 7769 7468 6f75  including withou
-00022760: 7420 6c69 6d69 7461 7469 6f6e 2074 6865  t limitation the
-00022770: 2072 6967 6874 7320 2020 2020 2020 207c   rights        |
-00022780: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00022790: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000227a0: 2074 6f20 7573 652c 2063 6f70 792c 206d   to use, copy, m
-000227b0: 6f64 6966 792c 206d 6572 6765 2c20 7075  odify, merge, pu
-000227c0: 626c 6973 682c 2064 6973 7472 6962 7574  blish, distribut
-000227d0: 652c 2073 7562 6c69 6365 6e73 652c 2061  e, sublicense, a
-000227e0: 6e64 2f6f 7220 7365 6c6c 2020 2020 2020  nd/or sell      
-000227f0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00022800: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00022810: 2020 2020 2020 2020 636f 7069 6573 206f          copies o
-00022820: 6620 7468 6520 536f 6674 7761 7265 2c20  f the Software, 
-00022830: 616e 6420 746f 2070 6572 6d69 7420 7065  and to permit pe
-00022840: 7273 6f6e 7320 746f 2077 686f 6d20 7468  rsons to whom th
-00022850: 6520 536f 6674 7761 7265 2069 7320 2020  e Software is   
-00022860: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00022870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022880: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00022890: 2020 2020 6675 726e 6973 6865 6420 746f      furnished to
-000228a0: 2064 6f20 736f 2c20 7375 626a 6563 7420   do so, subject 
-000228b0: 746f 2074 6865 2066 6f6c 6c6f 7769 6e67  to the following
-000228c0: 2063 6f6e 6469 7469 6f6e 733a 2020 2020   conditions:    
-000228d0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-000228e0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000228f0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00022720: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00022730: 2020 2020 2020 5468 6973 2053 6f75 7263        This Sourc
+00022740: 6520 436f 6465 2046 6f72 6d20 6973 2073  e Code Form is s
+00022750: 7562 6a65 6374 2074 6f20 7468 6520 7465  ubject to the te
+00022760: 726d 7320 6f66 2074 6865 2020 2020 2020  rms of the      
+00022770: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00022780: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00022790: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+000227a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000227b0: 2020 2020 204d 6f7a 696c 6c61 2050 7562       Mozilla Pub
+000227c0: 6c69 6320 4c69 6365 6e73 652c 2076 2e20  lic License, v. 
+000227d0: 322e 302e 2020 2020 2020 2020 2020 2020  2.0.            
+000227e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000227f0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+00022800: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00022810: 2020 2020 2020 2020 2020 2020 4966 2061              If a
+00022820: 2063 6f70 7920 6f66 2074 6865 204d 504c   copy of the MPL
+00022830: 2077 6173 206e 6f74 2064 6973 7472 6962   was not distrib
+00022840: 7574 6564 2077 6974 6820 7468 6973 2070  uted with this p
+00022850: 726f 6a65 6374 2c20 2020 2020 2020 2020  roject,         
+00022860: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+00022870: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00022880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022890: 2020 2020 2059 6f75 2063 616e 206f 6274       You can obt
+000228a0: 6169 6e20 6f6e 6520 6174 2068 7474 7073  ain one at https
+000228b0: 3a2f 2f6d 6f7a 696c 6c61 2e6f 7267 2f4d  ://mozilla.org/M
+000228c0: 504c 2f32 2e30 2f2e 2020 2020 2020 2020  PL/2.0/.        
+000228d0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000228e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000228f0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
 00022900: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022910: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022920: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022930: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022950: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00022960: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00022970: 2020 2020 2054 6865 2061 626f 7665 2063       The above c
-00022980: 6f70 7972 6967 6874 206e 6f74 6963 6520  opyright notice 
-00022990: 616e 6420 7468 6973 2070 6572 6d69 7373  and this permiss
-000229a0: 696f 6e20 6e6f 7469 6365 2073 6861 6c6c  ion notice shall
-000229b0: 2062 6520 696e 636c 7564 6564 2069 6e20   be included in 
-000229c0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-000229d0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00022950: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+00022960: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00022970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000229c0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+000229d0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 000229e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000229f0: 2020 2020 2061 6c6c 2063 6f70 6965 7320       all copies 
-00022a00: 6f72 2073 7562 7374 616e 7469 616c 2070  or substantial p
-00022a10: 6f72 7469 6f6e 7320 6f66 2074 6865 2053  ortions of the S
-00022a20: 6f66 7477 6172 652e 2020 2020 2020 2020  oftware.        
-00022a30: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+000229f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a00: 2020 2020 204d 4954 204c 6963 656e 7365       MIT License
+00022a10: 2028 4d49 5429 2020 2020 2020 2020 2020   (MIT)          
+00022a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a30: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 00022a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a50: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00022a50: 2020 207c 2020 2020 2020 2020 2020 2020     |            
 00022a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a70: 2020 2020 2020 2020 2020 2d2d 2d2d 2d2d            ------
+00022a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d20 2020 2020  -----------     
 00022a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022ab0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00022ac0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00022ad0: 2020 2020 5448 4520 534f 4654 5741 5245      THE SOFTWARE
-00022ae0: 2049 5320 5052 4f56 4944 4544 2022 4153   IS PROVIDED "AS
-00022af0: 2049 5322 2c20 5749 5448 4f55 5420 5741   IS", WITHOUT WA
-00022b00: 5252 414e 5459 204f 4620 414e 5920 4b49  RRANTY OF ANY KI
-00022b10: 4e44 2c20 4558 5052 4553 5320 4f52 2020  ND, EXPRESS OR  
-00022b20: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00022b30: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00022b40: 2020 2020 2020 2020 2020 494d 504c 4945            IMPLIE
-00022b50: 442c 2049 4e43 4c55 4449 4e47 2042 5554  D, INCLUDING BUT
-00022b60: 204e 4f54 204c 494d 4954 4544 2054 4f20   NOT LIMITED TO 
-00022b70: 5448 4520 5741 5252 414e 5449 4553 204f  THE WARRANTIES O
-00022b80: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
-00022b90: 592c 2020 2020 2020 2020 2020 7c0a 7c20  Y,          |.| 
+00022ab0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00022ac0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00022ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b20: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+00022b30: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00022b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b50: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00022b60: 6f70 7972 6967 6874 2028 6329 2032 3031  opyright (c) 201
+00022b70: 3320 6e6f 616d 7261 7068 2020 2020 2020  3 noamraph      
+00022b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022b90: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00022ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022bb0: 2020 207c 2020 2020 2020 2020 2046 4954     |         FIT
-00022bc0: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
-00022bd0: 4355 4c41 5220 5055 5250 4f53 4520 414e  CULAR PURPOSE AN
-00022be0: 4420 4e4f 4e49 4e46 5249 4e47 454d 454e  D NONINFRINGEMEN
-00022bf0: 542e 2049 4e20 4e4f 2045 5645 4e54 2053  T. IN NO EVENT S
-00022c00: 4841 4c4c 2054 4845 2020 2020 2020 2020  HALL THE        
-00022c10: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00022c20: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00022c30: 2020 2020 2041 5554 484f 5253 204f 5220       AUTHORS OR 
-00022c40: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
-00022c50: 5320 4245 204c 4941 424c 4520 464f 5220  S BE LIABLE FOR 
-00022c60: 414e 5920 434c 4149 4d2c 2044 414d 4147  ANY CLAIM, DAMAG
-00022c70: 4553 204f 5220 4f54 4845 5220 2020 2020  ES OR OTHER     
-00022c80: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00022c90: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00022ca0: 2020 2020 2020 4c49 4142 494c 4954 592c        LIABILITY,
-00022cb0: 2057 4845 5448 4552 2049 4e20 414e 2041   WHETHER IN AN A
-00022cc0: 4354 494f 4e20 4f46 2043 4f4e 5452 4143  CTION OF CONTRAC
-00022cd0: 542c 2054 4f52 5420 4f52 204f 5448 4552  T, TORT OR OTHER
-00022ce0: 5749 5345 2c20 4152 4953 494e 4720 4652  WISE, ARISING FR
-00022cf0: 4f4d 2c20 2020 2020 2020 207c 0a7c 2020  OM,        |.|  
+00022bb0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00022bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022c10: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00022c20: 2020 2020 2020 207c 2020 2020 2020 2050         |       P
+00022c30: 6572 6d69 7373 696f 6e20 6973 2068 6572  ermission is her
+00022c40: 6562 7920 6772 616e 7465 642c 2066 7265  eby granted, fre
+00022c50: 6520 6f66 2063 6861 7267 652c 2074 6f20  e of charge, to 
+00022c60: 616e 7920 7065 7273 6f6e 206f 6274 6169  any person obtai
+00022c70: 6e69 6e67 2061 2063 6f70 7920 6f66 2020  ning a copy of  
+00022c80: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+00022c90: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00022ca0: 2020 2020 2074 6869 7320 736f 6674 7761       this softwa
+00022cb0: 7265 2061 6e64 2061 7373 6f63 6961 7465  re and associate
+00022cc0: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
+00022cd0: 6669 6c65 7320 2874 6865 2022 536f 6674  files (the "Soft
+00022ce0: 7761 7265 2229 2c20 746f 2064 6561 6c20  ware"), to deal 
+00022cf0: 696e 2020 2020 2020 2020 7c0a 7c20 2020  in        |.|   
 00022d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022d10: 2020 7c20 2020 2020 2020 2020 204f 5554    |          OUT
-00022d20: 204f 4620 4f52 2049 4e20 434f 4e4e 4543   OF OR IN CONNEC
-00022d30: 5449 4f4e 2057 4954 4820 5448 4520 534f  TION WITH THE SO
-00022d40: 4654 5741 5245 204f 5220 5448 4520 5553  FTWARE OR THE US
-00022d50: 4520 4f52 204f 5448 4552 2044 4541 4c49  E OR OTHER DEALI
-00022d60: 4e47 5320 494e 2020 2020 2020 2020 2020  NGS IN          
-00022d70: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00022d80: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00022d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022db0: 5448 4520 534f 4654 5741 5245 2e20 2020  THE SOFTWARE.   
-00022dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022de0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00022df0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00022e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022e50: 2020 2020 2020 2020 2020 7c0a 2b2d 2d2d            |.+---
-00022e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00022e70: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00022e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00022e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00022ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00022eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00022ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00022ed0: 0a7c 2020 2020 2073 6574 7570 746f 6f6c  .|     setuptool
-00022ee0: 7320 2020 2020 7c20 2020 2020 2020 2020  s     |         
+00022d10: 207c 2020 2020 2020 2020 2074 6865 2053   |         the S
+00022d20: 6f66 7477 6172 6520 7769 7468 6f75 7420  oftware without 
+00022d30: 7265 7374 7269 6374 696f 6e2c 2069 6e63  restriction, inc
+00022d40: 6c75 6469 6e67 2077 6974 686f 7574 206c  luding without l
+00022d50: 696d 6974 6174 696f 6e20 7468 6520 7269  imitation the ri
+00022d60: 6768 7473 2074 6f20 2020 2020 2020 207c  ghts to        |
+00022d70: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00022d80: 2020 2020 2020 7c20 2020 2020 2020 7573        |       us
+00022d90: 652c 2063 6f70 792c 206d 6f64 6966 792c  e, copy, modify,
+00022da0: 206d 6572 6765 2c20 7075 626c 6973 682c   merge, publish,
+00022db0: 2064 6973 7472 6962 7574 652c 2073 7562   distribute, sub
+00022dc0: 6c69 6365 6e73 652c 2061 6e64 2f6f 7220  license, and/or 
+00022dd0: 7365 6c6c 2063 6f70 6965 7320 6f66 2020  sell copies of  
+00022de0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+00022df0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00022e00: 2020 2074 6865 2053 6f66 7477 6172 652c     the Software,
+00022e10: 2061 6e64 2074 6f20 7065 726d 6974 2070   and to permit p
+00022e20: 6572 736f 6e73 2074 6f20 7768 6f6d 2074  ersons to whom t
+00022e30: 6865 2053 6f66 7477 6172 6520 6973 2066  he Software is f
+00022e40: 7572 6e69 7368 6564 2074 6f20 646f 2073  urnished to do s
+00022e50: 6f2c 2020 2020 2020 207c 0a7c 2020 2020  o,       |.|    
+00022e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022e70: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00022e80: 2020 2020 2020 2020 2020 2020 2020 7375                su
+00022e90: 626a 6563 7420 746f 2074 6865 2066 6f6c  bject to the fol
+00022ea0: 6c6f 7769 6e67 2063 6f6e 6469 7469 6f6e  lowing condition
+00022eb0: 733a 2020 2020 2020 2020 2020 2020 2020  s:              
+00022ec0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00022ed0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00022ee0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 00022ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022f00: 2020 2020 2020 2020 2043 6f70 7972 6967           Copyrig
-00022f10: 6874 204a 6173 6f6e 2052 2e20 436f 6f6d  ht Jason R. Coom
-00022f20: 6273 2020 2020 2020 2020 2020 2020 2020  bs              
+00022f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00022f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022f40: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00022f50: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00022f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022fb0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00022fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022fd0: 7c20 2020 2020 2020 2020 5065 726d 6973  |         Permis
-00022fe0: 7369 6f6e 2069 7320 6865 7265 6279 2067  sion is hereby g
-00022ff0: 7261 6e74 6564 2c20 6672 6565 206f 6620  ranted, free of 
-00023000: 6368 6172 6765 2c20 746f 2061 6e79 2070  charge, to any p
-00023010: 6572 736f 6e20 6f62 7461 696e 696e 6720  erson obtaining 
-00023020: 6120 636f 7079 2020 2020 2020 2020 7c0a  a copy        |.
-00023030: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00023040: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00023050: 206f 6620 7468 6973 2073 6f66 7477 6172   of this softwar
-00023060: 6520 616e 6420 6173 736f 6369 6174 6564  e and associated
-00023070: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
-00023080: 696c 6573 2028 7468 6520 2253 6f66 7477  iles (the "Softw
-00023090: 6172 6522 292c 2074 6f20 2020 2020 2020  are"), to       
-000230a0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-000230b0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000230c0: 2020 2020 2064 6561 6c20 696e 2074 6865       deal in the
-000230d0: 2053 6f66 7477 6172 6520 7769 7468 6f75   Software withou
-000230e0: 7420 7265 7374 7269 6374 696f 6e2c 2069  t restriction, i
-000230f0: 6e63 6c75 6469 6e67 2077 6974 686f 7574  ncluding without
-00023100: 206c 696d 6974 6174 696f 6e20 7468 6520   limitation the 
-00023110: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00023120: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00023130: 2020 2020 2020 2020 2072 6967 6874 7320           rights 
-00023140: 746f 2075 7365 2c20 636f 7079 2c20 6d6f  to use, copy, mo
-00023150: 6469 6679 2c20 6d65 7267 652c 2070 7562  dify, merge, pub
-00023160: 6c69 7368 2c20 6469 7374 7269 6275 7465  lish, distribute
-00023170: 2c20 7375 626c 6963 656e 7365 2c20 616e  , sublicense, an
-00023180: 642f 6f72 2020 2020 2020 2020 207c 0a7c  d/or         |.|
+00022f40: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+00022f50: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00022f60: 2020 2054 6865 2061 626f 7665 2063 6f70     The above cop
+00022f70: 7972 6967 6874 206e 6f74 6963 6520 616e  yright notice an
+00022f80: 6420 7468 6973 2070 6572 6d69 7373 696f  d this permissio
+00022f90: 6e20 6e6f 7469 6365 2073 6861 6c6c 2062  n notice shall b
+00022fa0: 6520 696e 636c 7564 6564 2069 6e20 616c  e included in al
+00022fb0: 6c20 2020 2020 2020 7c0a 7c20 2020 2020  l       |.|     
+00022fc0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00022fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022fe0: 2020 2020 2020 2063 6f70 6965 7320 6f72         copies or
+00022ff0: 2073 7562 7374 616e 7469 616c 2070 6f72   substantial por
+00023000: 7469 6f6e 7320 6f66 2074 6865 2053 6f66  tions of the Sof
+00023010: 7477 6172 652e 2020 2020 2020 2020 2020  tware.          
+00023020: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00023030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023040: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00023050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000230a0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+000230b0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+000230c0: 2020 2020 5448 4520 534f 4654 5741 5245      THE SOFTWARE
+000230d0: 2049 5320 5052 4f56 4944 4544 2022 4153   IS PROVIDED "AS
+000230e0: 2049 5322 2c20 5749 5448 4f55 5420 5741   IS", WITHOUT WA
+000230f0: 5252 414e 5459 204f 4620 414e 5920 4b49  RRANTY OF ANY KI
+00023100: 4e44 2c20 4558 5052 4553 5320 4f52 2020  ND, EXPRESS OR  
+00023110: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+00023120: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00023130: 2020 2020 2020 494d 504c 4945 442c 2049        IMPLIED, I
+00023140: 4e43 4c55 4449 4e47 2042 5554 204e 4f54  NCLUDING BUT NOT
+00023150: 204c 494d 4954 4544 2054 4f20 5448 4520   LIMITED TO THE 
+00023160: 5741 5252 414e 5449 4553 204f 4620 4d45  WARRANTIES OF ME
+00023170: 5243 4841 4e54 4142 494c 4954 592c 2046  RCHANTABILITY, F
+00023180: 4954 4e45 5353 2020 2020 2020 7c0a 7c20  ITNESS      |.| 
 00023190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000231a0: 2020 2020 7c20 2020 2020 2020 2020 2073      |          s
-000231b0: 656c 6c20 636f 7069 6573 206f 6620 7468  ell copies of th
-000231c0: 6520 536f 6674 7761 7265 2c20 616e 6420  e Software, and 
-000231d0: 746f 2070 6572 6d69 7420 7065 7273 6f6e  to permit person
-000231e0: 7320 746f 2077 686f 6d20 7468 6520 536f  s to whom the So
-000231f0: 6674 7761 7265 2069 7320 2020 2020 2020  ftware is       
-00023200: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00023210: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00023220: 2020 2020 2020 2020 2020 2020 2066 7572               fur
-00023230: 6e69 7368 6564 2074 6f20 646f 2073 6f2c  nished to do so,
-00023240: 2073 7562 6a65 6374 2074 6f20 7468 6520   subject to the 
-00023250: 666f 6c6c 6f77 696e 6720 636f 6e64 6974  following condit
-00023260: 696f 6e73 3a20 2020 2020 2020 2020 2020  ions:           
-00023270: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00023280: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00023290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000232e0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+000231a0: 2020 207c 2020 2020 2020 2020 464f 5220     |        FOR 
+000231b0: 4120 5041 5254 4943 554c 4152 2050 5552  A PARTICULAR PUR
+000231c0: 504f 5345 2041 4e44 204e 4f4e 494e 4652  POSE AND NONINFR
+000231d0: 494e 4745 4d45 4e54 2e20 494e 204e 4f20  INGEMENT. IN NO 
+000231e0: 4556 454e 5420 5348 414c 4c20 5448 4520  EVENT SHALL THE 
+000231f0: 4155 5448 4f52 5320 4f52 2020 2020 2020  AUTHORS OR      
+00023200: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00023210: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00023220: 2043 4f50 5952 4947 4854 2048 4f4c 4445   COPYRIGHT HOLDE
+00023230: 5253 2042 4520 4c49 4142 4c45 2046 4f52  RS BE LIABLE FOR
+00023240: 2041 4e59 2043 4c41 494d 2c20 4441 4d41   ANY CLAIM, DAMA
+00023250: 4745 5320 4f52 204f 5448 4552 204c 4941  GES OR OTHER LIA
+00023260: 4249 4c49 5459 2c20 5748 4554 4845 5220  BILITY, WHETHER 
+00023270: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+00023280: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+00023290: 2020 2020 2020 2020 2049 4e20 414e 2041           IN AN A
+000232a0: 4354 494f 4e20 4f46 2043 4f4e 5452 4143  CTION OF CONTRAC
+000232b0: 542c 2054 4f52 5420 4f52 204f 5448 4552  T, TORT OR OTHER
+000232c0: 5749 5345 2c20 4152 4953 494e 4720 4652  WISE, ARISING FR
+000232d0: 4f4d 2c20 4f55 5420 4f46 204f 5220 494e  OM, OUT OF OR IN
+000232e0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 000232f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023300: 2020 207c 2020 2020 2020 2020 2020 5468     |          Th
-00023310: 6520 6162 6f76 6520 636f 7079 7269 6768  e above copyrigh
-00023320: 7420 6e6f 7469 6365 2061 6e64 2074 6869  t notice and thi
-00023330: 7320 7065 726d 6973 7369 6f6e 206e 6f74  s permission not
-00023340: 6963 6520 7368 616c 6c20 6265 2069 6e63  ice shall be inc
-00023350: 6c75 6465 6420 696e 2020 2020 2020 2020  luded in        
-00023360: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00023370: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00023380: 2020 2020 2020 2020 2020 2020 2020 616c                al
-00023390: 6c20 636f 7069 6573 206f 7220 7375 6273  l copies or subs
-000233a0: 7461 6e74 6961 6c20 706f 7274 696f 6e73  tantial portions
-000233b0: 206f 6620 7468 6520 536f 6674 7761 7265   of the Software
-000233c0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-000233d0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-000233e0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-000233f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023440: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00023450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023460: 2020 7c20 2020 2020 2020 2020 2054 4845    |          THE
-00023470: 2053 4f46 5457 4152 4520 4953 2050 524f   SOFTWARE IS PRO
-00023480: 5649 4445 4420 2241 5320 4953 222c 2057  VIDED "AS IS", W
-00023490: 4954 484f 5554 2057 4152 5241 4e54 5920  ITHOUT WARRANTY 
-000234a0: 4f46 2041 4e59 204b 494e 442c 2045 5850  OF ANY KIND, EXP
-000234b0: 5245 5353 204f 5220 2020 2020 2020 2020  RESS OR         
-000234c0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-000234d0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-000234e0: 2020 2049 4d50 4c49 4544 2c20 494e 434c     IMPLIED, INCL
-000234f0: 5544 494e 4720 4255 5420 4e4f 5420 4c49  UDING BUT NOT LI
-00023500: 4d49 5445 4420 544f 2054 4845 2057 4152  MITED TO THE WAR
-00023510: 5241 4e54 4945 5320 4f46 204d 4552 4348  RANTIES OF MERCH
-00023520: 414e 5441 4249 4c49 5459 2c20 2020 2020  ANTABILITY,     
-00023530: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00023540: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00023550: 2020 2020 2020 4649 544e 4553 5320 464f        FITNESS FO
-00023560: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
-00023570: 5552 504f 5345 2041 4e44 204e 4f4e 494e  URPOSE AND NONIN
-00023580: 4652 494e 4745 4d45 4e54 2e20 494e 204e  FRINGEMENT. IN N
-00023590: 4f20 4556 454e 5420 5348 414c 4c20 5448  O EVENT SHALL TH
-000235a0: 4520 2020 2020 2020 2020 7c0a 7c20 2020  E         |.|   
+00023300: 2020 7c20 2020 2020 2020 2020 2043 4f4e    |          CON
+00023310: 4e45 4354 494f 4e20 5749 5448 2054 4845  NECTION WITH THE
+00023320: 2053 4f46 5457 4152 4520 4f52 2054 4845   SOFTWARE OR THE
+00023330: 2055 5345 204f 5220 4f54 4845 5220 4445   USE OR OTHER DE
+00023340: 414c 494e 4753 2049 4e20 5448 4520 534f  ALINGS IN THE SO
+00023350: 4654 5741 5245 2e20 2020 2020 2020 2020  FTWARE.         
+00023360: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00023370: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00023380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000233a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000233b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000233c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000233d0: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
+000233e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+000233f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023400: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023420: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023430: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023440: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020  ----------+.|   
+00023450: 2020 2075 726c 6c69 6233 2020 2020 2020     urllib3      
+00023460: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00023470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023480: 2020 2020 2020 2020 2020 204d 4954 204c             MIT L
+00023490: 6963 656e 7365 2020 2020 2020 2020 2020  icense          
+000234a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000234b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000234c0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+000234d0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+000234e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000234f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023500: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023530: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+00023540: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00023550: 2020 2020 2020 2020 2020 2020 2020 2043                 C
+00023560: 6f70 7972 6967 6874 2028 6329 2032 3030  opyright (c) 200
+00023570: 382d 3230 3230 2041 6e64 7265 7920 5065  8-2020 Andrey Pe
+00023580: 7472 6f76 2061 6e64 2063 6f6e 7472 6962  trov and contrib
+00023590: 7574 6f72 732e 2020 2020 2020 2020 2020  utors.          
+000235a0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
 000235b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000235c0: 207c 2020 2020 2020 2020 2020 2020 4155   |            AU
-000235d0: 5448 4f52 5320 4f52 2043 4f50 5952 4947  THORS OR COPYRIG
-000235e0: 4854 2048 4f4c 4445 5253 2042 4520 4c49  HT HOLDERS BE LI
-000235f0: 4142 4c45 2046 4f52 2041 4e59 2043 4c41  ABLE FOR ANY CLA
-00023600: 494d 2c20 4441 4d41 4745 5320 4f52 204f  IM, DAMAGES OR O
-00023610: 5448 4552 2020 2020 2020 2020 2020 207c  THER           |
-00023620: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00023630: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00023640: 2020 4c49 4142 494c 4954 592c 2057 4845    LIABILITY, WHE
-00023650: 5448 4552 2049 4e20 414e 2041 4354 494f  THER IN AN ACTIO
-00023660: 4e20 4f46 2043 4f4e 5452 4143 542c 2054  N OF CONTRACT, T
-00023670: 4f52 5420 4f52 204f 5448 4552 5749 5345  ORT OR OTHERWISE
-00023680: 2c20 4152 4953 494e 4720 2020 2020 2020  , ARISING       
-00023690: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-000236a0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000236b0: 2020 2020 2046 524f 4d2c 204f 5554 204f       FROM, OUT O
-000236c0: 4620 4f52 2049 4e20 434f 4e4e 4543 5449  F OR IN CONNECTI
-000236d0: 4f4e 2057 4954 4820 5448 4520 534f 4654  ON WITH THE SOFT
-000236e0: 5741 5245 204f 5220 5448 4520 5553 4520  WARE OR THE USE 
-000236f0: 4f52 204f 5448 4552 2044 4541 4c49 4e47  OR OTHER DEALING
-00023700: 5320 2020 2020 2020 207c 0a7c 2020 2020  S        |.|    
-00023710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023720: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00023730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023740: 2020 2020 2020 2020 494e 2054 4845 2053          IN THE S
-00023750: 4f46 5457 4152 452e 2020 2020 2020 2020  OFTWARE.        
-00023760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023770: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00023780: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00023790: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000237a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000237f0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-00023800: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00023810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00023820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00023830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00023840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00023850: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00023860: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020  --------+.|     
-00023870: 2020 2073 6978 2020 2020 2020 2020 207c     six         |
+000235c0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+000235d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000235e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000235f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023610: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00023620: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00023630: 2020 2020 207c 2020 2020 2020 2020 2050       |         P
+00023640: 6572 6d69 7373 696f 6e20 6973 2068 6572  ermission is her
+00023650: 6562 7920 6772 616e 7465 642c 2066 7265  eby granted, fre
+00023660: 6520 6f66 2063 6861 7267 652c 2074 6f20  e of charge, to 
+00023670: 616e 7920 7065 7273 6f6e 206f 6274 6169  any person obtai
+00023680: 6e69 6e67 2061 2063 6f70 7920 2020 2020  ning a copy     
+00023690: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+000236a0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+000236b0: 2020 206f 6620 7468 6973 2073 6f66 7477     of this softw
+000236c0: 6172 6520 616e 6420 6173 736f 6369 6174  are and associat
+000236d0: 6564 2064 6f63 756d 656e 7461 7469 6f6e  ed documentation
+000236e0: 2066 696c 6573 2028 7468 6520 2253 6f66   files (the "Sof
+000236f0: 7477 6172 6522 292c 2074 6f20 6465 616c  tware"), to deal
+00023700: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
+00023710: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00023720: 2020 2020 2020 2020 2069 6e20 7468 6520           in the 
+00023730: 536f 6674 7761 7265 2077 6974 686f 7574  Software without
+00023740: 2072 6573 7472 6963 7469 6f6e 2c20 696e   restriction, in
+00023750: 636c 7564 696e 6720 7769 7468 6f75 7420  cluding without 
+00023760: 6c69 6d69 7461 7469 6f6e 2074 6865 2072  limitation the r
+00023770: 6967 6874 7320 2020 2020 2020 207c 0a7c  ights        |.|
+00023780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023790: 2020 2020 7c20 2020 2020 2020 2020 2074      |          t
+000237a0: 6f20 7573 652c 2063 6f70 792c 206d 6f64  o use, copy, mod
+000237b0: 6966 792c 206d 6572 6765 2c20 7075 626c  ify, merge, publ
+000237c0: 6973 682c 2064 6973 7472 6962 7574 652c  ish, distribute,
+000237d0: 2073 7562 6c69 6365 6e73 652c 2061 6e64   sublicense, and
+000237e0: 2f6f 7220 7365 6c6c 2020 2020 2020 2020  /or sell        
+000237f0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+00023800: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00023810: 2020 2020 2020 636f 7069 6573 206f 6620        copies of 
+00023820: 7468 6520 536f 6674 7761 7265 2c20 616e  the Software, an
+00023830: 6420 746f 2070 6572 6d69 7420 7065 7273  d to permit pers
+00023840: 6f6e 7320 746f 2077 686f 6d20 7468 6520  ons to whom the 
+00023850: 536f 6674 7761 7265 2069 7320 2020 2020  Software is     
+00023860: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
+00023870: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
 00023880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023890: 2020 2020 2020 2020 2020 436f 7079 7269            Copyri
-000238a0: 6768 7420 2863 2920 3230 3130 2d32 3032  ght (c) 2010-202
-000238b0: 3020 4265 6e6a 616d 696e 2050 6574 6572  0 Benjamin Peter
-000238c0: 736f 6e20 2020 2020 2020 2020 2020 2020  son             
-000238d0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
+00023890: 2020 6675 726e 6973 6865 6420 746f 2064    furnished to d
+000238a0: 6f20 736f 2c20 7375 626a 6563 7420 746f  o so, subject to
+000238b0: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+000238c0: 6f6e 6469 7469 6f6e 733a 2020 2020 2020  onditions:      
+000238d0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
 000238e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000238f0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+000238f0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
 00023900: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00023910: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00023920: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00023930: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00023940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023950: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00023960: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00023970: 2050 6572 6d69 7373 696f 6e20 6973 2068   Permission is h
-00023980: 6572 6562 7920 6772 616e 7465 642c 2066  ereby granted, f
-00023990: 7265 6520 6f66 2063 6861 7267 652c 2074  ree of charge, t
-000239a0: 6f20 616e 7920 7065 7273 6f6e 206f 6274  o any person obt
-000239b0: 6169 6e69 6e67 2061 2063 6f70 7920 6f66  aining a copy of
-000239c0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-000239d0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000239e0: 2020 2020 2020 2074 6869 7320 736f 6674         this soft
-000239f0: 7761 7265 2061 6e64 2061 7373 6f63 6961  ware and associa
-00023a00: 7465 6420 646f 6375 6d65 6e74 6174 696f  ted documentatio
-00023a10: 6e20 6669 6c65 7320 2874 6865 2022 536f  n files (the "So
-00023a20: 6674 7761 7265 2229 2c20 746f 2064 6561  ftware"), to dea
-00023a30: 6c20 696e 2020 2020 2020 2020 7c0a 7c20  l in        |.| 
+00023950: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00023960: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00023970: 2054 6865 2061 626f 7665 2063 6f70 7972   The above copyr
+00023980: 6967 6874 206e 6f74 6963 6520 616e 6420  ight notice and 
+00023990: 7468 6973 2070 6572 6d69 7373 696f 6e20  this permission 
+000239a0: 6e6f 7469 6365 2073 6861 6c6c 2062 6520  notice shall be 
+000239b0: 696e 636c 7564 6564 2069 6e20 616c 6c20  included in all 
+000239c0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
+000239d0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
+000239e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000239f0: 2020 2020 2063 6f70 6965 7320 6f72 2073       copies or s
+00023a00: 7562 7374 616e 7469 616c 2070 6f72 7469  ubstantial porti
+00023a10: 6f6e 7320 6f66 2074 6865 2053 6f66 7477  ons of the Softw
+00023a20: 6172 652e 2020 2020 2020 2020 2020 2020  are.            
+00023a30: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 00023a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023a50: 2020 207c 2020 2020 2020 2020 2074 6865     |         the
-00023a60: 2053 6f66 7477 6172 6520 7769 7468 6f75   Software withou
-00023a70: 7420 7265 7374 7269 6374 696f 6e2c 2069  t restriction, i
-00023a80: 6e63 6c75 6469 6e67 2077 6974 686f 7574  ncluding without
-00023a90: 206c 696d 6974 6174 696f 6e20 7468 6520   limitation the 
-00023aa0: 7269 6768 7473 2074 6f20 2020 2020 2020  rights to       
-00023ab0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00023ac0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00023ad0: 7573 652c 2063 6f70 792c 206d 6f64 6966  use, copy, modif
-00023ae0: 792c 206d 6572 6765 2c20 7075 626c 6973  y, merge, publis
-00023af0: 682c 2064 6973 7472 6962 7574 652c 2073  h, distribute, s
-00023b00: 7562 6c69 6365 6e73 652c 2061 6e64 2f6f  ublicense, and/o
-00023b10: 7220 7365 6c6c 2063 6f70 6965 7320 6f66  r sell copies of
-00023b20: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00023b30: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00023b40: 2020 2020 2074 6865 2053 6f66 7477 6172       the Softwar
-00023b50: 652c 2061 6e64 2074 6f20 7065 726d 6974  e, and to permit
-00023b60: 2070 6572 736f 6e73 2074 6f20 7768 6f6d   persons to whom
-00023b70: 2074 6865 2053 6f66 7477 6172 6520 6973   the Software is
-00023b80: 2066 7572 6e69 7368 6564 2074 6f20 646f   furnished to do
-00023b90: 2073 6f2c 2020 2020 2020 207c 0a7c 2020   so,       |.|  
+00023a50: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00023a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023ab0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
+00023ac0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00023ad0: 2020 5448 4520 534f 4654 5741 5245 2049    THE SOFTWARE I
+00023ae0: 5320 5052 4f56 4944 4544 2022 4153 2049  S PROVIDED "AS I
+00023af0: 5322 2c20 5749 5448 4f55 5420 5741 5252  S", WITHOUT WARR
+00023b00: 414e 5459 204f 4620 414e 5920 4b49 4e44  ANTY OF ANY KIND
+00023b10: 2c20 4558 5052 4553 5320 4f52 2020 2020  , EXPRESS OR    
+00023b20: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
+00023b30: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00023b40: 2020 2020 2020 2020 494d 504c 4945 442c          IMPLIED,
+00023b50: 2049 4e43 4c55 4449 4e47 2042 5554 204e   INCLUDING BUT N
+00023b60: 4f54 204c 494d 4954 4544 2054 4f20 5448  OT LIMITED TO TH
+00023b70: 4520 5741 5252 414e 5449 4553 204f 4620  E WARRANTIES OF 
+00023b80: 4d45 5243 4841 4e54 4142 494c 4954 592c  MERCHANTABILITY,
+00023b90: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
 00023ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023bb0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00023bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023bd0: 7375 626a 6563 7420 746f 2074 6865 2066  subject to the f
-00023be0: 6f6c 6c6f 7769 6e67 2063 6f6e 6469 7469  ollowing conditi
-00023bf0: 6f6e 733a 2020 2020 2020 2020 2020 2020  ons:            
-00023c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c10: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00023c20: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00023c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023c80: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00023c90: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00023ca0: 2020 2020 2054 6865 2061 626f 7665 2063       The above c
-00023cb0: 6f70 7972 6967 6874 206e 6f74 6963 6520  opyright notice 
-00023cc0: 616e 6420 7468 6973 2070 6572 6d69 7373  and this permiss
-00023cd0: 696f 6e20 6e6f 7469 6365 2073 6861 6c6c  ion notice shall
-00023ce0: 2062 6520 696e 636c 7564 6564 2069 6e20   be included in 
-00023cf0: 616c 6c20 2020 2020 2020 7c0a 7c20 2020  all       |.|   
+00023bb0: 207c 2020 2020 2020 2020 2046 4954 4e45   |         FITNE
+00023bc0: 5353 2046 4f52 2041 2050 4152 5449 4355  SS FOR A PARTICU
+00023bd0: 4c41 5220 5055 5250 4f53 4520 414e 4420  LAR PURPOSE AND 
+00023be0: 4e4f 4e49 4e46 5249 4e47 454d 454e 542e  NONINFRINGEMENT.
+00023bf0: 2049 4e20 4e4f 2045 5645 4e54 2053 4841   IN NO EVENT SHA
+00023c00: 4c4c 2054 4845 2020 2020 2020 2020 207c  LL THE         |
+00023c10: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
+00023c20: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00023c30: 2020 2041 5554 484f 5253 204f 5220 434f     AUTHORS OR CO
+00023c40: 5059 5249 4748 5420 484f 4c44 4552 5320  PYRIGHT HOLDERS 
+00023c50: 4245 204c 4941 424c 4520 464f 5220 414e  BE LIABLE FOR AN
+00023c60: 5920 434c 4149 4d2c 2044 414d 4147 4553  Y CLAIM, DAMAGES
+00023c70: 204f 5220 4f54 4845 5220 2020 2020 2020   OR OTHER       
+00023c80: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+00023c90: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00023ca0: 2020 2020 4c49 4142 494c 4954 592c 2057      LIABILITY, W
+00023cb0: 4845 5448 4552 2049 4e20 414e 2041 4354  HETHER IN AN ACT
+00023cc0: 494f 4e20 4f46 2043 4f4e 5452 4143 542c  ION OF CONTRACT,
+00023cd0: 2054 4f52 5420 4f52 204f 5448 4552 5749   TORT OR OTHERWI
+00023ce0: 5345 2c20 4152 4953 494e 4720 4652 4f4d  SE, ARISING FROM
+00023cf0: 2c20 2020 2020 2020 207c 0a7c 2020 2020  ,        |.|    
 00023d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023d10: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00023d20: 2020 2020 2020 2020 2063 6f70 6965 7320           copies 
-00023d30: 6f72 2073 7562 7374 616e 7469 616c 2070  or substantial p
-00023d40: 6f72 7469 6f6e 7320 6f66 2074 6865 2053  ortions of the S
-00023d50: 6f66 7477 6172 652e 2020 2020 2020 2020  oftware.        
-00023d60: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00023d70: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00023d80: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00023d10: 7c20 2020 2020 2020 204f 5554 204f 4620  |        OUT OF 
+00023d20: 4f52 2049 4e20 434f 4e4e 4543 5449 4f4e  OR IN CONNECTION
+00023d30: 2057 4954 4820 5448 4520 534f 4654 5741   WITH THE SOFTWA
+00023d40: 5245 204f 5220 5448 4520 5553 4520 4f52  RE OR THE USE OR
+00023d50: 204f 5448 4552 2044 4541 4c49 4e47 5320   OTHER DEALINGS 
+00023d60: 494e 2054 4845 2020 2020 2020 2020 7c0a  IN THE        |.
+00023d70: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00023d80: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 00023d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00023da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023db0: 534f 4654 5741 5245 2e20 2020 2020 2020  SOFTWARE.       
 00023dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00023dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023de0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00023df0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00023e00: 2020 2020 2020 5448 4520 534f 4654 5741        THE SOFTWA
-00023e10: 5245 2049 5320 5052 4f56 4944 4544 2022  RE IS PROVIDED "
-00023e20: 4153 2049 5322 2c20 5749 5448 4f55 5420  AS IS", WITHOUT 
-00023e30: 5741 5252 414e 5459 204f 4620 414e 5920  WARRANTY OF ANY 
-00023e40: 4b49 4e44 2c20 4558 5052 4553 5320 4f52  KIND, EXPRESS OR
-00023e50: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00023e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00023e70: 7c20 2020 2020 2020 494d 504c 4945 442c  |       IMPLIED,
-00023e80: 2049 4e43 4c55 4449 4e47 2042 5554 204e   INCLUDING BUT N
-00023e90: 4f54 204c 494d 4954 4544 2054 4f20 5448  OT LIMITED TO TH
-00023ea0: 4520 5741 5252 414e 5449 4553 204f 4620  E WARRANTIES OF 
-00023eb0: 4d45 5243 4841 4e54 4142 494c 4954 592c  MERCHANTABILITY,
-00023ec0: 2046 4954 4e45 5353 2020 2020 2020 7c0a   FITNESS      |.
-00023ed0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00023ee0: 2020 2020 207c 2020 2020 2020 2020 464f       |        FO
-00023ef0: 5220 4120 5041 5254 4943 554c 4152 2050  R A PARTICULAR P
-00023f00: 5552 504f 5345 2041 4e44 204e 4f4e 494e  URPOSE AND NONIN
-00023f10: 4652 494e 4745 4d45 4e54 2e20 494e 204e  FRINGEMENT. IN N
-00023f20: 4f20 4556 454e 5420 5348 414c 4c20 5448  O EVENT SHALL TH
-00023f30: 4520 4155 5448 4f52 5320 4f52 2020 2020  E AUTHORS OR    
-00023f40: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00023f50: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00023f60: 2020 2043 4f50 5952 4947 4854 2048 4f4c     COPYRIGHT HOL
-00023f70: 4445 5253 2042 4520 4c49 4142 4c45 2046  DERS BE LIABLE F
-00023f80: 4f52 2041 4e59 2043 4c41 494d 2c20 4441  OR ANY CLAIM, DA
-00023f90: 4d41 4745 5320 4f52 204f 5448 4552 204c  MAGES OR OTHER L
-00023fa0: 4941 4249 4c49 5459 2c20 5748 4554 4845  IABILITY, WHETHE
-00023fb0: 5220 2020 2020 2020 7c0a 7c20 2020 2020  R       |.|     
-00023fc0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00023fd0: 2020 2020 2020 2020 2020 2049 4e20 414e             IN AN
-00023fe0: 2041 4354 494f 4e20 4f46 2043 4f4e 5452   ACTION OF CONTR
-00023ff0: 4143 542c 2054 4f52 5420 4f52 204f 5448  ACT, TORT OR OTH
-00024000: 4552 5749 5345 2c20 4152 4953 494e 4720  ERWISE, ARISING 
-00024010: 4652 4f4d 2c20 4f55 5420 4f46 204f 5220  FROM, OUT OF OR 
-00024020: 494e 2020 2020 2020 2020 2020 207c 0a7c  IN           |.|
-00024030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024040: 2020 2020 7c20 2020 2020 2020 2020 2043      |          C
-00024050: 4f4e 4e45 4354 494f 4e20 5749 5448 2054  ONNECTION WITH T
-00024060: 4845 2053 4f46 5457 4152 4520 4f52 2054  HE SOFTWARE OR T
-00024070: 4845 2055 5345 204f 5220 4f54 4845 5220  HE USE OR OTHER 
-00024080: 4445 414c 494e 4753 2049 4e20 5448 4520  DEALINGS IN THE 
-00024090: 534f 4654 5741 5245 2e20 2020 2020 2020  SOFTWARE.       
-000240a0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-000240b0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000240c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000240d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000240e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000240f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024110: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
-00024120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-00024130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00024140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00024150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00024160: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00024170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00024180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20  ------------+.| 
-00024190: 2020 2020 2074 6162 756c 6174 6520 2020       tabulate   
-000241a0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-000241b0: 2020 2020 2020 2043 6f70 7972 6967 6874         Copyright
-000241c0: 2028 6329 2032 3031 312d 3230 3230 2053   (c) 2011-2020 S
-000241d0: 6572 6765 7920 4173 7461 6e69 6e20 616e  ergey Astanin an
-000241e0: 6420 636f 6e74 7269 6275 746f 7273 2020  d contributors  
-000241f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024200: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00024210: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00024220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024270: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00024280: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00024290: 2020 2020 2020 2020 2020 5065 726d 6973            Permis
-000242a0: 7369 6f6e 2069 7320 6865 7265 6279 2067  sion is hereby g
-000242b0: 7261 6e74 6564 2c20 6672 6565 206f 6620  ranted, free of 
-000242c0: 6368 6172 6765 2c20 746f 2061 6e79 2070  charge, to any p
-000242d0: 6572 736f 6e20 6f62 7461 696e 696e 6720  erson obtaining 
-000242e0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-000242f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024300: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00024310: 2020 6120 636f 7079 206f 6620 7468 6973    a copy of this
-00024320: 2073 6f66 7477 6172 6520 616e 6420 6173   software and as
-00024330: 736f 6369 6174 6564 2064 6f63 756d 656e  sociated documen
-00024340: 7461 7469 6f6e 2066 696c 6573 2028 7468  tation files (th
-00024350: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-00024360: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00024370: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00024380: 2020 2020 2022 536f 6674 7761 7265 2229       "Software")
-00024390: 2c20 746f 2064 6561 6c20 696e 2074 6865  , to deal in the
-000243a0: 2053 6f66 7477 6172 6520 7769 7468 6f75   Software withou
-000243b0: 7420 7265 7374 7269 6374 696f 6e2c 2069  t restriction, i
-000243c0: 6e63 6c75 6469 6e67 2020 2020 2020 2020  ncluding        
-000243d0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-000243e0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000243f0: 2020 2020 2020 2020 2020 7769 7468 6f75            withou
-00024400: 7420 6c69 6d69 7461 7469 6f6e 2074 6865  t limitation the
-00024410: 2072 6967 6874 7320 746f 2075 7365 2c20   rights to use, 
-00024420: 636f 7079 2c20 6d6f 6469 6679 2c20 6d65  copy, modify, me
-00024430: 7267 652c 2070 7562 6c69 7368 2c20 2020  rge, publish,   
-00024440: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00024450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024460: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00024470: 6469 7374 7269 6275 7465 2c20 7375 626c  distribute, subl
-00024480: 6963 656e 7365 2c20 616e 642f 6f72 2073  icense, and/or s
-00024490: 656c 6c20 636f 7069 6573 206f 6620 7468  ell copies of th
-000244a0: 6520 536f 6674 7761 7265 2c20 616e 6420  e Software, and 
-000244b0: 746f 2020 2020 2020 2020 2020 2020 207c  to             |
-000244c0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-000244d0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000244e0: 2020 2070 6572 6d69 7420 7065 7273 6f6e     permit person
-000244f0: 7320 746f 2077 686f 6d20 7468 6520 536f  s to whom the So
-00024500: 6674 7761 7265 2069 7320 6675 726e 6973  ftware is furnis
-00024510: 6865 6420 746f 2064 6f20 736f 2c20 7375  hed to do so, su
-00024520: 626a 6563 7420 746f 2020 2020 2020 2020  bject to        
-00024530: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00024540: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00024550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024560: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00024570: 6520 666f 6c6c 6f77 696e 6720 636f 6e64  e following cond
-00024580: 6974 696f 6e73 3a20 2020 2020 2020 2020  itions:         
-00024590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000245a0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-000245b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000245c0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000245d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000245e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000245f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024610: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00024620: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00024630: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00024640: 2020 2020 2020 5468 6520 6162 6f76 6520        The above 
-00024650: 636f 7079 7269 6768 7420 6e6f 7469 6365  copyright notice
-00024660: 2061 6e64 2074 6869 7320 7065 726d 6973   and this permis
-00024670: 7369 6f6e 206e 6f74 6963 6520 7368 616c  sion notice shal
-00024680: 6c20 6265 2020 2020 2020 2020 2020 2020  l be            
-00024690: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-000246a0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000246b0: 2020 2020 2020 2020 2020 696e 636c 7564            includ
-000246c0: 6564 2069 6e20 616c 6c20 636f 7069 6573  ed in all copies
-000246d0: 206f 7220 7375 6273 7461 6e74 6961 6c20   or substantial 
-000246e0: 706f 7274 696f 6e73 206f 6620 7468 6520  portions of the 
-000246f0: 536f 6674 7761 7265 2e20 2020 2020 2020  Software.       
-00024700: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00024710: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00024720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024770: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00024780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024790: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-000247a0: 2020 2020 5448 4520 534f 4654 5741 5245      THE SOFTWARE
-000247b0: 2049 5320 5052 4f56 4944 4544 2022 4153   IS PROVIDED "AS
-000247c0: 2049 5322 2c20 5749 5448 4f55 5420 5741   IS", WITHOUT WA
-000247d0: 5252 414e 5459 204f 4620 414e 5920 4b49  RRANTY OF ANY KI
-000247e0: 4e44 2c20 2020 2020 2020 2020 2020 2020  ND,             
-000247f0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00024800: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00024810: 2020 2020 2020 2020 4558 5052 4553 5320          EXPRESS 
-00024820: 4f52 2049 4d50 4c49 4544 2c20 494e 434c  OR IMPLIED, INCL
-00024830: 5544 494e 4720 4255 5420 4e4f 5420 4c49  UDING BUT NOT LI
-00024840: 4d49 5445 4420 544f 2054 4845 2057 4152  MITED TO THE WAR
-00024850: 5241 4e54 4945 5320 4f46 2020 2020 2020  RANTIES OF      
-00024860: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00024870: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00024880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024890: 2020 204d 4552 4348 414e 5441 4249 4c49     MERCHANTABILI
-000248a0: 5459 2c20 4649 544e 4553 5320 464f 5220  TY, FITNESS FOR 
-000248b0: 4120 5041 5254 4943 554c 4152 2050 5552  A PARTICULAR PUR
-000248c0: 504f 5345 2041 4e44 2020 2020 2020 2020  POSE AND        
-000248d0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
+00023de0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
+00023df0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00023e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023e50: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
+00023e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00023e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a  -------------+..
+00023ed0: 5375 6d6d 6172 7920 6f66 2061 6c6c 206d  Summary of all m
+00023ee0: 6f64 756c 6573 2075 7365 6420 6279 2062  odules used by b
+00023ef0: 322c 2073 6869 7070 6564 2077 6974 6820  2, shipped with 
+00023f00: 6974 2069 6e20 6269 6e61 7279 2066 6f72  it in binary for
+00023f10: 6d3a 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  m:.+------------
+00023f20: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00023f30: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00023f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+00023f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023f80: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00023f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00023fc0: 2d2d 2d2d 2b0a 7c20 2020 204d 6f64 756c  ----+.|    Modul
+00023fd0: 6520 6e61 6d65 2020 2020 207c 2020 2056  e name     |   V
+00023fe0: 6572 7369 6f6e 2020 207c 2020 2020 2020  ersion   |      
+00023ff0: 2020 2020 2020 2020 2020 4c69 6365 6e73            Licens
+00024000: 6520 2020 2020 2020 2020 2020 2020 2020  e               
+00024010: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+00024020: 2020 2020 4175 7468 6f72 2020 2020 2020      Author      
+00024030: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
+00024040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024050: 2020 2020 2020 2020 5552 4c20 2020 2020          URL     
+00024060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024070: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+00024080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+00024090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+000240a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000240b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000240c0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+000240d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000240e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+000240f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024120: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020  ----------+.|   
+00024130: 2061 7267 636f 6d70 6c65 7465 2020 2020   argcomplete    
+00024140: 207c 2020 2020 332e 312e 3220 2020 207c   |    3.1.2    |
+00024150: 2020 2020 2020 2020 4170 6163 6865 2053          Apache S
+00024160: 6f66 7477 6172 6520 4c69 6365 6e73 6520  oftware License 
+00024170: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00024180: 2020 2020 2020 416e 6472 6579 204b 6973        Andrey Kis
+00024190: 6c79 756b 2020 2020 2020 2020 2020 2020  lyuk            
+000241a0: 2020 7c20 2020 2020 2020 2020 2068 7474    |          htt
+000241b0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000241c0: 6b69 736c 7975 6b2f 6172 6763 6f6d 706c  kislyuk/argcompl
+000241d0: 6574 6520 2020 2020 2020 2020 207c 0a2b  ete          |.+
+000241e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000241f0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00024200: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00024210: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024220: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00024230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024250: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00024260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024290: 2b0a 7c20 2020 2020 2020 6172 726f 7720  +.|       arrow 
+000242a0: 2020 2020 2020 207c 2020 2020 312e 322e         |    1.2.
+000242b0: 3320 2020 207c 2020 2020 2020 2020 4170  3    |        Ap
+000242c0: 6163 6865 2053 6f66 7477 6172 6520 4c69  ache Software Li
+000242d0: 6365 6e73 6520 2020 2020 2020 207c 2020  cense        |  
+000242e0: 2020 2020 2020 2020 2020 2020 2043 6872               Chr
+000242f0: 6973 2053 6d69 7468 2020 2020 2020 2020  is Smith        
+00024300: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00024310: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+00024320: 6172 726f 772e 7265 6164 7468 6564 6f63  arrow.readthedoc
+00024330: 732e 696f 2020 2020 2020 2020 2020 2020  s.io            
+00024340: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
+00024350: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+00024360: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00024370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024390: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+000243a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000243b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+000243c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000243d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000243e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000243f0: 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020 2020  ------+.|       
+00024400: 6232 7364 6b20 2020 2020 2020 207c 2020  b2sdk        |  
+00024410: 2020 322e 322e 3120 2020 207c 2020 2020    2.2.1    |    
+00024420: 2020 2020 2020 2020 2020 4d49 5420 4c69            MIT Li
+00024430: 6365 6e73 6520 2020 2020 2020 2020 2020  cense           
+00024440: 2020 207c 2020 4261 636b 626c 617a 6520     |  Backblaze 
+00024450: 496e 6320 3c73 7570 706f 7274 4062 6163  Inc <support@bac
+00024460: 6b62 6c61 7a65 2e63 6f6d 3e20 2020 7c20  kblaze.com>   | 
+00024470: 2020 2020 2020 2068 7474 7073 3a2f 2f67         https://g
+00024480: 6974 6875 622e 636f 6d2f 4261 636b 626c  ithub.com/Backbl
+00024490: 617a 652f 6232 2d73 646b 2d70 7974 686f  aze/b2-sdk-pytho
+000244a0: 6e20 2020 2020 2020 207c 0a2b 2d2d 2d2d  n        |.+----
+000244b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000244c0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  +-------------+-
+000244d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000244e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000244f0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00024500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024520: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
+00024530: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024540: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024550: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20  ------------+.| 
+00024560: 2020 2020 2063 6572 7469 6669 2020 2020       certifi    
+00024570: 2020 207c 2020 2032 3032 342e 322e 3220     |   2024.2.2 
+00024580: 207c 2020 4d6f 7a69 6c6c 6120 5075 626c   |  Mozilla Publ
+00024590: 6963 204c 6963 656e 7365 2032 2e30 2028  ic License 2.0 (
+000245a0: 4d50 4c20 322e 3029 207c 2020 2020 2020  MPL 2.0) |      
+000245b0: 2020 2020 2020 2020 4b65 6e6e 6574 6820          Kenneth 
+000245c0: 5265 6974 7a20 2020 2020 2020 2020 2020  Reitz           
+000245d0: 2020 2020 7c20 2020 2020 2020 2068 7474      |        htt
+000245e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000245f0: 6365 7274 6966 692f 7079 7468 6f6e 2d63  certifi/python-c
+00024600: 6572 7469 6669 2020 2020 2020 2020 207c  ertifi         |
+00024610: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+00024620: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00024630: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00024640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00024660: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024680: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00024690: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000246a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000246b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000246c0: 2d2d 2b0a 7c20 6368 6172 7365 742d 6e6f  --+.| charset-no
+000246d0: 726d 616c 697a 6572 207c 2020 2020 332e  rmalizer |    3.
+000246e0: 332e 3220 2020 207c 2020 2020 2020 2020  3.2    |        
+000246f0: 2020 2020 2020 4d49 5420 4c69 6365 6e73        MIT Licens
+00024700: 6520 2020 2020 2020 2020 2020 2020 207c  e              |
+00024710: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+00024720: 686d 6564 2054 4148 5249 2020 2020 2020  hmed TAHRI      
+00024730: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00024740: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
+00024750: 2e63 6f6d 2f4f 7573 7265 742f 6368 6172  .com/Ousret/char
+00024760: 7365 745f 6e6f 726d 616c 697a 6572 2020  set_normalizer  
+00024770: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
+00024780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00024790: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+000247a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000247b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000247c0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+000247d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000247e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+000247f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024810: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024820: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020  --------+.|     
+00024830: 2064 6f63 7574 696c 7320 2020 2020 207c   docutils      |
+00024840: 2020 2020 302e 3138 2e31 2020 207c 2020      0.18.1   |  
+00024850: 2020 2020 2020 2020 2020 2020 4253 4420              BSD 
+00024860: 4c69 6365 6e73 6520 2020 2020 2020 2020  License         
+00024870: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00024880: 2020 2020 4461 7669 6420 476f 6f64 6765      David Goodge
+00024890: 7220 2020 2020 2020 2020 2020 2020 2020  r               
+000248a0: 7c20 2020 2020 2020 2020 2020 2020 6874  |             ht
+000248b0: 7470 3a2f 2f64 6f63 7574 696c 732e 736f  tp://docutils.so
+000248c0: 7572 6365 666f 7267 652e 6e65 742f 2020  urceforge.net/  
+000248d0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
 000248e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000248f0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00024900: 4e4f 4e49 4e46 5249 4e47 454d 454e 542e  NONINFRINGEMENT.
-00024910: 2049 4e20 4e4f 2045 5645 4e54 2053 4841   IN NO EVENT SHA
-00024920: 4c4c 2054 4845 2041 5554 484f 5253 204f  LL THE AUTHORS O
-00024930: 5220 434f 5059 5249 4748 5420 484f 4c44  R COPYRIGHT HOLD
-00024940: 4552 5320 4245 2020 2020 2020 2020 2020  ERS BE          
-00024950: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00024960: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00024970: 2020 2020 204c 4941 424c 4520 464f 5220       LIABLE FOR 
-00024980: 414e 5920 434c 4149 4d2c 2044 414d 4147  ANY CLAIM, DAMAG
-00024990: 4553 204f 5220 4f54 4845 5220 4c49 4142  ES OR OTHER LIAB
-000249a0: 494c 4954 592c 2057 4845 5448 4552 2049  ILITY, WHETHER I
-000249b0: 4e20 414e 2041 4354 494f 4e20 2020 2020  N AN ACTION     
-000249c0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-000249d0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-000249e0: 2020 2020 2020 2020 2020 4f46 2043 4f4e            OF CON
-000249f0: 5452 4143 542c 2054 4f52 5420 4f52 204f  TRACT, TORT OR O
-00024a00: 5448 4552 5749 5345 2c20 4152 4953 494e  THERWISE, ARISIN
-00024a10: 4720 4652 4f4d 2c20 4f55 5420 4f46 204f  G FROM, OUT OF O
-00024a20: 5220 494e 2043 4f4e 4e45 4354 494f 4e20  R IN CONNECTION 
-00024a30: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00024a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024a50: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00024a60: 2020 5749 5448 2054 4845 2053 4f46 5457    WITH THE SOFTW
-00024a70: 4152 4520 4f52 2054 4845 2055 5345 204f  ARE OR THE USE O
-00024a80: 5220 4f54 4845 5220 4445 414c 494e 4753  R OTHER DEALINGS
-00024a90: 2049 4e20 5448 4520 534f 4654 5741 5245   IN THE SOFTWARE
-00024aa0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
-00024ab0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00024ac0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+000248f0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00024900: 7c20 2020 2047 4e55 2047 656e 6572 616c  |    GNU General
+00024910: 2050 7562 6c69 6320 4c69 6365 6e73 6520   Public License 
+00024920: 2847 504c 2920 2020 7c20 2020 2020 2020  (GPL)   |       
+00024930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024950: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+00024960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024980: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+00024990: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+000249a0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+000249b0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+000249c0: 2020 5075 626c 6963 2044 6f6d 6169 6e20    Public Domain 
+000249d0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+000249e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000249f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024a00: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00024a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024a40: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
+00024a50: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
+00024a60: 2020 2020 2020 7c20 2020 5079 7468 6f6e        |   Python
+00024a70: 2053 6f66 7477 6172 6520 466f 756e 6461   Software Founda
+00024a80: 7469 6f6e 204c 6963 656e 7365 2020 7c20  tion License  | 
+00024a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00024ab0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00024ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00024ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00024ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024b20: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
-00024b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00024b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024af0: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
+00024b00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00024b10: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+00024b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024b40: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
 00024b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00024b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024b60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
 00024b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
 00024b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00024b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020  ----------+.|   
-00024ba0: 2020 2020 2074 7164 6d20 2020 2020 2020       tqdm       
-00024bb0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00024bc0: 2020 2020 2020 2020 2020 2020 6074 7164              `tqd
-00024bd0: 6d60 2069 7320 6120 7072 6f64 7563 7420  m` is a product 
-00024be0: 6f66 2063 6f6c 6c61 626f 7261 7469 7665  of collaborative
-00024bf0: 2077 6f72 6b2e 2020 2020 2020 2020 2020   work.          
-00024c00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00024c10: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00024c20: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00024c30: 2020 556e 6c65 7373 206f 7468 6572 7769    Unless otherwi
-00024c40: 7365 2073 7461 7465 642c 2061 6c6c 2061  se stated, all a
-00024c50: 7574 686f 7273 2028 7365 6520 636f 6d6d  uthors (see comm
-00024c60: 6974 206c 6f67 7329 2072 6574 6169 6e20  it logs) retain 
-00024c70: 636f 7079 7269 6768 7420 2020 2020 2020  copyright       
-00024c80: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00024c90: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00024ca0: 2020 2020 2020 2020 666f 7220 7468 6569          for thei
-00024cb0: 7220 7265 7370 6563 7469 7665 2077 6f72  r respective wor
-00024cc0: 6b2c 2061 6e64 2072 656c 6561 7365 2074  k, and release t
-00024cd0: 6865 2077 6f72 6b20 756e 6465 7220 7468  he work under th
-00024ce0: 6520 4d49 5420 6c69 6365 6e63 6520 2020  e MIT licence   
-00024cf0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00024d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024d10: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00024d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024d30: 2020 2020 2020 2020 2028 7465 7874 2062           (text b
-00024d40: 656c 6f77 292e 2020 2020 2020 2020 2020  elow).          
-00024d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024d60: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00024d70: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00024d80: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00024d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024de0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00024df0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00024e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e10: 2020 2045 7863 6570 7469 6f6e 7320 6f72     Exceptions or
-00024e20: 206e 6f74 6162 6c65 2061 7574 686f 7273   notable authors
-00024e30: 2061 7265 206c 6973 7465 6420 6265 6c6f   are listed belo
-00024e40: 7720 2020 2020 2020 2020 2020 2020 2020  w               
-00024e50: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00024e60: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00024e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024e80: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00024e90: 6e20 7265 7665 7273 6520 6368 726f 6e6f  n reverse chrono
-00024ea0: 6c6f 6769 6361 6c20 6f72 6465 723a 2020  logical order:  
-00024eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024ec0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00024ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024ee0: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00024ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f40: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00024f50: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00024f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024f80: 2020 2020 2a20 6669 6c65 733a 202a 2020      * files: *  
-00024f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024fb0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00024fc0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00024fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00024fe0: 2020 2020 2020 2020 2020 4d50 4c76 322e            MPLv2.
-00024ff0: 3020 3230 3135 2d32 3032 3320 2863 2920  0 2015-2023 (c) 
-00025000: 4361 7370 6572 2064 6120 436f 7374 612d  Casper da Costa-
-00025010: 4c75 6973 2020 2020 2020 2020 2020 2020  Luis            
-00025020: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00025030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025040: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00025050: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00025060: 6361 7370 6572 6463 6c5d 2868 7474 7073  casperdcl](https
-00025070: 3a2f 2f67 6974 6875 622e 636f 6d2f 6361  ://github.com/ca
-00025080: 7370 6572 6463 6c29 2e20 2020 2020 2020  sperdcl).       
+00024b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024ba0: 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020 2020  -------+.|      
+00024bb0: 2020 6964 6e61 2020 2020 2020 2020 7c20    idna        | 
+00024bc0: 2020 2020 332e 3620 2020 2020 7c20 2020      3.6     |   
+00024bd0: 2020 2020 2020 2020 2020 2042 5344 204c             BSD L
+00024be0: 6963 656e 7365 2020 2020 2020 2020 2020  icense          
+00024bf0: 2020 2020 7c20 2020 204b 696d 2044 6176      |    Kim Dav
+00024c00: 6965 7320 3c6b 696d 2b70 7970 6940 6775  ies <kim+pypi@gu
+00024c10: 6d6c 6561 662e 6f72 673e 2020 2020 207c  mleaf.org>     |
+00024c20: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00024c30: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00024c40: 6d2f 6b6a 642f 6964 6e61 2020 2020 2020  m/kjd/idna      
+00024c50: 2020 2020 2020 2020 2020 7c0a 2b2d 2d2d            |.+---
+00024c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024c70: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  -+-------------+
+00024c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024c90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024ca0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00024cb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024cd0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00024ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
+00024d10: 2020 2020 2020 6c6f 6766 7572 7920 2020        logfury   
+00024d20: 2020 2020 7c20 2020 2031 2e30 2e31 2020      |    1.0.1  
+00024d30: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00024d40: 2042 5344 204c 6963 656e 7365 2020 2020   BSD License    
+00024d50: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00024d60: 2020 2020 2020 2020 2050 6177 656c 2050           Pawel P
+00024d70: 6f6c 6577 6963 7a20 2020 2020 2020 2020  olewicz         
+00024d80: 2020 2020 207c 2020 2020 2020 2068 7474       |       htt
+00024d90: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00024da0: 7265 6566 2d74 6563 686e 6f6c 6f67 6965  reef-technologie
+00024db0: 732f 6c6f 6766 7572 7920 2020 2020 2020  s/logfury       
+00024dc0: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
+00024dd0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00024de0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00024df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00024e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024e30: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00024e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024e70: 2d2d 2d2b 0a7c 2070 6878 2d63 6c61 7373  ---+.| phx-class
+00024e80: 2d72 6567 6973 7472 7920 7c20 2020 2034  -registry |    4
+00024e90: 2e30 2e36 2020 2020 7c20 2020 2020 2020  .0.6    |       
+00024ea0: 2020 2020 2020 204d 4954 204c 6963 656e         MIT Licen
+00024eb0: 7365 2020 2020 2020 2020 2020 2020 2020  se              
+00024ec0: 7c20 2020 2020 2020 2050 686f 656e 6978  |        Phoenix
+00024ed0: 205a 6572 696e 203c 7068 7840 7068 782e   Zerin <phx@phx.
+00024ee0: 6e7a 3e20 2020 2020 2020 207c 2020 2020  nz>        |    
+00024ef0: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
+00024f00: 2e63 6f6d 2f74 6f64 6f66 6978 7468 6973  .com/todofixthis
+00024f10: 2f63 6c61 7373 2d72 6567 6973 7472 7920  /class-registry 
+00024f20: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
+00024f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00024f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00024f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024f60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024f70: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+00024f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+00024fa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024fb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024fc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00024fd0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020 7079  ---------+.|  py
+00024fe0: 7468 6f6e 2d64 6174 6575 7469 6c20 2020  thon-dateutil   
+00024ff0: 7c20 322e 392e 302e 706f 7374 3020 7c20  | 2.9.0.post0 | 
+00025000: 2020 2020 2020 2041 7061 6368 6520 536f         Apache So
+00025010: 6674 7761 7265 204c 6963 656e 7365 2020  ftware License  
+00025020: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00025030: 2020 2020 4775 7374 6176 6f20 4e69 656d      Gustavo Niem
+00025040: 6579 6572 2020 2020 2020 2020 2020 2020  eyer            
+00025050: 207c 2020 2020 2020 2020 2020 2068 7474   |           htt
+00025060: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00025070: 6461 7465 7574 696c 2f64 6174 6575 7469  dateutil/dateuti
+00025080: 6c20 2020 2020 2020 2020 2020 7c0a 7c20  l           |.| 
 00025090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000250a0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-000250b0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000250c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000250d0: 2020 2020 2020 2020 2020 2020 202a 2066               * f
-000250e0: 696c 6573 3a20 7471 646d 2f5f 7471 646d  iles: tqdm/_tqdm
-000250f0: 2e70 7920 2020 2020 2020 2020 2020 2020  .py             
-00025100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025110: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00025120: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00025130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025140: 2020 2020 2020 204d 4954 2032 3031 3620         MIT 2016 
-00025150: 2863 2920 5b50 5220 2339 365d 206f 6e20  (c) [PR #96] on 
-00025160: 6265 6861 6c66 206f 6620 476f 6f67 6c65  behalf of Google
-00025170: 2049 6e63 2e20 2020 2020 2020 2020 2020   Inc.           
-00025180: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00025190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000251a0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-000251b0: 202a 2066 696c 6573 3a20 7471 646d 2f5f   * files: tqdm/_
-000251c0: 7471 646d 2e70 7920 7365 7475 702e 7079  tqdm.py setup.py
-000251d0: 2052 4541 444d 452e 7273 7420 4d41 4e49   README.rst MANI
-000251e0: 4645 5354 2e69 6e20 2e67 6974 6967 6e6f  FEST.in .gitigno
-000251f0: 7265 2020 2020 2020 2020 2020 2020 2020  re              
-00025200: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00025210: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00025220: 2020 2020 2020 2020 2020 2020 2020 204d                 M
-00025230: 4954 2032 3031 3320 2863 2920 4e6f 616d  IT 2013 (c) Noam
-00025240: 2059 6f72 6176 2d52 6170 6861 656c 2c20   Yorav-Raphael, 
-00025250: 6f72 6967 696e 616c 2061 7574 686f 722e  original author.
-00025260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025270: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00025280: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00025290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000252a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000252b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000252c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000252d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000252e0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-000252f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025300: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00025310: 2020 2020 2020 2020 2020 5b50 5220 2339            [PR #9
-00025320: 365d 3a20 6874 7470 733a 2f2f 6769 7468  6]: https://gith
-00025330: 7562 2e63 6f6d 2f74 7164 6d2f 7471 646d  ub.com/tqdm/tqdm
-00025340: 2f70 756c 6c2f 3936 2020 2020 2020 2020  /pull/96        
-00025350: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00025360: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00025370: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00025380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000253a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000253b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000250a0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+000250b0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
+000250c0: 2042 5344 204c 6963 656e 7365 2020 2020   BSD License    
+000250d0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+000250e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000250f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025100: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00025110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025130: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+00025140: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
+00025150: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00025160: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00025170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025180: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00025190: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000251a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000251b0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+000251c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000251d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000251e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000251f0: 2d2d 2b0a 7c20 2020 2020 2072 6571 7565  --+.|      reque
+00025200: 7374 7320 2020 2020 207c 2020 2020 322e  sts      |    2.
+00025210: 3331 2e30 2020 207c 2020 2020 2020 2020  31.0   |        
+00025220: 4170 6163 6865 2053 6f66 7477 6172 6520  Apache Software 
+00025230: 4c69 6365 6e73 6520 2020 2020 2020 207c  License        |
+00025240: 2020 2020 2020 2020 2020 2020 2020 4b65                Ke
+00025250: 6e6e 6574 6820 5265 6974 7a20 2020 2020  nneth Reitz     
+00025260: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+00025270: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+00025280: 7265 7175 6573 7473 2e72 6561 6474 6865  requests.readthe
+00025290: 646f 6373 2e69 6f20 2020 2020 2020 2020  docs.io         
+000252a0: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
+000252b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+000252c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
+000252d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000252e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000252f0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00025300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025310: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00025320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025340: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025350: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020  --------+.|     
+00025360: 2072 7374 3261 6e73 6920 2020 2020 207c   rst2ansi      |
+00025370: 2020 2020 302e 312e 3520 2020 207c 2020      0.1.5    |  
+00025380: 2020 2020 2020 2020 2020 2020 4d49 5420              MIT 
+00025390: 4c69 6365 6e73 6520 2020 2020 2020 2020  License         
+000253a0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+000253b0: 2020 2020 2020 2020 536e 6169 7065 2020          Snaipe  
 000253c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000253d0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-000253e0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000253f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025440: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00025450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025460: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00025470: 2020 2020 2020 2020 4d6f 7a69 6c6c 6120          Mozilla 
-00025480: 5075 626c 6963 204c 6963 656e 6365 2028  Public Licence (
-00025490: 4d50 4c29 2076 2e20 322e 3020 2d20 4578  MPL) v. 2.0 - Ex
-000254a0: 6869 6269 7420 4120 2020 2020 2020 2020  hibit A         
-000254b0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-000254c0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000254d0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000254e0: 2020 2020 2020 2020 2020 2020 202d 2d2d               ---
-000254f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00025500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00025510: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2020 2020  ------------    
-00025520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025530: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00025540: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00025550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000255a0: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-000255b0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000255c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000255d0: 2020 2020 2054 6869 7320 536f 7572 6365       This Source
-000255e0: 2043 6f64 6520 466f 726d 2069 7320 7375   Code Form is su
-000255f0: 626a 6563 7420 746f 2074 6865 2074 6572  bject to the ter
-00025600: 6d73 206f 6620 7468 6520 2020 2020 2020  ms of the       
-00025610: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00025620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025630: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00025640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025650: 2020 2020 4d6f 7a69 6c6c 6120 5075 626c      Mozilla Publ
-00025660: 6963 204c 6963 656e 7365 2c20 762e 2032  ic License, v. 2
-00025670: 2e30 2e20 2020 2020 2020 2020 2020 2020  .0.             
-00025680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025690: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-000256a0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000256b0: 2020 2020 2020 2020 2020 2049 6620 6120             If a 
-000256c0: 636f 7079 206f 6620 7468 6520 4d50 4c20  copy of the MPL 
-000256d0: 7761 7320 6e6f 7420 6469 7374 7269 6275  was not distribu
-000256e0: 7465 6420 7769 7468 2074 6869 7320 7072  ted with this pr
-000256f0: 6f6a 6563 742c 2020 2020 2020 2020 2020  oject,          
-00025700: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00025710: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00025720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025730: 2020 2020 596f 7520 6361 6e20 6f62 7461      You can obta
-00025740: 696e 206f 6e65 2061 7420 6874 7470 733a  in one at https:
-00025750: 2f2f 6d6f 7a69 6c6c 612e 6f72 672f 4d50  //mozilla.org/MP
-00025760: 4c2f 322e 302f 2e20 2020 2020 2020 2020  L/2.0/.         
-00025770: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00025780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025790: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-000257a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000257f0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00025800: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00025810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000253d0: 7c20 2020 2020 2020 6874 7470 733a 2f2f  |       https://
+000253e0: 6769 7468 7562 2e63 6f6d 2f53 6e61 6970  github.com/Snaip
+000253f0: 652f 7079 7468 6f6e 2d72 7374 2d74 6f2d  e/python-rst-to-
+00025400: 616e 7369 2020 2020 2020 207c 0a2b 2d2d  ansi       |.+--
+00025410: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025420: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
+00025430: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
+00025440: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025450: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00025460: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025470: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025480: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+00025490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000254a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000254b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
+000254c0: 7c20 2020 2020 2020 2073 6978 2020 2020  |        six    
+000254d0: 2020 2020 207c 2020 2020 312e 3136 2e30       |    1.16.0
+000254e0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
+000254f0: 2020 4d49 5420 4c69 6365 6e73 6520 2020    MIT License   
+00025500: 2020 2020 2020 2020 2020 207c 2020 2020             |    
+00025510: 2020 2020 2020 2020 4265 6e6a 616d 696e          Benjamin
+00025520: 2050 6574 6572 736f 6e20 2020 2020 2020   Peterson       
+00025530: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
+00025540: 2020 2020 6874 7470 733a 2f2f 6769 7468      https://gith
+00025550: 7562 2e63 6f6d 2f62 656e 6a61 6d69 6e70  ub.com/benjaminp
+00025560: 2f73 6978 2020 2020 2020 2020 2020 2020  /six            
+00025570: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
+00025580: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00025590: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+000255a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000255b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+000255c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000255d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000255e0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
+000255f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025620: 2d2d 2d2d 2b0a 7c20 2020 2020 2074 6162  ----+.|      tab
+00025630: 756c 6174 6520 2020 2020 207c 2020 2020  ulate      |    
+00025640: 302e 392e 3020 2020 207c 2020 2020 2020  0.9.0    |      
+00025650: 2020 2020 2020 2020 4d49 5420 4c69 6365          MIT Lice
+00025660: 6e73 6520 2020 2020 2020 2020 2020 2020  nse             
+00025670: 207c 2020 2053 6572 6765 7920 4173 7461   |   Sergey Asta
+00025680: 6e69 6e20 3c73 2e61 7374 616e 696e 4067  nin <s.astanin@g
+00025690: 6d61 696c 2e63 6f6d 3e20 2020 7c20 2020  mail.com>   |   
+000256a0: 2020 2020 2068 7474 7073 3a2f 2f67 6974       https://git
+000256b0: 6875 622e 636f 6d2f 6173 7461 6e69 6e2f  hub.com/astanin/
+000256c0: 7079 7468 6f6e 2d74 6162 756c 6174 6520  python-tabulate 
+000256d0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
+000256e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+000256f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
+00025700: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025710: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025720: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00025730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025740: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00025750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025770: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025780: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020  ----------+.|   
+00025790: 2020 2020 2074 7164 6d20 2020 2020 2020       tqdm       
+000257a0: 207c 2020 2020 342e 3636 2e32 2020 207c   |    4.66.2   |
+000257b0: 2020 2020 2020 2020 2020 2020 2020 4d49                MI
+000257c0: 5420 4c69 6365 6e73 6520 2020 2020 2020  T License       
+000257d0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+000257e0: 2020 2020 2020 2020 2055 4e4b 4e4f 574e           UNKNOWN
+000257f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025800: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
+00025810: 2020 2020 2068 7474 7073 3a2f 2f74 7164       https://tqd
+00025820: 6d2e 6769 7468 7562 2e69 6f20 2020 2020  m.github.io     
+00025830: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
 00025840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025860: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00025870: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00025880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025850: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+00025860: 2020 7c20 204d 6f7a 696c 6c61 2050 7562    |  Mozilla Pub
+00025870: 6c69 6320 4c69 6365 6e73 6520 322e 3020  lic License 2.0 
+00025880: 284d 504c 2032 2e30 2920 7c20 2020 2020  (MPL 2.0) |     
 00025890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000258a0: 2020 2020 4d49 5420 4c69 6365 6e73 6520      MIT License 
-000258b0: 284d 4954 2920 2020 2020 2020 2020 2020  (MIT)           
+000258a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000258b0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
 000258c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000258d0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+000258d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000258e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000258f0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00025900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025910: 2020 2020 2020 2020 202d 2d2d 2d2d 2d2d           -------
-00025920: 2d2d 2d2d 2d2d 2d2d 2d2d 2020 2020 2020  ----------      
-00025930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025950: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00025960: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00025970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000259a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000259b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000259c0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-000259d0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000259e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000259f0: 2020 2020 2020 2020 2020 2020 2020 436f                Co
-00025a00: 7079 7269 6768 7420 2863 2920 3230 3133  pyright (c) 2013
-00025a10: 206e 6f61 6d72 6170 6820 2020 2020 2020   noamraph       
-00025a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a30: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00025a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a50: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00025a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025aa0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00025ab0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00025ac0: 2020 2020 2020 7c20 2020 2020 2020 5065        |       Pe
-00025ad0: 726d 6973 7369 6f6e 2069 7320 6865 7265  rmission is here
-00025ae0: 6279 2067 7261 6e74 6564 2c20 6672 6565  by granted, free
-00025af0: 206f 6620 6368 6172 6765 2c20 746f 2061   of charge, to a
-00025b00: 6e79 2070 6572 736f 6e20 6f62 7461 696e  ny person obtain
-00025b10: 696e 6720 6120 636f 7079 206f 6620 2020  ing a copy of   
-00025b20: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00025b30: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00025b40: 2020 2020 7468 6973 2073 6f66 7477 6172      this softwar
-00025b50: 6520 616e 6420 6173 736f 6369 6174 6564  e and associated
-00025b60: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
-00025b70: 696c 6573 2028 7468 6520 2253 6f66 7477  iles (the "Softw
-00025b80: 6172 6522 292c 2074 6f20 6465 616c 2069  are"), to deal i
-00025b90: 6e20 2020 2020 2020 207c 0a7c 2020 2020  n        |.|    
-00025ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025bb0: 7c20 2020 2020 2020 2020 7468 6520 536f  |         the So
-00025bc0: 6674 7761 7265 2077 6974 686f 7574 2072  ftware without r
-00025bd0: 6573 7472 6963 7469 6f6e 2c20 696e 636c  estriction, incl
-00025be0: 7564 696e 6720 7769 7468 6f75 7420 6c69  uding without li
-00025bf0: 6d69 7461 7469 6f6e 2074 6865 2072 6967  mitation the rig
-00025c00: 6874 7320 746f 2020 2020 2020 2020 7c0a  hts to        |.
-00025c10: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00025c20: 2020 2020 207c 2020 2020 2020 2075 7365       |       use
-00025c30: 2c20 636f 7079 2c20 6d6f 6469 6679 2c20  , copy, modify, 
-00025c40: 6d65 7267 652c 2070 7562 6c69 7368 2c20  merge, publish, 
-00025c50: 6469 7374 7269 6275 7465 2c20 7375 626c  distribute, subl
-00025c60: 6963 656e 7365 2c20 616e 642f 6f72 2073  icense, and/or s
-00025c70: 656c 6c20 636f 7069 6573 206f 6620 2020  ell copies of   
-00025c80: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00025c90: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00025ca0: 2020 7468 6520 536f 6674 7761 7265 2c20    the Software, 
-00025cb0: 616e 6420 746f 2070 6572 6d69 7420 7065  and to permit pe
-00025cc0: 7273 6f6e 7320 746f 2077 686f 6d20 7468  rsons to whom th
-00025cd0: 6520 536f 6674 7761 7265 2069 7320 6675  e Software is fu
-00025ce0: 726e 6973 6865 6420 746f 2064 6f20 736f  rnished to do so
-00025cf0: 2c20 2020 2020 2020 7c0a 7c20 2020 2020  ,       |.|     
-00025d00: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00025d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d20: 2020 2020 2020 2020 2020 2020 2073 7562               sub
-00025d30: 6a65 6374 2074 6f20 7468 6520 666f 6c6c  ject to the foll
-00025d40: 6f77 696e 6720 636f 6e64 6974 696f 6e73  owing conditions
-00025d50: 3a20 2020 2020 2020 2020 2020 2020 2020  :               
-00025d60: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00025d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025d80: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
+000258f0: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
+00025900: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
+00025910: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
+00025920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00025940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025960: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
+00025970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000259a0: 2d2d 2d2b 0a7c 2020 2020 2020 7572 6c6c  ---+.|      urll
+000259b0: 6962 3320 2020 2020 2020 7c20 2020 2032  ib3       |    2
+000259c0: 2e30 2e37 2020 2020 7c20 2020 2020 2020  .0.7    |       
+000259d0: 2020 2020 2020 204d 4954 204c 6963 656e         MIT Licen
+000259e0: 7365 2020 2020 2020 2020 2020 2020 2020  se              
+000259f0: 7c20 416e 6472 6579 2050 6574 726f 7620  | Andrey Petrov 
+00025a00: 3c61 6e64 7265 792e 7065 7472 6f76 4073  <andrey.petrov@s
+00025a10: 6861 7a6f 772e 6e65 743e 207c 2068 7474  hazow.net> | htt
+00025a20: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00025a30: 7572 6c6c 6962 332f 7572 6c6c 6962 332f  urllib3/urllib3/
+00025a40: 626c 6f62 2f6d 6169 6e2f 4348 414e 4745  blob/main/CHANGE
+00025a50: 532e 7273 7420 7c0a 2b2d 2d2d 2d2d 2d2d  S.rst |.+-------
+00025a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
+00025a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
+00025a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025aa0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
+00025ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025ac0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
+00025ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025b00: 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a 5468 6972  ---------+..Thir
+00025b10: 6420 7061 7274 7920 6c69 6272 6172 6965  d party librarie
+00025b20: 7320 6d6f 6469 6669 6564 2061 6e64 2069  s modified and i
+00025b30: 6e63 6c75 6465 6420 696e 2062 3220 6f72  ncluded in b2 or
+00025b40: 2062 3273 646b 3a0a 0a72 6571 7565 7374   b2sdk:..request
+00025b50: 730a 496e 636c 7564 6564 2069 6e20 6120  s.Included in a 
+00025b60: 7265 7669 7365 6420 666f 726d 0a46 696c  revised form.Fil
+00025b70: 6573 2069 6e63 6c75 6465 6420 666f 7220  es included for 
+00025b80: 6c65 6761 6c20 636f 6d70 6c69 616e 6365  legal compliance
+00025b90: 2072 6561 736f 6e73 3a0a 2b2d 2d2d 2d2d   reasons:.+-----
+00025ba0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
+00025bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025bc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
+00025c20: 0a7c 2046 696c 6520 6e61 6d65 207c 2020  .| File name |  
+00025c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025c60: 2020 2020 2020 436f 6e74 656e 7420 2020        Content   
+00025c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025ca0: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
+00025cb0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
+00025cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025cf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00025d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
+00025d30: 2020 204e 4f54 4943 4520 207c 2020 2020     NOTICE  |    
+00025d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025d70: 2020 2020 5265 7175 6573 7473 2020 2020      Requests    
+00025d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00025d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00025da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025db0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
+00025dc0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
 00025dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025de0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00025df0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00025e00: 2020 5468 6520 6162 6f76 6520 636f 7079    The above copy
-00025e10: 7269 6768 7420 6e6f 7469 6365 2061 6e64  right notice and
-00025e20: 2074 6869 7320 7065 726d 6973 7369 6f6e   this permission
-00025e30: 206e 6f74 6963 6520 7368 616c 6c20 6265   notice shall be
-00025e40: 2069 6e63 6c75 6465 6420 696e 2061 6c6c   included in all
-00025e50: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00025e60: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
+00025de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025df0: 2043 6f70 7972 6967 6874 2032 3031 3920   Copyright 2019 
+00025e00: 4b65 6e6e 6574 6820 5265 6974 7a20 2020  Kenneth Reitz   
+00025e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e30: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
+00025e40: 2020 2020 2020 2020 207c 2020 2020 2020           |      
+00025e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00025e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025e80: 2020 2020 2020 636f 7069 6573 206f 7220        copies or 
-00025e90: 7375 6273 7461 6e74 6961 6c20 706f 7274  substantial port
-00025ea0: 696f 6e73 206f 6620 7468 6520 536f 6674  ions of the Soft
-00025eb0: 7761 7265 2e20 2020 2020 2020 2020 2020  ware.           
-00025ec0: 2020 2020 2020 2020 2020 2020 7c0a 7c20              |.| 
-00025ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025ee0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00025ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025ec0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
+00025ed0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
+00025ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025ef0: 2020 2020 2020 2020 2020 2020 2020 436f                Co
+00025f00: 7079 7269 6768 7420 3230 3231 2042 6163  pyright 2021 Bac
+00025f10: 6b62 6c61 7a65 2049 6e63 2e20 2020 2020  kblaze Inc.     
 00025f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00025f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00025f40: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00025f50: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00025f60: 2020 2054 4845 2053 4f46 5457 4152 4520     THE SOFTWARE 
-00025f70: 4953 2050 524f 5649 4445 4420 2241 5320  IS PROVIDED "AS 
-00025f80: 4953 222c 2057 4954 484f 5554 2057 4152  IS", WITHOUT WAR
-00025f90: 5241 4e54 5920 4f46 2041 4e59 204b 494e  RANTY OF ANY KIN
-00025fa0: 442c 2045 5850 5245 5353 204f 5220 2020  D, EXPRESS OR   
-00025fb0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00025fc0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00025fd0: 2020 2020 2049 4d50 4c49 4544 2c20 494e       IMPLIED, IN
-00025fe0: 434c 5544 494e 4720 4255 5420 4e4f 5420  CLUDING BUT NOT 
-00025ff0: 4c49 4d49 5445 4420 544f 2054 4845 2057  LIMITED TO THE W
-00026000: 4152 5241 4e54 4945 5320 4f46 204d 4552  ARRANTIES OF MER
-00026010: 4348 414e 5441 4249 4c49 5459 2c20 4649  CHANTABILITY, FI
-00026020: 544e 4553 5320 2020 2020 207c 0a7c 2020  TNESS      |.|  
-00026030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026040: 2020 7c20 2020 2020 2020 2046 4f52 2041    |        FOR A
-00026050: 2050 4152 5449 4355 4c41 5220 5055 5250   PARTICULAR PURP
-00026060: 4f53 4520 414e 4420 4e4f 4e49 4e46 5249  OSE AND NONINFRI
-00026070: 4e47 454d 454e 542e 2049 4e20 4e4f 2045  NGEMENT. IN NO E
-00026080: 5645 4e54 2053 4841 4c4c 2054 4845 2041  VENT SHALL THE A
-00026090: 5554 484f 5253 204f 5220 2020 2020 2020  UTHORS OR       
-000260a0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-000260b0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-000260c0: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
-000260d0: 5320 4245 204c 4941 424c 4520 464f 5220  S BE LIABLE FOR 
-000260e0: 414e 5920 434c 4149 4d2c 2044 414d 4147  ANY CLAIM, DAMAG
-000260f0: 4553 204f 5220 4f54 4845 5220 4c49 4142  ES OR OTHER LIAB
-00026100: 494c 4954 592c 2057 4845 5448 4552 2020  ILITY, WHETHER  
-00026110: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00026120: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00026130: 2020 2020 2020 2020 494e 2041 4e20 4143          IN AN AC
-00026140: 5449 4f4e 204f 4620 434f 4e54 5241 4354  TION OF CONTRACT
-00026150: 2c20 544f 5254 204f 5220 4f54 4845 5257  , TORT OR OTHERW
-00026160: 4953 452c 2041 5249 5349 4e47 2046 524f  ISE, ARISING FRO
-00026170: 4d2c 204f 5554 204f 4620 4f52 2049 4e20  M, OUT OF OR IN 
-00026180: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00026190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000261a0: 207c 2020 2020 2020 2020 2020 434f 4e4e   |          CONN
-000261b0: 4543 5449 4f4e 2057 4954 4820 5448 4520  ECTION WITH THE 
-000261c0: 534f 4654 5741 5245 204f 5220 5448 4520  SOFTWARE OR THE 
-000261d0: 5553 4520 4f52 204f 5448 4552 2044 4541  USE OR OTHER DEA
-000261e0: 4c49 4e47 5320 494e 2054 4845 2053 4f46  LINGS IN THE SOF
-000261f0: 5457 4152 452e 2020 2020 2020 2020 207c  TWARE.         |
-00026200: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00026210: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00026220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026270: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
-00026280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00026290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000262a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000262b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000262c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000262d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000262e0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020  ---------+.|    
-000262f0: 2020 7572 6c6c 6962 3320 2020 2020 2020    urllib3       
-00026300: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00026310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026320: 2020 2020 2020 2020 2020 4d49 5420 4c69            MIT Li
-00026330: 6365 6e73 6520 2020 2020 2020 2020 2020  cense           
-00026340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026350: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00026360: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00026370: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00026380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000263a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000263b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000263c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000263d0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-000263e0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000263f0: 2020 2043 6f70 7972 6967 6874 2028 6329     Copyright (c)
-00026400: 2032 3030 382d 3230 3230 2041 6e64 7265   2008-2020 Andre
-00026410: 7920 5065 7472 6f76 2061 6e64 2063 6f6e  y Petrov and con
-00026420: 7472 6962 7574 6f72 7320 2873 6565 2043  tributors (see C
-00026430: 4f4e 5452 4942 5554 4f52 532e 7478 7429  ONTRIBUTORS.txt)
-00026440: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00026450: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00026460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000264a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000264b0: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-000264c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000264d0: 2020 2020 7c20 2020 2020 2020 2020 5065      |         Pe
-000264e0: 726d 6973 7369 6f6e 2069 7320 6865 7265  rmission is here
-000264f0: 6279 2067 7261 6e74 6564 2c20 6672 6565  by granted, free
-00026500: 206f 6620 6368 6172 6765 2c20 746f 2061   of charge, to a
-00026510: 6e79 2070 6572 736f 6e20 6f62 7461 696e  ny person obtain
-00026520: 696e 6720 6120 636f 7079 2020 2020 2020  ing a copy      
-00026530: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00026540: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00026550: 2020 6f66 2074 6869 7320 736f 6674 7761    of this softwa
-00026560: 7265 2061 6e64 2061 7373 6f63 6961 7465  re and associate
-00026570: 6420 646f 6375 6d65 6e74 6174 696f 6e20  d documentation 
-00026580: 6669 6c65 7320 2874 6865 2022 536f 6674  files (the "Soft
-00026590: 7761 7265 2229 2c20 746f 2064 6561 6c20  ware"), to deal 
-000265a0: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-000265b0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000265c0: 2020 2020 2020 2020 696e 2074 6865 2053          in the S
-000265d0: 6f66 7477 6172 6520 7769 7468 6f75 7420  oftware without 
-000265e0: 7265 7374 7269 6374 696f 6e2c 2069 6e63  restriction, inc
-000265f0: 6c75 6469 6e67 2077 6974 686f 7574 206c  luding without l
-00026600: 696d 6974 6174 696f 6e20 7468 6520 7269  imitation the ri
-00026610: 6768 7473 2020 2020 2020 2020 7c0a 7c20  ghts        |.| 
-00026620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026630: 2020 207c 2020 2020 2020 2020 2020 746f     |          to
-00026640: 2075 7365 2c20 636f 7079 2c20 6d6f 6469   use, copy, modi
-00026650: 6679 2c20 6d65 7267 652c 2070 7562 6c69  fy, merge, publi
-00026660: 7368 2c20 6469 7374 7269 6275 7465 2c20  sh, distribute, 
-00026670: 7375 626c 6963 656e 7365 2c20 616e 642f  sublicense, and/
-00026680: 6f72 2073 656c 6c20 2020 2020 2020 2020  or sell         
-00026690: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-000266a0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000266b0: 2020 2020 2063 6f70 6965 7320 6f66 2074       copies of t
-000266c0: 6865 2053 6f66 7477 6172 652c 2061 6e64  he Software, and
-000266d0: 2074 6f20 7065 726d 6974 2070 6572 736f   to permit perso
-000266e0: 6e73 2074 6f20 7768 6f6d 2074 6865 2053  ns to whom the S
-000266f0: 6f66 7477 6172 6520 6973 2020 2020 2020  oftware is      
-00026700: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00026710: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00026720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026730: 2066 7572 6e69 7368 6564 2074 6f20 646f   furnished to do
-00026740: 2073 6f2c 2073 7562 6a65 6374 2074 6f20   so, subject to 
-00026750: 7468 6520 666f 6c6c 6f77 696e 6720 636f  the following co
-00026760: 6e64 6974 696f 6e73 3a20 2020 2020 2020  nditions:       
-00026770: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00026780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026790: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-000267a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000267b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000267c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000267d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000267e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000267f0: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00026800: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00026810: 5468 6520 6162 6f76 6520 636f 7079 7269  The above copyri
-00026820: 6768 7420 6e6f 7469 6365 2061 6e64 2074  ght notice and t
-00026830: 6869 7320 7065 726d 6973 7369 6f6e 206e  his permission n
-00026840: 6f74 6963 6520 7368 616c 6c20 6265 2069  otice shall be i
-00026850: 6e63 6c75 6465 6420 696e 2061 6c6c 2020  ncluded in all  
-00026860: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00026870: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00026880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026890: 2020 2020 636f 7069 6573 206f 7220 7375      copies or su
-000268a0: 6273 7461 6e74 6961 6c20 706f 7274 696f  bstantial portio
-000268b0: 6e73 206f 6620 7468 6520 536f 6674 7761  ns of the Softwa
-000268c0: 7265 2e20 2020 2020 2020 2020 2020 2020  re.             
-000268d0: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-000268e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000268f0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00026900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026940: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00026950: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00026960: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00026970: 2054 4845 2053 4f46 5457 4152 4520 4953   THE SOFTWARE IS
-00026980: 2050 524f 5649 4445 4420 2241 5320 4953   PROVIDED "AS IS
-00026990: 222c 2057 4954 484f 5554 2057 4152 5241  ", WITHOUT WARRA
-000269a0: 4e54 5920 4f46 2041 4e59 204b 494e 442c  NTY OF ANY KIND,
-000269b0: 2045 5850 5245 5353 204f 5220 2020 2020   EXPRESS OR     
-000269c0: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-000269d0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000269e0: 2020 2020 2020 2049 4d50 4c49 4544 2c20         IMPLIED, 
-000269f0: 494e 434c 5544 494e 4720 4255 5420 4e4f  INCLUDING BUT NO
-00026a00: 5420 4c49 4d49 5445 4420 544f 2054 4845  T LIMITED TO THE
-00026a10: 2057 4152 5241 4e54 4945 5320 4f46 204d   WARRANTIES OF M
-00026a20: 4552 4348 414e 5441 4249 4c49 5459 2c20  ERCHANTABILITY, 
-00026a30: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00026a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026a50: 7c20 2020 2020 2020 2020 4649 544e 4553  |         FITNES
-00026a60: 5320 464f 5220 4120 5041 5254 4943 554c  S FOR A PARTICUL
-00026a70: 4152 2050 5552 504f 5345 2041 4e44 204e  AR PURPOSE AND N
-00026a80: 4f4e 494e 4652 494e 4745 4d45 4e54 2e20  ONINFRINGEMENT. 
-00026a90: 494e 204e 4f20 4556 454e 5420 5348 414c  IN NO EVENT SHAL
-00026aa0: 4c20 5448 4520 2020 2020 2020 2020 7c0a  L THE         |.
-00026ab0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00026ac0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00026ad0: 2020 4155 5448 4f52 5320 4f52 2043 4f50    AUTHORS OR COP
-00026ae0: 5952 4947 4854 2048 4f4c 4445 5253 2042  YRIGHT HOLDERS B
-00026af0: 4520 4c49 4142 4c45 2046 4f52 2041 4e59  E LIABLE FOR ANY
-00026b00: 2043 4c41 494d 2c20 4441 4d41 4745 5320   CLAIM, DAMAGES 
-00026b10: 4f52 204f 5448 4552 2020 2020 2020 2020  OR OTHER        
-00026b20: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00026b30: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00026b40: 2020 204c 4941 4249 4c49 5459 2c20 5748     LIABILITY, WH
-00026b50: 4554 4845 5220 494e 2041 4e20 4143 5449  ETHER IN AN ACTI
-00026b60: 4f4e 204f 4620 434f 4e54 5241 4354 2c20  ON OF CONTRACT, 
-00026b70: 544f 5254 204f 5220 4f54 4845 5257 4953  TORT OR OTHERWIS
-00026b80: 452c 2041 5249 5349 4e47 2046 524f 4d2c  E, ARISING FROM,
-00026b90: 2020 2020 2020 2020 7c0a 7c20 2020 2020          |.|     
-00026ba0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00026bb0: 2020 2020 2020 2020 4f55 5420 4f46 204f          OUT OF O
-00026bc0: 5220 494e 2043 4f4e 4e45 4354 494f 4e20  R IN CONNECTION 
-00026bd0: 5749 5448 2054 4845 2053 4f46 5457 4152  WITH THE SOFTWAR
-00026be0: 4520 4f52 2054 4845 2055 5345 204f 5220  E OR THE USE OR 
-00026bf0: 4f54 4845 5220 4445 414c 494e 4753 2049  OTHER DEALINGS I
-00026c00: 4e20 5448 4520 2020 2020 2020 207c 0a7c  N THE        |.|
-00026c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c20: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00026c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c40: 2020 2020 2020 2020 2020 2020 2020 2053                 S
-00026c50: 4f46 5457 4152 452e 2020 2020 2020 2020  OFTWARE.        
-00026c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026c80: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00026c90: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00026ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026cf0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
-00026d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-00026d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00026d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00026d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00026d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00026d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00026d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20  ------------+.| 
-00026d70: 2020 2020 2077 6377 6964 7468 2020 2020       wcwidth    
-00026d80: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00026d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026da0: 2020 2020 2020 2020 5468 6520 4d49 5420          The MIT 
-00026db0: 4c69 6365 6e73 6520 284d 4954 2920 2020  License (MIT)   
-00026dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026de0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00026df0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00026e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026e50: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00026e60: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00026e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026e80: 2020 436f 7079 7269 6768 7420 2863 2920    Copyright (c) 
-00026e90: 3230 3134 204a 6566 6620 5175 6173 7420  2014 Jeff Quast 
-00026ea0: 3c63 6f6e 7461 6374 406a 6566 6671 7561  <contact@jeffqua
-00026eb0: 7374 2e63 6f6d 3e20 2020 2020 2020 2020  st.com>         
-00026ec0: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00026ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026ee0: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00026ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00026f40: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-00026f50: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00026f60: 2050 6572 6d69 7373 696f 6e20 6973 2068   Permission is h
-00026f70: 6572 6562 7920 6772 616e 7465 642c 2066  ereby granted, f
-00026f80: 7265 6520 6f66 2063 6861 7267 652c 2074  ree of charge, t
-00026f90: 6f20 616e 7920 7065 7273 6f6e 206f 6274  o any person obt
-00026fa0: 6169 6e69 6e67 2061 2063 6f70 7920 2020  aining a copy   
-00026fb0: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00026fc0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00026fd0: 2020 2020 206f 6620 7468 6973 2073 6f66       of this sof
-00026fe0: 7477 6172 6520 616e 6420 6173 736f 6369  tware and associ
-00026ff0: 6174 6564 2064 6f63 756d 656e 7461 7469  ated documentati
-00027000: 6f6e 2066 696c 6573 2028 7468 6520 2253  on files (the "S
-00027010: 6f66 7477 6172 6522 292c 2074 6f20 6465  oftware"), to de
-00027020: 616c 2020 2020 2020 2020 7c0a 7c20 2020  al        |.|   
-00027030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027040: 207c 2020 2020 2020 2020 2069 6e20 7468   |         in th
-00027050: 6520 536f 6674 7761 7265 2077 6974 686f  e Software witho
-00027060: 7574 2072 6573 7472 6963 7469 6f6e 2c20  ut restriction, 
-00027070: 696e 636c 7564 696e 6720 7769 7468 6f75  including withou
-00027080: 7420 6c69 6d69 7461 7469 6f6e 2074 6865  t limitation the
-00027090: 2072 6967 6874 7320 2020 2020 2020 207c   rights        |
-000270a0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-000270b0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-000270c0: 2074 6f20 7573 652c 2063 6f70 792c 206d   to use, copy, m
-000270d0: 6f64 6966 792c 206d 6572 6765 2c20 7075  odify, merge, pu
-000270e0: 626c 6973 682c 2064 6973 7472 6962 7574  blish, distribut
-000270f0: 652c 2073 7562 6c69 6365 6e73 652c 2061  e, sublicense, a
-00027100: 6e64 2f6f 7220 7365 6c6c 2020 2020 2020  nd/or sell      
-00027110: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00027120: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00027130: 2020 2020 2020 2020 636f 7069 6573 206f          copies o
-00027140: 6620 7468 6520 536f 6674 7761 7265 2c20  f the Software, 
-00027150: 616e 6420 746f 2070 6572 6d69 7420 7065  and to permit pe
-00027160: 7273 6f6e 7320 746f 2077 686f 6d20 7468  rsons to whom th
-00027170: 6520 536f 6674 7761 7265 2069 7320 2020  e Software is   
-00027180: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00027190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000271a0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000271b0: 2020 2020 6675 726e 6973 6865 6420 746f      furnished to
-000271c0: 2064 6f20 736f 2c20 7375 626a 6563 7420   do so, subject 
-000271d0: 746f 2074 6865 2066 6f6c 6c6f 7769 6e67  to the following
-000271e0: 2063 6f6e 6469 7469 6f6e 733a 2020 2020   conditions:    
-000271f0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00027200: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00027210: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00027220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027270: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-00027280: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00027290: 2020 2054 6865 2061 626f 7665 2063 6f70     The above cop
-000272a0: 7972 6967 6874 206e 6f74 6963 6520 616e  yright notice an
-000272b0: 6420 7468 6973 2070 6572 6d69 7373 696f  d this permissio
-000272c0: 6e20 6e6f 7469 6365 2073 6861 6c6c 2062  n notice shall b
-000272d0: 6520 696e 636c 7564 6564 2069 6e20 616c  e included in al
-000272e0: 6c20 2020 2020 2020 7c0a 7c20 2020 2020  l       |.|     
-000272f0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00027300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027310: 2020 2020 2020 2063 6f70 6965 7320 6f72         copies or
-00027320: 2073 7562 7374 616e 7469 616c 2070 6f72   substantial por
-00027330: 7469 6f6e 7320 6f66 2074 6865 2053 6f66  tions of the Sof
-00027340: 7477 6172 652e 2020 2020 2020 2020 2020  tware.          
-00027350: 2020 2020 2020 2020 2020 2020 207c 0a7c               |.|
-00027360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027370: 2020 2020 7c20 2020 2020 2020 2020 2020      |           
-00027380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000273a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000273b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000273c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000273d0: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-000273e0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-000273f0: 2020 2020 5448 4520 534f 4654 5741 5245      THE SOFTWARE
-00027400: 2049 5320 5052 4f56 4944 4544 2022 4153   IS PROVIDED "AS
-00027410: 2049 5322 2c20 5749 5448 4f55 5420 5741   IS", WITHOUT WA
-00027420: 5252 414e 5459 204f 4620 414e 5920 4b49  RRANTY OF ANY KI
-00027430: 4e44 2c20 4558 5052 4553 5320 4f52 2020  ND, EXPRESS OR  
-00027440: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-00027450: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00027460: 2020 2020 2020 2020 2020 494d 504c 4945            IMPLIE
-00027470: 442c 2049 4e43 4c55 4449 4e47 2042 5554  D, INCLUDING BUT
-00027480: 204e 4f54 204c 494d 4954 4544 2054 4f20   NOT LIMITED TO 
-00027490: 5448 4520 5741 5252 414e 5449 4553 204f  THE WARRANTIES O
-000274a0: 4620 4d45 5243 4841 4e54 4142 494c 4954  F MERCHANTABILIT
-000274b0: 592c 2020 2020 2020 2020 2020 7c0a 7c20  Y,          |.| 
-000274c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000274d0: 2020 207c 2020 2020 2020 2020 2046 4954     |         FIT
-000274e0: 4e45 5353 2046 4f52 2041 2050 4152 5449  NESS FOR A PARTI
-000274f0: 4355 4c41 5220 5055 5250 4f53 4520 414e  CULAR PURPOSE AN
-00027500: 4420 4e4f 4e49 4e46 5249 4e47 454d 454e  D NONINFRINGEMEN
-00027510: 542e 2049 4e20 4e4f 2045 5645 4e54 2053  T. IN NO EVENT S
-00027520: 4841 4c4c 2054 4845 2020 2020 2020 2020  HALL THE        
-00027530: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-00027540: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00027550: 2020 2020 2041 5554 484f 5253 204f 5220       AUTHORS OR 
-00027560: 434f 5059 5249 4748 5420 484f 4c44 4552  COPYRIGHT HOLDER
-00027570: 5320 4245 204c 4941 424c 4520 464f 5220  S BE LIABLE FOR 
-00027580: 414e 5920 434c 4149 4d2c 2044 414d 4147  ANY CLAIM, DAMAG
-00027590: 4553 204f 5220 4f54 4845 5220 2020 2020  ES OR OTHER     
-000275a0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-000275b0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-000275c0: 2020 2020 2020 4c49 4142 494c 4954 592c        LIABILITY,
-000275d0: 2057 4845 5448 4552 2049 4e20 414e 2041   WHETHER IN AN A
-000275e0: 4354 494f 4e20 4f46 2043 4f4e 5452 4143  CTION OF CONTRAC
-000275f0: 542c 2054 4f52 5420 4f52 204f 5448 4552  T, TORT OR OTHER
-00027600: 5749 5345 2c20 4152 4953 494e 4720 4652  WISE, ARISING FR
-00027610: 4f4d 2c20 2020 2020 2020 207c 0a7c 2020  OM,        |.|  
-00027620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027630: 2020 7c20 2020 2020 2020 204f 5554 204f    |        OUT O
-00027640: 4620 4f52 2049 4e20 434f 4e4e 4543 5449  F OR IN CONNECTI
-00027650: 4f4e 2057 4954 4820 5448 4520 534f 4654  ON WITH THE SOFT
-00027660: 5741 5245 204f 5220 5448 4520 5553 4520  WARE OR THE USE 
-00027670: 4f52 204f 5448 4552 2044 4541 4c49 4e47  OR OTHER DEALING
-00027680: 5320 494e 2054 4845 2020 2020 2020 2020  S IN THE        
-00027690: 7c0a 7c20 2020 2020 2020 2020 2020 2020  |.|             
-000276a0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-000276b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000276c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000276d0: 2020 534f 4654 5741 5245 2e20 2020 2020    SOFTWARE.     
-000276e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000276f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027700: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00027710: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00027720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027770: 2020 2020 2020 2020 2020 7c0a 7c20 2020            |.|   
-00027780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027790: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-000277a0: 2020 2020 2020 2020 2020 2020 204d 6172               Mar
-000277b0: 6b75 7320 4b75 686e 202d 2d20 3230 3037  kus Kuhn -- 2007
-000277c0: 2d30 352d 3236 2028 556e 6963 6f64 6520  -05-26 (Unicode 
-000277d0: 352e 3029 2020 2020 2020 2020 2020 2020  5.0)            
-000277e0: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-000277f0: 0a7c 2020 2020 2020 2020 2020 2020 2020  .|              
-00027800: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00027810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027850: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027860: 2020 2020 7c0a 7c20 2020 2020 2020 2020      |.|         
-00027870: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-00027880: 2020 2020 2020 2020 2020 2020 5065 726d              Perm
-00027890: 6973 7369 6f6e 2074 6f20 7573 652c 2063  ission to use, c
-000278a0: 6f70 792c 206d 6f64 6966 792c 2061 6e64  opy, modify, and
-000278b0: 2064 6973 7472 6962 7574 6520 7468 6973   distribute this
-000278c0: 2073 6f66 7477 6172 6520 2020 2020 2020   software       
-000278d0: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-000278e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000278f0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00027900: 2066 6f72 2061 6e79 2070 7572 706f 7365   for any purpose
-00027910: 2061 6e64 2077 6974 686f 7574 2066 6565   and without fee
-00027920: 2069 7320 6865 7265 6279 2067 7261 6e74   is hereby grant
-00027930: 6564 2e20 5468 6520 6175 7468 6f72 2020  ed. The author  
-00027940: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00027950: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00027960: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00027970: 2020 2020 2020 2020 2020 6469 7363 6c61            discla
-00027980: 696d 7320 616c 6c20 7761 7272 616e 7469  ims all warranti
-00027990: 6573 2077 6974 6820 7265 6761 7264 2074  es with regard t
-000279a0: 6f20 7468 6973 2073 6f66 7477 6172 652e  o this software.
-000279b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000279c0: 2020 207c 0a7c 2020 2020 2020 2020 2020     |.|          
-000279d0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-000279e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000279f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027a30: 2020 2020 2020 2020 7c0a 2b2d 2d2d 2d2d          |.+-----
-00027a40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00027a50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027a70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a0a  -------------+..
-00027ab0: 5375 6d6d 6172 7920 6f66 2061 6c6c 206d  Summary of all m
-00027ac0: 6f64 756c 6573 2075 7365 6420 6279 2062  odules used by b
-00027ad0: 322c 2073 6869 7070 6564 2077 6974 6820  2, shipped with 
-00027ae0: 6974 2069 6e20 6269 6e61 7279 2066 6f72  it in binary for
-00027af0: 6d3a 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  m:.+------------
-00027b00: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00027b10: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00027b20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027b30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00027b40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027b50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027b60: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-00027b70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027b80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027b90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20  ------------+.| 
-00027ba0: 2020 204d 6f64 756c 6520 6e61 6d65 2020     Module name  
-00027bb0: 2020 207c 2020 5665 7273 696f 6e20 207c     |  Version  |
-00027bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027bd0: 4c69 6365 6e73 6520 2020 2020 2020 2020  License         
-00027be0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00027bf0: 2020 2020 2020 2020 4175 7468 6f72 2020          Author  
-00027c00: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-00027c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027c20: 2020 2020 2020 2020 2055 524c 2020 2020           URL    
-00027c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00027c40: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
-00027c50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-00027c60: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00027c70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027c80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027c90: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00027ca0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027cb0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00027cc0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027cd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027ce0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027cf0: 2d2d 2b0a 7c20 2020 2061 7267 636f 6d70  --+.|    argcomp
-00027d00: 6c65 7465 2020 2020 207c 2020 2033 2e30  lete     |   3.0
-00027d10: 2e38 2020 207c 2020 2020 2020 2020 4170  .8   |        Ap
-00027d20: 6163 6865 2053 6f66 7477 6172 6520 4c69  ache Software Li
-00027d30: 6365 6e73 6520 2020 2020 2020 207c 2020  cense        |  
-00027d40: 2020 2020 2020 2020 2020 416e 6472 6579            Andrey
-00027d50: 204b 6973 6c79 756b 2020 2020 2020 2020   Kislyuk        
-00027d60: 2020 2020 7c20 2020 2020 2020 2020 6874      |         ht
-00027d70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00027d80: 2f6b 6973 6c79 756b 2f61 7267 636f 6d70  /kislyuk/argcomp
-00027d90: 6c65 7465 2020 2020 2020 2020 207c 0a2b  lete         |.+
-00027da0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027db0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00027dc0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00027dd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027de0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00027df0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027e00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00027e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027e40: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020  --------+.|     
-00027e50: 2020 6172 726f 7720 2020 2020 2020 207c    arrow        |
-00027e60: 2020 2031 2e32 2e33 2020 207c 2020 2020     1.2.3   |    
-00027e70: 2020 2020 4170 6163 6865 2053 6f66 7477      Apache Softw
-00027e80: 6172 6520 4c69 6365 6e73 6520 2020 2020  are License     
-00027e90: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00027ea0: 2043 6872 6973 2053 6d69 7468 2020 2020   Chris Smith    
-00027eb0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00027ec0: 2020 2020 2020 2020 2068 7474 7073 3a2f           https:/
-00027ed0: 2f61 7272 6f77 2e72 6561 6474 6865 646f  /arrow.readthedo
-00027ee0: 6373 2e69 6f20 2020 2020 2020 2020 2020  cs.io           
-00027ef0: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-00027f00: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00027f10: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00027f20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027f30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-00027f40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027f50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027f60: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00027f70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027f80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00027f90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
-00027fa0: 7c20 2020 2020 2020 6232 7364 6b20 2020  |       b2sdk   
-00027fb0: 2020 2020 207c 2020 2031 2e32 312e 3020       |   1.21.0 
-00027fc0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00027fd0: 4d49 5420 4c69 6365 6e73 6520 2020 2020  MIT License     
-00027fe0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00027ff0: 2020 2020 2042 6163 6b62 6c61 7a65 2c20       Backblaze, 
-00028000: 496e 632e 2020 2020 2020 2020 2020 2020  Inc.            
-00028010: 7c20 2020 2020 2020 6874 7470 733a 2f2f  |       https://
-00028020: 6769 7468 7562 2e63 6f6d 2f42 6163 6b62  github.com/Backb
-00028030: 6c61 7a65 2f62 322d 7364 6b2d 7079 7468  laze/b2-sdk-pyth
-00028040: 6f6e 2020 2020 2020 207c 0a2b 2d2d 2d2d  on       |.+----
-00028050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028060: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  +-----------+---
-00028070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028090: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-000280a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000280b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-000280c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000280d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000280e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000280f0: 2d2d 2d2d 2b0a 7c20 2020 2020 2063 6572  ----+.|      cer
-00028100: 7469 6669 2020 2020 2020 207c 2032 3032  tifi       | 202
-00028110: 322e 3132 2e37 207c 2020 4d6f 7a69 6c6c  2.12.7 |  Mozill
-00028120: 6120 5075 626c 6963 204c 6963 656e 7365  a Public License
-00028130: 2032 2e30 2028 4d50 4c20 322e 3029 207c   2.0 (MPL 2.0) |
-00028140: 2020 2020 2020 2020 2020 2020 4b65 6e6e              Kenn
-00028150: 6574 6820 5265 6974 7a20 2020 2020 2020  eth Reitz       
-00028160: 2020 2020 2020 7c20 2020 2020 2020 6874        |       ht
-00028170: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00028180: 2f63 6572 7469 6669 2f70 7974 686f 6e2d  /certifi/python-
-00028190: 6365 7274 6966 6920 2020 2020 2020 207c  certifi        |
-000281a0: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
-000281b0: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-000281c0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-000281d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000281e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-000281f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028210: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00028220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028240: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 6368  ----------+.| ch
-00028250: 6172 7365 742d 6e6f 726d 616c 697a 6572  arset-normalizer
-00028260: 207c 2020 2033 2e31 2e30 2020 207c 2020   |   3.1.0   |  
-00028270: 2020 2020 2020 2020 2020 2020 4d49 5420              MIT 
-00028280: 4c69 6365 6e73 6520 2020 2020 2020 2020  License         
-00028290: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-000282a0: 2020 2041 686d 6564 2054 4148 5249 2020     Ahmed TAHRI  
-000282b0: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-000282c0: 2020 2068 7474 7073 3a2f 2f67 6974 6875     https://githu
-000282d0: 622e 636f 6d2f 4f75 7372 6574 2f63 6861  b.com/Ousret/cha
-000282e0: 7273 6574 5f6e 6f72 6d61 6c69 7a65 7220  rset_normalizer 
-000282f0: 2020 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d       |.+--------
-00028300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00028310: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00028320: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028340: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00028350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028360: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00028370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000283a0: 2b0a 7c20 2020 2020 2064 6f63 7574 696c  +.|      docutil
-000283b0: 7320 2020 2020 207c 2020 2020 302e 3139  s      |    0.19
-000283c0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-000283d0: 2020 4253 4420 4c69 6365 6e73 6520 2020    BSD License   
-000283e0: 2020 2020 2020 2020 2020 207c 2020 2020             |    
-000283f0: 2020 2020 2020 2020 4461 7669 6420 476f          David Go
-00028400: 6f64 6765 7220 2020 2020 2020 2020 2020  odger           
-00028410: 2020 7c20 2020 2020 2020 2020 2020 2068    |            h
-00028420: 7474 7073 3a2f 2f64 6f63 7574 696c 732e  ttps://docutils.
-00028430: 736f 7572 6365 666f 7267 652e 696f 2f20  sourceforge.io/ 
-00028440: 2020 2020 2020 2020 2020 207c 0a7c 2020             |.|  
-00028450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028460: 2020 7c20 2020 2020 2020 2020 2020 7c20    |           | 
-00028470: 2020 2047 4e55 2047 656e 6572 616c 2050     GNU General P
-00028480: 7562 6c69 6320 4c69 6365 6e73 6520 2847  ublic License (G
-00028490: 504c 2920 2020 7c20 2020 2020 2020 2020  PL)   |         
-000284a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000284b0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-000284c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000284d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000284e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000284f0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00028500: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00028510: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00028520: 2020 2020 2020 2020 5075 626c 6963 2044          Public D
-00028530: 6f6d 6169 6e20 2020 2020 2020 2020 2020  omain           
-00028540: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00028550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028560: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00028570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000285a0: 207c 0a7c 2020 2020 2020 2020 2020 2020   |.|            
-000285b0: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000285c0: 2020 2020 7c20 2020 5079 7468 6f6e 2053      |   Python S
-000285d0: 6f66 7477 6172 6520 466f 756e 6461 7469  oftware Foundati
-000285e0: 6f6e 204c 6963 656e 7365 2020 7c20 2020  on License  |   
-000285f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028610: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-00028620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00028640: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
-00028650: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028660: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---+-----------+
-00028670: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028680: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028690: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-000286a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000286b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-000286c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000286d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000286e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000286f0: 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020 2020  -------+.|      
-00028700: 2020 6964 6e61 2020 2020 2020 2020 7c20    idna        | 
-00028710: 2020 2033 2e34 2020 2020 7c20 2020 2020     3.4    |     
-00028720: 2020 2020 2020 2020 2042 5344 204c 6963           BSD Lic
-00028730: 656e 7365 2020 2020 2020 2020 2020 2020  ense            
-00028740: 2020 7c20 2020 4b69 6d20 4461 7669 6573    |   Kim Davies
-00028750: 203c 6b69 6d40 6379 6e6f 7375 7265 2e63   <kim@cynosure.c
-00028760: 6f6d 2e61 753e 2020 207c 2020 2020 2020  om.au>   |      
-00028770: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00028780: 6769 7468 7562 2e63 6f6d 2f6b 6a64 2f69  github.com/kjd/i
-00028790: 646e 6120 2020 2020 2020 2020 2020 2020  dna             
-000287a0: 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d    |.+-----------
-000287b0: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-000287c0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-000287d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000287e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-000287f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028800: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028810: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00028820: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028830: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028840: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
-00028850: 2020 2020 2020 6c6f 6766 7572 7920 2020        logfury   
-00028860: 2020 2020 7c20 2020 312e 302e 3120 2020      |   1.0.1   
-00028870: 7c20 2020 2020 2020 2020 2020 2020 2042  |              B
-00028880: 5344 204c 6963 656e 7365 2020 2020 2020  SD License      
-00028890: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-000288a0: 2020 2020 2050 6177 656c 2050 6f6c 6577       Pawel Polew
-000288b0: 6963 7a20 2020 2020 2020 2020 2020 207c  icz            |
-000288c0: 2020 2020 2020 6874 7470 733a 2f2f 6769        https://gi
-000288d0: 7468 7562 2e63 6f6d 2f72 6565 662d 7465  thub.com/reef-te
-000288e0: 6368 6e6f 6c6f 6769 6573 2f6c 6f67 6675  chnologies/logfu
-000288f0: 7279 2020 2020 2020 7c0a 2b2d 2d2d 2d2d  ry      |.+-----
-00028900: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00028910: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00028920: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028940: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-00028950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028960: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00028970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000289a0: 2d2d 2d2b 0a7c 2070 6878 2d63 6c61 7373  ---+.| phx-class
-000289b0: 2d72 6567 6973 7472 7920 7c20 2020 342e  -registry |   4.
-000289c0: 302e 3620 2020 7c20 2020 2020 2020 2020  0.6   |         
-000289d0: 2020 2020 204d 4954 204c 6963 656e 7365       MIT License
-000289e0: 2020 2020 2020 2020 2020 2020 2020 7c20                | 
-000289f0: 2020 2020 2050 686f 656e 6978 205a 6572       Phoenix Zer
-00028a00: 696e 203c 7068 7840 7068 782e 6e7a 3e20  in <phx@phx.nz> 
-00028a10: 2020 2020 207c 2068 7474 7073 3a2f 2f67       | https://g
-00028a20: 6974 6875 622e 636f 6d2f 746f 646f 6669  ithub.com/todofi
-00028a30: 7874 6869 732f 636c 6173 732d 7265 6769  xthis/class-regi
-00028a40: 7374 7279 2f72 656c 6561 7365 7320 7c0a  stry/releases |.
-00028a50: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00028a60: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00028a70: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00028a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028a90: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00028aa0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028ac0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00028ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028af0: 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020 2020  ---------+.|    
-00028b00: 2020 2020 7069 7020 2020 2020 2020 2020      pip         
-00028b10: 7c20 2020 3232 2e33 2e31 2020 7c20 2020  |   22.3.1  |   
-00028b20: 2020 2020 2020 2020 2020 204d 4954 204c             MIT L
-00028b30: 6963 656e 7365 2020 2020 2020 2020 2020  icense          
-00028b40: 2020 2020 7c20 2020 2020 2020 2020 2054      |          T
-00028b50: 6865 2070 6970 2064 6576 656c 6f70 6572  he pip developer
-00028b60: 7320 2020 2020 2020 2020 207c 2020 2020  s          |    
-00028b70: 2020 2020 2020 2020 2020 2020 2020 6874                ht
-00028b80: 7470 733a 2f2f 7069 702e 7079 7061 2e69  tps://pip.pypa.i
-00028b90: 6f2f 2020 2020 2020 2020 2020 2020 2020  o/              
-00028ba0: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
-00028bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00028bc0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00028bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00028bf0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028c10: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00028c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00028c50: 0a7c 2020 2020 7069 702d 6c69 6365 6e73  .|    pip-licens
-00028c60: 6573 2020 2020 7c20 2020 342e 332e 3020  es    |   4.3.0 
-00028c70: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00028c80: 204d 4954 204c 6963 656e 7365 2020 2020   MIT License    
-00028c90: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
-00028ca0: 2020 2020 2020 2020 2020 2072 6169 6d6f             raimo
-00028cb0: 6e20 2020 2020 2020 2020 2020 2020 2020  n               
-00028cc0: 207c 2020 2020 2020 2020 6874 7470 733a   |        https:
-00028cd0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6169  //github.com/rai
-00028ce0: 6d6f 6e34 392f 7069 702d 6c69 6365 6e73  mon49/pip-licens
-00028cf0: 6573 2020 2020 2020 2020 7c0a 2b2d 2d2d  es        |.+---
-00028d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028d10: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -+-----------+--
-00028d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028d40: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-00028d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-00028d70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028d80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028d90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028da0: 2d2d 2d2d 2d2b 0a7c 2020 2020 7072 6574  -----+.|    pret
-00028db0: 7479 7461 626c 6520 2020 2020 7c20 2020  tytable     |   
-00028dc0: 332e 372e 3020 2020 7c20 2020 2020 2020  3.7.0   |       
-00028dd0: 2020 2020 2020 2042 5344 204c 6963 656e         BSD Licen
-00028de0: 7365 2020 2020 2020 2020 2020 2020 2020  se              
-00028df0: 7c20 204c 756b 6520 4d61 7572 6974 7320  |  Luke Maurits 
-00028e00: 3c6c 756b 6540 6d61 7572 6974 732e 6964  <luke@maurits.id
-00028e10: 2e61 753e 2020 207c 2020 2020 2020 2020  .au>   |        
-00028e20: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00028e30: 6f6d 2f6a 617a 7a62 616e 642f 7072 6574  om/jazzband/pret
-00028e40: 7479 7461 626c 6520 2020 2020 2020 2020  tytable         
-00028e50: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
-00028e60: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00028e70: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-00028e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00028ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028ec0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00028ed0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028ee0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00028ef0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020  -----------+.|  
-00028f00: 7079 7468 6f6e 2d64 6174 6575 7469 6c20  python-dateutil 
-00028f10: 2020 7c20 2020 322e 382e 3220 2020 7c20    |   2.8.2   | 
-00028f20: 2020 2020 2020 2041 7061 6368 6520 536f         Apache So
-00028f30: 6674 7761 7265 204c 6963 656e 7365 2020  ftware License  
-00028f40: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00028f50: 2020 4775 7374 6176 6f20 4e69 656d 6579    Gustavo Niemey
-00028f60: 6572 2020 2020 2020 2020 2020 207c 2020  er           |  
-00028f70: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
-00028f80: 6769 7468 7562 2e63 6f6d 2f64 6174 6575  github.com/dateu
-00028f90: 7469 6c2f 6461 7465 7574 696c 2020 2020  til/dateutil    
-00028fa0: 2020 2020 2020 7c0a 7c20 2020 2020 2020        |.|       
-00028fb0: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00028fc0: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00028fd0: 2020 2020 2020 2020 2042 5344 204c 6963           BSD Lic
-00028fe0: 656e 7365 2020 2020 2020 2020 2020 2020  ense            
-00028ff0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00029000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029010: 2020 2020 2020 2020 7c20 2020 2020 2020          |       
-00029020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029050: 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d   |.+------------
-00029060: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00029070: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00029080: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029090: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  ------------+---
-000290a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000290b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000290c0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-000290d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000290e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000290f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20  ------------+.| 
-00029100: 2020 2020 2072 6571 7565 7374 7320 2020       requests   
-00029110: 2020 207c 2020 2032 2e32 392e 3020 207c     |   2.29.0  |
-00029120: 2020 2020 2020 2020 4170 6163 6865 2053          Apache S
-00029130: 6f66 7477 6172 6520 4c69 6365 6e73 6520  oftware License 
-00029140: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00029150: 2020 2020 4b65 6e6e 6574 6820 5265 6974      Kenneth Reit
-00029160: 7a20 2020 2020 2020 2020 2020 2020 7c20  z             | 
-00029170: 2020 2020 2020 2020 2020 2068 7474 7073             https
-00029180: 3a2f 2f72 6571 7565 7374 732e 7265 6164  ://requests.read
-00029190: 7468 6564 6f63 732e 696f 2020 2020 2020  thedocs.io      
-000291a0: 2020 2020 2020 207c 0a2b 2d2d 2d2d 2d2d         |.+------
-000291b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-000291c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-000291d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000291e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000291f0: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00029200: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029210: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00029220: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029230: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029250: 2d2d 2b0a 7c20 2020 2020 2072 7374 3261  --+.|      rst2a
-00029260: 6e73 6920 2020 2020 207c 2020 2030 2e31  nsi      |   0.1
-00029270: 2e35 2020 207c 2020 2020 2020 2020 2020  .5   |          
-00029280: 2020 2020 4d49 5420 4c69 6365 6e73 6520      MIT License 
-00029290: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-000292a0: 2020 2020 2020 2020 2020 2020 2020 536e                Sn
-000292b0: 6169 7065 2020 2020 2020 2020 2020 2020  aipe            
-000292c0: 2020 2020 7c20 2020 2020 2068 7474 7073      |      https
-000292d0: 3a2f 2f67 6974 6875 622e 636f 6d2f 536e  ://github.com/Sn
-000292e0: 6169 7065 2f70 7974 686f 6e2d 7273 742d  aipe/python-rst-
-000292f0: 746f 2d61 6e73 6920 2020 2020 207c 0a2b  to-ansi      |.+
-00029300: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029310: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00029320: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  +---------------
-00029330: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029340: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00029350: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029360: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---------------+
-00029370: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029380: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029390: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000293a0: 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020 2020  --------+.|     
-000293b0: 7365 7475 7074 6f6f 6c73 2020 2020 207c  setuptools     |
-000293c0: 2020 2036 352e 352e 3020 207c 2020 2020     65.5.0  |    
-000293d0: 2020 2020 2020 2020 2020 4d49 5420 4c69            MIT Li
-000293e0: 6365 6e73 6520 2020 2020 2020 2020 2020  cense           
-000293f0: 2020 207c 2020 2020 2020 5079 7468 6f6e     |      Python
-00029400: 2050 6163 6b61 6769 6e67 2041 7574 686f   Packaging Autho
-00029410: 7269 7479 2020 2020 2020 7c20 2020 2020  rity      |     
-00029420: 2020 2020 2020 6874 7470 733a 2f2f 6769        https://gi
-00029430: 7468 7562 2e63 6f6d 2f70 7970 612f 7365  thub.com/pypa/se
-00029440: 7475 7074 6f6f 6c73 2020 2020 2020 2020  tuptools        
-00029450: 2020 207c 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d     |.+----------
-00029460: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00029470: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00029480: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-000294a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000294b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000294c0: 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d  -----+----------
-000294d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000294e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000294f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a  --------------+.
-00029500: 7c20 2020 2020 2020 2073 6978 2020 2020  |        six    
-00029510: 2020 2020 207c 2020 2031 2e31 362e 3020       |   1.16.0 
-00029520: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00029530: 4d49 5420 4c69 6365 6e73 6520 2020 2020  MIT License     
-00029540: 2020 2020 2020 2020 207c 2020 2020 2020           |      
-00029550: 2020 2020 4265 6e6a 616d 696e 2050 6574      Benjamin Pet
-00029560: 6572 736f 6e20 2020 2020 2020 2020 2020  erson           
-00029570: 7c20 2020 2020 2020 2020 2020 2068 7474  |            htt
-00029580: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00029590: 6265 6e6a 616d 696e 702f 7369 7820 2020  benjaminp/six   
-000295a0: 2020 2020 2020 2020 207c 0a2b 2d2d 2d2d           |.+----
-000295b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000295c0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  +-----------+---
-000295d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000295e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000295f0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00029600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00029620: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029630: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029640: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029650: 2d2d 2d2d 2b0a 7c20 2020 2020 2074 6162  ----+.|      tab
-00029660: 756c 6174 6520 2020 2020 207c 2020 2030  ulate      |   0
-00029670: 2e39 2e30 2020 207c 2020 2020 2020 2020  .9.0   |        
-00029680: 2020 2020 2020 4d49 5420 4c69 6365 6e73        MIT Licens
-00029690: 6520 2020 2020 2020 2020 2020 2020 207c  e              |
-000296a0: 2053 6572 6765 7920 4173 7461 6e69 6e20   Sergey Astanin 
-000296b0: 3c73 2e61 7374 616e 696e 4067 6d61 696c  <s.astanin@gmail
-000296c0: 2e63 6f6d 3e20 7c20 2020 2020 2020 6874  .com> |       ht
-000296d0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-000296e0: 2f61 7374 616e 696e 2f70 7974 686f 6e2d  /astanin/python-
-000296f0: 7461 6275 6c61 7465 2020 2020 2020 207c  tabulate       |
-00029700: 0a2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  .+--------------
-00029710: 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d  ------+---------
-00029720: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00029730: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029740: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-00029750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029760: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029770: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00029780: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029790: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000297a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2b0a 7c20 2020  ----------+.|   
-000297b0: 2020 2020 2074 7164 6d20 2020 2020 2020       tqdm       
-000297c0: 207c 2020 2034 2e36 352e 3020 207c 2020   |   4.65.0  |  
-000297d0: 2020 2020 2020 2020 2020 2020 4d49 5420              MIT 
-000297e0: 4c69 6365 6e73 6520 2020 2020 2020 2020  License         
-000297f0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-00029800: 2020 2020 2055 4e4b 4e4f 574e 2020 2020       UNKNOWN    
-00029810: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00029820: 2020 2020 2020 2020 2020 2020 2020 6874                ht
-00029830: 7470 733a 2f2f 7471 646d 2e67 6974 6875  tps://tqdm.githu
-00029840: 622e 696f 2020 2020 2020 2020 2020 2020  b.io            
-00029850: 2020 2020 207c 0a7c 2020 2020 2020 2020       |.|        
-00029860: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00029870: 2020 2020 2020 2020 7c20 204d 6f7a 696c          |  Mozil
-00029880: 6c61 2050 7562 6c69 6320 4c69 6365 6e73  la Public Licens
-00029890: 6520 322e 3020 284d 504c 2032 2e30 2920  e 2.0 (MPL 2.0) 
-000298a0: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-000298b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000298c0: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-000298d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000298e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000298f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029900: 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  |.+-------------
-00029910: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00029920: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ---+------------
-00029930: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029940: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d  -----------+----
-00029950: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029970: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00029980: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029990: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000299a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020  -----------+.|  
-000299b0: 2020 2020 7572 6c6c 6962 3320 2020 2020      urllib3     
-000299c0: 2020 7c20 2031 2e32 362e 3135 2020 7c20    |  1.26.15  | 
-000299d0: 2020 2020 2020 2020 2020 2020 204d 4954               MIT
-000299e0: 204c 6963 656e 7365 2020 2020 2020 2020   License        
-000299f0: 2020 2020 2020 7c20 2020 2020 2020 2020        |         
-00029a00: 2020 2041 6e64 7265 7920 5065 7472 6f76     Andrey Petrov
-00029a10: 2020 2020 2020 2020 2020 2020 207c 2020               |  
-00029a20: 2020 2020 2020 2020 2020 6874 7470 733a            https:
-00029a30: 2f2f 7572 6c6c 6962 332e 7265 6164 7468  //urllib3.readth
-00029a40: 6564 6f63 732e 696f 2f20 2020 2020 2020  edocs.io/       
-00029a50: 2020 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d        |.+-------
-00029a60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d  -------------+--
-00029a70: 2d2d 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d  ---------+------
-00029a80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029a90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029aa0: 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  -+--------------
-00029ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029ac0: 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d  --------+-------
-00029ad0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029ae0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029af0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029b00: 2d2b 0a7c 2020 2020 2020 7763 7769 6474  -+.|      wcwidt
-00029b10: 6820 2020 2020 2020 7c20 2020 302e 322e  h       |   0.2.
-00029b20: 3620 2020 7c20 2020 2020 2020 2020 2020  6   |           
-00029b30: 2020 204d 4954 204c 6963 656e 7365 2020     MIT License  
-00029b40: 2020 2020 2020 2020 2020 2020 7c20 2020              |   
-00029b50: 2020 2020 2020 2020 2020 204a 6566 6620             Jeff 
-00029b60: 5175 6173 7420 2020 2020 2020 2020 2020  Quast           
-00029b70: 2020 207c 2020 2020 2020 2020 2020 2068     |           h
-00029b80: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00029b90: 6d2f 6a71 7561 7374 2f77 6377 6964 7468  m/jquast/wcwidth
-00029ba0: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
-00029bb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029bc0: 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b  ---+-----------+
-00029bd0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029be0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029bf0: 2d2d 2d2d 2d2d 2d2b 2d2d 2d2d 2d2d 2d2d  -------+--------
-00029c00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029c10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d  --------------+-
-00029c20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029c30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029c40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029c50: 2d2d 2d2d 2d2d 2d2b 0a0a 5468 6972 6420  -------+..Third 
-00029c60: 7061 7274 7920 6c69 6272 6172 6965 7320  party libraries 
-00029c70: 6d6f 6469 6669 6564 2061 6e64 2069 6e63  modified and inc
-00029c80: 6c75 6465 6420 696e 2062 3220 6f72 2062  luded in b2 or b
-00029c90: 3273 646b 3a0a 0a72 6571 7565 7374 730a  2sdk:..requests.
-00029ca0: 496e 636c 7564 6564 2069 6e20 6120 7265  Included in a re
-00029cb0: 7669 7365 6420 666f 726d 0a46 696c 6573  vised form.Files
-00029cc0: 2069 6e63 6c75 6465 6420 666f 7220 6c65   included for le
-00029cd0: 6761 6c20 636f 6d70 6c69 616e 6365 2072  gal compliance r
-00029ce0: 6561 736f 6e73 3a0a 2b2d 2d2d 2d2d 2d2d  easons:.+-------
-00029cf0: 2d2d 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----+-----------
-00029d00: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029d10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029d20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029d30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029d40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029d50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029d60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c  -------------+.|
-00029d70: 2046 696c 6520 6e61 6d65 207c 2020 2020   File name |    
-00029d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029db0: 2020 2020 436f 6e74 656e 7420 2020 2020      Content     
-00029dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029df0: 2020 2020 7c0a 2b2d 2d2d 2d2d 2d2d 2d2d      |.+---------
-00029e00: 2d2d 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  --+-------------
-00029e10: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029e20: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029e30: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029e40: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029e50: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029e60: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00029e70: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2b 0a7c 2020  -----------+.|  
-00029e80: 204e 4f54 4943 4520 207c 2020 2020 2020   NOTICE  |      
-00029e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ec0: 2020 5265 7175 6573 7473 2020 2020 2020    Requests      
-00029ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029f00: 2020 7c0a 7c20 2020 2020 2020 2020 2020    |.|           
-00029f10: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
-00029f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029f30: 2020 2020 2020 2020 2020 2020 2020 2043                 C
-00029f40: 6f70 7972 6967 6874 2032 3031 3920 4b65  opyright 2019 Ke
-00029f50: 6e6e 6574 6820 5265 6974 7a20 2020 2020  nneth Reitz     
-00029f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029f80: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
-00029f90: 2020 2020 2020 207c 2020 2020 2020 2020         |        
-00029fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00029ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a010: 7c0a 7c20 2020 2020 2020 2020 2020 7c20  |.|           | 
-0002a020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a040: 2020 2020 2020 2020 2020 2020 436f 7079              Copy
-0002a050: 7269 6768 7420 3230 3231 2042 6163 6b62  right 2021 Backb
-0002a060: 6c61 7a65 2049 6e63 2e20 2020 2020 2020  laze Inc.       
-0002a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a090: 2020 2020 2020 207c 0a7c 2020 2020 2020         |.|      
-0002a0a0: 2020 2020 207c 2020 2020 2020 2020 2020       |          
-0002a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a0d0: 4368 616e 6765 7320 6d61 6465 2074 6f20  Changes made to 
-0002a0e0: 7468 6520 6f72 6967 696e 616c 2073 6f75  the original sou
-0002a0f0: 7263 653a 2020 2020 2020 2020 2020 2020  rce:            
-0002a100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a110: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-0002a120: 7c20 2020 2020 2020 2020 2020 7c20 7265  |           | re
-0002a130: 7175 6573 7473 2e6d 6f64 656c 732e 5265  quests.models.Re
-0002a140: 7370 6f6e 7365 2e69 7465 725f 636f 6e74  sponse.iter_cont
-0002a150: 656e 7420 6861 7320 6265 656e 206f 7665  ent has been ove
-0002a160: 7272 6964 6465 6e20 746f 2070 6173 7320  rridden to pass 
-0002a170: 6064 6563 6f64 655f 636f 6e74 656e 743d  `decode_content=
-0002a180: 4661 6c73 6560 2061 7267 756d 656e 7420  False` argument 
-0002a190: 746f 2060 7365 6c66 2e72 6177 2e73 7472  to `self.raw.str
-0002a1a0: 6561 6d60 207c 0a7c 2020 2020 2020 2020  eam` |.|        
-0002a1b0: 2020 207c 2020 2020 2020 2020 2020 2020     |            
-0002a1c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a1d0: 696e 206f 7264 6572 2074 6f20 4e4f 5420  in order to NOT 
-0002a1e0: 6465 636f 6d70 7265 7373 2064 6174 6120  decompress data 
-0002a1f0: 6261 7365 6420 6f6e 2043 6f6e 7465 6e74  based on Content
-0002a200: 2d45 6e63 6f64 696e 6720 6865 6164 6572  -Encoding header
-0002a210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0002a220: 2020 2020 2020 2020 2020 2020 7c0a 2b2d              |.+-
-0002a230: 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d 2d2d  ----------+-----
-0002a240: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0002a250: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0002a260: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0002a270: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0002a280: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0002a290: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0002a2a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-0002a2b0: 2d2d 2d2b 0a0a 6232 206c 6963 656e 7365  ---+..b2 license
-0002a2c0: 3a0a 4261 636b 626c 617a 6520 7761 6e74  :.Backblaze want
-0002a2d0: 7320 6465 7665 6c6f 7065 7273 2061 6e64  s developers and
-0002a2e0: 206f 7267 616e 697a 6174 696f 6e20 746f   organization to
-0002a2f0: 2063 6f70 7920 616e 6420 7265 2d75 7365   copy and re-use
-0002a300: 206f 7572 0a63 6f64 6520 6578 616d 706c   our.code exampl
-0002a310: 6573 2c20 736f 2077 6520 6d61 6b65 2074  es, so we make t
-0002a320: 6865 2073 616d 706c 6573 2061 7661 696c  he samples avail
-0002a330: 6162 6c65 2062 7920 7365 7665 7261 6c20  able by several 
-0002a340: 6469 6666 6572 656e 740a 6c69 6365 6e73  different.licens
-0002a350: 6573 2e20 204f 6e65 206f 7074 696f 6e20  es.  One option 
-0002a360: 6973 2074 6865 204d 4954 206c 6963 656e  is the MIT licen
-0002a370: 7365 2028 6265 6c6f 7729 2e20 204f 7468  se (below).  Oth
-0002a380: 6572 206f 7074 696f 6e73 2061 7265 0a61  er options are.a
-0002a390: 7661 696c 6162 6c65 2068 6572 653a 0a0a  vailable here:..
-0002a3a0: 2020 2020 6874 7470 733a 2f2f 7777 772e      https://www.
-0002a3b0: 6261 636b 626c 617a 652e 636f 6d2f 7573  backblaze.com/us
-0002a3c0: 696e 675f 6232 5f63 6f64 652e 6874 6d6c  ing_b2_code.html
-0002a3d0: 0a0a 0a54 6865 204d 4954 204c 6963 656e  ...The MIT Licen
-0002a3e0: 7365 2028 4d49 5429 0a0a 436f 7079 7269  se (MIT)..Copyri
-0002a3f0: 6768 7420 2863 2920 3230 3135 2042 6163  ght (c) 2015 Bac
-0002a400: 6b62 6c61 7a65 0a0a 5065 726d 6973 7369  kblaze..Permissi
-0002a410: 6f6e 2069 7320 6865 7265 6279 2067 7261  on is hereby gra
-0002a420: 6e74 6564 2c20 6672 6565 206f 6620 6368  nted, free of ch
-0002a430: 6172 6765 2c20 746f 2061 6e79 2070 6572  arge, to any per
-0002a440: 736f 6e20 6f62 7461 696e 696e 6720 6120  son obtaining a 
-0002a450: 636f 7079 0a6f 6620 7468 6973 2073 6f66  copy.of this sof
-0002a460: 7477 6172 6520 616e 6420 6173 736f 6369  tware and associ
-0002a470: 6174 6564 2064 6f63 756d 656e 7461 7469  ated documentati
-0002a480: 6f6e 2066 696c 6573 2028 7468 6520 2253  on files (the "S
-0002a490: 6f66 7477 6172 6522 292c 2074 6f20 6465  oftware"), to de
-0002a4a0: 616c 0a69 6e20 7468 6520 536f 6674 7761  al.in the Softwa
-0002a4b0: 7265 2077 6974 686f 7574 2072 6573 7472  re without restr
-0002a4c0: 6963 7469 6f6e 2c20 696e 636c 7564 696e  iction, includin
-0002a4d0: 6720 7769 7468 6f75 7420 6c69 6d69 7461  g without limita
-0002a4e0: 7469 6f6e 2074 6865 2072 6967 6874 730a  tion the rights.
-0002a4f0: 746f 2075 7365 2c20 636f 7079 2c20 6d6f  to use, copy, mo
-0002a500: 6469 6679 2c20 6d65 7267 652c 2070 7562  dify, merge, pub
-0002a510: 6c69 7368 2c20 6469 7374 7269 6275 7465  lish, distribute
-0002a520: 2c20 7375 626c 6963 656e 7365 2c20 616e  , sublicense, an
-0002a530: 642f 6f72 2073 656c 6c0a 636f 7069 6573  d/or sell.copies
-0002a540: 206f 6620 7468 6520 536f 6674 7761 7265   of the Software
-0002a550: 2c20 616e 6420 746f 2070 6572 6d69 7420  , and to permit 
-0002a560: 7065 7273 6f6e 7320 746f 2077 686f 6d20  persons to whom 
-0002a570: 7468 6520 536f 6674 7761 7265 2069 730a  the Software is.
-0002a580: 6675 726e 6973 6865 6420 746f 2064 6f20  furnished to do 
-0002a590: 736f 2c20 7375 626a 6563 7420 746f 2074  so, subject to t
-0002a5a0: 6865 2066 6f6c 6c6f 7769 6e67 2063 6f6e  he following con
-0002a5b0: 6469 7469 6f6e 733a 0a0a 5468 6520 6162  ditions:..The ab
-0002a5c0: 6f76 6520 636f 7079 7269 6768 7420 6e6f  ove copyright no
-0002a5d0: 7469 6365 2061 6e64 2074 6869 7320 7065  tice and this pe
-0002a5e0: 726d 6973 7369 6f6e 206e 6f74 6963 6520  rmission notice 
-0002a5f0: 7368 616c 6c20 6265 2069 6e63 6c75 6465  shall be include
-0002a600: 6420 696e 2061 6c6c 0a63 6f70 6965 7320  d in all.copies 
-0002a610: 6f72 2073 7562 7374 616e 7469 616c 2070  or substantial p
-0002a620: 6f72 7469 6f6e 7320 6f66 2074 6865 2053  ortions of the S
-0002a630: 6f66 7477 6172 652e 0a0a 5448 4520 534f  oftware...THE SO
-0002a640: 4654 5741 5245 2049 5320 5052 4f56 4944  FTWARE IS PROVID
-0002a650: 4544 2022 4153 2049 5322 2c20 5749 5448  ED "AS IS", WITH
-0002a660: 4f55 5420 5741 5252 414e 5459 204f 4620  OUT WARRANTY OF 
-0002a670: 414e 5920 4b49 4e44 2c20 4558 5052 4553  ANY KIND, EXPRES
-0002a680: 5320 4f52 0a49 4d50 4c49 4544 2c20 494e  S OR.IMPLIED, IN
-0002a690: 434c 5544 494e 4720 4255 5420 4e4f 5420  CLUDING BUT NOT 
-0002a6a0: 4c49 4d49 5445 4420 544f 2054 4845 2057  LIMITED TO THE W
-0002a6b0: 4152 5241 4e54 4945 5320 4f46 204d 4552  ARRANTIES OF MER
-0002a6c0: 4348 414e 5441 4249 4c49 5459 2c0a 4649  CHANTABILITY,.FI
-0002a6d0: 544e 4553 5320 464f 5220 4120 5041 5254  TNESS FOR A PART
-0002a6e0: 4943 554c 4152 2050 5552 504f 5345 2041  ICULAR PURPOSE A
-0002a6f0: 4e44 204e 4f4e 494e 4652 494e 4745 4d45  ND NONINFRINGEME
-0002a700: 4e54 2e20 494e 204e 4f20 4556 454e 5420  NT. IN NO EVENT 
-0002a710: 5348 414c 4c20 5448 450a 4155 5448 4f52  SHALL THE.AUTHOR
-0002a720: 5320 4f52 2043 4f50 5952 4947 4854 2048  S OR COPYRIGHT H
-0002a730: 4f4c 4445 5253 2042 4520 4c49 4142 4c45  OLDERS BE LIABLE
-0002a740: 2046 4f52 2041 4e59 2043 4c41 494d 2c20   FOR ANY CLAIM, 
-0002a750: 4441 4d41 4745 5320 4f52 204f 5448 4552  DAMAGES OR OTHER
-0002a760: 0a4c 4941 4249 4c49 5459 2c20 5748 4554  .LIABILITY, WHET
-0002a770: 4845 5220 494e 2041 4e20 4143 5449 4f4e  HER IN AN ACTION
-0002a780: 204f 4620 434f 4e54 5241 4354 2c20 544f   OF CONTRACT, TO
-0002a790: 5254 204f 5220 4f54 4845 5257 4953 452c  RT OR OTHERWISE,
-0002a7a0: 2041 5249 5349 4e47 2046 524f 4d2c 0a4f   ARISING FROM,.O
-0002a7b0: 5554 204f 4620 4f52 2049 4e20 434f 4e4e  UT OF OR IN CONN
-0002a7c0: 4543 5449 4f4e 2057 4954 4820 5448 4520  ECTION WITH THE 
-0002a7d0: 534f 4654 5741 5245 204f 5220 5448 4520  SOFTWARE OR THE 
-0002a7e0: 5553 4520 4f52 204f 5448 4552 2044 4541  USE OR OTHER DEA
-0002a7f0: 4c49 4e47 5320 494e 2054 4845 0a53 4f46  LINGS IN THE.SOF
-0002a800: 5457 4152 452e 0a0a                      TWARE...
+00025f40: 2020 2020 2020 2020 207c 0a7c 2020 2020           |.|    
+00025f50: 2020 2020 2020 207c 2020 2020 2020 2020         |        
+00025f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025f80: 2020 4368 616e 6765 7320 6d61 6465 2074    Changes made t
+00025f90: 6f20 7468 6520 6f72 6967 696e 616c 2073  o the original s
+00025fa0: 6f75 7263 653a 2020 2020 2020 2020 2020  ource:          
+00025fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00025fd0: 7c0a 7c20 2020 2020 2020 2020 2020 7c20  |.|           | 
+00025fe0: 7265 7175 6573 7473 2e6d 6f64 656c 732e  requests.models.
+00025ff0: 5265 7370 6f6e 7365 2e69 7465 725f 636f  Response.iter_co
+00026000: 6e74 656e 7420 6861 7320 6265 656e 206f  ntent has been o
+00026010: 7665 7272 6964 6465 6e20 746f 2070 6173  verridden to pas
+00026020: 7320 6064 6563 6f64 655f 636f 6e74 656e  s `decode_conten
+00026030: 743d 4661 6c73 6560 2061 7267 756d 656e  t=False` argumen
+00026040: 7420 746f 2060 7365 6c66 2e72 6177 2e73  t to `self.raw.s
+00026050: 7472 6561 6d60 207c 0a7c 2020 2020 2020  tream` |.|      
+00026060: 2020 2020 207c 2020 2020 2020 2020 2020       |          
+00026070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026080: 2020 696e 206f 7264 6572 2074 6f20 4e4f    in order to NO
+00026090: 5420 6465 636f 6d70 7265 7373 2064 6174  T decompress dat
+000260a0: 6120 6261 7365 6420 6f6e 2043 6f6e 7465  a based on Conte
+000260b0: 6e74 2d45 6e63 6f64 696e 6720 6865 6164  nt-Encoding head
+000260c0: 6572 2020 2020 2020 2020 2020 2020 2020  er              
+000260d0: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
+000260e0: 2b2d 2d2d 2d2d 2d2d 2d2d 2d2d 2b2d 2d2d  +-----------+---
+000260f0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00026100: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00026110: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00026120: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00026130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00026140: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00026150: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00026160: 2d2d 2d2d 2d2b 0a0a 6232 206c 6963 656e  -----+..b2 licen
+00026170: 7365 3a0a 4261 636b 626c 617a 6520 7761  se:.Backblaze wa
+00026180: 6e74 7320 6465 7665 6c6f 7065 7273 2061  nts developers a
+00026190: 6e64 206f 7267 616e 697a 6174 696f 6e20  nd organization 
+000261a0: 746f 2063 6f70 7920 616e 6420 7265 2d75  to copy and re-u
+000261b0: 7365 206f 7572 0a63 6f64 6520 6578 616d  se our.code exam
+000261c0: 706c 6573 2c20 736f 2077 6520 6d61 6b65  ples, so we make
+000261d0: 2074 6865 2073 616d 706c 6573 2061 7661   the samples ava
+000261e0: 696c 6162 6c65 2062 7920 7365 7665 7261  ilable by severa
+000261f0: 6c20 6469 6666 6572 656e 740a 6c69 6365  l different.lice
+00026200: 6e73 6573 2e20 204f 6e65 206f 7074 696f  nses.  One optio
+00026210: 6e20 6973 2074 6865 204d 4954 206c 6963  n is the MIT lic
+00026220: 656e 7365 2028 6265 6c6f 7729 2e20 204f  ense (below).  O
+00026230: 7468 6572 206f 7074 696f 6e73 2061 7265  ther options are
+00026240: 0a61 7661 696c 6162 6c65 2068 6572 653a  .available here:
+00026250: 0a0a 2020 2020 6874 7470 733a 2f2f 7777  ..    https://ww
+00026260: 772e 6261 636b 626c 617a 652e 636f 6d2f  w.backblaze.com/
+00026270: 7573 696e 675f 6232 5f63 6f64 652e 6874  using_b2_code.ht
+00026280: 6d6c 0a0a 0a54 6865 204d 4954 204c 6963  ml...The MIT Lic
+00026290: 656e 7365 2028 4d49 5429 0a0a 436f 7079  ense (MIT)..Copy
+000262a0: 7269 6768 7420 2863 2920 3230 3135 2042  right (c) 2015 B
+000262b0: 6163 6b62 6c61 7a65 0a0a 5065 726d 6973  ackblaze..Permis
+000262c0: 7369 6f6e 2069 7320 6865 7265 6279 2067  sion is hereby g
+000262d0: 7261 6e74 6564 2c20 6672 6565 206f 6620  ranted, free of 
+000262e0: 6368 6172 6765 2c20 746f 2061 6e79 2070  charge, to any p
+000262f0: 6572 736f 6e20 6f62 7461 696e 696e 6720  erson obtaining 
+00026300: 6120 636f 7079 0a6f 6620 7468 6973 2073  a copy.of this s
+00026310: 6f66 7477 6172 6520 616e 6420 6173 736f  oftware and asso
+00026320: 6369 6174 6564 2064 6f63 756d 656e 7461  ciated documenta
+00026330: 7469 6f6e 2066 696c 6573 2028 7468 6520  tion files (the 
+00026340: 2253 6f66 7477 6172 6522 292c 2074 6f20  "Software"), to 
+00026350: 6465 616c 0a69 6e20 7468 6520 536f 6674  deal.in the Soft
+00026360: 7761 7265 2077 6974 686f 7574 2072 6573  ware without res
+00026370: 7472 6963 7469 6f6e 2c20 696e 636c 7564  triction, includ
+00026380: 696e 6720 7769 7468 6f75 7420 6c69 6d69  ing without limi
+00026390: 7461 7469 6f6e 2074 6865 2072 6967 6874  tation the right
+000263a0: 730a 746f 2075 7365 2c20 636f 7079 2c20  s.to use, copy, 
+000263b0: 6d6f 6469 6679 2c20 6d65 7267 652c 2070  modify, merge, p
+000263c0: 7562 6c69 7368 2c20 6469 7374 7269 6275  ublish, distribu
+000263d0: 7465 2c20 7375 626c 6963 656e 7365 2c20  te, sublicense, 
+000263e0: 616e 642f 6f72 2073 656c 6c0a 636f 7069  and/or sell.copi
+000263f0: 6573 206f 6620 7468 6520 536f 6674 7761  es of the Softwa
+00026400: 7265 2c20 616e 6420 746f 2070 6572 6d69  re, and to permi
+00026410: 7420 7065 7273 6f6e 7320 746f 2077 686f  t persons to who
+00026420: 6d20 7468 6520 536f 6674 7761 7265 2069  m the Software i
+00026430: 730a 6675 726e 6973 6865 6420 746f 2064  s.furnished to d
+00026440: 6f20 736f 2c20 7375 626a 6563 7420 746f  o so, subject to
+00026450: 2074 6865 2066 6f6c 6c6f 7769 6e67 2063   the following c
+00026460: 6f6e 6469 7469 6f6e 733a 0a0a 5468 6520  onditions:..The 
+00026470: 6162 6f76 6520 636f 7079 7269 6768 7420  above copyright 
+00026480: 6e6f 7469 6365 2061 6e64 2074 6869 7320  notice and this 
+00026490: 7065 726d 6973 7369 6f6e 206e 6f74 6963  permission notic
+000264a0: 6520 7368 616c 6c20 6265 2069 6e63 6c75  e shall be inclu
+000264b0: 6465 6420 696e 2061 6c6c 0a63 6f70 6965  ded in all.copie
+000264c0: 7320 6f72 2073 7562 7374 616e 7469 616c  s or substantial
+000264d0: 2070 6f72 7469 6f6e 7320 6f66 2074 6865   portions of the
+000264e0: 2053 6f66 7477 6172 652e 0a0a 5448 4520   Software...THE 
+000264f0: 534f 4654 5741 5245 2049 5320 5052 4f56  SOFTWARE IS PROV
+00026500: 4944 4544 2022 4153 2049 5322 2c20 5749  IDED "AS IS", WI
+00026510: 5448 4f55 5420 5741 5252 414e 5459 204f  THOUT WARRANTY O
+00026520: 4620 414e 5920 4b49 4e44 2c20 4558 5052  F ANY KIND, EXPR
+00026530: 4553 5320 4f52 0a49 4d50 4c49 4544 2c20  ESS OR.IMPLIED, 
+00026540: 494e 434c 5544 494e 4720 4255 5420 4e4f  INCLUDING BUT NO
+00026550: 5420 4c49 4d49 5445 4420 544f 2054 4845  T LIMITED TO THE
+00026560: 2057 4152 5241 4e54 4945 5320 4f46 204d   WARRANTIES OF M
+00026570: 4552 4348 414e 5441 4249 4c49 5459 2c0a  ERCHANTABILITY,.
+00026580: 4649 544e 4553 5320 464f 5220 4120 5041  FITNESS FOR A PA
+00026590: 5254 4943 554c 4152 2050 5552 504f 5345  RTICULAR PURPOSE
+000265a0: 2041 4e44 204e 4f4e 494e 4652 494e 4745   AND NONINFRINGE
+000265b0: 4d45 4e54 2e20 494e 204e 4f20 4556 454e  MENT. IN NO EVEN
+000265c0: 5420 5348 414c 4c20 5448 450a 4155 5448  T SHALL THE.AUTH
+000265d0: 4f52 5320 4f52 2043 4f50 5952 4947 4854  ORS OR COPYRIGHT
+000265e0: 2048 4f4c 4445 5253 2042 4520 4c49 4142   HOLDERS BE LIAB
+000265f0: 4c45 2046 4f52 2041 4e59 2043 4c41 494d  LE FOR ANY CLAIM
+00026600: 2c20 4441 4d41 4745 5320 4f52 204f 5448  , DAMAGES OR OTH
+00026610: 4552 0a4c 4941 4249 4c49 5459 2c20 5748  ER.LIABILITY, WH
+00026620: 4554 4845 5220 494e 2041 4e20 4143 5449  ETHER IN AN ACTI
+00026630: 4f4e 204f 4620 434f 4e54 5241 4354 2c20  ON OF CONTRACT, 
+00026640: 544f 5254 204f 5220 4f54 4845 5257 4953  TORT OR OTHERWIS
+00026650: 452c 2041 5249 5349 4e47 2046 524f 4d2c  E, ARISING FROM,
+00026660: 0a4f 5554 204f 4620 4f52 2049 4e20 434f  .OUT OF OR IN CO
+00026670: 4e4e 4543 5449 4f4e 2057 4954 4820 5448  NNECTION WITH TH
+00026680: 4520 534f 4654 5741 5245 204f 5220 5448  E SOFTWARE OR TH
+00026690: 4520 5553 4520 4f52 204f 5448 4552 2044  E USE OR OTHER D
+000266a0: 4541 4c49 4e47 5320 494e 2054 4845 0a53  EALINGS IN THE.S
+000266b0: 4f46 5457 4152 452e 0a0a                 OFTWARE...
```

